# Comparing `tmp/mypy-boto3-drs-1.26.17.tar.gz` & `tmp/mypy-boto3-drs-1.26.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.26.17.tar", last modified: Mon Nov 28 04:09:25 2022, max compression
+gzip compressed data, was "mypy-boto3-drs-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
```

## Comparing `mypy-boto3-drs-1.26.17.tar` & `mypy-boto3-drs-1.26.80.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.520745 mypy-boto3-drs-1.26.17/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    19578 2022-11-28 04:09:25.520745 mypy-boto3-drs-1.26.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18157 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.516745 mypy-boto3-drs-1.26.17/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      892 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30538 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    30488 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15294 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    15292 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10424 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10414 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    44576 2022-11-28 04:08:36.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    44537 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 04:09:25.516745 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19578 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      604 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-28 04:09:25.000000 mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 04:09:25.520745 mypy-boto3-drs-1.26.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1925 2022-11-28 04:08:35.000000 mypy-boto3-drs-1.26.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.144039 mypy-boto3-drs-1.26.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-02-27 20:35:29.140040 mypy-boto3-drs-1.26.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18156 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.132040 mypy-boto3-drs-1.26.80/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30488 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15681 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-02-27 20:35:04.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-02-27 20:35:05.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44692 2023-02-27 20:35:05.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.140040 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-27 20:35:28.000000 mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.144039 mypy-boto3-drs-1.26.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-27 20:35:03.000000 mypy-boto3-drs-1.26.80/setup.py
```

### Comparing `mypy-boto3-drs-1.26.17/LICENSE` & `mypy-boto3-drs-1.26.80/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/PKG-INFO` & `mypy-boto3-drs-1.26.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.26.17
-Summary: Type annotations for boto3.drs 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.80
+Summary: Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.26.17/README.md` & `mypy-boto3-drs-1.26.80/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.26.17\nVersion:         1.26.17\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.drs 1.26.80\nVersion:         1.26.80\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.17")
+    print("1.26.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,14 +258,15 @@
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
@@ -276,27 +277,30 @@
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
@@ -325,14 +329,15 @@
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
@@ -377,14 +382,15 @@
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
@@ -399,30 +405,33 @@
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
@@ -455,28 +464,31 @@
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
@@ -504,30 +516,34 @@
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
@@ -543,14 +559,15 @@
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

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -256,14 +256,15 @@
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
@@ -274,27 +275,30 @@
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
@@ -323,14 +327,15 @@
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
@@ -375,14 +380,15 @@
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
@@ -397,30 +403,33 @@
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
@@ -453,28 +462,31 @@
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
@@ -502,30 +514,34 @@
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
@@ -541,14 +557,15 @@
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

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1213,14 +1213,15 @@
     pass
 
 
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
+        "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
@@ -1373,14 +1374,15 @@
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[DataReplicationInfoReplicatedDiskTypeDef],
+        "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
@@ -1431,14 +1433,15 @@
     {
         "dataReplicationError": RecoveryInstanceDataReplicationErrorTypeDef,
         "dataReplicationInitiation": RecoveryInstanceDataReplicationInitiationTypeDef,
         "dataReplicationState": RecoveryInstanceDataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef],
+        "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
@@ -1492,14 +1495,15 @@
         "arn": str,
         "dataReplicationInfo": RecoveryInstanceDataReplicationInfoTypeDef,
         "ec2InstanceID": str,
         "ec2InstanceState": EC2InstanceStateType,
         "failback": RecoveryInstanceFailbackTypeDef,
         "isDrill": bool,
         "jobID": str,
+        "originAvailabilityZone": str,
         "originEnvironment": OriginEnvironmentType,
         "pointInTimeSnapshotDateTime": str,
         "recoveryInstanceID": str,
         "recoveryInstanceProperties": RecoveryInstancePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
     },
```

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1178,14 +1178,15 @@
 ):
     pass
 
 LifeCycleLastLaunchTypeDef = TypedDict(
     "LifeCycleLastLaunchTypeDef",
     {
         "initiated": LifeCycleLastLaunchInitiatedTypeDef,
+        "status": LaunchStatusType,
     },
     total=False,
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
@@ -1334,14 +1335,15 @@
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
         "dataReplicationInitiation": DataReplicationInitiationTypeDef,
         "dataReplicationState": DataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[DataReplicationInfoReplicatedDiskTypeDef],
+        "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
@@ -1392,14 +1394,15 @@
     {
         "dataReplicationError": RecoveryInstanceDataReplicationErrorTypeDef,
         "dataReplicationInitiation": RecoveryInstanceDataReplicationInitiationTypeDef,
         "dataReplicationState": RecoveryInstanceDataReplicationStateType,
         "etaDateTime": str,
         "lagDuration": str,
         "replicatedDisks": List[RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef],
+        "stagingAvailabilityZone": str,
     },
     total=False,
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
@@ -1453,14 +1456,15 @@
         "arn": str,
         "dataReplicationInfo": RecoveryInstanceDataReplicationInfoTypeDef,
         "ec2InstanceID": str,
         "ec2InstanceState": EC2InstanceStateType,
         "failback": RecoveryInstanceFailbackTypeDef,
         "isDrill": bool,
         "jobID": str,
+        "originAvailabilityZone": str,
         "originEnvironment": OriginEnvironmentType,
         "pointInTimeSnapshotDateTime": str,
         "recoveryInstanceID": str,
         "recoveryInstanceProperties": RecoveryInstancePropertiesTypeDef,
         "sourceServerID": str,
         "tags": Dict[str, str],
     },
```

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.26.17
-Summary: Type annotations for boto3.drs 1.26.17 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.80
+Summary: Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
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
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-drs?color=blue)](https://pypistats.org/packages/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.26.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [mypy-boto3-drs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-drs-1.26.17/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.26.80/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.26.17/setup.py` & `mypy-boto3-drs-1.26.80/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.26.17",
+    version="1.26.80",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.26.17 service generated with mypy-boto3-builder 7.11.11"
+        "Type annotations for boto3.drs 1.26.80 service generated with mypy-boto3-builder 7.12.4"
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
     keywords="boto3 drs type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_drs": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_drs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

