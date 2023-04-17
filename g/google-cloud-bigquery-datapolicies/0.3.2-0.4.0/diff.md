# Comparing `tmp/google-cloud-bigquery-datapolicies-0.3.2.tar.gz` & `tmp/google-cloud-bigquery-datapolicies-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-datapolicies-0.3.2.tar", last modified: Mon Mar 27 14:58:21 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-datapolicies-0.4.0.tar", last modified: Mon Apr 17 10:42:42 2023, max compression
```

## Comparing `google-cloud-bigquery-datapolicies-0.3.2.tar` & `google-cloud-bigquery-datapolicies-0.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4849 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3904 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.215424 google-cloud-bigquery-datapolicies-0.3.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.215424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.219424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.219424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/
--rw-rw-r--   0 root         (0)     1003     1580 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.219424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003     1451 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4125 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.219424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    56334 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    63536 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     5969 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12955 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21504 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21939 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    59846 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/types/
--rw-rw-r--   0 root         (0)     1003     1141 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11389 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1396 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2620 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.223424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    51605 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58819 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     6014 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12185 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20383 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20782 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1081 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10282 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/
--rw-r--r--   0 root         (0)     1003     4849 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3168 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:21.000000 google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:58:21.231423 google-cloud-bigquery-datapolicies-0.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3055 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   224205 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:21.227424 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   123065 2023-03-27 14:55:52.000000 google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4849 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3904 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.801092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/
+-rw-rw-r--   0 root         (0)     1003     1625 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003     1451 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4125 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.805092 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    56334 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63536 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5969 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12955 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21504 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21939 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    59846 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1141 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11389 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1396 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2620 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.809091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51605 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58819 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6014 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12185 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20383 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20782 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1081 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10282 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/
+-rw-r--r--   0 root         (0)     1003     4849 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3168 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-17 10:42:42.000000 google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-04-17 10:42:42.817091 google-cloud-bigquery-datapolicies-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3055 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   224205 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-17 10:42:42.813091 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   123065 2023-04-17 10:40:10.000000 google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/LICENSE` & `google-cloud-bigquery-datapolicies-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/MANIFEST.in` & `google-cloud-bigquery-datapolicies-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.3.2
+Version: 0.4.0
 Summary: Google Cloud Bigquery Datapolicies API client library
 Home-page: https://github.com/googleapis/python-bigquery-datapolicies
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/README.rst` & `google-cloud-bigquery-datapolicies-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,36 +14,38 @@
 # limitations under the License.
 #
 from google.cloud.bigquery.datapolicies import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.async_client import (
+from google.cloud.bigquery.datapolicies_v1.services.data_policy_service.async_client import (
     DataPolicyServiceAsyncClient,
 )
-from google.cloud.bigquery.datapolicies_v1beta1.services.data_policy_service.client import (
+from google.cloud.bigquery.datapolicies_v1.services.data_policy_service.client import (
     DataPolicyServiceClient,
 )
-from google.cloud.bigquery.datapolicies_v1beta1.types.datapolicy import (
+from google.cloud.bigquery.datapolicies_v1.types.datapolicy import (
     CreateDataPolicyRequest,
     DataMaskingPolicy,
     DataPolicy,
     DeleteDataPolicyRequest,
     GetDataPolicyRequest,
     ListDataPoliciesRequest,
     ListDataPoliciesResponse,
+    RenameDataPolicyRequest,
     UpdateDataPolicyRequest,
 )
 
 __all__ = (
     "DataPolicyServiceClient",
     "DataPolicyServiceAsyncClient",
     "CreateDataPolicyRequest",
     "DataMaskingPolicy",
     "DataPolicy",
     "DeleteDataPolicyRequest",
     "GetDataPolicyRequest",
     "ListDataPoliciesRequest",
     "ListDataPoliciesResponse",
+    "RenameDataPolicyRequest",
     "UpdateDataPolicyRequest",
 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/services/data_policy_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1/types/datapolicy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/gapic_version.py`

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
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.4.0/google/cloud/bigquery/datapolicies_v1beta1/types/datapolicy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.3.2
+Version: 0.4.0
 Summary: Google Cloud Bigquery Datapolicies API client library
 Home-page: https://github.com/googleapis/python-bigquery-datapolicies
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt` & `google-cloud-bigquery-datapolicies-0.4.0/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/setup.py` & `google-cloud-bigquery-datapolicies-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1/test_data_policy_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.3.2/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.4.0/tests/unit/gapic/datapolicies_v1beta1/test_data_policy_service.py`

 * *Files identical despite different names*

