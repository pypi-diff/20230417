# Comparing `tmp/josiann-1.1.2.tar.gz` & `tmp/josiann-1.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "josiann-1.1.2.tar", last modified: Mon Mar 13 10:25:51 2023, max compression
+gzip compressed data, was "josiann-1.1.3rc1.tar", last modified: Mon Apr 17 08:17:35 2023, max compression
```

## Comparing `josiann-1.1.2.tar` & `josiann-1.1.3rc1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.125524 josiann-1.1.2/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21395 2023-03-07 14:36:43.000000 josiann-1.1.2/LICENSE
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27593 2023-03-13 10:25:51.125524 josiann-1.1.2/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      937 2023-03-13 10:16:25.000000 josiann-1.1.2/README.md
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1356 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/__init__.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/backup/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/backup/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3376 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/backup/backup.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1685 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/backup/multicore.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/backup/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/backup/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2539 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/backup/parallel/backup.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2950 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/compute.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      310 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/errors.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/moves/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/moves/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3885 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/moves/base.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6953 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/moves/discrete.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3854 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/moves/ensemble.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3125 2023-03-11 15:52:52.000000 josiann-1.1.2/josiann/moves/parse.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4871 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/moves/sequential.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      367 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2616 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/parallel/arguments.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann/storage/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/storage/__init__.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.125524 josiann-1.1.2/josiann/storage/parallel/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.2/josiann/storage/parallel/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9964 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/storage/parallel/parameters.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12683 2023-03-07 14:36:43.000000 josiann-1.1.2/josiann/storage/parallel/trace.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10395 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/storage/parameters.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1520 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/storage/result.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    31976 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/storage/trace.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1132 2023-03-13 10:16:25.000000 josiann-1.1.2/josiann/typing.py
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.121524 josiann-1.1.2/josiann.egg-info/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27593 2023-03-13 10:25:51.000000 josiann-1.1.2/josiann.egg-info/PKG-INFO
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      958 2023-03-13 10:25:51.000000 josiann-1.1.2/josiann.egg-info/SOURCES.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-03-13 10:25:51.000000 josiann-1.1.2/josiann.egg-info/dependency_links.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      106 2023-03-13 10:25:51.000000 josiann-1.1.2/josiann.egg-info/requires.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        8 2023-03-13 10:25:51.000000 josiann-1.1.2/josiann.egg-info/top_level.txt
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1739 2023-03-13 10:25:10.000000 josiann-1.1.2/pyproject.toml
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      304 2023-03-13 10:25:51.125524 josiann-1.1.2/setup.cfg
-drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-03-13 10:25:51.125524 josiann-1.1.2/tests/
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.2/tests/__init__.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      457 2023-03-07 14:36:43.000000 josiann-1.1.2/tests/conftest.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1687 2023-03-07 14:36:43.000000 josiann-1.1.2/tests/test_mcsa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1184 2023-03-13 10:16:25.000000 josiann-1.1.2/tests/test_psa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3732 2023-03-13 10:16:25.000000 josiann-1.1.2/tests/test_sa.py
--rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4849 2023-03-13 10:16:25.000000 josiann-1.1.2/tests/test_vsa.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    21395 2023-03-07 14:36:43.000000 josiann-1.1.3rc1/LICENSE
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      937 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/README.md
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1188 2023-04-17 08:15:18.000000 josiann-1.1.3rc1/josiann/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/backup/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/backup/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3376 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/backup/backup.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1685 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/backup/multicore.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/backup/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/backup/parallel/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2539 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/backup/parallel/backup.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2950 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/compute.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      310 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/errors.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/moves/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/moves/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3885 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/moves/base.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     6953 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/moves/discrete.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3854 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/moves/ensemble.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3125 2023-03-11 15:52:52.000000 josiann-1.1.3rc1/josiann/moves/parse.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4871 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/moves/sequential.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      367 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/parallel/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     2616 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/parallel/arguments.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/storage/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/storage/__init__.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann/storage/parallel/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/josiann/storage/parallel/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     9964 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/storage/parallel/parameters.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    12683 2023-03-07 14:36:43.000000 josiann-1.1.3rc1/josiann/storage/parallel/trace.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    10395 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/storage/parameters.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1520 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/storage/result.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    31976 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/storage/trace.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1132 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/josiann/typing.py
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/josiann.egg-info/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)    27596 2023-04-17 08:17:35.000000 josiann-1.1.3rc1/josiann.egg-info/PKG-INFO
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      958 2023-04-17 08:17:35.000000 josiann-1.1.3rc1/josiann.egg-info/SOURCES.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        1 2023-04-17 08:17:35.000000 josiann-1.1.3rc1/josiann.egg-info/dependency_links.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      106 2023-04-17 08:17:35.000000 josiann-1.1.3rc1/josiann.egg-info/requires.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)        8 2023-04-17 08:17:35.000000 josiann-1.1.3rc1/josiann.egg-info/top_level.txt
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1773 2023-04-17 08:17:02.000000 josiann-1.1.3rc1/pyproject.toml
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      304 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/setup.cfg
+drwxrwxr-x   0 mbouvier  (1001) mbouvier  (1001)        0 2023-04-17 08:17:35.387999 josiann-1.1.3rc1/tests/
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      193 2023-02-01 15:40:02.000000 josiann-1.1.3rc1/tests/__init__.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)      457 2023-03-07 14:36:43.000000 josiann-1.1.3rc1/tests/conftest.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1687 2023-03-07 14:36:43.000000 josiann-1.1.3rc1/tests/test_mcsa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     1184 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/tests/test_psa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     3732 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/tests/test_sa.py
+-rw-rw-r--   0 mbouvier  (1001) mbouvier  (1001)     4849 2023-03-13 10:16:25.000000 josiann-1.1.3rc1/tests/test_vsa.py
```

### Comparing `josiann-1.1.2/LICENSE` & `josiann-1.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/PKG-INFO` & `josiann-1.1.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: josiann
-Version: 1.1.2
+Version: 1.1.3rc1
 Summary: Simulated Annealing for noisy cost functions.
 Author-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 Maintainer-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 License: CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `josiann-1.1.2/README.md` & `josiann-1.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/__init__.py` & `josiann-1.1.3rc1/josiann/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,22 @@
 # imports
 try:
     from importlib import metadata
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata  # type: ignore[import, no-redef]
 
 from josiann.algorithms.sequential.base.sa import sa
-from josiann.algorithms.sequential.vectorized.vsa import vsa
 from josiann.algorithms.sequential.multicore.mcsa import mcsa
-
+from josiann.algorithms.sequential.vectorized.vsa import vsa
+from josiann.moves.discrete import SetStep, SetStretch
+from josiann.moves.ensemble import Stretch, StretchAdaptive
+from josiann.moves.sequential import Metropolis, Metropolis1D, RandomStep
 from josiann.storage.result import Result
 from josiann.storage.trace import Trace
 
-from josiann.moves.sequential import RandomStep
-from josiann.moves.sequential import Metropolis
-from josiann.moves.sequential import Metropolis1D
-from josiann.moves.discrete import SetStep
-from josiann.moves.discrete import SetStretch
-from josiann.moves.ensemble import Stretch
-from josiann.moves.ensemble import StretchAdaptive
-
-import josiann.parallel
-
-
 # ====================================================
 # code
 __all__ = [
     "sa",
     "vsa",
     "mcsa",
     "Result",
```

### Comparing `josiann-1.1.2/josiann/backup/backup.py` & `josiann-1.1.3rc1/josiann/backup/backup.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/backup/multicore.py` & `josiann-1.1.3rc1/josiann/backup/multicore.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/backup/parallel/backup.py` & `josiann-1.1.3rc1/josiann/backup/parallel/backup.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/compute.py` & `josiann-1.1.3rc1/josiann/compute.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/moves/base.py` & `josiann-1.1.3rc1/josiann/moves/base.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/moves/discrete.py` & `josiann-1.1.3rc1/josiann/moves/discrete.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/moves/ensemble.py` & `josiann-1.1.3rc1/josiann/moves/ensemble.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/moves/parse.py` & `josiann-1.1.3rc1/josiann/moves/parse.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/moves/sequential.py` & `josiann-1.1.3rc1/josiann/moves/sequential.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/parallel/arguments.py` & `josiann-1.1.3rc1/josiann/parallel/arguments.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/storage/parallel/parameters.py` & `josiann-1.1.3rc1/josiann/storage/parallel/parameters.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/storage/parallel/trace.py` & `josiann-1.1.3rc1/josiann/storage/parallel/trace.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/storage/parameters.py` & `josiann-1.1.3rc1/josiann/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/storage/result.py` & `josiann-1.1.3rc1/josiann/storage/result.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/storage/trace.py` & `josiann-1.1.3rc1/josiann/storage/trace.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann/typing.py` & `josiann-1.1.3rc1/josiann/typing.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/josiann.egg-info/PKG-INFO` & `josiann-1.1.3rc1/josiann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: josiann
-Version: 1.1.2
+Version: 1.1.3rc1
 Summary: Simulated Annealing for noisy cost functions.
 Author-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 Maintainer-email: Matteo Bouvier <m.bouvier@vidium-solutions.com>
 License: CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
```

### Comparing `josiann-1.1.2/josiann.egg-info/SOURCES.txt` & `josiann-1.1.3rc1/josiann.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/pyproject.toml` & `josiann-1.1.3rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "josiann"
 description = "Simulated Annealing for noisy cost functions."
-version = "1.1.2"
+version = "1.1.3rc1"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Matteo Bouvier", email = "m.bouvier@vidium-solutions.com"}
 ]
 maintainers = [
     {name = "Matteo Bouvier", email = "m.bouvier@vidium-solutions.com"}
@@ -65,7 +65,10 @@
     "josiann.storage.parallel",
     "josiann.backup",
     "josiann.backup.parallel"
 ]
 
 [tool.vulture]
 paths = ["josiann", "tests", "vulture_whitelist.py"]
+
+[tool.ruff]
+line-length = 120
```

### Comparing `josiann-1.1.2/tests/test_mcsa.py` & `josiann-1.1.3rc1/tests/test_mcsa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/tests/test_psa.py` & `josiann-1.1.3rc1/tests/test_psa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/tests/test_sa.py` & `josiann-1.1.3rc1/tests/test_sa.py`

 * *Files identical despite different names*

### Comparing `josiann-1.1.2/tests/test_vsa.py` & `josiann-1.1.3rc1/tests/test_vsa.py`

 * *Files identical despite different names*

