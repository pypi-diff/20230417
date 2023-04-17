# Comparing `tmp/triad-0.8.5.tar.gz` & `tmp/triad-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.5.tar", last modified: Tue Apr 11 07:37:31 2023, max compression
+gzip compressed data, was "triad-0.8.6.tar", last modified: Mon Apr 17 00:38:41 2023, max compression
```

## Comparing `triad-0.8.5.tar` & `triad-0.8.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 07:36:52.000000 triad-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-11 07:37:31.611298 triad-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-11 07:36:52.000000 triad-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-11 07:37:31.611298 triad-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-11 07:36:52.000000 triad-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.603298 triad-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:36:52.000000 triad-0.8.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.603298 triad-0.8.5/tests/collections/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-11 07:36:52.000000 triad-0.8.5/tests/collections/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/convert_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/tests/utils/dispatcher_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/dispatcher_examples/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_pyarrow_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-11 07:36:52.000000 triad-0.8.5/tests/utils/test_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.607298 triad-0.8.5/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-11 07:36:52.000000 triad-0.8.5/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-11 07:36:52.000000 triad-0.8.5/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 07:36:52.000000 triad-0.8.5/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 07:36:52.000000 triad-0.8.5/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-11 07:36:52.000000 triad-0.8.5/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 07:37:31.000000 triad-0.8.5/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:37:31.611298 triad-0.8.5/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 07:36:52.000000 triad-0.8.5/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 00:38:01.000000 triad-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-17 00:38:41.933053 triad-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-17 00:38:01.000000 triad-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 00:38:41.933053 triad-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 00:38:01.000000 triad-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:01.000000 triad-0.8.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-04-17 00:38:01.000000 triad-0.8.6/tests/collections/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/convert_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.929053 triad-0.8.6/tests/utils/dispatcher_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/dispatcher_examples/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_pyarrow_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 00:38:01.000000 triad-0.8.6/tests/utils/test_threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 00:38:01.000000 triad-0.8.6/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-17 00:38:01.000000 triad-0.8.6/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 00:38:01.000000 triad-0.8.6/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-17 00:38:01.000000 triad-0.8.6/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24206 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-17 00:38:01.000000 triad-0.8.6/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 00:38:41.000000 triad-0.8.6/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:38:41.933053 triad-0.8.6/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 00:38:01.000000 triad-0.8.6/triad_version/__init__.py
```

### Comparing `triad-0.8.5/LICENSE` & `triad-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/PKG-INFO` & `triad-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.5
+Version: 0.8.6
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.6
+        
+        * Fixed timestamp conversion for pandas 2.0
+        
         ### 0.8.5
         
         * Ensure pandas 2.0 compatibility
         * Improve `to_schema` in `PandasUtils`
         
         ### 0.8.4
```

### Comparing `triad-0.8.5/README.md` & `triad-0.8.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.8.6
+
+* Fixed timestamp conversion for pandas 2.0
+
 ### 0.8.5
 
 * Ensure pandas 2.0 compatibility
 * Improve `to_schema` in `PandasUtils`
 
 ### 0.8.4
```

### Comparing `triad-0.8.5/setup.py` & `triad-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/collections/test_dict.py` & `triad-0.8.6/tests/collections/test_dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/collections/test_fs.py` & `triad-0.8.6/tests/collections/test_fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/collections/test_function_wrapper.py` & `triad-0.8.6/tests/collections/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/collections/test_schema.py` & `triad-0.8.6/tests/collections/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_assertion.py` & `triad-0.8.6/tests/utils/test_assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_class_extension.py` & `triad-0.8.6/tests/utils/test_class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_convert.py` & `triad-0.8.6/tests/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_dispatcher.py` & `triad-0.8.6/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_hash.py` & `triad-0.8.6/tests/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_iter.py` & `triad-0.8.6/tests/utils/test_iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_pandas_like.py` & `triad-0.8.6/tests/utils/test_pandas_like.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,14 +181,58 @@
     assert [[1, True], [2, False]] == arr
 
     df = DF([[1, "trUe"], [2, "False"], [3, None]], "b:int,c:bool", True)
     arr = df.as_array(type_safe=True)
     assert [[1, True], [2, False], [3, None]] == arr
 
 
+def test_timestamp_enforce():
+    df = DF(
+        [
+            [1, pd.Timestamp("2020-01-02 00:00:00", tz="UTC")],
+            [2, pd.Timestamp("2020-01-03 00:00:00", tz="UTC")],
+        ],
+        "b:int,c:datetime",
+        True,
+    )
+    arr = df.as_array(type_safe=True)
+    assert [
+        [1, pd.Timestamp("2020-01-02 00:00:00")],
+        [2, pd.Timestamp("2020-01-03 00:00:00")],
+    ] == arr
+
+    df = DF(
+        [
+            [1, pd.Timestamp("2020-01-02 00:00:00")],
+            [2, pd.Timestamp("2020-01-03 00:00:00")],
+        ],
+        "b:int,c:timestamp(ns, UTC)",
+        True,
+    )
+    arr = df.as_array(type_safe=True)
+    assert [
+        [1, pd.Timestamp("2020-01-02 00:00:00", tz="UTC")],
+        [2, pd.Timestamp("2020-01-03 00:00:00", tz="UTC")],
+    ] == arr
+
+    df = DF(
+        [
+            [1, pd.Timestamp("2020-01-02 00:00:00", tz="US/Pacific")],
+            [2, pd.Timestamp("2020-01-03 00:00:00", tz="US/Pacific")],
+        ],
+        "b:int,c:timestamp(ns, UTC)",
+        True,
+    )
+    arr = df.as_array(type_safe=True)
+    assert [
+        [1, pd.Timestamp("2020-01-02 08:00:00", tz="UTC")],
+        [2, pd.Timestamp("2020-01-03 08:00:00", tz="UTC")],
+    ] == arr
+
+
 def test_fillna_default():
     df = pd.DataFrame([[1.0], [None]], columns=["x"])
     s = PD_UTILS.fillna_default(df["x"])
     assert [1.0, 0.0] == s.tolist()
 
     df = pd.DataFrame([["a"], [None]], columns=["x"])
     s = PD_UTILS.fillna_default(df["x"])
```

### Comparing `triad-0.8.5/tests/utils/test_pyarrow.py` & `triad-0.8.6/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_pyarrow_convert.py` & `triad-0.8.6/tests/utils/test_pyarrow_convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_rename.py` & `triad-0.8.6/tests/utils/test_rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_schema.py` & `triad-0.8.6/tests/utils/test_schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_string.py` & `triad-0.8.6/tests/utils/test_string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/tests/utils/test_threading.py` & `triad-0.8.6/tests/utils/test_threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/collections/dict.py` & `triad-0.8.6/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/collections/fs.py` & `triad-0.8.6/triad/collections/fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/collections/function_wrapper.py` & `triad-0.8.6/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/collections/schema.py` & `triad-0.8.6/triad/collections/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/assertion.py` & `triad-0.8.6/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/class_extension.py` & `triad-0.8.6/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/convert.py` & `triad-0.8.6/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/dispatcher.py` & `triad-0.8.6/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/entry_points.py` & `triad-0.8.6/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/hash.py` & `triad-0.8.6/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/iter.py` & `triad-0.8.6/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/json.py` & `triad-0.8.6/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/pandas_like.py` & `triad-0.8.6/triad/utils/pandas_like.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,15 +178,28 @@
                 s = (
                     s.fillna(0)
                     .astype(int)
                     .astype(to_single_pandas_dtype(v.type))
                     .mask(ns, None)
                 )
             elif not pa.types.is_struct(v.type) and not pa.types.is_list(v.type):
-                s = s.astype(to_single_pandas_dtype(v.type))
+                from_t = s.dtype
+                to_t = to_single_pandas_dtype(v.type)
+                if from_t != to_t:
+                    if pd.api.types.is_datetime64_any_dtype(
+                        from_t
+                    ) and pd.api.types.is_datetime64_any_dtype(to_t):
+                        from_tz = _get_tz(from_t)
+                        to_tz = _get_tz(to_t)
+                        if from_tz is None or to_tz is None:
+                            s = s.dt.tz_localize(to_tz)
+                        else:
+                            s = s.dt.tz_convert(to_tz)
+                    else:
+                        s = s.astype(to_single_pandas_dtype(v.type))
             data[v.name] = s
         return pd.DataFrame(data)
 
     def safe_groupby_apply(
         self,
         df: T,
         cols: List[str],
@@ -269,7 +282,13 @@
 class PandasUtils(PandasLikeUtils[pd.DataFrame]):
     """A collection of pandas utils"""
 
     pass
 
 
 PD_UTILS = PandasUtils()
+
+
+def _get_tz(ts: Any) -> Any:
+    if hasattr(ts, "tz"):
+        return ts.tz
+    return None
```

### Comparing `triad-0.8.5/triad/utils/pyarrow.py` & `triad-0.8.6/triad/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/rename.py` & `triad-0.8.6/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/schema.py` & `triad-0.8.6/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/string.py` & `triad-0.8.6/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad/utils/threading.py` & `triad-0.8.6/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.5/triad.egg-info/PKG-INFO` & `triad-0.8.6/triad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.5
+Version: 0.8.6
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.8.6
+        
+        * Fixed timestamp conversion for pandas 2.0
+        
         ### 0.8.5
         
         * Ensure pandas 2.0 compatibility
         * Improve `to_schema` in `PandasUtils`
         
         ### 0.8.4
```

### Comparing `triad-0.8.5/triad.egg-info/SOURCES.txt` & `triad-0.8.6/triad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

