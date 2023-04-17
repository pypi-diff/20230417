# Comparing `tmp/deepdriver-0.9.4.tar.gz` & `tmp/deepdriver-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdriver-0.9.4.tar", last modified: Fri Feb 10 07:23:27 2023, max compression
+gzip compressed data, was "deepdriver-0.9.5.tar", last modified: Wed Feb 15 06:24:48 2023, max compression
```

## Comparing `deepdriver-0.9.4.tar` & `deepdriver-0.9.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.308374 deepdriver-0.9.4/
--rw-r--r--   0 root         (0) root         (0)     1068 2023-02-03 07:06:55.000000 deepdriver-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      897 2023-02-10 07:23:27.308374 deepdriver-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-02-03 07:06:55.000000 deepdriver-0.9.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.300376 deepdriver-0.9.4/deepdriver/
--rw-r--r--   0 root         (0) root         (0)     2226 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.300376 deepdriver-0.9.4/deepdriver/cli/
--rw-r--r--   0 root         (0) root         (0)     5786 2023-02-10 03:13:59.000000 deepdriver-0.9.4/deepdriver/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-02-10 03:13:59.000000 deepdriver-0.9.4/deepdriver/cli/cli_ctx.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-02-10 03:13:59.000000 deepdriver-0.9.4/deepdriver/cli/cli_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.296377 deepdriver-0.9.4/deepdriver/intergration/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.300376 deepdriver-0.9.4/deepdriver/intergration/keras/
--rw-r--r--   0 root         (0) root         (0)      669 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/intergration/keras/keras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.300376 deepdriver-0.9.4/deepdriver/intergration/torch/
--rw-r--r--   0 root         (0) root         (0)     5883 2023-02-03 07:07:24.000000 deepdriver-0.9.4/deepdriver/intergration/torch/torch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.300376 deepdriver-0.9.4/deepdriver/sdk/
--rw-r--r--   0 root         (0) root         (0)    17918 2023-02-10 05:28:10.000000 deepdriver-0.9.4/deepdriver/sdk/artifact.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.304375 deepdriver-0.9.4/deepdriver/sdk/chart/
--rw-r--r--   0 root         (0) root         (0)      432 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/bar.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-07 07:28:44.000000 deepdriver-0.9.4/deepdriver/sdk/chart/chart.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/confusion_matrix.py
--rw-r--r--   0 root         (0) root         (0)      735 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/histogram.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/line.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/roc_curve.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/chart/scatter.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.304375 deepdriver-0.9.4/deepdriver/sdk/data_types/
--rw-r--r--   0 root         (0) root         (0)     1809 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/boundingBoxes.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/dataFrame.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/experiment.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-02-10 06:46:24.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/image.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/media.py
--rw-r--r--   0 root         (0) root         (0)     5602 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/run.py
--rw-r--r--   0 root         (0) root         (0)     3828 2023-02-07 09:18:35.000000 deepdriver-0.9.4/deepdriver/sdk/data_types/table.py
--rw-r--r--   0 root         (0) root         (0)    11882 2023-02-07 08:11:50.000000 deepdriver-0.9.4/deepdriver/sdk/experiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.304375 deepdriver-0.9.4/deepdriver/sdk/interface/
--rw-r--r--   0 root         (0) root         (0)     8738 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/interface/grpc_interface_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13528 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4690 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/interface/http_interface.py
--rw-r--r--   0 root         (0) root         (0)    13132 2023-02-06 08:10:22.000000 deepdriver-0.9.4/deepdriver/sdk/interface/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.304375 deepdriver-0.9.4/deepdriver/sdk/lib/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/lib/lazyloader.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-02-06 08:10:22.000000 deepdriver-0.9.4/deepdriver/sdk/login.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/run.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/setting.py
--rw-r--r--   0 root         (0) root         (0)     3597 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/util.py
--rw-r--r--   0 root         (0) root         (0)     6637 2023-02-03 07:06:55.000000 deepdriver-0.9.4/deepdriver/sdk/visualization.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-02-03 07:07:24.000000 deepdriver-0.9.4/deepdriver/sdk/watch.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-10 07:23:15.000000 deepdriver-0.9.4/deepdriver/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 07:23:27.308374 deepdriver-0.9.4/deepdriver.egg-info/
--rw-r--r--   0 root         (0) root         (0)      897 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1452 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-10 07:23:27.000000 deepdriver-0.9.4/deepdriver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      252 2023-02-03 07:06:55.000000 deepdriver-0.9.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-10 07:23:27.308374 deepdriver-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-02-07 05:10:59.000000 deepdriver-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.246580 deepdriver-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-02-03 07:06:55.000000 deepdriver-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      897 2023-02-15 06:24:48.246580 deepdriver-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2023-02-03 07:06:55.000000 deepdriver-0.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.222586 deepdriver-0.9.5/deepdriver/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.222586 deepdriver-0.9.5/deepdriver/cli/
+-rw-r--r--   0 root         (0) root         (0)     7671 2023-02-14 02:05:12.000000 deepdriver-0.9.5/deepdriver/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-02-10 03:13:59.000000 deepdriver-0.9.5/deepdriver/cli/cli_ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-02-13 02:13:12.000000 deepdriver-0.9.5/deepdriver/cli/cli_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.214587 deepdriver-0.9.5/deepdriver/intergration/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.226585 deepdriver-0.9.5/deepdriver/intergration/keras/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/intergration/keras/keras.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.226585 deepdriver-0.9.5/deepdriver/intergration/torch/
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-02-03 07:07:24.000000 deepdriver-0.9.5/deepdriver/intergration/torch/torch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.230584 deepdriver-0.9.5/deepdriver/sdk/
+-rw-r--r--   0 root         (0) root         (0)    17918 2023-02-10 05:28:10.000000 deepdriver-0.9.5/deepdriver/sdk/artifact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.234583 deepdriver-0.9.5/deepdriver/sdk/chart/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/bar.py
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-02-14 02:22:02.000000 deepdriver-0.9.5/deepdriver/sdk/chart/chart.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/confusion_matrix.py
+-rw-r--r--   0 root         (0) root         (0)      735 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/histogram.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/line.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/roc_curve.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/chart/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.238582 deepdriver-0.9.5/deepdriver/sdk/data_types/
+-rw-r--r--   0 root         (0) root         (0)     1809 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/boundingBoxes.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/dataFrame.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-02-10 06:46:24.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/image.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/media.py
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-02-14 02:22:02.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/run.py
+-rw-r--r--   0 root         (0) root         (0)     4161 2023-02-14 02:22:02.000000 deepdriver-0.9.5/deepdriver/sdk/data_types/table.py
+-rw-r--r--   0 root         (0) root         (0)    12343 2023-02-13 02:01:22.000000 deepdriver-0.9.5/deepdriver/sdk/experiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.242581 deepdriver-0.9.5/deepdriver/sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)     8738 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/interface/grpc_interface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13528 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4690 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/interface/http_interface.py
+-rw-r--r--   0 root         (0) root         (0)    13132 2023-02-06 08:10:22.000000 deepdriver-0.9.5/deepdriver/sdk/interface/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.242581 deepdriver-0.9.5/deepdriver/sdk/lib/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/lib/lazyloader.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-02-06 08:10:22.000000 deepdriver-0.9.5/deepdriver/sdk/login.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/run.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/setting.py
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/util.py
+-rw-r--r--   0 root         (0) root         (0)     6637 2023-02-03 07:06:55.000000 deepdriver-0.9.5/deepdriver/sdk/visualization.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-02-03 07:07:24.000000 deepdriver-0.9.5/deepdriver/sdk/watch.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-02-15 06:24:33.000000 deepdriver-0.9.5/deepdriver/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 06:24:48.246580 deepdriver-0.9.5/deepdriver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      897 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-02-15 06:24:48.000000 deepdriver-0.9.5/deepdriver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2023-02-03 07:06:55.000000 deepdriver-0.9.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 06:24:48.246580 deepdriver-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-02-07 05:10:59.000000 deepdriver-0.9.5/setup.py
```

### Comparing `deepdriver-0.9.4/LICENSE.txt` & `deepdriver-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/PKG-INFO` & `deepdriver-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdriver
-Version: 0.9.4
+Version: 0.9.5
 Summary: deepdriver experiments
 Home-page: https://bokchi.com
 Author: bokchi
 Author-email: molamola.bokchi@gmail.com
 Project-URL: bokchi git hub, https://github.com/molabokchi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdriver-0.9.4/deepdriver/__init__.py` & `deepdriver-0.9.5/deepdriver/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/cli/cli.py` & `deepdriver-0.9.5/deepdriver/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import os
-
+import json
 from click import UsageError
 
 import deepdriver
 import click
 import re
 import configparser
 import pipes
@@ -116,54 +116,102 @@
     #         show_default=False,
     #     )
 
     cli_func.api_setting(config)
     cli_func.api_login(config)
 
     run = deepdriver.init(exp_name=exp_name, team_name=team_name)
-
-    cli_func.run_dump(path_dir=config.config_base_dir, run=run)
+    cli_func.save_run_dump(path_dir=config.config_base_dir, run=run)
 
 
 @click.command('artifact', short_help='Upload or Download the Deepdriver Artifact')
-@click.argument('command', type=click.Choice(['upload', 'download'], case_sensitive=False))
+@click.argument('command', type=click.Choice(['upload', 'download'], case_sensitive=False), required=True)
 @click.option('--type', help='Type of artifact', prompt="Select type f Artifact",
               type=click.Choice(['model', 'dataset', 'code']), required=True)
 @click.option('--name', help='Name of artifact', prompt="Input the name of Artifact", required=True)
 @click.option('--tag', help='Tag of artifact', required=False)
 @click.argument('path', type=click.Path(exists=True, file_okay=False, resolve_path=True), required=True)
 @pass_config
 def artifact(config, command, type, name, tag, path):
     if command == 'upload':  # upload artifact
         cli_func.api_setting(config)
         cli_func.api_login(config)
 
-        run = cli_func.run_load(path_dir=config.config_base_dir)
-
+        run = cli_func.load_run_file(path_dir=config.config_base_dir)
         from deepdriver.sdk.data_types.run import set_run, Run, get_run
         set_run(run)
 
         arti = deepdriver.get_artifact(**{"type": type, "name": name, "tag": tag})
         print(f"artfact info : {arti.__dict__}")
         arti.add(path)
         deepdriver.upload_artifact(arti)
 
 
     elif command == 'download':
         cli_func.api_setting(config)
         cli_func.api_login(config)
 
-        run = cli_func.run_load(path_dir=config.config_base_dir)
-
+        run = cli_func.load_run_file(path_dir=config.config_base_dir)
         from deepdriver.sdk.data_types.run import set_run, Run, get_run
         set_run(run)
+
         arti = deepdriver.get_artifact(**{"type": type, "name": name, "tag": tag})
         arti.download(path)
 
 
+@click.command('hpo', short_help='Create or Run HPO(Hyper-parameter optimization)')
+@click.option('--exp_name', help='Experiment Name', required=False)
+@click.option('--team_name', help='Team Name', default="", required=False)
+@click.option('--tag', help='Tag of artifact', required=False)
+@click.option('--remote', help='Is Run HPO in remote', type=click.Choice(['True', 'False'], case_sensitive=False),
+              required=False)
+@click.option('--config', help='HPO Config File Path or Json String', required=False)
+@click.option('--artifact', help='Artifact Name', required=False)
+@click.option('--count', help='Count', type=click.INT, required=False)
+@click.argument('command', type=click.Choice(['create', 'run'], case_sensitive=False), required=True)
+@pass_config
+def hpo(ctx_config, exp_name, team_name, tag, remote, config, artifact, count, command):
+    if command == "create":
+        print("create")
+        cli_func.api_setting(ctx_config)
+        cli_func.api_login(ctx_config)
+
+        try:
+            config = json.loads(config)
+        except ValueError:
+            pass
+        params = {
+            "exp_name": exp_name,
+            "team_name": team_name,
+            "remote": remote,
+            "hpo_config": config,
+        }
+        deepdriver.create_hpo(**{k: v for k, v in params.items() if v is not None})
+
+
+    elif command == "run":
+        cli_func.api_setting(ctx_config)
+        cli_func.api_login(ctx_config)
+
+        try:
+            artifact = json.loads(artifact)
+        except ValueError:
+            pass
+
+        params = {
+            "exp_name": exp_name,
+            "team_name": team_name,
+            "remote": remote,
+            "artifact": artifact,
+            "count": count,
+        }
+        deepdriver.run_hpo(**{k: v for k, v in params.items() if v is not None})
+
+
 cli.add_command(setting)
 cli.add_command(login)
 cli.add_command(init)
 cli.add_command(artifact)
+cli.add_command(hpo)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `deepdriver-0.9.4/deepdriver/cli/cli_ctx.py` & `deepdriver-0.9.5/deepdriver/cli/cli_ctx.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/cli/cli_func.py` & `deepdriver-0.9.5/deepdriver/cli/cli_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,32 +33,32 @@
 def api_setting(config: Config):
     """ deepdriver setting """
     from deepdriver.sdk.interface.interface import set_http_host, set_grpc_host
     set_http_host(config.http_host)
     set_grpc_host(config.grpc_host)
 
 def api_login(config: Config):
+    """ deepdriver login """
     channel = grpc.insecure_channel(config.grpc_host)
     stub = ResourceStub(channel)
     set_stub(stub)
 
     set_jwt_key(config.token)
 
-def api_init(run):
-    pass
 
 
-def run_dump(path_dir, run:Run):
+def save_run_dump(path_dir, run:Run):
     with open(os.path.join(path_dir, "run"), 'wb') as f:  # run 객체를 dump함
         pickle.dump(run, f)
 
-def run_load(path_dir):
+def load_run_file(path_dir):
     with open(os.path.join(path_dir, "run"), 'rb') as f:
         run = pickle.load(f)
         return run
+
 def check_exp_name(exp_name):
     # raise click.BadParameter("Couldn't understand date.", param=exp_name)
     pattern = re.compile('[^a-zA-Z0-9._]+')
     if pattern.findall(exp_name):
         raise click.BadParameter("Experiment Name은 숫자(number), 영문자(alphabet), 언더바(_), 온점(.)만 가능합니다.",
                                  param=exp_name)
         return None
```

### Comparing `deepdriver-0.9.4/deepdriver/intergration/keras/keras.py` & `deepdriver-0.9.5/deepdriver/intergration/keras/keras.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/intergration/torch/torch.py` & `deepdriver-0.9.5/deepdriver/intergration/torch/torch.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/artifact.py` & `deepdriver-0.9.5/deepdriver/sdk/artifact.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/chart/chart.py` & `deepdriver-0.9.5/deepdriver/sdk/chart/chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,24 +46,35 @@
             "log_type": self.log_type,
             "chart_type": self.chart_type,
             "data_fields": self.data_fields,
             "label_fields": self.label_fields,
             "path": self.get_path(key_name),
         }
 
-    def to_json(self, key_name: str) -> str:
+    def to_json(self, key_name: str, only_meta:bool=False) -> str:
         assert_that(key_name).is_not_none()
-        return json.dumps({
-            "data": self.data.to_dict(),
-            "log_type": self.log_type,
-            "chart_type": self.chart_type,
-            "data_fields": self.data_fields,
-            "label_fields": self.label_fields,
-            "path": self.get_path(key_name),
-        })
+        if only_meta:
+            return json.dumps({
+                "log_type": self.log_type,
+                "chart_type": self.chart_type,
+                "data_fields": self.data_fields,
+                "label_fields": self.label_fields,
+                "path": self.get_path(key_name),
+            })
+        else:
+            return json.dumps({
+                "data": self.data.to_dict(),
+                "log_type": self.log_type,
+                "chart_type": self.chart_type,
+                "data_fields": self.data_fields,
+                "label_fields": self.label_fields,
+                "path": self.get_path(key_name),
+            })
+
+
 
     def upload_file(self, run: Run, key_name: str) -> None:
         local_path = self.get_local_path(run.run_id, key_name)
         digest, size = self.file_dump(local_path, key_name)
 
         # 서버로 파일 전송
         root_path = self.get_root_path(run.run_id)
```

### Comparing `deepdriver-0.9.4/deepdriver/sdk/chart/confusion_matrix.py` & `deepdriver-0.9.5/deepdriver/sdk/chart/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/chart/histogram.py` & `deepdriver-0.9.5/deepdriver/sdk/chart/histogram.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/chart/roc_curve.py` & `deepdriver-0.9.5/deepdriver/sdk/chart/roc_curve.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/config.py` & `deepdriver-0.9.5/deepdriver/sdk/config.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/boundingBoxes.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/boundingBoxes.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/dataFrame.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/dataFrame.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/experiment.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/experiment.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/image.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/image.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/media.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/media.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/run.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
         from deepdriver.sdk.data_types.image import Image
         from deepdriver.sdk.data_types.table import Table
         from deepdriver.sdk.chart.chart import Chart
 
         for key, value in data.items():
             # TODO: Image, Chart등 다른 데이터 형식도 추가해야함
             if isinstance(value, Table):
-                data[key] = value.to_json(key)
+                data[key] = value.to_json(key, only_meta=True)
                 logger.debug(f"Table을 str(json)로 변환 변환 : {data[key]}")
                 value.upload_file(self, key)
             elif isinstance(value, Image):
                 data[key] = value.to_json(key)
                 logger.debug(f"Image를 str(json)로 변환 변환 : {data[key]}")
                 value.upload_file(self, key)
             elif isinstance(value, Chart):
-                data[key] = value.to_json(key)
+                data[key] = value.to_json(key, only_meta=True)
                 logger.debug(f"Chart를 str(json)로 변환 변환 : {data[key]}")
                 value.upload_file(self, key)
             elif isinstance(value, list):
                 if all(isinstance(n, Image) for n in value):    #Image 객체 배열일 경우
                         list_dict = []
                         for index, n in enumerate(value):
                             list_dict.append(n.to_dict(key_name=key, is_list=True, index=index))
```

### Comparing `deepdriver-0.9.4/deepdriver/sdk/data_types/table.py` & `deepdriver-0.9.5/deepdriver/sdk/data_types/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,32 @@
             "data": self.data.to_dict(),
             "log_type": self.log_type,
             "path": self.get_path(key_name),
             "cols": len(self.data.dataframe.columns),
             "rows": len(self.data.dataframe),
         }
 
-    def to_json(self, key_name: str) -> str:
+    def to_json(self, key_name: str, only_meta:bool=False) -> str:
         assert_that(key_name).is_not_none()
 
-        return json.dumps({
-            "data": self.data.to_dict(),
-            "log_type": self.log_type,
-            "path": self.get_path(key_name),
-            "cols": len(self.data.dataframe.columns),
-            "rows": len(self.data.dataframe),
-        })
+        if only_meta:
+            return json.dumps({
+                "log_type": self.log_type,
+                "path": self.get_path(key_name),
+                "cols": len(self.data.dataframe.columns),
+                "rows": len(self.data.dataframe),
+            })
+        else:
+            return json.dumps({
+                "data": self.data.to_dict(),
+                "log_type": self.log_type,
+                "path": self.get_path(key_name),
+                "cols": len(self.data.dataframe.columns),
+                "rows": len(self.data.dataframe),
+            })
 
     # 실제 파일 서버로 전송
     # Run.log에 Image 객체가 기록된 경우 Image 의 값을 올리기 위한 함수
     # table내용을 json으로 변환하여 파일로 저장후 전송
     def upload_file(self, run: Run, key_name: str) -> None:
         # Table의 data인 deepdriver.dataframe으로부터 column과 data를 가져와서 json형태의 파일로 저장
         local_path = self.get_local_path(run.run_id, key_name)
```

### Comparing `deepdriver-0.9.4/deepdriver/sdk/experiment.py` & `deepdriver-0.9.5/deepdriver/sdk/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import json
 import os
 import re
-from typing import Dict, Callable, Tuple
+from typing import Dict, Callable, Tuple, Union
 from urllib.parse import urljoin
 
 import optuna
 import ast
 from assertpy import assert_that
 
 from optuna.exceptions import DuplicatedStudyError
@@ -52,15 +53,21 @@
         for key, value in config.items():
             setattr(deepdriver.config, key, value)
 
     return run
 
 
 @util.login_required
-def create_hpo(exp_name: str = "", team_name: str = "", remote: bool = False, hpo_config: Dict = None) -> (bool, int):
+def create_hpo(exp_name: str = "", team_name: str = "", remote: bool = False, hpo_config: Union[str, Dict] = None) -> (bool, int):
+
+    if isinstance(hpo_config, str):
+        # str 인 경우 파일을 읽어서 hpo_config json(dict)를 생성
+        with open(hpo_config, "rb") as f:
+            hpo_config = json.loads(f.read())
+
     # hpo_config['parameters']를 REST API스펙에 맞게 key-value 형식으로 변환
     if hpo_config and 'parameters' in hpo_config:
         parameters_dict = hpo_config['parameters']
         key_value_parameters_list = []
         for key, value in parameters_dict.items():
             key_value_dict = {
                 "key": key,
@@ -129,23 +136,29 @@
         except Exception:
             logger.info("please check url ")
 
     return rsp['result'], rsp['expId']
 
 
 @util.login_required
-def run_hpo(exp_name: str = "", team_name: str = "", remote: bool = False, hpo_config: Dict = None,
-            func: Callable = None, count: int = 10, artifact: Dict = None, job_count: int = 0) -> bool:
+def run_hpo(exp_name: str = "", team_name: str = "", remote: bool = False, hpo_config: Dict  = None,
+            func: Callable = None, count: int = 10, artifact: Union[str, Dict] = None, job_count: int = 0) -> bool:
     # assert_that(func).is_not_none()
 
     result1, hpoConfig, team_name_from_hpo = get_hpo(exp_name=exp_name, team_name=team_name)
     if not result1:
         raise Exception("HPO not found")
     result2, study = load_hpo(exp_name=exp_name, team_name=team_name_from_hpo)
 
+    if isinstance(artifact, str):
+        # artifact 가 str인 경우 path로 보고 파일을 읽어서 json(dict)로 만듬
+        with open(artifact,  "rb") as f:
+            artifact = json.loads(f.read())
+
+
     if artifact:
         if not get_run():
             deepdriver.init(exp_name=artifact["code"]["exp_name"])
         if "dataset" in artifact:
             result, dataset_path = prepare_dataset(artifact["dataset"])
             if result:
                 hpoConfig['dataset_path'] = dataset_path
```

### Comparing `deepdriver-0.9.4/deepdriver/sdk/interface/grpc_interface_pb2.py` & `deepdriver-0.9.5/deepdriver/sdk/interface/grpc_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py` & `deepdriver-0.9.5/deepdriver/sdk/interface/grpc_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/interface/http_interface.py` & `deepdriver-0.9.5/deepdriver/sdk/interface/http_interface.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/interface/interface.py` & `deepdriver-0.9.5/deepdriver/sdk/interface/interface.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/lib/lazyloader.py` & `deepdriver-0.9.5/deepdriver/sdk/lib/lazyloader.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/login.py` & `deepdriver-0.9.5/deepdriver/sdk/login.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/run.py` & `deepdriver-0.9.5/deepdriver/sdk/run.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/util.py` & `deepdriver-0.9.5/deepdriver/sdk/util.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/visualization.py` & `deepdriver-0.9.5/deepdriver/sdk/visualization.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver/sdk/watch.py` & `deepdriver-0.9.5/deepdriver/sdk/watch.py`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/deepdriver.egg-info/PKG-INFO` & `deepdriver-0.9.5/deepdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepdriver
-Version: 0.9.4
+Version: 0.9.5
 Summary: deepdriver experiments
 Home-page: https://bokchi.com
 Author: bokchi
 Author-email: molamola.bokchi@gmail.com
 Project-URL: bokchi git hub, https://github.com/molabokchi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `deepdriver-0.9.4/deepdriver.egg-info/SOURCES.txt` & `deepdriver-0.9.5/deepdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepdriver-0.9.4/setup.py` & `deepdriver-0.9.5/setup.py`

 * *Files identical despite different names*

