# Comparing `tmp/spams-bin-2.6.5.tar.gz` & `tmp/spams-bin-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spams-bin-2.6.5.tar", last modified: Wed Feb 15 11:29:01 2023, max compression
+gzip compressed data, was "spams-bin-2.6.6.tar", last modified: Mon Apr 17 14:28:43 2023, max compression
```

## Comparing `spams-bin-2.6.5.tar` & `spams-bin-2.6.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.688953 spams-bin-2.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-02-15 11:28:47.000000 spams-bin-2.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-15 11:28:47.000000 spams-bin-2.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-15 11:29:01.688953 spams-bin-2.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-15 11:28:47.000000 spams-bin-2.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-02-15 11:28:47.000000 spams-bin-2.6.5/openmp_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-15 11:28:47.000000 spams-bin-2.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 11:29:01.688953 spams-bin-2.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-02-15 11:28:47.000000 spams-bin-2.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams/spams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams_bin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-15 11:29:01.000000 spams-bin-2.6.5/spams_bin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-15 11:29:01.000000 spams-bin-2.6.5/spams_bin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 11:29:01.000000 spams-bin-2.6.5/spams_bin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-15 11:29:01.000000 spams-bin-2.6.5/spams_bin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-15 11:29:01.000000 spams-bin-2.6.5/spams_bin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams_wrap/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams_wrap/spams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams_wrap/spams/decomp/
--rw-r--r--   0 runner    (1001) docker     (123)    92283 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/decomp/decomp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/decomp/lsqsplx.h
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/decomp/projsplx.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.684953 spams-bin-2.6.5/spams_wrap/spams/dictLearn/
--rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/dictLearn/arch.h
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/dictLearn/dicts.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.688953 spams-bin-2.6.5/spams_wrap/spams/linalg/
--rwxr-xr-x   0 runner    (1001) docker     (123)    40668 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_alt_template.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1291 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_defvar.h
--rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_template.h
--rwxr-xr-x   0 runner    (1001) docker     (123)   165896 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/linalg.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     7765 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/list.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     7948 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/mexutils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/misc.h
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/linalg/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.688953 spams-bin-2.6.5/spams_wrap/spams/prox/
--rw-r--r--   0 runner    (1001) docker     (123)   155546 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/fista.h
--rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/groups-graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/mexgrouputils.h
--rw-r--r--   0 runner    (1001) docker     (123)   110823 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/project.h
--rw-r--r--   0 runner    (1001) docker     (123)    53725 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/surrogate.h
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams/prox/svm.h
--rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams.h
--rw-r--r--   0 runner    (1001) docker     (123)   742180 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams_wrap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-15 11:28:47.000000 spams-bin-2.6.5/spams_wrap/spams_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 11:29:01.688953 spams-bin-2.6.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)   177762 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/boat.png
--rw-r--r--   0 runner    (1001) docker     (123)   151199 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/lena.png
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_dictLearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    38902 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_prox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_spams.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-15 11:28:47.000000 spams-bin-2.6.5/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.279169 spams-bin-2.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-04-17 14:28:31.000000 spams-bin-2.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-17 14:28:31.000000 spams-bin-2.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 14:28:43.279169 spams-bin-2.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 14:28:31.000000 spams-bin-2.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-17 14:28:31.000000 spams-bin-2.6.6/openmp_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 14:28:31.000000 spams-bin-2.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:28:43.279169 spams-bin-2.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-17 14:28:31.000000 spams-bin-2.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.275169 spams-bin-2.6.6/spams/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28693 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams/spams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.275169 spams-bin-2.6.6/spams_bin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-17 14:28:43.000000 spams-bin-2.6.6/spams_bin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-17 14:28:43.000000 spams-bin-2.6.6/spams_bin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:28:43.000000 spams-bin-2.6.6/spams_bin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 14:28:43.000000 spams-bin-2.6.6/spams_bin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 14:28:43.000000 spams-bin-2.6.6/spams_bin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.275169 spams-bin-2.6.6/spams_wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.271170 spams-bin-2.6.6/spams_wrap/spams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.275169 spams-bin-2.6.6/spams_wrap/spams/decomp/
+-rw-r--r--   0 runner    (1001) docker     (123)    92283 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/decomp/decomp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/decomp/lsqsplx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/decomp/projsplx.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.275169 spams-bin-2.6.6/spams_wrap/spams/dictLearn/
+-rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/dictLearn/arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/dictLearn/dicts.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.279169 spams-bin-2.6.6/spams_wrap/spams/linalg/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40668 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_alt_template.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1291 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_defvar.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_template.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165896 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/linalg.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7765 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/list.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7948 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/mexutils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/misc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/linalg/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.279169 spams-bin-2.6.6/spams_wrap/spams/prox/
+-rw-r--r--   0 runner    (1001) docker     (123)   155546 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/fista.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20447 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/groups-graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/mexgrouputils.h
+-rw-r--r--   0 runner    (1001) docker     (123)   110823 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/project.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53725 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/surrogate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams/prox/svm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44470 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams.h
+-rw-r--r--   0 runner    (1001) docker     (123)   742180 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams_wrap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-17 14:28:31.000000 spams-bin-2.6.6/spams_wrap/spams_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:28:43.279169 spams-bin-2.6.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)   177762 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/boat.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151199 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/lena.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_dictLearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38902 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_prox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_spams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-17 14:28:31.000000 spams-bin-2.6.6/test/test_utils.py
```

### Comparing `spams-bin-2.6.5/LICENSE` & `spams-bin-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/PKG-INFO` & `spams-bin-2.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spams-bin
-Version: 2.6.5
+Version: 2.6.6
 Summary: Python interface for SPAMS - binary wheels with openblas (mac, linux, windows)
 Home-page: http://spams-devel.gforge.inria.fr/
 Author: Julien Mairal
 Author-email: spams.dev@inria.fr
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `spams-bin-2.6.5/README.md` & `spams-bin-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/openmp_helpers.py` & `spams-bin-2.6.6/openmp_helpers.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/setup.py` & `spams-bin-2.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 In addition, building from source explicitly requires openblas on mac/linux and intel mkl on windows,
 unlike the official version which can use any blas implementation.
 
 The source code for this fork is also available at https://github.com/samuelstjean/spams-python/"""
 
 setup(name='spams-bin',
-      version='2.6.5',
+      version='2.6.6',
       description='Python interface for SPAMS - binary wheels with openblas (mac, linux, windows)',
       long_description=long_description,
       author='Julien Mairal',
       author_email='spams.dev@inria.fr',
       url='http://spams-devel.gforge.inria.fr/',
       ext_modules=[spams_wrap],
       packages=find_packages(),
```

### Comparing `spams-bin-2.6.5/spams/spams.py` & `spams-bin-2.6.6/spams/spams.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_bin.egg-info/PKG-INFO` & `spams-bin-2.6.6/spams_bin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spams-bin
-Version: 2.6.5
+Version: 2.6.6
 Summary: Python interface for SPAMS - binary wheels with openblas (mac, linux, windows)
 Home-page: http://spams-devel.gforge.inria.fr/
 Author: Julien Mairal
 Author-email: spams.dev@inria.fr
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `spams-bin-2.6.5/spams_bin.egg-info/SOURCES.txt` & `spams-bin-2.6.6/spams_bin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/decomp/decomp.h` & `spams-bin-2.6.6/spams_wrap/spams/decomp/decomp.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/decomp/lsqsplx.h` & `spams-bin-2.6.6/spams_wrap/spams/decomp/lsqsplx.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/decomp/projsplx.h` & `spams-bin-2.6.6/spams_wrap/spams/decomp/projsplx.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/dictLearn/arch.h` & `spams-bin-2.6.6/spams_wrap/spams/dictLearn/arch.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/dictLearn/dicts.h` & `spams-bin-2.6.6/spams_wrap/spams/dictLearn/dicts.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_alt_template.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_alt_template.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_defvar.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_defvar.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/cblas_template.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/cblas_template.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/linalg.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/linalg.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/list.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/list.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/mexutils.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/mexutils.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/misc.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/misc.h`

 * *Files 2% similar despite different names*

```diff
@@ -285,20 +285,28 @@
    return sqrtf(x);
 };
 
 static inline int init_omp(const int numThreads) {
    int NUM_THREADS;
 #ifdef _OPENMP
    NUM_THREADS = (numThreads == -1) ? MIN(MAX_THREADS,omp_get_num_procs()) : numThreads;
+
+   // using 0 thread is undefined behavior/implementation defined, so we force it to 1 instead
+   // https://github.com/samuelstjean/spams-python/issues/33
+   // https://www.openmp.org/spec-html/5.0/openmpsu110.html
+   if (NUM_THREADS == 0) {
+      NUM_THREADS = 1;
+   }
    // omp_set_max_active_levels(1);
    omp_set_dynamic(0);
    omp_set_num_threads(NUM_THREADS);
 #else
    NUM_THREADS = 1;
 #endif
+
    return NUM_THREADS;
 }
 
 template <typename T1, typename T2, typename T3>
 struct Triplet {
    T1 x;
    T2 z;
```

### Comparing `spams-bin-2.6.5/spams_wrap/spams/linalg/utils.h` & `spams-bin-2.6.6/spams_wrap/spams/linalg/utils.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/fista.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/fista.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/groups-graph.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/groups-graph.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/mexgrouputils.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/mexgrouputils.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/project.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/project.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/surrogate.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/surrogate.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams/prox/svm.h` & `spams-bin-2.6.6/spams_wrap/spams/prox/svm.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams.h` & `spams-bin-2.6.6/spams_wrap/spams.h`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams_wrap.cpp` & `spams-bin-2.6.6/spams_wrap/spams_wrap.cpp`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/spams_wrap/spams_wrap.py` & `spams-bin-2.6.6/spams_wrap/spams_wrap.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/boat.png` & `spams-bin-2.6.6/test/boat.png`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/lena.png` & `spams-bin-2.6.6/test/lena.png`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_decomp.py` & `spams-bin-2.6.6/test/test_decomp.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_dictLearn.py` & `spams-bin-2.6.6/test/test_dictLearn.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_linalg.py` & `spams-bin-2.6.6/test/test_linalg.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_prox.py` & `spams-bin-2.6.6/test/test_prox.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_spams.py` & `spams-bin-2.6.6/test/test_spams.py`

 * *Files identical despite different names*

### Comparing `spams-bin-2.6.5/test/test_utils.py` & `spams-bin-2.6.6/test/test_utils.py`

 * *Files identical despite different names*

