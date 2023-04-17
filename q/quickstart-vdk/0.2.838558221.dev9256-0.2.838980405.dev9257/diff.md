# Comparing `tmp/quickstart-vdk-0.2.838558221.dev9256.tar.gz` & `tmp/quickstart-vdk-0.2.838980405.dev9257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.838558221.dev9256.tar", last modified: Sun Apr 16 04:26:45 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.838980405.dev9257.tar", last modified: Mon Apr 17 04:29:27 2023, max compression
```

## Comparing `quickstart-vdk-0.2.838558221.dev9256.tar` & `quickstart-vdk-0.2.838980405.dev9257.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 04:26:45.018055 quickstart-vdk-0.2.838558221.dev9256/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-16 04:26:45.018055 quickstart-vdk-0.2.838558221.dev9256/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-16 04:23:57.000000 quickstart-vdk-0.2.838558221.dev9256/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 04:26:45.018055 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-16 04:26:44.000000 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-16 04:26:44.000000 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 04:26:44.000000 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-16 04:26:44.000000 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-16 04:26:44.000000 quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 04:26:45.018055 quickstart-vdk-0.2.838558221.dev9256/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-16 04:26:34.000000 quickstart-vdk-0.2.838558221.dev9256/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 04:26:45.018055 quickstart-vdk-0.2.838558221.dev9256/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-16 04:23:57.000000 quickstart-vdk-0.2.838558221.dev9256/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:29:27.512861 quickstart-vdk-0.2.838980405.dev9257/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-17 04:29:27.512861 quickstart-vdk-0.2.838980405.dev9257/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-17 04:26:40.000000 quickstart-vdk-0.2.838980405.dev9257/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:29:27.512861 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-17 04:29:27.000000 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-17 04:29:27.000000 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 04:29:27.000000 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-17 04:29:27.000000 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-17 04:29:27.000000 quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 04:29:27.512861 quickstart-vdk-0.2.838980405.dev9257/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-17 04:29:06.000000 quickstart-vdk-0.2.838980405.dev9257/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:29:27.512861 quickstart-vdk-0.2.838980405.dev9257/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-17 04:26:40.000000 quickstart-vdk-0.2.838980405.dev9257/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.838558221.dev9256/PKG-INFO` & `quickstart-vdk-0.2.838980405.dev9257/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.838558221.dev9256
+Version: 0.2.838980405.dev9257
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.838558221.dev9256/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.838980405.dev9257/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.838558221.dev9256
+Version: 0.2.838980405.dev9257
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.838558221.dev9256/setup.py` & `quickstart-vdk-0.2.838980405.dev9257/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.838558221.dev9256"
+__version__ = "0.2.838980405.dev9257"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

