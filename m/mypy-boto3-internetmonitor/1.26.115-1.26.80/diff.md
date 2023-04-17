# Comparing `tmp/mypy-boto3-internetmonitor-1.26.115.tar.gz` & `tmp/mypy-boto3-internetmonitor-1.26.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-internetmonitor-1.26.115.tar", last modified: Mon Apr 17 19:43:45 2023, max compression
+gzip compressed data, was "mypy-boto3-internetmonitor-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
```

## Comparing `mypy-boto3-internetmonitor-1.26.115.tar` & `mypy-boto3-internetmonitor-1.26.80.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:43:45.709453 mypy-boto3-internetmonitor-1.26.115/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-04-17 19:43:45.709453 mypy-boto3-internetmonitor-1.26.115/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:43:45.709453 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-04-17 19:43:26.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-17 19:43:26.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-17 19:43:26.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:43:45.709453 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 19:43:45.000000 mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:43:45.709453 mypy-boto3-internetmonitor-1.26.115/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-17 19:43:25.000000 mypy-boto3-internetmonitor-1.26.115/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-internetmonitor-1.26.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-02-27 20:35:29.116040 mypy-boto3-internetmonitor-1.26.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.112040 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10987 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-02-27 20:35:06.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-02-27 20:35:06.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-02-27 20:35:06.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-02-27 20:35:06.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.116040 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-27 20:35:28.000000 mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.120040 mypy-boto3-internetmonitor-1.26.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-02-27 20:35:05.000000 mypy-boto3-internetmonitor-1.26.80/setup.py
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/LICENSE` & `mypy-boto3-internetmonitor-1.26.80/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/PKG-INFO` & `mypy-boto3-internetmonitor-1.26.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.26.115
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.26.115 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.80
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.26.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,15 +303,14 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
@@ -329,40 +328,38 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
+    CreateMonitorInputRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateMonitorInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
+    GetMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
@@ -374,42 +371,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/README.md` & `mypy-boto3-internetmonitor-1.26.80/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.26.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,15 +271,14 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
@@ -297,40 +296,38 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
+    CreateMonitorInputRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateMonitorInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
+    GetMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
@@ -342,42 +339,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__init__.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__init__.pyi` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/__main__.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.26.115\nVersion:        "
-        " 1.26.115\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.26.80\nVersion:        "
+        " 1.26.80\nBuilder version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.115")
+    print("1.26.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/client.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,53 +21,48 @@
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchInternetMonitorClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class CloudWatchInternetMonitorClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/)
     """
 
     meta: ClientMeta
@@ -76,89 +71,79 @@
     def exceptions(self) -> Exceptions:
         """
         CloudWatchInternetMonitorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#close)
         """
-
     def create_monitor(
         self,
         *,
         MonitorName: str,
+        MaxCityNetworksToMonitor: int,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...,
-        MaxCityNetworksToMonitor: int = ...,
-        InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        Tags: Mapping[str, str] = ...
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#create_monitor)
         """
-
     def delete_monitor(self, *, MonitorName: str) -> Dict[str, Any]:
         """
         Deletes a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.delete_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#delete_monitor)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#generate_presigned_url)
         """
-
     def get_health_event(self, *, MonitorName: str, EventId: str) -> GetHealthEventOutputTypeDef:
         """
         Gets information the Amazon CloudWatch Internet Monitor has created and stored
         about a health event for a specified monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_health_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_health_event)
         """
-
     def get_monitor(self, *, MonitorName: str) -> GetMonitorOutputTypeDef:
         """
         Gets information about a monitor in Amazon CloudWatch Internet Monitor based on
         a monitor name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_monitor)
         """
-
     def list_health_events(
         self,
         *,
         MonitorName: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         NextToken: str = ...,
@@ -167,77 +152,68 @@
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_health_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_health_events)
         """
-
     def list_monitors(
         self, *, NextToken: str = ..., MaxResults: int = ..., MonitorStatus: str = ...
     ) -> ListMonitorsOutputTypeDef:
         """
         Lists all of your monitors for Amazon CloudWatch Internet Monitor and their
         statuses, along with the Amazon Resource Name (ARN) and name of each monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_monitors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_monitors)
         """
-
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists the tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_tags_for_resource)
         """
-
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds a tag to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#untag_resource)
         """
-
     def update_monitor(
         self,
         *,
         MonitorName: str,
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
-        MaxCityNetworksToMonitor: int = ...,
-        InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        MaxCityNetworksToMonitor: int = ...
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#update_monitor)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_health_events"]
     ) -> ListHealthEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_monitors"]) -> ListMonitorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/client.pyi` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,49 +21,52 @@
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CloudWatchInternetMonitorClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class CloudWatchInternetMonitorClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/)
     """
 
     meta: ClientMeta
@@ -72,81 +75,87 @@
     def exceptions(self) -> Exceptions:
         """
         CloudWatchInternetMonitorClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#close)
         """
+
     def create_monitor(
         self,
         *,
         MonitorName: str,
+        MaxCityNetworksToMonitor: int,
         Resources: Sequence[str] = ...,
         ClientToken: str = ...,
-        Tags: Mapping[str, str] = ...,
-        MaxCityNetworksToMonitor: int = ...,
-        InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        Tags: Mapping[str, str] = ...
     ) -> CreateMonitorOutputTypeDef:
         """
         Creates a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#create_monitor)
         """
+
     def delete_monitor(self, *, MonitorName: str) -> Dict[str, Any]:
         """
         Deletes a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.delete_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#delete_monitor)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#generate_presigned_url)
         """
+
     def get_health_event(self, *, MonitorName: str, EventId: str) -> GetHealthEventOutputTypeDef:
         """
         Gets information the Amazon CloudWatch Internet Monitor has created and stored
         about a health event for a specified monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_health_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_health_event)
         """
+
     def get_monitor(self, *, MonitorName: str) -> GetMonitorOutputTypeDef:
         """
         Gets information about a monitor in Amazon CloudWatch Internet Monitor based on
         a monitor name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_monitor)
         """
+
     def list_health_events(
         self,
         *,
         MonitorName: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         NextToken: str = ...,
@@ -155,70 +164,75 @@
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_health_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_health_events)
         """
+
     def list_monitors(
         self, *, NextToken: str = ..., MaxResults: int = ..., MonitorStatus: str = ...
     ) -> ListMonitorsOutputTypeDef:
         """
         Lists all of your monitors for Amazon CloudWatch Internet Monitor and their
         statuses, along with the Amazon Resource Name (ARN) and name of each monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_monitors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_monitors)
         """
+
     def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Lists the tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#list_tags_for_resource)
         """
+
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds a tag to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a tag from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#untag_resource)
         """
+
     def update_monitor(
         self,
         *,
         MonitorName: str,
         ResourcesToAdd: Sequence[str] = ...,
         ResourcesToRemove: Sequence[str] = ...,
         Status: MonitorConfigStateType = ...,
         ClientToken: str = ...,
-        MaxCityNetworksToMonitor: int = ...,
-        InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,
-        TrafficPercentageToMonitor: int = ...
+        MaxCityNetworksToMonitor: int = ...
     ) -> UpdateMonitorOutputTypeDef:
         """
         Updates a monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#update_monitor)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_health_events"]
     ) -> ListHealthEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_monitors"]) -> ListMonitorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/literals.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/literals.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
-    "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
@@ -36,15 +35,14 @@
 )
 
 
 HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
-LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
     "INSUFFICIENT_DATA",
@@ -215,15 +213,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -379,15 +376,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -407,35 +403,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
     "ap-northeast-3",
-    "ap-south-1",
     "ap-south-2",
-    "ap-southeast-1",
-    "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
-    "ca-central-1",
-    "eu-central-1",
     "eu-central-2",
-    "eu-north-1",
-    "eu-south-1",
     "eu-south-2",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
     "me-central-1",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
 ]
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/literals.pyi` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/literals.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -19,30 +19,28 @@
     from typing_extensions import Literal
 
 __all__ = (
     "HealthEventImpactTypeType",
     "HealthEventStatusType",
     "ListHealthEventsPaginatorName",
     "ListMonitorsPaginatorName",
-    "LogDeliveryStatusType",
     "MonitorConfigStateType",
     "MonitorProcessingStatusCodeType",
     "TriangulationEventTypeType",
     "CloudWatchInternetMonitorServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 HealthEventImpactTypeType = Literal["AVAILABILITY", "PERFORMANCE"]
 HealthEventStatusType = Literal["ACTIVE", "RESOLVED"]
 ListHealthEventsPaginatorName = Literal["list_health_events"]
 ListMonitorsPaginatorName = Literal["list_monitors"]
-LogDeliveryStatusType = Literal["DISABLED", "ENABLED"]
 MonitorConfigStateType = Literal["ACTIVE", "ERROR", "INACTIVE", "PENDING"]
 MonitorProcessingStatusCodeType = Literal[
     "COLLECTING_DATA",
     "FAULT_ACCESS_CLOUDWATCH",
     "FAULT_SERVICE",
     "INACTIVE",
     "INSUFFICIENT_DATA",
@@ -213,15 +211,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -377,15 +374,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -405,35 +401,15 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_health_events", "list_monitors"]
 RegionName = Literal[
-    "af-south-1",
-    "ap-east-1",
-    "ap-northeast-1",
-    "ap-northeast-2",
     "ap-northeast-3",
-    "ap-south-1",
     "ap-south-2",
-    "ap-southeast-1",
-    "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
-    "ca-central-1",
-    "eu-central-1",
     "eu-central-2",
-    "eu-north-1",
-    "eu-south-1",
     "eu-south-2",
-    "eu-west-1",
-    "eu-west-2",
-    "eu-west-3",
     "me-central-1",
-    "me-south-1",
-    "sa-east-1",
-    "us-east-1",
-    "us-east-2",
-    "us-west-1",
-    "us-west-2",
 ]
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/paginator.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/paginator.pyi` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/type_defs.py` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -14,54 +14,50 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
-    LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AvailabilityMeasurementTypeDef",
+    "CreateMonitorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
-    "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateMonitorInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
+    "GetMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
-    "InternetMeasurementsLogDeliveryTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "CreateMonitorInputRequestTypeDef",
-    "GetMonitorOutputTypeDef",
-    "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
 
@@ -71,14 +67,36 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
+_RequiredCreateMonitorInputRequestTypeDef = TypedDict(
+    "_RequiredCreateMonitorInputRequestTypeDef",
+    {
+        "MonitorName": str,
+        "MaxCityNetworksToMonitor": int,
+    },
+)
+_OptionalCreateMonitorInputRequestTypeDef = TypedDict(
+    "_OptionalCreateMonitorInputRequestTypeDef",
+    {
+        "Resources": Sequence[str],
+        "ClientToken": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateMonitorInputRequestTypeDef(
+    _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
+):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -104,24 +122,14 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
-S3ConfigTypeDef = TypedDict(
-    "S3ConfigTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "LogDeliveryStatus": LogDeliveryStatusType,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -142,21 +150,19 @@
         "NextToken": str,
         "MaxResults": int,
         "EventStatus": HealthEventStatusType,
     },
     total=False,
 )
 
-
 class ListHealthEventsInputRequestTypeDef(
     _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
 ):
     pass
 
-
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -175,19 +181,17 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
-
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -221,23 +225,63 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateMonitorInputRequestTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateMonitorInputRequestTypeDef",
+    {
+        "ResourcesToAdd": Sequence[str],
+        "ResourcesToRemove": Sequence[str],
+        "Status": MonitorConfigStateType,
+        "ClientToken": str,
+        "MaxCityNetworksToMonitor": int,
+    },
+    total=False,
+)
+
+class UpdateMonitorInputRequestTypeDef(
+    _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
+):
+    pass
+
 CreateMonitorOutputTypeDef = TypedDict(
     "CreateMonitorOutputTypeDef",
     {
         "Arn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -247,22 +291,14 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InternetMeasurementsLogDeliveryTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryTypeDef",
-    {
-        "S3Config": S3ConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
@@ -272,22 +308,20 @@
         "EndTime": Union[datetime, str],
         "EventStatus": HealthEventStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListHealthEventsInputListHealthEventsPaginateTypeDef(
     _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
     _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
 ):
     pass
 
-
 ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     {
         "MonitorStatus": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -318,86 +352,14 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMonitorInputRequestTypeDef = TypedDict(
-    "_RequiredCreateMonitorInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalCreateMonitorInputRequestTypeDef = TypedDict(
-    "_OptionalCreateMonitorInputRequestTypeDef",
-    {
-        "Resources": Sequence[str],
-        "ClientToken": str,
-        "Tags": Mapping[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-    },
-    total=False,
-)
-
-
-class CreateMonitorInputRequestTypeDef(
-    _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
-):
-    pass
-
-
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateMonitorInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateMonitorInputRequestTypeDef",
-    {
-        "ResourcesToAdd": Sequence[str],
-        "ResourcesToRemove": Sequence[str],
-        "Status": MonitorConfigStateType,
-        "ClientToken": str,
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-    },
-    total=False,
-)
-
-
-class UpdateMonitorInputRequestTypeDef(
-    _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
-):
-    pass
-
-
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -425,19 +387,17 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
-
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
-
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
@@ -469,19 +429,17 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
     },
     total=False,
 )
 
-
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
-
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor/type_defs.pyi` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,53 +14,51 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
-    LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AvailabilityMeasurementTypeDef",
+    "CreateMonitorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
-    "S3ConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "NetworkTypeDef",
     "RoundTripTimeTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "UpdateMonitorInputRequestTypeDef",
     "CreateMonitorOutputTypeDef",
+    "GetMonitorOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
-    "InternetMeasurementsLogDeliveryTypeDef",
     "ListHealthEventsInputListHealthEventsPaginateTypeDef",
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "CreateMonitorInputRequestTypeDef",
-    "GetMonitorOutputTypeDef",
-    "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
 
@@ -70,14 +68,38 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
+_RequiredCreateMonitorInputRequestTypeDef = TypedDict(
+    "_RequiredCreateMonitorInputRequestTypeDef",
+    {
+        "MonitorName": str,
+        "MaxCityNetworksToMonitor": int,
+    },
+)
+_OptionalCreateMonitorInputRequestTypeDef = TypedDict(
+    "_OptionalCreateMonitorInputRequestTypeDef",
+    {
+        "Resources": Sequence[str],
+        "ClientToken": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateMonitorInputRequestTypeDef(
+    _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
+):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -103,24 +125,14 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
-S3ConfigTypeDef = TypedDict(
-    "S3ConfigTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "LogDeliveryStatus": LogDeliveryStatusType,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -141,19 +153,21 @@
         "NextToken": str,
         "MaxResults": int,
         "EventStatus": HealthEventStatusType,
     },
     total=False,
 )
 
+
 class ListHealthEventsInputRequestTypeDef(
     _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
 ):
     pass
 
+
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -172,17 +186,19 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
+
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -216,23 +232,65 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateMonitorInputRequestTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateMonitorInputRequestTypeDef",
+    {
+        "ResourcesToAdd": Sequence[str],
+        "ResourcesToRemove": Sequence[str],
+        "Status": MonitorConfigStateType,
+        "ClientToken": str,
+        "MaxCityNetworksToMonitor": int,
+    },
+    total=False,
+)
+
+
+class UpdateMonitorInputRequestTypeDef(
+    _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
+):
+    pass
+
+
 CreateMonitorOutputTypeDef = TypedDict(
     "CreateMonitorOutputTypeDef",
     {
         "Arn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -242,22 +300,14 @@
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InternetMeasurementsLogDeliveryTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryTypeDef",
-    {
-        "S3Config": S3ConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
     "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
@@ -267,20 +317,22 @@
         "EndTime": Union[datetime, str],
         "EventStatus": HealthEventStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListHealthEventsInputListHealthEventsPaginateTypeDef(
     _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
     _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
 ):
     pass
 
+
 ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
     "ListMonitorsInputListMonitorsPaginateTypeDef",
     {
         "MonitorStatus": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -311,82 +363,14 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMonitorInputRequestTypeDef = TypedDict(
-    "_RequiredCreateMonitorInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalCreateMonitorInputRequestTypeDef = TypedDict(
-    "_OptionalCreateMonitorInputRequestTypeDef",
-    {
-        "Resources": Sequence[str],
-        "ClientToken": str,
-        "Tags": Mapping[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-    },
-    total=False,
-)
-
-class CreateMonitorInputRequestTypeDef(
-    _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
-):
-    pass
-
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateMonitorInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateMonitorInputRequestTypeDef",
-    {
-        "ResourcesToAdd": Sequence[str],
-        "ResourcesToRemove": Sequence[str],
-        "Status": MonitorConfigStateType,
-        "ClientToken": str,
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
-        "TrafficPercentageToMonitor": int,
-    },
-    total=False,
-)
-
-class UpdateMonitorInputRequestTypeDef(
-    _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
-):
-    pass
-
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -414,17 +398,19 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
+
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
+
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
@@ -456,17 +442,19 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
     },
     total=False,
 )
 
+
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
+
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/PKG-INFO` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.26.115
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.26.115 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.80
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-internetmonitor"></a>
 
 # mypy-boto3-internetmonitor
 
 [![PyPI - mypy-boto3-internetmonitor](https://img.shields.io/pypi/v/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-internetmonitor?color=blue)](https://pypistats.org/packages/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.26.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,15 +303,14 @@
 
 ```python
 from mypy_boto3_internetmonitor.literals import (
     HealthEventImpactTypeType,
     HealthEventStatusType,
     ListHealthEventsPaginatorName,
     ListMonitorsPaginatorName,
-    LogDeliveryStatusType,
     MonitorConfigStateType,
     MonitorProcessingStatusCodeType,
     TriangulationEventTypeType,
     CloudWatchInternetMonitorServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
@@ -329,40 +328,38 @@
 
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
+    CreateMonitorInputRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    S3ConfigTypeDef,
     PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     NetworkTypeDef,
     RoundTripTimeTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    UpdateMonitorInputRequestTypeDef,
     CreateMonitorOutputTypeDef,
+    GetMonitorOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsInputListHealthEventsPaginateTypeDef,
     ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    CreateMonitorInputRequestTypeDef,
-    GetMonitorOutputTypeDef,
-    UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
@@ -374,42 +371,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-internetmonitor-1.26.115/mypy_boto3_internetmonitor.egg-info/SOURCES.txt` & `mypy-boto3-internetmonitor-1.26.80/mypy_boto3_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.26.115/setup.py` & `mypy-boto3-internetmonitor-1.26.80/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-internetmonitor.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-internetmonitor",
-    version="1.26.115",
+    version="1.26.80",
     packages=["mypy_boto3_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.26.115 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.26.80 service generated with"
+        " mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

