# Comparing `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.97.tar.gz` & `tmp/renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.97.tar", last modified: Mon Apr 17 13:17:25 2023, max compression
+gzip compressed data, was "renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar", last modified: Mon Apr 17 13:25:19 2023, max compression
```

## Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97.tar` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.97.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:17:12.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:17:25.340408 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-17 13:17:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 13:17:25.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:17:24.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 13:17:25.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 13:17:25.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:25:19.548142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.98.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:25:05.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:25:19.544142 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 13:25:19.000000 renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/LICENSE` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/LICENSE`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.97
+Version: 2.3.98
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,9 +41,7 @@
 * npm installed on your machine
 * AWS CDK installed on your machine
 * python installed on your machine
 * dotnet installed on your machine
 * a github account
 
 This project is managed with `projen`. Modify the `.projenrc.js` file and run `npx projen`. You can also modify this `README` file and the `src` code directory as needed. Github actions take care of publishing utilizing the automatically created workflows from `projen`.
-
-
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/README.md` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/README.md`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/setup.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "renovosolutions.aws-cdk-managed-instance-role",
-    "version": "2.3.97",
+    "version": "2.3.98",
     "description": "AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.",
     "license": "Apache-2.0",
     "url": "https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git",
     "long_description_content_type": "text/markdown",
     "author": "Renovo Solutions<webmaster+cdk@renovo1.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "managed_instance_role",
         "managed_instance_role._jsii"
     ],
     "package_data": {
         "managed_instance_role._jsii": [
-            "cdk-library-managed-instance-role@2.3.97.jsii.tgz"
+            "cdk-library-managed-instance-role@2.3.98.jsii.tgz"
         ],
         "managed_instance_role": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
@@ -45,14 +45,15 @@
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/managed_instance_role/__init__.py` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/managed_instance_role/__init__.py`

 * *Files identical despite different names*

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: renovosolutions.aws-cdk-managed-instance-role
-Version: 2.3.97
+Version: 2.3.98
 Summary: AWS CDK Construct Library to create an instance role for instances managed by SSM and capable of joining an AWS managed domain.
 Home-page: https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
 Author: Renovo Solutions<webmaster+cdk@renovo1.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/RenovoSolutions/cdk-library-managed-instance-role.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,9 +41,7 @@
 * npm installed on your machine
 * AWS CDK installed on your machine
 * python installed on your machine
 * dotnet installed on your machine
 * a github account
 
 This project is managed with `projen`. Modify the `.projenrc.js` file and run `npx projen`. You can also modify this `README` file and the `src` code directory as needed. Github actions take care of publishing utilizing the automatically created workflows from `projen`.
-
-
```

### Comparing `renovosolutions.aws-cdk-managed-instance-role-2.3.97/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt` & `renovosolutions.aws-cdk-managed-instance-role-2.3.98/src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/managed_instance_role/__init__.py
 src/managed_instance_role/py.typed
 src/managed_instance_role/_jsii/__init__.py
-src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.97.jsii.tgz
+src/managed_instance_role/_jsii/cdk-library-managed-instance-role@2.3.98.jsii.tgz
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/PKG-INFO
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/SOURCES.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/dependency_links.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/requires.txt
 src/renovosolutions.aws_cdk_managed_instance_role.egg-info/top_level.txt
```

