# Comparing `tmp/google-cloud-notebooks-1.6.1.tar.gz` & `tmp/google-cloud-notebooks-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-notebooks-1.6.1.tar", last modified: Mon Jan 23 15:51:08 2023, max compression
+gzip compressed data, was "google-cloud-notebooks-1.7.0.tar", last modified: Mon Apr 17 10:44:39 2023, max compression
```

## Comparing `google-cloud-notebooks-1.6.1.tar` & `google-cloud-notebooks-1.7.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4944 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4022 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.080044 google-cloud-notebooks-1.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.084044 google-cloud-notebooks-1.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.084044 google-cloud-notebooks-1.6.1/google/cloud/notebooks/
--rw-rw-r--   0 root         (0)     1003     6284 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.088044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/
--rw-rw-r--   0 root         (0)     1003     5770 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    12874 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.088044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.088044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/
--rw-rw-r--   0 root         (0)     1003      801 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    98226 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   108678 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003     5785 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.088044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1273 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14018 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    35729 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36386 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.088044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   178912 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   194252 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003    20735 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.092044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    23439 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    59398 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    60689 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.092044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/
--rw-rw-r--   0 root         (0)     1003     5244 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2920 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/diagnostic_config.py
--rw-rw-r--   0 root         (0)     1003     5330 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/environment.py
--rw-rw-r--   0 root         (0)     1003     2772 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/event.py
--rw-rw-r--   0 root         (0)     1003    18036 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/execution.py
--rw-rw-r--   0 root         (0)     1003    31206 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/instance.py
--rw-rw-r--   0 root         (0)     1003     1488 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/instance_config.py
--rw-rw-r--   0 root         (0)     1003    12489 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/managed_service.py
--rw-rw-r--   0 root         (0)     1003    35663 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/runtime.py
--rw-rw-r--   0 root         (0)     1003     5352 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/schedule.py
--rw-rw-r--   0 root         (0)     1003    33596 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.092044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2522 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5456 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       83 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.096044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.096044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   104669 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   116111 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/client.py
--rw-rw-r--   0 root         (0)     1003    10868 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.096044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    16641 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42380 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43205 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.096044 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2239 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5354 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/environment.py
--rw-rw-r--   0 root         (0)     1003    18101 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/instance.py
--rw-rw-r--   0 root         (0)     1003    17571 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/
--rw-r--r--   0 root         (0)     1003     4944 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3729 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 15:51:08.000000 google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-23 15:51:08.104044 google-cloud-notebooks-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3030 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   222490 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py
--rw-rw-r--   0 root         (0)     1003   380606 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/test_notebook_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 15:51:08.100044 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   224522 2023-01-23 15:47:52.000000 google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4944 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4022 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.244054 google-cloud-notebooks-1.7.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.244054 google-cloud-notebooks-1.7.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks/
+-rw-rw-r--   0 root         (0)     1003     6284 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/
+-rw-rw-r--   0 root         (0)     1003     5773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12874 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.248056 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/
+-rw-rw-r--   0 root         (0)     1003      801 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    98226 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   108678 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5785 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1273 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14018 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35729 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36386 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.252058 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   178928 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   194268 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20735 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23439 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    59398 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    60689 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5244 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2956 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/diagnostic_config.py
+-rw-rw-r--   0 root         (0)     1003     5366 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/environment.py
+-rw-rw-r--   0 root         (0)     1003     2808 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/event.py
+-rw-rw-r--   0 root         (0)     1003    18072 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/execution.py
+-rw-rw-r--   0 root         (0)     1003    31242 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance.py
+-rw-rw-r--   0 root         (0)     1003     1524 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance_config.py
+-rw-rw-r--   0 root         (0)     1003    12525 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/managed_service.py
+-rw-rw-r--   0 root         (0)     1003    35699 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/runtime.py
+-rw-rw-r--   0 root         (0)     1003     5388 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/schedule.py
+-rw-rw-r--   0 root         (0)     1003    33632 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2530 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8015 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       83 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.256060 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104669 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   116232 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10868 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1414 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16641 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    42380 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43205 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   140287 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2239 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5390 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/environment.py
+-rw-rw-r--   0 root         (0)     1003    18137 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/instance.py
+-rw-rw-r--   0 root         (0)     1003    17607 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/
+-rw-r--r--   0 root         (0)     1003     4944 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3805 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-17 10:44:39.000000 google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.260062 google-cloud-notebooks-1.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   222490 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py
+-rw-rw-r--   0 root         (0)     1003   380606 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_notebook_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:44:39.264064 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   406758 2023-04-17 10:41:29.000000 google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/test_notebook_service.py
```

### Comparing `google-cloud-notebooks-1.6.1/LICENSE` & `google-cloud-notebooks-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/MANIFEST.in` & `google-cloud-notebooks-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/PKG-INFO` & `google-cloud-notebooks-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-notebooks
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Notebooks API client library
 Home-page: https://github.com/googleapis/python-notebooks
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-notebooks-1.6.1/README.rst` & `google-cloud-notebooks-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks/gapic_version.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.notebooks import gapic_version as package_version
+from google.cloud.notebooks_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.managed_notebook_service import (
     ManagedNotebookServiceAsyncClient,
     ManagedNotebookServiceClient,
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/gapic_metadata.json` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/gapic_version.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1376,16 +1376,16 @@
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.notebooks_v1.types.UpgradeRuntimeRequest, dict]]):
-                The request object. Request for upgrading a Managed
-                Notebook Runtime to the latest version. option
+                The request object. Request for upgrading a Managed Notebook Runtime to the
+                latest version. option
                 (google.api.message_visibility).restriction =
                 "TRUSTED_TESTER,SPECIAL_TESTER";
             name (:class:`str`):
                 Required. Format:
                 ``projects/{project_id}/locations/{location}/runtimes/{runtime_id}``
 
                 This corresponds to the ``name`` field
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1600,16 +1600,16 @@
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.notebooks_v1.types.UpgradeRuntimeRequest, dict]):
-                The request object. Request for upgrading a Managed
-                Notebook Runtime to the latest version. option
+                The request object. Request for upgrading a Managed Notebook Runtime to the
+                latest version. option
                 (google.api.message_visibility).restriction =
                 "TRUSTED_TESTER,SPECIAL_TESTER";
             name (str):
                 Required. Format:
                 ``projects/{project_id}/locations/{location}/runtimes/{runtime_id}``
 
                 This corresponds to the ``name`` field
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/managed_notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/async_client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1031,16 +1031,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.notebooks_v1.types.UpdateShieldedInstanceConfigRequest, dict]]):
                 The request object. Request for updating the Shielded
-                Instance config for a notebook instance. You can only
-                use this method on a stopped instance
+                Instance config for a notebook instance.
+                You can only use this method on a
+                stopped instance
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1338,16 +1338,17 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.notebooks_v1.types.UpdateShieldedInstanceConfigRequest, dict]):
                 The request object. Request for updating the Shielded
-                Instance config for a notebook instance. You can only
-                use this method on a stopped instance
+                Instance config for a notebook instance.
+                You can only use this method on a
+                stopped instance
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/pagers.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/services/notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/diagnostic_config.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/diagnostic_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1",
     manifest={
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/environment.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1",
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/event.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1",
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/execution.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1",
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/instance.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1.types import environment
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/instance_config.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/instance_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1",
     manifest={
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/managed_service.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/managed_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1.types import diagnostic_config as gcn_diagnostic_config
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/runtime.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1.types import environment
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/schedule.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1.types import execution
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1/types/service.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1.types import diagnostic_config as gcn_diagnostic_config
 from google.cloud.notebooks_v1.types import environment as gcn_environment
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.notebooks import gapic_version as package_version
+from google.cloud.notebooks_v1beta1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.notebook_service import NotebookServiceAsyncClient, NotebookServiceClient
 from .types.environment import ContainerImage, Environment, VmImage
 from .types.instance import Instance, ReservationAffinity
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/gapic_metadata.json` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_metadata.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555555%*

 * *Differences: {"'services'": "{'NotebookService': {'clients': {'rest': OrderedDict([('libraryClient', "*

 * *               "'NotebookServiceClient'), ('rpcs', OrderedDict([('CreateEnvironment', "*

 * *               "OrderedDict([('methods', ['create_environment'])])), ('CreateInstance', "*

 * *               "OrderedDict([('methods', ['create_instance'])])), ('DeleteEnvironment', "*

 * *               "OrderedDict([('methods', ['delete_environment'])])), ('DeleteInstance', "*

 * *               "OrderedDict([('methods', ['delete_instance'])])) […]*

```diff
@@ -202,12 +202,112 @@
                         },
                         "UpgradeInstanceInternal": {
                             "methods": [
                                 "upgrade_instance_internal"
                             ]
                         }
                     }
+                },
+                "rest": {
+                    "libraryClient": "NotebookServiceClient",
+                    "rpcs": {
+                        "CreateEnvironment": {
+                            "methods": [
+                                "create_environment"
+                            ]
+                        },
+                        "CreateInstance": {
+                            "methods": [
+                                "create_instance"
+                            ]
+                        },
+                        "DeleteEnvironment": {
+                            "methods": [
+                                "delete_environment"
+                            ]
+                        },
+                        "DeleteInstance": {
+                            "methods": [
+                                "delete_instance"
+                            ]
+                        },
+                        "GetEnvironment": {
+                            "methods": [
+                                "get_environment"
+                            ]
+                        },
+                        "GetInstance": {
+                            "methods": [
+                                "get_instance"
+                            ]
+                        },
+                        "IsInstanceUpgradeable": {
+                            "methods": [
+                                "is_instance_upgradeable"
+                            ]
+                        },
+                        "ListEnvironments": {
+                            "methods": [
+                                "list_environments"
+                            ]
+                        },
+                        "ListInstances": {
+                            "methods": [
+                                "list_instances"
+                            ]
+                        },
+                        "RegisterInstance": {
+                            "methods": [
+                                "register_instance"
+                            ]
+                        },
+                        "ReportInstanceInfo": {
+                            "methods": [
+                                "report_instance_info"
+                            ]
+                        },
+                        "ResetInstance": {
+                            "methods": [
+                                "reset_instance"
+                            ]
+                        },
+                        "SetInstanceAccelerator": {
+                            "methods": [
+                                "set_instance_accelerator"
+                            ]
+                        },
+                        "SetInstanceLabels": {
+                            "methods": [
+                                "set_instance_labels"
+                            ]
+                        },
+                        "SetInstanceMachineType": {
+                            "methods": [
+                                "set_instance_machine_type"
+                            ]
+                        },
+                        "StartInstance": {
+                            "methods": [
+                                "start_instance"
+                            ]
+                        },
+                        "StopInstance": {
+                            "methods": [
+                                "stop_instance"
+                            ]
+                        },
+                        "UpgradeInstance": {
+                            "methods": [
+                                "upgrade_instance"
+                            ]
+                        },
+                        "UpgradeInstanceInternal": {
+                            "methods": [
+                                "upgrade_instance_internal"
+                            ]
+                        }
+                    }
                 }
             }
         }
     }
 }
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/gapic_version.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/client.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 from google.cloud.notebooks_v1beta1.services.notebook_service import pagers
 from google.cloud.notebooks_v1beta1.types import environment, instance, service
 
 from .transports.base import DEFAULT_CLIENT_INFO, NotebookServiceTransport
 from .transports.grpc import NotebookServiceGrpcTransport
 from .transports.grpc_asyncio import NotebookServiceGrpcAsyncIOTransport
+from .transports.rest import NotebookServiceRestTransport
 
 
 class NotebookServiceClientMeta(type):
     """Metaclass for the NotebookService client.
 
     This provides class-level methods for building and retrieving
     support objects (e.g. transport) without polluting the client instance
@@ -73,14 +74,15 @@
     """
 
     _transport_registry = (
         OrderedDict()
     )  # type: Dict[str, Type[NotebookServiceTransport]]
     _transport_registry["grpc"] = NotebookServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = NotebookServiceGrpcAsyncIOTransport
+    _transport_registry["rest"] = NotebookServiceRestTransport
 
     def get_transport_class(
         cls,
         label: Optional[str] = None,
     ) -> Type[NotebookServiceTransport]:
         """Returns an appropriate transport class.
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,22 @@
 #
 from collections import OrderedDict
 from typing import Dict, Type
 
 from .base import NotebookServiceTransport
 from .grpc import NotebookServiceGrpcTransport
 from .grpc_asyncio import NotebookServiceGrpcAsyncIOTransport
+from .rest import NotebookServiceRestInterceptor, NotebookServiceRestTransport
 
 # Compile a registry of transports.
 _transport_registry = OrderedDict()  # type: Dict[str, Type[NotebookServiceTransport]]
 _transport_registry["grpc"] = NotebookServiceGrpcTransport
 _transport_registry["grpc_asyncio"] = NotebookServiceGrpcAsyncIOTransport
+_transport_registry["rest"] = NotebookServiceRestTransport
 
 __all__ = (
     "NotebookServiceTransport",
     "NotebookServiceGrpcTransport",
     "NotebookServiceGrpcAsyncIOTransport",
+    "NotebookServiceRestTransport",
+    "NotebookServiceRestInterceptor",
 )
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/__init__.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/environment.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
     package="google.cloud.notebooks.v1beta1",
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/instance.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1beta1.types import environment
```

### Comparing `google-cloud-notebooks-1.6.1/google/cloud/notebooks_v1beta1/types/service.py` & `google-cloud-notebooks-1.7.0/google/cloud/notebooks_v1beta1/types/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 from google.cloud.notebooks_v1beta1.types import environment as gcn_environment
 from google.cloud.notebooks_v1beta1.types import instance as gcn_instance
```

### Comparing `google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/PKG-INFO` & `google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-notebooks
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Notebooks API client library
 Home-page: https://github.com/googleapis/python-notebooks
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-notebooks-1.6.1/google_cloud_notebooks.egg-info/SOURCES.txt` & `google-cloud-notebooks-1.7.0/google_cloud_notebooks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 google/cloud/notebooks_v1beta1/services/notebook_service/async_client.py
 google/cloud/notebooks_v1beta1/services/notebook_service/client.py
 google/cloud/notebooks_v1beta1/services/notebook_service/pagers.py
 google/cloud/notebooks_v1beta1/services/notebook_service/transports/__init__.py
 google/cloud/notebooks_v1beta1/services/notebook_service/transports/base.py
 google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc.py
 google/cloud/notebooks_v1beta1/services/notebook_service/transports/grpc_asyncio.py
+google/cloud/notebooks_v1beta1/services/notebook_service/transports/rest.py
 google/cloud/notebooks_v1beta1/types/__init__.py
 google/cloud/notebooks_v1beta1/types/environment.py
 google/cloud/notebooks_v1beta1/types/instance.py
 google/cloud/notebooks_v1beta1/types/service.py
 google_cloud_notebooks.egg-info/PKG-INFO
 google_cloud_notebooks.egg-info/SOURCES.txt
 google_cloud_notebooks.egg-info/dependency_links.txt
```

### Comparing `google-cloud-notebooks-1.6.1/setup.py` & `google-cloud-notebooks-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
-    "grpc-google-iam-v1 >= 0.12.4, < 1.0.0dev",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
 url = "https://github.com/googleapis/python-notebooks"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
@@ -52,17 +52,15 @@
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("google")
 ]
 
-namespaces = ["google"]
-if "google.cloud" in packages:
-    namespaces.append("google.cloud")
+namespaces = ["google", "google.cloud"]
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
```

### Comparing `google-cloud-notebooks-1.6.1/tests/__init__.py` & `google-cloud-notebooks-1.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/__init__.py` & `google-cloud-notebooks-1.7.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/gapic/__init__.py` & `google-cloud-notebooks-1.7.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/__init__.py` & `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py` & `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_managed_notebook_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1/test_notebook_service.py` & `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1/test_notebook_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-notebooks-1.6.1/tests/unit/gapic/notebooks_v1beta1/__init__.py` & `google-cloud-notebooks-1.7.0/tests/unit/gapic/notebooks_v1beta1/__init__.py`

 * *Files identical despite different names*

