# Comparing `tmp/speechtotext-python-0.3.3.tar.gz` & `tmp/speechtotext-python-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.3.tar", last modified: Mon Apr 17 13:42:26 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.4.tar", last modified: Mon Apr 17 15:30:09 2023, max compression
```

## Comparing `speechtotext-python-0.3.3.tar` & `speechtotext-python-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:42:26.265459 speechtotext-python-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 13:42:26.265459 speechtotext-python-0.3.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      357 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:42:26.265459 speechtotext-python-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4283 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:42:26.265459 speechtotext-python-0.3.3/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3458 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6399 2023-04-17 13:35:48.000000 speechtotext-python-0.3.3/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:42:26.265459 speechtotext-python-0.3.3/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 13:42:26.000000 speechtotext-python-0.3.3/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-17 13:42:26.000000 speechtotext-python-0.3.3/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:42:26.000000 speechtotext-python-0.3.3/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 13:42:26.000000 speechtotext-python-0.3.3/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 13:42:26.000000 speechtotext-python-0.3.3/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4066 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3458 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6399 2023-04-17 15:24:35.000000 speechtotext-python-0.3.4/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:30:09.221864 speechtotext-python-0.3.4/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 15:30:09.000000 speechtotext-python-0.3.4/speechtotext_python.egg-info/top_level.txt
```

### Comparing `speechtotext-python-0.3.3/LICENSE` & `speechtotext-python-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.3/speechtotext/datasets.py` & `speechtotext-python-0.3.4/speechtotext/datasets.py`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.3/speechtotext/functions.py` & `speechtotext-python-0.3.4/speechtotext/functions.py`

 * *Files identical despite different names*

