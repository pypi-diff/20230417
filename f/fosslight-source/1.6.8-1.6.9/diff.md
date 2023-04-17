# Comparing `tmp/fosslight_source-1.6.8.tar.gz` & `tmp/fosslight_source-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fosslight_source-1.6.8.tar", last modified: Fri Mar 11 05:37:53 2022, max compression
+gzip compressed data, was "dist/fosslight_source-1.6.9.tar", last modified: Wed Apr  6 10:10:58 2022, max compression
```

## Comparing `fosslight_source-1.6.8.tar` & `fosslight_source-1.6.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       59 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2322 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       82 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1805 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/src/fosslight_source/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/_help.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1613 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/_license_matched.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6417 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/_parsing_scancode_file_item.py
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/_parsing_scanoss_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     5759 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/_scan_item.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     8563 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     6261 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/convert_scancode.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5920 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/run_scancode.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     3534 2022-03-11 05:37:35.000000 fosslight_source-1.6.8/src/fosslight_source/run_scanoss.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-11 05:37:53.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      700 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      231 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      167 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-03-11 05:37:52.000000 fosslight_source-1.6.8/src/fosslight_source.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2322 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1805 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source/
+-rwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2484 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/_help.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1613 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/_license_matched.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6417 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/_parsing_scancode_file_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2190 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/_parsing_scanoss_file.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5759 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/_scan_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8563 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     6261 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/convert_scancode.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     5920 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/run_scancode.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     3534 2022-04-06 10:10:49.000000 fosslight_source-1.6.9/src/fosslight_source/run_scanoss.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3335 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      700 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      231 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2022-04-06 10:10:58.000000 fosslight_source-1.6.9/src/fosslight_source.egg-info/top_level.txt
```

### Comparing `fosslight_source-1.6.8/LICENSE` & `fosslight_source-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/PKG-INFO` & `fosslight_source-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_source
-Version: 1.6.8
+Version: 1.6.9
 Summary: FOSSLight Source Scanner
 Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_source_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight_source Version: 1.6.8 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight_source Version: 1.6.9 Summary: FOSSLight
 Source Scanner Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics License: Apache-2.0 Download-URL: https://github.com/
 fosslight/fosslight_source_scanner Description:
                                                                        [Korean]
 # FOSSLight Source Scanner [FOSSLight Source Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_source] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_source-1.6.8/README.md` & `fosslight_source-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/setup.py` & `fosslight_source-1.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_source',
-        version='1.6.8',
+        version='1.6.9',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Source Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_source-1.6.8/src/fosslight_source/_help.py` & `fosslight_source-1.6.9/src/fosslight_source/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/_license_matched.py` & `fosslight_source-1.6.9/src/fosslight_source/_license_matched.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/_parsing_scancode_file_item.py` & `fosslight_source-1.6.9/src/fosslight_source/_parsing_scancode_file_item.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/_parsing_scanoss_file.py` & `fosslight_source-1.6.9/src/fosslight_source/_parsing_scanoss_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/_scan_item.py` & `fosslight_source-1.6.9/src/fosslight_source/_scan_item.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/cli.py` & `fosslight_source-1.6.9/src/fosslight_source/cli.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/convert_scancode.py` & `fosslight_source-1.6.9/src/fosslight_source/convert_scancode.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/run_scancode.py` & `fosslight_source-1.6.9/src/fosslight_source/run_scancode.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source/run_scanoss.py` & `fosslight_source-1.6.9/src/fosslight_source/run_scanoss.py`

 * *Files identical despite different names*

### Comparing `fosslight_source-1.6.8/src/fosslight_source.egg-info/PKG-INFO` & `fosslight_source-1.6.9/src/fosslight_source.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-source
-Version: 1.6.8
+Version: 1.6.9
 Summary: FOSSLight Source Scanner
 Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_source_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fosslight-source Version: 1.6.8 Summary: FOSSLight
+Metadata-Version: 2.1 Name: fosslight-source Version: 1.6.9 Summary: FOSSLight
 Source Scanner Home-page: https://github.com/fosslight/fosslight_source_scanner
 Author: LG Electronics License: Apache-2.0 Download-URL: https://github.com/
 fosslight/fosslight_source_scanner Description:
                                                                        [Korean]
 # FOSSLight Source Scanner [FOSSLight Source Scanner is released under the
 Apache-2.0 License.] [Current python package version.] [https://img.shields.io/
 pypi/pyversions/fosslight_source] [![REUSE status](https://api.reuse.software/
```

### Comparing `fosslight_source-1.6.8/src/fosslight_source.egg-info/SOURCES.txt` & `fosslight_source-1.6.9/src/fosslight_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

