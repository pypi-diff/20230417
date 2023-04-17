# Comparing `tmp/nx5d-0.3.0.tar.gz` & `tmp/nx5d-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.0.tar", last modified: Wed Apr 12 13:16:02 2023, max compression
+gzip compressed data, was "nx5d-0.3.1.tar", last modified: Mon Apr 17 15:48:04 2023, max compression
```

## Comparing `nx5d-0.3.0.tar` & `nx5d-0.3.1.tar`

### file list

```diff
@@ -1,167 +1,172 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.453487 nx5d-0.3.0/
--rw-r--r--   0 florin    (1000) florin    (1000)       53 2023-03-14 11:33:48.000000 nx5d-0.3.0/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.0/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.0/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-12 13:16:02.453487 nx5d-0.3.0/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.0/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.435487 nx5d-0.3.0/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.436488 nx5d-0.3.0/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.0/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.0/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27046 2023-03-27 10:25:44.000000 nx5d-0.3.0/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.0/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2482 2023-03-27 10:54:07.000000 nx5d-0.3.0/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.0/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.0/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.0/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.0/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.0/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.437487 nx5d-0.3.0/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.0/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.438487 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.438487 nx5d-0.3.0/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.0/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.438487 nx5d-0.3.0/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.0/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.0/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.0/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.0/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.0/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      900 2023-04-12 13:16:02.453487 nx5d-0.3.0/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.433488 nx5d-0.3.0/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.439488 nx5d-0.3.0/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.440487 nx5d-0.3.0/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.0/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5639 2023-04-12 12:32:44.000000 nx5d-0.3.0/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    23212 2023-04-11 11:34:50.000000 nx5d-0.3.0/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    32873 2023-04-12 10:02:22.000000 nx5d-0.3.0/src/nx5d/scan.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.442488 nx5d-0.3.0/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)    13272 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)     9022 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/signal.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.0/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.440487 nx5d-0.3.0/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     7482 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      113 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-12 13:16:02.000000 nx5d-0.3.0/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.442488 nx5d-0.3.0/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     1269 2023-04-12 11:45:47.000000 nx5d-0.3.0/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/runlog_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.433488 nx5d-0.3.0/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.447487 nx5d-0.3.0/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.433488 nx5d-0.3.0/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.447487 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.434487 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.448488 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-12 13:16:02.453487 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     1524 2023-03-24 22:02:23.000000 nx5d-0.3.0/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/xrd_data_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.0/tests/xrd_kmc3_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.474620 nx5d-0.3.1/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.1/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.1/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.1/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-17 15:48:04.474620 nx5d-0.3.1/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.1/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.454620 nx5d-0.3.1/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.456620 nx5d-0.3.1/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.1/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.1/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27046 2023-03-27 10:25:44.000000 nx5d-0.3.1/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.1/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2482 2023-03-27 10:54:07.000000 nx5d-0.3.1/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.1/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.1/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.1/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.1/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.1/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.456620 nx5d-0.3.1/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.1/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.457620 nx5d-0.3.1/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.1/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.1/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.1/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.1/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.1/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      900 2023-04-17 15:48:04.475620 nx5d-0.3.1/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.452620 nx5d-0.3.1/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.458620 nx5d-0.3.1/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.459620 nx5d-0.3.1/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.1/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    10778 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.1/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    13662 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.461620 nx5d-0.3.1/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    13272 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    18117 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1223 2023-04-17 15:45:54.000000 nx5d-0.3.1/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.1/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.459620 nx5d-0.3.1/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3449 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     7583 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      113 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-04-17 15:48:04.000000 nx5d-0.3.1/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.462620 nx5d-0.3.1/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.1/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.1/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/runlog_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.466620 nx5d-0.3.1/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.466620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.453620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.468620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-04-17 15:48:04.474620 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.1/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/xrd_data_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      915 2023-03-14 11:33:48.000000 nx5d-0.3.1/tests/xrd_kmc3_test.py
```

### Comparing `nx5d-0.3.0/COPYING.md` & `nx5d-0.3.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/PKG-INFO` & `nx5d-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.0
+Version: 0.3.1
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.0/README.md` & `nx5d-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/concepts.md` & `nx5d-0.3.1/doc/mkdocs/concepts.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/frame.svg` & `nx5d-0.3.1/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/index.md` & `nx5d-0.3.1/doc/mkdocs/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/license.md` & `nx5d-0.3.1/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/module-nx.md` & `nx5d-0.3.1/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/scan.svg` & `nx5d-0.3.1/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/streak1.svg` & `nx5d-0.3.1/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/streak2.svg` & `nx5d-0.3.1/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.1/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.1/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.1/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/doc/mkdocs.yml` & `nx5d-0.3.1/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/scratch.org` & `nx5d-0.3.1/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/setup.cfg` & `nx5d-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/edf.py` & `nx5d-0.3.1/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/h5like/pypod.py` & `nx5d-0.3.1/src/nx5d/h5like/pypod.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,16 +102,17 @@
         except KeyError as e:
             # dataset does not yet exist -- we're creating it.
             logging.debug("Creating dataset '%s' in '%s'" % (path, h5like.name))
 
             # If the user didn't specify anything else, we make the dataset
             # infinitely extensible in the 1st dimension.
             max_shape = tuple([None] + [i for i in data.shape[1:]])
-            dset_args.setdefault('maxshape', max_shape)
-            h5like.create_dataset(path, data=data, **dset_args)
+            create_args = dset_args.copy()
+            create_args.setdefault('maxshape', max_shape)
+            h5like.create_dataset(path, data=data, **create_args)
 
     else:
         try:
             group = h5like[path]
         except KeyError:
             # need to create group first
             split = path.rsplit('/')
```

### Comparing `nx5d-0.3.0/src/nx5d/h5like/xfel.py` & `nx5d-0.3.1/src/nx5d/h5like/xfel.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from numpy import array as np_array
 from itertools import product as itr_product
 
 from numpy import array as np_array
 
 from xarray import DataArray, Dataset, concat
 
+import extra_data.components as ex_comp
+
 import logging
 
 '''
 Reading XFEL Data
 =================
 
 This module implements analysis and transformation routines which enable
@@ -48,27 +50,38 @@
     different sequences from different acquisition devices don't
     necessarily align, which is a requirement for our frames and
     streaks.
 
   - **train**: this is the usefully organized sub-unit of data acquisition;
     it holds all the data points (a.k.a. *frames*, in nx5d lingo) that
     come with a pulse train. (A pulse train is one "shot" of the XFEL, taking
-    place within a a significant fraction of a second, and containing
+    place within a significant fraction of a second, and containing
     up to several hundreds of pulses at once.)
 
     Each of the instruments saves their data according to the current
     *train ID*, which is unique. Not every instrument does, however, necessarily
     save any data for each train, and those that do, don't necessarily save
     only a single data point; in fact, many save several, e.g. one data point
     for each pulse. The number of data points one specific instrument
     saves may also vary from one train to the next.
 
     As such, trains do not neatly align with our initial idea of *frames*,
     but don't outright contradict it.
 
+  - Finally, the smallest data item in XFEL data is a **pulse**: this
+    corresponds to exactly one X-ray event. This is what in XFEL lingo
+    is a "frame". It is also possible to map one XFEL "frame" on an
+    nx5d frame, conceptually.
+
+  - There are "regular" detectors and devices, and there "multi-module"
+    detectors. The latter are made up of several modules which show up
+    as individual devices in the data (e.g. when building a "selection"),
+    but mostly are being combined to actually yield a more useful
+    representation (e.g. an X-ray diffraction image we know as a "frame"
+    from the nx5d data model).
 
 Data Adapter Strategy
 ---------------------
 
 Analyzing XFEL data is a two-step process:
 
   1. Data needs to be extracted from the pecular XFEL storage
@@ -102,29 +115,44 @@
 one datapoint per pulse train (but on a different pulse than another),
 others collect several at different times, and yet others don't collect
 any data at all.
 
 In the first phase -- extracting and preparing -- we make it the
 user's (or: higher API level's) responsibility to address only those
 devices that have a similar storage scheme, e.g. the 16 modules
-that make up one particular detector. To simplify and encourage
-"correct behavior", addressing scheme will have syntactic sugar
-to address a whole class of devices at once (e.g. selecting
-`detector="AGIPD1M-1"` instead of `("MID_DET_AGIPD1M-1/DET/*CH0:xtdf")`),
-in addition to regular, completely free key addressing.
-
-This in turn also means that we are offering a list of special XFEL
-devices, detectors in particular, with their naming scheme and data
-processing particualrities. Beyond addressing, this is important for
-a variety of reasons: XFEL detectors are not single pieces of equipment,
-they are (sometimes?) made up of distinct components -- e.g. up to 16
-individual chips. These have a non-trivial geometry and spatial relation
-to one another, and need supplementary data (and API elements from
-EXtra-data) in order to assemle a full, "regular" x-ray diffraction
-pattern picture.
+that make up one particular detector. The `ExdatH5` class below
+uses `extra_data` API elements to automatically detect multi-module
+data and treat it accordingly.
+
+Aggregtion of module data into X-ray images is done by `DetectorTiler`.
+It makes a few reasonable assumptions while trying to remain as
+flexible as possible. If it doesn't offer what you need, feel free
+to subclass or build your own after its example ;-)
+
+Relation to "Scan, Streak, Frame"
+---------------------------------
+
+There are actually two good candidates for a "frame" when processing
+XFEL data:
+
+ - data of a "pulse", i.e. of one single X-ray flash; there are typically
+   somewhere around 10^6 pulses in a run;
+
+ - data of a "train", i.e. of an X-ray "shot" consisting of several pulses;
+   there are typically around 10^3 pulses in a "run".
+
+The `ExdatH5` class below doesn't discriminate between the two. It will
+push either dimension to the front of the shape -- preferrably the pulse,
+if it is available.
+
+Streaking is done with the usual nx5d suspects from `nx5d.streaks`. In
+addition, there are specialized streakers for XFEL specific information
+(e.g. to streak from train to train, or to get specific train IDs
+as streaks).
+
 '''
 
 class ExdatLazyDataset(ch5.LazyLoadableDataset):
     ''' Node to lazily load `extra_data.KeyData` datasets.
     '''
     def __init__(self, keydata, name, parent=None, attrs=None, array_like='dask_array'):
         super().__init__(name, parent, attrs)
@@ -204,27 +232,96 @@
 
     def __len__(self):
         ''' Same problem as __getitem__(): overzealous superclass discards data if it's not numpy.
         '''
         return self._get_data().__len__() \
             if hasattr(self._get_data(), "__len__") \
                else super().__len__()
+
+
+class ExdatDataset(ch5.LazyLoadableDataset):
+    '''Dataset class for dask arrays.
+
+    Dask arrays need special treatment because they're not "regular" numpy arrays,
+    so some members (`__len__`, `size`, `shape`, `__getitem__` need to be overwritten
+    with respect to Silx default behavior.
+
+    See `ExdatLazyDataset.__getitem__()` for more details.
+    '''
+    def __init__(self, name, modobj, datakey, parent=None, attrs=None):
+        super().__init__(name, parent, attrs)
+        self._modobj = modobj
+        self._datakey = datakey
+
+    def _create_data(self):
+
+        data = self._modobj.get_dask_array(self._datakey)
+            
+        # To stay compatible with nx5d data models, we need the 'train_pulse' dimension
+        # first. Some data keys don't have that. What we do to those datasets us up
+        # to us; could leave them alone, but we try to get the 'trainId' dimension
+        # (the next best thing) up in front.
+        if 'train_pulse' in data.dims:
+            dat2 = data.transpose('train_pulse', ...)
+        elif 'trainId' in data.dims:
+            dat2 = data.transpose('trainId', ...)
+        else:
+            dat2 = data
+            
+        #logging.debug("  Reshape: dimensions %r, shape %r, name '%s'" % (data.dims, data.shape, key))
+        
+        return dat2
+
     
+    def __getitem__(self, item):
+        ''' Overriding __getitem__() from silx's LazyLoadableDataset.
+        '''
+        if hasattr(self._get_data(), "__getitem__"):
+            return self._get_data().__getitem__(item)
+        else:
+            return super().__getitem__(item)
+
+
+    @property
+    def shape(self):
+        ''' Same problem as __getitem__(): overzealous superclass discards data if it's not numpy.
+        '''
+        return self._get_data().shape \
+            if hasattr(self._get_data(), "shape") \
+               else super().shape
+
+    @property
+    def size(self):
+        ''' Same problem as __getitem__(): overzealous superclass discards data if it's not numpy.
+        '''
+        return self._get_data().size \
+            if hasattr(self._get_data(), "size") \
+               else super().size
+
+
+    def __len__(self):
+        ''' Same problem as __getitem__(): overzealous superclass discards data if it's not numpy.
+        '''
+        return self._get_data().__len__() \
+            if hasattr(self._get_data(), "__len__") \
+               else super().__len__()
         
 
 class ExdatSourcesGroup(ch5.Group):
     '''Mock HDF5 node for a subset of `extra_data.DataCollection` keys.
     '''
     def __init__(self, name, parent, selection, array_like='auto'):
         super().__init__(name=name, parent=parent)
         self.sel = selection
 
+        logging.debug("Selection group node at: %s" % (self.name,))
+
         for src in self.sel.all_sources:
             snode = self._ensure_group(self, src)
-            logging.debug("Have node: %s" % snode.name)
+            logging.debug("Group: %s" % snode.name)
             
             for key in self.sel.keys_for_source(src):
                 kdata = self.sel[src,key]
 
                 if array_like == 'auto':
                     numpts = np_array(kdata.shape).prod()
                     array_like = 'dask_array' if numpts > 1e6 else 'ndarray'
@@ -247,14 +344,32 @@
         them = parts[1:] if len(parts)>1 else None
         
         if me not in parent:
             parent.add_node(ch5.Group(name=me, parent=parent))
 
         return parent[me] if them is None \
             else self._ensure_group(parent[me], them)
+
+
+class ExdatMultimodalDetector(ch5.Group):
+    ''' Mock HDF5 group for a multimodal detector.
+
+    The specialty here is that we don't get the data directly via a `DataCollection`,
+    we're using one of the special `extra_data.components` designated to assembling
+    motor data.
+    '''
+    def __init__(self, name, parent, multimod):
+        super().__init__(name=name, parent=parent)
+        self.modobj = multimod
+
+        logging.debug("Multimodule detector: %s, at: %s" % (multimod.detector_name, self.name))
+        module_source = next(iter(multimod.data.all_sources))
+        for key in multimod.data.keys_for_source(module_source):
+            logging.debug("  Dataset: %s" % key)
+            self.add_node(ExdatDataset(name=key, modobj=multimod, datakey=key, parent=self))
         
         
 class ExdatH5(ch5.File):
     '''Generic class to offer HDF5-like access to a `DataCollection` object.
 
     This implementation is not necessarily fully h5py-API compatible. It contains
     just enough of a mock up to be able to work nicely with nx5d.scan.ScanReader.
@@ -274,30 +389,119 @@
               since it's considerably faster. However, "dask" will provide you
               with distribuited arrays that work across a large number of nodes,
               should you need it. The default "auto" will always try "numpy"
               first, and fall back to "dask" if that fails.
         '''
         super().__init__()
 
-        self.add_node(ExdatSourcesGroup(name="measurement", parent=self,
-                                        selection=dsel.select([
-                                            (k, '*') for k in dsel.all_sources
-                                        ]),
-                                        array_like=array_like))
+        self.original_dsel = dsel
+
+        for det_name,DetClass in ex_comp.identify_multimod_detectors(dsel):
+            logging.debug("Multimodal detector: %s" % det_name)
+            multimod = DetClass(dsel, detector_name=det_name)
+
+            self.__add_multimodule(multimod, "instrument/multimod", self, array_like)
+
+            # split away data sources which were already in 'multimod'
+            dsel = dsel.deselect([(m, '*') for m in multimod.source_to_modno])
+
+
+        self.nonmmod_dsel = dsel            
+        logging.debug("Following non-multimodal entries")
+        self.__add_selection(self.nonmmod_dsel, "instrument/selection", self, array_like)
         
         #self.add_node(ch5.Group(name="instrument", parent=self))
         #self['instrument'].add_node(ExdatGroup(name="positioners", parent=self['instrument'],
         #                                       selection=None))
-        
-        self.dsel = dsel
 
         # could split these in instrument_sources and control_sources.
         #self.datasets = {k:self.dsel.get_virtual_dataset(k) \
         #                 for k in self.datc.all_sources}
 
+
+    def __ensure_path(self, path, root, parent_only=False):
+        '''Makes sure that path and all its parent nodes exist as a `silx.io.commonh5.Group`.
+
+        Essentially this means that this function creates all path elements from
+        `path`, *except for the final one*, as a `silx.io.commonh5.Group`. The final
+        one is only created of `parent_only` is set to `False` (default), otherwise
+        it is omitted.
+        The reasoning is that the final element is likely to requrie something more
+        specialized, and will be created next.
+
+        Args:
+            path: The full HDF5 path, relative to `root`
+            root: The root node to whoch `path` relates
+            parent_only: If set to `True`, then the last path component
+              (i.e. the one after the last "/") will *not* be created.
+              Default is `False`.
+
+        Returns: A tuple ("name", parent), where "name" is the last node
+          component (yet to be created), and `parent` is an object reference to
+          what is supposed to become its parent Group node object.
+          If the last component has already been created, the corresponding
+          tuple item is set to `None`, and `parent` points instead to the
+          final node in the `path` list.
+        '''
+        
+        paths = path.split('/')
+        node = root
+        for p in (paths[:-1] if parent_only else paths):
+            try:
+                node = node[p]
+            except KeyError:
+                old_parent = node
+                node.add_node(ch5.Group(p, old_parent))
+                node = node[p]
+    
+            logging.debug("Have node: %r, as: %s (%s), parent %r" % \
+                          (node, node.name, p, node.parent))
+                
+        if parent_only:
+            return paths[-1], node
+        else:
+            return None, node
+
+
+    def __add_multimodule(self, modobj, path, root, array_like):
+        ''' Adds a multimodule detector at `path`, starting from root node `parent`.
+        '''
+
+        (moo, node) = self.__ensure_path(path, root)
+        logging.debug("Got multi-module parent: %r" % ((moo, node),))
+        
+        node.add_node(ExdatMultimodalDetector(modobj.detector_name, node, modobj))
+        
+
+    def __add_selection(self, dsel, path, parent, array_like):
+        ''' Adds all data soruces from `dsel` to a node at `path`.
+
+        The path elements from `path` are created as simple ch5.Group
+        if they don't exist (yet). Note that generally, the data source names
+        in `dsel` will contain slashes ("/"), making them somewhat similar
+        to HDF5 subpath names. `ExdatSourcesGroup`, used here within, will
+        take care of also creating those subpaths.
+
+        Args:
+            dsel: DataCollection / selection-like
+            path: string as HDF5-like path
+            parent: parent object in which to insert the top-level entry of `path`
+            array_like: "auto", "dask_array" or "ndarray". See `__init__()`.
+        '''
+
+        (child_name, parent_node) = self.__ensure_path(path, root=parent, parent_only=True)
+        
+        [ logging.debug("Non-multimodal source: %r" % (s,)) for s in dsel.all_sources ]
+
+        parent_node.add_node(ExdatSourcesGroup(child_name, parent_node, array_like=array_like,
+                                               selection=dsel.select([
+                                                   (k, '*') for k in dsel.all_sources
+                                               ]) ) )
+
+
     def __enter__(self, *args, **kwargs):
         ''' Overriding the `silx.io.commonh5.File` enter/exit mechanism.
         
         ScanReader depends on using nested with-guards (enter/exit), i.e.
         entering/exitting multiple times on the same object.
         This is an extension to do just that.
         '''
@@ -314,46 +518,41 @@
         if self._enter_cnt == 0:
             super().__exit__(*args, **kwargs)
 
 
 from extra_data.components import AGIPD1M
             
 ''' Quick'n Dirty database of XFEL detectors and their data.
-
 This is what we need to convert detector tiles into XRD images.
 '''
 detectors = {
     'AGIPD1M-1': {
         'selection': [
             ('MID_DET_AGIPD1M-1/DET/*CH0:xtdf', '*'),
             ('MID_AGIPD_MOTION/MDL/DOWNSAMPLER', '*ActualPosition.value'),
             ('MID_EXP_EPIX-1/DET/RECEIVER:daqOutput','data.image.pixels'),
             ('SA2_XTD1_XGM/XGM/DOOCS:output','data.intensityTD'),
             ('MID_EXP_SAM/MDL/DOWNSAMPLER','ssryActualPosition.value'),
         ],
 
         'data_template': {
-            'tmp':  tuple([ '@{measurement}/MID_DET_AGIPD1M-1/DET/%dCH0:xtdf/'
-                              'image.data' % i \
-                              for i in range(1) ]),
 
-            'tiles': lambda h5, nodeOnly, slicer: \
-            AGIPD1M(h5.dsel).get_dask_array('image.data').transpose('train_pulse', 'module', 'dim_0', 'dim_1')[slicer],
-            
-            'motors': tuple([ ('@{measurement}/MID_AGIPD_MOTION/MDL/DOWNSAMPLER/q%dm1ActualPosition.value' % i,
-                               '@{measurement}/MID_AGIPD_MOTION/MDL/DOWNSAMPLER/q%dm2ActualPosition.value' % i)
+            'tiles': '@{instrument}/multimod/MID_DET_AGIPD1M-1/image.data',
+                        
+            'motors': tuple([ ('@{instrument}/selection/MID_AGIPD_MOTION/MDL/DOWNSAMPLER/q%dm1ActualPosition.value' % i,
+                               '@{instrument}/selection/MID_AGIPD_MOTION/MDL/DOWNSAMPLER/q%dm2ActualPosition.value' % i)
                               for i in range(1,5) ]),
 
             'angles': {
-                'theta': '@{measurement}/MID_EXP_SAM/MDL/DOWNSAMPLER/ssryActualPosition.value',
+                'theta': '@{instrument}/selection/MID_EXP_SAM/MDL/DOWNSAMPLER/ssryActualPosition.value',
             },
 
             'norm': {
-                'epix': '@{measurement}/MID_EXP_EPIX-1/DET/RECEIVER:daqOutput/data.image.pixels',
-                'xgm':  '@{measurement}/SA2_XTD1_XGM/XGM/DOOCS:output/data.intensityTD',
+                'epix': '@{instrument}/selection/MID_EXP_EPIX-1/DET/RECEIVER:daqOutput/data.image.pixels',
+                'xgm':  '@{instrument}/selection/SA2_XTD1_XGM/XGM/DOOCS:output/data.intensityTD',
             }
         },
     },
 }
 
 
 class DetectorTiler:
@@ -508,24 +707,33 @@
             tiles = lambda t: t.sum("train_pulse") if len(t.shape)>3 else t
 
         if mask is None:
             mask = self.mask if self.mask is not None else 1
              
         motorset = [(motors(x), motors(y)) for x,y in self.motors]
         geom = self._geom_from_motors(*tuple(motorset))
-
+        
         tileset = tiles(self.tiles[pulse_slicer])
        
         xrd_image, xrd_center = geom.position_modules(tileset * mask)
         x, y, z = geom.get_pixel_positions().T
 
+        # Build coordinate axes of resulting image: the last two coordinates
+        # (X/Y) have the same labels as the detector module directions (typically
+        # dim_0 / dim_1). The other dimensions (there may be others in front)
+        # we just take over from the tileset. We ignore -3 (it being the "module"
+        # dimension which we just "tiled" away).
+        result_coords = { d:tileset.coords[d] for d in tileset.dims[:-3] }
+        result_coords.update({ tileset.dims[i]: np_array(range(xrd_image.shape[i])) - xrd_center[i] \
+                               for i in (-2,-1) })
+
+        print ("result axes:", result_coords)
+
         result = {
-            "image": DataArray(data=xrd_image,
-                               coords={"x": np_array(range(xrd_image.shape[-2])) - xrd_center[-2],
-                                       "y": np_array(range(xrd_image.shape[-1])) - xrd_center[-1]}),
+            "image": DataArray(data=xrd_image, coords=result_coords),
             "metrics": {
                 "imageChannelSize": ((x[-1,0,0] - x[0,0,0]) / x.shape[0],
                                      (y[0,-1,0] - y[0,0,0]) / y.shape[1]),
                 "imageSize": xrd_image.shape,
                 "imageCenter": tuple(xrd_center),
                 "imageDistance": z.mean()
             }
```

### Comparing `nx5d-0.3.0/src/nx5d/nx.py` & `nx5d-0.3.1/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/runlog.py` & `nx5d-0.3.1/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.1/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/analysis.py` & `nx5d-0.3.1/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.1/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.1/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/experiment.py` & `nx5d-0.3.1/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/kmc3.py` & `nx5d-0.3.1/src/nx5d/xrd/kmc3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/roi.py` & `nx5d-0.3.1/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.1/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.1/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.1/src/nx5d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.0
+Version: 0.3.1
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.0/src/nx5d.egg-info/SOURCES.txt` & `nx5d-0.3.1/src/nx5d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.gitlab-ci.yml
 .readthedocs.yaml
 COPYING.md
 README.md
 mkdocs.yml
 pyproject.toml
 scratch.org
 setup.cfg
@@ -28,34 +29,38 @@
 doc/mkdocs/user-guide/index.md
 src/nx5d/__init__.py
 src/nx5d/_version.py
 src/nx5d/edf.py
 src/nx5d/nx.py
 src/nx5d/runlog.py
 src/nx5d/scan.py
+src/nx5d/streaks.py
 src/nx5d.egg-info/PKG-INFO
 src/nx5d.egg-info/SOURCES.txt
 src/nx5d.egg-info/dependency_links.txt
 src/nx5d.egg-info/requires.txt
 src/nx5d.egg-info/top_level.txt
 src/nx5d/h5like/__init__.py
 src/nx5d/h5like/pypod.py
+src/nx5d/h5like/tools.py
 src/nx5d/h5like/xfel.py
 src/nx5d/xrd/ColonelSandersFinest.py
 src/nx5d/xrd/__init__.py
 src/nx5d/xrd/analysis.py
 src/nx5d/xrd/esrf_id09.py
 src/nx5d/xrd/experiment-xpp.yml
 src/nx5d/xrd/experiment.py
 src/nx5d/xrd/kmc3.py
 src/nx5d/xrd/roi.py
 src/nx5d/xrd/signal.py
+src/nx5d/xrd/xfel.py
 src/nx5d/xrd/xraytest.py
 src/nx5d/xrd/xrd_helpers.py
 tests/.gitignore
+tests/pabst_test.py
 tests/pypod_test.py
 tests/runlog_test.py
 tests/xfel_test.py
 tests/xrd_data_test.py
 tests/xrd_kmc3_test.py
 tests/test_data/runfile/run04.log
 tests/test_data/runfile/run105.log
```

### Comparing `nx5d-0.3.0/tests/pypod_test.py` & `nx5d-0.3.1/tests/pypod_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,8 +43,20 @@
     concat_h5(h5, {"boron": {"theMoron": np_array(range(30)).reshape(6,5)}})
 
     s = h5["boron/theMoron"]
 
     assert s.shape == (10, 5)
             
 
-        
+def test_concat_hetero():
+    '''Returns a HDF5 object with virtual data.'''
+
+    data = {
+        "idx": np_array(range(100)),
+        "moo": np_array(range(300)).reshape(100,3)
+    }
+
+    h5 = h5py.File("/dev/null", "a", driver="core", backing_store=False)
+    concat_h5(h5, data)
+
+    return h5
+
```

### Comparing `nx5d-0.3.0/tests/runlog_test.py` & `nx5d-0.3.1/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run04.log` & `nx5d-0.3.1/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run105.log` & `nx5d-0.3.1/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.1/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.1/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.1/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.1/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.1/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.1/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.1/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/xrd_data_test.py` & `nx5d-0.3.1/tests/xrd_data_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.0/tests/xrd_kmc3_test.py` & `nx5d-0.3.1/tests/xrd_kmc3_test.py`

 * *Files identical despite different names*

