# Comparing `tmp/arvados-cwl-runner-2.6.0rc6.tar.gz` & `tmp/arvados-cwl-runner-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.0rc6.tar", last modified: Wed Apr  5 20:17:19 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.1.tar", last modified: Mon Apr 17 21:06:18 2023, max compression
```

## Comparing `arvados-cwl-runner-2.6.0rc6.tar` & `arvados-cwl-runner-2.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19885 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31804 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44286 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8005 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17931 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1353 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1174 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-05 20:17:19.000000 arvados-cwl-runner-2.6.0rc6/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17280 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2058 2023-04-05 20:17:08.000000 arvados-cwl-runner-2.6.0rc6/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19885 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31804 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44286 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8005 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17931 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1353 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1174 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      174 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:18.000000 arvados-cwl-runner-2.6.1/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17280 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2058 2023-04-17 21:06:09.000000 arvados-cwl-runner-2.6.1/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.0rc6/LICENSE-2.0.txt` & `arvados-cwl-runner-2.6.1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/PKG-INFO` & `arvados-cwl-runner-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.0rc6
+Version: 2.6.1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.6.1/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/arvcontainer.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/context.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/done.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/executor.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/executor.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/http.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/http.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/perf.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/runner.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl/util.py` & `arvados-cwl-runner-2.6.1/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.0rc6
+Version: 2.6.1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.6.1/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/arvados_version.py` & `arvados-cwl-runner-2.6.1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/setup.py` & `arvados-cwl-runner-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/matcher.py` & `arvados-cwl-runner-2.6.1/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_container.py` & `arvados-cwl-runner-2.6.1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_copy_deps.py` & `arvados-cwl-runner-2.6.1/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_fsaccess.py` & `arvados-cwl-runner-2.6.1/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_http.py` & `arvados-cwl-runner-2.6.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_make_output.py` & `arvados-cwl-runner-2.6.1/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_pathmapper.py` & `arvados-cwl-runner-2.6.1/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.6.1/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_submit.py` & `arvados-cwl-runner-2.6.1/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_tq.py` & `arvados-cwl-runner-2.6.1/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_urljoin.py` & `arvados-cwl-runner-2.6.1/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.0rc6/tests/test_util.py` & `arvados-cwl-runner-2.6.1/tests/test_util.py`

 * *Files identical despite different names*

