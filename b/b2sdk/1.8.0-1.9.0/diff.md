# Comparing `tmp/b2sdk-1.8.0.tar.gz` & `tmp/b2sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sdk-1.8.0.tar", last modified: Fri May 21 01:00:54 2021, max compression
+gzip compressed data, was "b2sdk-1.9.0.tar", last modified: Mon Jun  7 22:23:57 2021, max compression
```

## Comparing `b2sdk-1.8.0.tar` & `b2sdk-1.9.0.tar`

### file list

```diff
@@ -1,321 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.929958 b2sdk-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.897956 b2sdk-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.github/no-response.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.897956 b2sdk-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-05-21 01:00:49.000000 b2sdk-1.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6877 2021-05-21 01:00:49.000000 b2sdk-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-05-21 01:00:49.000000 b2sdk-1.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2021-05-21 01:00:49.000000 b2sdk-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-21 01:00:49.000000 b2sdk-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2021-05-21 01:00:54.929958 b2sdk-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-05-21 01:00:49.000000 b2sdk-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-05-21 01:00:49.000000 b2sdk-1.8.0/README.release.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/_pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/_pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/_pyinstaller/hook-b2sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/_v2/
--rw-r--r--   0 runner    (1001) docker     (121)     8582 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/_v2/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/account_info/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11920 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4306 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)    21789 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/sqlite_account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/stub.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/test_upload_url_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/account_info/upload_url_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    20551 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    17096 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    44233 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7027 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/download_dest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/encryption/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11562 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/encryption/setting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/encryption/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    15982 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    13787 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)     8732 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/file_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk/large_file/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/large_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/large_file/part.py
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/large_file/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/large_file/unfinished_large_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    46815 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    65343 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/raw_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    20284 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/chained.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/stream/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15339 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/encryption_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (121)    13319 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/folder_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    16948 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/policy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    11137 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    15194 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/transfer/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/transfer/emerge/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/emerger.py
--rw-r--r--   0 runner    (1001) docker     (121)    22612 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/transfer/emerge/planner/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/planner/part_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)    29454 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/planner/planner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/planner/upload_subpart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/emerge/write_intent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/transfer/inbound/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/download_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.905957 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)    14733 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/inbound/file_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/b2sdk/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11338 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/copy_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/large_file_upload_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/outbound_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/progress_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9807 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/upload_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6964 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/transfer/outbound/upload_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    12435 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/b2sdk/v0/
--rw-r--r--   0 runner    (1001) docker     (121)      670 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     7263 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v0/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/b2sdk/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5891 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/file_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/b2sdk/v1/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/sync/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/sync/folder_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/sync/scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/v1/sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2021-05-21 01:00:49.000000 b2sdk-1.8.0/b2sdk/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.901957 b2sdk-1.8.0/b2sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8119 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-05-21 01:00:54.000000 b2sdk-1.8.0/b2sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (121)      486 2021-05-21 01:00:49.000000 b2sdk-1.8.0/contrib/color-b2-logs.sh
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-05-21 01:00:49.000000 b2sdk-1.8.0/contrib/debug_logs.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.909957 b2sdk-1.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/bash_completion.md
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/markup-test.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)       84 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/render_sqlite_account_info_schema.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.913957 b2sdk-1.8.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)    20807 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/advanced.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.913957 b2sdk-1.8.0/doc/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4309 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/account_info.rst
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/bucket.rst
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/data_classes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      636 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/download_dest.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.913957 b2sdk-1.8.0/doc/source/api/encryption/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/encryption/setting.rst
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/encryption/types.rst
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)      847 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/file_lock.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.913957 b2sdk-1.8.0/doc/source/api/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/b2http.rst
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/download_dest.rst
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/raw_api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/raw_simulator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/session.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/internal/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/stream/chained.rst
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/stream/hashing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/stream/progress.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/stream/range.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/stream/wrapper.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/internal/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/action.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/file.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/folder.rst
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/folder_parser.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/policy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/policy_manager.rst
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/scan_policies.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/sync/sync.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.893956 b2sdk-1.8.0/doc/source/api/internal/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/download_manager.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/downloader/abstract.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/downloader/parallel.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/downloader/range.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/downloader/simple.rst
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/inbound/file_metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/internal/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/transfer/outbound/upload_source.rst
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/internal/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/progress.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8315 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/sync.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.893956 b2sdk-1.8.0/doc/source/api/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/transfer/emerge/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/transfer/emerge/write_intent.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/api/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/transfer/outbound/outbound_source.rst
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/api_types.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6630 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/doc/source/dot/
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/dot/sqlite_account_info_schema.dot
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/server_side_encryption.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/source/tutorial.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1052 2021-05-21 01:00:49.000000 b2sdk-1.8.0/doc/sqlite_account_info_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2021-05-21 01:00:49.000000 b2sdk-1.8.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-05-21 01:00:49.000000 b2sdk-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-05-21 01:00:54.929958 b2sdk-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2021-05-21 01:00:49.000000 b2sdk-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/integration/test_raw_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/test/static/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/static/test_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.917957 b2sdk-1.8.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/account_info/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/account_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/account_info/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)    16872 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/account_info/test_account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/account_info/test_sqlite_account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/file_lock/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/file_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/file_lock/test_legal_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/file_version/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/file_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/file_version/test_file_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/fixtures/b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/fixtures/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/fixtures/raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/fixtures/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/internal/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23009 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/internal/test_emerge_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.921957 b2sdk-1.8.0/test/unit/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/sync/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/sync/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/sync/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    32403 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/sync/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v0/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v0/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/apiver/apiver_deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     7663 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    49489 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_download_dest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_file_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    32972 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_sync_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v0/test_version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v1/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/apiver/apiver_deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    55383 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     6196 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_download_dest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_file_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     6817 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    34166 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_sync_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v1/test_version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v2/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.925958 b2sdk-1.8.0/test/unit/v2/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v2/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v2/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v2/apiver/apiver_deps_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 01:00:54.929958 b2sdk-1.8.0/test/unit/v_all/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-05-21 01:00:49.000000 b2sdk-1.8.0/test/unit/v_all/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.370168 b2sdk-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/no-response.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.370168 b2sdk-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2905 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     7781 2021-06-07 22:23:51.000000 b2sdk-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-06-07 22:23:51.000000 b2sdk-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2021-06-07 22:23:51.000000 b2sdk-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-07 22:23:51.000000 b2sdk-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-06-07 22:23:57.402168 b2sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-07 22:23:51.000000 b2sdk-1.9.0/README.release.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/_pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_pyinstaller/hook-b2sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/_v2/
+-rw-r--r--   0 runner    (1001) docker     (121)     8550 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_v2/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/account_info/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11920 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4306 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21789 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/sqlite_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4176 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/stub.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/test_upload_url_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/upload_url_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20530 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17096 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/b2http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/bounded_queue_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44096 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7027 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/download_dest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/encryption/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11557 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/setting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15966 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13787 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8901 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/file_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/large_file/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/part.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/unfinished_large_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5776 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46815 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/raw_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65343 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/raw_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/stream/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/chained.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/sync/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15187 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3967 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/encryption_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14288 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/folder_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17536 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3862 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/policy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11137 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9100 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/scan_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15571 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/emerge/
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4913 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/emerger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22537 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5317 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/part_definition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29454 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/planner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/upload_subpart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/write_intent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/inbound/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5584 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/download_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14733 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/range.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/file_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/transfer/outbound/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11309 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/copy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/copy_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/large_file_upload_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/outbound_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/progress_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9769 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/upload_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6964 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/upload_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12435 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v0/
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/account_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7265 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5891 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/account_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3972 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/file_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v1/sync/
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/encryption_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/file_to_path_translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/folder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/folder_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7122 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/scan_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5171 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7031 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8254 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/contrib/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      486 2021-06-07 22:23:51.000000 b2sdk-1.9.0/contrib/color-b2-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2021-06-07 22:23:51.000000 b2sdk-1.9.0/contrib/debug_logs.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/bash_completion.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4561 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/markup-test.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)       84 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/render_sqlite_account_info_schema.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (121)    20807 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/advanced.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     4401 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/account_info.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/bucket.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/data_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/download_dest.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/api/encryption/
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/encryption/setting.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/encryption/types.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/file_lock.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/b2http.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/download_dest.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/raw_api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/raw_simulator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/session.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/stream/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/chained.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/hashing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/progress.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/range.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/wrapper.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/sync/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/action.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/folder.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/folder_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/path.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/policy.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/policy_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/scan_policies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/sync.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.366168 b2sdk-1.9.0/doc/source/api/internal/transfer/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/download_manager.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/abstract.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/parallel.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/range.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/simple.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/file_metadata.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/outbound/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/outbound/upload_source.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/progress.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8407 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/sync.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.366168 b2sdk-1.9.0/doc/source/api/transfer/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/transfer/emerge/
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/transfer/emerge/write_intent.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/transfer/outbound/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/transfer/outbound/outbound_source.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6662 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api_types.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6630 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3357 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/dot/
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/dot/sqlite_account_info_schema.dot
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3269 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/server_side_encryption.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/tutorial.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1052 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/sqlite_account_info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6410 2021-06-07 22:23:51.000000 b2sdk-1.9.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2021-06-07 22:23:51.000000 b2sdk-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      940 2021-06-07 22:23:57.402168 b2sdk-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4764 2021-06-07 22:23:51.000000 b2sdk-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/integration/test_raw_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/static/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/static/test_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/account_info/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3140 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16872 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/test_account_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/test_sqlite_account_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12505 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/bucket/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/bucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56149 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/bucket/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4260 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/file_lock/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_lock/test_legal_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/file_version/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_version/test_file_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/b2http.py
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/raw_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23009 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/test_emerge_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/sync/
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4201 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2273 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_scan_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33498 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.398168 b2sdk-1.9.0/test/unit/v0/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.398168 b2sdk-1.9.0/test/unit/v0/apiver/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/apiver_deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/apiver_deps_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/deps_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_b2http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_bounded_queue_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49489 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6154 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_copy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_download_dest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_file_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_raw_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_scan_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34022 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_sync_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v1/apiver/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/apiver_deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/apiver_deps_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/deps_exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_b2http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_bounded_queue_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6196 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_copy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_download_dest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_file_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6817 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_raw_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_scan_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34972 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_sync_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v2/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v2/apiver/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/apiver_deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/apiver_deps_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v_all/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v_all/test_api.py
```

### Comparing `b2sdk-1.8.0/.github/SUPPORT.md` & `b2sdk-1.9.0/.github/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/.github/no-response.yml` & `b2sdk-1.9.0/.github/no-response.yml`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/.github/workflows/cd.yml` & `b2sdk-1.9.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/.github/workflows/ci.yml` & `b2sdk-1.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/.readthedocs.yml` & `b2sdk-1.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/CHANGELOG.md` & `b2sdk-1.9.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.9.0] - 2021-06-07
+
+### Added
+* `ScanPoliciesManager` is able to filter b2 files by upload timestamp
+
+### Changed
+* `Synchronizer.make_file_sync_actions` and `Synchronizer.make_folder_sync_actions` were made private in v2 interface
+* Refactored `sync.file.*File` and `sync.file.*FileVersion` to `sync.path.*SyncPath` in v2
+* Refactored `FileVersionInfo` to `FileVersion` in v2
+* `ScanPoliciesManager` exclusion interface changed in v2
+* `B2Api` unittests for v0, v1 and v2 are now common
+* `B2Api.cancel_large_file` returns a `FileIdAndName` object instead of a `FileVersion` object in v2
+* `FileVersion` has a mandatory `api` parameter in v2
+* `B2Folder` holds a handle to B2Api 
+* `Bucket` unit tests for v1 and v2 are now common
+
+### Fixed
+* Fix call to incorrect internal api in `B2Api.get_download_url_for_file_name`
+
 ## [1.8.0] - 2021-05-21
 
 ### Added
 * Add `get_bucket_name_or_none_from_bucket_id` to `AccountInfo` and `Cache`
 * Add possibility to change realm during integration tests
 * Add support for "file locks": file retention, legal hold and default bucket retention
 
@@ -179,15 +198,16 @@
 * Fix transferer crashing on empty file download attempt
 
 ## [0.1.4] - 2019-04-04
 
 ### Added
 Initial official release of SDK as a separate package (until now it was a part of B2 CLI)
 
-[Unreleased]: https://github.com/Backblaze/b2-sdk-python/compare/v1.8.0...HEAD
+[Unreleased]: https://github.com/Backblaze/b2-sdk-python/compare/v1.9.0...HEAD
+[1.9.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.8.0...v1.9.0
 [1.8.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.7.0...v1.8.0
 [1.7.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.6.0...v1.7.0
 [1.6.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.5.0...v1.6.0
 [1.5.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.4.0...v1.5.0
 [1.4.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.3.0...v1.4.0
 [1.3.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.2.0...v1.3.0
 [1.2.0]: https://github.com/Backblaze/b2-sdk-python/compare/v1.1.4...v1.2.0
```

### Comparing `b2sdk-1.8.0/CONTRIBUTING.md` & `b2sdk-1.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/LICENSE` & `b2sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/PKG-INFO` & `b2sdk-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Backblaze B2 SDK
 Home-page: https://github.com/Backblaze/b2-sdk-python
 Author: Backblaze, Inc.
 Author-email: support@backblaze.com
 License: MIT
-Description: # B2 Python SDK
-        &nbsp;[![Continuous Integration](https://github.com/Backblaze/b2-sdk-python/workflows/Continuous%20Integration/badge.svg)](https://github.com/Backblaze/b2-sdk-python/actions?query=workflow%3A%22Continuous+Integration%22)&nbsp;[![License](https://img.shields.io/pypi/l/b2sdk.svg?label=License)](https://pypi.python.org/pypi/b2)&nbsp;[![python versions](https://img.shields.io/pypi/pyversions/b2sdk.svg?label=python%20versions)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![PyPI version](https://img.shields.io/pypi/v/b2sdk.svg?label=PyPI%20version)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![Docs](https://readthedocs.org/projects/b2-sdk-python/badge/?version=master)](https://b2-sdk-python.readthedocs.io/en/master/)
-        
-        
-        
-        This repository contains a client library and a few handy utilities for easy access to all of the capabilities of B2 Cloud Storage.
-        
-        [B2 command-line tool](https://github.com/Backblaze/B2_Command_Line_Tool) is an example of how it can be used to provide command-line access to the B2 service, but there are many possible applications (including FUSE filesystems, storage backend drivers for backup applications etc).
-        
-        # Documentation
-        
-        The latest documentation is available on [Read the Docs](https://b2-sdk-python.readthedocs.io).
-        
-        # Installation
-        
-        The sdk can be installed with:
-        
-            pip install b2sdk
-        
-        # Version policy
-        
-        b2sdk follows [Semantic Versioning](https://semver.org/) policy, so in essence the version number is MAJOR.MINOR.PATCH (for example 1.2.3) and:
-        - we increase MAJOR version when we make incompatible API changes
-        - we increase MINOR version when we add functionality in a backwards-compatible manner, and
-        - we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
-        
-        Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
-        
-        ```
-        b2sdk>=0.0.0,<1.0.0
-        ```
-        
-        # Release History
-        
-        Please refer to the [changelog](CHANGELOG.md).
-        
-        # Developer Info
-        
-        Please see our [contributing guidelines](CONTRIBUTING.md).
-        
 Keywords: backblaze b2 cloud storage
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
+License-File: LICENSE
+
+# B2 Python SDK
+&nbsp;[![Continuous Integration](https://github.com/Backblaze/b2-sdk-python/workflows/Continuous%20Integration/badge.svg)](https://github.com/Backblaze/b2-sdk-python/actions?query=workflow%3A%22Continuous+Integration%22)&nbsp;[![License](https://img.shields.io/pypi/l/b2sdk.svg?label=License)](https://pypi.python.org/pypi/b2)&nbsp;[![python versions](https://img.shields.io/pypi/pyversions/b2sdk.svg?label=python%20versions)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![PyPI version](https://img.shields.io/pypi/v/b2sdk.svg?label=PyPI%20version)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![Docs](https://readthedocs.org/projects/b2-sdk-python/badge/?version=master)](https://b2-sdk-python.readthedocs.io/en/master/)
+
+
+
+This repository contains a client library and a few handy utilities for easy access to all of the capabilities of B2 Cloud Storage.
+
+[B2 command-line tool](https://github.com/Backblaze/B2_Command_Line_Tool) is an example of how it can be used to provide command-line access to the B2 service, but there are many possible applications (including FUSE filesystems, storage backend drivers for backup applications etc).
+
+# Documentation
+
+The latest documentation is available on [Read the Docs](https://b2-sdk-python.readthedocs.io).
+
+# Installation
+
+The sdk can be installed with:
+
+    pip install b2sdk
+
+# Version policy
+
+b2sdk follows [Semantic Versioning](https://semver.org/) policy, so in essence the version number is MAJOR.MINOR.PATCH (for example 1.2.3) and:
+- we increase MAJOR version when we make incompatible API changes
+- we increase MINOR version when we add functionality in a backwards-compatible manner, and
+- we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
+
+Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
+
+```
+b2sdk>=0.0.0,<1.0.0
+```
+
+# Release History
+
+Please refer to the [changelog](CHANGELOG.md).
+
+# Developer Info
+
+Please see our [contributing guidelines](CONTRIBUTING.md).
+
+
```

### Comparing `b2sdk-1.8.0/README.md` & `b2sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/README.release.md` & `b2sdk-1.9.0/README.release.md`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/__init__.py` & `b2sdk-1.9.0/b2sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/_pyinstaller/__init__.py` & `b2sdk-1.9.0/b2sdk/_pyinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/_v2/__init__.py` & `b2sdk-1.9.0/b2sdk/_v2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 )
 
 from b2sdk.utils import trace_call
 
 # data classes
 
 from b2sdk.file_version import FileIdAndName
-from b2sdk.file_version import FileVersionInfo
-from b2sdk.file_version import FileVersionInfoFactory
+from b2sdk.file_version import FileVersion
+from b2sdk.file_version import FileVersionFactory
 from b2sdk.large_file.part import Part
 from b2sdk.large_file.unfinished_large_file import UnfinishedLargeFile
 
 # file lock
 
 from b2sdk.file_lock import BucketRetentionSetting
 from b2sdk.file_lock import FileLockConfiguration
@@ -156,20 +156,19 @@
 from b2sdk.sync.action import B2DownloadAction
 from b2sdk.sync.action import B2HideAction
 from b2sdk.sync.action import B2UploadAction
 from b2sdk.sync.action import LocalDeleteAction
 from b2sdk.sync.exception import EnvironmentEncodingError
 from b2sdk.sync.exception import IncompleteSync
 from b2sdk.sync.exception import InvalidArgument
-from b2sdk.sync.file import File, B2File
-from b2sdk.sync.file import FileVersion, B2FileVersion
 from b2sdk.sync.folder import AbstractFolder
 from b2sdk.sync.folder import B2Folder
 from b2sdk.sync.folder import LocalFolder
 from b2sdk.sync.folder_parser import parse_sync_folder
+from b2sdk.sync.path import AbstractSyncPath, B2SyncPath, LocalSyncPath
 from b2sdk.sync.policy import AbstractFileSyncPolicy
 from b2sdk.sync.policy import CompareVersionMode
 from b2sdk.sync.policy import NewerFileSyncMode
 from b2sdk.sync.policy import DownAndDeletePolicy
 from b2sdk.sync.policy import DownAndKeepDaysPolicy
 from b2sdk.sync.policy import DownPolicy
 from b2sdk.sync.policy import CopyPolicy
```

### Comparing `b2sdk-1.8.0/b2sdk/_v2/exception.py` & `b2sdk-1.9.0/b2sdk/_v2/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/abstract.py` & `b2sdk-1.9.0/b2sdk/account_info/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/exception.py` & `b2sdk-1.9.0/b2sdk/account_info/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/in_memory.py` & `b2sdk-1.9.0/b2sdk/account_info/in_memory.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/sqlite_account_info.py` & `b2sdk-1.9.0/b2sdk/account_info/sqlite_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/stub.py` & `b2sdk-1.9.0/b2sdk/account_info/stub.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/test_upload_url_concurrency.py` & `b2sdk-1.9.0/b2sdk/account_info/test_upload_url_concurrency.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/account_info/upload_url_pool.py` & `b2sdk-1.9.0/b2sdk/account_info/upload_url_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/api.py` & `b2sdk-1.9.0/b2sdk/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from typing import Any, Dict, Optional
 
 from .bucket import Bucket, BucketFactory
 from .encryption.setting import EncryptionSetting
 from .exception import NonExistentBucket, RestrictedBucket
 from .file_lock import FileRetentionSetting, LegalHold
-from .file_version import FileIdAndName
+from .file_version import FileIdAndName, FileVersionFactory
 from .large_file.services import LargeFileServices
 from .raw_api import API_VERSION
 from .session import B2Session
 from .transfer import (
     CopyManager,
     DownloadManager,
     Emerger,
@@ -41,23 +41,24 @@
         base = info.get_api_url()
     return '%s/b2api/%s/%s' % (base, API_VERSION, api_name)
 
 
 class Services(object):
     """ Gathers objects that provide high level logic over raw api usage. """
 
-    def __init__(self, session, max_upload_workers=10, max_copy_workers=10):
+    def __init__(self, api, max_upload_workers=10, max_copy_workers=10):
         """
         Initialize Services object using given session.
 
-        :param b2sdk.v1.Session session:
+        :param b2sdk.v1.B2Api api:
         :param int max_upload_workers: a number of upload threads
         :param int max_copy_workers: a number of copy threads
         """
-        self.session = session
+        self.api = api
+        self.session = api.session
         self.large_file = LargeFileServices(self)
         self.download_manager = DownloadManager(self)
         self.upload_manager = UploadManager(self, max_upload_workers=max_upload_workers)
         self.copy_manager = CopyManager(self, max_copy_workers=max_copy_workers)
         self.emerger = Emerger(self)
 
 
@@ -80,14 +81,15 @@
 
     The class also keeps a cache of information needed to access the
     service, such as auth tokens and upload URLs.
     """
     BUCKET_FACTORY_CLASS = staticmethod(BucketFactory)
     BUCKET_CLASS = staticmethod(Bucket)
     SESSION_CLASS = staticmethod(B2Session)
+    FILE_VERSION_FACTORY_CLASS = staticmethod(FileVersionFactory)
 
     def __init__(
         self,
         account_info=None,
         cache=None,
         raw_api=None,
         max_upload_workers=10,
@@ -116,16 +118,17 @@
                         in tests and :class:`~b2sdk.raw_api.B2RawApi` in production.
                         default is :class:`~b2sdk.raw_api.B2RawApi`
 
         :param int max_upload_workers: a number of upload threads, default is 10
         :param int max_copy_workers: a number of copy threads, default is 10
         """
         self.session = self.SESSION_CLASS(account_info=account_info, cache=cache, raw_api=raw_api)
+        self.file_version_factory = self.FILE_VERSION_FACTORY_CLASS(self)
         self.services = Services(
-            self.session,
+            self,
             max_upload_workers=max_upload_workers,
             max_copy_workers=max_copy_workers,
         )
 
     @property
     def account_info(self):
         return self.session.account_info
@@ -390,36 +393,27 @@
         :rtype: generator
         """
         return self.services.large_file.list_parts(
             file_id, start_part_number=start_part_number, batch_size=batch_size
         )
 
     # delete/cancel
-    def cancel_large_file(self, file_id):
+    def cancel_large_file(self, file_id: str) -> FileIdAndName:
         """
         Cancel a large file upload.
-
-        :param str file_id: a file ID
-        :rtype: None
         """
         return self.services.large_file.cancel_large_file(file_id)
 
-    def delete_file_version(self, file_id, file_name):
+    def delete_file_version(self, file_id: str, file_name: str) -> FileIdAndName:
         """
         Permanently and irrevocably delete one version of a file.
-
-        :param str file_id: a file ID
-        :param str file_name: a file name
-        :rtype: FileIdAndName
         """
         # filename argument is not first, because one day it may become optional
         response = self.session.delete_file_version(file_id, file_name)
-        assert response['fileId'] == file_id
-        assert response['fileName'] == file_name
-        return FileIdAndName(file_id, file_name)
+        return FileIdAndName.from_cancel_or_delete_response(response)
 
     # download
     def get_download_url_for_fileid(self, file_id):
         """
         Return a URL to download the given file by ID.
 
         :param str file_id: a file ID
@@ -430,15 +424,15 @@
     def get_download_url_for_file_name(self, bucket_name, file_name):
         """
         Return a URL to download the given file by name.
 
         :param str bucket_name: a bucket name
         :param str file_name: a file name
         """
-        self.check_bucket_restrictions(bucket_name)
+        self.check_bucket_name_restrictions(bucket_name)
         return '%s/file/%s/%s' % (
             self.account_info.get_download_url(), bucket_name, b2_url_encode(file_name)
         )
 
     # keys
     def create_key(
         self,
```

### Comparing `b2sdk-1.8.0/b2sdk/b2http.py` & `b2sdk-1.9.0/b2sdk/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/bounded_queue_executor.py` & `b2sdk-1.9.0/b2sdk/bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/bucket.py` & `b2sdk-1.9.0/b2sdk/bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from .file_lock import (
     BucketRetentionSetting,
     FileLockConfiguration,
     FileRetentionSetting,
     UNKNOWN_BUCKET_RETENTION,
     LegalHold,
 )
-from .file_version import FileVersionInfo, FileVersionInfoFactory
+from .file_version import FileVersion
 from .progress import DoNothingProgressListener
 from .transfer.emerge.executor import AUTO_CONTENT_TYPE
 from .transfer.emerge.write_intent import WriteIntent
 from .transfer.outbound.copy_source import CopySource
 from .transfer.outbound.upload_source import UploadSourceBytes, UploadSourceLocalFile
 from .utils import B2TraceMeta, disable_trace, limit_trace_arguments
 from .utils import b2_url_encode, validate_b2_file_name
@@ -35,15 +35,14 @@
 
 class Bucket(metaclass=B2TraceMeta):
     """
     Provide access to a bucket in B2: listing files, uploading and downloading.
     """
 
     DEFAULT_CONTENT_TYPE = AUTO_CONTENT_TYPE
-    FILE_VERSION_FACTORY = staticmethod(FileVersionInfoFactory)
 
     def __init__(
         self,
         api,
         id_,
         name=None,
         type_=None,
@@ -220,32 +219,32 @@
             url,
             download_dest,
             progress_listener,
             range_,
             encryption=encryption,
         )
 
-    def get_file_info_by_id(self, file_id: str) -> FileVersionInfo:
+    def get_file_info_by_id(self, file_id: str) -> FileVersion:
         """
-        Gets a file version's info by ID.
+        Gets a file version's by ID.
 
         :param str file_id: the id of the file who's info will be retrieved.
         :rtype: generator[b2sdk.v1.FileVersionInfo]
         """
-        return self.FILE_VERSION_FACTORY.from_api_response(self.api.get_file_info(file_id))
+        return self.api.file_version_factory.from_api_response(self.api.get_file_info(file_id))
 
-    def get_file_info_by_name(self, file_name: str) -> FileVersionInfo:
+    def get_file_info_by_name(self, file_name: str) -> FileVersion:
         """
-        Gets a file version's info by its name.
+        Gets a file version's by its name.
 
         :param str file_name: the name of the file who's info will be retrieved.
         :rtype: generator[b2sdk.v1.FileVersionInfo]
         """
         try:
-            return self.FILE_VERSION_FACTORY.from_response_headers(
+            return self.api.file_version_factory.from_response_headers(
                 self.api.session.get_file_info_by_name(self.name, file_name)
             )
         except FileOrBucketNotFound:
             raise FileNotPresent(bucket_name=self.name, file_id_or_name=file_name)
 
     def get_download_authorization(self, file_name_prefix, valid_duration_in_seconds):
         """
@@ -286,19 +285,19 @@
         session = self.api.session
         while 1:
             response = session.list_file_versions(
                 self.id_, start_file_name, start_file_id, fetch_count, file_name
             )
 
             for entry in response['files']:
-                file_version_info = self.FILE_VERSION_FACTORY.from_api_response(entry)
-                if file_version_info.file_name != file_name:
+                file_version = self.api.file_version_factory.from_api_response(entry)
+                if file_version.file_name != file_name:
                     # All versions for the requested file name have been listed.
                     return
-                yield file_version_info
+                yield file_version
             start_file_name = response['nextFileName']
             start_file_id = response['nextFileId']
             if start_file_name is None:
                 return
 
     def ls(self, folder_to_list='', show_versions=False, recursive=False, fetch_count=10000):
         """
@@ -315,15 +314,15 @@
         :param str folder_to_list: the name of the folder to list; must not start with "/".
                                Empty string means top-level folder
         :param bool show_versions: when ``True`` returns info about all versions of a file,
                               when ``False``, just returns info about the most recent versions
         :param bool recursive: if ``True``, list folders recursively
         :param int,None fetch_count: how many entries to return or ``None`` to use the default. Acceptable values: 1 - 10000
         :rtype: generator[tuple[b2sdk.v1.FileVersionInfo, str]]
-        :returns: generator of (file_version_info, folder_name) tuples
+        :returns: generator of (file_version, folder_name) tuples
 
         .. note::
             In case of `recursive=True`, folder_name is returned only for first file in the folder.
         """
         # Every file returned must have a name that starts with the
         # folder name and a "/".
         prefix = folder_to_list
@@ -346,33 +345,33 @@
             if show_versions:
                 response = session.list_file_versions(
                     self.id_, start_file_name, start_file_id, fetch_count, prefix
                 )
             else:
                 response = session.list_file_names(self.id_, start_file_name, fetch_count, prefix)
             for entry in response['files']:
-                file_version_info = self.FILE_VERSION_FACTORY.from_api_response(entry)
-                if not file_version_info.file_name.startswith(prefix):
+                file_version = self.api.file_version_factory.from_api_response(entry)
+                if not file_version.file_name.startswith(prefix):
                     # We're past the files we care about
                     return
-                after_prefix = file_version_info.file_name[len(prefix):]
+                after_prefix = file_version.file_name[len(prefix):]
                 if '/' not in after_prefix or recursive:
                     # This is not a folder, so we'll print it out and
                     # continue on.
-                    yield file_version_info, None
+                    yield file_version, None
                     current_dir = None
                 else:
                     # This is a folder.  If it's different than the folder
                     # we're already in, then we can print it.  This check
                     # is needed, because all of the files in the folder
                     # will be in the list.
                     folder_with_slash = after_prefix.split('/')[0] + '/'
                     if folder_with_slash != current_dir:
                         folder_name = prefix + folder_with_slash
-                        yield file_version_info, folder_name
+                        yield file_version, folder_name
                         current_dir = folder_with_slash
             if response['nextFileName'] is None:
                 # The response says there are no more files in the bucket,
                 # so we can stop.
                 return
 
             # Now we need to set up the next search.  The response from
@@ -784,15 +783,15 @@
         """
         Hide a file.
 
         :param str file_name: a file name
         :rtype: b2sdk.v1.FileVersionInfo
         """
         response = self.api.session.hide_file(self.id_, file_name)
-        return self.FILE_VERSION_FACTORY.from_api_response(response)
+        return self.api.file_version_factory.from_api_response(response)
 
     def copy(
         self,
         file_id,
         new_file_name,
         content_type=None,
         file_info=None,
@@ -944,20 +943,20 @@
                    "isClientAuthorizedToRead" : true,
                    "value": {
                      "algorithm" : "AES256",
                      "mode" : "SSE-B2"
                    }
                },
                "fileLockConfiguration": {
-                   "isClientAuthorizedToRead": true, 
+                   "isClientAuthorizedToRead": true,
                    "value": {
                        "defaultRetention": {
                            "mode": null,
                            "period": null
-                        }, 
+                        },
                         "isFileLockEnabled": false
                     }
               }
            }
 
         into a Bucket object.
```

### Comparing `b2sdk-1.8.0/b2sdk/cache.py` & `b2sdk-1.9.0/b2sdk/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/download_dest.py` & `b2sdk-1.9.0/b2sdk/download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/encryption/setting.py` & `b2sdk-1.9.0/b2sdk/encryption/setting.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     # if authorized to read:
     #    "mode": "none"
     #    or
     #    "mode": "SSE-B2"
     # if not authorized to read:
     #    isClientAuthorizedToRead is False and there is no value, so no mode
     #
-    # BUT file_version_info (get_file_info, list_file_versions, upload_file etc)
+    # BUT file_version (get_file_info, list_file_versions, upload_file etc)
     # if the file is encrypted, then
     #     "serverSideEncryption": {"algorithm": "AES256", "mode": "SSE-B2"},
     #     or
     #     "serverSideEncryption": {"algorithm": "AES256", "mode": "SSE-C"},
     # if the file is not encrypted, then "serverSideEncryption" is not present at all
     @classmethod
     def from_file_version_dict(cls, file_version_dict: dict) -> EncryptionSetting:
```

### Comparing `b2sdk-1.8.0/b2sdk/encryption/types.py` & `b2sdk-1.9.0/b2sdk/encryption/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/exception.py` & `b2sdk-1.9.0/b2sdk/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,29 +195,29 @@
 class B2RequestTimeoutDuringUpload(B2RequestTimeout):
     # if a timeout is hit during upload, it is not guaranteed that the the server has released the upload token lock already, so we'll use a new token
     def should_retry_http(self):
         return False
 
 
 class DestFileNewer(B2Error):
-    def __init__(self, dest_file, source_file, dest_prefix, source_prefix):
+    def __init__(self, dest_path, source_path, dest_prefix, source_prefix):
         super(DestFileNewer, self).__init__()
-        self.dest_file = dest_file
-        self.source_file = source_file
+        self.dest_path = dest_path
+        self.source_path = source_path
         self.dest_prefix = dest_prefix
         self.source_prefix = source_prefix
 
     def __str__(self):
         return 'source file is older than destination: %s%s with a time of %s cannot be synced to %s%s with a time of %s, unless a valid newer_file_mode is provided' % (
             self.source_prefix,
-            self.source_file.name,
-            self.source_file.latest_version().mod_time,
+            self.source_path.relative_path,
+            self.source_path.mod_time,
             self.dest_prefix,
-            self.dest_file.name,
-            self.dest_file.latest_version().mod_time,
+            self.dest_path.relative_path,
+            self.dest_path.mod_time,
         )
 
     def should_retry_http(self):
         return True
 
 
 class DuplicateBucketName(B2SimpleError):
```

### Comparing `b2sdk-1.8.0/b2sdk/file_lock.py` & `b2sdk-1.9.0/b2sdk/file_lock.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/file_version.py` & `b2sdk-1.9.0/b2sdk/file_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
-from typing import Optional
-
 from .encryption.setting import EncryptionSetting, EncryptionSettingFactory
-from .file_lock import FileRetentionSetting, LegalHold
+from .file_lock import FileRetentionSetting, LegalHold, NO_RETENTION_FILE_SETTING
+from .raw_api import SRC_LAST_MODIFIED_MILLIS
+if False:
+    from .api import B2Api
 
 
-class FileVersionInfo(object):
+class FileVersion:
     """
     A structure which represents a version of a file (in B2 cloud).
 
     :ivar str ~.id\_: ``fileId``
     :ivar str ~.file_name: full file name (with path)
     :ivar ~.size: size in bytes, can be ``None`` (unknown)
     :vartype ~.size: int or None
@@ -31,100 +32,112 @@
     :ivar ~.upload_timestamp: in milliseconds since :abbr:`epoch (1970-01-01 00:00:00)`. Can be ``None`` (unknown).
     :vartype ~.upload_timestamp: int or None
     :ivar str ~.action: ``"upload"``, ``"hide"`` or ``"delete"``
     """
 
     __slots__ = [
         'id_',
+        'api',
         'file_name',
         'size',
         'content_type',
         'content_sha1',
         'content_md5',
         'file_info',
         'upload_timestamp',
         'action',
         'server_side_encryption',
         'legal_hold',
         'file_retention',
+        'mod_time_millis',
     ]
 
     def __init__(
         self,
+        api: 'B2Api',
         id_,
         file_name,
         size,
         content_type,
         content_sha1,
         file_info,
         upload_timestamp,
         action,
-        content_md5=None,
-        server_side_encryption: Optional[EncryptionSetting] = None,  # TODO: make it mandatory in v2
-        file_retention: Optional[
-            FileRetentionSetting
-        ] = None,  # TODO: in v2 change the default value to NO_RETENTION_FILE_SETTING
-        legal_hold: Optional[LegalHold
-                            ] = None,  # TODO: in v2 change the default value to LegalHold.UNSET
+        content_md5,
+        server_side_encryption: EncryptionSetting,
+        file_retention: FileRetentionSetting = NO_RETENTION_FILE_SETTING,
+        legal_hold: LegalHold = LegalHold.UNSET,
     ):
+        self.api = api
         self.id_ = id_
         self.file_name = file_name
         self.size = size
         self.content_type = content_type
         self.content_sha1 = content_sha1
         self.content_md5 = content_md5
         self.file_info = file_info or {}
         self.upload_timestamp = upload_timestamp
         self.action = action
         self.server_side_encryption = server_side_encryption
         self.legal_hold = legal_hold
         self.file_retention = file_retention
 
+        if SRC_LAST_MODIFIED_MILLIS in self.file_info:
+            self.mod_time_millis = int(self.file_info[SRC_LAST_MODIFIED_MILLIS])
+        else:
+            self.mod_time_millis = self.upload_timestamp
+
     def as_dict(self):
         """ represents the object as a dict which looks almost exactly like the raw api output for upload/list """
         result = {
             'fileId': self.id_,
             'fileName': self.file_name,
             'fileInfo': self.file_info,
             'legalHold': self.legal_hold.to_dict_repr() if self.legal_hold is not None else None,
+            'serverSideEncryption': self.server_side_encryption.as_dict(),
+            'fileRetention': self.file_retention.as_dict(),
         }
 
         if self.size is not None:
             result['size'] = self.size
         if self.upload_timestamp is not None:
             result['uploadTimestamp'] = self.upload_timestamp
         if self.action is not None:
             result['action'] = self.action
         if self.content_type is not None:
             result['contentType'] = self.content_type
         if self.content_sha1 is not None:
             result['contentSha1'] = self.content_sha1
         if self.content_md5 is not None:
             result['contentMd5'] = self.content_md5
-        if self.server_side_encryption is not None:  # this is for backward compatibility of interface only, b2sdk always sets it
-            result['serverSideEncryption'] = self.server_side_encryption.as_dict()
-        if self.file_retention is not None:  # this is for backward compatibility of interface only, b2sdk always sets it
-            result['fileRetention'] = self.file_retention.as_dict()
         return result
 
     def __eq__(self, other):
         sentry = object()
         for attr in self.__slots__:
             if getattr(self, attr) != getattr(other, attr, sentry):
                 return False
         return True
 
+    def __repr__(self):
+        return '%s(%s)' % (
+            self.__class__.__name__,
+            ', '.join(repr(getattr(self, attr)) for attr in self.__slots__)
+        )
+
 
-class FileVersionInfoFactory(object):
+class FileVersionFactory(object):
     """
     Construct :py:class:`b2sdk.v1.FileVersionInfo` objects from various structures.
     """
 
-    @classmethod
-    def from_api_response(cls, file_info_dict, force_action=None):
+    def __init__(self, api: 'B2Api'):
+        self.api = api
+
+    def from_api_response(self, file_version_dict, force_action=None):
         """
         Turn this:
 
         .. code-block:: python
 
            {
                "action": "hide",
@@ -149,90 +162,86 @@
                "fileName": "randomdata",
                "serverSideEncryption": {"algorithm": "AES256", "mode": "SSE-B2"}
            }
 
         into a :py:class:`b2sdk.v1.FileVersionInfo` object.
 
         """
-        assert file_info_dict.get('action') is None or force_action is None, \
+        assert file_version_dict.get('action') is None or force_action is None, \
             'action was provided by both info_dict and function argument'
-        action = file_info_dict.get('action') or force_action
-        file_name = file_info_dict['fileName']
-        id_ = file_info_dict['fileId']
-        if 'size' in file_info_dict:
-            size = file_info_dict['size']
-        elif 'contentLength' in file_info_dict:
-            size = file_info_dict['contentLength']
+        action = file_version_dict.get('action') or force_action
+        file_name = file_version_dict['fileName']
+        id_ = file_version_dict['fileId']
+        if 'size' in file_version_dict:
+            size = file_version_dict['size']
+        elif 'contentLength' in file_version_dict:
+            size = file_version_dict['contentLength']
         else:
             raise ValueError('no size or contentLength')
-        upload_timestamp = file_info_dict.get('uploadTimestamp')
-        content_type = file_info_dict.get('contentType')
-        content_sha1 = file_info_dict.get('contentSha1')
-        content_md5 = file_info_dict.get('contentMd5')
-        file_info = file_info_dict.get('fileInfo')
-        server_side_encryption = EncryptionSettingFactory.from_file_version_dict(file_info_dict)
-        file_retention = FileRetentionSetting.from_file_version_dict(file_info_dict)
+        upload_timestamp = file_version_dict.get('uploadTimestamp')
+        content_type = file_version_dict.get('contentType')
+        content_sha1 = file_version_dict.get('contentSha1')
+        content_md5 = file_version_dict.get('contentMd5')
+        file_info = file_version_dict.get('fileInfo')
+        server_side_encryption = EncryptionSettingFactory.from_file_version_dict(file_version_dict)
+        file_retention = FileRetentionSetting.from_file_version_dict(file_version_dict)
 
-        legal_hold = LegalHold.from_file_version_dict(file_info_dict)
+        legal_hold = LegalHold.from_file_version_dict(file_version_dict)
 
-        return FileVersionInfo(
+        return FileVersion(
+            self.api,
             id_,
             file_name,
             size,
             content_type,
             content_sha1,
             file_info,
             upload_timestamp,
             action,
             content_md5,
             server_side_encryption,
             file_retention,
             legal_hold,
         )
 
-    @classmethod
-    def from_cancel_large_file_response(cls, response):
-        return FileVersionInfo(
-            response['fileId'],
-            response['fileName'],
-            0,  # size
-            'unknown',
-            'none',
-            {},
-            0,  # upload timestamp
-            'cancel'
-        )
-
-    @classmethod
-    def from_response_headers(cls, headers):
-        return FileVersionInfo(
+    def from_response_headers(self, headers):
+        return FileVersion(
+            api=self.api,
             id_=headers.get('x-bz-file-id'),
             file_name=headers.get('x-bz-file-name'),
             size=headers.get('content-length'),
             content_type=headers.get('content-type'),
             content_sha1=headers.get('x-bz-content-sha1'),
             file_info=None,
             upload_timestamp=headers.get('x-bz-upload-timestamp'),
             action=None,
+            content_md5=None,
             server_side_encryption=EncryptionSettingFactory.from_response_headers(headers),
             file_retention=FileRetentionSetting.from_response_headers(headers),
             legal_hold=LegalHold.from_response_headers(headers),
         )
 
 
 class FileIdAndName(object):
     """
     A structure which represents a B2 cloud file with just `file_name` and `fileId` attributes.
 
-    Used to return data from calls to :py:meth:`b2sdk.v1.Bucket.delete_file_version`.
-
-    :ivar str ~.file_id: ``fileId``
-    :ivar str ~.file_name: full file name (with path)
+    Used to return data from calls to b2_delete_file_version and b2_cancel_large_file.
     """
 
-    def __init__(self, file_id, file_name):
+    def __init__(self, file_id: str, file_name: str):
         self.file_id = file_id
         self.file_name = file_name
 
+    @classmethod
+    def from_cancel_or_delete_response(cls, response):
+        return cls(response['fileId'], response['fileName'])
+
     def as_dict(self):
         """ represents the object as a dict which looks almost exactly like the raw api output for delete_file_version """
         return {'action': 'delete', 'fileId': self.file_id, 'fileName': self.file_name}
+
+    def __eq__(self, other):
+        return (self.file_id == other.file_id and self.file_name == other.file_name)
+
+    def __repr__(self):
+        return '%s(%s, %s)' % (self.__class__.__name__, repr(self.file_id), repr(self.file_name))
```

### Comparing `b2sdk-1.8.0/b2sdk/large_file/part.py` & `b2sdk-1.9.0/b2sdk/large_file/part.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/large_file/services.py` & `b2sdk-1.9.0/b2sdk/large_file/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 ######################################################################
 
 from typing import Optional
 
 from b2sdk.encryption.setting import EncryptionSetting
 from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.file_version import FileVersionInfoFactory
+from b2sdk.file_version import FileIdAndName
 from b2sdk.large_file.part import PartFactory
 from b2sdk.large_file.unfinished_large_file import UnfinishedLargeFile
 
 
 class LargeFileServices(object):
     def __init__(self, services):
         self.services = services
@@ -91,15 +91,15 @@
         """
         Start a large file transfer.
 
         :param str file_name: a file name
         :param str,None content_type: the MIME type, or ``None`` to accept the default based on file extension of the B2 file name
         :param dict,None file_info: a file info to store with the file or ``None`` to not store anything
         :param b2sdk.v1.EncryptionSetting encryption: encryption settings (``None`` if unknown)
-        :param bool legal_hold: legal hold setting
+        :param b2sdk.v1.LegalHold legal_hold: legal hold setting
         :param b2sdk.v1.FileRetentionSetting file_retention: file retention setting
         """
         return UnfinishedLargeFile(
             self.services.session.start_large_file(
                 bucket_id,
                 file_name,
                 content_type,
@@ -107,16 +107,13 @@
                 server_side_encryption=encryption,
                 file_retention=file_retention,
                 legal_hold=legal_hold,
             )
         )
 
     # delete/cancel
-    def cancel_large_file(self, file_id):
+    def cancel_large_file(self, file_id: str) -> FileIdAndName:
         """
         Cancel a large file upload.
-
-        :param str file_id: a file ID
-        :rtype: None
         """
         response = self.services.session.cancel_large_file(file_id)
-        return FileVersionInfoFactory.from_cancel_large_file_response(response)
+        return FileIdAndName.from_cancel_or_delete_response(response)
```

### Comparing `b2sdk-1.8.0/b2sdk/large_file/unfinished_large_file.py` & `b2sdk-1.9.0/b2sdk/large_file/unfinished_large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/progress.py` & `b2sdk-1.9.0/b2sdk/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/raw_api.py` & `b2sdk-1.9.0/b2sdk/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/raw_simulator.py` & `b2sdk-1.9.0/b2sdk/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/session.py` & `b2sdk-1.9.0/b2sdk/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/__init__.py` & `b2sdk-1.9.0/b2sdk/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/chained.py` & `b2sdk-1.9.0/b2sdk/stream/chained.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/hashing.py` & `b2sdk-1.9.0/b2sdk/stream/hashing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/progress.py` & `b2sdk-1.9.0/b2sdk/stream/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/range.py` & `b2sdk-1.9.0/b2sdk/stream/range.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/stream/wrapper.py` & `b2sdk-1.9.0/b2sdk/stream/wrapper.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/sync/action.py` & `b2sdk-1.9.0/b2sdk/sync/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 from ..download_dest import DownloadDestLocalFile
 from .encryption_provider import AbstractSyncEncryptionSettingsProvider
 from ..bucket import Bucket
 
 from ..raw_api import SRC_LAST_MODIFIED_MILLIS
 from ..transfer.outbound.upload_source import UploadSourceLocalFile
-from .file import B2File
+from .path import B2SyncPath
 from .report import SyncFileReporter
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractAction(metaclass=ABCMeta):
     """
@@ -206,37 +206,37 @@
     def __str__(self):
         return 'b2_hide(%s)' % (self.b2_file_name,)
 
 
 class B2DownloadAction(AbstractAction):
     def __init__(
         self,
-        source_file: B2File,
+        source_path: B2SyncPath,
         b2_file_name: str,
         local_full_path: str,
         encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
     ):
         """
-        :param b2sdk.v1.B2File source_file: the file to be downloaded
+        :param b2sdk.v1.B2SyncPath source_path: the file to be downloaded
         :param str b2_file_name: b2_file_name
         :param str local_full_path: a local file path
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
         """
-        self.source_file = source_file
+        self.source_path = source_path
         self.b2_file_name = b2_file_name
         self.local_full_path = local_full_path
         self.encryption_settings_provider = encryption_settings_provider
 
     def get_bytes(self):
         """
         Return file size.
 
         :rtype: int
         """
-        return self.source_file.latest_version().size
+        return self.source_path.size
 
     def _ensure_directory_existence(self):
         parent_dir = os.path.dirname(self.local_full_path)
         if not os.path.isdir(parent_dir):
             try:
                 os.makedirs(parent_dir)
             except OSError:
@@ -260,19 +260,19 @@
 
         # Download the file to a .tmp file
         download_path = self.local_full_path + '.b2.sync.tmp'
         download_dest = DownloadDestLocalFile(download_path)
 
         encryption = self.encryption_settings_provider.get_setting_for_download(
             bucket=bucket,
-            file_version_info=self.source_file.latest_version().file_version_info,
+            file_version=self.source_path.selected_version,
         )
 
         bucket.download_file_by_id(
-            self.source_file.latest_version().id_,
+            self.source_path.selected_version.id_,
             download_dest,
             progress_listener,
             encryption=encryption,
         )
 
         # Move the file into place
         try:
@@ -285,61 +285,61 @@
         """
         Report the downloading action performed.
 
         :param bucket: a Bucket object
         :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
-        reporter.print_completion('dnload ' + self.source_file.name)
+        reporter.print_completion('dnload ' + self.source_path.relative_path)
 
     def __str__(self):
         return (
             'b2_download(%s, %s, %s, %d)' % (
-                self.b2_file_name, self.source_file.latest_version().id_, self.local_full_path,
-                self.source_file.latest_version().mod_time
+                self.b2_file_name, self.source_path.selected_version.id_, self.local_full_path,
+                self.source_path.mod_time
             )
         )
 
 
 class B2CopyAction(AbstractAction):
     """
     File copying action.
     """
 
     def __init__(
         self,
         b2_file_name: str,
-        source_file: B2File,
+        source_path: B2SyncPath,
         dest_b2_file_name,
         source_bucket: Bucket,
         destination_bucket: Bucket,
         encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
     ):
         """
         :param str b2_file_name: a b2_file_name
-        :param b2sdk.v1.B2File source_file: the file to be copied
+        :param b2sdk.v1.B2SyncPath source_path: the file to be copied
         :param str dest_b2_file_name: a name of a destination remote file
         :param Bucket source_bucket: bucket to copy from
         :param Bucket destination_bucket: bucket to copy to
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
         """
         self.b2_file_name = b2_file_name
-        self.source_file = source_file
+        self.source_path = source_path
         self.dest_b2_file_name = dest_b2_file_name
         self.encryption_settings_provider = encryption_settings_provider
         self.source_bucket = source_bucket
         self.destination_bucket = destination_bucket
 
     def get_bytes(self):
         """
         Return file size.
 
         :rtype: int
         """
-        return self.source_file.latest_version().size
+        return self.source_path.size
 
     def do_action(self, bucket, reporter):
         """
         Perform the copying action, returning only after the action is completed.
 
         :param bucket: a Bucket object
         :type bucket: b2sdk.bucket.Bucket
@@ -348,49 +348,49 @@
         if reporter:
             progress_listener = SyncFileReporter(reporter)
         else:
             progress_listener = None
 
         source_encryption = self.encryption_settings_provider.get_source_setting_for_copy(
             bucket=self.source_bucket,
-            source_file_version_info=self.source_file.latest_version().file_version_info,
+            source_file_version=self.source_path.selected_version,
         )
 
         destination_encryption = self.encryption_settings_provider.get_destination_setting_for_copy(
             bucket=self.destination_bucket,
-            source_file_version_info=self.source_file.latest_version().file_version_info,
+            source_file_version=self.source_path.selected_version,
             dest_b2_file_name=self.dest_b2_file_name,
         )
 
         bucket.copy(
-            self.source_file.latest_version().id_,
+            self.source_path.selected_version.id_,
             self.dest_b2_file_name,
-            length=self.source_file.latest_version().size,
+            length=self.source_path.size,
             progress_listener=progress_listener,
             destination_encryption=destination_encryption,
             source_encryption=source_encryption,
-            source_file_info=self.source_file.latest_version().file_version_info.file_info,
-            source_content_type=self.source_file.latest_version().file_version_info.content_type,
+            source_file_info=self.source_path.selected_version.file_info,
+            source_content_type=self.source_path.selected_version.content_type,
         )
 
     def do_report(self, bucket, reporter):
         """
         Report the copying action performed.
 
         :param bucket: a Bucket object
         :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
-        reporter.print_completion('copy ' + self.source_file.name)
+        reporter.print_completion('copy ' + self.source_path.relative_path)
 
     def __str__(self):
         return (
             'b2_copy(%s, %s, %s, %d)' % (
-                self.b2_file_name, self.source_file.latest_version().id_, self.dest_b2_file_name,
-                self.source_file.latest_version().mod_time
+                self.b2_file_name, self.source_path.selected_version.id_, self.dest_b2_file_name,
+                self.source_path.mod_time
             )
         )
 
 
 class B2DeleteAction(AbstractAction):
     def __init__(self, relative_name, b2_file_name, file_id, note):
         """
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/encryption_provider.py` & `b2sdk-1.9.0/b2sdk/sync/encryption_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ######################################################################
 
 from abc import ABCMeta, abstractmethod
 from typing import Dict, Optional
 
 from ..encryption.setting import EncryptionSetting
 from ..bucket import Bucket
-from ..file_version import FileVersionInfo
+from ..file_version import FileVersion
 
 
 class AbstractSyncEncryptionSettingsProvider(metaclass=ABCMeta):
     """
     Object which provides an appropriate EncryptionSetting object
     for sync, i.e. complex operations with multiple sources and destinations
     """
@@ -34,37 +34,37 @@
         Return an EncryptionSetting for uploading an object or None if server should decide.
         """
 
     @abstractmethod
     def get_source_setting_for_copy(
         self,
         bucket: Bucket,
-        source_file_version_info: FileVersionInfo,
+        source_file_version: FileVersion,
     ) -> Optional[EncryptionSetting]:
         """
         Return an EncryptionSetting for a source of copying an object or None if not required
         """
 
     @abstractmethod
     def get_destination_setting_for_copy(
         self,
         bucket: Bucket,
         dest_b2_file_name: str,
-        source_file_version_info: FileVersionInfo,
+        source_file_version: FileVersion,
         target_file_info: Optional[dict] = None,
     ) -> Optional[EncryptionSetting]:
         """
         Return an EncryptionSetting for a destination for copying an object or None if server should decide
         """
 
     @abstractmethod
     def get_setting_for_download(
         self,
         bucket: Bucket,
-        file_version_info: FileVersionInfo,
+        file_version: FileVersion,
     ) -> Optional[EncryptionSetting]:
         """
         Return an EncryptionSetting for downloading an object from, or None if not required
         """
 
 
 class ServerDefaultSyncEncryptionSettingsProvider(AbstractSyncEncryptionSettingsProvider):
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/exception.py` & `b2sdk-1.9.0/b2sdk/sync/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/sync/file.py` & `b2sdk-1.9.0/b2sdk/v1/sync/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 ######################################################################
 #
-# File: b2sdk/sync/file.py
+# File: b2sdk/v1/sync/file.py
 #
-# Copyright 2019 Backblaze Inc. All Rights Reserved.
+# Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 from typing import List
 
-from ..file_version import FileVersionInfo
-from ..raw_api import SRC_LAST_MODIFIED_MILLIS
+from b2sdk.v1 import FileVersionInfo
+from b2sdk.raw_api import SRC_LAST_MODIFIED_MILLIS
 
 
+# This whole module is here to retain legacy classes so they can be used in retained legacy exception
 class File(object):
     """
     Hold information about one file in a folder.
 
     The name is relative to the folder in all cases.
 
     Files that have multiple versions (which only happens
@@ -50,22 +51,22 @@
 class B2File(File):
     """
     Hold information about one file in a folder in B2 cloud.
     """
 
     __slots__ = ['name', 'versions']
 
-    def __init__(self, name, versions: List['B2FileVersion']):
+    def __init__(self, name, versions: List['FileVersion']):
         """
         :param str name: a relative file name
-        :param List[B2FileVersion] versions: a list of file versions
+        :param List[FileVersion] versions: a list of file versions
         """
         super().__init__(name, versions)
 
-    def latest_version(self) -> 'B2FileVersion':
+    def latest_version(self) -> 'FileVersion':
         return super().latest_version()
 
 
 class FileVersion(object):
     """
     Hold information about one version of a file.
     """
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/folder.py` & `b2sdk-1.9.0/b2sdk/sync/folder.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 import os
 import platform
 import re
 import sys
 
 from abc import ABCMeta, abstractmethod
 from .exception import EmptyDirectory, EnvironmentEncodingError, UnSyncableFilename, NotADirectory, UnableToCreateDirectory
-from .file import File, B2File, FileVersion, B2FileVersion
-from .scan_policies import DEFAULT_SCAN_MANAGER
+from .path import B2SyncPath, LocalSyncPath
+from .report import SyncReport
+from .scan_policies import DEFAULT_SCAN_MANAGER, ScanPoliciesManager
 from ..utils import fix_windows_path_limit, get_file_mtime, is_file_readable
 
 DRIVE_MATCHER = re.compile(r"^([A-Za-z]):([/\\])")
 ABSOLUTE_PATH_MATCHER = re.compile(r"^(/)|^(\\)")
 RELATIVE_PATH_MATCHER = re.compile(
                            # "abc" and "xyz" represent anything, including "nothing"
     r"^(\.\.[/\\])|" +     # ../abc or ..\abc
     r"^(\.[/\\])|" +       # ./abc or .\abc
     r"([/\\]\.\.[/\\])|" + # abc/../xyz or abc\..\xyz or abc\../xyz or abc/..\xyz
     r"([/\\]\.[/\\])|" +   # abc/./xyz or abc\.\xyz or abc\./xyz or abc/.\xyz
     r"([/\\]\.\.)$|" +     # abc/.. or abc\..
-    r"([/\\]\.)$|" +       # abc/. or abc\. 
+    r"([/\\]\.)$|" +       # abc/. or abc\.
     r"^(\.\.)$|" +         # just ".."
     r"([/\\][/\\])|" +     # abc\/xyz or abc/\xyz or abc//xyz or abc\\xyz
     r"^(\.)$"              # just "."
 )  # yapf: disable
 
 logger = logging.getLogger(__name__)
 
@@ -82,27 +83,22 @@
 
         :param file_name: a file name
         :type file_name: str
         :rtype: str
         """
 
 
-def join_b2_path(b2_dir, b2_name):
+def join_b2_path(relative_dir_path: str, file_name: str):
     """
     Like os.path.join, but for B2 file names where the root directory is called ''.
-
-    :param b2_dir: a directory path
-    :type b2_dir: str
-    :param b2_name: a file name
-    :type b2_name: str
     """
-    if b2_dir == '':
-        return b2_name
+    if relative_dir_path == '':
+        return file_name
     else:
-        return b2_dir + '/' + b2_name
+        return relative_dir_path + '/' + file_name
 
 
 class LocalFolder(AbstractFolder):
     """
     Folder interface to a directory on the local machine.
     """
 
@@ -128,16 +124,15 @@
     def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
         """
         Yield all files.
 
         :param reporter: a place to report errors
         :param policies_manager: a policy manager object, default is DEFAULT_SCAN_MANAGER
         """
-        for file_object in self._walk_relative_paths(self.root, '', reporter, policies_manager):
-            yield file_object
+        yield from self._walk_relative_paths(self.root, '', reporter, policies_manager)
 
     def make_full_path(self, file_name):
         """
         Convert a file name into an absolute path, ensure it is not outside self.root
 
         :param file_name: a file name
         :type file_name: str
@@ -174,25 +169,23 @@
         Make sure that the directory exists and is non-empty.
         """
         self.ensure_present()
 
         if not os.listdir(self.root):
             raise EmptyDirectory(self.root)
 
-    @classmethod
-    def _walk_relative_paths(cls, local_dir, b2_dir, reporter, policies_manager):
+    def _walk_relative_paths(
+        self, local_dir: str, relative_dir_path: str, reporter: SyncReport,
+        policies_manager: ScanPoliciesManager
+    ):
         """
         Yield a File object for each of the files anywhere under this folder, in the
         order they would appear in B2, unless the path is excluded by policies manager.
 
-        :param local_dir: the local directory to list files in
-        :param b2_dir: the B2 path of this directory, or '' if at the root
-        :param reporter: a place to report errors
-        :param policies_manager: a manager for polices scan results
-        :return:
+        :param relative_dir_path: the path of this dir relative to the sync point, or '' if at sync point
         """
         if not isinstance(local_dir, str):
             raise ValueError('folder path should be unicode: %s' % repr(local_dir))
 
         # Collect the names.  We do this before returning any results, because
         # directories need to sort as if their names end in '/'.
         #
@@ -202,72 +195,77 @@
         #
         #    a.txt
         #    a/b.txt
         #    a/c.txt
         #    a0.txt
         #
         # This is because in Unicode '.' comes before '/', which comes before '0'.
-        names = []  # list of (name, local_path, b2_path)
+        names = []  # list of (name, local_path, relative_file_path)
         for name in os.listdir(local_dir):
             # We expect listdir() to return unicode if dir_path is unicode.
             # If the file name is not valid, based on the file system
             # encoding, then listdir() will return un-decoded str/bytes.
             if not isinstance(name, str):
-                name = cls._handle_non_unicode_file_name(name)
+                name = self._handle_non_unicode_file_name(name)
 
             if '/' in name:
                 raise UnSyncableFilename(
                     "sync does not support file names that include '/'",
                     "%s in dir %s" % (name, local_dir)
                 )
 
             local_path = os.path.join(local_dir, name)
-            b2_path = join_b2_path(b2_dir, name)
+            relative_file_path = join_b2_path(
+                relative_dir_path, name
+            )  # file path relative to the sync point
 
             # Skip broken symlinks or other inaccessible files
             if not is_file_readable(local_path, reporter):
                 continue
 
             if policies_manager.exclude_all_symlinks and os.path.islink(local_path):
                 if reporter is not None:
                     reporter.symlink_skipped(local_path)
                 continue
 
             if os.path.isdir(local_path):
                 name += '/'
-                if policies_manager.should_exclude_directory(b2_path):
-                    continue
-            else:
-                if policies_manager.should_exclude_file(b2_path):
+                if policies_manager.should_exclude_local_directory(relative_file_path):
                     continue
 
-            names.append((name, local_path, b2_path))
+            names.append((name, local_path, relative_file_path))
 
         # Yield all of the answers.
         #
         # Sorting the list of triples puts them in the right order because 'name',
         # the sort key, is the first thing in the triple.
-        for (name, local_path, b2_path) in sorted(names):
+        for (name, local_path, relative_file_path) in sorted(names):
             if name.endswith('/'):
-                for subdir_file in cls._walk_relative_paths(
-                    local_path, b2_path, reporter, policies_manager
+                for subdir_file in self._walk_relative_paths(
+                    local_path, relative_file_path, reporter, policies_manager
                 ):
                     yield subdir_file
             else:
                 # Check that the file still exists and is accessible, since it can take a long time
                 # to iterate through large folders
                 if is_file_readable(local_path, reporter):
                     file_mod_time = get_file_mtime(local_path)
                     file_size = os.path.getsize(local_path)
-                    version = FileVersion(local_path, b2_path, file_mod_time, 'upload', file_size)
 
-                    if policies_manager.should_exclude_file_version(version):
+                    local_sync_path = LocalSyncPath(
+                        absolute_path=self.make_full_path(relative_file_path),
+                        relative_path=relative_file_path,
+                        mod_time=file_mod_time,
+                        size=file_size,
+                    )
+
+                    if policies_manager.should_exclude_local_path(local_sync_path):
                         continue
 
-                    yield File(b2_path, [version])
+                    yield local_sync_path
 
     @classmethod
     def _handle_non_unicode_file_name(cls, name):
         """
         Decide what to do with a name returned from os.listdir()
         that isn't unicode.  We think that this only happens when
         the file name can't be decoded using the file system
@@ -279,14 +277,24 @@
             return name
         raise EnvironmentEncodingError(repr(name), sys.getfilesystemencoding())
 
     def __repr__(self):
         return 'LocalFolder(%s)' % (self.root,)
 
 
+def b2_parent_dir(file_name):
+    # Various Parent dir getting method have been tested, and this one seems to be the faste
+    # After dropping python 3.9 support: refactor this use the "match" syntax
+    try:
+        dir_name, _ = file_name.rsplit('/', 1)
+    except ValueError:
+        return ''
+    return dir_name
+
+
 class B2Folder(AbstractFolder):
     """
     Folder interface to b2.
     """
 
     def __init__(self, bucket_name, folder_name, api):
         """
@@ -296,72 +304,93 @@
         :type folder_name: str
         :param api: an API object
         :type api: b2sdk.api.B2Api
         """
         self.bucket_name = bucket_name
         self.folder_name = folder_name
         self.bucket = api.get_bucket_by_name(bucket_name)
+        self.api = api
         self.prefix = '' if self.folder_name == '' else self.folder_name + '/'
 
-    def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
+    def all_files(
+        self, reporter: SyncReport, policies_manager: ScanPoliciesManager = DEFAULT_SCAN_MANAGER
+    ):
         """
         Yield all files.
-
-        :param reporter: a place to report errors
-        :param policies_manager: a policies manager object, default is DEFAULT_SCAN_MANAGER
         """
         current_name = None
+        last_ignored_dir = None
         current_versions = []
-        current_file_version_info = None
-        for file_version_info, _ in self.bucket.ls(
-            self.folder_name,
-            show_versions=True,
-            recursive=True,
-        ):
-            if current_file_version_info is None:
-                current_file_version_info = file_version_info
+        current_file_version = None
+        for file_version in self.get_file_versions():
+            if current_file_version is None:
+                current_file_version = file_version
+
+            assert file_version.file_name.startswith(self.prefix)
+            if file_version.action == 'start':
+                continue
+            file_name = file_version.file_name[len(self.prefix):]
+            if last_ignored_dir is not None and file_name.startswith(last_ignored_dir):
+                continue
 
-            assert file_version_info.file_name.startswith(self.prefix)
-            if file_version_info.action == 'start':
+            dir_name = b2_parent_dir(file_name)
+
+            if policies_manager.should_exclude_b2_directory(dir_name):
+                last_ignored_dir = dir_name + '/'
                 continue
-            file_name = file_version_info.file_name[len(self.prefix):]
+            else:
+                last_ignored_dir = None
 
-            if policies_manager.should_exclude_file(file_name):
+            if policies_manager.should_exclude_b2_file_version(file_version, file_name):
                 continue
 
-            # Do not allow relative paths in file names
-            if RELATIVE_PATH_MATCHER.search(file_name):
-                raise UnSyncableFilename(
-                    "sync does not support file names that include relative paths", file_name
-                )
-            # Do not allow absolute paths in file names
-            if ABSOLUTE_PATH_MATCHER.search(file_name):
-                raise UnSyncableFilename(
-                    "sync does not support file names with absolute paths", file_name
-                )
-            # On Windows, do not allow drive letters in file names
-            if platform.system() == "Windows" and DRIVE_MATCHER.search(file_name):
-                raise UnSyncableFilename(
-                    "sync does not support file names with drive letters", file_name
-                )
+            self._validate_file_name(file_name)
 
             if current_name != file_name and current_name is not None and current_versions:
-                yield B2File(current_name, current_versions)
+                yield B2SyncPath(
+                    relative_path=current_name,
+                    selected_version=current_versions[0],
+                    all_versions=current_versions
+                )
                 current_versions = []
 
             current_name = file_name
-            file_version = B2FileVersion(file_version_info)
-
-            if policies_manager.should_exclude_file_version(file_version):
-                continue
-
             current_versions.append(file_version)
 
         if current_name is not None and current_versions:
-            yield B2File(current_name, current_versions)
+            yield B2SyncPath(
+                relative_path=current_name,
+                selected_version=current_versions[0],
+                all_versions=current_versions
+            )
+
+    def get_file_versions(self):
+        for file_version, _ in self.bucket.ls(
+            self.folder_name,
+            show_versions=True,
+            recursive=True,
+        ):
+            yield file_version
+
+    def _validate_file_name(self, file_name):
+        # Do not allow relative paths in file names
+        if RELATIVE_PATH_MATCHER.search(file_name):
+            raise UnSyncableFilename(
+                "sync does not support file names that include relative paths", file_name
+            )
+        # Do not allow absolute paths in file names
+        if ABSOLUTE_PATH_MATCHER.search(file_name):
+            raise UnSyncableFilename(
+                "sync does not support file names with absolute paths", file_name
+            )
+        # On Windows, do not allow drive letters in file names
+        if platform.system() == "Windows" and DRIVE_MATCHER.search(file_name):
+            raise UnSyncableFilename(
+                "sync does not support file names with drive letters", file_name
+            )
 
     def folder_type(self):
         """
         Return folder type.
 
         :rtype: str
         """
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/folder_parser.py` & `b2sdk-1.9.0/b2sdk/sync/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/sync/policy.py` & `b2sdk-1.9.0/b2sdk/sync/policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 from abc import ABCMeta, abstractmethod
 from enum import Enum, unique
+from typing import Optional
 
 import logging
 
 from ..exception import DestFileNewer
 from .encryption_provider import AbstractSyncEncryptionSettingsProvider, SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER
 from .action import LocalDeleteAction, B2CopyAction, B2DeleteAction, B2DownloadAction, B2HideAction, B2UploadAction
 from .exception import InvalidArgument
+from .folder import AbstractFolder
+from .path import AbstractSyncPath
 
 ONE_DAY_IN_MS = 24 * 60 * 60 * 1000
 
 logger = logging.getLogger(__name__)
 
 
 @unique
@@ -44,107 +47,107 @@
     Abstract policy class.
     """
     DESTINATION_PREFIX = NotImplemented
     SOURCE_PREFIX = NotImplemented
 
     def __init__(
         self,
-        source_file,
-        source_folder,
-        dest_file,
-        dest_folder,
-        now_millis,
-        keep_days,
-        newer_file_mode,
-        compare_threshold,
-        compare_version_mode=CompareVersionMode.MODTIME,
+        source_path: AbstractSyncPath,
+        source_folder: AbstractFolder,
+        dest_path: AbstractSyncPath,
+        dest_folder: AbstractFolder,
+        now_millis: int,
+        keep_days: int,
+        newer_file_mode: NewerFileSyncMode,
+        compare_threshold: int,
+        compare_version_mode: CompareVersionMode = CompareVersionMode.MODTIME,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
-        :param b2sdk.v1.File source_file: source file object
+        :param b2sdk.v1.AbstractSyncPath source_path: source file object
         :param b2sdk.v1.AbstractFolder source_folder: source folder object
-        :param b2sdk.v1.File dest_file: destination file object
+        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
         :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
         :param int now_millis: current time in milliseconds
         :param int keep_days: days to keep before delete
-        :param b2sdk.v1.NEWER_FILE_MODES newer_file_mode: setting which determines handling for destination files newer than on the source
+        :param b2sdk.v1.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
         :param int compare_threshold: when comparing with size or time for sync
         :param b2sdk.v1.COMPARE_VERSION_MODES compare_version_mode: how to compare source and destination files
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
         """
-        self._source_file = source_file
+        self._source_path = source_path
         self._source_folder = source_folder
-        self._dest_file = dest_file
+        self._dest_path = dest_path
         self._keep_days = keep_days
         self._newer_file_mode = newer_file_mode
         self._compare_version_mode = compare_version_mode
         self._compare_threshold = compare_threshold
         self._dest_folder = dest_folder
         self._now_millis = now_millis
         self._transferred = False
         self._encryption_settings_provider = encryption_settings_provider
 
     def _should_transfer(self):
         """
         Decide whether to transfer the file from the source to the destination.
         """
-        if self._source_file is None or self._source_file.latest_version().action == 'hide':
+        if self._source_path is None or not self._source_path.is_visible():
             # No source file.  Nothing to transfer.
             return False
-        elif self._dest_file is None:
+        elif self._dest_path is None:
             # Source file exists, but no destination file.  Always transfer.
             return True
         else:
             # Both exist.  Transfer only if the two are different.
             return self.files_are_different(
-                self._source_file,
-                self._dest_file,
+                self._source_path,
+                self._dest_path,
                 self._compare_threshold,
                 self._compare_version_mode,
                 self._newer_file_mode,
             )
 
     @classmethod
     def files_are_different(
         cls,
-        source_file,
-        dest_file,
-        compare_threshold=None,
-        compare_version_mode=CompareVersionMode.MODTIME,
-        newer_file_mode=NewerFileSyncMode.RAISE_ERROR,
+        source_path: AbstractSyncPath,
+        dest_path: AbstractSyncPath,
+        compare_threshold: Optional[int] = None,
+        compare_version_mode: CompareVersionMode = CompareVersionMode.MODTIME,
+        newer_file_mode: NewerFileSyncMode = NewerFileSyncMode.RAISE_ERROR,
     ):
         """
         Compare two files and determine if the the destination file
         should be replaced by the source file.
 
-        :param b2sdk.v1.File source_file: source file object
-        :param b2sdk.v1.File dest_file: destination file object
+        :param b2sdk.v1.AbstractSyncPath source_path: source file object
+        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
         :param int compare_threshold: compare threshold when comparing by time or size
         :param b2sdk.v1.CompareVersionMode compare_version_mode: source file version comparator method
         :param b2sdk.v1.NewerFileSyncMode newer_file_mode: newer destination handling method
         """
         # Optionally set a compare threshold for fuzzy comparison
         compare_threshold = compare_threshold or 0
 
         # Compare using file name only
         if compare_version_mode == CompareVersionMode.NONE:
             return False
 
         # Compare using modification time
         elif compare_version_mode == CompareVersionMode.MODTIME:
             # Get the modification time of the latest versions
-            source_mod_time = source_file.latest_version().mod_time
-            dest_mod_time = dest_file.latest_version().mod_time
+            source_mod_time = source_path.mod_time
+            dest_mod_time = dest_path.mod_time
             diff_mod_time = abs(source_mod_time - dest_mod_time)
             compare_threshold_exceeded = diff_mod_time > compare_threshold
 
             logger.debug(
                 'File %s: source time %s, dest time %s, diff %s, threshold %s, diff > threshold %s',
-                source_file.name,
+                source_path.relative_path,
                 source_mod_time,
                 dest_mod_time,
                 diff_mod_time,
                 compare_threshold,
                 compare_threshold_exceeded,
             )
 
@@ -157,28 +160,28 @@
                 elif source_mod_time < dest_mod_time:
                     if newer_file_mode == NewerFileSyncMode.REPLACE:
                         return True
                     elif newer_file_mode == NewerFileSyncMode.SKIP:
                         return False
                     else:
                         raise DestFileNewer(
-                            dest_file, source_file, cls.DESTINATION_PREFIX, cls.SOURCE_PREFIX
+                            dest_path, source_path, cls.DESTINATION_PREFIX, cls.SOURCE_PREFIX
                         )
 
         # Compare using file size
         elif compare_version_mode == CompareVersionMode.SIZE:
             # Get file size of the latest versions
-            source_size = source_file.latest_version().size
-            dest_size = dest_file.latest_version().size
+            source_size = source_path.size
+            dest_size = dest_path.size
             diff_size = abs(source_size - dest_size)
             compare_threshold_exceeded = diff_size > compare_threshold
 
             logger.debug(
                 'File %s: source size %s, dest size %s, diff %s, threshold %s, diff > threshold %s',
-                source_file.name,
+                source_path.relative_path,
                 source_size,
                 dest_size,
                 diff_size,
                 compare_threshold,
                 compare_threshold_exceeded,
             )
 
@@ -191,27 +194,27 @@
         """
         Yield file actions.
         """
         if self._should_transfer():
             yield self._make_transfer_action()
             self._transferred = True
 
-        assert self._dest_file is not None or self._source_file is not None
+        assert self._dest_path is not None or self._source_path is not None
 
         for action in self._get_hide_delete_actions():
             yield action
 
     def _get_hide_delete_actions(self):
         """
         Subclass policy can override this to hide or delete files.
         """
         return []
 
     def _get_source_mod_time(self):
-        return self._source_file.latest_version().mod_time
+        return self._source_path.mod_time
 
     @abstractmethod
     def _make_transfer_action(self):
         """
         Return an action representing transfer of file according to the selected policy.
         """
 
@@ -221,50 +224,50 @@
     File is synced down (from the cloud to disk).
     """
     DESTINATION_PREFIX = 'local://'
     SOURCE_PREFIX = 'b2://'
 
     def _make_transfer_action(self):
         return B2DownloadAction(
-            self._source_file,
-            self._source_folder.make_full_path(self._source_file.name),
-            self._dest_folder.make_full_path(self._source_file.name),
+            self._source_path,
+            self._source_folder.make_full_path(self._source_path.relative_path),
+            self._dest_folder.make_full_path(self._source_path.relative_path),
             self._encryption_settings_provider,
         )
 
 
 class UpPolicy(AbstractFileSyncPolicy):
     """
     File is synced up (from disk the cloud).
     """
     DESTINATION_PREFIX = 'b2://'
     SOURCE_PREFIX = 'local://'
 
     def _make_transfer_action(self):
         return B2UploadAction(
-            self._source_folder.make_full_path(self._source_file.name),
-            self._source_file.name,
-            self._dest_folder.make_full_path(self._source_file.name),
+            self._source_folder.make_full_path(self._source_path.relative_path),
+            self._source_path.relative_path,
+            self._dest_folder.make_full_path(self._source_path.relative_path),
             self._get_source_mod_time(),
-            self._source_file.latest_version().size,
+            self._source_path.size,
             self._encryption_settings_provider,
         )
 
 
 class UpAndDeletePolicy(UpPolicy):
     """
     File is synced up (from disk to the cloud) and the delete flag is SET.
     """
 
     def _get_hide_delete_actions(self):
         for action in super(UpAndDeletePolicy, self)._get_hide_delete_actions():
             yield action
         for action in make_b2_delete_actions(
-            self._source_file,
-            self._dest_file,
+            self._source_path,
+            self._dest_path,
             self._dest_folder,
             self._transferred,
         ):
             yield action
 
 
 class UpAndKeepDaysPolicy(UpPolicy):
@@ -272,16 +275,16 @@
     File is synced up (from disk to the cloud) and the keepDays flag is SET.
     """
 
     def _get_hide_delete_actions(self):
         for action in super(UpAndKeepDaysPolicy, self)._get_hide_delete_actions():
             yield action
         for action in make_b2_keep_days_actions(
-            self._source_file,
-            self._dest_file,
+            self._source_path,
+            self._dest_path,
             self._dest_folder,
             self._transferred,
             self._keep_days,
             self._now_millis,
         ):
             yield action
 
@@ -290,20 +293,21 @@
     """
     File is synced down (from the cloud to disk) and the delete flag is SET.
     """
 
     def _get_hide_delete_actions(self):
         for action in super(DownAndDeletePolicy, self)._get_hide_delete_actions():
             yield action
-        if self._dest_file is not None and (
-            self._source_file is None or self._source_file.latest_version().action == 'hide'
+        if self._dest_path is not None and (
+            self._source_path is None or not self._source_path.is_visible()
         ):
-            # Local files have either 0 or 1 versions.  If the file is there,
-            # it must have exactly 1 version.
-            yield LocalDeleteAction(self._dest_file.name, self._dest_file.versions[0].id_)
+            yield LocalDeleteAction(
+                self._dest_path.relative_path,
+                self._dest_folder.make_full_path(self._dest_path.relative_path)
+            )
 
 
 class DownAndKeepDaysPolicy(DownPolicy):
     """
     File is synced down (from the cloud to disk) and the keepDays flag is SET.
     """
     pass
@@ -315,17 +319,17 @@
     """
     DESTINATION_PREFIX = 'b2://'
     SOURCE_PREFIX = 'b2://'
 
     def _make_transfer_action(self):
 
         return B2CopyAction(
-            self._source_folder.make_full_path(self._source_file.name),
-            self._source_file,
-            self._dest_folder.make_full_path(self._source_file.name),
+            self._source_folder.make_full_path(self._source_path.relative_path),
+            self._source_path,
+            self._dest_folder.make_full_path(self._source_path.relative_path),
             self._source_folder.bucket,
             self._dest_folder.bucket,
             self._encryption_settings_provider,
         )
 
 
 class CopyAndDeletePolicy(CopyPolicy):
@@ -333,16 +337,16 @@
     File is copied (server-side) and the delete flag is SET.
     """
 
     def _get_hide_delete_actions(self):
         for action in super()._get_hide_delete_actions():
             yield action
         for action in make_b2_delete_actions(
-            self._source_file,
-            self._dest_file,
+            self._source_path,
+            self._dest_path,
             self._dest_folder,
             self._transferred,
         ):
             yield action
 
 
 class CopyAndKeepDaysPolicy(CopyPolicy):
@@ -350,16 +354,16 @@
     File is copied (server-side) and the keepDays flag is SET.
     """
 
     def _get_hide_delete_actions(self):
         for action in super()._get_hide_delete_actions():
             yield action
         for action in make_b2_keep_days_actions(
-            self._source_file,
-            self._dest_file,
+            self._source_path,
+            self._dest_path,
             self._dest_folder,
             self._transferred,
             self._keep_days,
             self._now_millis,
         ):
             yield action
 
@@ -376,94 +380,106 @@
     if version.action == 'hide':
         note = '(hide marker)'
     elif transferred or 0 < index:
         note = '(old version)'
     return note
 
 
-def make_b2_delete_actions(source_file, dest_file, dest_folder, transferred):
+def make_b2_delete_actions(
+    source_path: AbstractSyncPath,
+    dest_path: AbstractSyncPath,
+    dest_folder: AbstractFolder,
+    transferred: bool,
+):
     """
     Create the actions to delete files stored on B2, which are not present locally.
 
-    :param b2sdk.v1.File source_file: source file object
-    :param b2sdk.v1.File dest_file: destination file object
+    :param b2sdk.v1.AbstractSyncPath source_path: source file object
+    :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
     :param b2sdk.v1.AbstractFolder dest_folder: destination folder
     :param bool transferred: if True, file has been transferred, False otherwise
     """
-    if dest_file is None:
+    if dest_path is None:
         # B2 does not really store folders, so there is no need to hide
         # them or delete them
         return
-    for version_index, version in enumerate(dest_file.versions):
-        keep = (version_index == 0) and (source_file is not None) and not transferred
+    for version_index, version in enumerate(dest_path.all_versions):
+        keep = (version_index == 0) and (source_path is not None) and not transferred
         if not keep:
             yield B2DeleteAction(
-                dest_file.name,
-                dest_folder.make_full_path(dest_file.name),
+                dest_path.relative_path,
+                dest_folder.make_full_path(dest_path.relative_path),
                 version.id_,
                 make_b2_delete_note(version, version_index, transferred),
             )
 
 
 def make_b2_keep_days_actions(
-    source_file, dest_file, dest_folder, transferred, keep_days, now_millis
+    source_path: AbstractSyncPath,
+    dest_path: AbstractSyncPath,
+    dest_folder: AbstractFolder,
+    transferred: bool,
+    keep_days: int,
+    now_millis: int,
 ):
     """
     Create the actions to hide or delete existing versions of a file
     stored in b2.
 
     When keepDays is set, all files that were visible any time from
     keepDays ago until now must be kept.  If versions were uploaded 5
     days ago, 15 days ago, and 25 days ago, and the keepDays is 10,
     only the 25-day old version can be deleted.  The 15 day-old version
     was visible 10 days ago.
 
-    :param b2sdk.v1.File source_file: source file object
-    :param b2sdk.v1.File dest_file: destination file object
+    :param b2sdk.v1.AbstractSyncPath source_path: source file object
+    :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
     :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
     :param bool transferred: if True, file has been transferred, False otherwise
     :param int keep_days: how many days to keep a file
     :param int now_millis: current time in milliseconds
     """
     deleting = False
-    if dest_file is None:
+    if dest_path is None:
         # B2 does not really store folders, so there is no need to hide
         # them or delete them
         return
-    for version_index, version in enumerate(dest_file.versions):
+    for version_index, version in enumerate(dest_path.all_versions):
         # How old is this version?
-        age_days = (now_millis - version.mod_time) / ONE_DAY_IN_MS
+        age_days = (now_millis - version.mod_time_millis) / ONE_DAY_IN_MS
 
         # Mostly, the versions are ordered by time, newest first,
         # BUT NOT ALWAYS. The mod time we have is the src_last_modified_millis
         # from the file info (if present), or the upload start time
         # (if not present). The user-specified src_last_modified_millis
         # may not be in order. Because of that, we no longer
         # assert that age_days is non-decreasing.
         #
         # Note that if there is an out-of-order date that is old enough
         # to trigger deletions, all of the versions uploaded before that
         # (the ones after it in the list) will be deleted, even if they
         # aren't over the age threshold.
 
         # Do we need to hide this version?
-        if version_index == 0 and source_file is None and version.action == 'upload':
-            yield B2HideAction(dest_file.name, dest_folder.make_full_path(dest_file.name))
+        if version_index == 0 and source_path is None and version.action == 'upload':
+            yield B2HideAction(
+                dest_path.relative_path, dest_folder.make_full_path(dest_path.relative_path)
+            )
 
         # Can we start deleting? Once we start deleting, all older
         # versions will also be deleted.
         if version.action == 'hide':
             if keep_days < age_days:
                 deleting = True
 
         # Delete this version
         if deleting:
             yield B2DeleteAction(
-                dest_file.name,
-                dest_folder.make_full_path(dest_file.name),
+                dest_path.relative_path,
+                dest_folder.make_full_path(dest_path.relative_path),
                 version.id_,
                 make_b2_delete_note(version, version_index, transferred),
             )
 
         # Can we start deleting with the next version, based on the
         # age of this one?
         if keep_days < age_days:
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/policy_manager.py` & `b2sdk-1.9.0/b2sdk/sync/policy_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,63 +7,63 @@
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 from .policy import CopyAndDeletePolicy, CopyAndKeepDaysPolicy, CopyPolicy, \
     DownAndDeletePolicy, DownAndKeepDaysPolicy, DownPolicy, UpAndDeletePolicy, \
     UpAndKeepDaysPolicy, UpPolicy
-from .file import File
+from .path import AbstractSyncPath
 
 
 class SyncPolicyManager(object):
     """
     Policy manager; implement a logic to get a correct policy class
     and create a policy object based on various parameters.
     """
 
     def __init__(self):
         self.policies = {}  # dict<,>
 
     def get_policy(
         self,
         sync_type,
-        source_file: File,
+        source_path: AbstractSyncPath,
         source_folder,
-        dest_file: File,
+        dest_path: AbstractSyncPath,
         dest_folder,
         now_millis,
         delete,
         keep_days,
         newer_file_mode,
         compare_threshold,
         compare_version_mode,
         encryption_settings_provider,
     ):
         """
         Return a policy object.
 
         :param str sync_type: synchronization type
-        :param b2sdk.v1.File source_file: source file name
+        :param b2sdk.v1.AbstractSyncPath source_path: source file
         :param str source_folder: a source folder path
-        :param b2sdk.v1.File dest_file: destination file name
+        :param b2sdk.v1.AbstractSyncPath dest_path: destination file
         :param str dest_folder: a destination folder path
         :param int now_millis: current time in milliseconds
         :param bool delete: delete policy
         :param int keep_days: keep for days policy
         :param b2sdk.v1.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
         :param int compare_threshold: difference between file modification time or file size
         :param b2sdk.v1.CompareVersionMode compare_version_mode: setting which determines how to compare source and destination files
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: an object which decides which encryption to use (if any)
         :return: a policy object
         """
         policy_class = self.get_policy_class(sync_type, delete, keep_days)
         return policy_class(
-            source_file,
+            source_path,
             source_folder,
-            dest_file,
+            dest_path,
             dest_folder,
             now_millis,
             keep_days,
             newer_file_mode,
             compare_threshold,
             compare_version_mode,
             encryption_settings_provider,
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/report.py` & `b2sdk-1.9.0/b2sdk/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/sync/scan_policies.py` & `b2sdk-1.9.0/b2sdk/sync/scan_policies.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import logging
 import re
+from typing import Optional, Union, Iterable
 
 from .exception import InvalidArgument, check_invalid_argument
+from .path import LocalSyncPath
+from ..file_version import FileVersion
 
 logger = logging.getLogger(__name__)
 
+try:  # python 3.5 and 3.6 compatibility
+    regex_class = re.Pattern
+except AttributeError:
+    regex_class = re._pattern_type
+
 
 class RegexSet(object):
     """
     Hold a (possibly empty) set of regular expressions and know how to check
     whether a string matches any of them.
     """
 
@@ -114,34 +122,38 @@
     Code that scans may optionally use should_exclude_directory() to test whether
     it can skip a directory completely and not bother listing the files and
     sub-directories in it.
     """
 
     def __init__(
         self,
-        exclude_dir_regexes=tuple(),
-        exclude_file_regexes=tuple(),
-        include_file_regexes=tuple(),
-        exclude_all_symlinks=False,
-        exclude_modified_before=None,
-        exclude_modified_after=None,
+        exclude_dir_regexes: Iterable[Union[str, regex_class]] = tuple(),
+        exclude_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
+        include_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
+        exclude_all_symlinks: bool = False,
+        exclude_modified_before: Optional[int] = None,
+        exclude_modified_after: Optional[int] = None,
+        exclude_uploaded_before: Optional[int] = None,
+        exclude_uploaded_after: Optional[int] = None,
     ):
         """
-        :param exclude_dir_regexes: a tuple of regexes to exclude directories
-        :type exclude_dir_regexes: tuple
-        :param exclude_file_regexes: a tuple of regexes to exclude files
-        :type exclude_file_regexes: tuple
-        :param include_file_regexes: a tuple of regexes to include files
-        :type include_file_regexes: tuple
+        :param exclude_dir_regexes: regexes to exclude directories
+        :param exclude_file_regexes: regexes to exclude files
+        :param include_file_regexes: regexes to include files
         :param exclude_all_symlinks: if True, exclude all symlinks
-        :type exclude_all_symlinks: bool
-        :param exclude_modified_before: optionally exclude file versions modified before (in millis)
-        :type exclude_modified_before: int, optional
-        :param exclude_modified_after: optionally exclude file versions modified after (in millis)
-        :type exclude_modified_after: int, optional
+        :param exclude_modified_before: optionally exclude file versions (both local and b2) modified before (in millis)
+        :param exclude_modified_after: optionally exclude file versions (both local and b2) modified after (in millis)
+        :param exclude_uploaded_before: optionally exclude b2 file versions uploaded before (in millis)
+        :param exclude_uploaded_after: optionally exclude b2 file versions uploaded after (in millis)
+
+        The regex matching priority for a given path is:
+        1) the path is always excluded if it's dir matches `exclude_dir_regexes`, if not then
+        2) the path is always included if it matches `include_file_regexes`, if not then
+        3) the path is excluded if it matches `exclude_file_regexes`, if not then
+        4) the path is included
         """
         if include_file_regexes and not exclude_file_regexes:
             raise InvalidArgument(
                 'include_file_regexes',
                 'cannot be used without exclude_file_regexes at the same time'
             )
 
@@ -163,55 +175,57 @@
         self.exclude_all_symlinks = exclude_all_symlinks
         with check_invalid_argument(
             'exclude_modified_before,exclude_modified_after', '', ValueError
         ):
             self._include_mod_time_range = IntegerRange(
                 exclude_modified_before, exclude_modified_after
             )
+        with check_invalid_argument(
+            'exclude_uploaded_before,exclude_uploaded_after', '', ValueError
+        ):
+            self._include_upload_time_range = IntegerRange(
+                exclude_uploaded_before, exclude_uploaded_after
+            )
 
-    def should_exclude_file(self, file_path):
+    def _should_exclude_relative_path(self, relative_path: str):
+        if self._include_file_set.matches(relative_path):
+            return False
+        return self._exclude_file_set.matches(relative_path)
+
+    def should_exclude_local_path(self, local_path: LocalSyncPath):
         """
-        Given the full path of a file, decide if it should be excluded from the scan.
+        Whether a local path should be excluded from the Sync or not.
 
-        :param file_path: the path of the file, relative to the root directory
-                          being scanned.
-        :type: str
-        :return: True if excluded.
-        :rtype: bool
+        This method assumes that the directory holding the `path_` has already been checked for exclusion.
         """
-        # TODO: In v2 this should accept `b2sdk.v1.File`.
-        #  It requires some refactoring to be done first.
-        exclude_because_of_dir = self._exclude_file_because_of_dir_set.matches(file_path)
-        exclude_because_of_file = (
-            self._exclude_file_set.matches(file_path) and
-            not self._include_file_set.matches(file_path)
-        )
-        return exclude_because_of_dir or exclude_because_of_file
-
-    def should_exclude_file_version(self, file_version):
-        """
-        Given the modification time of a file version,
-        decide if it should be excluded from the scan.
-
-        :param file_version: the file version object
-        :type: b2sdk.v1.FileVersion
-        :return: True if excluded.
-        :rtype: bool
+        if local_path.mod_time not in self._include_mod_time_range:
+            return True
+        return self._should_exclude_relative_path(local_path.relative_path)
+
+    def should_exclude_b2_file_version(self, file_version: FileVersion, relative_path: str):
+        """
+        Whether a b2 file version should be excluded from the Sync or not.
+
+        This method assumes that the directory holding the `path_` has already been checked for exclusion.
         """
-        return file_version.mod_time not in self._include_mod_time_range
+        if file_version.upload_timestamp not in self._include_upload_time_range:
+            return True
+        if file_version.mod_time_millis not in self._include_mod_time_range:
+            return True
+        return self._should_exclude_relative_path(relative_path)
 
-    def should_exclude_directory(self, dir_path):
+    def should_exclude_b2_directory(self, dir_path: str):
         """
-        Given the full path of a directory, decide if all of the files in it should be
-        excluded from the scan.
+        Given the path of a directory, relative to the sync point,
+        decide if all of the files in it should be excluded from the scan.
+        """
+        return self._exclude_dir_set.matches(dir_path)
 
-        :param dir_path: the path of the directory, relative to the root directory
-                         being scanned.  The path will never end in '/'.
-        :type dir_path: str
-        :return: True if excluded.
+    def should_exclude_local_directory(self, dir_path: str):
+        """
+        Given the path of a directory, relative to the sync point,
+        decide if all of the files in it should be excluded from the scan.
         """
-        # TODO: In v2 this should accept `b2sdk.v1.AbstractFolder`.
-        #  It requires some refactoring to be done first.
         return self._exclude_dir_set.matches(dir_path)
 
 
 DEFAULT_SCAN_MANAGER = ScanPoliciesManager()
```

### Comparing `b2sdk-1.8.0/b2sdk/sync/sync.py` & `b2sdk-1.9.0/b2sdk/sync/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 import logging
 import concurrent.futures as futures
 from enum import Enum, unique
 
 from ..bounded_queue_executor import BoundedQueueExecutor
 from .encryption_provider import AbstractSyncEncryptionSettingsProvider, SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER
 from .exception import InvalidArgument, IncompleteSync
+from .folder import AbstractFolder
+from .path import AbstractSyncPath
 from .policy import CompareVersionMode, NewerFileSyncMode
-from .policy_manager import POLICY_MANAGER
+from .policy_manager import POLICY_MANAGER, SyncPolicyManager
+from .report import SyncReport
 from .scan_policies import DEFAULT_SCAN_MANAGER
 
 logger = logging.getLogger(__name__)
 
 
 def next_or_none(iterator):
     """
@@ -57,22 +60,22 @@
     while current_a is not None or current_b is not None:
         if current_a is None:
             yield (None, current_b)
             current_b = next_or_none(iter_b)
         elif current_b is None:
             yield (current_a, None)
             current_a = next_or_none(iter_a)
-        elif current_a.name < current_b.name:
+        elif current_a.relative_path < current_b.relative_path:
             yield (current_a, None)
             current_a = next_or_none(iter_a)
-        elif current_b.name < current_a.name:
+        elif current_b.relative_path < current_a.relative_path:
             yield (None, current_b)
             current_b = next_or_none(iter_b)
         else:
-            assert current_a.name == current_b.name
+            assert current_a.relative_path == current_b.relative_path
             yield (current_a, current_b)
             current_a = next_or_none(iter_a)
             current_b = next_or_none(iter_b)
 
 
 def count_files(local_folder, reporter, policies_manager):
     """
@@ -239,15 +242,15 @@
         action_bucket = None
         if dest_type == 'b2':
             action_bucket = dest_folder.bucket
         elif source_type == 'b2':
             action_bucket = source_folder.bucket
 
         # Schedule each of the actions.
-        for action in self.make_folder_sync_actions(
+        for action in self._make_folder_sync_actions(
             source_folder,
             dest_folder,
             now_millis,
             reporter,
             self.policies_manager,
             encryption_settings_provider,
         ):
@@ -255,69 +258,69 @@
             sync_executor.submit(action.run, action_bucket, reporter, self.dry_run)
 
         # Wait for everything to finish
         sync_executor.shutdown()
         if sync_executor.get_num_exceptions() != 0:
             raise IncompleteSync('sync is incomplete')
 
-    def make_folder_sync_actions(
+    def _make_folder_sync_actions(
         self,
-        source_folder,
-        dest_folder,
-        now_millis,
-        reporter,
-        policies_manager=DEFAULT_SCAN_MANAGER,
+        source_folder: AbstractFolder,
+        dest_folder: AbstractFolder,
+        now_millis: int,
+        reporter: SyncReport,
+        policies_manager: SyncPolicyManager = DEFAULT_SCAN_MANAGER,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
         Yield a sequence of actions that will sync the destination
         folder to the source folder.
 
         :param b2sdk.v1.AbstractFolder source_folder: source folder object
         :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
         :param int now_millis: current time in milliseconds
         :param b2sdk.v1.SyncReport reporter: reporter object
-        :param policies_manager: policies manager object
+        :param b2sdk.v1.SyncPolicyManager policies_manager: policies manager object
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
         """
         if self.keep_days_or_delete == KeepOrDeleteMode.KEEP_BEFORE_DELETE and dest_folder.folder_type(
         ) == 'local':
             raise InvalidArgument('keep_days_or_delete', 'cannot be used for local files')
 
         source_type = source_folder.folder_type()
         dest_type = dest_folder.folder_type()
         sync_type = '%s-to-%s' % (source_type, dest_type)
         if source_type != 'b2' and dest_type != 'b2':
             raise ValueError('Sync between two local folders is not supported!')
 
         total_files = 0
         total_bytes = 0
-        for source_file, dest_file in zip_folders(
+        for source_path, dest_path in zip_folders(
             source_folder,
             dest_folder,
             reporter,
             policies_manager,
         ):
-            if source_file is None:
-                logger.debug('determined that %s is not present on source', dest_file)
-            elif dest_file is None:
-                logger.debug('determined that %s is not present on destination', source_file)
+            if source_path is None:
+                logger.debug('determined that %s is not present on source', dest_path)
+            elif dest_path is None:
+                logger.debug('determined that %s is not present on destination', source_path)
 
-            if source_file is not None:
+            if source_path is not None:
                 if source_type == 'b2':
                     # For buckets we don't want to count files separately as it would require
                     # more API calls. Instead, we count them when comparing.
                     reporter.update_total(1)
                 reporter.update_compare(1)
 
-            for action in self.make_file_sync_actions(
+            for action in self._make_file_sync_actions(
                 sync_type,
-                source_file,
-                dest_file,
+                source_path,
+                dest_path,
                 source_folder,
                 dest_folder,
                 now_millis,
                 encryption_settings_provider,
             ):
                 total_files += 1
                 total_bytes += action.get_bytes()
@@ -326,44 +329,44 @@
         if reporter is not None:
             if source_type == 'b2':
                 # For buckets we don't want to count files separately as it would require
                 # more API calls. Instead, we count them when comparing.
                 reporter.end_total()
             reporter.end_compare(total_files, total_bytes)
 
-    def make_file_sync_actions(
+    def _make_file_sync_actions(
         self,
-        sync_type,
-        source_file,
-        dest_file,
-        source_folder,
-        dest_folder,
-        now_millis,
+        sync_type: str,
+        source_path: AbstractSyncPath,
+        dest_path: AbstractSyncPath,
+        source_folder: AbstractFolder,
+        dest_folder: AbstractFolder,
+        now_millis: int,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
         Yields the sequence of actions needed to sync the two files
 
         :param str sync_type: synchronization type
-        :param b2sdk.v1.File source_file: source file object
-        :param b2sdk.v1.File dest_file: destination file object
+        :param b2sdk.v1.AbstractSyncPath source_path: source file object
+        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
         :param b2sdk.v1.AbstractFolder source_folder: a source folder object
         :param b2sdk.v1.AbstractFolder dest_folder: a destination folder object
         :param int now_millis: current time in milliseconds
         :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
         """
         delete = self.keep_days_or_delete == KeepOrDeleteMode.DELETE
         keep_days = self.keep_days
 
         policy = POLICY_MANAGER.get_policy(
             sync_type,
-            source_file,
+            source_path,
             source_folder,
-            dest_file,
+            dest_path,
             dest_folder,
             now_millis,
             delete,
             keep_days,
             self.newer_file_mode,
             self.compare_threshold,
             self.compare_version_mode,
```

### Comparing `b2sdk-1.8.0/b2sdk/transfer/__init__.py` & `b2sdk-1.9.0/b2sdk/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/emerger.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/emerger.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/executor.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from abc import ABCMeta, abstractmethod
 from typing import Optional
 
 from b2sdk.encryption.setting import EncryptionSetting
 from b2sdk.exception import MaxFileSizeExceeded
 from b2sdk.file_lock import FileRetentionSetting, LegalHold, NO_RETENTION_FILE_SETTING
-from b2sdk.file_version import FileVersionInfoFactory
 from b2sdk.transfer.outbound.large_file_upload_state import LargeFileUploadState
 from b2sdk.transfer.outbound.upload_source import UploadSourceStream
 from b2sdk.utils import interruptible_get_result
 
 AUTO_CONTENT_TYPE = 'b2/x-auto'
 
 
@@ -147,15 +146,14 @@
         self._semaphore = None
         if self.max_queue_size is not None:
             self._semaphore = threading.Semaphore(self.max_queue_size)
 
     def execute_plan(self, emerge_plan):
         total_length = emerge_plan.get_total_length()
         encryption = self.encryption
-        encryption = self.encryption
 
         if total_length is not None and total_length > self.MAX_LARGE_FILE_SIZE:
             raise MaxFileSizeExceeded(total_length, self.MAX_LARGE_FILE_SIZE)
 
         plan_id = emerge_plan.get_plan_id()
 
         file_info = dict(self.file_info) if self.file_info is not None else {}
@@ -216,15 +214,15 @@
             # Collect the sha1 checksums of the parts as the uploads finish.
             # If any of them raised an exception, that same exception will
             # be raised here by result()
             part_sha1_array = [interruptible_get_result(f)['contentSha1'] for f in part_futures]
 
         # Finish the large file
         response = self.services.session.finish_large_file(file_id, part_sha1_array)
-        return FileVersionInfoFactory.from_api_response(response)
+        return self.services.api.file_version_factory.from_api_response(response)
 
     def _execute_step(self, execution_step):
         semaphore = self._semaphore
         if semaphore is None:
             return execution_step.execute()
         else:
             semaphore.acquire()
```

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/planner/part_definition.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/part_definition.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/planner/planner.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/planner.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/planner/upload_subpart.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/upload_subpart.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/emerge/write_intent.py` & `b2sdk-1.9.0/b2sdk/transfer/emerge/write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/download_manager.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/download_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/abstract.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/parallel.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/parallel.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/range.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/range.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/downloader/simple.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/simple.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/inbound/file_metadata.py` & `b2sdk-1.9.0/b2sdk/transfer/inbound/file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/copy_manager.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/copy_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import concurrent.futures as futures
 import logging
 from typing import Optional
 
 from b2sdk.encryption.setting import EncryptionMode, EncryptionSetting, SSE_C_KEY_ID_FILE_INFO_KEY_NAME
 from b2sdk.exception import AlreadyFailed, SSECKeyIdMismatchInCopy
 from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.file_version import FileVersionInfoFactory
 from b2sdk.raw_api import MetadataDirectiveMode
 from b2sdk.utils import B2TraceMetaAbstract
 
 logger = logging.getLogger(__name__)
 
 
 class CopyManager(metaclass=B2TraceMetaAbstract):
@@ -212,19 +211,19 @@
                 file_info=file_info,
                 destination_bucket_id=destination_bucket_id,
                 destination_server_side_encryption=destination_encryption,
                 source_server_side_encryption=source_encryption,
                 legal_hold=legal_hold,
                 file_retention=file_retention,
             )
-            file_info = FileVersionInfoFactory.from_api_response(response)
+            file_version = self.services.api.file_version_factory.from_api_response(response)
             if progress_listener is not None:
-                progress_listener.bytes_completed(file_info.size)
+                progress_listener.bytes_completed(file_version.size)
 
-        return file_info
+        return file_version
 
     @classmethod
     def establish_sse_c_file_metadata(
         cls,
         metadata_directive: MetadataDirectiveMode,
         destination_file_info: Optional[dict],
         destination_content_type: Optional[str],
```

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/copy_source.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/copy_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/large_file_upload_state.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/large_file_upload_state.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/outbound_source.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/outbound_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/progress_reporter.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/upload_manager.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/upload_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from b2sdk.encryption.setting import EncryptionMode, EncryptionSetting
 from b2sdk.exception import (
     AlreadyFailed,
     B2Error,
     MaxRetriesExceeded,
 )
 from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.file_version import FileVersionInfoFactory
 from b2sdk.stream.progress import ReadingStreamWithProgress
 from b2sdk.stream.hashing import StreamWithHash
 from b2sdk.raw_api import HEX_DIGITS_AT_END
 from b2sdk.utils import B2TraceMetaAbstract
 
 from .progress_reporter import PartProgressReporter
 
@@ -244,15 +243,15 @@
                             file_retention=file_retention,
                             legal_hold=legal_hold,
                         )
                         if content_sha1 == HEX_DIGITS_AT_END:
                             content_sha1 = input_stream.hash
                         assert content_sha1 == response[
                             'contentSha1'], '%s != %s' % (content_sha1, response['contentSha1'])
-                        return FileVersionInfoFactory.from_api_response(response)
+                        return self.services.api.file_version_factory.from_api_response(response)
 
                 except B2Error as e:
                     if not e.should_retry_upload():
                         raise
                     exception_info_list.append(e)
                     self.account_info.clear_bucket_upload_data(bucket_id)
```

### Comparing `b2sdk-1.8.0/b2sdk/transfer/outbound/upload_source.py` & `b2sdk-1.9.0/b2sdk/transfer/outbound/upload_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/utils.py` & `b2sdk-1.9.0/b2sdk/utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v0/__init__.py` & `b2sdk-1.9.0/b2sdk/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v0/account_info.py` & `b2sdk-1.9.0/b2sdk/v0/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v0/api.py` & `b2sdk-1.9.0/b2sdk/v0/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v0/bucket.py` & `b2sdk-1.9.0/b2sdk/v0/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v0/sync.py` & `b2sdk-1.9.0/b2sdk/v0/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
     def __init__(self, *args, **kwargs):
         try:
             super(Synchronizer, self).__init__(*args, **kwargs)
         except InvalidArgument as e:
             raise CommandError('--%s %s' % (e.parameter_name, e.message))
 
-    def make_file_sync_actions(self, *args, **kwargs):
+    def _make_file_sync_actions(self, *args, **kwargs):
         try:
-            for i in super(Synchronizer, self).make_file_sync_actions(*args, **kwargs):
+            for i in super(Synchronizer, self)._make_file_sync_actions(*args, **kwargs):
                 yield i
         except DestFileNewerV1 as e:
             raise DestFileNewer(e.dest_file, e.source_file, e.dest_prefix, e.source_prefix)
 
     def sync_folders(self, *args, **kwargs):
         try:
             super(Synchronizer, self).sync_folders(*args, **kwargs)
```

### Comparing `b2sdk-1.8.0/b2sdk/v1/__init__.py` & `b2sdk-1.9.0/b2sdk/v1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 from b2sdk._v2 import *  # noqa
 from b2sdk.v1.account_info import (
     AbstractAccountInfo, InMemoryAccountInfo, UrlPoolAccountInfo, SqliteAccountInfo, StubAccountInfo
 )
 from b2sdk.v1.api import B2Api
 from b2sdk.v1.bucket import Bucket, BucketFactory
 from b2sdk.v1.cache import AbstractCache
+from b2sdk.v1.exception import CommandError, DestFileNewer
 from b2sdk.v1.file_version import FileVersionInfo
 from b2sdk.v1.session import B2Session
 from b2sdk.v1.sync import (
     ScanPoliciesManager, DEFAULT_SCAN_MANAGER, zip_folders, Synchronizer, AbstractFolder,
-    LocalFolder, B2Folder, parse_sync_folder
+    LocalFolder, B2Folder, parse_sync_folder, File, B2File, FileVersion,
+    AbstractSyncEncryptionSettingsProvider
 )
```

### Comparing `b2sdk-1.8.0/b2sdk/v1/account_info.py` & `b2sdk-1.9.0/b2sdk/v1/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v1/api.py` & `b2sdk-1.9.0/b2sdk/v1/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 from b2sdk import _v2 as v2
 from .bucket import Bucket, BucketFactory
+from .file_version import FileVersionInfo, FileVersionInfoFactory, file_version_info_from_id_and_name
 from .session import B2Session
 
 
 # override to use legacy no-request method of creating a bucket from bucket_id and retain `check_bucket_restrictions`
 # public API method
 # and to use v1.Bucket
+# and to retain cancel_large_file return type
 class B2Api(v2.B2Api):
     SESSION_CLASS = staticmethod(B2Session)
     BUCKET_FACTORY_CLASS = staticmethod(BucketFactory)
     BUCKET_CLASS = staticmethod(Bucket)
+    FILE_VERSION_FACTORY_CLASS = staticmethod(FileVersionInfoFactory)
 
     def get_bucket_by_id(self, bucket_id):
         """
         Return a bucket object with a given ID.  Unlike ``get_bucket_by_name``, this method does not need to make any API calls.
 
         :param str bucket_id: a bucket ID
         :return: a Bucket object
@@ -38,7 +41,11 @@
         If it does, checks if the bucket_name for a given api call matches that.
         If not, it raises a :py:exc:`b2sdk.v1.exception.RestrictedBucket` error.
 
         :param str bucket_name: a bucket name
         :raises b2sdk.v1.exception.RestrictedBucket: if the account is not allowed to use this bucket
         """
         self.check_bucket_name_restrictions(bucket_name)
+
+    def cancel_large_file(self, file_id: str) -> FileVersionInfo:
+        file_id_and_name = super().cancel_large_file(file_id)
+        return file_version_info_from_id_and_name(file_id_and_name, self)
```

### Comparing `b2sdk-1.8.0/b2sdk/v1/bucket.py` & `b2sdk-1.9.0/b2sdk/v1/bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
+from .file_version import FileVersionInfoFactory
 from typing import Optional
-
-from .file_version import translate_single_file_version, FileVersionInfoFactory
 from b2sdk import _v2 as v2
 from b2sdk.utils import validate_b2_file_name
 
 
 # Overridden to retain the obsolete copy_file and start_large_file methods
+# and to return old style FILE_VERSION_FACTORY attribute
 class Bucket(v2.Bucket):
     FILE_VERSION_FACTORY = staticmethod(FileVersionInfoFactory)
 
     def copy_file(
         self,
         file_id,
         new_file_name,
@@ -85,14 +85,10 @@
             file_name,
             content_type=content_type,
             file_info=file_info,
             file_retention=file_retention,
             legal_hold=legal_hold,
         )
 
-    create_file = translate_single_file_version(v2.Bucket.create_file)
-    create_file_stream = translate_single_file_version(v2.Bucket.create_file_stream)
-    copy = translate_single_file_version(v2.Bucket.copy)
-
 
 class BucketFactory(v2.BucketFactory):
     BUCKET_CLASS = staticmethod(Bucket)
```

### Comparing `b2sdk-1.8.0/b2sdk/v1/cache.py` & `b2sdk-1.9.0/b2sdk/v1/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v1/session.py` & `b2sdk-1.9.0/b2sdk/v1/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/v1/sync/folder.py` & `b2sdk-1.9.0/b2sdk/v1/sync/folder.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 ######################################################################
 
 from abc import abstractmethod
 import functools
 
 from b2sdk import _v2 as v2
-from .scan_policies import DEFAULT_SCAN_MANAGER
+from .scan_policies import DEFAULT_SCAN_MANAGER, wrap_if_necessary
 from .. import exception
 
 
 def translate_errors(func):
     @functools.wraps(func)
     def wrapper(*a, **kw):
         try:
@@ -36,20 +36,28 @@
 # Override to change "policies_manager" default argument
 class AbstractFolder(v2.AbstractFolder):
     @abstractmethod
     def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
         pass
 
 
+# override to retain "policies_manager" default argument,
+# and wrap policies_manager
 class B2Folder(v2.B2Folder, AbstractFolder):
-    pass
+    def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
+        return super().all_files(reporter, wrap_if_necessary(policies_manager))
 
 
-# "policies_manager" default argument and translate nice errors to old style Exceptions and CommandError
+# override to retain "policies_manager" default argument,
+# translate nice errors to old style Exceptions and CommandError
+# and wrap policies_manager
 class LocalFolder(v2.LocalFolder, AbstractFolder):
     @translate_errors
     def ensure_present(self):
         return super().ensure_present()
 
     @translate_errors
     def ensure_non_empty(self):
         return super().ensure_non_empty()
+
+    def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
+        return super().all_files(reporter, wrap_if_necessary(policies_manager))
```

### Comparing `b2sdk-1.8.0/b2sdk/v1/sync/folder_parser.py` & `b2sdk-1.9.0/b2sdk/v1/sync/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/version.py` & `b2sdk-1.9.0/b2sdk/version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk/version_utils.py` & `b2sdk-1.9.0/b2sdk/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/b2sdk.egg-info/PKG-INFO` & `b2sdk-1.9.0/b2sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Backblaze B2 SDK
 Home-page: https://github.com/Backblaze/b2-sdk-python
 Author: Backblaze, Inc.
 Author-email: support@backblaze.com
 License: MIT
-Description: # B2 Python SDK
-        &nbsp;[![Continuous Integration](https://github.com/Backblaze/b2-sdk-python/workflows/Continuous%20Integration/badge.svg)](https://github.com/Backblaze/b2-sdk-python/actions?query=workflow%3A%22Continuous+Integration%22)&nbsp;[![License](https://img.shields.io/pypi/l/b2sdk.svg?label=License)](https://pypi.python.org/pypi/b2)&nbsp;[![python versions](https://img.shields.io/pypi/pyversions/b2sdk.svg?label=python%20versions)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![PyPI version](https://img.shields.io/pypi/v/b2sdk.svg?label=PyPI%20version)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![Docs](https://readthedocs.org/projects/b2-sdk-python/badge/?version=master)](https://b2-sdk-python.readthedocs.io/en/master/)
-        
-        
-        
-        This repository contains a client library and a few handy utilities for easy access to all of the capabilities of B2 Cloud Storage.
-        
-        [B2 command-line tool](https://github.com/Backblaze/B2_Command_Line_Tool) is an example of how it can be used to provide command-line access to the B2 service, but there are many possible applications (including FUSE filesystems, storage backend drivers for backup applications etc).
-        
-        # Documentation
-        
-        The latest documentation is available on [Read the Docs](https://b2-sdk-python.readthedocs.io).
-        
-        # Installation
-        
-        The sdk can be installed with:
-        
-            pip install b2sdk
-        
-        # Version policy
-        
-        b2sdk follows [Semantic Versioning](https://semver.org/) policy, so in essence the version number is MAJOR.MINOR.PATCH (for example 1.2.3) and:
-        - we increase MAJOR version when we make incompatible API changes
-        - we increase MINOR version when we add functionality in a backwards-compatible manner, and
-        - we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
-        
-        Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
-        
-        ```
-        b2sdk>=0.0.0,<1.0.0
-        ```
-        
-        # Release History
-        
-        Please refer to the [changelog](CHANGELOG.md).
-        
-        # Developer Info
-        
-        Please see our [contributing guidelines](CONTRIBUTING.md).
-        
 Keywords: backblaze b2 cloud storage
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
+License-File: LICENSE
+
+# B2 Python SDK
+&nbsp;[![Continuous Integration](https://github.com/Backblaze/b2-sdk-python/workflows/Continuous%20Integration/badge.svg)](https://github.com/Backblaze/b2-sdk-python/actions?query=workflow%3A%22Continuous+Integration%22)&nbsp;[![License](https://img.shields.io/pypi/l/b2sdk.svg?label=License)](https://pypi.python.org/pypi/b2)&nbsp;[![python versions](https://img.shields.io/pypi/pyversions/b2sdk.svg?label=python%20versions)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![PyPI version](https://img.shields.io/pypi/v/b2sdk.svg?label=PyPI%20version)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![Docs](https://readthedocs.org/projects/b2-sdk-python/badge/?version=master)](https://b2-sdk-python.readthedocs.io/en/master/)
+
+
+
+This repository contains a client library and a few handy utilities for easy access to all of the capabilities of B2 Cloud Storage.
+
+[B2 command-line tool](https://github.com/Backblaze/B2_Command_Line_Tool) is an example of how it can be used to provide command-line access to the B2 service, but there are many possible applications (including FUSE filesystems, storage backend drivers for backup applications etc).
+
+# Documentation
+
+The latest documentation is available on [Read the Docs](https://b2-sdk-python.readthedocs.io).
+
+# Installation
+
+The sdk can be installed with:
+
+    pip install b2sdk
+
+# Version policy
+
+b2sdk follows [Semantic Versioning](https://semver.org/) policy, so in essence the version number is MAJOR.MINOR.PATCH (for example 1.2.3) and:
+- we increase MAJOR version when we make incompatible API changes
+- we increase MINOR version when we add functionality in a backwards-compatible manner, and
+- we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
+
+Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
+
+```
+b2sdk>=0.0.0,<1.0.0
+```
+
+# Release History
+
+Please refer to the [changelog](CHANGELOG.md).
+
+# Developer Info
+
+Please see our [contributing guidelines](CONTRIBUTING.md).
+
+
```

### Comparing `b2sdk-1.8.0/b2sdk.egg-info/SOURCES.txt` & `b2sdk-1.9.0/b2sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 b2sdk/stream/progress.py
 b2sdk/stream/range.py
 b2sdk/stream/wrapper.py
 b2sdk/sync/__init__.py
 b2sdk/sync/action.py
 b2sdk/sync/encryption_provider.py
 b2sdk/sync/exception.py
-b2sdk/sync/file.py
 b2sdk/sync/folder.py
 b2sdk/sync/folder_parser.py
+b2sdk/sync/path.py
 b2sdk/sync/policy.py
 b2sdk/sync/policy_manager.py
 b2sdk/sync/report.py
 b2sdk/sync/scan_policies.py
 b2sdk/sync/sync.py
 b2sdk/transfer/__init__.py
 b2sdk/transfer/emerge/__init__.py
@@ -113,14 +113,17 @@
 b2sdk/v1/api.py
 b2sdk/v1/bucket.py
 b2sdk/v1/cache.py
 b2sdk/v1/exception.py
 b2sdk/v1/file_version.py
 b2sdk/v1/session.py
 b2sdk/v1/sync/__init__.py
+b2sdk/v1/sync/encryption_provider.py
+b2sdk/v1/sync/file.py
+b2sdk/v1/sync/file_to_path_translator.py
 b2sdk/v1/sync/folder.py
 b2sdk/v1/sync/folder_parser.py
 b2sdk/v1/sync/scan_policies.py
 b2sdk/v1/sync/sync.py
 contrib/color-b2-logs.sh
 contrib/debug_logs.ini
 doc/bash_completion.md
@@ -162,17 +165,17 @@
 doc/source/api/internal/stream/chained.rst
 doc/source/api/internal/stream/hashing.rst
 doc/source/api/internal/stream/progress.rst
 doc/source/api/internal/stream/range.rst
 doc/source/api/internal/stream/wrapper.rst
 doc/source/api/internal/sync/action.rst
 doc/source/api/internal/sync/exception.rst
-doc/source/api/internal/sync/file.rst
 doc/source/api/internal/sync/folder.rst
 doc/source/api/internal/sync/folder_parser.rst
+doc/source/api/internal/sync/path.rst
 doc/source/api/internal/sync/policy.rst
 doc/source/api/internal/sync/policy_manager.rst
 doc/source/api/internal/sync/scan_policies.rst
 doc/source/api/internal/sync/sync.rst
 doc/source/api/internal/transfer/inbound/download_manager.rst
 doc/source/api/internal/transfer/inbound/file_metadata.rst
 doc/source/api/internal/transfer/inbound/downloader/abstract.rst
@@ -193,14 +196,18 @@
 test/unit/test_base.py
 test/unit/test_exception.py
 test/unit/test_session.py
 test/unit/account_info/__init__.py
 test/unit/account_info/fixtures.py
 test/unit/account_info/test_account_info.py
 test/unit/account_info/test_sqlite_account_info.py
+test/unit/api/__init__.py
+test/unit/api/test_api.py
+test/unit/bucket/__init__.py
+test/unit/bucket/test_bucket.py
 test/unit/file_lock/__init__.py
 test/unit/file_lock/test_legal_hold.py
 test/unit/file_version/__init__.py
 test/unit/file_version/test_file_version.py
 test/unit/fixtures/__init__.py
 test/unit/fixtures/b2http.py
 test/unit/fixtures/cache.py
@@ -213,15 +220,14 @@
 test/unit/sync/fixtures.py
 test/unit/sync/test_exception.py
 test/unit/sync/test_scan_policies.py
 test/unit/sync/test_sync.py
 test/unit/v0/__init__.py
 test/unit/v0/deps.py
 test/unit/v0/deps_exception.py
-test/unit/v0/test_api.py
 test/unit/v0/test_b2http.py
 test/unit/v0/test_bounded_queue_executor.py
 test/unit/v0/test_bucket.py
 test/unit/v0/test_copy_manager.py
 test/unit/v0/test_download_dest.py
 test/unit/v0/test_file_metadata.py
 test/unit/v0/test_policy.py
@@ -235,18 +241,16 @@
 test/unit/v0/test_version_utils.py
 test/unit/v0/apiver/__init__.py
 test/unit/v0/apiver/apiver_deps.py
 test/unit/v0/apiver/apiver_deps_exception.py
 test/unit/v1/__init__.py
 test/unit/v1/deps.py
 test/unit/v1/deps_exception.py
-test/unit/v1/test_api.py
 test/unit/v1/test_b2http.py
 test/unit/v1/test_bounded_queue_executor.py
-test/unit/v1/test_bucket.py
 test/unit/v1/test_copy_manager.py
 test/unit/v1/test_download_dest.py
 test/unit/v1/test_file_metadata.py
 test/unit/v1/test_policy.py
 test/unit/v1/test_progress.py
 test/unit/v1/test_raw_api.py
 test/unit/v1/test_scan_policies.py
```

### Comparing `b2sdk-1.8.0/contrib/debug_logs.ini` & `b2sdk-1.9.0/contrib/debug_logs.ini`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/bash_completion.md` & `b2sdk-1.9.0/doc/bash_completion.md`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/markup-test.rst` & `b2sdk-1.9.0/doc/markup-test.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/advanced.rst` & `b2sdk-1.9.0/doc/source/advanced.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/api/account_info.rst` & `b2sdk-1.9.0/doc/source/api/account_info.rst`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
       The constructor takes no parameters.
 
 
 SqliteAccountInfo
 =================
 
 .. autoclass:: b2sdk.v1.SqliteAccountInfo()
+   :inherited-members:
    :no-members:
    :special-members: __init__
 
    Implements all methods of :ref:`AccountInfo interface <account_info_interface>`.
 
    Uses a `SQLite database <https://www.sqlite.org/index.html>`_ for persistence
    and access synchronization between multiple processes. Not suitable for usage over NFS.
@@ -86,26 +87,29 @@
 
 .. _account_info_interface:
 
 AccountInfo interface
 =====================
 
 .. autoclass:: b2sdk.v1.AbstractAccountInfo()
+   :inherited-members:
    :private-members:
    :exclude-members: _abc_cache, _abc_negative_cache, _abc_negative_cache_version, _abc_registry
 
 
 AccountInfo helper classes
 ==========================
 
 .. autoclass:: b2sdk.v1.UrlPoolAccountInfo()
+   :inherited-members:
    :no-members:
    :members: BUCKET_UPLOAD_POOL_CLASS, LARGE_FILE_UPLOAD_POOL_CLASS
 
    .. caution::
       This class is not part of the public interface. To find out how to safely use it, read :ref:`this <semantic_versioning>`.
 
 .. autoclass:: b2sdk.account_info.upload_url_pool.UploadUrlPool()
+   :inherited-members:
    :private-members:
 
    .. caution::
       This class is not part of the public interface. To find out how to safely use it, read :ref:`this <semantic_versioning>`.
```

### Comparing `b2sdk-1.8.0/doc/source/api/download_dest.rst` & `b2sdk-1.9.0/doc/source/api/download_dest.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Download destination
 ==================================================
 
 .. note::
    Concrete classes described in this chapter implement methods defined in ``AbstractDownloadDestination``
 
 .. autoclass:: b2sdk.v1.AbstractDownloadDestination
+   :inherited-members:
    :members:
 
 .. autoclass:: b2sdk.v1.DownloadDestLocalFile()
    :no-members:
    :special-members: __init__
 
 .. autoclass:: b2sdk.v1.DownloadDestBytes
```

### Comparing `b2sdk-1.8.0/doc/source/api/file_lock.rst` & `b2sdk-1.9.0/doc/source/api/file_lock.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     :special-members: ON, OFF, UNSET, UNKNOWN, is_on, is_off, is_unknown
 
 .. autoclass:: b2sdk.v1.FileRetentionSetting()
     :no-members:
     :special-members: __init__
 
 .. autoclass:: b2sdk.v1.RetentionMode()
+    :inherited-members:
     :members:
 
 .. autoclass:: b2sdk.v1.BucketRetentionSetting()
     :no-members:
     :special-members: __init__
 
 .. autoclass:: b2sdk.v1.RetentionPeriod()
+    :inherited-members:
     :special-members: __init__
 
 .. autoclass:: b2sdk.v1.FileLockConfiguration()
     :no-members:
     :special-members: __init__
 
 .. autoclass:: b2sdk.v1.UNKNOWN_BUCKET_RETENTION()
```

### Comparing `b2sdk-1.8.0/doc/source/api/progress.rst` & `b2sdk-1.9.0/doc/source/api/progress.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 .. todo::
    improve documentation of progress reporters
 
    include info about sync progress
 
 .. autoclass:: b2sdk.v1.AbstractProgressListener
+   :inherited-members:
    :members:
 
 .. autoclass:: b2sdk.v1.TqdmProgressListener
    :no-members:
 
 .. autoclass:: b2sdk.v1.SimpleProgressListener
    :no-members:
```

### Comparing `b2sdk-1.8.0/doc/source/api/sync.rst` & `b2sdk-1.9.0/doc/source/api/sync.rst`

 * *Files 7% similar despite different names*

```diff
@@ -195,33 +195,37 @@
 and :ref:`encryption_provider` for public API.
 
 
 Public API classes
 ==================
 
 .. autoclass:: b2sdk.v1.ScanPoliciesManager()
+   :inherited-members:
    :special-members: __init__
    :members:
 
 .. autoclass:: b2sdk.v1.Synchronizer()
+   :inherited-members:
    :special-members: __init__
    :members:
 
 .. autoclass:: b2sdk.v1.SyncReport()
+   :inherited-members:
    :special-members: __init__
    :members:
 
 
 .. _encryption_provider:
 
 Sync Encryption Settings Providers
 ==================================
 
 
 .. autoclass:: b2sdk.v1.AbstractSyncEncryptionSettingsProvider()
+   :inherited-members:
    :members:
 
 
 .. autoclass:: b2sdk.v1.ServerDefaultSyncEncryptionSettingsProvider()
    :no-members:
```

### Comparing `b2sdk-1.8.0/doc/source/api_reference.rst` & `b2sdk-1.9.0/doc/source/api_reference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
    api/internal/stream/chained
    api/internal/stream/hashing
    api/internal/stream/progress
    api/internal/stream/range
    api/internal/stream/wrapper
    api/internal/sync/action
    api/internal/sync/exception
-   api/internal/sync/file
    api/internal/sync/folder
    api/internal/sync/folder_parser
+   api/internal/sync/path
    api/internal/sync/policy
    api/internal/sync/policy_manager
    api/internal/sync/scan_policies
    api/internal/sync/sync
    api/internal/transfer/inbound/downloader/abstract
    api/internal/transfer/inbound/downloader/parallel
    api/internal/transfer/inbound/downloader/range
```

### Comparing `b2sdk-1.8.0/doc/source/api_types.rst` & `b2sdk-1.9.0/doc/source/api_types.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/conf.py` & `b2sdk-1.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/contributing.rst` & `b2sdk-1.9.0/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/dot/sqlite_account_info_schema.dot` & `b2sdk-1.9.0/doc/source/dot/sqlite_account_info_schema.dot`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/glossary.rst` & `b2sdk-1.9.0/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/index.rst` & `b2sdk-1.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/install.rst` & `b2sdk-1.9.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/quick_start.rst` & `b2sdk-1.9.0/doc/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/server_side_encryption.rst` & `b2sdk-1.9.0/doc/source/server_side_encryption.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/source/tutorial.rst` & `b2sdk-1.9.0/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/doc/sqlite_account_info_schema.py` & `b2sdk-1.9.0/doc/sqlite_account_info_schema.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/noxfile.py` & `b2sdk-1.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/setup.cfg` & `b2sdk-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/setup.py` & `b2sdk-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/integration/test_raw_api.py` & `b2sdk-1.9.0/test/integration/test_raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/static/test_licenses.py` & `b2sdk-1.9.0/test/static/test_licenses.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/account_info/fixtures.py` & `b2sdk-1.9.0/test/unit/account_info/fixtures.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/account_info/test_account_info.py` & `b2sdk-1.9.0/test/unit/account_info/test_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/account_info/test_sqlite_account_info.py` & `b2sdk-1.9.0/test/unit/account_info/test_sqlite_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/conftest.py` & `b2sdk-1.9.0/test/unit/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,14 +104,30 @@
                pytest.param(re.error, "invalid something", marks=pytest.mark.apiver(to_ver=1)),
            ],
        )
        def test_illegal_regex(self, exc_class, exc_msg):
            with pytest.raises(exc_class, match=exc_msg):
                error_raising_function()
 
+    If a test is merked with "apiver" multiple times, it will be skipped if at least one of the apiver conditions
+    cause it to be skipped. E.g. if a test module is marked with
+
+    .. code-block:: python
+
+       pytestmark = [pytest.mark.apiver(from_ver=1)]
+
+    and a test function is marked with
+
+    .. code-block:: python
+
+       @pytest.mark.apiver(to_ver=1)
+       def test_function(self):
+           ...
+
+    the test function will be run only for apiver=v1
     """
     for mark in item.iter_markers(name='apiver'):
         if mark.args and mark.kwargs:
             raise pytest.UsageError('apiver mark should not have both args and kwargs')
 
         int_ver = int(item.config.getoption('--api')[1:])
         if mark.args:
```

### Comparing `b2sdk-1.8.0/test/unit/file_lock/test_legal_hold.py` & `b2sdk-1.9.0/test/unit/file_lock/test_legal_hold.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/file_version/test_file_version.py` & `b2sdk-1.9.0/test/unit/file_version/test_file_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,26 @@
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import pytest
 
-from apiver_deps import FileVersionInfo
+import apiver_deps
+
+if apiver_deps.V <= 1:
+    from apiver_deps import FileVersionInfo as VFileVersion
+else:
+    from apiver_deps import FileVersion as VFileVersion
 
 
 class TestFileVersion:
     @pytest.mark.apiver(to_ver=1)
     def test_format_ls_entry(self):
-        file_version_info = FileVersionInfo(
+        file_version_info = VFileVersion(
             'a2', 'inner/a.txt', 200, 'text/plain', 'sha1', {}, 2000, 'upload'
         )
         expected_entry = (
             '                                                       '
             '                          a2  upload  1970-01-01  '
             '00:00:02        200  inner/a.txt'
         )
```

### Comparing `b2sdk-1.8.0/test/unit/fixtures/raw_api.py` & `b2sdk-1.9.0/test/unit/fixtures/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/fixtures/session.py` & `b2sdk-1.9.0/test/unit/fixtures/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/internal/test_base.py` & `b2sdk-1.9.0/test/unit/internal/test_base.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/internal/test_emerge_planner.py` & `b2sdk-1.9.0/test/unit/internal/test_emerge_planner.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/sync/test_exception.py` & `b2sdk-1.9.0/test/unit/sync/test_exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/sync/test_scan_policies.py` & `b2sdk-1.9.0/test/unit/sync/test_scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/sync/test_sync.py` & `b2sdk-1.9.0/test/unit/sync/test_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,37 @@
 
 
 class TestSynchronizer:
     class IllegalEnum(Enum):
         ILLEGAL = 5100
 
     @pytest.fixture(autouse=True)
-    def setup(self, folder_factory, mocker):
+    def setup(self, folder_factory, mocker, apiver):
         self.folder_factory = folder_factory
         self.local_folder_factory = partial(folder_factory, 'local')
         self.b2_folder_factory = partial(folder_factory, 'b2')
         self.reporter = mocker.MagicMock()
+        self.apiver = apiver
+
+    def _make_folder_sync_actions(self, synchronizer, *args, **kwargs):
+        if self.apiver in ['v0', 'v1']:
+            return synchronizer.make_folder_sync_actions(*args, **kwargs)
+        return synchronizer._make_folder_sync_actions(*args, **kwargs)
 
     def assert_folder_sync_actions(self, synchronizer, src_folder, dst_folder, expected_actions):
         """
         Checks the actions generated for one file.  The file may or may not
         exist at the source, and may or may not exist at the destination.
 
         The source and destination files may have multiple versions.
         """
+
         actions = list(
-            synchronizer.make_folder_sync_actions(
+            self._make_folder_sync_actions(
+                synchronizer,
                 src_folder,
                 dst_folder,
                 TODAY,
                 self.reporter,
             )
         )
         assert expected_actions == [str(a) for a in actions]
@@ -685,61 +693,76 @@
         src = self.folder_factory(src_type, ('a.txt', [200], 11))
         dst = self.folder_factory(dst_type, ('a.txt', [100], 10))
         self.assert_folder_sync_actions(synchronizer, src, dst, expected)
 
     # FIXME: rewrite this test to not use mock.call checks when all of Synchronizers tests are rewritten to test_bucket
     # style - i.e. with simulated api and fake files returned from methods. Then, checking EncryptionSetting used for
     # transmission will be done by the underlying simulator.
-    def test_encryption_b2_to_local(self, synchronizer_factory):
+    def test_encryption_b2_to_local(self, synchronizer_factory, apiver):
         local = self.local_folder_factory()
         remote = self.b2_folder_factory(('directory/b.txt', [100]))
         synchronizer = synchronizer_factory()
 
         encryption = object()
         bucket = mock.MagicMock()
         provider = TstEncryptionSettingsProvider(encryption, encryption)
         download_action = next(
             iter(
-                synchronizer.make_folder_sync_actions(
-                    remote, local, TODAY, self.reporter, encryption_settings_provider=provider
+                self._make_folder_sync_actions(
+                    synchronizer,
+                    remote,
+                    local,
+                    TODAY,
+                    self.reporter,
+                    encryption_settings_provider=provider
                 )
             )
         )
         with mock.patch.object(B2DownloadAction, '_ensure_directory_existence'):
             try:
                 download_action.do_action(bucket, self.reporter)
             except:
                 pass
 
         assert bucket.mock_calls == [
             mock.call.download_file_by_id('id_d_100', mock.ANY, mock.ANY, encryption=encryption),
         ]
 
-        assert provider.get_setting_for_download.mock_calls == [
-            mock.call(
+        if apiver in ['v0', 'v1']:
+            file_version_kwarg = 'file_version_info'
+        else:
+            file_version_kwarg = 'file_version'
+
+        provider.get_setting_for_download.assert_has_calls(
+            [mock.call(
                 bucket=bucket,
-                file_version_info=mock.ANY,
-            )
-        ]
+                **{file_version_kwarg: mock.ANY},
+            )]
+        )
 
     # FIXME: rewrite this test to not use mock.call checks when all of Synchronizers tests are rewritten to test_bucket
     # style - i.e. with simulated api and fake files returned from methods. Then, checking EncryptionSetting used for
     # transmission will be done by the underlying simulator.
     def test_encryption_local_to_b2(self, synchronizer_factory):
         local = self.local_folder_factory(('directory/a.txt', [100]))
         remote = self.b2_folder_factory()
         synchronizer = synchronizer_factory()
 
         encryption = object()
         bucket = mock.MagicMock()
         provider = TstEncryptionSettingsProvider(encryption, encryption)
         upload_action = next(
             iter(
-                synchronizer.make_folder_sync_actions(
-                    local, remote, TODAY, self.reporter, encryption_settings_provider=provider
+                self._make_folder_sync_actions(
+                    synchronizer,
+                    local,
+                    remote,
+                    TODAY,
+                    self.reporter,
+                    encryption_settings_provider=provider
                 )
             )
         )
         with mock.patch.object(UploadSourceLocalFile, 'check_path_and_get_size'):
             try:
                 upload_action.do_action(bucket, self.reporter)
             except:
@@ -763,27 +786,32 @@
                 length=10
             )
         ]
 
     # FIXME: rewrite this test to not use mock.call checks when all of Synchronizers tests are rewritten to test_bucket
     # style - i.e. with simulated api and fake files returned from methods. Then, checking EncryptionSetting used for
     # transmission will be done by the underlying simulator.
-    def test_encryption_b2_to_b2(self, synchronizer_factory):
+    def test_encryption_b2_to_b2(self, synchronizer_factory, apiver):
         src = self.b2_folder_factory(('directory/a.txt', [100]))
         dst = self.b2_folder_factory()
         synchronizer = synchronizer_factory()
 
         source_encryption = object()
         destination_encryption = object()
         bucket = mock.MagicMock()
         provider = TstEncryptionSettingsProvider(source_encryption, destination_encryption)
         copy_action = next(
             iter(
-                synchronizer.make_folder_sync_actions(
-                    src, dst, TODAY, self.reporter, encryption_settings_provider=provider
+                self._make_folder_sync_actions(
+                    synchronizer,
+                    src,
+                    dst,
+                    TODAY,
+                    self.reporter,
+                    encryption_settings_provider=provider
                 )
             )
         )
         copy_action.do_action(bucket, self.reporter)
 
         assert bucket.mock_calls == [
             mock.call.copy(
@@ -793,26 +821,35 @@
                 source_content_type='text/plain',
                 source_file_info={'in_b2': 'yes'},
                 progress_listener=mock.ANY,
                 source_encryption=source_encryption,
                 destination_encryption=destination_encryption
             )
         ]
+
+        if apiver in ['v0', 'v1']:
+            file_version_kwarg = 'source_file_version_info'
+            additional_kwargs = {'target_file_info': None}
+        else:
+            file_version_kwarg = 'source_file_version'
+            additional_kwargs = {}
+
         assert provider.get_source_setting_for_copy.mock_calls == [
             mock.call(
-                bucket='fake_bucket',
-                source_file_version_info=mock.ANY,
+                bucket=mock.ANY,
+                **{file_version_kwarg: mock.ANY},
             )
         ]
 
         assert provider.get_destination_setting_for_copy.mock_calls == [
             mock.call(
-                bucket='fake_bucket',
-                source_file_version_info=mock.ANY,
+                bucket=mock.ANY,
                 dest_b2_file_name='folder/directory/a.txt',
+                **additional_kwargs,
+                **{file_version_kwarg: mock.ANY},
             )
         ]
 
 
 class TstEncryptionSettingsProvider(AbstractSyncEncryptionSettingsProvider):
     def __init__(self, source_encryption_setting, destination_encryption_setting):
         self.get_setting_for_upload = mock.MagicMock(
```

### Comparing `b2sdk-1.8.0/test/unit/test_base.py` & `b2sdk-1.9.0/test/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/test_exception.py` & `b2sdk-1.9.0/test/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/test_session.py` & `b2sdk-1.9.0/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/deps.py` & `b2sdk-1.9.0/test/unit/v0/deps.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/deps_exception.py` & `b2sdk-1.9.0/test/unit/v0/deps_exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_b2http.py` & `b2sdk-1.9.0/test/unit/v0/test_b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_bounded_queue_executor.py` & `b2sdk-1.9.0/test/unit/v0/test_bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_bucket.py` & `b2sdk-1.9.0/test/unit/v0/test_bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_copy_manager.py` & `b2sdk-1.9.0/test/unit/v0/test_copy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_download_dest.py` & `b2sdk-1.9.0/test/unit/v0/test_download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_file_metadata.py` & `b2sdk-1.9.0/test/unit/v0/test_file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_policy.py` & `b2sdk-1.9.0/test/unit/v0/test_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 ######################################################################
 
 from unittest.mock import MagicMock
 
 from ..test_base import TestBase
 
-from .deps import File, FileVersion
+from .deps import FileVersionInfo
+from .deps import LocalSyncPath, B2SyncPath
 from .deps import B2Folder
 from .deps import make_b2_keep_days_actions
 
 
 class TestMakeB2KeepDaysActions(TestBase):
     def setUp(self):
         self.keep_days = 7
@@ -52,20 +53,30 @@
         # The one at date -3 will get deleted because the one before it is old.
         self.check_one_answer(
             True, [(1, -5, 'upload'), (2, -10, 'upload'), (3, -3, 'upload')],
             ['b2_delete(folder/a, 3, (old version))']
         )
 
     def check_one_answer(self, has_source, id_relative_date_action_list, expected_actions):
-        source_file = File('a', []) if has_source else None
+        source_file = LocalSyncPath('a', 'a', 100, 10) if has_source else None
         dest_file_versions = [
-            FileVersion(id_, 'a', self.today + relative_date * self.one_day_millis, action, 100)
-            for (id_, relative_date, action) in id_relative_date_action_list
+            FileVersionInfo(
+                id_=id_,
+                file_name='folder/' + 'a',
+                upload_timestamp=self.today + relative_date * self.one_day_millis,
+                action=action,
+                size=100,
+                file_info={},
+                content_type='text/plain',
+                content_sha1='content_sha1',
+            ) for (id_, relative_date, action) in id_relative_date_action_list
         ]
-        dest_file = File('a', dest_file_versions)
+        dest_file = B2SyncPath(
+            'a', selected_version=dest_file_versions[0], all_versions=dest_file_versions
+        ) if dest_file_versions else None
         bucket = MagicMock()
         api = MagicMock()
         api.get_bucket_by_name.return_value = bucket
         dest_folder = B2Folder('bucket-1', 'folder', api)
         actual_actions = list(
             make_b2_keep_days_actions(
                 source_file, dest_file, dest_folder, dest_folder, self.keep_days, self.today
```

### Comparing `b2sdk-1.8.0/test/unit/v0/test_progress.py` & `b2sdk-1.9.0/test/unit/v0/test_progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_raw_api.py` & `b2sdk-1.9.0/test/unit/v0/test_raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_scan_policies.py` & `b2sdk-1.9.0/test/unit/v0/test_scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_session.py` & `b2sdk-1.9.0/test/unit/v0/test_session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_sync.py` & `b2sdk-1.9.0/test/unit/v0/test_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import concurrent.futures as futures
 import os
 import platform
 import sys
 import threading
 import time
 import unittest
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, ANY
 
 import pytest
 
 from ..test_base import TestBase
 
 from .deps_exception import UnSyncableFilename, NotADirectory, UnableToCreateDirectory, EmptyDirectory, InvalidArgument, CommandError
 from .deps import FileVersionInfo
 from .deps import AbstractFolder, B2Folder, LocalFolder
-from .deps import File, FileVersion
+from .deps import LocalSyncPath, B2SyncPath
 from .deps import ScanPoliciesManager, DEFAULT_SCAN_MANAGER
 from .deps import BoundedQueueExecutor, make_folder_sync_actions, zip_folders
 from .deps import parse_sync_folder
 from .deps import TempDir
 
 DAY = 86400000  # milliseconds
 TODAY = DAY * 100  # an arbitrary reference time for testing
@@ -82,15 +82,15 @@
     ):
         raise NotImplementedError
 
     def all_files(self, policies_manager):
         return list(self.prepare_folder().all_files(self.reporter, policies_manager))
 
     def assert_filtered_files(self, scan_results, expected_scan_results):
-        self.assertEqual(expected_scan_results, list(f.name for f in scan_results))
+        self.assertEqual(expected_scan_results, list(f.relative_path for f in scan_results))
         self.reporter.local_access_error.assert_not_called()
 
     def test_exclusions(self):
         expected_list = [
             '.dot_file',
             'hello.',
             'hello/a/1',
@@ -302,37 +302,41 @@
         else:
             mod_time = int(round(TODAY / 1000))
         os.utime(path, (mod_time, mod_time))
 
     def test_slash_sorting(self):
         # '/' should sort between '.' and '0'
         folder = self.prepare_folder()
-        self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+        self.assertEqual(self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter)))
         self.reporter.local_access_error.assert_not_called()
 
     def test_broken_symlink(self):
         folder = self.prepare_folder(broken_symlink=True)
-        self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+        self.assertEqual(self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter)))
         self.reporter.local_access_error.assert_called_once_with(
             os.path.join(self.root_dir, 'bad_symlink')
         )
 
     def test_invalid_permissions(self):
         folder = self.prepare_folder(invalid_permissions=True)
         # tests differ depending on the user running them. "root" will
         # succeed in os.access(path, os.R_OK) even if the permissions of
         # the file are 0 as implemented on self._prepare_folder().
         # use-case: running test suite inside a docker container
         if not os.access(os.path.join(self.root_dir, self.NAMES[0]), os.R_OK):
-            self.assertEqual(self.NAMES[1:], list(f.name for f in folder.all_files(self.reporter)))
+            self.assertEqual(
+                self.NAMES[1:], list(f.relative_path for f in folder.all_files(self.reporter))
+            )
             self.reporter.local_permission_error.assert_called_once_with(
                 os.path.join(self.root_dir, self.NAMES[0])
             )
         else:
-            self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+            self.assertEqual(
+                self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter))
+            )
 
     def test_syncable_paths(self):
         syncable_paths = (
             ('test.txt', 'test.txt'), ('./a/test.txt', 'a/test.txt'),
             ('./a/../test.txt', 'test.txt')
         )
 
@@ -439,36 +443,31 @@
 
     def test_multiple_versions(self):
         # Test two files, to cover the yield within the loop, and the yield without.
         folder = self.prepare_folder(use_file_versions_info=True)
 
         self.assertEqual(
             [
-                "B2File(inner/a.txt, [B2FileVersion('a2', 'inner/a.txt', 2000, 'upload'), "
-                "B2FileVersion('a1', 'inner/a.txt', 1000, 'upload')])",
-                "B2File(inner/b.txt, [B2FileVersion('b2', 'inner/b.txt', 1999, 'upload'), "
-                "B2FileVersion('b1', 'inner/b.txt', 1001, 'upload')])",
+                "B2SyncPath(inner/a.txt, [('a2', 2000, 'upload'), ('a1', 1000, 'upload')])",
+                "B2SyncPath(inner/b.txt, [('b2', 1999, 'upload'), ('b1', 1001, 'upload')])"
             ], [
                 str(f) for f in folder.all_files(self.reporter)
-                if f.name in ('inner/a.txt', 'inner/b.txt')
+                if f.relative_path in ('inner/a.txt', 'inner/b.txt')
             ]
         )
 
     def test_exclude_modified_multiple_versions(self):
         polices_manager = ScanPoliciesManager(
             exclude_modified_before=1001, exclude_modified_after=1999
         )
         folder = self.prepare_folder(use_file_versions_info=True)
         self.assertEqual(
-            [
-                "B2File(inner/b.txt, [B2FileVersion('b2', 'inner/b.txt', 1999, 'upload'), "
-                "B2FileVersion('b1', 'inner/b.txt', 1001, 'upload')])",
-            ], [
+            ["B2SyncPath(inner/b.txt, [('b2', 1999, 'upload'), ('b1', 1001, 'upload')])"], [
                 str(f) for f in folder.all_files(self.reporter, policies_manager=polices_manager)
-                if f.name in ('inner/a.txt', 'inner/b.txt')
+                if f.relative_path in ('inner/a.txt', 'inner/b.txt')
             ]
         )
 
     def test_exclude_modified_all_versions(self):
         polices_manager = ScanPoliciesManager(
             exclude_modified_before=1500, exclude_modified_after=1500
         )
@@ -580,40 +579,73 @@
         for filename in filenames_to_test:
             self.bucket.ls.return_value = [
                 (FileVersionInfo('a1', filename, 1, 'text/plain', 'sha1', {}, 1000, 'upload'), '')
             ]
             list(b2_folder.all_files(self.reporter))
 
 
-class FakeFolder(AbstractFolder):
-    def __init__(self, f_type, files):
-        self.f_type = f_type
-        self.files = files
+class FakeLocalFolder(LocalFolder):
+    def __init__(self, local_sync_paths):
+        super().__init__('folder')
+        self.local_sync_paths = local_sync_paths
 
     def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
-        for single_file in self.files:
-            if single_file.name.endswith('/'):
-                if policies_manager.should_exclude_directory(single_file.name):
+        for single_path in self.local_sync_paths:
+            if single_path.relative_path.endswith('/'):
+                if policies_manager.should_exclude_b2_directory(single_path.relative_path):
                     continue
             else:
-                if policies_manager.should_exclude_file(single_file.name):
+                if policies_manager.should_exclude_local_path(single_path):
                     continue
-            yield single_file
-
-    def folder_type(self):
-        return self.f_type
+            yield single_path
 
     def make_full_path(self, name):
-        if self.f_type == 'local':
-            return '/dir/' + name
-        else:
-            return 'folder/' + name
+        return '/dir/' + name
+
+
+class FakeB2Folder(B2Folder):
+    def __init__(self, test_files):
+        self.file_versions = []
+        for test_file in test_files:
+            self.file_versions.extend(self.file_versions_from_file_tuples(*test_file))
+        super().__init__('test-bucket', 'folder', MagicMock())
 
-    def __str__(self):
-        return '%s(%s, %s)' % (self.__class__.__name__, self.f_type, self.make_full_path(''))
+    def get_file_versions(self):
+        yield from iter(self.file_versions)
+
+    @classmethod
+    def file_versions_from_file_tuples(cls, name, mod_times, size=10):
+        """
+        Makes FileVersion objects.
+
+        Positive modification times are uploads, and negative modification
+        times are hides.  It's a hack, but it works.
+
+        """
+        try:
+            mod_times = iter(mod_times)
+        except TypeError:
+            mod_times = [mod_times]
+        return [
+            FileVersionInfo(
+                id_='id_%s_%d' % (name[0], abs(mod_time)),
+                file_name='folder/' + name,
+                upload_timestamp=abs(mod_time),
+                action='upload' if 0 < mod_time else 'hide',
+                size=size,
+                file_info={'in_b2': 'yes'},
+                content_type='text/plain',
+                content_sha1='content_sha1',
+            ) for mod_time in mod_times
+        ]  # yapf disable
+
+    @classmethod
+    def sync_path_from_file_tuple(cls, name, mod_times, size=10):
+        file_versions = cls.file_versions_from_file_tuples(name, mod_times, size)
+        return B2SyncPath(name, file_versions[0], file_versions)
 
 
 class TestParseSyncFolder(TestBase):
     def test_b2_double_slash(self):
         self._check_one('B2Folder(my-bucket, folder/path)', 'b2://my-bucket/folder/path')
 
     def test_b2_no_double_slash(self):
@@ -716,51 +748,56 @@
 
         with pytest.raises(exception, match=msg):
             parse_sync_folder('b2://a//b', MagicMock())
 
 
 class TestZipFolders(TestSync):
     def test_empty(self):
-        folder_a = FakeFolder('b2', [])
-        folder_b = FakeFolder('b2', [])
+        folder_a = FakeB2Folder([])
+        folder_b = FakeB2Folder([])
         self.assertEqual([], list(zip_folders(folder_a, folder_b, self.reporter)))
 
     def test_one_empty(self):
-        file_a1 = File("a.txt", [FileVersion("a", "a", 100, "upload", 10)])
-        folder_a = FakeFolder('b2', [file_a1])
-        folder_b = FakeFolder('b2', [])
+        file_a1 = LocalSyncPath("a.txt", "a.txt", 100, 10)
+        folder_a = FakeLocalFolder([file_a1])
+        folder_b = FakeB2Folder([])
         self.assertEqual([(file_a1, None)], list(zip_folders(folder_a, folder_b, self.reporter)))
 
     def test_two(self):
-        file_a1 = File("a.txt", [FileVersion("a", "a", 100, "upload", 10)])
-        file_a2 = File("b.txt", [FileVersion("b", "b", 100, "upload", 10)])
-        file_a3 = File("d.txt", [FileVersion("c", "c", 100, "upload", 10)])
-        file_a4 = File("f.txt", [FileVersion("f", "f", 100, "upload", 10)])
-        file_b1 = File("b.txt", [FileVersion("b", "b", 200, "upload", 10)])
-        file_b2 = File("e.txt", [FileVersion("e", "e", 200, "upload", 10)])
-        folder_a = FakeFolder('b2', [file_a1, file_a2, file_a3, file_a4])
-        folder_b = FakeFolder('b2', [file_b1, file_b2])
+        file_a1 = ("a.txt", 100, 10)
+        file_a2 = ("b.txt", 100, 10)
+        file_a3 = ("d.txt", 100, 10)
+        file_a4 = ("f.txt", 100, 10)
+        file_b1 = ("b.txt", 200, 10)
+        file_b2 = ("e.txt", 200, 10)
+        folder_a = FakeB2Folder([file_a1, file_a2, file_a3, file_a4])
+        folder_b = FakeB2Folder([file_b1, file_b2])
         self.assertEqual(
             [
-                (file_a1, None), (file_a2, file_b1), (file_a3, None), (None, file_b2),
-                (file_a4, None)
+                (FakeB2Folder.sync_path_from_file_tuple(*file_a1), None),
+                (
+                    FakeB2Folder.sync_path_from_file_tuple(*file_a2),
+                    FakeB2Folder.sync_path_from_file_tuple(*file_b1)
+                ), (FakeB2Folder.sync_path_from_file_tuple(*file_a3), None),
+                (None, FakeB2Folder.sync_path_from_file_tuple(*file_b2)),
+                (FakeB2Folder.sync_path_from_file_tuple(*file_a4), None)
             ], list(zip_folders(folder_a, folder_b, self.reporter))
         )
 
     def test_pass_reporter_to_folder(self):
         """
         Check that the zip_folders() function passes the reporter through
         to both folders.
         """
         folder_a = MagicMock()
         folder_b = MagicMock()
         folder_a.all_files = MagicMock(return_value=iter([]))
         folder_b.all_files = MagicMock(return_value=iter([]))
         self.assertEqual([], list(zip_folders(folder_a, folder_b, self.reporter)))
-        folder_a.all_files.assert_called_once_with(self.reporter, DEFAULT_SCAN_MANAGER)
+        folder_a.all_files.assert_called_once_with(self.reporter, ANY)
         folder_b.all_files.assert_called_once_with(self.reporter)
 
 
 class FakeArgs(object):
     """
     Can be passed to sync code to simulate command-line options.
     """
@@ -798,42 +835,41 @@
         self.excludeDirRegex = excludeDirRegex
         self.debugLogs = debugLogs
         self.dryRun = dryRun
         self.allowEmptySource = allowEmptySource
         self.excludeAllSymlinks = excludeAllSymlinks
 
 
-def local_file(name, mod_times, size=10):
+def local_file(name, mod_time, size=10):
     """
     Makes a File object for a b2 file, with one FileVersion for
     each modification time given in mod_times.
     """
-    versions = [
-        FileVersion('/dir/%s' % (name,), name, mod_time, 'upload', size) for mod_time in mod_times
-    ]
-    return File(name, versions)
+    return LocalSyncPath(name, name, mod_time, size)
 
 
 class TestExclusions(TestSync):
     def _check_folder_sync(self, expected_actions, fakeargs):
         # only local
-        file_a = local_file('a.txt', [100])
-        file_b = local_file('b.txt', [100])
-        file_d = local_file('d/d.txt', [100])
-        file_e = local_file('e/e.incl', [100])
+        file_a = ('a.txt', 100)
+        file_b = ('b.txt', 100)
+        file_d = ('d/d.txt', 100)
+        file_e = ('e/e.incl', 100)
 
         # both local and remote
-        file_bi = local_file('b.txt.incl', [100])
-        file_z = local_file('z.incl', [100])
+        file_bi = ('b.txt.incl', 100)
+        file_z = ('z.incl', 100)
 
         # only remote
-        file_c = local_file('c.txt', [100])
+        file_c = ('c.txt', 100)
 
-        local_folder = FakeFolder('local', [file_a, file_b, file_d, file_e, file_bi, file_z])
-        b2_folder = FakeFolder('b2', [file_bi, file_c, file_z])
+        local_folder = FakeLocalFolder(
+            [local_file(*f) for f in (file_a, file_b, file_d, file_e, file_bi, file_z)]
+        )
+        b2_folder = FakeB2Folder([file_bi, file_c, file_z])
 
         policies_manager = ScanPoliciesManager(
             exclude_dir_regexes=fakeargs.excludeDirRegex,
             exclude_file_regexes=fakeargs.excludeRegex,
             include_file_regexes=fakeargs.includeRegex,
             exclude_all_symlinks=fakeargs.excludeAllSymlinks
         )
@@ -843,26 +879,26 @@
             )
         )
         self.assertEqual(expected_actions, [str(a) for a in actions])
 
     def test_file_exclusions_with_delete(self):
         expected_actions = [
             'b2_upload(/dir/a.txt, folder/a.txt, 100)',
-            'b2_delete(folder/b.txt.incl, /dir/b.txt.incl, )',
-            'b2_delete(folder/c.txt, /dir/c.txt, )',
+            'b2_delete(folder/b.txt.incl, id_b_100, )',
+            'b2_delete(folder/c.txt, id_c_100, )',
             'b2_upload(/dir/d/d.txt, folder/d/d.txt, 100)',
             'b2_upload(/dir/e/e.incl, folder/e/e.incl, 100)',
         ]
         self._check_folder_sync(expected_actions, FakeArgs(delete=True, excludeRegex=["b\\.txt"]))
 
     def test_file_exclusions_inclusions_with_delete(self):
         expected_actions = [
             'b2_upload(/dir/a.txt, folder/a.txt, 100)',
-            'b2_delete(folder/b.txt.incl, /dir/b.txt.incl, )',
-            'b2_delete(folder/c.txt, /dir/c.txt, )',
+            'b2_delete(folder/b.txt.incl, id_b_100, )',
+            'b2_delete(folder/c.txt, id_c_100, )',
             'b2_upload(/dir/d/d.txt, folder/d/d.txt, 100)',
             'b2_upload(/dir/e/e.incl, folder/e/e.incl, 100)',
             'b2_upload(/dir/b.txt.incl, folder/b.txt.incl, 100)',
         ]
         fakeargs = FakeArgs(delete=True, excludeRegex=["b\\.txt"], includeRegex=[".*\\.incl"])
         self._check_folder_sync(expected_actions, fakeargs)
```

### Comparing `b2sdk-1.8.0/test/unit/v0/test_sync_report.py` & `b2sdk-1.9.0/test/unit/v0/test_sync_report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_utils.py` & `b2sdk-1.9.0/test/unit/v0/test_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v0/test_version_utils.py` & `b2sdk-1.9.0/test/unit/v0/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/deps.py` & `b2sdk-1.9.0/test/unit/v1/deps.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/deps_exception.py` & `b2sdk-1.9.0/test/unit/v1/deps_exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_b2http.py` & `b2sdk-1.9.0/test/unit/v1/test_b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_bounded_queue_executor.py` & `b2sdk-1.9.0/test/unit/v1/test_bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_bucket.py` & `b2sdk-1.9.0/test/unit/bucket/test_bucket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ######################################################################
 #
-# File: test/unit/v1/test_bucket.py
+# File: test/unit/bucket/test_bucket.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
@@ -13,42 +13,48 @@
 import platform
 import unittest.mock as mock
 
 import pytest
 
 from ..test_base import TestBase
 
-from .deps_exception import (
+from apiver_deps_exception import (
     AlreadyFailed,
     B2Error,
     B2RequestTimeoutDuringUpload,
     InvalidAuthToken,
     InvalidMetadataDirective,
     InvalidRange,
     InvalidUploadSource,
     MaxRetriesExceeded,
     UnsatisfiableRange,
     FileSha1Mismatch,
     SSECKeyError,
 )
-from .deps import B2Api
-from .deps import LargeFileUploadState
-from .deps import DownloadDestBytes, PreSeekedDownloadDest
-from .deps import FileVersionInfo
-from .deps import MetadataDirectiveMode
-from .deps import Part
-from .deps import AbstractProgressListener
-from .deps import StubAccountInfo, RawSimulator, BucketSimulator, FakeResponse, FileSimulator
-from .deps import ParallelDownloader
-from .deps import SimpleDownloader
-from .deps import UploadSourceBytes
-from .deps import hex_sha1_of_bytes, TempDir
-from .deps import EncryptionAlgorithm, EncryptionSetting, EncryptionMode, EncryptionKey, SSE_NONE, SSE_B2_AES
-from .deps import CopySource, UploadSourceLocalFile, WriteIntent
-from .deps import FileRetentionSetting, LegalHold, RetentionMode, NO_RETENTION_FILE_SETTING
+from apiver_deps import B2Api
+from apiver_deps import LargeFileUploadState
+from apiver_deps import DownloadDestBytes, PreSeekedDownloadDest
+from apiver_deps import MetadataDirectiveMode
+from apiver_deps import Part
+from apiver_deps import AbstractProgressListener
+from apiver_deps import StubAccountInfo, RawSimulator, BucketSimulator, FakeResponse, FileSimulator
+from apiver_deps import ParallelDownloader
+from apiver_deps import SimpleDownloader
+from apiver_deps import UploadSourceBytes
+from apiver_deps import hex_sha1_of_bytes, TempDir
+from apiver_deps import EncryptionAlgorithm, EncryptionSetting, EncryptionMode, EncryptionKey, SSE_NONE, SSE_B2_AES
+from apiver_deps import CopySource, UploadSourceLocalFile, WriteIntent
+from apiver_deps import FileRetentionSetting, LegalHold, RetentionMode, NO_RETENTION_FILE_SETTING
+import apiver_deps
+if apiver_deps.V <= 1:
+    from apiver_deps import FileVersionInfo as VFileVersionInfo
+else:
+    from apiver_deps import FileVersion as VFileVersionInfo
+
+pytestmark = [pytest.mark.apiver(from_ver=1)]
 
 SSE_C_AES = EncryptionSetting(
     mode=EncryptionMode.SSE_C,
     algorithm=EncryptionAlgorithm.AES256,
     key=EncryptionKey(secret=b'some_key', key_id='some-id'),
 )
 SSE_C_AES_NO_SECRET = EncryptionSetting(
@@ -207,18 +213,20 @@
                 raise InvalidAuthToken('message', 401)
 
         self.simulator.create_bucket = InvalidAuthTokenWrapper(self.simulator.create_bucket)
         self.bucket = self.api.create_bucket('your-bucket', 'allPublic')
 
 
 class TestListParts(TestCaseWithBucket):
+    @pytest.mark.apiver(to_ver=1)
     def testEmpty(self):
         file1 = self.bucket.start_large_file('file1.txt', 'text/plain', {})
         self.assertEqual([], list(self.bucket.list_parts(file1.file_id, batch_size=1)))
 
+    @pytest.mark.apiver(to_ver=1)
     def testThree(self):
         file1 = self.bucket.start_large_file('file1.txt', 'text/plain', {})
         content = b'hello world'
         content_sha1 = hex_sha1_of_bytes(content)
         large_file_upload_state = mock.MagicMock()
         large_file_upload_state.has_error.return_value = False
         self.api.services.upload_manager.upload_part(
@@ -235,14 +243,15 @@
             Part('9999', 2, 11, content_sha1),
             Part('9999', 3, 11, content_sha1),
         ]
         self.assertEqual(expected_parts, list(self.bucket.list_parts(file1.file_id, batch_size=1)))
 
 
 class TestUploadPart(TestCaseWithBucket):
+    @pytest.mark.apiver(to_ver=1)
     def test_error_in_state(self):
         file1 = self.bucket.start_large_file('file1.txt', 'text/plain', {})
         content = b'hello world'
         file_progress_listener = mock.MagicMock()
         large_file_upload_state = LargeFileUploadState(file_progress_listener)
         large_file_upload_state.set_error('test error')
         try:
@@ -255,26 +264,29 @@
             pass
 
 
 class TestListUnfinished(TestCaseWithBucket):
     def test_empty(self):
         self.assertEqual([], list(self.bucket.list_unfinished_large_files()))
 
+    @pytest.mark.apiver(to_ver=1)
     def test_one(self):
         file1 = self.bucket.start_large_file('file1.txt', 'text/plain', {})
         self.assertEqual([file1], list(self.bucket.list_unfinished_large_files()))
 
+    @pytest.mark.apiver(to_ver=1)
     def test_three(self):
         file1 = self.bucket.start_large_file('file1.txt', 'text/plain', {})
         file2 = self.bucket.start_large_file('file2.txt', 'text/plain', {})
         file3 = self.bucket.start_large_file('file3.txt', 'text/plain', {})
         self.assertEqual(
             [file1, file2, file3], list(self.bucket.list_unfinished_large_files(batch_size=1))
         )
 
+    @pytest.mark.apiver(to_ver=1)
     def test_prefix(self):
         self.bucket.start_large_file('fileA', 'text/plain', {})
         file2 = self.bucket.start_large_file('fileAB', 'text/plain', {})
         file3 = self.bucket.start_large_file('fileABC', 'text/plain', {})
         self.assertEqual(
             [file2, file3],
             list(self.bucket.list_unfinished_large_files(
@@ -290,15 +302,15 @@
 class TestGetFileInfo(TestCaseWithBucket):
     def test_version_by_name(self):
         data = b'hello world'
         a_id = self.bucket.upload_bytes(data, 'a').id_
 
         info = self.bucket.get_file_info_by_name('a')
 
-        self.assertIsInstance(info, FileVersionInfo)
+        self.assertIsInstance(info, VFileVersionInfo)
         expected = (
             a_id, 'a', 11, None, 'b2/x-auto', 'none', NO_RETENTION_FILE_SETTING, LegalHold.UNSET
         )
         actual = (
             info.id_,
             info.file_name,
             info.size,
@@ -349,15 +361,15 @@
 
     def test_version_by_id(self):
         data = b'hello world'
         b_id = self.bucket.upload_bytes(data, 'b').id_
 
         info = self.bucket.get_file_info_by_id(b_id)
 
-        self.assertIsInstance(info, FileVersionInfo)
+        self.assertIsInstance(info, VFileVersionInfo)
         expected = (b_id, 'b', 11, 'upload', 'b2/x-auto', 'none')
         actual = (
             info.id_, info.file_name, info.size, info.action, info.content_type,
             info.server_side_encryption.mode.value
         )
         self.assertEqual(expected, actual)
 
@@ -414,14 +426,15 @@
         ]
         actual = [
             (info.id_, info.file_name, info.size, info.action, folder)
             for (info, folder) in self.bucket.ls('bb', show_versions=True, fetch_count=1)
         ]
         self.assertEqual(expected, actual)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_started_large_file(self):
         self.bucket.start_large_file('hello.txt')
         expected = [('hello.txt', 0, 'start', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
     def test_hidden_file(self):
         data = b'hello world'
@@ -544,26 +557,29 @@
         self.assertEqual(SSE_B2_AES, actual)  # explicitly requested sse-b2
 
         actual = [info.server_side_encryption for info in self.bucket.list_file_versions('e')][0]
         self.assertEqual(SSE_C_AES_NO_SECRET, actual)  # explicitly requested sse-c
 
 
 class TestCopyFile(TestCaseWithBucket):
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_without_optional_params(self):
         file_id = self._make_file()
         self.bucket.copy_file(file_id, 'hello_new.txt')
         expected = [('hello.txt', 11, 'upload', None), ('hello_new.txt', 11, 'copy', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_range(self):
         file_id = self._make_file()
         self.bucket.copy_file(file_id, 'hello_new.txt', bytes_range=(3, 9))
         expected = [('hello.txt', 11, 'upload', None), ('hello_new.txt', 6, 'copy', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_invalid_metadata(self):
         file_id = self._make_file()
         try:
             self.bucket.copy_file(
                 file_id,
                 'hello_new.txt',
                 metadata_directive=MetadataDirectiveMode.COPY,
@@ -574,14 +590,15 @@
             self.assertEqual(
                 'content_type and file_info should be None when metadata_directive is COPY',
                 str(e),
             )
         expected = [('hello.txt', 11, 'upload', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_invalid_metadata_replace(self):
         file_id = self._make_file()
         try:
             self.bucket.copy_file(
                 file_id,
                 'hello_new.txt',
                 metadata_directive=MetadataDirectiveMode.REPLACE,
@@ -591,14 +608,15 @@
             self.assertEqual(
                 'content_type cannot be None when metadata_directive is REPLACE',
                 str(e),
             )
         expected = [('hello.txt', 11, 'upload', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_replace_metadata(self):
         file_id = self._make_file()
         self.bucket.copy_file(
             file_id,
             'hello_new.txt',
             metadata_directive=MetadataDirectiveMode.REPLACE,
             content_type='text/plain',
@@ -609,14 +627,15 @@
         ]
         actual = [
             (info.file_name, info.size, info.action, info.content_type, folder)
             for (info, folder) in self.bucket.ls(show_versions=True)
         ]
         self.assertEqual(expected, actual)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_unsatisfied_range(self):
         file_id = self._make_file()
         try:
             self.bucket.copy_file(
                 file_id,
                 'hello_new.txt',
                 bytes_range=(12, 15),
@@ -626,14 +645,15 @@
             self.assertEqual(
                 'The range in the request is outside the size of the file',
                 str(e),
             )
         expected = [('hello.txt', 11, 'upload', None)]
         self.assertBucketContents(expected, '', show_versions=True)
 
+    @pytest.mark.apiver(to_ver=1)
     def test_copy_with_different_bucket(self):
         source_bucket = self.api.create_bucket('source-bucket', 'allPublic')
         file_id = self._make_file(source_bucket)
         self.bucket.copy_file(file_id, 'hello_new.txt')
 
         def ls(bucket):
             return [
@@ -779,28 +799,28 @@
                         file_info={'new': 'value'},
                         content_type='text/plain'
                     ), SSE_C_AES_2_NO_SECRET
                 ),
             ]:
                 with self.subTest(kwargs=kwargs, length=length, data=data):
                     file_info = self.bucket.copy(**kwargs, new_file_name='new_file', length=length)
-                    self.assertTrue(isinstance(file_info, FileVersionInfo))
+                    self.assertTrue(isinstance(file_info, VFileVersionInfo))
                     self.assertEqual(file_info.server_side_encryption, expected_encryption)
 
     def _make_file(self, bucket=None):
         data = b'hello world'
         actual_bucket = bucket or self.bucket
         return actual_bucket.upload_bytes(data, 'hello.txt').id_
 
 
 class TestUpload(TestCaseWithBucket):
     def test_upload_bytes(self):
         data = b'hello world'
         file_info = self.bucket.upload_bytes(data, 'file1')
-        self.assertTrue(isinstance(file_info, FileVersionInfo))
+        self.assertTrue(isinstance(file_info, VFileVersionInfo))
         self._check_file_contents('file1', data)
         self.assertEqual(file_info.server_side_encryption, SSE_NONE)
 
     def test_upload_bytes_file_retention(self):
         data = b'hello world'
         retention = FileRetentionSetting(RetentionMode.COMPLIANCE, 150)
         file_info = self.bucket.upload_bytes(
@@ -809,40 +829,40 @@
         self._check_file_contents('file1', data)
         self.assertEqual(retention, file_info.file_retention)
         self.assertEqual(LegalHold.ON, file_info.legal_hold)
 
     def test_upload_bytes_sse_b2(self):
         data = b'hello world'
         file_info = self.bucket.upload_bytes(data, 'file1', encryption=SSE_B2_AES)
-        self.assertTrue(isinstance(file_info, FileVersionInfo))
+        self.assertTrue(isinstance(file_info, VFileVersionInfo))
         self.assertEqual(file_info.server_side_encryption, SSE_B2_AES)
 
     def test_upload_bytes_sse_c(self):
         data = b'hello world'
         file_info = self.bucket.upload_bytes(data, 'file1', encryption=SSE_C_AES)
-        self.assertTrue(isinstance(file_info, FileVersionInfo))
+        self.assertTrue(isinstance(file_info, VFileVersionInfo))
         self.assertEqual(SSE_C_AES_NO_SECRET, file_info.server_side_encryption)
 
     def test_upload_local_file_sse_b2(self):
         with TempDir() as d:
             path = os.path.join(d, 'file1')
             data = b'hello world'
             write_file(path, data)
             file_info = self.bucket.upload_local_file(path, 'file1', encryption=SSE_B2_AES)
-            self.assertTrue(isinstance(file_info, FileVersionInfo))
+            self.assertTrue(isinstance(file_info, VFileVersionInfo))
             self.assertEqual(file_info.server_side_encryption, SSE_B2_AES)
             self._check_file_contents('file1', data)
 
     def test_upload_local_file_sse_c(self):
         with TempDir() as d:
             path = os.path.join(d, 'file1')
             data = b'hello world'
             write_file(path, data)
             file_info = self.bucket.upload_local_file(path, 'file1', encryption=SSE_C_AES)
-            self.assertTrue(isinstance(file_info, FileVersionInfo))
+            self.assertTrue(isinstance(file_info, VFileVersionInfo))
             self.assertEqual(SSE_C_AES_NO_SECRET, file_info.server_side_encryption)
             self._check_file_contents('file1', data)
 
     def test_upload_local_file_retention(self):
         with TempDir() as d:
             path = os.path.join(d, 'file1')
             data = b'hello world'
@@ -868,15 +888,15 @@
     def test_upload_local_file(self):
         with TempDir() as d:
             path = os.path.join(d, 'file1')
             data = b'hello world'
             write_file(path, data)
             file_info = self.bucket.upload_local_file(path, 'file1')
             self._check_file_contents('file1', data)
-            self.assertTrue(isinstance(file_info, FileVersionInfo))
+            self.assertTrue(isinstance(file_info, VFileVersionInfo))
             self.assertEqual(file_info.server_side_encryption, SSE_NONE)
             print(file_info.as_dict())
             self.assertEqual(file_info.as_dict()['serverSideEncryption'], {'mode': 'none'})
 
     @pytest.mark.skipif(platform.system() == 'Windows', reason='no os.mkfifo() on Windows')
     def test_upload_fifo(self):
         with TempDir() as d:
@@ -1077,15 +1097,15 @@
                 [
                     CopySource(f1_id, length=len(data), offset=0),
                     UploadSourceLocalFile(path),
                     CopySource(f2_id, length=len(data), offset=0),
                 ],
                 file_name='created_file'
             )
-            self.assertIsInstance(created_file, FileVersionInfo)
+            self.assertIsInstance(created_file, VFileVersionInfo)
             actual = (
                 created_file.id_, created_file.file_name, created_file.size,
                 created_file.server_side_encryption
             )
             expected = ('9997', 'created_file', 33, SSE_NONE)
             self.assertEqual(expected, actual)
 
@@ -1102,15 +1122,15 @@
                         CopySource(f1_id, length=len(data), offset=0, encryption=SSE_C_AES),
                         UploadSourceLocalFile(path),
                         CopySource(f2_id, length=len(data), offset=0, encryption=SSE_C_AES_2),
                     ],
                     file_name='created_file_%s' % (len(data),),
                     encryption=SSE_C_AES
                 )
-            self.assertIsInstance(created_file, FileVersionInfo)
+            self.assertIsInstance(created_file, VFileVersionInfo)
             actual = (
                 created_file.id_, created_file.file_name, created_file.size,
                 created_file.server_side_encryption
             )
             expected = (
                 mock.ANY,
                 'created_file_%s' % (len(data),),
```

### Comparing `b2sdk-1.8.0/test/unit/v1/test_copy_manager.py` & `b2sdk-1.9.0/test/unit/v1/test_copy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_download_dest.py` & `b2sdk-1.9.0/test/unit/v1/test_download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_file_metadata.py` & `b2sdk-1.9.0/test/unit/v1/test_file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_policy.py` & `b2sdk-1.9.0/test/unit/v1/test_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 ######################################################################
 
 from unittest.mock import MagicMock
 
 from ..test_base import TestBase
 
-from .deps import File, FileVersion
+from .deps import FileVersionInfo
+from .deps import LocalSyncPath, B2SyncPath
 from .deps import B2Folder
 from .deps import make_b2_keep_days_actions
 
 
 class TestMakeB2KeepDaysActions(TestBase):
     def setUp(self):
         self.keep_days = 7
@@ -52,20 +53,30 @@
         # The one at date -3 will get deleted because the one before it is old.
         self.check_one_answer(
             True, [(1, -5, 'upload'), (2, -10, 'upload'), (3, -3, 'upload')],
             ['b2_delete(folder/a, 3, (old version))']
         )
 
     def check_one_answer(self, has_source, id_relative_date_action_list, expected_actions):
-        source_file = File('a', []) if has_source else None
+        source_file = LocalSyncPath('a', 'a', 100, 10) if has_source else None
         dest_file_versions = [
-            FileVersion(id_, 'a', self.today + relative_date * self.one_day_millis, action, 100)
-            for (id_, relative_date, action) in id_relative_date_action_list
+            FileVersionInfo(
+                id_=id_,
+                file_name='folder/' + 'a',
+                upload_timestamp=self.today + relative_date * self.one_day_millis,
+                action=action,
+                size=100,
+                file_info={},
+                content_type='text/plain',
+                content_sha1='content_sha1',
+            ) for (id_, relative_date, action) in id_relative_date_action_list
         ]
-        dest_file = File('a', dest_file_versions)
+        dest_file = B2SyncPath(
+            'a', selected_version=dest_file_versions[0], all_versions=dest_file_versions
+        ) if dest_file_versions else None
         bucket = MagicMock()
         api = MagicMock()
         api.get_bucket_by_name.return_value = bucket
         dest_folder = B2Folder('bucket-1', 'folder', api)
         actual_actions = list(
             make_b2_keep_days_actions(
                 source_file, dest_file, dest_folder, dest_folder, self.keep_days, self.today
```

### Comparing `b2sdk-1.8.0/test/unit/v1/test_progress.py` & `b2sdk-1.9.0/test/unit/v1/test_progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_raw_api.py` & `b2sdk-1.9.0/test/unit/v1/test_raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_scan_policies.py` & `b2sdk-1.9.0/test/unit/v1/test_scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_session.py` & `b2sdk-1.9.0/test/unit/v1/test_session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_sync.py` & `b2sdk-1.9.0/test/unit/v1/test_sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import concurrent.futures as futures
 import os
 import platform
 import sys
 import threading
 import time
 import unittest
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, ANY
 
 import pytest
 
 from ..test_base import TestBase
 
 from .deps import AbstractFolder, B2Folder, LocalFolder
 from .deps import BoundedQueueExecutor, zip_folders
-from .deps import File, FileVersion
+from .deps import LocalSyncPath, B2SyncPath
 from .deps import FileVersionInfo
 from .deps import KeepOrDeleteMode, NewerFileSyncMode, CompareVersionMode
 from .deps import ScanPoliciesManager, DEFAULT_SCAN_MANAGER
 from .deps import Synchronizer
 from .deps import TempDir
 from .deps import parse_sync_folder
 from .deps_exception import UnSyncableFilename, NotADirectory, UnableToCreateDirectory, EmptyDirectory, InvalidArgument, CommandError
@@ -84,15 +84,15 @@
     ):
         raise NotImplementedError
 
     def all_files(self, policies_manager):
         return list(self.prepare_folder().all_files(self.reporter, policies_manager))
 
     def assert_filtered_files(self, scan_results, expected_scan_results):
-        self.assertEqual(expected_scan_results, list(f.name for f in scan_results))
+        self.assertEqual(expected_scan_results, list(f.relative_path for f in scan_results))
         self.reporter.local_access_error.assert_not_called()
 
     def test_exclusions(self):
         expected_list = [
             '.dot_file',
             'hello.',
             'hello/a/1',
@@ -306,37 +306,41 @@
         else:
             mod_time = int(round(TODAY / 1000))
         os.utime(path, (mod_time, mod_time))
 
     def test_slash_sorting(self):
         # '/' should sort between '.' and '0'
         folder = self.prepare_folder()
-        self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+        self.assertEqual(self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter)))
         self.reporter.local_access_error.assert_not_called()
 
     def test_broken_symlink(self):
         folder = self.prepare_folder(broken_symlink=True)
-        self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+        self.assertEqual(self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter)))
         self.reporter.local_access_error.assert_called_once_with(
             os.path.join(self.root_dir, 'bad_symlink')
         )
 
     def test_invalid_permissions(self):
         folder = self.prepare_folder(invalid_permissions=True)
         # tests differ depending on the user running them. "root" will
         # succeed in os.access(path, os.R_OK) even if the permissions of
         # the file are 0 as implemented on self._prepare_folder().
         # use-case: running test suite inside a docker container
         if not os.access(os.path.join(self.root_dir, self.NAMES[0]), os.R_OK):
-            self.assertEqual(self.NAMES[1:], list(f.name for f in folder.all_files(self.reporter)))
+            self.assertEqual(
+                self.NAMES[1:], list(f.relative_path for f in folder.all_files(self.reporter))
+            )
             self.reporter.local_permission_error.assert_called_once_with(
                 os.path.join(self.root_dir, self.NAMES[0])
             )
         else:
-            self.assertEqual(self.NAMES, list(f.name for f in folder.all_files(self.reporter)))
+            self.assertEqual(
+                self.NAMES, list(f.relative_path for f in folder.all_files(self.reporter))
+            )
 
     def test_syncable_paths(self):
         syncable_paths = (
             ('test.txt', 'test.txt'), ('./a/test.txt', 'a/test.txt'),
             ('./a/../test.txt', 'test.txt')
         )
 
@@ -443,36 +447,31 @@
 
     def test_multiple_versions(self):
         # Test two files, to cover the yield within the loop, and the yield without.
         folder = self.prepare_folder(use_file_versions_info=True)
 
         self.assertEqual(
             [
-                "B2File(inner/a.txt, [B2FileVersion('a2', 'inner/a.txt', 2000, 'upload'), "
-                "B2FileVersion('a1', 'inner/a.txt', 1000, 'upload')])",
-                "B2File(inner/b.txt, [B2FileVersion('b2', 'inner/b.txt', 1999, 'upload'), "
-                "B2FileVersion('b1', 'inner/b.txt', 1001, 'upload')])",
+                "B2SyncPath(inner/a.txt, [('a2', 2000, 'upload'), ('a1', 1000, 'upload')])",
+                "B2SyncPath(inner/b.txt, [('b2', 1999, 'upload'), ('b1', 1001, 'upload')])"
             ], [
                 str(f) for f in folder.all_files(self.reporter)
-                if f.name in ('inner/a.txt', 'inner/b.txt')
+                if f.relative_path in ('inner/a.txt', 'inner/b.txt')
             ]
         )
 
     def test_exclude_modified_multiple_versions(self):
         polices_manager = ScanPoliciesManager(
             exclude_modified_before=1001, exclude_modified_after=1999
         )
         folder = self.prepare_folder(use_file_versions_info=True)
         self.assertEqual(
-            [
-                "B2File(inner/b.txt, [B2FileVersion('b2', 'inner/b.txt', 1999, 'upload'), "
-                "B2FileVersion('b1', 'inner/b.txt', 1001, 'upload')])",
-            ], [
+            ["B2SyncPath(inner/b.txt, [('b2', 1999, 'upload'), ('b1', 1001, 'upload')])"], [
                 str(f) for f in folder.all_files(self.reporter, policies_manager=polices_manager)
-                if f.name in ('inner/a.txt', 'inner/b.txt')
+                if f.relative_path in ('inner/a.txt', 'inner/b.txt')
             ]
         )
 
     def test_exclude_modified_all_versions(self):
         polices_manager = ScanPoliciesManager(
             exclude_modified_before=1500, exclude_modified_after=1500
         )
@@ -584,46 +583,73 @@
         for filename in filenames_to_test:
             self.bucket.ls.return_value = [
                 (FileVersionInfo('a1', filename, 1, 'text/plain', 'sha1', {}, 1000, 'upload'), '')
             ]
             list(b2_folder.all_files(self.reporter))
 
 
-class FakeFolder(AbstractFolder):
-    def __init__(self, f_type, files):
-        self.f_type = f_type
-        self.files = files
-
-    @property
-    def bucket_name(self):
-        if self.f_type != 'b2':
-            raise ValueError('FakeFolder with type!=b2 does not have a bucket name')
-        return 'fake_bucket_name'
+class FakeLocalFolder(LocalFolder):
+    def __init__(self, local_sync_paths):
+        super().__init__('folder')
+        self.local_sync_paths = local_sync_paths
 
     def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
-        for single_file in self.files:
-            if single_file.name.endswith('/'):
-                if policies_manager.should_exclude_directory(single_file.name):
+        for single_path in self.local_sync_paths:
+            if single_path.relative_path.endswith('/'):
+                if policies_manager.should_exclude_b2_directory(single_path.relative_path):
                     continue
             else:
-                if policies_manager.should_exclude_file(single_file.name):
+                if policies_manager.should_exclude_local_path(single_path):
                     continue
-            yield single_file
-
-    def folder_type(self):
-        return self.f_type
+            yield single_path
 
     def make_full_path(self, name):
-        if self.f_type == 'local':
-            return '/dir/' + name
-        else:
-            return 'folder/' + name
+        return '/dir/' + name
+
+
+class FakeB2Folder(B2Folder):
+    def __init__(self, test_files):
+        self.file_versions = []
+        for test_file in test_files:
+            self.file_versions.extend(self.file_versions_from_file_tuples(*test_file))
+        super().__init__('test-bucket', 'folder', MagicMock())
 
-    def __str__(self):
-        return '%s(%s, %s)' % (self.__class__.__name__, self.f_type, self.make_full_path(''))
+    def get_file_versions(self):
+        yield from iter(self.file_versions)
+
+    @classmethod
+    def file_versions_from_file_tuples(cls, name, mod_times, size=10):
+        """
+        Makes FileVersion objects.
+
+        Positive modification times are uploads, and negative modification
+        times are hides.  It's a hack, but it works.
+
+        """
+        try:
+            mod_times = iter(mod_times)
+        except TypeError:
+            mod_times = [mod_times]
+        return [
+            FileVersionInfo(
+                id_='id_%s_%d' % (name[0], abs(mod_time)),
+                file_name='folder/' + name,
+                upload_timestamp=abs(mod_time),
+                action='upload' if 0 < mod_time else 'hide',
+                size=size,
+                file_info={'in_b2': 'yes'},
+                content_type='text/plain',
+                content_sha1='content_sha1',
+            ) for mod_time in mod_times
+        ]  # yapf disable
+
+    @classmethod
+    def sync_path_from_file_tuple(cls, name, mod_times, size=10):
+        file_versions = cls.file_versions_from_file_tuples(name, mod_times, size)
+        return B2SyncPath(name, file_versions[0], file_versions)
 
 
 class TestParseSyncFolder(TestBase):
     def test_b2_double_slash(self):
         self._check_one('B2Folder(my-bucket, folder/path)', 'b2://my-bucket/folder/path')
 
     def test_b2_no_double_slash(self):
@@ -726,51 +752,56 @@
 
         with pytest.raises(exception, match=msg):
             parse_sync_folder('b2://a//b', MagicMock())
 
 
 class TestZipFolders(TestSync):
     def test_empty(self):
-        folder_a = FakeFolder('b2', [])
-        folder_b = FakeFolder('b2', [])
+        folder_a = FakeB2Folder([])
+        folder_b = FakeB2Folder([])
         self.assertEqual([], list(zip_folders(folder_a, folder_b, self.reporter)))
 
     def test_one_empty(self):
-        file_a1 = File("a.txt", [FileVersion("a", "a", 100, "upload", 10)])
-        folder_a = FakeFolder('b2', [file_a1])
-        folder_b = FakeFolder('b2', [])
+        file_a1 = LocalSyncPath("a.txt", "a.txt", 100, 10)
+        folder_a = FakeLocalFolder([file_a1])
+        folder_b = FakeB2Folder([])
         self.assertEqual([(file_a1, None)], list(zip_folders(folder_a, folder_b, self.reporter)))
 
     def test_two(self):
-        file_a1 = File("a.txt", [FileVersion("a", "a", 100, "upload", 10)])
-        file_a2 = File("b.txt", [FileVersion("b", "b", 100, "upload", 10)])
-        file_a3 = File("d.txt", [FileVersion("c", "c", 100, "upload", 10)])
-        file_a4 = File("f.txt", [FileVersion("f", "f", 100, "upload", 10)])
-        file_b1 = File("b.txt", [FileVersion("b", "b", 200, "upload", 10)])
-        file_b2 = File("e.txt", [FileVersion("e", "e", 200, "upload", 10)])
-        folder_a = FakeFolder('b2', [file_a1, file_a2, file_a3, file_a4])
-        folder_b = FakeFolder('b2', [file_b1, file_b2])
+        file_a1 = ("a.txt", [100], 10)
+        file_a2 = ("b.txt", [100], 10)
+        file_a3 = ("d.txt", [100], 10)
+        file_a4 = ("f.txt", [100], 10)
+        file_b1 = ("b.txt", [200], 10)
+        file_b2 = ("e.txt", [200], 10)
+        folder_a = FakeB2Folder([file_a1, file_a2, file_a3, file_a4])
+        folder_b = FakeB2Folder([file_b1, file_b2])
         self.assertEqual(
             [
-                (file_a1, None), (file_a2, file_b1), (file_a3, None), (None, file_b2),
-                (file_a4, None)
+                (FakeB2Folder.sync_path_from_file_tuple(*file_a1), None),
+                (
+                    FakeB2Folder.sync_path_from_file_tuple(*file_a2),
+                    FakeB2Folder.sync_path_from_file_tuple(*file_b1)
+                ), (FakeB2Folder.sync_path_from_file_tuple(*file_a3), None),
+                (None, FakeB2Folder.sync_path_from_file_tuple(*file_b2)),
+                (FakeB2Folder.sync_path_from_file_tuple(*file_a4), None)
             ], list(zip_folders(folder_a, folder_b, self.reporter))
         )
 
     def test_pass_reporter_to_folder(self):
         """
         Check that the zip_folders() function passes the reporter through
         to both folders.
         """
         folder_a = MagicMock()
         folder_b = MagicMock()
         folder_a.all_files = MagicMock(return_value=iter([]))
         folder_b.all_files = MagicMock(return_value=iter([]))
         self.assertEqual([], list(zip_folders(folder_a, folder_b, self.reporter)))
-        folder_a.all_files.assert_called_once_with(self.reporter, DEFAULT_SCAN_MANAGER)
+        folder_a.all_files.assert_called_once_with(self.reporter, ANY)
         folder_b.all_files.assert_called_once_with(self.reporter)
 
 
 class FakeArgs(object):
     """
     Can be passed to sync code to simulate command-line options.
     """
@@ -819,42 +850,40 @@
             keep_days_or_delete=self.keep_days_or_delete,
             keep_days=self.keep_days,
             compare_version_mode=self.compare_version_mode,
             compare_threshold=self.compare_threshold,
         )
 
 
-def local_file(name, mod_times, size=10):
+def local_file(name, mod_time, size=10):
     """
-    Makes a File object for a b2 file, with one FileVersion for
-    each modification time given in mod_times.
+    Makes a LocalSyncPath object for a b2 file.
     """
-    versions = [
-        FileVersion('/dir/%s' % (name,), name, mod_time, 'upload', size) for mod_time in mod_times
-    ]
-    return File(name, versions)
+    return LocalSyncPath(name, name, mod_time, size)
 
 
 class TestExclusions(TestSync):
     def _check_folder_sync(self, expected_actions, fakeargs):
         # only local
-        file_a = local_file('a.txt', [100])
-        file_b = local_file('b.txt', [100])
-        file_d = local_file('d/d.txt', [100])
-        file_e = local_file('e/e.incl', [100])
+        file_a = ('a.txt', 100)
+        file_b = ('b.txt', 100)
+        file_d = ('d/d.txt', 100)
+        file_e = ('e/e.incl', 100)
 
         # both local and remote
-        file_bi = local_file('b.txt.incl', [100])
-        file_z = local_file('z.incl', [100])
+        file_bi = ('b.txt.incl', 100)
+        file_z = ('z.incl', 100)
 
         # only remote
-        file_c = local_file('c.txt', [100])
+        file_c = ('c.txt', 100)
 
-        local_folder = FakeFolder('local', [file_a, file_b, file_d, file_e, file_bi, file_z])
-        b2_folder = FakeFolder('b2', [file_bi, file_c, file_z])
+        local_folder = FakeLocalFolder(
+            [local_file(*f) for f in (file_a, file_b, file_d, file_e, file_bi, file_z)]
+        )
+        b2_folder = FakeB2Folder([file_bi, file_c, file_z])
 
         policies_manager = ScanPoliciesManager(
             exclude_dir_regexes=fakeargs.excludeDirRegex,
             exclude_file_regexes=fakeargs.excludeRegex,
             include_file_regexes=fakeargs.includeRegex,
             exclude_all_symlinks=fakeargs.excludeAllSymlinks
         )
@@ -865,32 +894,32 @@
             )
         )
         self.assertEqual(expected_actions, [str(a) for a in actions])
 
     def test_file_exclusions_with_delete(self):
         expected_actions = [
             'b2_upload(/dir/a.txt, folder/a.txt, 100)',
-            'b2_delete(folder/b.txt.incl, /dir/b.txt.incl, )',
-            'b2_delete(folder/c.txt, /dir/c.txt, )',
+            'b2_delete(folder/b.txt.incl, id_b_100, )',
+            'b2_delete(folder/c.txt, id_c_100, )',
             'b2_upload(/dir/d/d.txt, folder/d/d.txt, 100)',
             'b2_upload(/dir/e/e.incl, folder/e/e.incl, 100)',
         ]
         self._check_folder_sync(
             expected_actions,
             FakeArgs(
                 keep_days_or_delete=KeepOrDeleteMode.DELETE,
                 excludeRegex=["b\\.txt"],
             ),
         )
 
     def test_file_exclusions_inclusions_with_delete(self):
         expected_actions = [
             'b2_upload(/dir/a.txt, folder/a.txt, 100)',
-            'b2_delete(folder/b.txt.incl, /dir/b.txt.incl, )',
-            'b2_delete(folder/c.txt, /dir/c.txt, )',
+            'b2_delete(folder/b.txt.incl, id_b_100, )',
+            'b2_delete(folder/c.txt, id_c_100, )',
             'b2_upload(/dir/d/d.txt, folder/d/d.txt, 100)',
             'b2_upload(/dir/e/e.incl, folder/e/e.incl, 100)',
             'b2_upload(/dir/b.txt.incl, folder/b.txt.incl, 100)',
         ]
         fakeargs = FakeArgs(
             keep_days_or_delete=KeepOrDeleteMode.DELETE,
             excludeRegex=["b\\.txt"],
```

### Comparing `b2sdk-1.8.0/test/unit/v1/test_sync_report.py` & `b2sdk-1.9.0/test/unit/v1/test_sync_report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_utils.py` & `b2sdk-1.9.0/test/unit/v1/test_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v1/test_version_utils.py` & `b2sdk-1.9.0/test/unit/v1/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-1.8.0/test/unit/v_all/test_api.py` & `b2sdk-1.9.0/test/unit/v_all/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,7 +57,21 @@
             self.api.get_bucket_by_id("this id doesn't even exist")
         created_bucket = self.api.create_bucket('bucket1', 'allPrivate')
         read_bucket = self.api.get_bucket_by_id(created_bucket.id_)
         assert created_bucket.id_ == read_bucket.id_
         self.cache.save_bucket(Bucket(api=self.api, name='bucket_name', id_='bucket_id'))
         read_bucket = self.api.get_bucket_by_id('bucket_id')
         assert read_bucket.name == 'bucket_name'
+
+    def test_get_download_url_for_file_name(self):
+        self._authorize_account()
+
+        download_url = self.api.get_download_url_for_file_name('bucket1', 'some-file.txt')
+
+        assert download_url == 'http://download.example.com/file/bucket1/some-file.txt'
+
+    def test_get_download_url_for_fileid(self):
+        self._authorize_account()
+
+        download_url = self.api.get_download_url_for_fileid('file-id')
+
+        assert download_url == 'http://download.example.com/b2api/v2/b2_download_file_by_id?fileId=file-id'
```

