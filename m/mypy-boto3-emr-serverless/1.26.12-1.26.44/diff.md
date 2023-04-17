# Comparing `tmp/mypy-boto3-emr-serverless-1.26.12.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.26.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.26.12.tar", last modified: Thu Nov 17 20:31:18 2022, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.26.44.tar", last modified: Thu Jan  5 20:26:50 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.26.12.tar` & `mypy-boto3-emr-serverless-1.26.44.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.612782 mypy-boto3-emr-serverless-1.26.12/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14767 2022-11-17 20:31:18.604782 mypy-boto3-emr-serverless-1.26.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13303 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.596783 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13753 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13729 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7886 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    18051 2022-11-17 20:30:27.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    18020 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:31:18.604782 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14767 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-17 20:31:18.000000 mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:31:18.612782 mypy-boto3-emr-serverless-1.26.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-17 20:30:26.000000 mypy-boto3-emr-serverless-1.26.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.939952 mypy-boto3-emr-serverless-1.26.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-01-05 20:26:50.935952 mypy-boto3-emr-serverless-1.26.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.931952 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-01-05 20:26:25.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 20:26:50.935952 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-05 20:26:50.000000 mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 20:26:50.939952 mypy-boto3-emr-serverless-1.26.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-05 20:26:24.000000 mypy-boto3-emr-serverless-1.26.44/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/LICENSE` & `mypy-boto3-emr-serverless-1.26.44/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/PKG-INFO` & `mypy-boto3-emr-serverless-1.26.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.26.12
-Summary: Type annotations for boto3.EMRServerless 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.44
+Summary: Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,19 +328,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigurationTypeDef,
+    ImageConfigurationInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
@@ -351,20 +354,22 @@
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    WorkerTypeSpecificationTypeDef,
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/README.md` & `mypy-boto3-emr-serverless-1.26.44/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,19 +296,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigurationTypeDef,
+    ImageConfigurationInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
@@ -320,20 +322,22 @@
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    WorkerTypeSpecificationTypeDef,
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.26.12\nVersion:         1.26.12\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.26.44\nVersion:         1.26.44\nBuilder"
+        " version: 7.12.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.12")
+    print("1.26.44")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,25 @@
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
     ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
+    ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     UpdateApplicationResponseTypeDef,
+    WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -117,15 +119,17 @@
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
-        architecture: ArchitectureType = ...
+        architecture: ArchitectureType = ...,
+        imageConfiguration: ImageConfigurationInputTypeDef = ...,
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
@@ -274,15 +278,17 @@
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
-        architecture: ArchitectureType = ...
+        architecture: ArchitectureType = ...,
+        imageConfiguration: ImageConfigurationInputTypeDef = ...,
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,25 @@
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
     ConfigurationOverridesTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
+    ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     StartJobRunResponseTypeDef,
     UpdateApplicationResponseTypeDef,
+    WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -109,15 +111,17 @@
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
-        architecture: ArchitectureType = ...
+        architecture: ArchitectureType = ...,
+        imageConfiguration: ImageConfigurationInputTypeDef = ...,
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
@@ -252,15 +256,17 @@
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
         networkConfiguration: NetworkConfigurationTypeDef = ...,
-        architecture: ArchitectureType = ...
+        architecture: ArchitectureType = ...,
+        imageConfiguration: ImageConfigurationInputTypeDef = ...,
+        workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -80,27 +81,29 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -129,14 +132,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -184,14 +188,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -207,25 +212,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -257,28 +264,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -306,40 +317,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -78,27 +79,29 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -127,14 +130,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -182,14 +186,15 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -205,25 +210,27 @@
     "kafkaconnect",
     "kendra",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -255,28 +262,32 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -304,40 +315,44 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,21 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
+    "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigurationTypeDef",
+    "ImageConfigurationInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitTypeDef",
@@ -47,20 +49,22 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
@@ -116,14 +120,35 @@
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
+_RequiredImageConfigurationTypeDef = TypedDict(
+    "_RequiredImageConfigurationTypeDef",
+    {
+        "imageUri": str,
+    },
+)
+_OptionalImageConfigurationTypeDef = TypedDict(
+    "_OptionalImageConfigurationTypeDef",
+    {
+        "resolvedImageDigest": str,
+    },
+    total=False,
+)
+
+
+class ImageConfigurationTypeDef(
+    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
+):
+    pass
+
+
 _RequiredMaximumAllowedResourcesTypeDef = TypedDict(
     "_RequiredMaximumAllowedResourcesTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -186,14 +211,22 @@
 )
 
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
 
+ImageConfigurationInputTypeDef = TypedDict(
+    "ImageConfigurationInputTypeDef",
+    {
+        "imageUri": str,
+    },
+    total=False,
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -417,14 +450,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+    total=False,
+)
+
 CancelJobRunResponseTypeDef = TypedDict(
     "CancelJobRunResponseTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -471,14 +512,22 @@
         "applicationId": str,
         "jobRunId": str,
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkerTypeSpecificationInputTypeDef = TypedDict(
+    "WorkerTypeSpecificationInputTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -577,14 +626,16 @@
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationTypeDef,
+        "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
 
 class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
     pass
@@ -605,14 +656,16 @@
         "initialCapacity": Mapping[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Mapping[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
@@ -632,14 +685,16 @@
     {
         "initialCapacity": Mapping[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
+    "ImageConfigurationTypeDef",
     "MaximumAllowedResourcesTypeDef",
     "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigurationTypeDef",
+    "ImageConfigurationInputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
     "GetJobRunRequestRequestTypeDef",
     "HiveTypeDef",
     "WorkerResourceConfigTypeDef",
     "SparkSubmitTypeDef",
@@ -46,20 +48,22 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "WorkerTypeSpecificationTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
+    "WorkerTypeSpecificationInputTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
@@ -113,14 +117,33 @@
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
+_RequiredImageConfigurationTypeDef = TypedDict(
+    "_RequiredImageConfigurationTypeDef",
+    {
+        "imageUri": str,
+    },
+)
+_OptionalImageConfigurationTypeDef = TypedDict(
+    "_OptionalImageConfigurationTypeDef",
+    {
+        "resolvedImageDigest": str,
+    },
+    total=False,
+)
+
+class ImageConfigurationTypeDef(
+    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
+):
+    pass
+
 _RequiredMaximumAllowedResourcesTypeDef = TypedDict(
     "_RequiredMaximumAllowedResourcesTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -179,14 +202,22 @@
     },
     total=False,
 )
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+ImageConfigurationInputTypeDef = TypedDict(
+    "ImageConfigurationInputTypeDef",
+    {
+        "imageUri": str,
+    },
+    total=False,
+)
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -400,14 +431,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+    total=False,
+)
+
 CancelJobRunResponseTypeDef = TypedDict(
     "CancelJobRunResponseTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -454,14 +493,22 @@
         "applicationId": str,
         "jobRunId": str,
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+WorkerTypeSpecificationInputTypeDef = TypedDict(
+    "WorkerTypeSpecificationInputTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -556,14 +603,16 @@
         "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationTypeDef,
+        "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
     total=False,
 )
 
 class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
     pass
 
@@ -582,14 +631,16 @@
         "initialCapacity": Mapping[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Mapping[str, str],
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
@@ -607,14 +658,16 @@
     {
         "initialCapacity": Mapping[str, InitialCapacityConfigTypeDef],
         "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "autoStartConfiguration": AutoStartConfigTypeDef,
         "autoStopConfiguration": AutoStopConfigTypeDef,
         "networkConfiguration": NetworkConfigurationTypeDef,
         "architecture": ArchitectureType,
+        "imageConfiguration": ImageConfigurationInputTypeDef,
+        "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.26.12
-Summary: Type annotations for boto3.EMRServerless 1.26.12 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.44
+Summary: Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder 7.12.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.26.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.26.44](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,19 +328,21 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
+    ImageConfigurationTypeDef,
     MaximumAllowedResourcesTypeDef,
     NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigurationTypeDef,
+    ImageConfigurationInputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
     GetJobRunRequestRequestTypeDef,
     HiveTypeDef,
     WorkerResourceConfigTypeDef,
     SparkSubmitTypeDef,
@@ -351,20 +354,22 @@
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    WorkerTypeSpecificationTypeDef,
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
+    WorkerTypeSpecificationInputTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
```

### Comparing `mypy-boto3-emr-serverless-1.26.12/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.26.44/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.26.12/setup.py` & `mypy-boto3-emr-serverless-1.26.44/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.26.12",
+    version="1.26.44",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.26.12 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.EMRServerless 1.26.44 service generated with mypy-boto3-builder"
+        " 7.12.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_emr_serverless": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_emr_serverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

