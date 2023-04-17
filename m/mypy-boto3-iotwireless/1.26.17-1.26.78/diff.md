# Comparing `tmp/mypy-boto3-iotwireless-1.26.17.tar.gz` & `tmp/mypy-boto3-iotwireless-1.26.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.26.17.tar", last modified: Mon Nov 28 04:09:27 2022, max compression
+gzip compressed data, was "mypy-boto3-iotwireless-1.26.78.tar", last modified: Thu Feb 23 20:34:57 2023, max compression
```

## Comparing `mypy-boto3-iotwireless-1.26.17.tar` & `mypy-boto3-iotwireless-1.26.78.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.484745 mypy-boto3-iotwireless-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    24131 2022-11-28 04:09:27.484745 mypy-boto3-iotwireless-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22678 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.480745 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      924 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    66109 2022-11-28 04:08:52.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    66001 2022-11-28 04:08:52.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10953 2022-11-28 04:08:52.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10951 2022-11-28 04:08:52.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    86953 2022-11-28 04:08:54.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    86874 2022-11-28 04:08:53.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:27.484745 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    24131 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      683 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-11-28 04:09:27.000000 mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:27.484745 mypy-boto3-iotwireless-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2022-11-28 04:08:51.000000 mypy-boto3-iotwireless-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.316421 mypy-boto3-iotwireless-1.26.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24180 2023-02-23 20:34:57.316421 mypy-boto3-iotwireless-1.26.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.308421 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66339 2023-02-23 20:34:33.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66231 2023-02-23 20:34:33.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-02-23 20:34:33.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-02-23 20:34:33.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87262 2023-02-23 20:34:35.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87183 2023-02-23 20:34:34.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:34:57.316421 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24180 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-23 20:34:57.000000 mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:34:57.316421 mypy-boto3-iotwireless-1.26.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-23 20:34:32.000000 mypy-boto3-iotwireless-1.26.78/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.26.17/LICENSE` & `mypy-boto3-iotwireless-1.26.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.26.17/PKG-INFO` & `mypy-boto3-iotwireless-1.26.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.26.17
-Summary: Type annotations for boto3.IoTWireless 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.78
+Summary: Type annotations for boto3.IoTWireless 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.26.17/README.md` & `mypy-boto3-iotwireless-1.26.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/__main__.py` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.26.17\nVersion:         1.26.17\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.IoTWireless 1.26.78\nVersion:         1.26.78\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.26.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/client.py` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,18 @@
         *,
         FirmwareUpdateImage: str,
         FirmwareUpdateRole: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        RedundancyPercent: int = ...,
+        FragmentSizeBytes: int = ...,
+        FragmentIntervalMS: int = ...
     ) -> CreateFuotaTaskResponseTypeDef:
         """
         Creates a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_fuota_task)
         """
@@ -1185,15 +1188,18 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         FirmwareUpdateImage: str = ...,
-        FirmwareUpdateRole: str = ...
+        FirmwareUpdateRole: str = ...,
+        RedundancyPercent: int = ...,
+        FragmentSizeBytes: int = ...,
+        FragmentIntervalMS: int = ...
     ) -> Dict[str, Any]:
         """
         Updates properties of a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/client.pyi` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,18 @@
         *,
         FirmwareUpdateImage: str,
         FirmwareUpdateRole: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        RedundancyPercent: int = ...,
+        FragmentSizeBytes: int = ...,
+        FragmentIntervalMS: int = ...
     ) -> CreateFuotaTaskResponseTypeDef:
         """
         Creates a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_fuota_task)
         """
@@ -1086,15 +1089,18 @@
         self,
         *,
         Id: str,
         Name: str = ...,
         Description: str = ...,
         LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,
         FirmwareUpdateImage: str = ...,
-        FirmwareUpdateRole: str = ...
+        FirmwareUpdateRole: str = ...,
+        RedundancyPercent: int = ...,
+        FragmentSizeBytes: int = ...,
+        FragmentIntervalMS: int = ...
     ) -> Dict[str, Any]:
         """
         Updates properties of a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/literals.py` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -163,27 +164,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
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
+    "cloudtrail-data",
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
@@ -212,14 +216,15 @@
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
@@ -286,30 +291,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
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
@@ -342,28 +350,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -391,30 +402,34 @@
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
@@ -430,14 +445,15 @@
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

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/literals.pyi` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
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
@@ -161,27 +162,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
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
+    "cloudtrail-data",
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
@@ -210,14 +214,15 @@
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
@@ -284,30 +289,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
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
@@ -340,28 +348,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
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
@@ -389,30 +400,34 @@
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
@@ -428,14 +443,15 @@
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

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/type_defs.py` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2137,14 +2137,17 @@
     "_OptionalCreateFuotaTaskRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "ClientRequestToken": str,
         "LoRaWAN": LoRaWANFuotaTaskTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
     },
     total=False,
 )
 
 
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
@@ -2162,14 +2165,17 @@
     "_OptionalUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANFuotaTaskTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
     },
     total=False,
 )
 
 
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
@@ -2420,14 +2426,17 @@
         "Status": FuotaTaskStatusType,
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless/type_defs.pyi` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2100,14 +2100,17 @@
     "_OptionalCreateFuotaTaskRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "ClientRequestToken": str,
         "LoRaWAN": LoRaWANFuotaTaskTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
     },
     total=False,
 )
 
 class CreateFuotaTaskRequestRequestTypeDef(
     _RequiredCreateFuotaTaskRequestRequestTypeDef, _OptionalCreateFuotaTaskRequestRequestTypeDef
 ):
@@ -2123,14 +2126,17 @@
     "_OptionalUpdateFuotaTaskRequestRequestTypeDef",
     {
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANFuotaTaskTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
     },
     total=False,
 )
 
 class UpdateFuotaTaskRequestRequestTypeDef(
     _RequiredUpdateFuotaTaskRequestRequestTypeDef, _OptionalUpdateFuotaTaskRequestRequestTypeDef
 ):
@@ -2371,14 +2377,17 @@
         "Status": FuotaTaskStatusType,
         "Name": str,
         "Description": str,
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
+        "RedundancyPercent": int,
+        "FragmentSizeBytes": int,
+        "FragmentIntervalMS": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.26.17
-Summary: Type annotations for boto3.IoTWireless 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.78
+Summary: Type annotations for boto3.IoTWireless 1.26.78 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotwireless.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotwireless?color=blue)](https://pypistats.org/packages/mypy-boto3-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTWireless 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
+[boto3.IoTWireless 1.26.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.26.17/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy-boto3-iotwireless-1.26.78/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.26.17/setup.py` & `mypy-boto3-iotwireless-1.26.78/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.26.17",
+    version="1.26.78",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTWireless 1.26.17 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.IoTWireless 1.26.78 service generated with mypy-boto3-builder"
+        " 7.12.4"
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
     keywords="boto3 iotwireless type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_iotwireless": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_iotwireless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

