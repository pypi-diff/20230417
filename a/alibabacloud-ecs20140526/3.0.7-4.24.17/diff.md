# Comparing `tmp/alibabacloud_ecs20140526-3.0.7.tar.gz` & `tmp/alibabacloud_ecs20140526-4.24.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecs20140526-3.0.7.tar", last modified: Mon Apr 17 12:17:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ecs20140526-4.24.17.tar", last modified: Wed Apr 13 08:30:34 2022, max compression
```

## Comparing `alibabacloud_ecs20140526-3.0.7.tar` & `alibabacloud_ecs20140526-4.24.17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2348 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2660185 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526/client.py
--rw-r--r--   0 root         (0) root         (0)  4191334 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2348 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2023-04-17 12:17:23.000000 alibabacloud_ecs20140526-3.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/
+-rw-r--r--   0 root         (0) root         (0)      533 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2350 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1689159 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526/client.py
+-rw-r--r--   0 root         (0) root         (0)  2958925 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2350 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2630 2022-04-13 08:30:34.000000 alibabacloud_ecs20140526-4.24.17/setup.py
```

### Comparing `alibabacloud_ecs20140526-3.0.7/LICENSE` & `alibabacloud_ecs20140526-4.24.17/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecs20140526-3.0.7/PKG-INFO` & `alibabacloud_ecs20140526-4.24.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ecs20140526
-Version: 3.0.7
+Version: 4.24.17
 Summary: Alibaba Cloud Elastic Compute Service (20140526) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecs20140526-3.0.7/README-CN.md` & `alibabacloud_ecs20140526-4.24.17/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecs20140526-3.0.7/README.md` & `alibabacloud_ecs20140526-4.24.17/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecs20140526-3.0.7/alibabacloud_ecs20140526.egg-info/PKG-INFO` & `alibabacloud_ecs20140526-4.24.17/alibabacloud_ecs20140526.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ecs20140526
-Version: 3.0.7
+Version: 4.24.17
 Summary: Alibaba Cloud Elastic Compute Service (20140526) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecs20140526-3.0.7/setup.py` & `alibabacloud_ecs20140526-4.24.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecs20140526.
 
-Created on 17/04/2023
+Created on 13/04/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecs20140526"
 NAME = "alibabacloud_ecs20140526" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elastic Compute Service (20140526) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

