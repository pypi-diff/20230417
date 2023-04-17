# Comparing `tmp/iris_pex_embedded_python-2.0.1.tar.gz` & `tmp/iris_pex_embedded_python-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.0.1.tar", last modified: Fri Dec 16 16:10:17 2022, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.0.2.tar", last modified: Mon Apr 17 12:59:31 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.0.1.tar` & `iris_pex_embedded_python-2.0.2.tar`

### file list

```diff
@@ -1,57 +1,34 @@
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.128715 iris_pex_embedded_python-2.0.1/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.0.1/LICENSE
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35132 2022-12-16 16:10:17.128059 iris_pex_embedded_python-2.0.1/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    34254 2022-07-25 12:05:54.000000 iris_pex_embedded_python-2.0.1/README.md
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-15 09:05:00.000000 iris_pex_embedded_python-2.0.1/pyproject.toml
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2022-12-16 16:10:17.128956 iris_pex_embedded_python-2.0.1/setup.cfg
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1963 2022-12-16 16:09:06.000000 iris_pex_embedded_python-2.0.1/setup.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.054916 iris_pex_embedded_python-2.0.1/src/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.054174 iris_pex_embedded_python-2.0.1/src/grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.094643 iris_pex_embedded_python-2.0.1/src/grongier/iris/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.051334 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.081591 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      929 2022-07-11 08:43:06.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/BusinessOperation.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2615 2022-05-24 09:27:16.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/BusinessProcess.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1036 2022-05-11 12:48:11.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/BusinessService.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3282 2022-05-11 12:48:11.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Common.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      535 2022-12-14 15:47:59.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Director.cls
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.086590 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Duplex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      540 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Duplex/Operation.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7078 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Duplex/Process.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      179 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Duplex/Service.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      628 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/InboundAdapter.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8224 2022-07-12 13:24:38.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Message.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      973 2022-07-04 09:23:01.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/OutboundAdapter.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1691 2022-06-08 15:54:15.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PickleMessage.cls
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.088033 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8046 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Duplex.cls
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.093310 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Message/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      986 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Message/Ack.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      987 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Message/Poll.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      994 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Message/Start.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1435 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/PrivateSession/Message/Stop.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      546 2022-05-11 12:48:11.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Python.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1622 2022-05-11 12:48:11.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Test.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    12214 2022-10-06 19:17:50.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/Grongier/PEX/Utils.cls
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 14:04:47.000000 iris_pex_embedded_python-2.0.1/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.119244 iris_pex_embedded_python-2.0.1/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1138 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    19811 2022-12-16 16:02:41.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2022-07-13 11:46:16.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2022-07-19 14:30:32.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    14889 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3840 2022-05-11 12:46:53.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2022-07-13 11:27:14.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2022-05-24 12:26:05.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2022-07-13 11:28:33.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2022-06-08 14:40:43.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2022-07-25 14:16:24.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     6228 2022-12-16 14:11:00.000000 iris_pex_embedded_python-2.0.1/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:10:17.126701 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35132 2022-12-16 16:10:16.000000 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2900 2022-12-16 16:10:16.000000 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2022-12-16 16:10:16.000000 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       14 2022-12-16 16:10:16.000000 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2022-12-16 16:10:16.000000 iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.821010 iris_pex_embedded_python-2.0.2/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.0.2/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-17 12:59:31.820076 iris_pex_embedded_python-2.0.2/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.2/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.2/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-17 12:59:31.821247 iris_pex_embedded_python-2.0.2/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-17 12:54:41.000000 iris_pex_embedded_python-2.0.2/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.777791 iris_pex_embedded_python-2.0.2/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.777261 iris_pex_embedded_python-2.0.2/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.784283 iris_pex_embedded_python-2.0.2/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.806054 iris_pex_embedded_python-2.0.2/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1138 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    19811 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112    14889 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     6228 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.2/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.814906 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112      845 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-17 12:59:31.000000 iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-17 12:59:31.817317 iris_pex_embedded_python-2.0.2/test/
+-rw-r--r--   0 grongier (902446405) 1252422112      273 2023-01-06 14:56:27.000000 iris_pex_embedded_python-2.0.2/test/test_selectt.py
```

### Comparing `iris_pex_embedded_python-2.0.1/LICENSE` & `iris_pex_embedded_python-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/PKG-INFO` & `iris_pex_embedded_python-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: iris_pex_embedded_python
-Version: 2.0.1
-Summary: iris_pex_embedded_python
-Home-page: https://github.com/grongierisc/interoperability-embedded-python
-Author: grongier
-Author-email: guillaume.rongier@intersystems.com
-License: MIT
-Keywords: iris_pex_embedded_python
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -34,14 +10,16 @@
   - [1.3. Register a component](#13-register-a-component)
 - [2. Demo](#2-demo)
 - [3. Prerequisites](#3-prerequisites)
 - [4. Installation](#4-installation)
   - [4.1. With Docker](#41-with-docker)
   - [4.2. Without Docker](#42-without-docker)
   - [4.3. With ZPM](#43-with-zpm)
+  - [4.4. With PyPI](#44-with-pypi)
+    - [4.4.1. Known issues](#441-known-issues)
 - [5. How to Run the Sample](#5-how-to-run-the-sample)
   - [5.1. Docker containers](#51-docker-containers)
   - [5.2. Management Portal and VSCode](#52-management-portal-and-vscode)
   - [5.3. Open the production](#53-open-the-production)
 - [6. What's inside the repository](#6-whats-inside-the-repository)
   - [6.1. Dockerfile](#61-dockerfile)
   - [6.2. .vscode/settings.json](#62-vscodesettingsjson)
@@ -59,17 +37,17 @@
   - [7.8. The `business_operation` class](#78-the-business_operation-class)
     - [7.8.1. The dispacth system](#781-the-dispacth-system)
     - [7.8.2. The methods](#782-the-methods)
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
-    - [7.12.1. register_component](#7121-register_component)
-    - [7.12.2. register_file](#7122-register_file)
-    - [7.12.3. register_folder](#7123-register_folder)
+    - [7.12.1. register\_component](#7121-register_component)
+    - [7.12.2. register\_file](#7122-register_file)
+    - [7.12.3. register\_folder](#7123-register_folder)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -195,14 +173,43 @@
 ```
 ## 4.3. With ZPM 
 
 ```objectscript
 zpm "install pex-embbeded-python" 
 ```
 
+## 4.4. With PyPI
+
+```sh
+pip3 install iris_pex_embedded_python
+```
+
+Import the ObjectScript classes, open an embedded python shell and run :
+
+```python
+from grongier.pex import Utils
+Utils.setup()
+```
+
+### 4.4.1. Known issues
+
+If the module is not updated, make sure to remove the old version :
+
+```sh
+pip3 uninstall iris_pex_embedded_python
+```
+
+or manually remove the `grongier` folder in `<iris_installation>/lib/python/`
+
+or force the installation with pip :
+
+```sh
+pip3 install --upgrade iris_pex_embedded_python --target <iris_installation>/lib/python/
+```
+
 # 5. How to Run the Sample
 
 ## 5.1. Docker containers
 
 
 In order to have access to the InterSystems images, we need to go to the following url: http://container.intersystems.com. After connecting with our InterSystems credentials, we will get our password to connect to the registry. In the docker VScode addon, in the image tab, by pressing connect registry and entering the same url as before (http://container.intersystems.com) as a generic registry, we will be asked to give our credentials. The login is the usual one but the password is the one we got from the website.
 
@@ -827,9 +834,8 @@
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
-
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.0.1/README.md` & `iris_pex_embedded_python-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: iris_pex_embedded_python
+Version: 2.0.2
+Summary: iris_pex_embedded_python
+Home-page: https://github.com/grongierisc/interoperability-embedded-python
+Author: grongier
+Author-email: guillaume.rongier@intersystems.com
+License: MIT
+Keywords: iris_pex_embedded_python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -10,14 +34,16 @@
   - [1.3. Register a component](#13-register-a-component)
 - [2. Demo](#2-demo)
 - [3. Prerequisites](#3-prerequisites)
 - [4. Installation](#4-installation)
   - [4.1. With Docker](#41-with-docker)
   - [4.2. Without Docker](#42-without-docker)
   - [4.3. With ZPM](#43-with-zpm)
+  - [4.4. With PyPI](#44-with-pypi)
+    - [4.4.1. Known issues](#441-known-issues)
 - [5. How to Run the Sample](#5-how-to-run-the-sample)
   - [5.1. Docker containers](#51-docker-containers)
   - [5.2. Management Portal and VSCode](#52-management-portal-and-vscode)
   - [5.3. Open the production](#53-open-the-production)
 - [6. What's inside the repository](#6-whats-inside-the-repository)
   - [6.1. Dockerfile](#61-dockerfile)
   - [6.2. .vscode/settings.json](#62-vscodesettingsjson)
@@ -35,17 +61,17 @@
   - [7.8. The `business_operation` class](#78-the-business_operation-class)
     - [7.8.1. The dispacth system](#781-the-dispacth-system)
     - [7.8.2. The methods](#782-the-methods)
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
-    - [7.12.1. register_component](#7121-register_component)
-    - [7.12.2. register_file](#7122-register_file)
-    - [7.12.3. register_folder](#7123-register_folder)
+    - [7.12.1. register\_component](#7121-register_component)
+    - [7.12.2. register\_file](#7122-register_file)
+    - [7.12.3. register\_folder](#7123-register_folder)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -171,14 +197,43 @@
 ```
 ## 4.3. With ZPM 
 
 ```objectscript
 zpm "install pex-embbeded-python" 
 ```
 
+## 4.4. With PyPI
+
+```sh
+pip3 install iris_pex_embedded_python
+```
+
+Import the ObjectScript classes, open an embedded python shell and run :
+
+```python
+from grongier.pex import Utils
+Utils.setup()
+```
+
+### 4.4.1. Known issues
+
+If the module is not updated, make sure to remove the old version :
+
+```sh
+pip3 uninstall iris_pex_embedded_python
+```
+
+or manually remove the `grongier` folder in `<iris_installation>/lib/python/`
+
+or force the installation with pip :
+
+```sh
+pip3 install --upgrade iris_pex_embedded_python --target <iris_installation>/lib/python/
+```
+
 # 5. How to Run the Sample
 
 ## 5.1. Docker containers
 
 
 In order to have access to the InterSystems images, we need to go to the following url: http://container.intersystems.com. After connecting with our InterSystems credentials, we will get our password to connect to the registry. In the docker VScode addon, in the image tab, by pressing connect registry and entering the same url as before (http://container.intersystems.com) as a generic registry, we will be asked to give our credentials. The login is the usual one but the password is the one we got from the website.
 
@@ -803,8 +858,8 @@
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.0.1/setup.py` & `iris_pex_embedded_python-2.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,36 +22,37 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.0.1',
+        version='2.0.2',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
+            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Topic :: Utilities'
         ],
         package_dir={'': 'src'},
         packages=['grongier.pex','grongier.iris'],
         include_package_data=True,
-        python_requires='>=3.7',
+        python_requires='>=3.6',
         install_requires=[
             "dacite>=1.6.0",
         ]
     )
 
 
 if __name__ == '__main__':
```

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.0.2/src/grongier/pex/_utils.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.1/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.0.2/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.0.1
+Version: 2.0.2
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
@@ -34,14 +34,16 @@
   - [1.3. Register a component](#13-register-a-component)
 - [2. Demo](#2-demo)
 - [3. Prerequisites](#3-prerequisites)
 - [4. Installation](#4-installation)
   - [4.1. With Docker](#41-with-docker)
   - [4.2. Without Docker](#42-without-docker)
   - [4.3. With ZPM](#43-with-zpm)
+  - [4.4. With PyPI](#44-with-pypi)
+    - [4.4.1. Known issues](#441-known-issues)
 - [5. How to Run the Sample](#5-how-to-run-the-sample)
   - [5.1. Docker containers](#51-docker-containers)
   - [5.2. Management Portal and VSCode](#52-management-portal-and-vscode)
   - [5.3. Open the production](#53-open-the-production)
 - [6. What's inside the repository](#6-whats-inside-the-repository)
   - [6.1. Dockerfile](#61-dockerfile)
   - [6.2. .vscode/settings.json](#62-vscodesettingsjson)
@@ -59,17 +61,17 @@
   - [7.8. The `business_operation` class](#78-the-business_operation-class)
     - [7.8.1. The dispacth system](#781-the-dispacth-system)
     - [7.8.2. The methods](#782-the-methods)
   - [7.9. The `director` class](#79-the-director-class)
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
-    - [7.12.1. register_component](#7121-register_component)
-    - [7.12.2. register_file](#7122-register_file)
-    - [7.12.3. register_folder](#7123-register_folder)
+    - [7.12.1. register\_component](#7121-register_component)
+    - [7.12.2. register\_file](#7122-register_file)
+    - [7.12.3. register\_folder](#7123-register_folder)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
 - [8. Credits](#8-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
@@ -195,14 +197,43 @@
 ```
 ## 4.3. With ZPM 
 
 ```objectscript
 zpm "install pex-embbeded-python" 
 ```
 
+## 4.4. With PyPI
+
+```sh
+pip3 install iris_pex_embedded_python
+```
+
+Import the ObjectScript classes, open an embedded python shell and run :
+
+```python
+from grongier.pex import Utils
+Utils.setup()
+```
+
+### 4.4.1. Known issues
+
+If the module is not updated, make sure to remove the old version :
+
+```sh
+pip3 uninstall iris_pex_embedded_python
+```
+
+or manually remove the `grongier` folder in `<iris_installation>/lib/python/`
+
+or force the installation with pip :
+
+```sh
+pip3 install --upgrade iris_pex_embedded_python --target <iris_installation>/lib/python/
+```
+
 # 5. How to Run the Sample
 
 ## 5.1. Docker containers
 
 
 In order to have access to the InterSystems images, we need to go to the following url: http://container.intersystems.com. After connecting with our InterSystems credentials, we will get our password to connect to the registry. In the docker VScode addon, in the image tab, by pressing connect registry and entering the same url as before (http://container.intersystems.com) as a generic registry, we will be asked to give our credentials. The login is the usual one but the password is the one we got from the website.
 
@@ -828,8 +859,7 @@
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
 Works only on IRIS 2021.2 +
-
```

