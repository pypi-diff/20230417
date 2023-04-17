# Comparing `tmp/openmetadata_managed_apis-1.0.0.0.dev2.tar.gz` & `tmp/openmetadata_managed_apis-1.0.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.0.0.0.dev2.tar", last modified: Fri Apr 14 17:48:54 2023, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.0.0.0.dev3.tar", last modified: Mon Apr 17 15:29:07 2023, max compression
```

## Comparing `openmetadata_managed_apis-1.0.0.0.dev2.tar` & `openmetadata_managed_apis-1.0.0.0.dev3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.977172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.977172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.977172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.973172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:48:54.977172 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:48:36.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 17:48:51.000000 openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:48:54.981172 openmetadata_managed_apis-1.0.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 17:47:28.000000 openmetadata_managed_apis-1.0.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.211788 openmetadata_managed_apis-1.0.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-17 15:29:07.211788 openmetadata_managed_apis-1.0.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.199788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.199788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.203788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.203788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.203788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.207788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.207788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.195788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.207788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.207788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.211788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:29:07.199788 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:28:44.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 15:29:02.000000 openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:29:07.211788 openmetadata_managed_apis-1.0.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 15:27:23.000000 openmetadata_managed_apis-1.0.0.0.dev3/setup.py
```

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/PKG-INFO` & `openmetadata_managed_apis-1.0.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.0.0.0.dev2
+Version: 1.0.0.0.dev3
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/README.md` & `openmetadata_managed_apis-1.0.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/ip.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/run_automation.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/delete.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-managed-apis
-Version: 1.0.0.0.dev2
+Version: 1.0.0.0.dev3
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.0.0.0.dev3/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.0.dev2/setup.py` & `openmetadata_managed_apis-1.0.0.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 }
 
 setup(
     name=PLUGIN_NAME,
     packages=find_packages(include=[f"{PLUGIN_NAME}.*", PLUGIN_NAME]),
     include_package_data=True,
     package_data={PLUGIN_NAME: get_package_data()},
-    version="1.0.0.0.dev2",
+    version="1.0.0.0.dev3",
     url="https://open-metadata.org/",
     author="OpenMetadata Committers",
     license="Apache License 2.0",
     description="Airflow REST APIs to create and manage DAGS",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     entry_points={
```

