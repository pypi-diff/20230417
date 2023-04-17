# Comparing `tmp/storey-1.3.8.tar.gz` & `tmp/storey-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-wlps0ajy/storey-1.3.8.tar", last modified: Mon Feb 13 11:41:53 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-ww2czogr/storey-1.3.9.tar", last modified: Thu Feb 16 15:38:36 2023, max compression
```

## Comparing `storey-1.3.8.tar` & `storey-1.3.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 11:39:06.000000 storey-1.3.8/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-13 11:39:06.000000 storey-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-13 11:39:06.000000 storey-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-13 11:41:53.000000 storey-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-02-13 11:39:06.000000 storey-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-13 11:39:06.000000 storey-1.3.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-13 11:39:06.000000 storey-1.3.8/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-02-13 11:39:06.000000 storey-1.3.8/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-02-13 11:39:06.000000 storey-1.3.8/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   167676 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    43061 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-02-13 11:39:06.000000 storey-1.3.8/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-13 11:39:06.000000 storey-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-13 11:41:53.000000 storey-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-13 11:39:06.000000 storey-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-13 11:41:48.000000 storey-1.3.8/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-13 11:39:06.000000 storey-1.3.8/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-02-13 11:39:06.000000 storey-1.3.8/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-02-13 11:39:06.000000 storey-1.3.8/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28063 2023-02-13 11:39:06.000000 storey-1.3.8/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-02-13 11:39:06.000000 storey-1.3.8/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50620 2023-02-13 11:39:06.000000 storey-1.3.8/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-13 11:39:06.000000 storey-1.3.8/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-02-13 11:39:06.000000 storey-1.3.8/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    41331 2023-02-13 11:39:06.000000 storey-1.3.8/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-13 11:39:06.000000 storey-1.3.8/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-02-13 11:39:06.000000 storey-1.3.8/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79772 2023-02-13 11:39:06.000000 storey-1.3.8/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    50736 2023-02-13 11:39:06.000000 storey-1.3.8/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-13 11:39:06.000000 storey-1.3.8/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-02-13 11:39:06.000000 storey-1.3.8/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-02-13 11:39:06.000000 storey-1.3.8/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-13 11:41:53.000000 storey-1.3.8/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 11:41:53.000000 storey-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-13 11:39:06.000000 storey-1.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   117320 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-13 11:39:06.000000 storey-1.3.8/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-16 15:32:21.000000 storey-1.3.9/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 15:32:21.000000 storey-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-16 15:32:21.000000 storey-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-16 15:38:36.000000 storey-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-02-16 15:32:21.000000 storey-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-16 15:32:21.000000 storey-1.3.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-16 15:32:21.000000 storey-1.3.9/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-02-16 15:32:21.000000 storey-1.3.9/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-02-16 15:32:21.000000 storey-1.3.9/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43061 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-02-16 15:32:21.000000 storey-1.3.9/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-16 15:32:21.000000 storey-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-16 15:38:36.000000 storey-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-16 15:32:21.000000 storey-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-16 15:38:31.000000 storey-1.3.9/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-16 15:32:21.000000 storey-1.3.9/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-02-16 15:32:21.000000 storey-1.3.9/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-02-16 15:32:21.000000 storey-1.3.9/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-02-16 15:32:21.000000 storey-1.3.9/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-02-16 15:32:21.000000 storey-1.3.9/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50623 2023-02-16 15:32:21.000000 storey-1.3.9/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-16 15:32:21.000000 storey-1.3.9/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26785 2023-02-16 15:32:21.000000 storey-1.3.9/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41331 2023-02-16 15:32:21.000000 storey-1.3.9/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-16 15:32:21.000000 storey-1.3.9/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-02-16 15:32:21.000000 storey-1.3.9/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79845 2023-02-16 15:32:21.000000 storey-1.3.9/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50736 2023-02-16 15:32:21.000000 storey-1.3.9/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-16 15:32:21.000000 storey-1.3.9/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-02-16 15:32:21.000000 storey-1.3.9/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-02-16 15:32:21.000000 storey-1.3.9/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 15:38:36.000000 storey-1.3.9/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 15:38:36.000000 storey-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-16 15:32:21.000000 storey-1.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117320 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-16 15:32:21.000000 storey-1.3.9/tests/test_windowed_store.py
```

### Comparing `storey-1.3.8/LICENSE` & `storey-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/PKG-INFO` & `storey-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.3.8
+Version: 1.3.9
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.3.8/README.md` & `storey-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/__init__.py` & `storey-1.3.9/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/conftest.py` & `storey-1.3.9/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/integration_test_utils.py` & `storey-1.3.9/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_aggregation_integration.py` & `storey-1.3.9/integration/test_aggregation_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4745,7 +4745,85 @@
             "key_column2": 8.6,
             "time": datetime.datetime(2020, 7, 21, 21, 40, tzinfo=datetime.timezone.utc),
         }
     ]
     assert (
         actual == expected_results
     ), f"actual did not match expected. \n actual: {actual} \n expected: {expected_results}"
+
+
+# ML-3378
+def test_huge_fixed_window_starting_at_epoch(setup_teardown_test):
+
+    table = Table(setup_teardown_test.table_name, setup_teardown_test.driver())
+
+    controller = build_flow(
+        [
+            SyncEmitSource(),
+            AggregateByKey(
+                [
+                    FieldAggregator(
+                        "number_of_stuff",
+                        "col1",
+                        ["count"],
+                        FixedWindows(["30000d"]),
+                    )
+                ],
+                table,
+                time_field="time",
+            ),
+            NoSqlTarget(table),
+        ]
+    ).run()
+
+    for i in range(10):
+        data = {"col1": i, "time": setup_teardown_test.test_base_time + timedelta(minutes=25 * i)}
+        controller.emit(data, "tal")
+
+    controller.terminate()
+    controller.await_termination()
+
+    query1_table = Table(setup_teardown_test.table_name, setup_teardown_test.driver())
+    controller = build_flow(
+        [
+            SyncEmitSource(),
+            QueryByKey(["number_of_stuff_count_30000d"], query1_table, key_field=["key"], time_field="time"),
+            Reduce([], lambda acc, x: append_return(acc, x)),
+        ]
+    ).run()
+    controller.emit({"key": "tal", "time": setup_teardown_test.test_base_time}, key=[8.6])
+    controller.terminate()
+    actual = controller.await_termination()
+
+    expected_results = [
+        {
+            "key": "tal",
+            "number_of_stuff_count_30000d": 10,
+            "time": datetime.datetime(2020, 7, 21, 21, 40, tzinfo=datetime.timezone.utc),
+        }
+    ]
+    assert (
+        actual == expected_results
+    ), f"actual did not match expected. \n actual: {actual} \n expected: {expected_results}"
+
+    query2_table = Table(setup_teardown_test.table_name, setup_teardown_test.driver())
+    controller = build_flow(
+        [
+            SyncEmitSource(),
+            QueryByKey(["number_of_stuff_count_1h"], query2_table, key_field=["key"], time_field="time"),
+            Reduce([], lambda acc, x: append_return(acc, x)),
+        ]
+    ).run()
+    controller.emit({"key": "tal", "time": setup_teardown_test.test_base_time}, key=[8.6])
+    controller.terminate()
+    actual = controller.await_termination()
+
+    expected_results = [
+        {
+            "key": "tal",
+            "number_of_stuff_count_1h": 0,
+            "time": datetime.datetime(2020, 7, 21, 21, 40, tzinfo=datetime.timezone.utc),
+        }
+    ]
+    assert (
+        actual == expected_results
+    ), f"actual did not match expected. \n actual: {actual} \n expected: {expected_results}"
```

### Comparing `storey-1.3.8/integration/test_azure_filesystem_integration.py` & `storey-1.3.9/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_filesystems_integration.py` & `storey-1.3.9/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_flow_integration.py` & `storey-1.3.9/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_kafka_integration.py` & `storey-1.3.9/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_redis_specific.py` & `storey-1.3.9/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/integration/test_s3_filesystem_integration.py` & `storey-1.3.9/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/setup.py` & `storey-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/__init__.py` & `storey-1.3.9/storey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = '1.3.8'
+__version__ = '1.3.9'
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.3.8/storey/aggregation_utils.py` & `storey-1.3.9/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/aggregations.py` & `storey-1.3.9/storey/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 _default_emit_policy = EmitEveryEvent()
 
 
 class AggregateByKey(Flow):
     """
     Aggregates the data into the table object provided for later persistence,
-        and outputs an event enriched with the requested aggregation features.
+    and outputs an event enriched with the requested aggregation features.
     Persistence is done via the `NoSqlTarget` step and based on the Cache object persistence settings.
 
     :param aggregates: List of aggregates to apply for each event.
         accepts either list of FieldAggregators or a dictionary describing FieldAggregators.
     :param table: A Table object or name for persistence of aggregations.
         If a table name is provided, it will be looked up in the context object passed in kwargs.
     :param key_field: Key field to aggregate by, accepts either a string representing the key field or a key
@@ -55,15 +55,15 @@
         extracting function. Defaults to the processing time in the event's metadata. (Optional)
     :param emit_policy: Policy indicating when the data will be emitted. Defaults to EmitEveryEvent
     :param augmentation_fn: Function that augments the features into the event's body. Defaults to
         updating a dict. (Optional)
     :param enrich_with: List of attributes names from the associated storage object to be fetched
         and added to every event. (Optional)
     :param aliases: Dictionary specifying aliases for enriched or aggregate columns, of the
-     format `{'col_name': 'new_col_name'}`. (Optional)
+        format `{'col_name': 'new_col_name'}`. (Optional)
     :param time_format: If the value of the time field is of type string, this format will be used to parse it, as
         defined in datetime.strptime(). By default, parsing will follow ISO-8601.
     """
 
     def __init__(
         self,
         aggregates: Union[List[FieldAggregator], List[Dict[str, object]]],
```

### Comparing `storey-1.3.8/storey/dataframe.py` & `storey-1.3.9/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/drivers.py` & `storey-1.3.9/storey/drivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,15 +473,15 @@
 
                 for bucket_start_time, aggregation_values in pending_updates[name].items():
                     # the relevant attribute out of the 2 feature attributes
                     feature_attr = "a" if int(bucket_start_time / bucket.max_window_millis) % 2 == 0 else "b"
 
                     array_time_attribute_name = f"{self._aggregation_time_attribute_prefix}{bucket.name}_{feature_attr}"
 
-                    cached_time = bucket.storage_specific_cache.get(array_time_attribute_name, 0)
+                    cached_time = bucket.storage_specific_cache.get(array_time_attribute_name, -1)
 
                     expected_time = int(bucket_start_time / bucket.max_window_millis) * bucket.max_window_millis
                     expected_time_expr = self._convert_python_obj_to_expression_value(
                         datetime.fromtimestamp(expected_time / 1000)
                     )
                     index_to_update = int((bucket_start_time - expected_time) / bucket.period_millis)
 
@@ -497,15 +497,15 @@
                                     "first_index": index_to_update,
                                     "last_index": index_to_update,
                                     "default_value": aggregation_value.default_value,
                                     "aggregation": aggregation,
                                 }
                         # Possibly initiating the array
                         if cached_time < expected_time:
-                            if not initialized_attributes.get(array_attribute_name, 0) == expected_time:
+                            if not initialized_attributes.get(array_attribute_name, -1) == expected_time:
                                 initialized_attributes[array_attribute_name] = expected_time
                                 expressions.append(
                                     f"{array_attribute_name}=init_array({bucket.total_number_of_buckets},'double',"
                                     f"{aggregation_value.default_value})"
                                 )
                             if array_time_attribute_name not in times_update_expressions:
                                 times_update_expressions[
```

### Comparing `storey-1.3.8/storey/dtypes.py` & `storey-1.3.9/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/flow.py` & `storey-1.3.9/storey/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,14 +629,15 @@
             else:
                 self._filter = False  # clear the flag for future runs
 
 
 class Rename(Flow):
     """
     Rename fields in event body.
+
     :param mapping: Dictionary from old name to new name.
     :param name: Name of this step, as it should appear in logs. Defaults to class name (Rename).
     :type name: string
     """
 
     def __init__(self, mapping: Dict[str, str], **kwargs):
         super().__init__(**kwargs)
@@ -650,14 +651,15 @@
                     del event.body[old_name]
         return await self._do_downstream(event)
 
 
 class ReifyMetadata(Flow):
     """
     Inserts event metadata into the event body.
+
     :param mapping: Dictionary from event attribute name to entry key in the event body (which must be a
         dictionary). Alternatively, an iterable of names may be provided, and these will be used as both
         attribute name and entry key.
     :param name: Name of this step, as it should appear in logs. Defaults to class name (ReifyMetadata).
     :type name: string
     """
 
@@ -675,14 +677,15 @@
                     event.body[attribute_name] = getattr(event, attribute_name)
         return await self._do_downstream(event)
 
 
 class Complete(Flow):
     """
     Completes the AwaitableResult associated with incoming events.
+
     :param name: Name of this step, as it should appear in logs. Defaults to class name (Complete).
     :type name: string
     :param full_event: Whether to complete with an Event object (when True) or only the payload
         (when False). Default to False.
     :type full_event: boolean
     """
```

### Comparing `storey-1.3.8/storey/queue.py` & `storey-1.3.9/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/redis_driver.py` & `storey-1.3.9/storey/redis_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
                         feature_attr = "a" if int(bucket_start_time / bucket.max_window_millis) % 2 == 0 else "b"
 
                         aggr_time_attribute_name = f"{bucket.name}_{feature_attr}"
                         array_time_attribute_key = self._aggregation_time_key(
                             redis_key_prefix, aggr_time_attribute_name
                         )
 
-                        cached_time = bucket.storage_specific_cache.get(array_time_attribute_key, 0)
+                        cached_time = bucket.storage_specific_cache.get(array_time_attribute_key, -1)
 
                         expected_time = int(bucket_start_time / bucket.max_window_millis) * bucket.max_window_millis
                         expected_time_expr = self._convert_python_obj_to_lua_value(
                             datetime.fromtimestamp(expected_time / 1000)
                         )
                         index_to_update = int((bucket_start_time - expected_time) / bucket.period_millis)
 
@@ -303,15 +303,15 @@
                             )
                             list_attribute_key = self._list_key(redis_key_prefix, list_attribute_name)
                             if list_attribute_key not in redis_keys_involved:
                                 redis_keys_involved.append(list_attribute_key)
                             lua_script = f'{lua_script}list_attribute_key="{list_attribute_key}";\n'
 
                             if cached_time < expected_time:
-                                if not initialized_attributes.get(list_attribute_key, 0) == expected_time:
+                                if not initialized_attributes.get(list_attribute_key, -1) == expected_time:
                                     initialized_attributes[list_attribute_key] = expected_time
                                     lua_script = (
                                         f'{lua_script}local t=redis.call("GET","{array_time_attribute_key}");\n'
                                         f'if (type(t)~="boolean" and (tonumber(t) < {expected_time})) then '
                                         f'redis.call("DEL",list_attribute_key); end;\n'
                                     )
                                     default_value = self._convert_python_obj_to_redis_value(
```

### Comparing `storey-1.3.8/storey/sources.py` & `storey-1.3.9/storey/sources.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/sql_driver.py` & `storey-1.3.9/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/__init__.py` & `storey-1.3.9/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/assertion.py` & `storey-1.3.9/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/flatten.py` & `storey-1.3.9/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/foreach.py` & `storey-1.3.9/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/partition.py` & `storey-1.3.9/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/steps/sample.py` & `storey-1.3.9/storey/steps/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 class SampleWindow(Flow):
     """
     Emits a single event in a window of `window_size` events, in accordance with `emit_period` and
     `emit_before_termination`.
 
     :param window_size: The size of the window we want to sample a single event from.
     :param emit_period: What event should this step emit for each `window_size` (default: EmitPeriod.First).
-    Available options:
+        Available options:
         1.1) EmitPeriod.FIRST - will emit the first event in a window `window_size` events.
         1.2) EmitPeriod.LAST - will emit the last event in a window of `window_size` events.
     :param emit_before_termination: On termination signal, should the step emit the last event it seen (default: False).
-    Available options:
+        Available options:
         2.1) True - The last event seen will be emitted downstream.
         2.2) False - The last event seen will NOT be emitted downstream.
     :param key: The key by which events are sampled. By default (None), events are not sampled by key.
         Other options may be:
         Set to '$key' to sample events by the Event.key property.
         set to 'str' key to sample events by Event.body[str].
         set a Callable[[Event], str] to sample events by a custom key extractor.
```

### Comparing `storey-1.3.8/storey/table.py` & `storey-1.3.9/storey/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 import asyncio
 import copy
 import math
 from asyncio import Lock
 from typing import List, Optional
 
+from . import utils
 from .aggregation_utils import (
     get_all_raw_aggregates,
     get_all_raw_aggregates_with_hidden,
     get_implied_aggregates,
     get_virtual_aggregation_func,
     is_raw_aggregate,
 )
@@ -237,16 +238,16 @@
                         window_type = schema_aggr["window_type"]
                         period_secs = str(int(schema_aggr["period_millis"] / 1000)) + "s"
                         if window_type == "SlidingWindow":
                             aggr.windows = SlidingWindows(aggr.windows.windows, period_secs)
                         elif window_type == "FixedWindow":
                             aggr.windows = FixedWindows(aggr.windows.windows)
                             aggr.windows.period_millis = schema_aggr["period_millis"]
-                            aggr.windows.total_number_of_buckets = int(
-                                aggr.windows.max_window_millis / aggr.windows.period_millis
+                            aggr.windows.total_number_of_buckets = max(
+                                int(aggr.windows.max_window_millis / aggr.windows.period_millis), utils.bucketPerWindow
                             )
                         else:
                             raise TypeError(f'"{window_type}" unknown window type')
                 should_update = self._validate_schema_fit_aggregations(self._schema)
 
             if should_update and not self._aggregations_read_only:
                 self._schema = await self._save_schema()
@@ -865,15 +866,15 @@
             window_millis = win[0]
 
             if self.is_fixed_window:
                 aggregated_value.reset()
                 first_bucket_start_time = self.buckets[0].time
                 current_time_bucket_index = int((timestamp - first_bucket_start_time) / self.period_millis)
                 window_indexes = int(window_millis / self.period_millis)
-                start_index = int(current_time_bucket_index / window_indexes) * window_indexes
+                start_index = int(current_time_bucket_index / window_indexes) * window_indexes if window_indexes else 0
                 last_index = start_index + window_indexes - 1
                 if self.fixed_window_type == FixedWindowType.LastClosedWindow:
                     last_index -= window_indexes
                     start_index -= window_indexes
 
                 for bucket_index in range(start_index, last_index + 1):
                     bucket = self.buckets[bucket_index]
```

### Comparing `storey-1.3.8/storey/targets.py` & `storey-1.3.9/storey/targets.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/transformations/__init__.py` & `storey-1.3.9/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/utils.py` & `storey-1.3.9/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey/windowed_store.py` & `storey-1.3.9/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/storey.egg-info/PKG-INFO` & `storey-1.3.9/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.3.8
+Version: 1.3.9
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.3.8/storey.egg-info/SOURCES.txt` & `storey-1.3.9/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/__init__.py` & `storey-1.3.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_aggregate_by_key.py` & `storey-1.3.9/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_aggregate_store.py` & `storey-1.3.9/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_flow.py` & `storey-1.3.9/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_steps.py` & `storey-1.3.9/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_types.py` & `storey-1.3.9/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_v3io.py` & `storey-1.3.9/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.3.8/tests/test_windowed_store.py` & `storey-1.3.9/tests/test_windowed_store.py`

 * *Files identical despite different names*

