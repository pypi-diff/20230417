# Comparing `tmp/google-cloud-build-3.9.2.tar.gz` & `tmp/google-cloud-build-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-build-3.9.2.tar", last modified: Tue Oct  4 00:29:15 2022, max compression
+gzip compressed data, was "google-cloud-build-3.9.3.tar", last modified: Mon Oct 10 16:28:30 2022, max compression
```

## Comparing `google-cloud-build-3.9.2.tar` & `google-cloud-build-3.9.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4633 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3769 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.340664 google-cloud-build-3.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.340664 google-cloud-build-3.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.340664 google-cloud-build-3.9.2/google/cloud/devtools/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild/
--rw-rw-r--   0 root         (0)     1003     7109 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild/__init__.py
--rw-rw-r--   0 root         (0)     1003       79 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/
--rw-rw-r--   0 root         (0)     1003     4916 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5071 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/gapic_metadata.json
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/proto/
--rw-rw-r--   0 root         (0)     1003    55623 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/proto/cloudbuild.proto
--rw-rw-r--   0 root         (0)     1003       79 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/
--rw-rw-r--   0 root         (0)     1003      753 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/__init__.py
--rw-rw-r--   0 root         (0)     1003   109648 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/async_client.py
--rw-rw-r--   0 root         (0)     1003   122628 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/client.py
--rw-rw-r--   0 root         (0)     1003    16025 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/
--rw-rw-r--   0 root         (0)     1003     1158 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16826 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34027 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34819 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.344664 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/types/
--rw-rw-r--   0 root         (0)     1003     3357 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    93512 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/types/cloudbuild.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/google_cloud_build.egg-info/
--rw-r--r--   0 root         (0)     1003     4633 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1608 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      160 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 00:29:15.000000 google-cloud-build-3.9.2/google_cloud_build.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/scripts/
--rw-rw-r--   0 root         (0)     1003     7189 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/scripts/fixup_cloudbuild_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2773 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:29:15.348665 google-cloud-build-3.9.2/tests/unit/gapic/cloudbuild_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/tests/unit/gapic/cloudbuild_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   240153 2022-10-04 00:26:37.000000 google-cloud-build-3.9.2/tests/unit/gapic/cloudbuild_v1/test_cloud_build.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.611552 google-cloud-build-3.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4633 2022-10-10 16:28:30.611552 google-cloud-build-3.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3769 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.599550 google-cloud-build-3.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.599550 google-cloud-build-3.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.599550 google-cloud-build-3.9.3/google/cloud/devtools/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.603551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild/
+-rw-rw-r--   0 root         (0)     1003     7109 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild/__init__.py
+-rw-rw-r--   0 root         (0)     1003       79 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.603551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/
+-rw-rw-r--   0 root         (0)     1003     4916 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5071 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/gapic_metadata.json
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.603551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/proto/
+-rw-rw-r--   0 root         (0)     1003    55623 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/proto/cloudbuild.proto
+-rw-rw-r--   0 root         (0)     1003       79 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.603551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.603551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/
+-rw-rw-r--   0 root         (0)     1003      753 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/__init__.py
+-rw-rw-r--   0 root         (0)     1003   109648 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/async_client.py
+-rw-rw-r--   0 root         (0)     1003   122628 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/client.py
+-rw-rw-r--   0 root         (0)     1003    16025 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/
+-rw-rw-r--   0 root         (0)     1003     1158 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16826 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34027 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34819 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3357 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    93512 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/types/cloudbuild.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/google_cloud_build.egg-info/
+-rw-r--r--   0 root         (0)     1003     4633 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1608 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:28:30.000000 google-cloud-build-3.9.3/google_cloud_build.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/scripts/
+-rw-rw-r--   0 root         (0)     1003     7189 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/scripts/fixup_cloudbuild_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:28:30.611552 google-cloud-build-3.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2842 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:28:30.607551 google-cloud-build-3.9.3/tests/unit/gapic/cloudbuild_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/tests/unit/gapic/cloudbuild_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   240153 2022-10-10 16:25:43.000000 google-cloud-build-3.9.3/tests/unit/gapic/cloudbuild_v1/test_cloud_build.py
```

### Comparing `google-cloud-build-3.9.2/LICENSE` & `google-cloud-build-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/MANIFEST.in` & `google-cloud-build-3.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/PKG-INFO` & `google-cloud-build-3.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-build
-Version: 3.9.2
+Version: 3.9.3
 Summary: Google Cloud Build API client library
 Home-page: https://github.com/googleapis/python-cloudbuild
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-build-3.9.2/README.rst` & `google-cloud-build-3.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/gapic_metadata.json` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/proto/cloudbuild.proto` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/proto/cloudbuild.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/async_client.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/client.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/pagers.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/base.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc_asyncio.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/services/cloud_build/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/types/__init__.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google/cloud/devtools/cloudbuild_v1/types/cloudbuild.py` & `google-cloud-build-3.9.3/google/cloud/devtools/cloudbuild_v1/types/cloudbuild.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/google_cloud_build.egg-info/PKG-INFO` & `google-cloud-build-3.9.3/google_cloud_build.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-build
-Version: 3.9.2
+Version: 3.9.3
 Summary: Google Cloud Build API client library
 Home-page: https://github.com/googleapis/python-cloudbuild
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-build-3.9.2/google_cloud_build.egg-info/SOURCES.txt` & `google-cloud-build-3.9.3/google_cloud_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/scripts/fixup_cloudbuild_v1_keywords.py` & `google-cloud-build-3.9.3/scripts/fixup_cloudbuild_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/setup.py` & `google-cloud-build-3.9.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-build"
 description = "Google Cloud Build API client library"
-version = "3.9.2"
+version = "3.9.3"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 
 extras = {"libcst": "libcst >= 0.2.5"}
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
```

### Comparing `google-cloud-build-3.9.2/tests/__init__.py` & `google-cloud-build-3.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/tests/unit/__init__.py` & `google-cloud-build-3.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/tests/unit/gapic/__init__.py` & `google-cloud-build-3.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/tests/unit/gapic/cloudbuild_v1/__init__.py` & `google-cloud-build-3.9.3/tests/unit/gapic/cloudbuild_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-build-3.9.2/tests/unit/gapic/cloudbuild_v1/test_cloud_build.py` & `google-cloud-build-3.9.3/tests/unit/gapic/cloudbuild_v1/test_cloud_build.py`

 * *Files identical despite different names*

