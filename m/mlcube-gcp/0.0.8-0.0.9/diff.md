# Comparing `tmp/mlcube_gcp-0.0.8.tar.gz` & `tmp/mlcube_gcp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcube_gcp-0.0.8.tar", last modified: Wed Sep 21 22:31:35 2022, max compression
+gzip compressed data, was "mlcube_gcp-0.0.9.tar", last modified: Mon Apr 17 18:11:39 2023, max compression
```

## Comparing `mlcube_gcp-0.0.8.tar` & `mlcube_gcp-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.468953 mlcube_gcp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/mlcube_gcp/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/gcp_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/mlcube_gcp/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/mlcube_gcp/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/tests/test_data/platform_01.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/mlcube_gcp/tests/test_mlcube_gcp_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 22:31:35.464953 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-21 22:31:35.000000 mlcube_gcp-0.0.8/mlcube_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 22:31:35.468953 mlcube_gcp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-09-21 22:31:27.000000 mlcube_gcp-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/mlcube_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/gcp_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/mlcube_gcp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/mlcube_gcp/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/tests/test_data/platform_01.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/mlcube_gcp/tests/test_get_runner_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 18:11:39.000000 mlcube_gcp-0.0.9/mlcube_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:11:39.259864 mlcube_gcp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 18:11:25.000000 mlcube_gcp-0.0.9/setup.py
```

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/client.py` & `mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/client.py`

 * *Files identical despite different names*

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/instance.py` & `mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/instance.py`

 * *Files identical despite different names*

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/operation.py` & `mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/operation.py`

 * *Files identical despite different names*

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/gcp_client/service.py` & `mlcube_gcp-0.0.9/mlcube_gcp/gcp_client/service.py`

 * *Files identical despite different names*

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/gcp_run.py` & `mlcube_gcp-0.0.9/mlcube_gcp/gcp_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import logging
 import typing as t
 from pathlib import Path
 from omegaconf import (DictConfig, OmegaConf)
 from mlcube.validate import Validate
-from mlcube_ssh.ssh_run import Shell
+from mlcube.shell import Shell
 from ssh_config.client import (SSHConfig, Host)
 from mlcube.runner import (RunnerConfig, Runner)
 from mlcube.errors import ExecutionError
 from mlcube_gcp.gcp_client.instance import Instance as GCPInstance, Status as GCPInstanceStatus
 from mlcube_gcp.gcp_client.service import Service
```

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp/tests/test_data/platform_01.yaml` & `mlcube_gcp-0.0.9/mlcube_gcp/tests/test_data/platform_01.yaml`

 * *Files identical despite different names*

### Comparing `mlcube_gcp-0.0.8/mlcube_gcp.egg-info/SOURCES.txt` & `mlcube_gcp-0.0.9/mlcube_gcp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 mlcube_gcp.egg-info/top_level.txt
 mlcube_gcp/gcp_client/__init__.py
 mlcube_gcp/gcp_client/client.py
 mlcube_gcp/gcp_client/instance.py
 mlcube_gcp/gcp_client/operation.py
 mlcube_gcp/gcp_client/service.py
 mlcube_gcp/tests/__init__.py
-mlcube_gcp/tests/test_mlcube_gcp_cli.py
+mlcube_gcp/tests/test_get_runner_class.py
 mlcube_gcp/tests/test_data/platform_01.yaml
```

### Comparing `mlcube_gcp-0.0.8/setup.py` & `mlcube_gcp-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 extra_files = schemas()
 
 
 setup(
     name="mlcube_gcp",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(exclude=["tests"]),
     license="Apache 2.0",
     entry_points='''
         [console_scripts]
         mlcube_gcp=mlcube_gcp.__main__:cli
     ''',
     install_requires=requires,
```

