# Comparing `tmp/foundry-dev-tools-1.0.7.tar.gz` & `tmp/foundry-dev-tools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundry-dev-tools-1.0.7.tar", last modified: Wed Apr  5 12:01:41 2023, max compression
+gzip compressed data, was "foundry-dev-tools-1.0.8.tar", last modified: Mon Apr 17 13:53:10 2023, max compression
```

## Comparing `foundry-dev-tools-1.0.7.tar` & `foundry-dev-tools-1.0.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.741510 foundry-dev-tools-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.741510 foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/blank_issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.741510 foundry-dev-tools-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/Configuration_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/FoundryFileSystem_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/FoundryRestClient_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/SSO_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/docs/pictures/
--rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-already-cached-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-already-cached-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-new-transaction-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-new-transaction-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/pictures/tpa_config.png
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/docs/usage_and_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/src/foundry_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    86868 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/foundry_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/fsspec_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.749510 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/metadata_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/spark_caches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.749510 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/converter/foundry_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.749510 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/token_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/token_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.745510 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-05 12:01:41.000000 foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.749510 foundry-dev-tools-1.0.7/src/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.749510 foundry-dev-tools-1.0.7/src/transforms/api/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/api/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/api/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/api/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/src/transforms/api/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/foundry_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_cached_foundry_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_cached_foundry_client_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.737510 foundry-dev-tools-1.0.7/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/tests/test_data/binary_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_data/binary_dataset/bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:01:41.753510 foundry-dev-tools-1.0.7/tests/test_data/iris/
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_data/iris/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29242 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_foundry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_foundry_local_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_foundry_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_foundry_spark_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_foundry_sql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_fsspec_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_multipass_tpa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_spark_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/test_transforms_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-05 12:00:13.000000 foundry-dev-tools-1.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/blank_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/Configuration_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/FoundryFileSystem_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/FoundryRestClient_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/SSO_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/docs/pictures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87463 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/pictures/tpa_config.png
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/docs/usage_and_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-17 13:53:10.894557 foundry-dev-tools-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86868 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/foundry_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/fsspec_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/metadata_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/spark_caches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/foundry_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.886557 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:53:10.000000 foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/src/transforms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/src/transforms/api/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/foundry_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_cached_foundry_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_cached_foundry_client_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.882557 foundry-dev-tools-1.0.8/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:53:10.890557 foundry-dev-tools-1.0.8/tests/test_data/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_data/iris/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29242 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_local_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_spark_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_foundry_sql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33551 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_fsspec_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_multipass_tpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_spark_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/test_transforms_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-17 13:51:45.000000 foundry-dev-tools-1.0.8/tox.ini
```

### Comparing `foundry-dev-tools-1.0.7/.coveragerc` & `foundry-dev-tools-1.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/blank_issue.yml` & `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/blank_issue.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/bug_report.yml` & `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.github/ISSUE_TEMPLATE/feature_request.yml` & `foundry-dev-tools-1.0.8/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.github/pull_request_template.md` & `foundry-dev-tools-1.0.8/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.github/workflows/ci.yml` & `foundry-dev-tools-1.0.8/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     outputs:
       wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
       - uses: actions/checkout@v3
         with: {fetch-depth: 0}  # deep clone for setuptools-scm
       - uses: actions/setup-python@v4
         id: setup-python
-        with: {python-version: "3.10"}
+        with: {python-version: "3.11"}
       - name: Run static analysis and format checkers
         run: |
           pip install .[testing,transforms]
           pipx run --python '${{ steps.setup-python.outputs.python-path }}' tox -e lint
       - name: Build package distribution files
         run: >-
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
@@ -51,15 +51,15 @@
 
   test:
     needs: prepare
     strategy:
       matrix:
         python:
         - "3.8"
-        - "3.10"  # newest Python that is supported by pyspark
+        - "3.11"  # newest Python that is supported by pyspark
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         id: setup-python
         with:
           python-version: ${{ matrix.python }}
@@ -75,15 +75,15 @@
   publish:
     needs: test
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
-        with: {python-version: "3.10"}
+        with: {python-version: "3.11"}
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
       - name: Publish Package
         env:
           TWINE_REPOSITORY: pypi
           TWINE_USERNAME: __token__
```

### Comparing `foundry-dev-tools-1.0.7/.github/workflows/docs.yml` & `foundry-dev-tools-1.0.8/.github/workflows/docs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     permissions:
       contents: read
       pages: write
       id-token: write
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
-        with: {python-version: "3.10"}
+        with: {python-version: "3.11"}
       - name: Build Docs
         run: >-
           pipx run tox -e docs
       - name: Upload docs artifact
         uses: actions/upload-pages-artifact@v1
         with:
           path: 'docs/_build/html'
```

### Comparing `foundry-dev-tools-1.0.7/.gitignore` & `foundry-dev-tools-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/.pre-commit-config.yaml` & `foundry-dev-tools-1.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/LICENSE` & `foundry-dev-tools-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/PKG-INFO` & `foundry-dev-tools-1.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Home-page: https://github.com/emdgroup/foundry-dev-tools
 Author: Nicolas Renkamp, Jonas Wunderlich
 Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
@@ -14,14 +14,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
@@ -31,20 +32,22 @@
 License-File: LICENSE
 
 <div align="center">
   <br/>
 
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?color=important&style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square"/></a>
-
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
   <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
@@ -93,18 +96,24 @@
     df.shape
     # Out[2]: (17, 10)
     ```
 
 
 ## Quickstart
 
+With pip:
 ```shell
 pip install foundry-dev-tools
 ```
 
+With conda or mamba on the conda-forge channel:
+```shell
+conda install -c conda-forge foundry-dev-tools
+```
+
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
 * Local development experience in your favourite IDE (PyCharm, VSCode, ...)
     * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
 * Quicker turnaround time when making changes
```

#### html2text {}

```diff
@@ -1,37 +1,43 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.8 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
 Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
 jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
 URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
 Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
 https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
 https://emdgroup.github.io/foundry-dev-tools/changelog.html Platform: any
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Intended Audience :: Developers Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
-:: Windows Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: <4.0,>=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8 Provides-Extra: integration-testing Provides-Extra: testing
-Provides-Extra: transforms License-File: LICENSE
+Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
+Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
+System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
+Python: <4.0,>=3.8 Description-Content-Type: text/markdown; charset=UTF-
+8 Provides-Extra: integration-testing Provides-Extra: testing Provides-Extra:
+transforms License-File: LICENSE
 
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
                        tools/ci.yml?style=flat-square]
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
- tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/v/foundry-dev-
- tools.svg?style=flat-square]_[https://img.shields.io/pypi/pyversions/foundry-
- dev-tools?style=flat-square]_[https://shields.io/badge/License-Apache%202.0-
- green.svg?style=flat-square]_[https://img.shields.io/github/issues/emdgroup/
- foundry-dev-tools?color=important&style=flat-square]_[https://img.shields.io/
-github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square]
+  tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/pyversions/
+                         foundry-dev-tools?style=flat-
+     square&label=Supported%20Python%20versions&color=%23ffb86c]_[https://
+            img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-
+    square&label=PyPI%20version&color=%23bd93f9]_[Conda_Version]_[https://
+  img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-
+   square&color=%236272a4]_[Conda_Downloads]_[https://img.shields.io/github/
+issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6]_[https://
+    img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-
+    square&color=%23ff79c6]_[https://shields.io/badge/License-Apache%202.0-
+                   green.svg?style=flat-square&color=%234c1]
                                  Documentation
                                  Installation
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
@@ -54,25 +60,26 @@
 branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
 emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
 implementation of `fsspec` for Foundry. Useful to interact with Foundry from
 popular data science libraries such as `pandas` or `dask`. * For example:
 ```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
 Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
 ("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart ```shell pip install foundry-dev-
-tools ``` [Further instructions](https://emdgroup.github.io/foundry-dev-tools/
-installation.html) can be found in our documentation. ## Why did we build this?
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...) *
-Access to modern developer tools and workflows such as pylint, black, isort,
-pre-commit hooks etc. * Quicker turnaround time when making changes * Debug,
-change code and run in a matter of seconds instead of minutes * No accidental
-or auto commits * Keep your git history clean # License Copyright (c) 2023
-Merck KGaA, Darmstadt, Germany Licensed under the Apache License, Version 2.0
-(the "License"); you may not use this file except in compliance with the
-License. You may obtain a copy of the License at https://www.apache.org/
-licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
-software distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
-the License for the specific language governing permissions and limitations
-under the License. The full text of the license can be found in the [LICENSE]
-(https://github.com/emdgroup/foundry-dev-tools/blob/main/LICENSE) file in the
-repository root directory.
+df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
+foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
+conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
+(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
+in our documentation. ## Why did we build this? * Local development experience
+in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
+and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
+turnaround time when making changes * Debug, change code and run in a matter of
+seconds instead of minutes * No accidental or auto commits * Keep your git
+history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use
+this file except in compliance with the License. You may obtain a copy of the
+License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
+applicable law or agreed to in writing, software distributed under the License
+is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied. See the License for the specific language
+governing permissions and limitations under the License. The full text of the
+license can be found in the [LICENSE](https://github.com/emdgroup/foundry-dev-
+tools/blob/main/LICENSE) file in the repository root directory.
```

### Comparing `foundry-dev-tools-1.0.7/README.md` & `foundry-dev-tools-1.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 <div align="center">
   <br/>
 
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?color=important&style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square"/></a>
-
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
   <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
@@ -61,18 +63,24 @@
     df.shape
     # Out[2]: (17, 10)
     ```
 
 
 ## Quickstart
 
+With pip:
 ```shell
 pip install foundry-dev-tools
 ```
 
+With conda or mamba on the conda-forge channel:
+```shell
+conda install -c conda-forge foundry-dev-tools
+```
+
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
 * Local development experience in your favourite IDE (PyCharm, VSCode, ...)
     * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
 * Quicker turnaround time when making changes
```

#### html2text {}

```diff
@@ -1,17 +1,22 @@
 
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
                        tools/ci.yml?style=flat-square]
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
- tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/v/foundry-dev-
- tools.svg?style=flat-square]_[https://img.shields.io/pypi/pyversions/foundry-
- dev-tools?style=flat-square]_[https://shields.io/badge/License-Apache%202.0-
- green.svg?style=flat-square]_[https://img.shields.io/github/issues/emdgroup/
- foundry-dev-tools?color=important&style=flat-square]_[https://img.shields.io/
-github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square]
+  tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/pyversions/
+                         foundry-dev-tools?style=flat-
+     square&label=Supported%20Python%20versions&color=%23ffb86c]_[https://
+            img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-
+    square&label=PyPI%20version&color=%23bd93f9]_[Conda_Version]_[https://
+  img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-
+   square&color=%236272a4]_[Conda_Downloads]_[https://img.shields.io/github/
+issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6]_[https://
+    img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-
+    square&color=%23ff79c6]_[https://shields.io/badge/License-Apache%202.0-
+                   green.svg?style=flat-square&color=%234c1]
                                  Documentation
                                  Installation
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
@@ -34,25 +39,26 @@
 branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
 emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
 implementation of `fsspec` for Foundry. Useful to interact with Foundry from
 popular data science libraries such as `pandas` or `dask`. * For example:
 ```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
 Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
 ("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart ```shell pip install foundry-dev-
-tools ``` [Further instructions](https://emdgroup.github.io/foundry-dev-tools/
-installation.html) can be found in our documentation. ## Why did we build this?
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...) *
-Access to modern developer tools and workflows such as pylint, black, isort,
-pre-commit hooks etc. * Quicker turnaround time when making changes * Debug,
-change code and run in a matter of seconds instead of minutes * No accidental
-or auto commits * Keep your git history clean # License Copyright (c) 2023
-Merck KGaA, Darmstadt, Germany Licensed under the Apache License, Version 2.0
-(the "License"); you may not use this file except in compliance with the
-License. You may obtain a copy of the License at https://www.apache.org/
-licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
-software distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
-the License for the specific language governing permissions and limitations
-under the License. The full text of the license can be found in the [LICENSE]
-(https://github.com/emdgroup/foundry-dev-tools/blob/main/LICENSE) file in the
-repository root directory.
+df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
+foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
+conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
+(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
+in our documentation. ## Why did we build this? * Local development experience
+in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
+and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
+turnaround time when making changes * Debug, change code and run in a matter of
+seconds instead of minutes * No accidental or auto commits * Keep your git
+history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use
+this file except in compliance with the License. You may obtain a copy of the
+License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
+applicable law or agreed to in writing, software distributed under the License
+is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied. See the License for the specific language
+governing permissions and limitations under the License. The full text of the
+license can be found in the [LICENSE](https://github.com/emdgroup/foundry-dev-
+tools/blob/main/LICENSE) file in the repository root directory.
```

### Comparing `foundry-dev-tools-1.0.7/docs/Configuration_usage.md` & `foundry-dev-tools-1.0.8/docs/Configuration_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/FoundryFileSystem_usage.md` & `foundry-dev-tools-1.0.8/docs/FoundryFileSystem_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/FoundryRestClient_usage.md` & `foundry-dev-tools-1.0.8/docs/FoundryRestClient_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/SSO_usage.md` & `foundry-dev-tools-1.0.8/docs/SSO_usage.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/architecture.md` & `foundry-dev-tools-1.0.8/docs/architecture.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/changelog.md` & `foundry-dev-tools-1.0.8/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
+## [1.0.8] - 2023-04-17
+
+### Added
+
+- python 3.11 support, as pyspark 3.4 gained support for it (#13)
+- conda-forge badges to the README (#13)
+
+### Fixed
+
+- typo in docs (#12)
+
+### Removed
+
+- pandas<2 restriction, as pyspark 3.4 supports it (#13)
+
+
 ## [1.0.7] - 2023-04-05
 
 ### Added
 
 - skip_instance_cache kwarg to FoundryFileSystem, which gets passed to fsspec
   it should be set to True in a multithreaded environment (e.g. Streamlit),
   as the same filesystem instance gets reused by default,
@@ -76,14 +92,15 @@
 
 ## [1.0] - 2023-02-28 [YANKED]
 
 - First public Open Source Release of Foundry DevTools.
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/spec/v2.0.0.html
+[1.0.8]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.7...v1.0.8
 [1.0.7]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.6...v1.0.7
 [1.0.6]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.5...v1.0.6
 [1.0.5]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.4...v1.0.5
 [1.0.4]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.3...v1.0.4
 [1.0.3]: https://github.com/emdgroup/foundry-dev-tools/compare/v1.0.2...v1.0.3
 [1.0.2]: https://github.com/emdgroup/foundry-dev-tools/releases/tag/v1.0.2
 [1.0.1]: https://github.com/emdgroup/foundry-dev-tools
```

### Comparing `foundry-dev-tools-1.0.7/docs/conf.py` & `foundry-dev-tools-1.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/develop.md` & `foundry-dev-tools-1.0.8/docs/develop.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/index.md` & `foundry-dev-tools-1.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/installation.md` & `foundry-dev-tools-1.0.8/docs/installation.md`

 * *Files 14% similar despite different names*

```diff
@@ -29,18 +29,24 @@
 ```
 
 ## Install the latest version of Foundry DevTools
 
 We recommend using a new [conda environment] or [python environment],
 after you activated it, just run:
 
-```bash
+With pip:
+```shell
 pip install foundry-dev-tools
 ```
 
+With conda or mamba on the conda-forge channel:
+```shell
+conda install -c conda-forge foundry-dev-tools
+```
+
 or, if you have the repository locally available and want to tinker with the source code
 you could install it in "editable"/"develop mode". Run the following command in
 the Foundry DevTools root directory:
 
 ```bash
 pip install -e .
 ```
```

### Comparing `foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-already-cached-dark.svg` & `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-already-cached-light.svg` & `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-already-cached-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-new-transaction-dark.svg` & `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-dark.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/pictures/mermaid-diagram-new-transaction-light.svg` & `foundry-dev-tools-1.0.8/docs/pictures/mermaid-diagram-new-transaction-light.svg`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/pictures/tpa_config.png` & `foundry-dev-tools-1.0.8/docs/pictures/tpa_config.png`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/docs/usage_and_examples.md` & `foundry-dev-tools-1.0.8/docs/usage_and_examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
 Open the `transforms-python/src/setup.py` file of your repository and change line 8 and 9 by adding a default value 
 for package name and package version:
 
 ```diff
 -      name=os.environ['PKG_NAME'],
 +      name=os.getenv('PKG_NAME', 'your-package-name'),
--      name=os.environ['PKG_VERSION'],
-+      name=os.getenv('PKG_VERSION', 'your-package-version'),
+-      version=os.environ['PKG_VERSION'],
++      version=os.getenv('PKG_VERSION', 'your-package-version'),
 ```
 
 Now you can install the repository into your local environment, when in directory `transform-python/src`:
 
 ```shell
 pip install -e .
 ```
```

### Comparing `foundry-dev-tools-1.0.7/setup.cfg` & `foundry-dev-tools-1.0.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Intended Audience :: Developers
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Topic :: Scientific/Engineering :: Information Analysis
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	pyarrow
-	pandas < 2 # until pyspark supports v2 or also sets this limitation
+	pandas
 	requests
 	fs
 	backoff
 	palantir-oauth-client
 python_requires = >=3.8,<4.0
 
 [options.packages.find]
```

### Comparing `foundry-dev-tools-1.0.7/setup.py` & `foundry-dev-tools-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/__init__.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/cached_foundry_client.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/config.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/foundry_api_client.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/foundry_api_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/fsspec_impl.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/metadata_store.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/metadata_store.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/caches/spark_caches.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/caches/spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/converter/foundry_spark.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/converter/foundry_spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/importer.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/importer.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/spark.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/spark.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools/utils/token_provider/foundry_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/PKG-INFO` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundry-dev-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: Seamlessly run your Palantir Foundry Repository transforms code on your local machine.
 Home-page: https://github.com/emdgroup/foundry-dev-tools
 Author: Nicolas Renkamp, Jonas Wunderlich
 Author-email: nicolas.renkamp@merckgroup.com, jonas.wunderlich@merckgroup.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://emdgroup.github.io/foundry-dev-tools
 Project-URL: Source, https://github.com/emdgroup/foundry-dev-tools
@@ -14,14 +14,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
@@ -31,20 +32,22 @@
 License-File: LICENSE
 
 <div align="center">
   <br/>
 
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/ci.yml?style=flat-square"/></img>
   <a href="https://github.com/emdgroup/foundry-dev-tools/actions/workflows/docs.yml"><img src="https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-tools/docs.yml?style=flat-square"/></img>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square"/></a>
-  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square"/></a>
-  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?color=important&style=flat-square"/></a>
-  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square"/></a>
-
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/pyversions/foundry-dev-tools?style=flat-square&label=Supported%20Python%20versions&color=%23ffb86c"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-square&label=PyPI%20version&color=%23bd93f9"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/vn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Version&color=%23bd93f9" alt="Conda Version"/></a>
+  <a href="https://pypi.org/project/foundry-dev-tools/"><img src="https://img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-square&color=%236272a4"/></a>
+  <a href="https://anaconda.org/conda-forge/foundry-dev-tools"><img src="https://img.shields.io/conda/dn/conda-forge/foundry-dev-tools.svg?style=flat-square&label=Conda%20Forge%20Downloads&color=%236272a4" alt="Conda Downloads"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/issues"><img src="https://img.shields.io/github/issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="https://github.com/emdgroup/foundry-dev-tools/pulls"><img src="https://img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6"/></a>
+  <a href="http://www.apache.org/licenses/LICENSE-2.0"><img src="https://shields.io/badge/License-Apache%202.0-green.svg?style=flat-square&color=%234c1"/></a>
   <p><a href="https://emdgroup.github.io/foundry-dev-tools">Documentation</a></p>
 
   <a href="https://emdgroup.github.io/foundry-dev-tools/installation.html">Installation<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/usage_and_examples.html">Usage<a/>
   &nbsp;•&nbsp;
   <a href="https://emdgroup.github.io/foundry-dev-tools/develop.html">Development<a/>
@@ -93,18 +96,24 @@
     df.shape
     # Out[2]: (17, 10)
     ```
 
 
 ## Quickstart
 
+With pip:
 ```shell
 pip install foundry-dev-tools
 ```
 
+With conda or mamba on the conda-forge channel:
+```shell
+conda install -c conda-forge foundry-dev-tools
+```
+
 [Further instructions](https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found in our documentation.
 
 ## Why did we build this?
 
 * Local development experience in your favourite IDE (PyCharm, VSCode, ...)
     * Access to modern developer tools and workflows such as pylint, black, isort, pre-commit hooks etc.
 * Quicker turnaround time when making changes
```

#### html2text {}

```diff
@@ -1,37 +1,43 @@
-Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: foundry-dev-tools Version: 1.0.8 Summary:
 Seamlessly run your Palantir Foundry Repository transforms code on your local
 machine. Home-page: https://github.com/emdgroup/foundry-dev-tools Author:
 Nicolas Renkamp, Jonas Wunderlich Author-email: nicolas.renkamp@merckgroup.com,
 jonas.wunderlich@merckgroup.com License: Apache License, Version 2.0 Project-
 URL: Documentation, https://emdgroup.github.io/foundry-dev-tools Project-URL:
 Source, https://github.com/emdgroup/foundry-dev-tools Project-URL: Tracker,
 https://github.com/emdgroup/foundry-dev-tools/issues Project-URL: Changelog,
 https://emdgroup.github.io/foundry-dev-tools/changelog.html Platform: any
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Intended Audience :: Developers Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
-:: Windows Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: <4.0,>=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8 Provides-Extra: integration-testing Provides-Extra: testing
-Provides-Extra: transforms License-File: LICENSE
+Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
+Developers Classifier: Operating System :: POSIX :: Linux Classifier: Operating
+System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Scientific/Engineering :: Information Analysis Requires-
+Python: <4.0,>=3.8 Description-Content-Type: text/markdown; charset=UTF-
+8 Provides-Extra: integration-testing Provides-Extra: testing Provides-Extra:
+transforms License-File: LICENSE
 
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
                        tools/ci.yml?style=flat-square]
  [https://img.shields.io/github/actions/workflow/status/emdgroup/foundry-dev-
- tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/v/foundry-dev-
- tools.svg?style=flat-square]_[https://img.shields.io/pypi/pyversions/foundry-
- dev-tools?style=flat-square]_[https://shields.io/badge/License-Apache%202.0-
- green.svg?style=flat-square]_[https://img.shields.io/github/issues/emdgroup/
- foundry-dev-tools?color=important&style=flat-square]_[https://img.shields.io/
-github/issues-pr/emdgroup/foundry-dev-tools?color=blueviolet&style=flat-square]
+  tools/docs.yml?style=flat-square]_[https://img.shields.io/pypi/pyversions/
+                         foundry-dev-tools?style=flat-
+     square&label=Supported%20Python%20versions&color=%23ffb86c]_[https://
+            img.shields.io/pypi/v/foundry-dev-tools.svg?style=flat-
+    square&label=PyPI%20version&color=%23bd93f9]_[Conda_Version]_[https://
+  img.shields.io/pypi/dm/foundry-dev-tools?label=PyPI%20Downloads&style=flat-
+   square&color=%236272a4]_[Conda_Downloads]_[https://img.shields.io/github/
+issues/emdgroup/foundry-dev-tools?style=flat-square&color=%23ff79c6]_[https://
+    img.shields.io/github/issues-pr/emdgroup/foundry-dev-tools?style=flat-
+    square&color=%23ff79c6]_[https://shields.io/badge/License-Apache%202.0-
+                   green.svg?style=flat-square&color=%234c1]
                                  Documentation
                                  Installation
                                      â¢ 
                                      Usage
                                      â¢ 
                                   Development
 # Foundry DevTools Seamlessly run your Palantir Foundry Repository transforms
@@ -54,25 +60,26 @@
 branch='master') df.shape # Out[2]: (17, 10) ``` * [FoundryFileSystem](https://
 emdgroup.github.io/foundry-dev-tools/FoundryFileSystem_usage.html) * An
 implementation of `fsspec` for Foundry. Useful to interact with Foundry from
 popular data science libraries such as `pandas` or `dask`. * For example:
 ```python import pandas as pd # /Global/Foundry Training and Resources/Foundry
 Reference Project/Ontology Project: Aviation/airlines df = pd.read_parquet
 ("foundry://ri.foundry.main.dataset.5d78f3ae-a588-4fd8-9ba2-66827808c85f")
-df.shape # Out[2]: (17, 10) ``` ## Quickstart ```shell pip install foundry-dev-
-tools ``` [Further instructions](https://emdgroup.github.io/foundry-dev-tools/
-installation.html) can be found in our documentation. ## Why did we build this?
-* Local development experience in your favourite IDE (PyCharm, VSCode, ...) *
-Access to modern developer tools and workflows such as pylint, black, isort,
-pre-commit hooks etc. * Quicker turnaround time when making changes * Debug,
-change code and run in a matter of seconds instead of minutes * No accidental
-or auto commits * Keep your git history clean # License Copyright (c) 2023
-Merck KGaA, Darmstadt, Germany Licensed under the Apache License, Version 2.0
-(the "License"); you may not use this file except in compliance with the
-License. You may obtain a copy of the License at https://www.apache.org/
-licenses/LICENSE-2.0 Unless required by applicable law or agreed to in writing,
-software distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See
-the License for the specific language governing permissions and limitations
-under the License. The full text of the license can be found in the [LICENSE]
-(https://github.com/emdgroup/foundry-dev-tools/blob/main/LICENSE) file in the
-repository root directory.
+df.shape # Out[2]: (17, 10) ``` ## Quickstart With pip: ```shell pip install
+foundry-dev-tools ``` With conda or mamba on the conda-forge channel: ```shell
+conda install -c conda-forge foundry-dev-tools ``` [Further instructions]
+(https://emdgroup.github.io/foundry-dev-tools/installation.html) can be found
+in our documentation. ## Why did we build this? * Local development experience
+in your favourite IDE (PyCharm, VSCode, ...) * Access to modern developer tools
+and workflows such as pylint, black, isort, pre-commit hooks etc. * Quicker
+turnaround time when making changes * Debug, change code and run in a matter of
+seconds instead of minutes * No accidental or auto commits * Keep your git
+history clean # License Copyright (c) 2023 Merck KGaA, Darmstadt, Germany
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use
+this file except in compliance with the License. You may obtain a copy of the
+License at https://www.apache.org/licenses/LICENSE-2.0 Unless required by
+applicable law or agreed to in writing, software distributed under the License
+is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied. See the License for the specific language
+governing permissions and limitations under the License. The full text of the
+license can be found in the [LICENSE](https://github.com/emdgroup/foundry-dev-
+tools/blob/main/LICENSE) file in the repository root directory.
```

### Comparing `foundry-dev-tools-1.0.7/src/foundry_dev_tools.egg-info/SOURCES.txt` & `foundry-dev-tools-1.0.8/src/foundry_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/transforms/api/__init__.py` & `foundry-dev-tools-1.0.8/src/transforms/api/__init__.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/transforms/api/_configure.py` & `foundry-dev-tools-1.0.8/src/transforms/api/_configure.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/transforms/api/_dataset.py` & `foundry-dev-tools-1.0.8/src/transforms/api/_dataset.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/transforms/api/_decorators.py` & `foundry-dev-tools-1.0.8/src/transforms/api/_decorators.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/src/transforms/api/_transform.py` & `foundry-dev-tools-1.0.8/src/transforms/api/_transform.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/conftest.py` & `foundry-dev-tools-1.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/foundry_mock_client.py` & `foundry-dev-tools-1.0.8/tests/foundry_mock_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_cached_foundry_client.py` & `foundry-dev-tools-1.0.8/tests/test_cached_foundry_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_cached_foundry_client_integration.py` & `foundry-dev-tools-1.0.8/tests/test_cached_foundry_client_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_config.py` & `foundry-dev-tools-1.0.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_data/binary_dataset/bin` & `foundry-dev-tools-1.0.8/tests/test_data/binary_dataset/bin`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_data/iris/iris.csv` & `foundry-dev-tools-1.0.8/tests/test_data/iris/iris.csv`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_foundry_api.py` & `foundry-dev-tools-1.0.8/tests/test_foundry_api.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_foundry_local_deprecation.py` & `foundry-dev-tools-1.0.8/tests/test_foundry_local_deprecation.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_foundry_mock.py` & `foundry-dev-tools-1.0.8/tests/test_foundry_mock.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_foundry_spark_converters.py` & `foundry-dev-tools-1.0.8/tests/test_foundry_spark_converters.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_foundry_sql_client.py` & `foundry-dev-tools-1.0.8/tests/test_foundry_sql_client.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_fsspec_impl.py` & `foundry-dev-tools-1.0.8/tests/test_fsspec_impl.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_multipass_tpa.py` & `foundry-dev-tools-1.0.8/tests/test_multipass_tpa.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_spark_caches.py` & `foundry-dev-tools-1.0.8/tests/test_spark_caches.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_token_provider.py` & `foundry-dev-tools-1.0.8/tests/test_token_provider.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_transforms.py` & `foundry-dev-tools-1.0.8/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/test_transforms_integration.py` & `foundry-dev-tools-1.0.8/tests/test_transforms_integration.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tests/utils.py` & `foundry-dev-tools-1.0.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `foundry-dev-tools-1.0.7/tox.ini` & `foundry-dev-tools-1.0.8/tox.ini`

 * *Files identical despite different names*

