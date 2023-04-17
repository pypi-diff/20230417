# Comparing `tmp/cdk-cloudformation-datadog-slos-slo-1.0.1a7.tar.gz` & `tmp/cdk-cloudformation-datadog-slos-slo-1.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-slos-slo/dist/python/cdk-cloudformation-datadog", last modified: Fri Feb  3 17:32:40 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-slos-slo/dist/python/cdk-cloudformation-datadog", last modified: Mon Apr 17 06:14:14 2023, max compression
```

## Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7.tar` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2605 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1752 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1775 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    25308 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      448 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    22225 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/datadog-slos-slo@1.0.1-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 17:32:29.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2605 2023-02-03 17:32:39.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      612 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 17:32:39.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 17:32:39.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       36 2023-02-03 17:32:40.000000 cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2636 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1752 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1825 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    25308 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      448 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    22237 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/_jsii/datadog-slos-slo@1.1.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:14:08.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2636 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      612 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       36 2023-04-17 06:14:14.000000 cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/LICENSE` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/PKG-INFO` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-slos-slo
-Version: 1.0.1a7
-Summary: Datadog SLO 1.0.1
+Version: 1.1.0a7
+Summary: Datadog SLO 1.1.0
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
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
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datadog-slos-slo
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.0.1.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.1.0.
 
 ## Description
 
-Datadog SLO 1.0.1
+Datadog SLO 1.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::SLOs::SLO`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.0.1).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.1.0).
 * Issues related to `Datadog::SLOs::SLO` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/README.md` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # datadog-slos-slo
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.0.1.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.1.0.
 
 ## Description
 
-Datadog SLO 1.0.1
+Datadog SLO 1.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::SLOs::SLO`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.0.1).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.1.0).
 * Issues related to `Datadog::SLOs::SLO` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/setup.py` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-datadog-slos-slo",
-    "version": "1.0.1.a7",
-    "description": "Datadog SLO 1.0.1",
+    "version": "1.1.0.a7",
+    "description": "Datadog SLO 1.1.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-cloudformation.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_cloudformation_datadog_slos_slo",
         "cdk_cloudformation_datadog_slos_slo._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_datadog_slos_slo._jsii": [
-            "datadog-slos-slo@1.0.1-alpha.7.jsii.tgz"
+            "datadog-slos-slo@1.1.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_datadog_slos_slo": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.63.0, <3.0.0",
-        "constructs>=10.1.239, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "aws-cdk-lib>=2.72.1, <3.0.0",
+        "constructs>=10.1.302, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo/__init__.py` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 # datadog-slos-slo
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.0.1.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.1.0.
 
 ## Description
 
-Datadog SLO 1.0.1
+Datadog SLO 1.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -29,15 +29,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::SLOs::SLO`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.0.1).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.1.0).
 * Issues related to `Datadog::SLOs::SLO` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -190,15 +190,15 @@
         creator: typing.Optional[typing.Union["Creator", typing.Dict[builtins.str, typing.Any]]] = None,
         description: typing.Optional[builtins.str] = None,
         groups: typing.Optional[typing.Sequence[builtins.str]] = None,
         monitor_ids: typing.Optional[typing.Sequence[jsii.Number]] = None,
         query: typing.Optional[typing.Union["Query", typing.Dict[builtins.str, typing.Any]]] = None,
         tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
-        '''Datadog SLO 1.0.1.
+        '''Datadog SLO 1.1.0.
 
         :param name: Name of the slo.
         :param thresholds: 
         :param type: The type of the slo.
         :param creator: 
         :param description: Description of the slo.
         :param groups: A list of (up to 20) monitor groups that narrow the scope of a monitor service level objective.
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/PKG-INFO` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-slos-slo
-Version: 1.0.1a7
-Summary: Datadog SLO 1.0.1
+Version: 1.1.0a7
+Summary: Datadog SLO 1.1.0
 Home-page: https://github.com/cdklabs/cdk-cloudformation.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
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
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datadog-slos-slo
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.0.1.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::SLOs::SLO` v1.1.0.
 
 ## Description
 
-Datadog SLO 1.0.1
+Datadog SLO 1.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::SLOs::SLO`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.0.1).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-slos-slo+v1.1.0).
 * Issues related to `Datadog::SLOs::SLO` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-slos-slo-1.0.1a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/SOURCES.txt` & `cdk-cloudformation-datadog-slos-slo-1.1.0a7/src/cdk_cloudformation_datadog_slos_slo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_datadog_slos_slo/py.typed
 src/cdk_cloudformation_datadog_slos_slo.egg-info/PKG-INFO
 src/cdk_cloudformation_datadog_slos_slo.egg-info/SOURCES.txt
 src/cdk_cloudformation_datadog_slos_slo.egg-info/dependency_links.txt
 src/cdk_cloudformation_datadog_slos_slo.egg-info/requires.txt
 src/cdk_cloudformation_datadog_slos_slo.egg-info/top_level.txt
 src/cdk_cloudformation_datadog_slos_slo/_jsii/__init__.py
-src/cdk_cloudformation_datadog_slos_slo/_jsii/datadog-slos-slo@1.0.1-alpha.7.jsii.tgz
+src/cdk_cloudformation_datadog_slos_slo/_jsii/datadog-slos-slo@1.1.0-alpha.7.jsii.tgz
```

