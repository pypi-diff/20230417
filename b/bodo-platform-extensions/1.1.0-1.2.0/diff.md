# Comparing `tmp/bodo_platform_extensions-1.1.0.tar.gz` & `tmp/bodo_platform_extensions-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodo_platform_extensions-1.1.0.tar", last modified: Thu Nov  3 18:29:58 2022, max compression
+gzip compressed data, was "bodo_platform_extensions-1.2.0.tar", last modified: Mon Apr 17 17:35:52 2023, max compression
```

## Comparing `bodo_platform_extensions-1.1.0.tar` & `bodo_platform_extensions-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/bodo_platform_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/bodo_platform_extensions/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4908 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/adls_setup_magic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/hostfile_update_magic.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/magics_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/package_installation_magics.py
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/parallel_shell_magic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/platform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-11-03 18:29:58.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-03 18:29:58.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 18:29:58.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-03 18:29:58.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-03 18:29:58.000000 bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-03 18:29:58.941097 bodo_platform_extensions-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-11-03 18:27:54.000000 bodo_platform_extensions-1.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/bodo_platform_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/bodo_platform_extensions/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/adls_setup_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/hostfile_update_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/magics_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/package_installation_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/parallel_shell_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/platform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-17 17:35:52.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 17:35:52.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:35:52.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 17:35:52.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 17:35:52.000000 bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:35:52.105434 bodo_platform_extensions-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/tests/test_magics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-04-17 17:33:45.000000 bodo_platform_extensions-1.2.0/versioneer.py
```

### Comparing `bodo_platform_extensions-1.1.0/LICENSE` & `bodo_platform_extensions-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/PKG-INFO` & `bodo_platform_extensions-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo_platform_extensions
-Version: 1.1.0
+Version: 1.2.0
 Summary: IPython magic extensions for the Bodo Cloud Platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-extensions
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Description: # bodo-platform-extensions
         List of packages installations to extend the Bodo platform experience.
```

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/__init__.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/adls_setup_magic.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/adls_setup_magic.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/helper.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/helper.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/hostfile_update_magic.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/hostfile_update_magic.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/package_installation_magics.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/package_installation_magics.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/parallel_shell_magic.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/parallel_shell_magic.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/platform_utils.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/platform_utils.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql/transform.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql/transform.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions/sql_magic.py` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions/sql_magic.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/bodo_platform_extensions.egg-info/PKG-INFO` & `bodo_platform_extensions-1.2.0/bodo_platform_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo-platform-extensions
-Version: 1.1.0
+Version: 1.2.0
 Summary: IPython magic extensions for the Bodo Cloud Platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-extensions
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Description: # bodo-platform-extensions
         List of packages installations to extend the Bodo platform experience.
```

### Comparing `bodo_platform_extensions-1.1.0/setup.py` & `bodo_platform_extensions-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_extensions-1.1.0/versioneer.py` & `bodo_platform_extensions-1.2.0/versioneer.py`

 * *Files identical despite different names*

