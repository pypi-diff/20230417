# Comparing `tmp/cdk-cloudformation-datadog-integrations-aws-2.3.0a7.tar.gz` & `tmp/cdk-cloudformation-datadog-integrations-aws-2.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-integrations-aws/dist/python/cdk-cloudformation", last modified: Fri Feb  3 16:12:54 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/datadog-integrations-aws/dist/python/cdk-cloudformation", last modified: Mon Apr 17 06:14:06 2023, max compression
```

## Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7.tar` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2693 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1820 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1835 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    18550 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      464 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    19834 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/datadog-integrations-aws@2.3.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:12:46.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2693 2023-02-03 16:12:53.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      692 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:12:53.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       44 2023-02-03 16:12:54.000000 cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2724 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1820 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     1885 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    19736 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      464 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    20062 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/_jsii/datadog-integrations-aws@2.4.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:13:59.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2724 2023-04-17 06:14:05.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      692 2023-04-17 06:14:06.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-17 06:14:05.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-17 06:14:05.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       44 2023-04-17 06:14:05.000000 cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/LICENSE` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/PKG-INFO` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-integrations-aws
-Version: 2.3.0a7
-Summary: Datadog AWS Integration 2.2.1
+Version: 2.4.0a7
+Summary: Datadog AWS Integration 2.4.0
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
 
 # datadog-integrations-aws
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.4.0.
 
 ## Description
 
-Datadog AWS Integration 2.2.1
+Datadog AWS Integration 2.4.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Integrations::AWS`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.4.0).
 * Issues related to `Datadog::Integrations::AWS` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/README.md` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # datadog-integrations-aws
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.4.0.
 
 ## Description
 
-Datadog AWS Integration 2.2.1
+Datadog AWS Integration 2.4.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -28,13 +28,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Integrations::AWS`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.4.0).
 * Issues related to `Datadog::Integrations::AWS` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/setup.py` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-datadog-integrations-aws",
-    "version": "2.3.0.a7",
-    "description": "Datadog AWS Integration 2.2.1",
+    "version": "2.4.0.a7",
+    "description": "Datadog AWS Integration 2.4.0",
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
         "cdk_cloudformation_datadog_integrations_aws",
         "cdk_cloudformation_datadog_integrations_aws._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_datadog_integrations_aws._jsii": [
-            "datadog-integrations-aws@2.3.0-alpha.7.jsii.tgz"
+            "datadog-integrations-aws@2.4.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_datadog_integrations_aws": [
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

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws/__init__.py` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 # datadog-integrations-aws
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.4.0.
 
 ## Description
 
-Datadog AWS Integration 2.2.1
+Datadog AWS Integration 2.4.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -29,15 +29,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Integrations::AWS`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.4.0).
 * Issues related to `Datadog::Integrations::AWS` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
@@ -74,14 +74,15 @@
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         access_key_id: typing.Optional[builtins.str] = None,
         account_id: typing.Optional[builtins.str] = None,
         account_specific_namespace_rules: typing.Any = None,
         cspm_resource_collection: typing.Optional[builtins.bool] = None,
+        excluded_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
         external_id_secret_name: typing.Optional[builtins.str] = None,
         filter_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         host_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         metrics_collection: typing.Optional[builtins.bool] = None,
         resource_collection: typing.Optional[builtins.bool] = None,
         role_name: typing.Optional[builtins.str] = None,
     ) -> None:
@@ -89,14 +90,15 @@
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param access_key_id: If your AWS account is a GovCloud or China account, enter the corresponding Access Key ID.
         :param account_id: Your AWS Account ID without dashes.
         :param account_specific_namespace_rules: An object (in the form {"namespace1":true/false, "namespace2":true/false}) that enables or disables metric collection for specific AWS namespaces for this AWS account only.
         :param cspm_resource_collection: Enable the compliance and security posture management Datadog product. This will enable collecting information on your AWS resources and providing security validation.
+        :param excluded_regions: Array of AWS regions to exclude from metrics collection.
         :param external_id_secret_name: The name of the AWS SecretsManager secret created in your account to hold this integration's ``external_id``. Defaults to ``DatadogIntegrationExternalID``. Cannot be referenced from created resource. Default: DatadogIntegrationExternalID`. Cannot be referenced from created resource.
         :param filter_tags: The array of EC2 tags (in the form key:value) defines a filter that Datadog uses when collecting metrics from EC2.
         :param host_tags: Array of tags (in the form key:value) to add to all hosts and metrics reporting through this integration.
         :param metrics_collection: Enable the infrastructure monitoring Datadog product for this AWS Account. This will enable collecting all AWS metrics in your account.
         :param resource_collection: Enable collecting information on your AWS resources for use in Datadog products such as Network Process Monitoring.
         :param role_name: Your Datadog role delegation name.
         '''
@@ -105,14 +107,15 @@
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = CfnAwsProps(
             access_key_id=access_key_id,
             account_id=account_id,
             account_specific_namespace_rules=account_specific_namespace_rules,
             cspm_resource_collection=cspm_resource_collection,
+            excluded_regions=excluded_regions,
             external_id_secret_name=external_id_secret_name,
             filter_tags=filter_tags,
             host_tags=host_tags,
             metrics_collection=metrics_collection,
             resource_collection=resource_collection,
             role_name=role_name,
         )
@@ -145,14 +148,15 @@
     jsii_type="@cdk-cloudformation/datadog-integrations-aws.CfnAwsProps",
     jsii_struct_bases=[],
     name_mapping={
         "access_key_id": "accessKeyId",
         "account_id": "accountId",
         "account_specific_namespace_rules": "accountSpecificNamespaceRules",
         "cspm_resource_collection": "cspmResourceCollection",
+        "excluded_regions": "excludedRegions",
         "external_id_secret_name": "externalIdSecretName",
         "filter_tags": "filterTags",
         "host_tags": "hostTags",
         "metrics_collection": "metricsCollection",
         "resource_collection": "resourceCollection",
         "role_name": "roleName",
     },
@@ -161,27 +165,29 @@
     def __init__(
         self,
         *,
         access_key_id: typing.Optional[builtins.str] = None,
         account_id: typing.Optional[builtins.str] = None,
         account_specific_namespace_rules: typing.Any = None,
         cspm_resource_collection: typing.Optional[builtins.bool] = None,
+        excluded_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
         external_id_secret_name: typing.Optional[builtins.str] = None,
         filter_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         host_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
         metrics_collection: typing.Optional[builtins.bool] = None,
         resource_collection: typing.Optional[builtins.bool] = None,
         role_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Datadog AWS Integration 2.2.1.
+        '''Datadog AWS Integration 2.4.0.
 
         :param access_key_id: If your AWS account is a GovCloud or China account, enter the corresponding Access Key ID.
         :param account_id: Your AWS Account ID without dashes.
         :param account_specific_namespace_rules: An object (in the form {"namespace1":true/false, "namespace2":true/false}) that enables or disables metric collection for specific AWS namespaces for this AWS account only.
         :param cspm_resource_collection: Enable the compliance and security posture management Datadog product. This will enable collecting information on your AWS resources and providing security validation.
+        :param excluded_regions: Array of AWS regions to exclude from metrics collection.
         :param external_id_secret_name: The name of the AWS SecretsManager secret created in your account to hold this integration's ``external_id``. Defaults to ``DatadogIntegrationExternalID``. Cannot be referenced from created resource. Default: DatadogIntegrationExternalID`. Cannot be referenced from created resource.
         :param filter_tags: The array of EC2 tags (in the form key:value) defines a filter that Datadog uses when collecting metrics from EC2.
         :param host_tags: Array of tags (in the form key:value) to add to all hosts and metrics reporting through this integration.
         :param metrics_collection: Enable the infrastructure monitoring Datadog product for this AWS Account. This will enable collecting all AWS metrics in your account.
         :param resource_collection: Enable collecting information on your AWS resources for use in Datadog products such as Network Process Monitoring.
         :param role_name: Your Datadog role delegation name.
 
@@ -189,14 +195,15 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__43439c00d9be4cf1962f105015e4a84d7c2028cd1f85427390e822315830bd53)
             check_type(argname="argument access_key_id", value=access_key_id, expected_type=type_hints["access_key_id"])
             check_type(argname="argument account_id", value=account_id, expected_type=type_hints["account_id"])
             check_type(argname="argument account_specific_namespace_rules", value=account_specific_namespace_rules, expected_type=type_hints["account_specific_namespace_rules"])
             check_type(argname="argument cspm_resource_collection", value=cspm_resource_collection, expected_type=type_hints["cspm_resource_collection"])
+            check_type(argname="argument excluded_regions", value=excluded_regions, expected_type=type_hints["excluded_regions"])
             check_type(argname="argument external_id_secret_name", value=external_id_secret_name, expected_type=type_hints["external_id_secret_name"])
             check_type(argname="argument filter_tags", value=filter_tags, expected_type=type_hints["filter_tags"])
             check_type(argname="argument host_tags", value=host_tags, expected_type=type_hints["host_tags"])
             check_type(argname="argument metrics_collection", value=metrics_collection, expected_type=type_hints["metrics_collection"])
             check_type(argname="argument resource_collection", value=resource_collection, expected_type=type_hints["resource_collection"])
             check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -204,14 +211,16 @@
             self._values["access_key_id"] = access_key_id
         if account_id is not None:
             self._values["account_id"] = account_id
         if account_specific_namespace_rules is not None:
             self._values["account_specific_namespace_rules"] = account_specific_namespace_rules
         if cspm_resource_collection is not None:
             self._values["cspm_resource_collection"] = cspm_resource_collection
+        if excluded_regions is not None:
+            self._values["excluded_regions"] = excluded_regions
         if external_id_secret_name is not None:
             self._values["external_id_secret_name"] = external_id_secret_name
         if filter_tags is not None:
             self._values["filter_tags"] = filter_tags
         if host_tags is not None:
             self._values["host_tags"] = host_tags
         if metrics_collection is not None:
@@ -256,14 +265,23 @@
 
         :schema: CfnAwsProps#CSPMResourceCollection
         '''
         result = self._values.get("cspm_resource_collection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def excluded_regions(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Array of AWS regions to exclude from metrics collection.
+
+        :schema: CfnAwsProps#ExcludedRegions
+        '''
+        result = self._values.get("excluded_regions")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def external_id_secret_name(self) -> typing.Optional[builtins.str]:
         '''The name of the AWS SecretsManager secret created in your account to hold this integration's ``external_id``.
 
         Defaults to ``DatadogIntegrationExternalID``. Cannot be referenced from created resource.
 
         :default: DatadogIntegrationExternalID`. Cannot be referenced from created resource.
 
@@ -342,14 +360,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     access_key_id: typing.Optional[builtins.str] = None,
     account_id: typing.Optional[builtins.str] = None,
     account_specific_namespace_rules: typing.Any = None,
     cspm_resource_collection: typing.Optional[builtins.bool] = None,
+    excluded_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
     external_id_secret_name: typing.Optional[builtins.str] = None,
     filter_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     host_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     metrics_collection: typing.Optional[builtins.bool] = None,
     resource_collection: typing.Optional[builtins.bool] = None,
     role_name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -358,14 +377,15 @@
 
 def _typecheckingstub__43439c00d9be4cf1962f105015e4a84d7c2028cd1f85427390e822315830bd53(
     *,
     access_key_id: typing.Optional[builtins.str] = None,
     account_id: typing.Optional[builtins.str] = None,
     account_specific_namespace_rules: typing.Any = None,
     cspm_resource_collection: typing.Optional[builtins.bool] = None,
+    excluded_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
     external_id_secret_name: typing.Optional[builtins.str] = None,
     filter_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     host_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     metrics_collection: typing.Optional[builtins.bool] = None,
     resource_collection: typing.Optional[builtins.bool] = None,
     role_name: typing.Optional[builtins.str] = None,
 ) -> None:
```

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/PKG-INFO` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-datadog-integrations-aws
-Version: 2.3.0a7
-Summary: Datadog AWS Integration 2.2.1
+Version: 2.4.0a7
+Summary: Datadog AWS Integration 2.4.0
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
 
 # datadog-integrations-aws
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.3.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `Datadog::Integrations::AWS` v2.4.0.
 
 ## Description
 
-Datadog AWS Integration 2.2.1
+Datadog AWS Integration 2.4.0
 
 ## Usage
 
 In order to use this library, you will need to activate this AWS CloudFormation Registry type in your account. You can do this via the AWS Management Console or using the [AWS CLI](https://aws.amazon.com/cli/) using the following command:
 
 ```sh
 aws cloudformation activate-type \
@@ -51,15 +51,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `Datadog::Integrations::AWS`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.3.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fdatadog-integrations-aws+v2.4.0).
 * Issues related to `Datadog::Integrations::AWS` should be reported to the [publisher](undefined).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-datadog-integrations-aws-2.3.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/SOURCES.txt` & `cdk-cloudformation-datadog-integrations-aws-2.4.0a7/src/cdk_cloudformation_datadog_integrations_aws.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_datadog_integrations_aws/py.typed
 src/cdk_cloudformation_datadog_integrations_aws.egg-info/PKG-INFO
 src/cdk_cloudformation_datadog_integrations_aws.egg-info/SOURCES.txt
 src/cdk_cloudformation_datadog_integrations_aws.egg-info/dependency_links.txt
 src/cdk_cloudformation_datadog_integrations_aws.egg-info/requires.txt
 src/cdk_cloudformation_datadog_integrations_aws.egg-info/top_level.txt
 src/cdk_cloudformation_datadog_integrations_aws/_jsii/__init__.py
-src/cdk_cloudformation_datadog_integrations_aws/_jsii/datadog-integrations-aws@2.3.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_datadog_integrations_aws/_jsii/datadog-integrations-aws@2.4.0-alpha.7.jsii.tgz
```

