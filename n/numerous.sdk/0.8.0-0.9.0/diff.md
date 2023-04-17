# Comparing `tmp/numerous.sdk-0.8.0.tar.gz` & `tmp/numerous.sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerous.sdk-0.8.0.tar", last modified: Wed Feb 22 03:54:55 2023, max compression
+gzip compressed data, was "numerous.sdk-0.9.0.tar", last modified: Thu Feb 23 08:07:58 2023, max compression
```

## Comparing `numerous.sdk-0.8.0.tar` & `numerous.sdk-0.9.0.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.655116 numerous.sdk-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2023-02-22 03:54:55.651116 numerous.sdk-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-02-22 03:54:43.000000 numerous.sdk-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-22 03:54:55.655116 numerous.sdk-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.599110 numerous.sdk-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.603111 numerous.sdk-0.8.0/src/numerous/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.619113 numerous.sdk-0.8.0/src/numerous/cli/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/.exclude
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     3548 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     5699 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/build_manager_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.631114 numerous.sdk-0.8.0/src/numerous/cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/build.py
--rw-rw-rw-   0 root         (0) root         (0)     3338 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/checkout.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/clone.py
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/init.py
--rw-rw-rw-   0 root         (0) root         (0)     3412 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/log.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/login.py
--rw-rw-rw-   0 root         (0) root         (0)     4547 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/push.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/commands/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/job.py
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     6149 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/run.py
--rw-rw-rw-   0 root         (0) root         (0)     4309 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.635114 numerous.sdk-0.8.0/src/numerous/client/
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4733 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/common.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/config.py
--rw-rw-rw-   0 root         (0) root         (0)    14384 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/data_source.py
--rw-rw-rw-   0 root         (0) root         (0)    14883 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/numerous_admin_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/numerous_buffered_writer.py
--rw-rw-rw-   0 root         (0) root         (0)    62542 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/numerous_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1830 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/numerous_log_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.639115 numerous.sdk-0.8.0/src/numerous/client/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8676 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/optimization/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     9861 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/client/optimization/orchestrator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.643115 numerous.sdk-0.8.0/src/numerous/image_tools/
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8844 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/app.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.643115 numerous.sdk-0.8.0/src/numerous/image_tools/example_models/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/example_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.643115 numerous.sdk-0.8.0/src/numerous/image_tools/example_models/multiply_by_two/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/example_models/multiply_by_two/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/example_models/multiply_by_two/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.647116 numerous.sdk-0.8.0/src/numerous/image_tools/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/examples/make_report.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/examples/multiply_by_two.py
--rw-rw-rw-   0 root         (0) root         (0)    14832 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.647116 numerous.sdk-0.8.0/src/numerous/image_tools/report/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23917 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/report/report.py
--rw-rw-rw-   0 root         (0) root         (0)    14004 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/image_tools/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.647116 numerous.sdk-0.8.0/src/numerous/sdk/
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.651116 numerous.sdk-0.8.0/src/numerous/sdk/connect/
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     8063 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/job_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3783 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/job_state.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/connect/job_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.651116 numerous.sdk-0.8.0/src/numerous/sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/models/scenario.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-02-22 03:54:30.000000 numerous.sdk-0.8.0/src/numerous/sdk/models/time_setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 03:54:55.611112 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2289 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      522 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-22 03:54:55.000000 numerous.sdk-0.8.0/src/numerous.sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.173327 numerous.sdk-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-02-23 08:07:58.173327 numerous.sdk-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-02-23 08:07:42.000000 numerous.sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 08:07:58.173327 numerous.sdk-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.141323 numerous.sdk-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.141323 numerous.sdk-0.9.0/src/numerous/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.149324 numerous.sdk-0.9.0/src/numerous/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/.exclude
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     5699 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/build_manager_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.153325 numerous.sdk-0.9.0/src/numerous/cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/build.py
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/checkout.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/clone.py
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     3412 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     4547 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/push.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/commands/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     6149 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     4309 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.157325 numerous.sdk-0.9.0/src/numerous/client/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4733 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    14384 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/data_source.py
+-rw-rw-rw-   0 root         (0) root         (0)    14883 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/numerous_admin_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2978 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/numerous_buffered_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    62542 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/numerous_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/numerous_log_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.157325 numerous.sdk-0.9.0/src/numerous/client/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8676 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/optimization/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     9861 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/client/optimization/orchestrator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.157325 numerous.sdk-0.9.0/src/numerous/image_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.157325 numerous.sdk-0.9.0/src/numerous/image_tools/example_models/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/example_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.157325 numerous.sdk-0.9.0/src/numerous/image_tools/example_models/multiply_by_two/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/example_models/multiply_by_two/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/example_models/multiply_by_two/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.161326 numerous.sdk-0.9.0/src/numerous/image_tools/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/examples/make_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/examples/multiply_by_two.py
+-rw-rw-rw-   0 root         (0) root         (0)    14832 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.161326 numerous.sdk-0.9.0/src/numerous/image_tools/report/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23917 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/report/report.py
+-rw-rw-rw-   0 root         (0) root         (0)    14004 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/image_tools/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.161326 numerous.sdk-0.9.0/src/numerous/sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.173327 numerous.sdk-0.9.0/src/numerous/sdk/connect/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/config.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/file_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     8627 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/job_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/job_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/connect/job_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.173327 numerous.sdk-0.9.0/src/numerous/sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/models/scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-02-23 08:07:19.000000 numerous.sdk-0.9.0/src/numerous/sdk/models/time_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 08:07:58.145324 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      522 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-02-23 08:07:58.000000 numerous.sdk-0.9.0/src/numerous.sdk.egg-info/top_level.txt
```

### Comparing `numerous.sdk-0.8.0/LICENSE.txt` & `numerous.sdk-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/PKG-INFO` & `numerous.sdk-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous.sdk
-Version: 0.8.0
+Version: 0.9.0
 License: MIT License
         
         Copyright (c) 2023 Energy Machines ApS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `numerous.sdk-0.8.0/README.md` & `numerous.sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/pyproject.toml` & `numerous.sdk-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "numerous.sdk"
-version = "0.8.0"
+version = "0.9.0"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
```

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/auth.py` & `numerous.sdk-0.9.0/src/numerous/cli/auth.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/build_manager_client.py` & `numerous.sdk-0.9.0/src/numerous/cli/build_manager_client.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/client.py` & `numerous.sdk-0.9.0/src/numerous/cli/client.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/build.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/checkout.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/clone.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/clone.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/config.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/init.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/log.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/log.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/login.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/commands/push.py` & `numerous.sdk-0.9.0/src/numerous/cli/commands/push.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/job.py` & `numerous.sdk-0.9.0/src/numerous/cli/job.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/repository.py` & `numerous.sdk-0.9.0/src/numerous/cli/repository.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/run.py` & `numerous.sdk-0.9.0/src/numerous/cli/run.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/cli/utils.py` & `numerous.sdk-0.9.0/src/numerous/cli/utils.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/__init__.py` & `numerous.sdk-0.9.0/src/numerous/client/__init__.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/common.py` & `numerous.sdk-0.9.0/src/numerous/client/common.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/config.py` & `numerous.sdk-0.9.0/src/numerous/client/config.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/data_source.py` & `numerous.sdk-0.9.0/src/numerous/client/data_source.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/numerous_admin_client.py` & `numerous.sdk-0.9.0/src/numerous/client/numerous_admin_client.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/numerous_buffered_writer.py` & `numerous.sdk-0.9.0/src/numerous/client/numerous_buffered_writer.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/numerous_client.py` & `numerous.sdk-0.9.0/src/numerous/client/numerous_client.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/numerous_log_handler.py` & `numerous.sdk-0.9.0/src/numerous/client/numerous_log_handler.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/optimization/configuration.py` & `numerous.sdk-0.9.0/src/numerous/client/optimization/configuration.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/client/optimization/orchestrator.py` & `numerous.sdk-0.9.0/src/numerous/client/optimization/orchestrator.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/app.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/app.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/examples/make_report.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/examples/make_report.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/examples/multiply_by_two.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/examples/multiply_by_two.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/job.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/job.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/report/report.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/report/report.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/image_tools/system.py` & `numerous.sdk-0.9.0/src/numerous/image_tools/system.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/sdk/connect/auth.py` & `numerous.sdk-0.9.0/src/numerous/sdk/connect/auth.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/sdk/connect/job_client.py` & `numerous.sdk-0.9.0/src/numerous/sdk/connect/job_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from typing import Any
 
 import grpc
 import spm_pb2
 from spm_pb2 import RefreshRequest, Token
 from spm_pb2_grpc import SPMStub, TokenManagerStub
 
-from numerous.sdk.connect import defaults
 from numerous.sdk.connect.auth import AccessTokenAuthMetadataPlugin
+from numerous.sdk.connect.config import Config
+from numerous.sdk.connect.file_manager import FileManager
 from numerous.sdk.connect.job_state import JobState
 from numerous.sdk.connect.job_utils import JobIdentifier
 from numerous.sdk.models.scenario import Scenario
 from numerous.sdk.models.time_setup import TimeSetup
 
 
 class JobStatus(str, Enum):
@@ -37,26 +38,34 @@
     return min(max(minimum, value), maximum)
 
 
 class JobClient:
     """The JobClient is the recommended way to connect to the numerous platform."""
 
     def __init__(
-        self, channel: grpc.Channel, identity: JobIdentifier, execution_id: str
+        self,
+        channel: grpc.Channel,
+        identity: JobIdentifier,
+        execution_id: str,
+        config: Config | None = None,
     ):
         """Initialize the job client with a gRPC channel. The channel must be
         configured with credentials.
 
         :param channel: A gRPC channel configured with required authorization.
         :param identity: Contains identity information for the job object and related objects.
         """
+        self._config = Config() if config is None else config
         self._channel = channel
         self._spm_client = SPMStub(self._channel)
         self._identity = identity
         self._execution_id = execution_id
+        self._file_manager = FileManager(
+            self._spm_client, self._identity.project_id, self._identity.scenario_id
+        )
         self._status: JobStatus = JobStatus.INITIALIZING
         self._progress: float = 0.0
         self._message: str = ""
         self._job_state: JobState | None = None
         self._scenario_document: dict[str, Any] | None = None
 
     def __enter__(self) -> "JobClient":
@@ -70,59 +79,60 @@
         traceback: TracebackType | None,  # noqa: F841
     ) -> bool | None:
         """Closes the gRPC channel upon exiting the context manager."""
         self.close()
         return None
 
     @staticmethod
-    def channel_options() -> list[tuple[str, Any]]:
+    def channel_options(config: Config) -> list[tuple[str, Any]]:
         """Returns the default gRPC channel options."""
         return [
-            ("grpc.max_message_length", defaults.GRPC_MAX_MESSAGE_SIZE),
-            ("grpc.max_send_message_length", defaults.GRPC_MAX_MESSAGE_SIZE),
-            ("grpc.max_receive_message_length", defaults.GRPC_MAX_MESSAGE_SIZE),
+            ("grpc.max_message_length", config.GRPC_MAX_MESSAGE_SIZE),
+            ("grpc.max_send_message_length", config.GRPC_MAX_MESSAGE_SIZE),
+            ("grpc.max_receive_message_length", config.GRPC_MAX_MESSAGE_SIZE),
         ]
 
     @staticmethod
     def create(
         hostname: str,
         port: str,
         refresh_token: str,
         identity: JobIdentifier,
         execution_id: str,
+        config: Config,
     ) -> "JobClient":
         """Create a JobClient from connection parameters.
 
         :param hostname: Hostname of the numerous server
         :param port: gRPC port of the numerous server
         :param refresh_token: Refresh token for the execution.
         :param identity: Contains identity information for the job object and related objects.
         """
         with grpc.secure_channel(
             f"{hostname}:{port}",
             grpc.ssl_channel_credentials(),
-            JobClient.channel_options(),
+            JobClient.channel_options(config),
         ) as unauthorized_channel:
             token_manager = TokenManagerStub(unauthorized_channel)
             access_token = token_manager.GetAccessToken(
                 RefreshRequest(refresh_token=Token(val=refresh_token))
             )
 
         authorized_channel = grpc.secure_channel(
             f"{hostname}:{port}",
             grpc.composite_channel_credentials(
                 grpc.ssl_channel_credentials(),
                 grpc.metadata_call_credentials(
                     AccessTokenAuthMetadataPlugin(access_token.val)
                 ),
             ),
-            JobClient.channel_options(),
+            JobClient.channel_options(config),
         )
 
-        return JobClient(authorized_channel, identity, execution_id)
+        return JobClient(authorized_channel, identity, execution_id, config)
 
     @staticmethod
     def from_environment() -> "JobClient":
         """Create a JobClient from environment variables.
 
         Uses the following environment variables:
          - `NUMEROUS_API_SERVER`
@@ -139,27 +149,33 @@
             os.environ["NUMEROUS_API_REFRESH_TOKEN"],
             JobIdentifier(
                 os.environ["NUMEROUS_PROJECT"],
                 os.environ["NUMEROUS_SCENARIO"],
                 os.environ["JOB_ID"],
             ),
             os.environ["NUMEROUS_EXECUTION_ID"],
+            config=Config.from_environment(),
         )
 
     def close(self) -> None:
         """Close the JobClient.
 
         Closes the JobClient's connection to the numerous platform, immediately
         terminating any active communication.
 
         This method is idempotent.
         """
         self._channel.close()
 
     @property
+    def file_manager(self) -> FileManager:
+        """Access the file manager of the job."""
+        return self._file_manager
+
+    @property
     def state(self) -> JobState:
         """The job state, which can be persisted across hibernations.
 
         It is a lazy property, that will load any remote state on access.
         """
         if self._job_state is None:
             self._job_state = JobState(
@@ -196,15 +212,15 @@
 
         Getting the status message returns a locally cached value.
         """
         return self._message
 
     @message.setter
     def message(self, value: str):
-        self._message = value[: defaults.MAXIMUM_STATUS_MESSAGE_LENGTH]
+        self._message = value[: self._config.MAX_STATUS_MESSAGE_LENGTH]
         self._set_scenario_progress()
 
     @property
     def progress(self) -> float:
         """Progress of the job, reported to the platform. Is clamped between 0.0 and 100.0 upon setting.
 
         Getting the progress returns a locally cached value.
```

### Comparing `numerous.sdk-0.8.0/src/numerous/sdk/connect/job_state.py` & `numerous.sdk-0.9.0/src/numerous/sdk/connect/job_state.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous/sdk/models/time_setup.py` & `numerous.sdk-0.9.0/src/numerous/sdk/models/time_setup.py`

 * *Files identical despite different names*

### Comparing `numerous.sdk-0.8.0/src/numerous.sdk.egg-info/PKG-INFO` & `numerous.sdk-0.9.0/src/numerous.sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous.sdk
-Version: 0.8.0
+Version: 0.9.0
 License: MIT License
         
         Copyright (c) 2023 Energy Machines ApS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `numerous.sdk-0.8.0/src/numerous.sdk.egg-info/SOURCES.txt` & `numerous.sdk-0.9.0/src/numerous.sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,15 @@
 src/numerous/image_tools/examples/make_report.py
 src/numerous/image_tools/examples/multiply_by_two.py
 src/numerous/image_tools/report/__init__.py
 src/numerous/image_tools/report/report.py
 src/numerous/sdk/__init__.py
 src/numerous/sdk/connect/__init__.py
 src/numerous/sdk/connect/auth.py
+src/numerous/sdk/connect/config.py
 src/numerous/sdk/connect/defaults.py
+src/numerous/sdk/connect/file_manager.py
 src/numerous/sdk/connect/job_client.py
 src/numerous/sdk/connect/job_state.py
 src/numerous/sdk/connect/job_utils.py
 src/numerous/sdk/models/scenario.py
 src/numerous/sdk/models/time_setup.py
```

### Comparing `numerous.sdk-0.8.0/src/numerous.sdk.egg-info/requires.txt` & `numerous.sdk-0.9.0/src/numerous.sdk.egg-info/requires.txt`

 * *Files identical despite different names*

