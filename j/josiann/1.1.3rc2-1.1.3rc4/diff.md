# Comparing `tmp/josiann-1.1.3rc2.tar.gz` & `tmp/josiann-1.1.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "josiann-1.1.3rc2.tar", last modified: Mon Apr 17 08:28:16 2023, max compression
+gzip compressed data, was "josiann-1.1.3rc4.tar", last modified: Mon Apr 17 08:35:07 2023, max compression
```

## Comparing `josiann-1.1.3rc2.tar` & `josiann-1.1.3rc4.tar`

### file list

```diff
@@ -1,53 +1,102 @@
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21395 2023-03-07 14:36:43.000000 josiann-1.1.3rc2/LICENSE
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      937 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/README.md
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1188 2023-04-17 08:15:18.000000 josiann-1.1.3rc2/josiann/__init__.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/algorithms/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/algorithms/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5653 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/algorithms/run.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/backup/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/backup/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3376 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/backup/backup.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1685 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/backup/multicore.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/backup/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/backup/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2539 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/backup/parallel/backup.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2950 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/compute.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      310 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/errors.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/moves/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/moves/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3885 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/moves/base.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6953 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/moves/discrete.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3854 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/moves/ensemble.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3125 2023-03-11 15:52:52.000000 josiann-1.1.3rc2/josiann/moves/parse.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4871 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/moves/sequential.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      367 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2616 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/parallel/arguments.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/josiann/storage/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/storage/__init__.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/josiann/storage/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/josiann/storage/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9964 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/storage/parallel/parameters.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12683 2023-03-07 14:36:43.000000 josiann-1.1.3rc2/josiann/storage/parallel/trace.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10395 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/storage/parameters.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1520 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/storage/result.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    31976 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/storage/trace.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1132 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/josiann/typing.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.765628 josiann-1.1.3rc2/josiann.egg-info/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:28:16.000000 josiann-1.1.3rc2/josiann.egg-info/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1015 2023-04-17 08:28:16.000000 josiann-1.1.3rc2/josiann.egg-info/SOURCES.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-04-17 08:28:16.000000 josiann-1.1.3rc2/josiann.egg-info/dependency_links.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      106 2023-04-17 08:28:16.000000 josiann-1.1.3rc2/josiann.egg-info/requires.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        8 2023-04-17 08:28:16.000000 josiann-1.1.3rc2/josiann.egg-info/top_level.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1799 2023-04-17 08:27:32.000000 josiann-1.1.3rc2/pyproject.toml
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      304 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/setup.cfg
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:28:16.769628 josiann-1.1.3rc2/tests/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc2/tests/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      457 2023-03-07 14:36:43.000000 josiann-1.1.3rc2/tests/conftest.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1687 2023-03-07 14:36:43.000000 josiann-1.1.3rc2/tests/test_mcsa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1184 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/tests/test_psa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3732 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/tests/test_sa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4849 2023-03-13 10:16:25.000000 josiann-1.1.3rc2/tests/test_vsa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21395 2023-03-07 14:36:43.000000 josiann-1.1.3rc4/LICENSE
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      937 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/README.md
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/docs/
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/docs/source/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3210 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/docs/source/conf.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1188 2023-04-17 08:15:18.000000 josiann-1.1.3rc4/josiann/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/map/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2085 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/linear.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2860 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/multicore.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      773 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/typing.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3091 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/utils.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     7632 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/map/vectorized.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5653 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/run.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/sequential/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/sequential/base/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/base/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1159 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/base/compute.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5566 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/base/intialize.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5082 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/base/sa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/sequential/multicore/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/multicore/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     7126 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/multicore/initialize.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     5608 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/multicore/mcsa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/algorithms/sequential/vectorized/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/vectorized/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3557 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/vectorized/compute.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9265 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/vectorized/intialize.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     7867 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/algorithms/sequential/vectorized/vsa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann/backup/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/backup/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3376 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/backup/backup.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1685 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/backup/multicore.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/backup/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/backup/parallel/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2539 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/backup/parallel/backup.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2950 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/compute.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      310 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/errors.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/moves/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/moves/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3885 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/moves/base.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6953 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/moves/discrete.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3854 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/moves/ensemble.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3125 2023-03-11 15:52:52.000000 josiann-1.1.3rc4/josiann/moves/parse.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4871 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/moves/sequential.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      367 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/parallel/algorithms/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/algorithms/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1895 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/algorithms/compute.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4964 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/algorithms/mappers.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     8792 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/algorithms/psa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2616 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/arguments.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/parallel/moves/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      145 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/moves/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2677 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/moves/base.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3667 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/parallel/moves/discrete.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/storage/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/storage/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/josiann/storage/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/josiann/storage/parallel/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9964 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/storage/parallel/parameters.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12683 2023-03-07 14:36:43.000000 josiann-1.1.3rc4/josiann/storage/parallel/trace.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10395 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/storage/parameters.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1520 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/storage/result.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    31976 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/storage/trace.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1132 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/josiann/typing.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/josiann.egg-info/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:35:07.000000 josiann-1.1.3rc4/josiann.egg-info/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2445 2023-04-17 08:35:07.000000 josiann-1.1.3rc4/josiann.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-04-17 08:35:07.000000 josiann-1.1.3rc4/josiann.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      106 2023-04-17 08:35:07.000000 josiann-1.1.3rc4/josiann.egg-info/requires.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        8 2023-04-17 08:35:07.000000 josiann-1.1.3rc4/josiann.egg-info/top_level.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1615 2023-04-17 08:34:38.000000 josiann-1.1.3rc4/pyproject.toml
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      304 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/setup.cfg
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/tests/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc4/tests/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      457 2023-03-07 14:36:43.000000 josiann-1.1.3rc4/tests/conftest.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1687 2023-03-07 14:36:43.000000 josiann-1.1.3rc4/tests/test_mcsa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1184 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/tests/test_psa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3732 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/tests/test_sa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4849 2023-03-13 10:16:25.000000 josiann-1.1.3rc4/tests/test_vsa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.177566 josiann-1.1.3rc4/venv_josiann/
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:35:07.181566 josiann-1.1.3rc4/venv_josiann/bin/
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      631 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2html.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      751 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2html4.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)     1119 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2html5.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      828 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2latex.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      636 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2man.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      801 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2odt.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)     1763 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      638 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      674 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2s5.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      908 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2xetex.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      639 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rst2xml.py
+-rwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)      707 2023-03-09 22:42:43.000000 josiann-1.1.3rc4/venv_josiann/bin/rstpep2html.py
```

### Comparing `josiann-1.1.3rc2/LICENSE` & `josiann-1.1.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/PKG-INFO` & `josiann-1.1.3rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: josiann
-Version: 1.1.3rc2
+Version: 1.1.3rc4
 Summary: Simulated Annealing for noisy cost functions.
 Author-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 Maintainer-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 License: CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `josiann-1.1.3rc2/README.md` & `josiann-1.1.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/__init__.py` & `josiann-1.1.3rc4/josiann/__init__.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/algorithms/run.py` & `josiann-1.1.3rc4/josiann/algorithms/run.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/backup/backup.py` & `josiann-1.1.3rc4/josiann/backup/backup.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/backup/multicore.py` & `josiann-1.1.3rc4/josiann/backup/multicore.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/backup/parallel/backup.py` & `josiann-1.1.3rc4/josiann/backup/parallel/backup.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/compute.py` & `josiann-1.1.3rc4/josiann/compute.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/moves/base.py` & `josiann-1.1.3rc4/josiann/moves/base.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/moves/discrete.py` & `josiann-1.1.3rc4/josiann/moves/discrete.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/moves/ensemble.py` & `josiann-1.1.3rc4/josiann/moves/ensemble.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/moves/parse.py` & `josiann-1.1.3rc4/josiann/moves/parse.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/moves/sequential.py` & `josiann-1.1.3rc4/josiann/moves/sequential.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/parallel/arguments.py` & `josiann-1.1.3rc4/josiann/parallel/arguments.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/storage/parallel/parameters.py` & `josiann-1.1.3rc4/josiann/storage/parallel/parameters.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/storage/parallel/trace.py` & `josiann-1.1.3rc4/josiann/storage/parallel/trace.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/storage/parameters.py` & `josiann-1.1.3rc4/josiann/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/storage/result.py` & `josiann-1.1.3rc4/josiann/storage/result.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/storage/trace.py` & `josiann-1.1.3rc4/josiann/storage/trace.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann/typing.py` & `josiann-1.1.3rc4/josiann/typing.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/josiann.egg-info/PKG-INFO` & `josiann-1.1.3rc4/josiann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: josiann
-Version: 1.1.3rc2
+Version: 1.1.3rc4
 Summary: Simulated Annealing for noisy cost functions.
 Author-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 Maintainer-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 License: CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `josiann-1.1.3rc2/tests/test_mcsa.py` & `josiann-1.1.3rc4/tests/test_mcsa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/tests/test_psa.py` & `josiann-1.1.3rc4/tests/test_psa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/tests/test_sa.py` & `josiann-1.1.3rc4/tests/test_sa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.3rc2/tests/test_vsa.py` & `josiann-1.1.3rc4/tests/test_vsa.py`

 * *Files identical despite different names*

