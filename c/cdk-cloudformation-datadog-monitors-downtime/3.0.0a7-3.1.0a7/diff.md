# Comparing `tmp/cdk-cloudformation-datadog-monitors-downtime-3.0.0a7.tar.gz` & `tmp/cdk-cloudformation-datadog-monitors-downtime-3.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-monitors-downtime/dist/python/cdk-cloudformatio", last modified: Fri Feb  3 16:13:03 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-monitors-downtime/dist/python/cdk-cloudformatio", last modified: Mon Apr 17 06:15:01 2023, max compression
```

## Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7.tar` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2705 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1829 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1843 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    15208 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      466 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    19342 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/datadog-monitors-downtime@3.0.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:12:56.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2705 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      702 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       45 2023-02-03 16:13:03.000000 cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2736 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1829 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1893 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    15208 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      466 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    19366 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/_jsii/datadog-monitors-downtime@3.1.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:14:52.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2736 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      702 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       45 2023-04-17 06:15:01.000000 cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/LICENSE` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/PKG-INFO` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-monitors-downtime
-Version: 3.0.0a7
-Summary: Datadog Monitors Downtime 3.0.0
+Version: 3.1.0a7
+Summary: Datadog Monitors Downtime 3.1.0
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
 
 # datadog-monitors-downtime
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.1.0.
 
 ## Description
 
-Datadog Monitors Downtime 3.0.0
+Datadog Monitors Downtime 3.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Monitors::Downtime`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.1.0).
 * Issues related to `Datadog::Monitors::Downtime` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/README.md` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # datadog-monitors-downtime
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.1.0.
 
 ## Description
 
-Datadog Monitors Downtime 3.0.0
+Datadog Monitors Downtime 3.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Monitors::Downtime`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.1.0).
 * Issues related to `Datadog::Monitors::Downtime` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/setup.py` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-datadog-monitors-downtime",
-    "version": "3.0.0.a7",
-    "description": "Datadog Monitors Downtime 3.0.0",
+    "version": "3.1.0.a7",
+    "description": "Datadog Monitors Downtime 3.1.0",
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
         "cdk_cloudformation_datadog_monitors_downtime",
         "cdk_cloudformation_datadog_monitors_downtime._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_datadog_monitors_downtime._jsii": [
-            "datadog-monitors-downtime@3.0.0-alpha.7.jsii.tgz"
+            "datadog-monitors-downtime@3.1.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_datadog_monitors_downtime": [
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

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime/__init__.py` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 # datadog-monitors-downtime
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.1.0.
 
 ## Description
 
-Datadog Monitors Downtime 3.0.0
+Datadog Monitors Downtime 3.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -29,15 +29,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Monitors::Downtime`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.1.0).
 * Issues related to `Datadog::Monitors::Downtime` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -212,15 +212,15 @@
         end: typing.Optional[jsii.Number] = None,
         message: typing.Optional[builtins.str] = None,
         monitor_id: typing.Optional[jsii.Number] = None,
         monitor_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         start: typing.Optional[jsii.Number] = None,
         timezone: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Datadog Monitors Downtime 3.0.0.
+        '''Datadog Monitors Downtime 3.1.0.
 
         :param scope: The scope(s) to which the downtime applies.
         :param disabled: Whether or not this downtime is disabled.
         :param end: POSIX timestamp to end the downtime. If not provided, the downtime is in effect indefinitely (i.e. until you cancel it).
         :param message: Message on the downtime.
         :param monitor_id: A single monitor to which the downtime applies. If not provided, the downtime applies to all monitors.
         :param monitor_tags: A comma-separated list of monitor tags, to which the downtime applies. The resulting downtime applies to monitors that match ALL provided monitor tags.
```

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/PKG-INFO` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-monitors-downtime
-Version: 3.0.0a7
-Summary: Datadog Monitors Downtime 3.0.0
+Version: 3.1.0a7
+Summary: Datadog Monitors Downtime 3.1.0
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
 
 # datadog-monitors-downtime
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Monitors::Downtime` v3.1.0.
 
 ## Description
 
-Datadog Monitors Downtime 3.0.0
+Datadog Monitors Downtime 3.1.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Monitors::Downtime`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-monitors-downtime+v3.1.0).
 * Issues related to `Datadog::Monitors::Downtime` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-monitors-downtime-3.0.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/SOURCES.txt` & `cdk-cloudformation-datadog-monitors-downtime-3.1.0a7/src/cdk_cloudformation_datadog_monitors_downtime.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_datadog_monitors_downtime/py.typed
 src/cdk_cloudformation_datadog_monitors_downtime.egg-info/PKG-INFO
 src/cdk_cloudformation_datadog_monitors_downtime.egg-info/SOURCES.txt
 src/cdk_cloudformation_datadog_monitors_downtime.egg-info/dependency_links.txt
 src/cdk_cloudformation_datadog_monitors_downtime.egg-info/requires.txt
 src/cdk_cloudformation_datadog_monitors_downtime.egg-info/top_level.txt
 src/cdk_cloudformation_datadog_monitors_downtime/_jsii/__init__.py
-src/cdk_cloudformation_datadog_monitors_downtime/_jsii/datadog-monitors-downtime@3.0.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_datadog_monitors_downtime/_jsii/datadog-monitors-downtime@3.1.0-alpha.7.jsii.tgz
```

