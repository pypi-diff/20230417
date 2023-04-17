# Comparing `tmp/mypy-boto3-lambda-1.26.55.tar.gz` & `tmp/mypy-boto3-lambda-1.26.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.26.55.tar", last modified: Mon Jan 23 20:32:37 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.26.55.tar` & `mypy-boto3-lambda-1.26.80.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:32:37.240476 mypy-boto3-lambda-1.26.55/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-23 20:32:04.000000 mypy-boto3-lambda-1.26.55/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-01-23 20:32:37.236475 mypy-boto3-lambda-1.26.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-01-23 20:32:04.000000 mypy-boto3-lambda-1.26.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:32:37.236475 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58654 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58565 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-01-23 20:32:06.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-01-23 20:32:06.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75690 2023-01-23 20:32:07.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75585 2023-01-23 20:32:06.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-23 20:32:04.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-01-23 20:32:06.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-01-23 20:32:05.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:32:37.236475 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 20:32:37.000000 mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 20:32:37.240476 mypy-boto3-lambda-1.26.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-23 20:32:04.000000 mypy-boto3-lambda-1.26.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.132040 mypy-boto3-lambda-1.26.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-02-27 20:35:29.128040 mypy-boto3-lambda-1.26.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23093 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58852 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58763 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76307 2023-02-27 20:35:10.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76202 2023-02-27 20:35:09.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-02-27 20:35:08.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-02-27 20:35:28.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-27 20:35:29.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 20:35:28.000000 mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.132040 mypy-boto3-lambda-1.26.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-27 20:35:07.000000 mypy-boto3-lambda-1.26.80/setup.py
```

### Comparing `mypy-boto3-lambda-1.26.55/LICENSE` & `mypy-boto3-lambda-1.26.80/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/PKG-INFO` & `mypy-boto3-lambda-1.26.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.26.55
-Summary: Type annotations for boto3.Lambda 1.26.55 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.80
+Summary: Type annotations for boto3.Lambda 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.26.55](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,14 +399,15 @@
 
 ```python
 from mypy_boto3_lambda.literals import (
     ArchitectureType,
     CodeSigningPolicyType,
     EndPointTypeType,
     EventSourcePositionType,
+    FullDocumentType,
     FunctionActiveV2WaiterName,
     FunctionActiveWaiterName,
     FunctionExistsWaiterName,
     FunctionResponseTypeType,
     FunctionUpdatedV2WaiterName,
     FunctionUpdatedWaiterName,
     FunctionUrlAuthTypeType,
@@ -466,14 +467,15 @@
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsTypeDef,
+    DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
```

### Comparing `mypy-boto3-lambda-1.26.55/README.md` & `mypy-boto3-lambda-1.26.80/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.26.55](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,14 +367,15 @@
 
 ```python
 from mypy_boto3_lambda.literals import (
     ArchitectureType,
     CodeSigningPolicyType,
     EndPointTypeType,
     EventSourcePositionType,
+    FullDocumentType,
     FunctionActiveV2WaiterName,
     FunctionActiveWaiterName,
     FunctionExistsWaiterName,
     FunctionResponseTypeType,
     FunctionUpdatedV2WaiterName,
     FunctionUpdatedWaiterName,
     FunctionUrlAuthTypeType,
@@ -434,14 +435,15 @@
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsTypeDef,
+    DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.26.55\nVersion:         1.26.55\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Lambda 1.26.80\nVersion:         1.26.80\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.55")
+    print("1.26.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseMetadataTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
+    DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseMetadataTypeDef,
     FileSystemConfigTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
@@ -300,15 +301,16 @@
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
-        ScalingConfig: ScalingConfigTypeDef = ...
+        ScalingConfig: ScalingConfigTypeDef = ...,
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_event_source_mapping)
         """
@@ -1015,15 +1017,16 @@
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
-        ScalingConfig: ScalingConfigTypeDef = ...
+        ScalingConfig: ScalingConfigTypeDef = ...,
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseMetadataTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
+    DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseMetadataTypeDef,
     FileSystemConfigTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
@@ -289,15 +290,16 @@
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
-        ScalingConfig: ScalingConfigTypeDef = ...
+        ScalingConfig: ScalingConfigTypeDef = ...,
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_event_source_mapping)
         """
@@ -947,15 +949,16 @@
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
-        ScalingConfig: ScalingConfigTypeDef = ...
+        ScalingConfig: ScalingConfigTypeDef = ...,
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ArchitectureType",
     "CodeSigningPolicyType",
     "EndPointTypeType",
     "EventSourcePositionType",
+    "FullDocumentType",
     "FunctionActiveV2WaiterName",
     "FunctionActiveWaiterName",
     "FunctionExistsWaiterName",
     "FunctionResponseTypeType",
     "FunctionUpdatedV2WaiterName",
     "FunctionUpdatedWaiterName",
     "FunctionUrlAuthTypeType",
@@ -62,19 +62,19 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ArchitectureType = Literal["arm64", "x86_64"]
 CodeSigningPolicyType = Literal["Enforce", "Warn"]
 EndPointTypeType = Literal["KAFKA_BOOTSTRAP_SERVERS"]
 EventSourcePositionType = Literal["AT_TIMESTAMP", "LATEST", "TRIM_HORIZON"]
+FullDocumentType = Literal["Default", "UpdateLookup"]
 FunctionActiveV2WaiterName = Literal["function_active_v2"]
 FunctionActiveWaiterName = Literal["function_active"]
 FunctionExistsWaiterName = Literal["function_exists"]
 FunctionResponseTypeType = Literal["ReportBatchItemFailures"]
 FunctionUpdatedV2WaiterName = Literal["function_updated_v2"]
 FunctionUpdatedWaiterName = Literal["function_updated"]
 FunctionUrlAuthTypeType = Literal["AWS_IAM", "NONE"]
@@ -241,14 +241,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -334,14 +335,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -510,14 +512,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ArchitectureType",
     "CodeSigningPolicyType",
     "EndPointTypeType",
     "EventSourcePositionType",
+    "FullDocumentType",
     "FunctionActiveV2WaiterName",
     "FunctionActiveWaiterName",
     "FunctionExistsWaiterName",
     "FunctionResponseTypeType",
     "FunctionUpdatedV2WaiterName",
     "FunctionUpdatedWaiterName",
     "FunctionUrlAuthTypeType",
@@ -61,18 +63,20 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ArchitectureType = Literal["arm64", "x86_64"]
 CodeSigningPolicyType = Literal["Enforce", "Warn"]
 EndPointTypeType = Literal["KAFKA_BOOTSTRAP_SERVERS"]
 EventSourcePositionType = Literal["AT_TIMESTAMP", "LATEST", "TRIM_HORIZON"]
+FullDocumentType = Literal["Default", "UpdateLookup"]
 FunctionActiveV2WaiterName = Literal["function_active_v2"]
 FunctionActiveWaiterName = Literal["function_active"]
 FunctionExistsWaiterName = Literal["function_exists"]
 FunctionResponseTypeType = Literal["ReportBatchItemFailures"]
 FunctionUpdatedV2WaiterName = Literal["function_updated_v2"]
 FunctionUpdatedWaiterName = Literal["function_updated"]
 FunctionUrlAuthTypeType = Literal["AWS_IAM", "NONE"]
@@ -239,14 +243,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -332,14 +337,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -508,14 +514,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ArchitectureType,
     CodeSigningPolicyType,
     EventSourcePositionType,
+    FullDocumentType,
     FunctionUrlAuthTypeType,
     InvocationTypeType,
     LastUpdateStatusReasonCodeType,
     LastUpdateStatusType,
     LogTypeType,
     PackageTypeType,
     ProvisionedConcurrencyStatusEnumType,
@@ -56,14 +57,15 @@
     "AddPermissionRequestRequestTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
     "CorsTypeDef",
+    "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
     "DeadLetterConfigTypeDef",
     "EnvironmentTypeDef",
     "EphemeralStorageTypeDef",
@@ -361,14 +363,24 @@
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
+DocumentDBEventSourceConfigTypeDef = TypedDict(
+    "DocumentDBEventSourceConfigTypeDef",
+    {
+        "DatabaseName": str,
+        "CollectionName": str,
+        "FullDocument": FullDocumentType,
+    },
+    total=False,
+)
+
 ScalingConfigTypeDef = TypedDict(
     "ScalingConfigTypeDef",
     {
         "MaximumConcurrency": int,
     },
     total=False,
 )
@@ -1459,14 +1471,15 @@
 )
 
 GetRuntimeManagementConfigResponseTypeDef = TypedDict(
     "GetRuntimeManagementConfigResponseTypeDef",
     {
         "UpdateRuntimeOn": UpdateRuntimeOnType,
         "RuntimeVersionArn": str,
+        "FunctionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvocationResponseTypeDef = TypedDict(
     "InvocationResponseTypeDef",
     {
@@ -2488,14 +2501,15 @@
         "Queues": Sequence[str],
         "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateEventSourceMappingRequestRequestTypeDef(
     _RequiredCreateEventSourceMappingRequestRequestTypeDef,
@@ -2529,14 +2543,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
@@ -2562,14 +2577,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
@@ -2589,14 +2605,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "ParallelizationFactor": int,
         "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpdateEventSourceMappingRequestRequestTypeDef(
     _RequiredUpdateEventSourceMappingRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ArchitectureType,
     CodeSigningPolicyType,
     EventSourcePositionType,
+    FullDocumentType,
     FunctionUrlAuthTypeType,
     InvocationTypeType,
     LastUpdateStatusReasonCodeType,
     LastUpdateStatusType,
     LogTypeType,
     PackageTypeType,
     ProvisionedConcurrencyStatusEnumType,
@@ -55,14 +56,15 @@
     "AddPermissionRequestRequestTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "CodeSigningPoliciesTypeDef",
     "ConcurrencyTypeDef",
     "CorsTypeDef",
+    "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
     "SourceAccessConfigurationTypeDef",
     "DeadLetterConfigTypeDef",
     "EnvironmentTypeDef",
     "EphemeralStorageTypeDef",
@@ -356,14 +358,24 @@
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
+DocumentDBEventSourceConfigTypeDef = TypedDict(
+    "DocumentDBEventSourceConfigTypeDef",
+    {
+        "DatabaseName": str,
+        "CollectionName": str,
+        "FullDocument": FullDocumentType,
+    },
+    total=False,
+)
+
 ScalingConfigTypeDef = TypedDict(
     "ScalingConfigTypeDef",
     {
         "MaximumConcurrency": int,
     },
     total=False,
 )
@@ -1410,14 +1422,15 @@
 )
 
 GetRuntimeManagementConfigResponseTypeDef = TypedDict(
     "GetRuntimeManagementConfigResponseTypeDef",
     {
         "UpdateRuntimeOn": UpdateRuntimeOnType,
         "RuntimeVersionArn": str,
+        "FunctionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InvocationResponseTypeDef = TypedDict(
     "InvocationResponseTypeDef",
     {
@@ -2387,14 +2400,15 @@
         "Queues": Sequence[str],
         "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceTypeDef,
         "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 class CreateEventSourceMappingRequestRequestTypeDef(
     _RequiredCreateEventSourceMappingRequestRequestTypeDef,
     _OptionalCreateEventSourceMappingRequestRequestTypeDef,
@@ -2426,14 +2440,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
@@ -2459,14 +2474,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventSourceMappingRequestRequestTypeDef",
     {
@@ -2486,14 +2502,15 @@
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "ParallelizationFactor": int,
         "SourceAccessConfigurations": Sequence[SourceAccessConfigurationTypeDef],
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": Sequence[Literal["ReportBatchItemFailures"]],
         "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateEventSourceMappingRequestRequestTypeDef(
     _RequiredUpdateEventSourceMappingRequestRequestTypeDef,
     _OptionalUpdateEventSourceMappingRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.26.55
-Summary: Type annotations for boto3.Lambda 1.26.55 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.80
+Summary: Type annotations for boto3.Lambda 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.26.55](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,14 +399,15 @@
 
 ```python
 from mypy_boto3_lambda.literals import (
     ArchitectureType,
     CodeSigningPolicyType,
     EndPointTypeType,
     EventSourcePositionType,
+    FullDocumentType,
     FunctionActiveV2WaiterName,
     FunctionActiveWaiterName,
     FunctionExistsWaiterName,
     FunctionResponseTypeType,
     FunctionUpdatedV2WaiterName,
     FunctionUpdatedWaiterName,
     FunctionUrlAuthTypeType,
@@ -466,14 +467,15 @@
     AddPermissionRequestRequestTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyTypeDef,
     CorsTypeDef,
+    DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SourceAccessConfigurationTypeDef,
     DeadLetterConfigTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
```

### Comparing `mypy-boto3-lambda-1.26.55/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.26.80/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.26.55/setup.py` & `mypy-boto3-lambda-1.26.80/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.26.55",
+    version="1.26.80",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.26.55 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Lambda 1.26.80 service generated with mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

