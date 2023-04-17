# Comparing `tmp/antchain_yuqing-1.1.9.tar.gz` & `tmp/antchain_yuqing-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_yuqing-1.1.9.tar", last modified: Fri Apr 15 09:30:21 2022, max compression
+gzip compressed data, was "dist/antchain_yuqing-1.2.3.tar", last modified: Mon Apr 17 08:00:56 2023, max compression
```

## Comparing `antchain_yuqing-1.1.9.tar` & `antchain_yuqing-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/
--rw-r--r--   0 root         (0) root         (0)      600 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2188 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      821 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1007 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_sdk_yuqing/
--rw-r--r--   0 root         (0) root         (0)       21 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/antchain_sdk_yuqing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26653 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/antchain_sdk_yuqing/client.py
--rw-r--r--   0 root         (0) root         (0)    66551 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/antchain_sdk_yuqing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2188 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/antchain_yuqing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-15 09:30:21.000000 antchain_yuqing-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2503 2022-04-15 09:30:20.000000 antchain_yuqing-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      999 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47795 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/client.py
+-rw-r--r--   0 root         (0) root         (0)   152781 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/setup.py
```

### Comparing `antchain_yuqing-1.1.9/LICENSE` & `antchain_yuqing-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_yuqing-1.1.9/PKG-INFO` & `antchain_yuqing-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_yuqing
-Version: 1.1.9
+Version: 1.2.3
 Summary: Ant Chain YUQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_yuqing
-        pip install antchain_sdk_yuqing
+        # Install the antchain-yuqing
+        pip install antchain-yuqing
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_yuqing-1.1.9/README-CN.md` & `antchain_yuqing-1.2.3/README-CN.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_yuqing
-pip install antchain_sdk_yuqing
+# 安装 antchain-yuqing
+pip install antchain-yuqing
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_yuqing-1.1.9/README.md` & `antchain_yuqing-1.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_yuqing
-pip install antchain_sdk_yuqing
+# Install the antchain-yuqing
+pip install antchain-yuqing
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_yuqing-1.1.9/antchain_yuqing.egg-info/PKG-INFO` & `antchain_yuqing-1.2.3/antchain_yuqing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-yuqing
-Version: 1.1.9
+Version: 1.2.3
 Summary: Ant Chain YUQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_yuqing
-        pip install antchain_sdk_yuqing
+        # Install the antchain-yuqing
+        pip install antchain-yuqing
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_yuqing-1.1.9/setup.py` & `antchain_yuqing-1.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_yuqing.
 
-Created on 15/04/2022
+Created on 17/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_yuqing"
 NAME = "antchain_yuqing" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain YUQING SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

