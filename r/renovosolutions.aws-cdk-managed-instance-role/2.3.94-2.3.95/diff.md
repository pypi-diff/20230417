# Comparing `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.94.tar.gz` & `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.94.tar", last modified: Mon Mar  6 14:16:32 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.95.tar", last modified: Tue Mar  7 14:37:34 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94.tar` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:32.242581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-06 14:16:32.242581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:16:32.242581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:32.238581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:32.238581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:32.238581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.94.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:16:16.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:32.242581 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-06 14:16:31.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-06 14:16:32.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:16:31.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-06 14:16:32.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 14:16:32.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.95.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 14:37:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 14:37:34.847698 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-07 14:37:34.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-07 14:37:34.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 14:37:34.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-07 14:37:34.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-07 14:37:34.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/LICENSE` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.94
+Version: 2.3.95
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/README.md` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/setup.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-managed-instance-role",
-    "version": "2.3.94",
+    "version": "2.3.95",
     "description": "AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "managed_instance_role",
         "managed_instance_role._jsii"
     ],
     "package_data": {
         "managed_instance_role._jsii": [
-            "cdk-library-managed-instance-role@2.3.94.jsii.tgz"
+            "cdk-library-managed-instance-role@2.3.95.jsii.tgz"
         ],
         "managed_instance_role": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.66.1, <3.0.0",
+        "aws-cdk-lib>=2.67.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.73.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/managed_instance_role/__init__.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/managed_instance_role/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.94
+Version: 2.3.95
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.94/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-managed-instance-role-2.3.95/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/managed_instance_role/__init__.py
 src/managed_instance_role/py.typed
 src/managed_instance_role/_jsii/__init__.py
-src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.94.jsii.tgz
+src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.95.jsii.tgz
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```

