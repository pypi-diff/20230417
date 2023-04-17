# Comparing `tmp/google-cloud-dataproc-metastore-1.9.0.tar.gz` & `tmp/google-cloud-dataproc-metastore-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataproc-metastore-1.9.0.tar", last modified: Tue Jan 10 19:32:32 2023, max compression
+gzip compressed data, was "google-cloud-dataproc-metastore-1.9.1.tar", last modified: Mon Jan 23 16:18:25 2023, max compression
```

## Comparing `google-cloud-dataproc-metastore-1.9.0.tar` & `google-cloud-dataproc-metastore-1.9.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4918 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3969 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.589912 google-cloud-dataproc-metastore-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.589912 google-cloud-dataproc-metastore-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.593912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/
--rw-rw-r--   0 root         (0)     1003     3611 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.593912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/
--rw-rw-r--   0 root         (0)     1003     3320 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5875 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.593912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.593912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/__init__.py
--rw-rw-r--   0 root         (0)     1003    87083 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/async_client.py
--rw-rw-r--   0 root         (0)     1003   100206 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/client.py
--rw-rw-r--   0 root         (0)     1003    15766 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.593912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12386 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28966 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29706 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/
--rw-rw-r--   0 root         (0)     1003      821 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/__init__.py
--rw-rw-r--   0 root         (0)     1003    36759 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/async_client.py
--rw-rw-r--   0 root         (0)     1003    46224 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/client.py
--rw-rw-r--   0 root         (0)     1003     5968 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/
--rw-rw-r--   0 root         (0)     1003     1318 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8214 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18038 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18431 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/
--rw-rw-r--   0 root         (0)     1003     2794 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    59064 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/metastore.py
--rw-rw-r--   0 root         (0)     1003    14470 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/metastore_federation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/
--rw-rw-r--   0 root         (0)     1003     4078 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     6967 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.597912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/__init__.py
--rw-rw-r--   0 root         (0)     1003   103198 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/async_client.py
--rw-rw-r--   0 root         (0)     1003   117420 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/client.py
--rw-rw-r--   0 root         (0)     1003    15891 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14272 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34013 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34878 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/
--rw-rw-r--   0 root         (0)     1003      821 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/__init__.py
--rw-rw-r--   0 root         (0)     1003    36904 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/async_client.py
--rw-rw-r--   0 root         (0)     1003    46369 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/client.py
--rw-rw-r--   0 root         (0)     1003     6013 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/
--rw-rw-r--   0 root         (0)     1003     1318 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8224 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18068 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18461 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     3552 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    70907 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/metastore.py
--rw-rw-r--   0 root         (0)     1003    14526 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/metastore_federation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/
--rw-rw-r--   0 root         (0)     1003     4078 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     6965 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.601912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.605912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/
--rw-rw-r--   0 root         (0)     1003      781 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/__init__.py
--rw-rw-r--   0 root         (0)     1003   103072 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/async_client.py
--rw-rw-r--   0 root         (0)     1003   117294 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/client.py
--rw-rw-r--   0 root         (0)     1003    15866 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.605912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14270 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33993 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34858 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.605912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/
--rw-rw-r--   0 root         (0)     1003      821 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/__init__.py
--rw-rw-r--   0 root         (0)     1003    36875 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/async_client.py
--rw-rw-r--   0 root         (0)     1003    46340 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/client.py
--rw-rw-r--   0 root         (0)     1003     6004 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.605912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/
--rw-rw-r--   0 root         (0)     1003     1318 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8222 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18062 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18455 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.605912 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     3552 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    70831 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/metastore.py
--rw-rw-r--   0 root         (0)     1003    14519 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/metastore_federation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/
--rw-r--r--   0 root         (0)     1003     4918 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6096 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 19:32:32.000000 google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3009 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   207484 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/test_dataproc_metastore.py
--rw-rw-r--   0 root         (0)     1003   107360 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/test_dataproc_metastore_federation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   230193 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore.py
--rw-rw-r--   0 root         (0)     1003   107390 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore_federation.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 19:32:32.609912 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   230187 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore.py
--rw-rw-r--   0 root         (0)     1003   107384 2023-01-10 19:29:51.000000 google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.506810 google-cloud-dataproc-metastore-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4918 2023-01-23 16:18:25.506810 google-cloud-dataproc-metastore-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3969 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.482809 google-cloud-dataproc-metastore-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.482809 google-cloud-dataproc-metastore-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.486809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/
+-rw-rw-r--   0 root         (0)     1003     3611 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.486809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/
+-rw-rw-r--   0 root         (0)     1003     3320 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5875 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.486809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.486809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/
+-rw-rw-r--   0 root         (0)     1003      781 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003    87083 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/async_client.py
+-rw-rw-r--   0 root         (0)     1003   100235 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/client.py
+-rw-rw-r--   0 root         (0)     1003    15766 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12386 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28966 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29706 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/
+-rw-rw-r--   0 root         (0)     1003      821 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36759 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46263 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/client.py
+-rw-rw-r--   0 root         (0)     1003     5968 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/
+-rw-rw-r--   0 root         (0)     1003     1318 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8214 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18038 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18431 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2794 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    64570 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/metastore.py
+-rw-rw-r--   0 root         (0)     1003    15585 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     4078 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6967 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.490809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.494809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/
+-rw-rw-r--   0 root         (0)     1003      781 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103198 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/async_client.py
+-rw-rw-r--   0 root         (0)     1003   117449 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/client.py
+-rw-rw-r--   0 root         (0)     1003    15891 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.494809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14272 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34013 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34878 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.494809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/
+-rw-rw-r--   0 root         (0)     1003      821 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36904 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46408 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/client.py
+-rw-rw-r--   0 root         (0)     1003     6013 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.494809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/
+-rw-rw-r--   0 root         (0)     1003     1318 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8224 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18068 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18461 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.494809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     3552 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76771 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/metastore.py
+-rw-rw-r--   0 root         (0)     1003    15718 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/
+-rw-rw-r--   0 root         (0)     1003     4078 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6965 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/
+-rw-rw-r--   0 root         (0)     1003      781 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103072 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/async_client.py
+-rw-rw-r--   0 root         (0)     1003   117323 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/client.py
+-rw-rw-r--   0 root         (0)     1003    15866 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14270 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33993 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34858 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/
+-rw-rw-r--   0 root         (0)     1003      821 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36875 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/async_client.py
+-rw-rw-r--   0 root         (0)     1003    46379 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/client.py
+-rw-rw-r--   0 root         (0)     1003     6004 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/
+-rw-rw-r--   0 root         (0)     1003     1318 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8222 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18062 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18455 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.498809 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     3552 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    76695 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/metastore.py
+-rw-rw-r--   0 root         (0)     1003    15711 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/
+-rw-r--r--   0 root         (0)     1003     4918 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6096 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:18:25.000000 google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:18:25.506810 google-cloud-dataproc-metastore-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3009 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   207484 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/test_dataproc_metastore.py
+-rw-rw-r--   0 root         (0)     1003   107360 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/test_dataproc_metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.502809 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   230193 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore.py
+-rw-rw-r--   0 root         (0)     1003   107390 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore_federation.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:25.506810 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   230187 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore.py
+-rw-rw-r--   0 root         (0)     1003   107384 2023-01-23 16:15:40.000000 google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore_federation.py
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/LICENSE` & `google-cloud-dataproc-metastore-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/MANIFEST.in` & `google-cloud-dataproc-metastore-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/PKG-INFO` & `google-cloud-dataproc-metastore-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc-metastore
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Dataproc Metastore API client library
 Home-page: https://github.com/googleapis/python-dataproc-metastore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/README.rst` & `google-cloud-dataproc-metastore-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore/gapic_version.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/gapic_metadata.json` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/gapic_version.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2416,15 +2416,15 @@
             empty_pb2.Empty,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
             empty_pb2.Empty,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreFederationClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/services/dataproc_metastore_federation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/metastore.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/metastore.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,42 +142,108 @@
         telemetry_config (google.cloud.metastore_v1.types.TelemetryConfig):
             The configuration specifying telemetry settings for the
             Dataproc Metastore service. If unspecified defaults to
             ``JSON``.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metastore service."""
+        r"""The current state of the metastore service.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore service is
+                unknown.
+            CREATING (1):
+                The metastore service is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore service is running and ready to
+                serve queries.
+            SUSPENDING (3):
+                The metastore service is entering suspension.
+                Its query-serving availability may cease
+                unexpectedly.
+            SUSPENDED (4):
+                The metastore service is suspended and unable
+                to serve queries.
+            UPDATING (5):
+                The metastore service is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (6):
+                The metastore service is undergoing deletion.
+                It cannot be used.
+            ERROR (7):
+                The metastore service has encountered an
+                error and cannot be used. The metastore service
+                should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         SUSPENDING = 3
         SUSPENDED = 4
         UPDATING = 5
         DELETING = 6
         ERROR = 7
 
     class Tier(proto.Enum):
-        r"""Available service tiers."""
+        r"""Available service tiers.
+
+        Values:
+            TIER_UNSPECIFIED (0):
+                The tier is not set.
+            DEVELOPER (1):
+                The developer tier provides limited
+                scalability and no fault tolerance. Good for
+                low-cost proof-of-concept.
+            ENTERPRISE (3):
+                The enterprise tier provides multi-zone high
+                availability, and sufficient scalability for
+                enterprise-level Dataproc Metastore workloads.
+        """
         TIER_UNSPECIFIED = 0
         DEVELOPER = 1
         ENTERPRISE = 3
 
     class ReleaseChannel(proto.Enum):
         r"""Release channels bundle features of varying levels of
         stability. Newer features may be introduced initially into less
         stable release channels and can be automatically promoted into
         more stable release channels.
+
+        Values:
+            RELEASE_CHANNEL_UNSPECIFIED (0):
+                Release channel is not specified.
+            CANARY (1):
+                The ``CANARY`` release channel contains the newest features,
+                which may be unstable and subject to unresolved issues with
+                no known workarounds. Services using the ``CANARY`` release
+                channel are not subject to any SLAs.
+            STABLE (2):
+                The ``STABLE`` release channel contains features that are
+                considered stable and have been validated for production
+                use.
         """
         RELEASE_CHANNEL_UNSPECIFIED = 0
         CANARY = 1
         STABLE = 2
 
     class DatabaseType(proto.Enum):
-        r"""The backend database type for the metastore service."""
+        r"""The backend database type for the metastore service.
+
+        Values:
+            DATABASE_TYPE_UNSPECIFIED (0):
+                The DATABASE_TYPE is not set.
+            MYSQL (1):
+                MySQL is used to persist the metastore data.
+            SPANNER (2):
+                Spanner is used to persist the metastore
+                data.
+        """
         DATABASE_TYPE_UNSPECIFIED = 0
         MYSQL = 1
         SPANNER = 2
 
     hive_metastore_config: "HiveMetastoreConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
@@ -468,15 +534,24 @@
     Attributes:
         log_format (google.cloud.metastore_v1.types.TelemetryConfig.LogFormat):
             The output format of the Dataproc Metastore
             service's logs.
     """
 
     class LogFormat(proto.Enum):
-        r""""""
+        r"""
+
+        Values:
+            LOG_FORMAT_UNSPECIFIED (0):
+                The LOG_FORMAT is not set.
+            LEGACY (1):
+                Logging output uses the legacy ``textPayload`` format.
+            JSON (2):
+                Logging output uses the ``jsonPayload`` format.
+        """
         LOG_FORMAT_UNSPECIFIED = 0
         LEGACY = 1
         JSON = 2
 
     log_format: LogFormat = proto.Field(
         proto.ENUM,
         number=1,
@@ -537,15 +612,29 @@
             import finished.
         state (google.cloud.metastore_v1.types.MetadataImport.State):
             Output only. The current state of the
             metadata import.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata import."""
+        r"""The current state of the metadata import.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata import is unknown.
+            RUNNING (1):
+                The metadata import is running.
+            SUCCEEDED (2):
+                The metadata import completed successfully.
+            UPDATING (3):
+                The metadata import is being updated.
+            FAILED (4):
+                The metadata import failed, and attempted
+                metadata changes were rolled back.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         UPDATING = 3
         FAILED = 4
 
     class DatabaseDump(proto.Message):
@@ -561,15 +650,22 @@
                 ``gs://``.
             type_ (google.cloud.metastore_v1.types.DatabaseDumpSpec.Type):
                 Optional. The type of the database dump. If unspecified,
                 defaults to ``MYSQL``.
         """
 
         class DatabaseType(proto.Enum):
-            r"""The type of the database."""
+            r"""The type of the database.
+
+            Values:
+                DATABASE_TYPE_UNSPECIFIED (0):
+                    The type of the source database is unknown.
+                MYSQL (1):
+                    The type of the source database is MySQL.
+            """
             DATABASE_TYPE_UNSPECIFIED = 0
             MYSQL = 1
 
         database_type: "MetadataImport.DatabaseDump.DatabaseType" = proto.Field(
             proto.ENUM,
             number=1,
             enum="MetadataImport.DatabaseDump.DatabaseType",
@@ -641,15 +737,28 @@
         state (google.cloud.metastore_v1.types.MetadataExport.State):
             Output only. The current state of the export.
         database_dump_type (google.cloud.metastore_v1.types.DatabaseDumpSpec.Type):
             Output only. The type of the database dump.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata export."""
+        r"""The current state of the metadata export.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata export is unknown.
+            RUNNING (1):
+                The metadata export is running.
+            SUCCEEDED (2):
+                The metadata export completed successfully.
+            FAILED (3):
+                The metadata export failed.
+            CANCELLED (4):
+                The metadata export is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     destination_gcs_uri: str = proto.Field(
@@ -703,15 +812,30 @@
             The description of the backup.
         restoring_services (MutableSequence[str]):
             Output only. Services that are restoring from
             the backup.
     """
 
     class State(proto.Enum):
-        r"""The current state of the backup."""
+        r"""The current state of the backup.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the backup is unknown.
+            CREATING (1):
+                The backup is being created.
+            DELETING (2):
+                The backup is being deleted.
+            ACTIVE (3):
+                The backup is active and ready to use.
+            FAILED (4):
+                The backup failed.
+            RESTORING (5):
+                The backup is being restored.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         DELETING = 2
         ACTIVE = 3
         FAILED = 4
         RESTORING = 5
 
@@ -771,23 +895,46 @@
         details (str):
             Output only. The restore details containing
             the revision of the service to be restored to,
             in format of JSON.
     """
 
     class State(proto.Enum):
-        r"""The current state of the restore."""
+        r"""The current state of the restore.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata restore is unknown.
+            RUNNING (1):
+                The metadata restore is running.
+            SUCCEEDED (2):
+                The metadata restore completed successfully.
+            FAILED (3):
+                The metadata restore failed.
+            CANCELLED (4):
+                The metadata restore is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     class RestoreType(proto.Enum):
-        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``."""
+        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``.
+
+        Values:
+            RESTORE_TYPE_UNSPECIFIED (0):
+                The restore type is unknown.
+            FULL (1):
+                The service's metadata and configuration are
+                restored.
+            METADATA_ONLY (2):
+                Only the service's metadata is restored.
+        """
         RESTORE_TYPE_UNSPECIFIED = 0
         FULL = 1
         METADATA_ONLY = 2
 
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=1,
@@ -1731,14 +1878,23 @@
 class DatabaseDumpSpec(proto.Message):
     r"""The specification of database dump to import from or export
     to.
 
     """
 
     class Type(proto.Enum):
-        r"""The type of the database dump."""
+        r"""The type of the database dump.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                The type of the database dump is unknown.
+            MYSQL (1):
+                Database dump is a MySQL dump file.
+            AVRO (2):
+                Database dump contains Avro files.
+        """
         TYPE_UNSPECIFIED = 0
         MYSQL = 1
         AVRO = 2
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1/types/metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1/types/metastore_federation.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,38 @@
             available.
         uid (str):
             Output only. The globally unique resource
             identifier of the metastore federation.
     """
 
     class State(proto.Enum):
-        r"""The current state of the federation."""
+        r"""The current state of the federation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore federation is
+                unknown.
+            CREATING (1):
+                The metastore federation is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore federation is running and ready
+                to serve queries.
+            UPDATING (3):
+                The metastore federation is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (4):
+                The metastore federation is undergoing
+                deletion. It cannot be used.
+            ERROR (5):
+                The metastore federation has encountered an
+                error and cannot be used. The metastore
+                federation should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         UPDATING = 3
         DELETING = 4
         ERROR = 5
 
@@ -157,15 +180,22 @@
 
                -  ``projects/{project_id}/locations/{location}/services/{service_id}``
         metastore_type (google.cloud.metastore_v1.types.BackendMetastore.MetastoreType):
             The type of the backend metastore.
     """
 
     class MetastoreType(proto.Enum):
-        r"""The type of the backend metastore."""
+        r"""The type of the backend metastore.
+
+        Values:
+            METASTORE_TYPE_UNSPECIFIED (0):
+                The metastore type is not set.
+            DATAPROC_METASTORE (3):
+                The backend metastore is Dataproc Metastore.
+        """
         METASTORE_TYPE_UNSPECIFIED = 0
         DATAPROC_METASTORE = 3
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/gapic_metadata.json` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/gapic_version.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2818,15 +2818,15 @@
             metastore.AlterMetadataResourceLocationResponse,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
             empty_pb2.Empty,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreFederationClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/services/dataproc_metastore_federation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/metastore.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/metastore.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,42 +159,108 @@
         telemetry_config (google.cloud.metastore_v1alpha.types.TelemetryConfig):
             The configuration specifying telemetry settings for the
             Dataproc Metastore service. If unspecified defaults to
             ``JSON``.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metastore service."""
+        r"""The current state of the metastore service.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore service is
+                unknown.
+            CREATING (1):
+                The metastore service is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore service is running and ready to
+                serve queries.
+            SUSPENDING (3):
+                The metastore service is entering suspension.
+                Its query-serving availability may cease
+                unexpectedly.
+            SUSPENDED (4):
+                The metastore service is suspended and unable
+                to serve queries.
+            UPDATING (5):
+                The metastore service is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (6):
+                The metastore service is undergoing deletion.
+                It cannot be used.
+            ERROR (7):
+                The metastore service has encountered an
+                error and cannot be used. The metastore service
+                should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         SUSPENDING = 3
         SUSPENDED = 4
         UPDATING = 5
         DELETING = 6
         ERROR = 7
 
     class Tier(proto.Enum):
-        r"""Available service tiers."""
+        r"""Available service tiers.
+
+        Values:
+            TIER_UNSPECIFIED (0):
+                The tier is not set.
+            DEVELOPER (1):
+                The developer tier provides limited
+                scalability and no fault tolerance. Good for
+                low-cost proof-of-concept.
+            ENTERPRISE (3):
+                The enterprise tier provides multi-zone high
+                availability, and sufficient scalability for
+                enterprise-level Dataproc Metastore workloads.
+        """
         TIER_UNSPECIFIED = 0
         DEVELOPER = 1
         ENTERPRISE = 3
 
     class ReleaseChannel(proto.Enum):
         r"""Release channels bundle features of varying levels of
         stability. Newer features may be introduced initially into less
         stable release channels and can be automatically promoted into
         more stable release channels.
+
+        Values:
+            RELEASE_CHANNEL_UNSPECIFIED (0):
+                Release channel is not specified.
+            CANARY (1):
+                The ``CANARY`` release channel contains the newest features,
+                which may be unstable and subject to unresolved issues with
+                no known workarounds. Services using the ``CANARY`` release
+                channel are not subject to any SLAs.
+            STABLE (2):
+                The ``STABLE`` release channel contains features that are
+                considered stable and have been validated for production
+                use.
         """
         RELEASE_CHANNEL_UNSPECIFIED = 0
         CANARY = 1
         STABLE = 2
 
     class DatabaseType(proto.Enum):
-        r"""The backend database type for the metastore service."""
+        r"""The backend database type for the metastore service.
+
+        Values:
+            DATABASE_TYPE_UNSPECIFIED (0):
+                The DATABASE_TYPE is not set.
+            MYSQL (1):
+                MySQL is used to persist the metastore data.
+            SPANNER (2):
+                Spanner is used to persist the metastore
+                data.
+        """
         DATABASE_TYPE_UNSPECIFIED = 0
         MYSQL = 1
         SPANNER = 2
 
     hive_metastore_config: "HiveMetastoreConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
@@ -434,14 +500,24 @@
             lowercase letters, or digits, except the last character,
             which cannot be a hyphen.
     """
 
     class EndpointProtocol(proto.Enum):
         r"""Protocols available for serving the metastore service
         endpoint.
+
+        Values:
+            ENDPOINT_PROTOCOL_UNSPECIFIED (0):
+                The protocol is not set.
+            THRIFT (1):
+                Use the legacy Apache Thrift protocol for the
+                metastore service endpoint.
+            GRPC (2):
+                Use the modernized gRPC protocol for the
+                metastore service endpoint.
         """
         ENDPOINT_PROTOCOL_UNSPECIFIED = 0
         THRIFT = 1
         GRPC = 2
 
     version: str = proto.Field(
         proto.STRING,
@@ -639,15 +715,24 @@
     Attributes:
         log_format (google.cloud.metastore_v1alpha.types.TelemetryConfig.LogFormat):
             The output format of the Dataproc Metastore
             service's logs.
     """
 
     class LogFormat(proto.Enum):
-        r""""""
+        r"""
+
+        Values:
+            LOG_FORMAT_UNSPECIFIED (0):
+                The LOG_FORMAT is not set.
+            LEGACY (1):
+                Logging output uses the legacy ``textPayload`` format.
+            JSON (2):
+                Logging output uses the ``jsonPayload`` format.
+        """
         LOG_FORMAT_UNSPECIFIED = 0
         LEGACY = 1
         JSON = 2
 
     log_format: LogFormat = proto.Field(
         proto.ENUM,
         number=1,
@@ -708,15 +793,29 @@
             import finished.
         state (google.cloud.metastore_v1alpha.types.MetadataImport.State):
             Output only. The current state of the
             metadata import.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata import."""
+        r"""The current state of the metadata import.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata import is unknown.
+            RUNNING (1):
+                The metadata import is running.
+            SUCCEEDED (2):
+                The metadata import completed successfully.
+            UPDATING (3):
+                The metadata import is being updated.
+            FAILED (4):
+                The metadata import failed, and attempted
+                metadata changes were rolled back.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         UPDATING = 3
         FAILED = 4
 
     class DatabaseDump(proto.Message):
@@ -734,15 +833,22 @@
                 The name of the source database.
             type_ (google.cloud.metastore_v1alpha.types.DatabaseDumpSpec.Type):
                 Optional. The type of the database dump. If unspecified,
                 defaults to ``MYSQL``.
         """
 
         class DatabaseType(proto.Enum):
-            r"""The type of the database."""
+            r"""The type of the database.
+
+            Values:
+                DATABASE_TYPE_UNSPECIFIED (0):
+                    The type of the source database is unknown.
+                MYSQL (1):
+                    The type of the source database is MySQL.
+            """
             DATABASE_TYPE_UNSPECIFIED = 0
             MYSQL = 1
 
         database_type: "MetadataImport.DatabaseDump.DatabaseType" = proto.Field(
             proto.ENUM,
             number=1,
             enum="MetadataImport.DatabaseDump.DatabaseType",
@@ -818,15 +924,28 @@
         state (google.cloud.metastore_v1alpha.types.MetadataExport.State):
             Output only. The current state of the export.
         database_dump_type (google.cloud.metastore_v1alpha.types.DatabaseDumpSpec.Type):
             Output only. The type of the database dump.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata export."""
+        r"""The current state of the metadata export.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata export is unknown.
+            RUNNING (1):
+                The metadata export is running.
+            SUCCEEDED (2):
+                The metadata export completed successfully.
+            FAILED (3):
+                The metadata export failed.
+            CANCELLED (4):
+                The metadata export is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     destination_gcs_uri: str = proto.Field(
@@ -880,15 +999,30 @@
             The description of the backup.
         restoring_services (MutableSequence[str]):
             Output only. Services that are restoring from
             the backup.
     """
 
     class State(proto.Enum):
-        r"""The current state of the backup."""
+        r"""The current state of the backup.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the backup is unknown.
+            CREATING (1):
+                The backup is being created.
+            DELETING (2):
+                The backup is being deleted.
+            ACTIVE (3):
+                The backup is active and ready to use.
+            FAILED (4):
+                The backup failed.
+            RESTORING (5):
+                The backup is being restored.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         DELETING = 2
         ACTIVE = 3
         FAILED = 4
         RESTORING = 5
 
@@ -948,23 +1082,46 @@
         details (str):
             Output only. The restore details containing
             the revision of the service to be restored to,
             in format of JSON.
     """
 
     class State(proto.Enum):
-        r"""The current state of the restore."""
+        r"""The current state of the restore.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata restore is unknown.
+            RUNNING (1):
+                The metadata restore is running.
+            SUCCEEDED (2):
+                The metadata restore completed successfully.
+            FAILED (3):
+                The metadata restore failed.
+            CANCELLED (4):
+                The metadata restore is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     class RestoreType(proto.Enum):
-        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``."""
+        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``.
+
+        Values:
+            RESTORE_TYPE_UNSPECIFIED (0):
+                The restore type is unknown.
+            FULL (1):
+                The service's metadata and configuration are
+                restored.
+            METADATA_ONLY (2):
+                Only the service's metadata is restored.
+        """
         RESTORE_TYPE_UNSPECIFIED = 0
         FULL = 1
         METADATA_ONLY = 2
 
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=1,
@@ -1908,15 +2065,24 @@
 class DatabaseDumpSpec(proto.Message):
     r"""The specification of database dump to import from or export
     to.
 
     """
 
     class Type(proto.Enum):
-        r"""The type of the database dump."""
+        r"""The type of the database dump.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                The type of the database dump is unknown.
+            MYSQL (1):
+                Database dump is a MySQL dump file.
+            AVRO (2):
+                Database dump contains Avro files.
+        """
         TYPE_UNSPECIFIED = 0
         MYSQL = 1
         AVRO = 2
 
 
 class RemoveIamPolicyRequest(proto.Message):
     r"""Request message for
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1alpha/types/metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1alpha/types/metastore_federation.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,38 @@
             available.
         uid (str):
             Output only. The globally unique resource
             identifier of the metastore federation.
     """
 
     class State(proto.Enum):
-        r"""The current state of the federation."""
+        r"""The current state of the federation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore federation is
+                unknown.
+            CREATING (1):
+                The metastore federation is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore federation is running and ready
+                to serve queries.
+            UPDATING (3):
+                The metastore federation is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (4):
+                The metastore federation is undergoing
+                deletion. It cannot be used.
+            ERROR (5):
+                The metastore federation has encountered an
+                error and cannot be used. The metastore
+                federation should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         UPDATING = 3
         DELETING = 4
         ERROR = 5
 
@@ -157,15 +180,24 @@
 
                -  ``projects/{project_id}/locations/{location}/services/{service_id}``
         metastore_type (google.cloud.metastore_v1alpha.types.BackendMetastore.MetastoreType):
             The type of the backend metastore.
     """
 
     class MetastoreType(proto.Enum):
-        r"""The type of the backend metastore."""
+        r"""The type of the backend metastore.
+
+        Values:
+            METASTORE_TYPE_UNSPECIFIED (0):
+                The metastore type is not set.
+            BIGQUERY (2):
+                The backend metastore is BigQuery.
+            DATAPROC_METASTORE (3):
+                The backend metastore is Dataproc Metastore.
+        """
         METASTORE_TYPE_UNSPECIFIED = 0
         BIGQUERY = 2
         DATAPROC_METASTORE = 3
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/gapic_metadata.json` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/gapic_version.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2818,15 +2818,15 @@
             metastore.AlterMetadataResourceLocationResponse,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/async_client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/client.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
             empty_pb2.Empty,
             metadata_type=metastore.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    def __enter__(self):
+    def __enter__(self) -> "DataprocMetastoreFederationClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/pagers.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/base.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc_asyncio.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/services/dataproc_metastore_federation/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/metastore.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/metastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,42 +159,108 @@
         telemetry_config (google.cloud.metastore_v1beta.types.TelemetryConfig):
             The configuration specifying telemetry settings for the
             Dataproc Metastore service. If unspecified defaults to
             ``JSON``.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metastore service."""
+        r"""The current state of the metastore service.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore service is
+                unknown.
+            CREATING (1):
+                The metastore service is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore service is running and ready to
+                serve queries.
+            SUSPENDING (3):
+                The metastore service is entering suspension.
+                Its query-serving availability may cease
+                unexpectedly.
+            SUSPENDED (4):
+                The metastore service is suspended and unable
+                to serve queries.
+            UPDATING (5):
+                The metastore service is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (6):
+                The metastore service is undergoing deletion.
+                It cannot be used.
+            ERROR (7):
+                The metastore service has encountered an
+                error and cannot be used. The metastore service
+                should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         SUSPENDING = 3
         SUSPENDED = 4
         UPDATING = 5
         DELETING = 6
         ERROR = 7
 
     class Tier(proto.Enum):
-        r"""Available service tiers."""
+        r"""Available service tiers.
+
+        Values:
+            TIER_UNSPECIFIED (0):
+                The tier is not set.
+            DEVELOPER (1):
+                The developer tier provides limited
+                scalability and no fault tolerance. Good for
+                low-cost proof-of-concept.
+            ENTERPRISE (3):
+                The enterprise tier provides multi-zone high
+                availability, and sufficient scalability for
+                enterprise-level Dataproc Metastore workloads.
+        """
         TIER_UNSPECIFIED = 0
         DEVELOPER = 1
         ENTERPRISE = 3
 
     class ReleaseChannel(proto.Enum):
         r"""Release channels bundle features of varying levels of
         stability. Newer features may be introduced initially into less
         stable release channels and can be automatically promoted into
         more stable release channels.
+
+        Values:
+            RELEASE_CHANNEL_UNSPECIFIED (0):
+                Release channel is not specified.
+            CANARY (1):
+                The ``CANARY`` release channel contains the newest features,
+                which may be unstable and subject to unresolved issues with
+                no known workarounds. Services using the ``CANARY`` release
+                channel are not subject to any SLAs.
+            STABLE (2):
+                The ``STABLE`` release channel contains features that are
+                considered stable and have been validated for production
+                use.
         """
         RELEASE_CHANNEL_UNSPECIFIED = 0
         CANARY = 1
         STABLE = 2
 
     class DatabaseType(proto.Enum):
-        r"""The backend database type for the metastore service."""
+        r"""The backend database type for the metastore service.
+
+        Values:
+            DATABASE_TYPE_UNSPECIFIED (0):
+                The DATABASE_TYPE is not set.
+            MYSQL (1):
+                MySQL is used to persist the metastore data.
+            SPANNER (2):
+                Spanner is used to persist the metastore
+                data.
+        """
         DATABASE_TYPE_UNSPECIFIED = 0
         MYSQL = 1
         SPANNER = 2
 
     hive_metastore_config: "HiveMetastoreConfig" = proto.Field(
         proto.MESSAGE,
         number=5,
@@ -434,14 +500,24 @@
             lowercase letters, or digits, except the last character,
             which cannot be a hyphen.
     """
 
     class EndpointProtocol(proto.Enum):
         r"""Protocols available for serving the metastore service
         endpoint.
+
+        Values:
+            ENDPOINT_PROTOCOL_UNSPECIFIED (0):
+                The protocol is not set.
+            THRIFT (1):
+                Use the legacy Apache Thrift protocol for the
+                metastore service endpoint.
+            GRPC (2):
+                Use the modernized gRPC protocol for the
+                metastore service endpoint.
         """
         ENDPOINT_PROTOCOL_UNSPECIFIED = 0
         THRIFT = 1
         GRPC = 2
 
     version: str = proto.Field(
         proto.STRING,
@@ -639,15 +715,24 @@
     Attributes:
         log_format (google.cloud.metastore_v1beta.types.TelemetryConfig.LogFormat):
             The output format of the Dataproc Metastore
             service's logs.
     """
 
     class LogFormat(proto.Enum):
-        r""""""
+        r"""
+
+        Values:
+            LOG_FORMAT_UNSPECIFIED (0):
+                The LOG_FORMAT is not set.
+            LEGACY (1):
+                Logging output uses the legacy ``textPayload`` format.
+            JSON (2):
+                Logging output uses the ``jsonPayload`` format.
+        """
         LOG_FORMAT_UNSPECIFIED = 0
         LEGACY = 1
         JSON = 2
 
     log_format: LogFormat = proto.Field(
         proto.ENUM,
         number=1,
@@ -708,15 +793,29 @@
             import finished.
         state (google.cloud.metastore_v1beta.types.MetadataImport.State):
             Output only. The current state of the
             metadata import.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata import."""
+        r"""The current state of the metadata import.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata import is unknown.
+            RUNNING (1):
+                The metadata import is running.
+            SUCCEEDED (2):
+                The metadata import completed successfully.
+            UPDATING (3):
+                The metadata import is being updated.
+            FAILED (4):
+                The metadata import failed, and attempted
+                metadata changes were rolled back.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         UPDATING = 3
         FAILED = 4
 
     class DatabaseDump(proto.Message):
@@ -734,15 +833,22 @@
                 The name of the source database.
             type_ (google.cloud.metastore_v1beta.types.DatabaseDumpSpec.Type):
                 Optional. The type of the database dump. If unspecified,
                 defaults to ``MYSQL``.
         """
 
         class DatabaseType(proto.Enum):
-            r"""The type of the database."""
+            r"""The type of the database.
+
+            Values:
+                DATABASE_TYPE_UNSPECIFIED (0):
+                    The type of the source database is unknown.
+                MYSQL (1):
+                    The type of the source database is MySQL.
+            """
             DATABASE_TYPE_UNSPECIFIED = 0
             MYSQL = 1
 
         database_type: "MetadataImport.DatabaseDump.DatabaseType" = proto.Field(
             proto.ENUM,
             number=1,
             enum="MetadataImport.DatabaseDump.DatabaseType",
@@ -818,15 +924,28 @@
         state (google.cloud.metastore_v1beta.types.MetadataExport.State):
             Output only. The current state of the export.
         database_dump_type (google.cloud.metastore_v1beta.types.DatabaseDumpSpec.Type):
             Output only. The type of the database dump.
     """
 
     class State(proto.Enum):
-        r"""The current state of the metadata export."""
+        r"""The current state of the metadata export.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata export is unknown.
+            RUNNING (1):
+                The metadata export is running.
+            SUCCEEDED (2):
+                The metadata export completed successfully.
+            FAILED (3):
+                The metadata export failed.
+            CANCELLED (4):
+                The metadata export is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     destination_gcs_uri: str = proto.Field(
@@ -880,15 +999,30 @@
             The description of the backup.
         restoring_services (MutableSequence[str]):
             Output only. Services that are restoring from
             the backup.
     """
 
     class State(proto.Enum):
-        r"""The current state of the backup."""
+        r"""The current state of the backup.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the backup is unknown.
+            CREATING (1):
+                The backup is being created.
+            DELETING (2):
+                The backup is being deleted.
+            ACTIVE (3):
+                The backup is active and ready to use.
+            FAILED (4):
+                The backup failed.
+            RESTORING (5):
+                The backup is being restored.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         DELETING = 2
         ACTIVE = 3
         FAILED = 4
         RESTORING = 5
 
@@ -948,23 +1082,46 @@
         details (str):
             Output only. The restore details containing
             the revision of the service to be restored to,
             in format of JSON.
     """
 
     class State(proto.Enum):
-        r"""The current state of the restore."""
+        r"""The current state of the restore.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metadata restore is unknown.
+            RUNNING (1):
+                The metadata restore is running.
+            SUCCEEDED (2):
+                The metadata restore completed successfully.
+            FAILED (3):
+                The metadata restore failed.
+            CANCELLED (4):
+                The metadata restore is cancelled.
+        """
         STATE_UNSPECIFIED = 0
         RUNNING = 1
         SUCCEEDED = 2
         FAILED = 3
         CANCELLED = 4
 
     class RestoreType(proto.Enum):
-        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``."""
+        r"""The type of restore. If unspecified, defaults to ``METADATA_ONLY``.
+
+        Values:
+            RESTORE_TYPE_UNSPECIFIED (0):
+                The restore type is unknown.
+            FULL (1):
+                The service's metadata and configuration are
+                restored.
+            METADATA_ONLY (2):
+                Only the service's metadata is restored.
+        """
         RESTORE_TYPE_UNSPECIFIED = 0
         FULL = 1
         METADATA_ONLY = 2
 
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=1,
@@ -1908,15 +2065,24 @@
 class DatabaseDumpSpec(proto.Message):
     r"""The specification of database dump to import from or export
     to.
 
     """
 
     class Type(proto.Enum):
-        r"""The type of the database dump."""
+        r"""The type of the database dump.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                The type of the database dump is unknown.
+            MYSQL (1):
+                Database dump is a MySQL dump file.
+            AVRO (2):
+                Database dump contains Avro files.
+        """
         TYPE_UNSPECIFIED = 0
         MYSQL = 1
         AVRO = 2
 
 
 class RemoveIamPolicyRequest(proto.Message):
     r"""Request message for
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google/cloud/metastore_v1beta/types/metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/google/cloud/metastore_v1beta/types/metastore_federation.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,38 @@
             available.
         uid (str):
             Output only. The globally unique resource
             identifier of the metastore federation.
     """
 
     class State(proto.Enum):
-        r"""The current state of the federation."""
+        r"""The current state of the federation.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The state of the metastore federation is
+                unknown.
+            CREATING (1):
+                The metastore federation is in the process of
+                being created.
+            ACTIVE (2):
+                The metastore federation is running and ready
+                to serve queries.
+            UPDATING (3):
+                The metastore federation is being updated. It
+                remains usable but cannot accept additional
+                update requests or be deleted at this time.
+            DELETING (4):
+                The metastore federation is undergoing
+                deletion. It cannot be used.
+            ERROR (5):
+                The metastore federation has encountered an
+                error and cannot be used. The metastore
+                federation should be deleted.
+        """
         STATE_UNSPECIFIED = 0
         CREATING = 1
         ACTIVE = 2
         UPDATING = 3
         DELETING = 4
         ERROR = 5
 
@@ -157,15 +180,24 @@
 
                -  ``projects/{project_id}/locations/{location}/services/{service_id}``
         metastore_type (google.cloud.metastore_v1beta.types.BackendMetastore.MetastoreType):
             The type of the backend metastore.
     """
 
     class MetastoreType(proto.Enum):
-        r"""The type of the backend metastore."""
+        r"""The type of the backend metastore.
+
+        Values:
+            METASTORE_TYPE_UNSPECIFIED (0):
+                The metastore type is not set.
+            BIGQUERY (2):
+                The backend metastore is BigQuery.
+            DATAPROC_METASTORE (3):
+                The backend metastore is Dataproc Metastore.
+        """
         METASTORE_TYPE_UNSPECIFIED = 0
         BIGQUERY = 2
         DATAPROC_METASTORE = 3
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/PKG-INFO` & `google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataproc-metastore
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Dataproc Metastore API client library
 Home-page: https://github.com/googleapis/python-dataproc-metastore
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataproc-metastore-1.9.0/google_cloud_dataproc_metastore.egg-info/SOURCES.txt` & `google-cloud-dataproc-metastore-1.9.1/google_cloud_dataproc_metastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/setup.py` & `google-cloud-dataproc-metastore-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/test_dataproc_metastore.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/test_dataproc_metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1/test_dataproc_metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1/test_dataproc_metastore_federation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1alpha/test_dataproc_metastore_federation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/__init__.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataproc-metastore-1.9.0/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore_federation.py` & `google-cloud-dataproc-metastore-1.9.1/tests/unit/gapic/metastore_v1beta/test_dataproc_metastore_federation.py`

 * *Files identical despite different names*

