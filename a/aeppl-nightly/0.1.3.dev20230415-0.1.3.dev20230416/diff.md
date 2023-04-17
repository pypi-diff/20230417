# Comparing `tmp/aeppl-nightly-0.1.3.dev20230415.tar.gz` & `tmp/aeppl-nightly-0.1.3.dev20230416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.3.dev20230415.tar", last modified: Sat Apr 15 00:32:11 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.3.dev20230416.tar", last modified: Sun Apr 16 00:31:26 2023, max compression
```

## Comparing `aeppl-nightly-0.1.3.dev20230415.tar` & `aeppl-nightly-0.1.3.dev20230416.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:32:11.778541 aeppl-nightly-0.1.3.dev20230415/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-15 00:32:11.778541 aeppl-nightly-0.1.3.dev20230415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:32:11.782541 aeppl-nightly-0.1.3.dev20230415/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-15 00:32:11.782541 aeppl-nightly-0.1.3.dev20230415/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:32:11.774541 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 00:32:11.000000 aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-15 00:32:11.782541 aeppl-nightly-0.1.3.dev20230415/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:32:11.778541 aeppl-nightly-0.1.3.dev20230415/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-15 00:32:02.000000 aeppl-nightly-0.1.3.dev20230415/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:31:26.766593 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 00:31:26.000000 aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 00:31:26.770594 aeppl-nightly-0.1.3.dev20230416/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-16 00:31:10.000000 aeppl-nightly-0.1.3.dev20230416/versioneer.py
```

### Comparing `aeppl-nightly-0.1.3.dev20230415/LICENSE` & `aeppl-nightly-0.1.3.dev20230416/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230416/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230415
+Version: 0.1.3.dev20230416
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230415/README.md` & `aeppl-nightly-0.1.3.dev20230416/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/abstract.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/censoring.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/cumsum.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/dists.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/logprob.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/mixture.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/printing.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/rewriting.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/scan.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/tensor.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/transforms.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl/utils.py` & `aeppl-nightly-0.1.3.dev20230416/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230415
+Version: 0.1.3.dev20230416
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230415/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.3.dev20230416/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/setup.cfg` & `aeppl-nightly-0.1.3.dev20230416/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/setup.py` & `aeppl-nightly-0.1.3.dev20230416/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_abstract.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_censoring.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_cumsum.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_dist.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_logprob.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_mixture.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_printing.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_rewriting.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_scan.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_tensor.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_transforms.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/tests/test_utils.py` & `aeppl-nightly-0.1.3.dev20230416/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230415/versioneer.py` & `aeppl-nightly-0.1.3.dev20230416/versioneer.py`

 * *Files identical despite different names*

