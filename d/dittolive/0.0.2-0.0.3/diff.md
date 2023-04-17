# Comparing `tmp/dittolive-0.0.2.tar.gz` & `tmp/dittolive-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dittolive-0.0.2.tar", last modified: Fri Apr 14 15:36:26 2023, max compression
+gzip compressed data, was "dittolive-0.0.3.tar", last modified: Mon Apr 17 09:35:35 2023, max compression
```

## Comparing `dittolive-0.0.2.tar` & `dittolive-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.720179 dittolive-0.0.2/
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1815 2023-04-14 13:25:48.000000 dittolive-0.0.2/LICENSE.md
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2472 2023-04-14 15:36:26.720179 dittolive-0.0.2/PKG-INFO
--rw-r--r--   0 ronan     (1000) ronan     (1000)       29 2023-04-14 13:25:48.000000 dittolive-0.0.2/README.md
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1054 2023-04-14 15:36:17.000000 dittolive-0.0.2/pyproject.toml
--rw-r--r--   0 ronan     (1000) ronan     (1000)       38 2023-04-14 15:36:26.720179 dittolive-0.0.2/setup.cfg
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/dittolive/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      189 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/__init__.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      422 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/__observer.py
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/dittolive/_transports/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      136 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/_transports/__init__.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2168 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/_transports/sync_state.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2287 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/_transports/transport_config.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     3970 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/_transports/transport_sync.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2837 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/_utils.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     6771 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/ditto.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1120 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/exceptions.py
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/dittolive/identity/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      265 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/identity/__init__.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2032 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/identity/identity.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1261 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/identity/offline_playground.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1905 2023-04-14 13:25:48.000000 dittolive-0.0.2/src/dittolive/identity/online_playground.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      158 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/log.py
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/dittolive/store/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      116 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/__init__.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      695 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/__transaction.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     3220 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/abstract_document_path.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     5537 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/collection.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1451 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/document.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1114 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/document_id.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1056 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/document_path.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     5220 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/live_query.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1103 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/mutable_document.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2857 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/mutable_document_path.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     5684 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/pending_id_specific_operation.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1039 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/store.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2200 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/subscription.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      350 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/types.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1065 2023-04-13 15:26:57.000000 dittolive-0.0.2/src/dittolive/store/update_result.py
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.710179 dittolive-0.0.2/src/dittolive.egg-info/
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2472 2023-04-14 15:36:26.000000 dittolive-0.0.2/src/dittolive.egg-info/PKG-INFO
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1447 2023-04-14 15:36:26.000000 dittolive-0.0.2/src/dittolive.egg-info/SOURCES.txt
--rw-r--r--   0 ronan     (1000) ronan     (1000)        1 2023-04-14 15:36:26.000000 dittolive-0.0.2/src/dittolive.egg-info/dependency_links.txt
--rw-r--r--   0 ronan     (1000) ronan     (1000)       29 2023-04-14 15:36:26.000000 dittolive-0.0.2/src/dittolive.egg-info/requires.txt
--rw-r--r--   0 ronan     (1000) ronan     (1000)       10 2023-04-14 15:36:26.000000 dittolive-0.0.2/src/dittolive.egg-info/top_level.txt
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:36:26.720179 dittolive-0.0.2/tests/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      287 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/collection_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      606 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/ditto_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     3300 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/document_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      960 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/observer_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     4180 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/pending_id_specific_operation_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)      401 2023-04-13 15:26:57.000000 dittolive-0.0.2/tests/store_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1585 2023-04-14 13:25:48.000000 dittolive-0.0.2/tests/transports_test.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1772 2023-04-14 13:25:48.000000 dittolive-0.0.2/tests/utils.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1815 2023-04-14 13:25:48.000000 dittolive-0.0.3/LICENSE.md
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2472 2023-04-17 09:35:35.144543 dittolive-0.0.3/PKG-INFO
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       29 2023-04-14 13:25:48.000000 dittolive-0.0.3/README.md
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1055 2023-04-17 09:35:19.000000 dittolive-0.0.3/pyproject.toml
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       38 2023-04-17 09:35:35.144543 dittolive-0.0.3/setup.cfg
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/dittolive/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      189 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/__init__.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      422 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/__observer.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/dittolive/_transports/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      136 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/_transports/__init__.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2168 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/_transports/sync_state.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2287 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/_transports/transport_config.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     3970 2023-04-17 06:48:58.000000 dittolive-0.0.3/src/dittolive/_transports/transport_sync.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2837 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/_utils.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     6771 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/ditto.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1120 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/exceptions.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/dittolive/identity/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      265 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/identity/__init__.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2032 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/identity/identity.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1261 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/identity/offline_playground.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1905 2023-04-14 13:25:48.000000 dittolive-0.0.3/src/dittolive/identity/online_playground.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      158 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/log.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/dittolive/store/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      116 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/__init__.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      695 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/__transaction.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     3220 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/abstract_document_path.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     5537 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/collection.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1451 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/document.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1114 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/document_id.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1056 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/document_path.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     5220 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/live_query.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1103 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/mutable_document.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2857 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/mutable_document_path.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     5684 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/pending_id_specific_operation.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1039 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/store.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2200 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/subscription.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      350 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/types.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1065 2023-04-13 15:26:57.000000 dittolive-0.0.3/src/dittolive/store/update_result.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/src/dittolive.egg-info/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2472 2023-04-17 09:35:34.000000 dittolive-0.0.3/src/dittolive.egg-info/PKG-INFO
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1447 2023-04-17 09:35:35.000000 dittolive-0.0.3/src/dittolive.egg-info/SOURCES.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)        1 2023-04-17 09:35:34.000000 dittolive-0.0.3/src/dittolive.egg-info/dependency_links.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       29 2023-04-17 09:35:34.000000 dittolive-0.0.3/src/dittolive.egg-info/requires.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       10 2023-04-17 09:35:34.000000 dittolive-0.0.3/src/dittolive.egg-info/top_level.txt
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:35:35.144543 dittolive-0.0.3/tests/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      287 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/collection_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      606 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/ditto_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     3300 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/document_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      960 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/observer_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     4180 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/pending_id_specific_operation_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      401 2023-04-13 15:26:57.000000 dittolive-0.0.3/tests/store_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1585 2023-04-14 13:25:48.000000 dittolive-0.0.3/tests/transports_test.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1772 2023-04-14 13:25:48.000000 dittolive-0.0.3/tests/utils.py
```

### Comparing `dittolive-0.0.2/LICENSE.md` & `dittolive-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/PKG-INFO` & `dittolive-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dittolive
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ditto Python SDK.
 Author-email: Ditto Engineering Team <engineering@ditto.live>
 License: Ditto Binary License
         
         Copyright © 2021 DittoLive Incorporated. All rights reserved.
         
         NOTICE: All information contained herein is, and remains the property of
```

### Comparing `dittolive-0.0.2/pyproject.toml` & `dittolive-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
-requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.5.0", "cffi>=1.0.1", "ruff"]
+requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.5.0", "cffi>=1.15.1", "ruff"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dittolive"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 description = "Ditto Python SDK."
 authors = [{name="Ditto Engineering Team", email="engineering@ditto.live"}]
 #CHECKME
 keywords = ["database", "P2P", "CRDT"]
 # dependencies
 dependencies = [
-    "dittoffi == 0.0.2",
+    "dittoffi == 0.0.3",
     "cbor2 == 5.4.6",
 ]
 
 [project.license]
 type = "Proprietary"
 file = "LICENSE.md"
```

### Comparing `dittolive-0.0.2/src/dittolive/_transports/sync_state.py` & `dittolive-0.0.3/src/dittolive/_transports/sync_state.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/_transports/transport_config.py` & `dittolive-0.0.3/src/dittolive/_transports/transport_config.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/_transports/transport_sync.py` & `dittolive-0.0.3/src/dittolive/_transports/transport_sync.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/_utils.py` & `dittolive-0.0.3/src/dittolive/_utils.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/ditto.py` & `dittolive-0.0.3/src/dittolive/ditto.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/exceptions.py` & `dittolive-0.0.3/src/dittolive/exceptions.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/identity/identity.py` & `dittolive-0.0.3/src/dittolive/identity/identity.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/identity/offline_playground.py` & `dittolive-0.0.3/src/dittolive/identity/offline_playground.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/identity/online_playground.py` & `dittolive-0.0.3/src/dittolive/identity/online_playground.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/__transaction.py` & `dittolive-0.0.3/src/dittolive/store/__transaction.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/abstract_document_path.py` & `dittolive-0.0.3/src/dittolive/store/abstract_document_path.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/collection.py` & `dittolive-0.0.3/src/dittolive/store/collection.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/document.py` & `dittolive-0.0.3/src/dittolive/store/document.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/document_id.py` & `dittolive-0.0.3/src/dittolive/store/document_id.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/document_path.py` & `dittolive-0.0.3/src/dittolive/store/document_path.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/live_query.py` & `dittolive-0.0.3/src/dittolive/store/live_query.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/mutable_document.py` & `dittolive-0.0.3/src/dittolive/store/mutable_document.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/mutable_document_path.py` & `dittolive-0.0.3/src/dittolive/store/mutable_document_path.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/pending_id_specific_operation.py` & `dittolive-0.0.3/src/dittolive/store/pending_id_specific_operation.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/store.py` & `dittolive-0.0.3/src/dittolive/store/store.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/subscription.py` & `dittolive-0.0.3/src/dittolive/store/subscription.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive/store/update_result.py` & `dittolive-0.0.3/src/dittolive/store/update_result.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/src/dittolive.egg-info/PKG-INFO` & `dittolive-0.0.3/src/dittolive.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dittolive
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ditto Python SDK.
 Author-email: Ditto Engineering Team <engineering@ditto.live>
 License: Ditto Binary License
         
         Copyright © 2021 DittoLive Incorporated. All rights reserved.
         
         NOTICE: All information contained herein is, and remains the property of
```

### Comparing `dittolive-0.0.2/src/dittolive.egg-info/SOURCES.txt` & `dittolive-0.0.3/src/dittolive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/ditto_test.py` & `dittolive-0.0.3/tests/ditto_test.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/document_test.py` & `dittolive-0.0.3/tests/document_test.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/observer_test.py` & `dittolive-0.0.3/tests/observer_test.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/pending_id_specific_operation_test.py` & `dittolive-0.0.3/tests/pending_id_specific_operation_test.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/transports_test.py` & `dittolive-0.0.3/tests/transports_test.py`

 * *Files identical despite different names*

### Comparing `dittolive-0.0.2/tests/utils.py` & `dittolive-0.0.3/tests/utils.py`

 * *Files identical despite different names*

