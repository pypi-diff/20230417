# Comparing `tmp/pbsrollout-0.2.8.tar.gz` & `tmp/pbsrollout-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.2.8.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.0.tar", max compression
```

## Comparing `pbsrollout-0.2.8.tar` & `pbsrollout-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.2.8/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.2.8/pbsrollout/__init__.py
--rw-r--r--   0        0        0     2811 2022-12-01 22:25:39.246801 pbsrollout-0.2.8/pbsrollout/check_cluster_ready.py
--rw-r--r--   0        0        0     3450 2022-11-29 19:21:36.847264 pbsrollout-0.2.8/pbsrollout/k8s_utils.py
--rw-r--r--   0        0        0    10984 2022-12-01 22:25:32.815911 pbsrollout-0.2.8/pbsrollout/main.py
--rw-r--r--   0        0        0     9163 2022-12-05 23:00:42.482416 pbsrollout-0.2.8/pbsrollout/process_cluster.py
--rw-r--r--   0        0        0     1208 2022-11-29 18:54:57.731960 pbsrollout-0.2.8/pbsrollout/test_k8s_utils.py
--rw-r--r--   0        0        0      593 2022-11-29 21:02:30.148894 pbsrollout-0.2.8/pbsrollout/test_process_cluster.py
--rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.2.8/pbsrollout/utils.py
--rw-r--r--   0        0        0      446 2022-12-05 23:06:15.157921 pbsrollout-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 pbsrollout-0.2.8/setup.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 pbsrollout-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.0/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.0/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.0/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.0/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.0/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.0/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.0/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.0/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.0/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.0/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     4645 2023-04-13 22:01:13.155828 pbsrollout-0.3.0/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.0/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.0/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.0/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     5907 2023-04-13 22:27:23.574087 pbsrollout-0.3.0/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      522 2023-04-17 21:46:12.481295 pbsrollout-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.0/PKG-INFO
```

### Comparing `pbsrollout-0.2.8/pbsrollout/check_cluster_ready.py` & `pbsrollout-0.3.0/pbsrollout/internal/check_cluster_ready.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import subprocess
 
 from kubernetes import client, config
 from kubernetes.client import ApiClient
 from rich.console import Console
 from shellpython.helpers import Dir
 
-from pbsrollout.k8s_utils import import_kube_config
-from pbsrollout.utils import clean_stderr, Error, print_error_body
+from pbsrollout.internal.k8s_utils import import_kube_config
+from pbsrollout.internal.utils import clean_stderr, Error, print_error_body
 
 
 def check_cluster_ready(name: str, path: str, api_client: ApiClient) -> bool:
     console = Console()
     print(f'\tChecking cluster {name}')
     daemonset_check = dict()
     daemonset_check['pbs'] = check_only_one_daemonset(path, 'pbs-prod')
```

### Comparing `pbsrollout-0.2.8/pbsrollout/k8s_utils.py` & `pbsrollout-0.3.0/pbsrollout/internal/k8s_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,21 @@
         - name: AWS_PROFILE
           value: "ctv_engineer"
 """
 
 
 # Add aws env vars to the kubeconfig file. save it in a temp place and return the new path
 def import_kube_config(path: str) -> str:
+    """
+    Before importing kube config file, we need to modify it
+    We need to add the AWS_PROFILE value to it. (see `data_to_append`)
+    In order to do that, let's copy the file to a temp location, modify it and return this temp file path
+    :param path:
+    :return:
+    """
     with open(path) as fp:
         lines = fp.readlines()[:-1]
         for d in data_to_append.split('\n'):
             lines.append(d + '\n')
         with tempfile.NamedTemporaryFile(delete=False, mode='w') as tmp:
             tmp.writelines(lines)
             tmp.close()
```

### Comparing `pbsrollout-0.2.8/pbsrollout/process_cluster.py` & `pbsrollout-0.3.0/pbsrollout/internal/process_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from kubernetes.client import ApiClient
 from rich.console import Console
 from rich.padding import Padding
 from rich.table import Table
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
-from pbsrollout.k8s_utils import get_all_pbs_daemonset, get_all_pblog_daemonset, get_services, \
+from pbsrollout.internal.k8s_utils import get_all_pbs_daemonset, get_all_pblog_daemonset, get_services, \
     get_all_prebid_daemonset_V2, delete_namespaced_daemonset
-from pbsrollout.utils import Error, print_error_body, clean_stderr
+from pbsrollout.internal.utils import Error, print_error_body, clean_stderr
 
 
 def launch_pods(name: str, path: str, api_client: ApiClient) -> bool:
     with Dir(path):
         print(f'\tLaunching new pods for cluster {name}')
         # run make clean deploy-new-pbs-prod
         cmd = "direnv exec . make clean deploy-new-pbs-prod"
```

### Comparing `pbsrollout-0.2.8/pbsrollout/test_k8s_utils.py` & `pbsrollout-0.3.0/pbsrollout/internal/test_k8s_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from unittest import TestCase
 
 from kubernetes import config
 
-from pbsrollout.k8s_utils import import_kube_config, get_pods_for_daemonsets, get_all_pbs_daemonset, get_services
+from pbsrollout.internal.k8s_utils import import_kube_config, get_pods_for_daemonsets, get_all_pbs_daemonset, get_services
 
 
 class Test(TestCase):
     def test_get_pods_for_daemonset(self):
         path = os.environ['GOPATH'] + '/src/github.com/publica-project/prebid-kube-manifests/aws.eu-west-1-eks-16-v3'
         api_client = config.new_client_from_config(config_file=import_kube_config(path + '/.k8s-assets/kubeconfig'))
```

### Comparing `pbsrollout-0.2.8/pbsrollout/utils.py` & `pbsrollout-0.3.0/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.2.8/PKG-INFO` & `pbsrollout-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.2.8
+Version: 0.3.0
 Summary: 
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.26.107,<2.0.0)
+Requires-Dist: boto3-stubs[ecr] (>=1.26.107,<2.0.0)
 Requires-Dist: kubernetes (>=24.2.0,<25.0.0)
 Requires-Dist: pync (>=2.0.3,<3.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: shellpy (>=0.5.1,<0.6.0)
 Requires-Dist: simple-term-menu (>=1.5.0,<2.0.0)
```

