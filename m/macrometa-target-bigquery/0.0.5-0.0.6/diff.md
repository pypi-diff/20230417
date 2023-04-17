# Comparing `tmp/macrometa-target-bigquery-0.0.5.tar.gz` & `tmp/macrometa-target-bigquery-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-bigquery-0.0.5.tar", last modified: Mon Apr 17 02:56:00 2023, max compression
+gzip compressed data, was "macrometa-target-bigquery-0.0.6.tar", last modified: Mon Apr 17 09:52:21 2023, max compression
```

## Comparing `macrometa-target-bigquery-0.0.5.tar` & `macrometa-target-bigquery-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:00.681662 macrometa-target-bigquery-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 02:56:00.681662 macrometa-target-bigquery-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:00.681662 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/db_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/flattening.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/stream_ref_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:00.681662 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 02:56:00.000000 macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 02:56:00.681662 macrometa-target-bigquery-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 02:55:45.000000 macrometa-target-bigquery-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/db_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/flattening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_ref_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 09:52:21.000000 macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:52:21.513465 macrometa-target-bigquery-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-17 09:52:04.000000 macrometa-target-bigquery-0.0.6/setup.py
```

### Comparing `macrometa-target-bigquery-0.0.5/LICENSE` & `macrometa-target-bigquery-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/PKG-INFO` & `macrometa-target-bigquery-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.5
+Version: 0.0.6
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.5/README.md` & `macrometa-target-bigquery-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/__init__.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/db_sync.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/db_sync.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/exceptions.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/flattening.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/flattening.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/sql_utils.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/stream_ref_helper.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_ref_helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery/stream_utils.py` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery/stream_utils.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/PKG-INFO` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-bigquery
-Version: 0.0.5
+Version: 0.0.6
 Summary: Macrometa target bigquery connector for loading data to BigQuery
 Home-page: https://github.com/Macrometacorp/macrometa-target-bigquery
 Author: Macrometa
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `macrometa-target-bigquery-0.0.5/macrometa_target_bigquery.egg-info/SOURCES.txt` & `macrometa-target-bigquery-0.0.6/macrometa_target_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrometa-target-bigquery-0.0.5/setup.py` & `macrometa-target-bigquery-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name="macrometa-target-bigquery",
-      version='0.0.5',
+      version='0.0.6',
       description="Macrometa target bigquery connector for loading data to BigQuery",
       long_description=long_description,
       long_description_content_type='text/markdown',
       author="Macrometa",
       url='https://github.com/Macrometacorp/macrometa-target-bigquery',
       classifiers=[
           'License :: OSI Approved :: Apache Software License',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=["macrometa_target_bigquery"],
       install_requires=[
           'pipelinewise-singer-python==1.2.0',
           'google-cloud-bigquery>=2.20.0,<3.1.0',
           'fastavro>=0.22.8,<1.4.11',
-          'c8connector==0.0.19'
+          'c8connector>=0.0.20'
       ],
       extras_require={
           "test": [
               'pytest==7.0.1',
               'pylint==2.13.4',
               'pytest-cov==3.0.0',
           ]
```

