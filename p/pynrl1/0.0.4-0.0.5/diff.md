# Comparing `tmp/pynrl1-0.0.4.tar.gz` & `tmp/pynrl1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrl1-0.0.4.tar", last modified: Thu Mar 23 12:33:20 2023, max compression
+gzip compressed data, was "pynrl1-0.0.5.tar", last modified: Mon Apr 17 08:59:42 2023, max compression
```

## Comparing `pynrl1-0.0.4.tar` & `pynrl1-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.650021 pynrl1-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-23 12:33:11.000000 pynrl1-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-23 12:33:20.650021 pynrl1-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 12:33:11.000000 pynrl1-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.646021 pynrl1-0.0.4/pynrl1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.646021 pynrl1-0.0.4/pynrl1/downlink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/downlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/downlink/nr_pbch.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/downlink/nr_pbch_dmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/downlink/nr_pss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/downlink/nr_sss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.646021 pynrl1-0.0.4/pynrl1/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/util/nr_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pynrl1/util/nr_prbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.646021 pynrl1-0.0.4/pynrl1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-23 12:33:20.000000 pynrl1-0.0.4/pynrl1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-23 12:33:20.000000 pynrl1-0.0.4/pynrl1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:33:20.000000 pynrl1-0.0.4/pynrl1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-23 12:33:20.000000 pynrl1-0.0.4/pynrl1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 12:33:20.000000 pynrl1-0.0.4/pynrl1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 12:33:11.000000 pynrl1-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-23 12:33:20.650021 pynrl1-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-23 12:33:11.000000 pynrl1-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:33:20.650021 pynrl1-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_pbch.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_pbch_dmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_prbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_pss.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-23 12:33:11.000000 pynrl1-0.0.4/tests/test_nr_sss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 08:59:27.000000 pynrl1-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 08:59:42.477290 pynrl1-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-17 08:59:27.000000 pynrl1-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.473290 pynrl1-0.0.5/pynrl1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1/downlink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pbch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pbch_dmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pdschdmrs_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_pss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/downlink/nr_sss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/nr_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pynrl1/util/nr_prbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/pynrl1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 08:59:42.000000 pynrl1-0.0.5/pynrl1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 08:59:27.000000 pynrl1-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 08:59:42.481290 pynrl1-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 08:59:27.000000 pynrl1-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:42.477290 pynrl1-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pbch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pbch_dmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pdschdmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pdschdmrs_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_prbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_pss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 08:59:27.000000 pynrl1-0.0.5/tests/test_nr_sss.py
```

### Comparing `pynrl1-0.0.4/LICENSE` & `pynrl1-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/downlink/nr_pbch.py` & `pynrl1-0.0.5/pynrl1/downlink/nr_pbch.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/downlink/nr_pbch_dmrs.py` & `pynrl1-0.0.5/pynrl1/downlink/nr_pbch_dmrs.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/downlink/nr_pss.py` & `pynrl1-0.0.5/pynrl1/downlink/nr_pss.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/downlink/nr_sss.py` & `pynrl1-0.0.5/pynrl1/downlink/nr_sss.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/util/nr_mapper.py` & `pynrl1-0.0.5/pynrl1/util/nr_mapper.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1/util/nr_prbs.py` & `pynrl1-0.0.5/pynrl1/util/nr_prbs.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/pynrl1.egg-info/SOURCES.txt` & `pynrl1-0.0.5/pynrl1.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,23 @@
 pynrl1.egg-info/SOURCES.txt
 pynrl1.egg-info/dependency_links.txt
 pynrl1.egg-info/requires.txt
 pynrl1.egg-info/top_level.txt
 pynrl1/downlink/__init__.py
 pynrl1/downlink/nr_pbch.py
 pynrl1/downlink/nr_pbch_dmrs.py
+pynrl1/downlink/nr_pdschdmrs.py
+pynrl1/downlink/nr_pdschdmrs_indices.py
 pynrl1/downlink/nr_pss.py
 pynrl1/downlink/nr_sss.py
 pynrl1/util/__init__.py
+pynrl1/util/configurations.py
 pynrl1/util/nr_mapper.py
 pynrl1/util/nr_prbs.py
 tests/test_nr_mapper.py
 tests/test_nr_pbch.py
 tests/test_nr_pbch_dmrs.py
+tests/test_nr_pdschdmrs.py
+tests/test_nr_pdschdmrs_indices.py
 tests/test_nr_prbs.py
 tests/test_nr_pss.py
 tests/test_nr_sss.py
```

### Comparing `pynrl1-0.0.4/setup.cfg` & `pynrl1-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_mapper.py` & `pynrl1-0.0.5/tests/test_nr_mapper.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_pbch.py` & `pynrl1-0.0.5/tests/test_nr_pbch.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_pbch_dmrs.py` & `pynrl1-0.0.5/tests/test_nr_pbch_dmrs.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_prbs.py` & `pynrl1-0.0.5/tests/test_nr_prbs.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_pss.py` & `pynrl1-0.0.5/tests/test_nr_pss.py`

 * *Files identical despite different names*

### Comparing `pynrl1-0.0.4/tests/test_nr_sss.py` & `pynrl1-0.0.5/tests/test_nr_sss.py`

 * *Files identical despite different names*

