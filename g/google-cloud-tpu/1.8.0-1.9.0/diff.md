# Comparing `tmp/google-cloud-tpu-1.8.0.tar.gz` & `tmp/google-cloud-tpu-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-tpu-1.8.0.tar", last modified: Fri Feb 24 00:47:17 2023, max compression
+gzip compressed data, was "google-cloud-tpu-1.9.0.tar", last modified: Mon Mar 27 16:08:45 2023, max compression
```

## Comparing `google-cloud-tpu-1.8.0.tar` & `google-cloud-tpu-1.9.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.237889 google-cloud-tpu-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4525 2023-02-24 00:47:17.237889 google-cloud-tpu-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3621 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.217890 google-cloud-tpu-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.217890 google-cloud-tpu-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.221890 google-cloud-tpu-1.8.0/google/cloud/tpu/
--rw-rw-r--   0 root         (0)     1003     2016 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.221890 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/
--rw-rw-r--   0 root         (0)     1003     1917 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3204 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.221890 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.225890 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/
--rw-rw-r--   0 root         (0)     1003      725 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/__init__.py
--rw-rw-r--   0 root         (0)     1003    66827 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/async_client.py
--rw-rw-r--   0 root         (0)     1003    78536 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/client.py
--rw-rw-r--   0 root         (0)     1003    15914 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.225890 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/
--rw-rw-r--   0 root         (0)     1003     1094 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12056 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28229 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    28740 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.225890 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/types/
--rw-rw-r--   0 root         (0)     1003     1710 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    23681 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v1/types/cloud_tpu.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.225890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/
--rw-rw-r--   0 root         (0)     1003     2583 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     5434 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.225890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/
--rw-rw-r--   0 root         (0)     1003      725 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/__init__.py
--rw-rw-r--   0 root         (0)     1003    75415 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/async_client.py
--rw-rw-r--   0 root         (0)     1003    87542 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/client.py
--rw-rw-r--   0 root         (0)     1003    15816 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13060 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30606 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31179 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    95999 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/types/
--rw-rw-r--   0 root         (0)     1003     2376 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32571 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2/types/cloud_tpu.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/
--rw-rw-r--   0 root         (0)     1003     3139 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5106 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       77 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.229890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/
--rw-rw-r--   0 root         (0)     1003      725 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/__init__.py
--rw-rw-r--   0 root         (0)     1003    98643 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/async_client.py
--rw-rw-r--   0 root         (0)     1003   112059 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/client.py
--rw-rw-r--   0 root         (0)     1003    21124 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/
--rw-rw-r--   0 root         (0)     1003     1094 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    15428 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/base.py
--rw-rw-r--   0 root         (0)     1003    36493 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37227 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/types/
--rw-rw-r--   0 root         (0)     1003     2926 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    53730 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/types/cloud_tpu.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/
--rw-r--r--   0 root         (0)     1003     4525 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2833 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-02-24 00:47:17.000000 google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-02-24 00:47:17.237889 google-cloud-tpu-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2905 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.233890 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   187818 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v1/test_tpu.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.237889 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   346991 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2/test_tpu.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-02-24 00:47:17.237889 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2alpha1/
--rw-rw-r--   0 root         (0)     1003      600 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2alpha1/__init__.py
--rw-rw-r--   0 root         (0)     1003   249453 2023-02-24 00:44:47.000000 google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2alpha1/test_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.062954 google-cloud-tpu-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4525 2023-03-27 16:08:45.062954 google-cloud-tpu-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3621 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.042952 google-cloud-tpu-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.042952 google-cloud-tpu-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.046953 google-cloud-tpu-1.9.0/google/cloud/tpu/
+-rw-rw-r--   0 root         (0)     1003     2016 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.046953 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/
+-rw-rw-r--   0 root         (0)     1003     1917 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3204 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.046953 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.046953 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/
+-rw-rw-r--   0 root         (0)     1003      725 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/__init__.py
+-rw-rw-r--   0 root         (0)     1003    66817 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/async_client.py
+-rw-rw-r--   0 root         (0)     1003    78526 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/client.py
+-rw-rw-r--   0 root         (0)     1003    15914 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.050953 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/
+-rw-rw-r--   0 root         (0)     1003     1094 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12056 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28229 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    28740 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.050953 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1710 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    23717 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v1/types/cloud_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.050953 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/
+-rw-rw-r--   0 root         (0)     1003     2631 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5434 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.050953 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.050953 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/
+-rw-rw-r--   0 root         (0)     1003      725 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/__init__.py
+-rw-rw-r--   0 root         (0)     1003    75411 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/async_client.py
+-rw-rw-r--   0 root         (0)     1003    87538 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/client.py
+-rw-rw-r--   0 root         (0)     1003    15816 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13060 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30606 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31179 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    96168 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/types/
+-rw-rw-r--   0 root         (0)     1003     2424 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34014 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2/types/cloud_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/
+-rw-rw-r--   0 root         (0)     1003     3139 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5106 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       77 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/
+-rw-rw-r--   0 root         (0)     1003      725 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/__init__.py
+-rw-rw-r--   0 root         (0)     1003    98643 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112059 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/client.py
+-rw-rw-r--   0 root         (0)     1003    21124 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/
+-rw-rw-r--   0 root         (0)     1003     1094 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15428 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    36493 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37227 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.054954 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/types/
+-rw-rw-r--   0 root         (0)     1003     2926 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53767 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/types/cloud_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/
+-rw-r--r--   0 root         (0)     1003     4525 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2833 2023-03-27 16:08:45.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-03-27 16:08:44.000000 google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-03-27 16:08:45.062954 google-cloud-tpu-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2905 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   187818 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v1/test_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   347287 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2/test_tpu.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 16:08:45.058954 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2alpha1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2alpha1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   249453 2023-03-27 16:06:07.000000 google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2alpha1/test_tpu.py
```

### Comparing `google-cloud-tpu-1.8.0/LICENSE` & `google-cloud-tpu-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/MANIFEST.in` & `google-cloud-tpu-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/PKG-INFO` & `google-cloud-tpu-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-tpu
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Tpu API client library
 Home-page: https://github.com/googleapis/python-tpu
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-tpu-1.8.0/README.rst` & `google-cloud-tpu-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu/gapic_version.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/gapic_metadata.json` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/gapic_version.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/async_client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,16 +366,15 @@
                 response = await client.get_node(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.tpu_v1.types.GetNodeRequest, dict]]):
-                The request object. Request for
-                [GetNode][google.cloud.tpu.v1.Tpu.GetNode].
+                The request object. Request for [GetNode][google.cloud.tpu.v1.Tpu.GetNode].
             name (:class:`str`):
                 Required. The resource name.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1010,15 +1009,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v1.services.tpu.pagers.ListTensorFlowVersionsAsyncPager:
                 Response for
-                [ListTensorFlowVersions][google.cloud.tpu.v1.Tpu.ListTensorFlowVersions].
+                   [ListTensorFlowVersions][google.cloud.tpu.v1.Tpu.ListTensorFlowVersions].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1223,15 +1222,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v1.services.tpu.pagers.ListAcceleratorTypesAsyncPager:
                 Response for
-                [ListAcceleratorTypes][google.cloud.tpu.v1.Tpu.ListAcceleratorTypes].
+                   [ListAcceleratorTypes][google.cloud.tpu.v1.Tpu.ListAcceleratorTypes].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,16 +639,15 @@
                 response = client.get_node(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.tpu_v1.types.GetNodeRequest, dict]):
-                The request object. Request for
-                [GetNode][google.cloud.tpu.v1.Tpu.GetNode].
+                The request object. Request for [GetNode][google.cloud.tpu.v1.Tpu.GetNode].
             name (str):
                 Required. The resource name.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1286,15 +1285,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v1.services.tpu.pagers.ListTensorFlowVersionsPager:
                 Response for
-                [ListTensorFlowVersions][google.cloud.tpu.v1.Tpu.ListTensorFlowVersions].
+                   [ListTensorFlowVersions][google.cloud.tpu.v1.Tpu.ListTensorFlowVersions].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1501,15 +1500,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v1.services.tpu.pagers.ListAcceleratorTypesPager:
                 Response for
-                [ListAcceleratorTypes][google.cloud.tpu.v1.Tpu.ListAcceleratorTypes].
+                   [ListAcceleratorTypes][google.cloud.tpu.v1.Tpu.ListAcceleratorTypes].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/pagers.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/base.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/grpc.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/services/tpu/transports/grpc_asyncio.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/services/tpu/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/types/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v1/types/cloud_tpu.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v1/types/cloud_tpu.py`

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
     package="google.cloud.tpu.v1",
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from google.cloud.tpu_v2 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.tpu import TpuAsyncClient, TpuClient
 from .types.cloud_tpu import (
+    AcceleratorConfig,
     AcceleratorType,
     AccessConfig,
     AttachedDisk,
     CreateNodeRequest,
     DeleteNodeRequest,
     GenerateServiceIdentityRequest,
     GenerateServiceIdentityResponse,
@@ -54,14 +55,15 @@
     StopNodeRequest,
     Symptom,
     UpdateNodeRequest,
 )
 
 __all__ = (
     "TpuAsyncClient",
+    "AcceleratorConfig",
     "AcceleratorType",
     "AccessConfig",
     "AttachedDisk",
     "CreateNodeRequest",
     "DeleteNodeRequest",
     "GenerateServiceIdentityRequest",
     "GenerateServiceIdentityResponse",
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/gapic_metadata.json` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/gapic_version.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/async_client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,16 +366,15 @@
                 response = await client.get_node(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.tpu_v2.types.GetNodeRequest, dict]]):
-                The request object. Request for
-                [GetNode][google.cloud.tpu.v2.Tpu.GetNode].
+                The request object. Request for [GetNode][google.cloud.tpu.v2.Tpu.GetNode].
             name (:class:`str`):
                 Required. The resource name.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1054,15 +1053,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.types.GenerateServiceIdentityResponse:
                 Response for
-                [GenerateServiceIdentity][google.cloud.tpu.v2.Tpu.GenerateServiceIdentity].
+                   [GenerateServiceIdentity][google.cloud.tpu.v2.Tpu.GenerateServiceIdentity].
 
         """
         # Create or coerce a protobuf request object.
         request = cloud_tpu.GenerateServiceIdentityRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -1141,15 +1140,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.services.tpu.pagers.ListAcceleratorTypesAsyncPager:
                 Response for
-                [ListAcceleratorTypes][google.cloud.tpu.v2.Tpu.ListAcceleratorTypes].
+                   [ListAcceleratorTypes][google.cloud.tpu.v2.Tpu.ListAcceleratorTypes].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1354,15 +1353,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.services.tpu.pagers.ListRuntimeVersionsAsyncPager:
                 Response for
-                [ListRuntimeVersions][google.cloud.tpu.v2.Tpu.ListRuntimeVersions].
+                   [ListRuntimeVersions][google.cloud.tpu.v2.Tpu.ListRuntimeVersions].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1560,15 +1559,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.types.GetGuestAttributesResponse:
                 Response for
-                [GetGuestAttributes][google.cloud.tpu.v2.Tpu.GetGuestAttributes].
+                   [GetGuestAttributes][google.cloud.tpu.v2.Tpu.GetGuestAttributes].
 
         """
         # Create or coerce a protobuf request object.
         request = cloud_tpu.GetGuestAttributesRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,16 +643,15 @@
                 response = client.get_node(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.tpu_v2.types.GetNodeRequest, dict]):
-                The request object. Request for
-                [GetNode][google.cloud.tpu.v2.Tpu.GetNode].
+                The request object. Request for [GetNode][google.cloud.tpu.v2.Tpu.GetNode].
             name (str):
                 Required. The resource name.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1333,15 +1332,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.types.GenerateServiceIdentityResponse:
                 Response for
-                [GenerateServiceIdentity][google.cloud.tpu.v2.Tpu.GenerateServiceIdentity].
+                   [GenerateServiceIdentity][google.cloud.tpu.v2.Tpu.GenerateServiceIdentity].
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a cloud_tpu.GenerateServiceIdentityRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
@@ -1423,15 +1422,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.services.tpu.pagers.ListAcceleratorTypesPager:
                 Response for
-                [ListAcceleratorTypes][google.cloud.tpu.v2.Tpu.ListAcceleratorTypes].
+                   [ListAcceleratorTypes][google.cloud.tpu.v2.Tpu.ListAcceleratorTypes].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1636,15 +1635,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.services.tpu.pagers.ListRuntimeVersionsPager:
                 Response for
-                [ListRuntimeVersions][google.cloud.tpu.v2.Tpu.ListRuntimeVersions].
+                   [ListRuntimeVersions][google.cloud.tpu.v2.Tpu.ListRuntimeVersions].
 
                 Iterating over this object will yield results and
                 resolve additional pages automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1842,15 +1841,15 @@
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.tpu_v2.types.GetGuestAttributesResponse:
                 Response for
-                [GetGuestAttributes][google.cloud.tpu.v2.Tpu.GetGuestAttributes].
+                   [GetGuestAttributes][google.cloud.tpu.v2.Tpu.GetGuestAttributes].
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a cloud_tpu.GetGuestAttributesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/pagers.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/base.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/grpc.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/grpc_asyncio.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/services/tpu/transports/rest.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/services/tpu/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import dataclasses
 import json  # type: ignore
 import re
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 import warnings
 
 from google.api_core import (
     gapic_v1,
     operations_v1,
     path_template,
     rest_helpers,
@@ -466,139 +466,135 @@
         """
         return response
 
     def pre_get_location(
         self,
         request: locations_pb2.GetLocationRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> locations_pb2.Location:
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_location
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
     def post_get_location(
-        self, response: locations_pb2.GetLocationRequest
+        self, response: locations_pb2.Location
     ) -> locations_pb2.Location:
         """Post-rpc interceptor for get_location
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
         return response
 
     def pre_list_locations(
         self,
         request: locations_pb2.ListLocationsRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> locations_pb2.ListLocationsResponse:
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for list_locations
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
     def post_list_locations(
-        self, response: locations_pb2.ListLocationsRequest
+        self, response: locations_pb2.ListLocationsResponse
     ) -> locations_pb2.ListLocationsResponse:
         """Post-rpc interceptor for list_locations
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
         return response
 
     def pre_cancel_operation(
         self,
         request: operations_pb2.CancelOperationRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> None:
+    ) -> Tuple[operations_pb2.CancelOperationRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for cancel_operation
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
-    def post_cancel_operation(
-        self, response: operations_pb2.CancelOperationRequest
-    ) -> None:
+    def post_cancel_operation(self, response: None) -> None:
         """Post-rpc interceptor for cancel_operation
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
         return response
 
     def pre_delete_operation(
         self,
         request: operations_pb2.DeleteOperationRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> None:
+    ) -> Tuple[operations_pb2.DeleteOperationRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for delete_operation
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
-    def post_delete_operation(
-        self, response: operations_pb2.DeleteOperationRequest
-    ) -> None:
+    def post_delete_operation(self, response: None) -> None:
         """Post-rpc interceptor for delete_operation
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
         return response
 
     def pre_get_operation(
         self,
         request: operations_pb2.GetOperationRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> operations_pb2.Operation:
+    ) -> Tuple[operations_pb2.GetOperationRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_operation
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
     def post_get_operation(
-        self, response: operations_pb2.GetOperationRequest
+        self, response: operations_pb2.Operation
     ) -> operations_pb2.Operation:
         """Post-rpc interceptor for get_operation
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
         return response
 
     def pre_list_operations(
         self,
         request: operations_pb2.ListOperationsRequest,
         metadata: Sequence[Tuple[str, str]],
-    ) -> operations_pb2.ListOperationsResponse:
+    ) -> Tuple[operations_pb2.ListOperationsRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for list_operations
 
         Override in a subclass to manipulate the request or metadata
         before they are sent to the Tpu server.
         """
         return request, metadata
 
     def post_list_operations(
-        self, response: operations_pb2.ListOperationsRequest
+        self, response: operations_pb2.ListOperationsResponse
     ) -> operations_pb2.ListOperationsResponse:
         """Post-rpc interceptor for list_operations
 
         Override in a subclass to manipulate the response
         after it is returned by the Tpu server but before
         it is returned to user code.
         """
@@ -755,15 +751,15 @@
         # Return the client from cache.
         return self._operations_client
 
     class _CreateNode(TpuRestStub):
         def __hash__(self):
             return hash("CreateNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -779,15 +775,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the create node method over HTTP.
 
             Args:
                 request (~.cloud_tpu.CreateNodeRequest):
                     The request object. Request for
                 [CreateNode][google.cloud.tpu.v2.Tpu.CreateNode].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -853,15 +848,15 @@
             resp = self._interceptor.post_create_node(resp)
             return resp
 
     class _DeleteNode(TpuRestStub):
         def __hash__(self):
             return hash("DeleteNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -877,15 +872,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the delete node method over HTTP.
 
             Args:
                 request (~.cloud_tpu.DeleteNodeRequest):
                     The request object. Request for
                 [DeleteNode][google.cloud.tpu.v2.Tpu.DeleteNode].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -942,15 +936,15 @@
             resp = self._interceptor.post_delete_node(resp)
             return resp
 
     class _GenerateServiceIdentity(TpuRestStub):
         def __hash__(self):
             return hash("GenerateServiceIdentity")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -966,15 +960,14 @@
         ) -> cloud_tpu.GenerateServiceIdentityResponse:
             r"""Call the generate service identity method over HTTP.
 
             Args:
                 request (~.cloud_tpu.GenerateServiceIdentityRequest):
                     The request object. Request for
                 [GenerateServiceIdentity][google.cloud.tpu.v2.Tpu.GenerateServiceIdentity].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1043,15 +1036,15 @@
             resp = self._interceptor.post_generate_service_identity(resp)
             return resp
 
     class _GetAcceleratorType(TpuRestStub):
         def __hash__(self):
             return hash("GetAcceleratorType")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1067,15 +1060,14 @@
         ) -> cloud_tpu.AcceleratorType:
             r"""Call the get accelerator type method over HTTP.
 
             Args:
                 request (~.cloud_tpu.GetAcceleratorTypeRequest):
                     The request object. Request for
                 [GetAcceleratorType][google.cloud.tpu.v2.Tpu.GetAcceleratorType].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1135,15 +1127,15 @@
             resp = self._interceptor.post_get_accelerator_type(resp)
             return resp
 
     class _GetGuestAttributes(TpuRestStub):
         def __hash__(self):
             return hash("GetGuestAttributes")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1159,15 +1151,14 @@
         ) -> cloud_tpu.GetGuestAttributesResponse:
             r"""Call the get guest attributes method over HTTP.
 
             Args:
                 request (~.cloud_tpu.GetGuestAttributesRequest):
                     The request object. Request for
                 [GetGuestAttributes][google.cloud.tpu.v2.Tpu.GetGuestAttributes].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1236,15 +1227,15 @@
             resp = self._interceptor.post_get_guest_attributes(resp)
             return resp
 
     class _GetNode(TpuRestStub):
         def __hash__(self):
             return hash("GetNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1322,15 +1313,15 @@
             resp = self._interceptor.post_get_node(resp)
             return resp
 
     class _GetRuntimeVersion(TpuRestStub):
         def __hash__(self):
             return hash("GetRuntimeVersion")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1346,15 +1337,14 @@
         ) -> cloud_tpu.RuntimeVersion:
             r"""Call the get runtime version method over HTTP.
 
             Args:
                 request (~.cloud_tpu.GetRuntimeVersionRequest):
                     The request object. Request for
                 [GetRuntimeVersion][google.cloud.tpu.v2.Tpu.GetRuntimeVersion].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1414,15 +1404,15 @@
             resp = self._interceptor.post_get_runtime_version(resp)
             return resp
 
     class _ListAcceleratorTypes(TpuRestStub):
         def __hash__(self):
             return hash("ListAcceleratorTypes")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1438,15 +1428,14 @@
         ) -> cloud_tpu.ListAcceleratorTypesResponse:
             r"""Call the list accelerator types method over HTTP.
 
             Args:
                 request (~.cloud_tpu.ListAcceleratorTypesRequest):
                     The request object. Request for
                 [ListAcceleratorTypes][google.cloud.tpu.v2.Tpu.ListAcceleratorTypes].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1506,15 +1495,15 @@
             resp = self._interceptor.post_list_accelerator_types(resp)
             return resp
 
     class _ListNodes(TpuRestStub):
         def __hash__(self):
             return hash("ListNodes")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1530,15 +1519,14 @@
         ) -> cloud_tpu.ListNodesResponse:
             r"""Call the list nodes method over HTTP.
 
             Args:
                 request (~.cloud_tpu.ListNodesRequest):
                     The request object. Request for
                 [ListNodes][google.cloud.tpu.v2.Tpu.ListNodes].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1596,15 +1584,15 @@
             resp = self._interceptor.post_list_nodes(resp)
             return resp
 
     class _ListRuntimeVersions(TpuRestStub):
         def __hash__(self):
             return hash("ListRuntimeVersions")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1620,15 +1608,14 @@
         ) -> cloud_tpu.ListRuntimeVersionsResponse:
             r"""Call the list runtime versions method over HTTP.
 
             Args:
                 request (~.cloud_tpu.ListRuntimeVersionsRequest):
                     The request object. Request for
                 [ListRuntimeVersions][google.cloud.tpu.v2.Tpu.ListRuntimeVersions].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1688,15 +1675,15 @@
             resp = self._interceptor.post_list_runtime_versions(resp)
             return resp
 
     class _StartNode(TpuRestStub):
         def __hash__(self):
             return hash("StartNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1712,15 +1699,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the start node method over HTTP.
 
             Args:
                 request (~.cloud_tpu.StartNodeRequest):
                     The request object. Request for
                 [StartNode][google.cloud.tpu.v2.Tpu.StartNode].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1786,15 +1772,15 @@
             resp = self._interceptor.post_start_node(resp)
             return resp
 
     class _StopNode(TpuRestStub):
         def __hash__(self):
             return hash("StopNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {}
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
                 for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
                 if k not in message_dict
@@ -1810,15 +1796,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the stop node method over HTTP.
 
             Args:
                 request (~.cloud_tpu.StopNodeRequest):
                     The request object. Request for
                 [StopNode][google.cloud.tpu.v2.Tpu.StopNode].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1884,15 +1869,15 @@
             resp = self._interceptor.post_stop_node(resp)
             return resp
 
     class _UpdateNode(TpuRestStub):
         def __hash__(self):
             return hash("UpdateNode")
 
-        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, str] = {
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "updateMask": {},
         }
 
         @classmethod
         def _get_unset_required_fields(cls, message_dict):
             return {
                 k: v
@@ -1910,15 +1895,14 @@
         ) -> operations_pb2.Operation:
             r"""Call the update node method over HTTP.
 
             Args:
                 request (~.cloud_tpu.UpdateNodeRequest):
                     The request object. Request for
                 [UpdateNode][google.cloud.tpu.v2.Tpu.UpdateNode].
-
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/types/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .cloud_tpu import (
+    AcceleratorConfig,
     AcceleratorType,
     AccessConfig,
     AttachedDisk,
     CreateNodeRequest,
     DeleteNodeRequest,
     GenerateServiceIdentityRequest,
     GenerateServiceIdentityResponse,
@@ -47,14 +48,15 @@
     StartNodeRequest,
     StopNodeRequest,
     Symptom,
     UpdateNodeRequest,
 )
 
 __all__ = (
+    "AcceleratorConfig",
     "AcceleratorType",
     "AccessConfig",
     "AttachedDisk",
     "CreateNodeRequest",
     "DeleteNodeRequest",
     "GenerateServiceIdentityRequest",
     "GenerateServiceIdentityResponse",
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2/types/cloud_tpu.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2/types/cloud_tpu.py`

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
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
@@ -51,14 +53,15 @@
         "GetRuntimeVersionRequest",
         "ListRuntimeVersionsRequest",
         "ListRuntimeVersionsResponse",
         "OperationMetadata",
         "Symptom",
         "GetGuestAttributesRequest",
         "GetGuestAttributesResponse",
+        "AcceleratorConfig",
         "ShieldedInstanceConfig",
     },
 )
 
 
 class GuestAttributes(proto.Message):
     r"""A guest attributes.
@@ -373,14 +376,16 @@
             Output only. The API version that created
             this Node.
         symptoms (MutableSequence[google.cloud.tpu_v2.types.Symptom]):
             Output only. The Symptoms that have occurred
             to the TPU Node.
         shielded_instance_config (google.cloud.tpu_v2.types.ShieldedInstanceConfig):
             Shielded Instance options.
+        accelerator_config (google.cloud.tpu_v2.types.AcceleratorConfig):
+            The AccleratorConfig for the TPU Node.
     """
 
     class State(proto.Enum):
         r"""Represents the different states of a TPU node during its
         lifecycle.
 
         Values:
@@ -574,14 +579,19 @@
         message="Symptom",
     )
     shielded_instance_config: "ShieldedInstanceConfig" = proto.Field(
         proto.MESSAGE,
         number=45,
         message="ShieldedInstanceConfig",
     )
+    accelerator_config: "AcceleratorConfig" = proto.Field(
+        proto.MESSAGE,
+        number=46,
+        message="AcceleratorConfig",
+    )
 
 
 class ListNodesRequest(proto.Message):
     r"""Request for [ListNodes][google.cloud.tpu.v2.Tpu.ListNodes].
 
     Attributes:
         parent (str):
@@ -797,24 +807,31 @@
     r"""A accelerator type that a Node can be configured with.
 
     Attributes:
         name (str):
             The resource name.
         type_ (str):
             the accelerator type.
+        accelerator_configs (MutableSequence[google.cloud.tpu_v2.types.AcceleratorConfig]):
+            The accelerator config.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     type_: str = proto.Field(
         proto.STRING,
         number=2,
     )
+    accelerator_configs: MutableSequence["AcceleratorConfig"] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=3,
+        message="AcceleratorConfig",
+    )
 
 
 class GetAcceleratorTypeRequest(proto.Message):
     r"""Request for
     [GetAcceleratorType][google.cloud.tpu.v2.Tpu.GetAcceleratorType].
 
     Attributes:
@@ -1167,14 +1184,53 @@
     guest_attributes: MutableSequence["GuestAttributes"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="GuestAttributes",
     )
 
 
+class AcceleratorConfig(proto.Message):
+    r"""A TPU accelerator configuration.
+
+    Attributes:
+        type_ (google.cloud.tpu_v2.types.AcceleratorConfig.Type):
+            Required. Type of TPU.
+        topology (str):
+            Required. Topology of TPU in chips.
+    """
+
+    class Type(proto.Enum):
+        r"""TPU type.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                Unspecified version.
+            V2 (2):
+                TPU v2.
+            V3 (4):
+                TPU v3.
+            V4 (7):
+                TPU v4.
+        """
+        TYPE_UNSPECIFIED = 0
+        V2 = 2
+        V3 = 4
+        V4 = 7
+
+    type_: Type = proto.Field(
+        proto.ENUM,
+        number=1,
+        enum=Type,
+    )
+    topology: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
 class ShieldedInstanceConfig(proto.Message):
     r"""A set of Shielded Instance options.
 
     Attributes:
         enable_secure_boot (bool):
             Defines whether the instance has Secure Boot
             enabled.
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/gapic_metadata.json` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/gapic_version.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.0"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/async_client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/client.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/pagers.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/base.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc_asyncio.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/services/tpu/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/types/__init__.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/google/cloud/tpu_v2alpha1/types/cloud_tpu.py` & `google-cloud-tpu-1.9.0/google/cloud/tpu_v2alpha1/types/cloud_tpu.py`

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
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 from google.type import interval_pb2  # type: ignore
@@ -631,15 +633,15 @@
             The Guaranteed tier
 
             This field is a member of `oneof`_ ``tier``.
         queueing_policy (google.cloud.tpu_v2alpha1.types.QueuedResource.QueueingPolicy):
             The queueing policy of the QueuedRequest.
         state (google.cloud.tpu_v2alpha1.types.QueuedResourceState):
             Output only. State of the QueuedResource
-            request
+            request.
     """
 
     class Tpu(proto.Message):
         r"""Details of the TPU resource(s) being requested.
 
         Attributes:
             node_spec (MutableSequence[google.cloud.tpu_v2alpha1.types.QueuedResource.Tpu.NodeSpec]):
```

### Comparing `google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/PKG-INFO` & `google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-tpu
-Version: 1.8.0
+Version: 1.9.0
 Summary: Google Cloud Tpu API client library
 Home-page: https://github.com/googleapis/python-tpu
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-tpu-1.8.0/google_cloud_tpu.egg-info/SOURCES.txt` & `google-cloud-tpu-1.9.0/google_cloud_tpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/setup.py` & `google-cloud-tpu-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/__init__.py` & `google-cloud-tpu-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/__init__.py` & `google-cloud-tpu-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/__init__.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v1/__init__.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v1/test_tpu.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v1/test_tpu.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2/__init__.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2/test_tpu.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2/test_tpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -4708,14 +4708,15 @@
                 "create_time": {},
                 "symptom_type": 1,
                 "details": "details_value",
                 "worker_id": "worker_id_value",
             }
         ],
         "shielded_instance_config": {"enable_secure_boot": True},
+        "accelerator_config": {"type_": 2, "topology": "topology_value"},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -4930,14 +4931,15 @@
                 "create_time": {},
                 "symptom_type": 1,
                 "details": "details_value",
                 "worker_id": "worker_id_value",
             }
         ],
         "shielded_instance_config": {"enable_secure_boot": True},
+        "accelerator_config": {"type_": 2, "topology": "topology_value"},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -5731,14 +5733,15 @@
                 "create_time": {},
                 "symptom_type": 1,
                 "details": "details_value",
                 "worker_id": "worker_id_value",
             }
         ],
         "shielded_instance_config": {"enable_secure_boot": True},
+        "accelerator_config": {"type_": 2, "topology": "topology_value"},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -5950,14 +5953,15 @@
                 "create_time": {},
                 "symptom_type": 1,
                 "details": "details_value",
                 "worker_id": "worker_id_value",
             }
         ],
         "shielded_instance_config": {"enable_secure_boot": True},
+        "accelerator_config": {"type_": 2, "topology": "topology_value"},
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
```

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2alpha1/__init__.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-tpu-1.8.0/tests/unit/gapic/tpu_v2alpha1/test_tpu.py` & `google-cloud-tpu-1.9.0/tests/unit/gapic/tpu_v2alpha1/test_tpu.py`

 * *Files identical despite different names*

