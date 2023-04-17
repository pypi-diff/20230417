# Comparing `tmp/mypy-boto3-appflow-1.26.53.tar.gz` & `tmp/mypy-boto3-appflow-1.26.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.26.53.tar", last modified: Thu Jan 19 22:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.26.53.tar` & `mypy-boto3-appflow-1.26.78.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:39.033057 mypy-boto3-appflow-1.26.53/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-01-19 22:27:39.029057 mypy-boto3-appflow-1.26.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:39.029057 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-01-19 22:25:54.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-01-19 22:25:54.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68323 2023-01-19 22:25:55.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68227 2023-01-19 22:25:55.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 22:27:39.029057 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-19 22:27:38.000000 mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 22:27:39.033057 mypy-boto3-appflow-1.26.53/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-19 22:25:53.000000 mypy-boto3-appflow-1.26.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-02-23 20:34:20.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68382 2023-02-23 20:34:22.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68286 2023-02-23 20:34:21.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 20:34:57.000000 mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.308421 mypy-boto3-appflow-1.26.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-23 20:34:19.000000 mypy-boto3-appflow-1.26.78/setup.py
```

### Comparing `mypy-boto3-appflow-1.26.53/LICENSE` & `mypy-boto3-appflow-1.26.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.26.53/PKG-INFO` & `mypy-boto3-appflow-1.26.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.26.53
-Summary: Type annotations for boto3.Appflow 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.26.53/README.md` & `mypy-boto3-appflow-1.26.78/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.26.53\nVersion:         1.26.53\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Appflow 1.26.78\nVersion:         1.26.78\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.53")
+    print("1.26.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,14 +516,15 @@
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
@@ -785,14 +786,15 @@
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

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -514,14 +514,15 @@
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
@@ -783,14 +784,15 @@
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

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,14 +600,15 @@
 
 
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
+        "usePrivateLinkForMetadataAndAuthorization": bool,
     },
     total=False,
 )
 
 ServiceNowConnectorProfilePropertiesTypeDef = TypedDict(
     "ServiceNowConnectorProfilePropertiesTypeDef",
     {
```

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -593,14 +593,15 @@
     pass
 
 SalesforceConnectorProfilePropertiesTypeDef = TypedDict(
     "SalesforceConnectorProfilePropertiesTypeDef",
     {
         "instanceUrl": str,
         "isSandboxEnvironment": bool,
+        "usePrivateLinkForMetadataAndAuthorization": bool,
     },
     total=False,
 )
 
 ServiceNowConnectorProfilePropertiesTypeDef = TypedDict(
     "ServiceNowConnectorProfilePropertiesTypeDef",
     {
```

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.26.53
-Summary: Type annotations for boto3.Appflow 1.26.53 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.78
+Summary: Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appflow.svg?color=blue)](https://pypi.org/project/mypy-boto3-appflow)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appflow?color=blue)](https://pypistats.org/packages/mypy-boto3-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Appflow 1.26.53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[boto3.Appflow 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.26.53/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.26.78/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.26.53/setup.py` & `mypy-boto3-appflow-1.26.78/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.26.53",
+    version="1.26.78",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Appflow 1.26.53 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Appflow 1.26.78 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

