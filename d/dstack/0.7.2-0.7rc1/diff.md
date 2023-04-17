# Comparing `tmp/dstack-0.7.2.tar.gz` & `tmp/dstack-0.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.7.2.tar", last modified: Mon Apr 17 10:00:49 2023, max compression
+gzip compressed data, was "dstack-0.7rc1.tar", last modified: Tue Apr 11 14:42:51 2023, max compression
```

## Comparing `dstack-0.7.2.tar` & `dstack-0.7rc1.tar`

### file list

```diff
@@ -1,233 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:49.001645 dstack-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-04-17 10:00:14.000000 dstack-0.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-17 10:00:49.001645 dstack-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-17 10:00:14.000000 dstack-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.981645 dstack-0.7.2/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.981645 dstack-0.7.2/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.981645 dstack-0.7.2/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/api/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.981645 dstack-0.7.2/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.985645 dstack-0.7.2/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.985645 dstack-0.7.2/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.985645 dstack-0.7.2/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    23710 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.985645 dstack-0.7.2/cli/dstack/backend/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/hub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/hub/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/cp/
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/prune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/pull/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/pull/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/push/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/push/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    13917 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/run/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.989645 dstack-0.7.2/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/core/userconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/background/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/background/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/background/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/background/tasks/resubmit_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/migration/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/migration/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/migration/versions/3b900659c822_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/migration/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.993645 dstack-0.7.2/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/repository/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/routers/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/security/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/hub/security/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/utils/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.981645 dstack-0.7.2/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 10:00:48.000000 dstack-0.7.2/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/tests/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/backend/base/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:48.997645 dstack-0.7.2/cli/tests/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/routers/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/routers/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/hub/routers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:49.001645 dstack-0.7.2/cli/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/integration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/integration/test_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:49.001645 dstack-0.7.2/cli/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:49.001645 dstack-0.7.2/cli/tests/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/providers/docker/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/providers/test_local_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:49.001645 dstack-0.7.2/cli/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-17 10:00:14.000000 dstack-0.7.2/cli/tests/utils/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:00:49.001645 dstack-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-17 10:00:14.000000 dstack-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-04-11 14:42:02.000000 dstack-0.7rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.143200 dstack-0.7rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 14:42:02.000000 dstack-0.7rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/api/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/hub/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.131200 dstack-0.7rc1/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/pull/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/pull/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/push/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/push/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.135200 dstack-0.7rc1/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.139200 dstack-0.7rc1/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 14:42:50.000000 dstack-0.7rc1/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.127200 dstack-0.7rc1/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:42:51.000000 dstack-0.7rc1/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:51.143200 dstack-0.7rc1/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-11 14:42:02.000000 dstack-0.7rc1/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:42:51.143200 dstack-0.7rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-11 14:42:02.000000 dstack-0.7rc1/setup.py
```

### Comparing `dstack-0.7.2/LICENSE.md` & `dstack-0.7rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/PKG-INFO` & `dstack-0.7rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.7.2
+Version: 0.7rc1
 Summary: The hassle-free tool for managing ML workflows on any cloud platform.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.7.2 Summary: The hassle-free tool
-for managing ML workflows on any cloud platform. Home-page: https://dstack.ai
-Author: Andrey Cheptsov Author-email: andrey@dstack.ai License: UNKNOWN
-Project-URL: Source, https://github.com/dstackai/dstack Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
+Metadata-Version: 2.1 Name: dstack Version: 0.7rc1 Summary: The hassle-free
+tool for managing ML workflows on any cloud platform. Home-page: https://
+dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
+UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
+UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
 Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
                             ****** [dstack] ******
                 *** Automate your ML workflows on any cloud ***
      The hassle-free tool for managing ML workflows on any cloud platform.
```

### Comparing `dstack-0.7.2/README.md` & `dstack-0.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/artifacts.py` & `dstack-0.7rc1/cli/dstack/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/backend.py` & `dstack-0.7rc1/cli/dstack/api/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Dict, List, Optional
 
+from dstack import version
 from dstack.backend.aws import AwsBackend
 from dstack.backend.base import Backend, BackendType, RemoteBackend
 from dstack.backend.gcp import GCPBackend
 from dstack.backend.hub import HubBackend
 from dstack.backend.local import LocalBackend
 
-backends_classes = [HubBackend, AwsBackend, GCPBackend, LocalBackend]
+backends_classes = [AwsBackend, GCPBackend, LocalBackend]
+if not version.__is_release__:
+    backends_classes.append(HubBackend)
 
 
 def get_all_backends():
     return [backend_cls() for backend_cls in backends_classes]
 
 
 def list_backends(all_backend: bool = False) -> List[Backend]:
```

### Comparing `dstack-0.7.2/cli/dstack/api/config.py` & `dstack-0.7rc1/cli/dstack/api/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/logs.py` & `dstack-0.7rc1/cli/dstack/api/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/repo.py` & `dstack-0.7rc1/cli/dstack/api/repo.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/run.py` & `dstack-0.7rc1/cli/dstack/api/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/api/tags.py` & `dstack-0.7rc1/cli/dstack/api/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/compute.py` & `dstack-0.7rc1/cli/dstack/backend/aws/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/config.py` & `dstack-0.7rc1/cli/dstack/backend/aws/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,34 +68,30 @@
         )
         self.profile_name = (
             profile_name or os.getenv("DSTACK_AWS_PROFILE") or os.getenv("AWS_PROFILE")
         )
         self.subnet_id = subnet_id or os.getenv("DSTACK_AWS_EC2_SUBNET")
         self.credentials = credentials
 
-    def load(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def load(self, path: Path = get_config_path()):
         if path.exists():
             with path.open() as f:
                 config_data = yaml.load(f, Loader=yaml.FullLoader)
                 if config_data.get("backend") != "aws":
                     raise ConfigError(f"It's not AWS config")
                 if not config_data.get("bucket"):
                     raise Exception(f"For AWS backend:the bucket field is required")
                 self.profile_name = config_data.get("profile") or os.getenv("AWS_PROFILE")
                 self.region_name = config_data.get("region") or os.getenv("AWS_DEFAULT_REGION")
                 self.bucket_name = config_data["bucket"]
                 self.subnet_id = config_data.get("subnet")
         else:
             raise ConfigError()
 
-    def save(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def save(self, path: Path = get_config_path()):
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
         with path.open("w+") as f:
             f.write(self.serialize_yaml())
 
     def serialize(self) -> Dict:
         config_data = {
```

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/logs.py` & `dstack-0.7rc1/cli/dstack/backend/aws/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/runners.py` & `dstack-0.7rc1/cli/dstack/backend/aws/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/storage.py` & `dstack-0.7rc1/cli/dstack/backend/aws/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/aws/utils.py` & `dstack-0.7rc1/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/artifacts.py` & `dstack-0.7rc1/cli/dstack/backend/base/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/compute.py` & `dstack-0.7rc1/cli/dstack/backend/base/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/jobs.py` & `dstack-0.7rc1/cli/dstack/backend/base/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/logs.py` & `dstack-0.7rc1/cli/dstack/backend/base/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/repos.py` & `dstack-0.7rc1/cli/dstack/backend/base/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/runners.py` & `dstack-0.7rc1/cli/dstack/backend/base/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/runs.py` & `dstack-0.7rc1/cli/dstack/backend/base/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/base/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/storage.py` & `dstack-0.7rc1/cli/dstack/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/base/tags.py` & `dstack-0.7rc1/cli/dstack/backend/base/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/compute.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/config.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,25 +171,21 @@
     def deserialize_yaml(cls, yaml_content: str) -> "GCPConfig":
         content = yaml.load(yaml_content, yaml.FullLoader)
         if content is None:
             raise ConfigError("Cannot load config")
         return cls.deserialize(content)
 
     @classmethod
-    def load(cls, path: Optional[Path] = None) -> "GCPConfig":
-        if path is None:
-            path = get_config_path()
+    def load(cls, path: Path = get_config_path()) -> "GCPConfig":
         if not path.exists():
             raise ConfigError("No config found")
         with open(path) as f:
             return GCPConfig.deserialize_yaml(f.read())
 
-    def save(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def save(self, path: Path = get_config_path()):
         with open(path, "w+") as f:
             f.write(self.serialize_yaml())
 
 
 class GCPConfigurator(Configurator):
     @property
     def name(self):
```

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/logs.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import time
 from datetime import datetime
 from typing import Dict, Generator, Optional
 
 from google.cloud import logging
 from google.oauth2 import service_account
 
 from dstack.backend.base import jobs
 from dstack.backend.base.logs import fix_urls
 from dstack.backend.base.storage import Storage
 from dstack.core.job import Job
 from dstack.core.log_event import LogEvent, LogEventSource
 from dstack.core.repo import RepoAddress
 
+POLL_LOGS_ATTEMPTS = 5
+POLL_LOGS_WAIT_TIME = 2
+
 
 class GCPLogging:
     def __init__(
         self, project_id: str, bucket_name: str, credentials: Optional[service_account.Credentials]
     ):
         self.project_id = project_id
         self.bucket_name = bucket_name
@@ -27,17 +31,26 @@
         run_name: str,
         start_time: int,
     ) -> Generator[LogEvent, None, None]:
         log_name = _get_log_name(self.bucket_name, repo_address, run_name)
         timestamp = datetime.fromtimestamp(start_time / 1000).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
         logger = self.logging_client.logger(log_name)
         jobs_cache = {}
-        log_entries = logger.list_entries(filter_=f'timestamp>="{timestamp}"')
-        for log_entry in log_entries:
-            yield _log_entry_to_log_event(storage, repo_address, log_entry, jobs_cache)
+        # Hack: It takes some time for logs to become available after runner writes them.
+        # So we try reading logs multiple times.
+        # The proper solution would be for the runner to ensure logs availability before marking job as Done.
+        found_log = False
+        for _ in range(POLL_LOGS_ATTEMPTS):
+            log_entries = logger.list_entries(filter_=f'timestamp>="{timestamp}"')
+            for log_entry in log_entries:
+                found_log = True
+                yield _log_entry_to_log_event(storage, repo_address, log_entry, jobs_cache)
+            if found_log:
+                break
+            time.sleep(POLL_LOGS_WAIT_TIME)
 
 
 def _get_log_name(bucket_name: str, repo_address: RepoAddress, run_name) -> str:
     return f"dstack-jobs-{bucket_name}-{repo_address.path('-')}-{run_name}"
 
 
 def _log_entry_to_log_event(
```

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/storage.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/gcp/utils.py` & `dstack-0.7rc1/cli/dstack/backend/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/hub/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/hub/client.py` & `dstack-0.7rc1/cli/dstack/backend/hub/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from typing import Dict, Generator, List, Optional
 from urllib.parse import urlencode, urlparse, urlunparse
 
 import requests
 
 from dstack.core.artifact import Artifact
-from dstack.core.error import BackendError
 from dstack.core.job import Job, JobHead
 from dstack.core.log_event import LogEvent
 from dstack.core.repo import LocalRepoData, RepoAddress, RepoCredentials
 from dstack.core.run import RunHead
 from dstack.core.secret import Secret
 from dstack.core.tag import TagHead
 from dstack.hub.models import (
@@ -24,14 +23,32 @@
     SaveRepoCredentials,
     SecretAddUpdate,
     StopRunners,
     UserRepoAddress,
 )
 
 
+def _url(url: str, project: str, additional_path: str, query: dict = {}):
+    unparse_url = urlparse(url=url)
+    if additional_path.startswith("/"):
+        additional_path = additional_path[1:]
+
+    new_url = urlunparse(
+        (
+            unparse_url.scheme,
+            unparse_url.netloc,
+            f"/api/project/{project}/{additional_path}",
+            None,
+            urlencode(query=query),
+            unparse_url.fragment,
+        )
+    )
+    return new_url
+
+
 class HubClient:
     def __init__(self, url: str, project: str, token: str):
         self.url = url
         self.token = token
         self.project = project
 
     @staticmethod
@@ -57,572 +74,685 @@
         return headers
 
     def _headers(self):
         headers = HubClient._auth(token=self.token)
         headers["Content-type"] = "application/json"
         return headers
 
-    def create_run(self, repo_address: RepoAddress) -> str:
+    def get_repos_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/runs/create",
+            additional_path=f"/repos/credentials/get",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            return resp.text
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                json_data = resp.json()
+                return RepoCredentials(**json_data)
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
-    def create_job(self, job: Job):
+    def save_repos_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/create",
-        )
-        resp = _make_hub_request(
-            requests.post, host=self.url, url=url, headers=self._headers(), data=job.json()
+            additional_path=f"/repos/credentials/save",
         )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=SaveRepoCredentials(
+                    repo_address=repo_address,
+                    repo_credentials=repo_credentials,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
-    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
+    def create_run(self, repo_address: RepoAddress) -> str:
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/get",
+            additional_path=f"/runs/create",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=JobsGet(
-                repo_address=repo_address,
-                job_id=job_id,
-            ).json(),
-        )
-        if resp.ok:
-            json_data = resp.json()
-            return Job.parse_obj(json_data)
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                return resp.text
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return ""
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return ""
 
-    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
+    def create_job(self, job: Job):
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/jobs/list",
+            additional_path=f"/jobs/create",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=JobsList(repo_address=repo_address, run_name=run_name).json(),
-        )
-        if resp.ok:
-            body = resp.json()
-            return [Job.parse_obj(job) for job in body]
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=job.json())
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def run_job(self, job: Job):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/runners/run",
         )
-        resp = _make_hub_request(
-            requests.post, host=self.url, url=url, headers=self._headers(), data=job.json()
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=job.json())
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def stop_job(self, repo_address: RepoAddress, job_id: str, abort: bool):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/runners/stop",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=StopRunners(
-                repo_address=repo_address,
-                job_id=job_id,
-                abort=abort,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
-
-    def list_job_heads(
-        self, repo_address: RepoAddress, run_name: Optional[str] = None
-    ) -> Optional[List[JobHead]]:
-        query = {}
-        if run_name is not None:
-            query["run_name"] = run_name
-        url = _url(
-            url=self.url, project=self.project, additional_path=f"/jobs/list/heads", query=query
-        )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            body = resp.json()
-            return [JobHead.parse_obj(job) for job in body]
-        resp.raise_for_status()
-
-    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
-        url = _url(
-            url=self.url,
-            project=self.project,
-            additional_path=f"/jobs/delete",
-        )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=JobsGet(repo_address=repo_address, job_id=job_id).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=StopRunners(
+                    repo_address=repo_address,
+                    job_id=job_id,
+                    abort=abort,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def get_tag_head(self, repo_address: RepoAddress, tag_name: str) -> Optional[TagHead]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/{tag_name}",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            return TagHead.parse_obj(resp.json())
-        elif resp.status_code == 404:
-            return None
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                return TagHead.parse_obj(resp.json())
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def list_tag_heads(self, repo_address: RepoAddress) -> Optional[List[TagHead]]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/list/heads",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            body = resp.json()
-            return [TagHead.parse_obj(tag) for tag in body]
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                body = resp.json()
+                return [TagHead.parse_obj(tag) for tag in body]
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def add_tag_from_run(
         self,
         repo_address: RepoAddress,
         tag_name: str,
         run_name: str,
         run_jobs: Optional[List[Job]],
     ):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/add/run",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=AddTagRun(
-                repo_address=repo_address,
-                tag_name=tag_name,
-                run_name=run_name,
-                run_jobs=run_jobs,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=AddTagRun(
+                    repo_address=repo_address,
+                    tag_name=tag_name,
+                    run_name=run_name,
+                    run_jobs=run_jobs,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def add_tag_from_local_dirs(
         self,
         repo_data: LocalRepoData,
         tag_name: str,
         local_dirs: List[str],
     ):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/add/path",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=AddTagPath(
-                repo_data=repo_data,
-                tag_name=tag_name,
-                local_dirs=local_dirs,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=AddTagPath(
+                    repo_data=repo_data,
+                    tag_name=tag_name,
+                    local_dirs=local_dirs,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def delete_tag_head(self, repo_address: RepoAddress, tag_head: TagHead):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/tags/{tag_head.tag_name}/delete",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
-    def list_run_heads(
-        self,
-        repo_address: RepoAddress,
-        run_name: Optional[str] = None,
-        include_request_heads: bool = True,
-    ) -> List[RunHead]:
+    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/runs/list",
+            additional_path=f"/repos/update",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=RunsList(
-                repo_address=repo_address,
-                run_name=run_name,
-                include_request_heads=include_request_heads,
-            ).json(),
-        )
-        if resp.ok:
-            body = resp.json()
-            return [RunHead.parse_obj(run) for run in body]
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=ReposUpdate(
+                    repo_address=repo_address,
+                    last_run_at=last_run_at,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
-    def update_repo_last_run_at(self, repo_address: RepoAddress, last_run_at: int):
+    def list_job_heads(
+        self, repo_address: RepoAddress, run_name: Optional[str] = None
+    ) -> Optional[List[JobHead]]:
+        query = {}
+        if not (run_name is None):
+            query["run_name"] = run_name
         url = _url(
-            url=self.url,
-            project=self.project,
-            additional_path=f"/repos/update",
+            url=self.url, project=self.project, additional_path=f"/jobs/list/heads", query=query
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=ReposUpdate(
-                repo_address=repo_address,
-                last_run_at=last_run_at,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(url=url, headers=self._headers(), data=repo_address.json())
+            if resp.ok:
+                body = resp.json()
+                return [JobHead.parse_obj(job) for job in body]
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
-    def get_repos_credentials(self, repo_address: RepoAddress) -> Optional[RepoCredentials]:
+    def list_run_heads(
+        self,
+        repo_address: RepoAddress,
+        run_name: Optional[str] = None,
+        include_request_heads: bool = True,
+    ) -> List[RunHead]:
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/repos/credentials/get",
+            additional_path=f"/runs/list",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            json_data = resp.json()
-            return RepoCredentials(**json_data)
-        elif resp.status_code == 404:
-            return None
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=RunsList(
+                    repo_address=repo_address,
+                    run_name=run_name,
+                    include_request_heads=include_request_heads,
+                ).json(),
+            )
+            if resp.ok:
+                body = resp.json()
+                return [RunHead.parse_obj(run) for run in body]
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return []
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return []
 
-    def save_repos_credentials(self, repo_address: RepoAddress, repo_credentials: RepoCredentials):
+    def get_job(self, repo_address: RepoAddress, job_id: str) -> Optional[Job]:
         url = _url(
             url=self.url,
             project=self.project,
-            additional_path=f"/repos/credentials/save",
+            additional_path=f"/jobs/get",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=SaveRepoCredentials(
-                repo_address=repo_address,
-                repo_credentials=repo_credentials,
-            ).json(),
-        )
-        if resp.ok:
-            return resp.text
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=JobsGet(
+                    repo_address=repo_address,
+                    job_id=job_id,
+                ).json(),
+            )
+            if resp.ok:
+                json_data = resp.json()
+                return Job.parse_obj(json_data)
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def list_secret_names(self, repo_address: RepoAddress) -> List[str]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/secrets/list",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            return resp.json()
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=repo_address.json(),
+            )
+            if resp.ok:
+                json_data = resp.json()
+                return json_data
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return []
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return []
 
     def get_secret(self, repo_address: RepoAddress, secret_name: str) -> Optional[Secret]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/secrets/{secret_name}/get",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            json_data = resp.json()
-            return Secret.parse_obj(json_data)
-        elif resp.status_code == 404:
-            return None
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=repo_address.json(),
+            )
+            if resp.ok:
+                json_data = resp.json()
+                return Secret.parse_obj(json_data)
+            elif resp.status_code == 404:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def add_secret(self, repo_address: RepoAddress, secret: Secret):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/secrets/add",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=SecretAddUpdate(
-                repo_address=repo_address,
-                secret=secret,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=SecretAddUpdate(
+                    repo_address=repo_address,
+                    secret=secret,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def update_secret(self, repo_address: RepoAddress, secret: Secret):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/secrets/update",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=SecretAddUpdate(
-                repo_address=repo_address,
-                secret=secret,
-            ).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=SecretAddUpdate(
+                    repo_address=repo_address,
+                    secret=secret,
+                ).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def delete_secret(self, repo_address: RepoAddress, secret_name: str):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/secrets/{secret_name}/delete",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=repo_address.json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=repo_address.json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
+
+    def list_jobs(self, repo_address: RepoAddress, run_name: str) -> List[Job]:
+        url = _url(
+            url=self.url,
+            project=self.project,
+            additional_path=f"/jobs/list",
+        )
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=JobsList(repo_address=repo_address, run_name=run_name).json(),
+            )
+            if resp.ok:
+                job_data = resp.json()
+                return [Job.parse_obj(job) for job in job_data]
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return []
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return []
 
     def list_run_artifact_files(self, repo_address: RepoAddress, run_name: str) -> List[Artifact]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/artifacts/list",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=JobsList(repo_address=repo_address, run_name=run_name).json(),
-        )
-        if resp.ok:
-            artifact_data = resp.json()
-            return [Artifact.parse_obj(artifact) for artifact in artifact_data]
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=JobsList(repo_address=repo_address, run_name=run_name).json(),
+            )
+            if resp.ok:
+                artifact_data = resp.json()
+                return [Artifact.parse_obj(artifact) for artifact in artifact_data]
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return []
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return []
+
+    def delete_job_head(self, repo_address: RepoAddress, job_id: str):
+        url = _url(
+            url=self.url,
+            project=self.project,
+            additional_path=f"/jobs/delete",
+        )
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=JobsGet(repo_address=repo_address, job_id=job_id).json(),
+            )
+            if resp.ok:
+                return None
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def poll_logs(
         self,
         repo_address: RepoAddress,
         job_heads: List[JobHead],
         start_time: int,
         attached: bool,
     ) -> Generator[LogEvent, None, None]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/logs/poll",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=PollLogs(
-                repo_address=repo_address,
-                job_heads=job_heads,
-                start_time=start_time,
-                attached=attached,
-            ).json(),
-        )
-        if resp.ok:
-            _braces = 0
-            _body = bytearray()
-            for chunk in resp.iter_content(chunk_size=128):
-                for b in chunk:
-                    if b == 123:
-                        _braces += 1
-                    elif b == 125:
-                        _braces -= 1
-                    _body.append(b)
-                    if _braces == 0:
-                        json_data = json.loads(_body)
-                        _body = bytearray()
-                        yield LogEvent.parse_obj(json_data)
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=PollLogs(
+                    repo_address=repo_address,
+                    job_heads=job_heads,
+                    start_time=start_time,
+                    attached=attached,
+                ).json(),
+                stream=True,
+            )
+            if resp.ok:
+                _braces = 0
+                _body = bytearray()
+                for chunk in resp.iter_content(chunk_size=128):
+                    for b in chunk:
+                        if b == 123:
+                            _braces += 1
+                        elif b == 125:
+                            _braces -= 1
+                        _body.append(b)
+
+                        if _braces == 0:
+                            json_data = json.loads(_body)
+                            _body = bytearray()
+                            yield LogEvent.parse_obj(json_data)
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def upload_file(self, dest_path: str) -> Optional[str]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/link/upload",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=LinkUpload(object_key=dest_path).json(),
-        )
-        if resp.ok:
-            return resp.text
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=LinkUpload(object_key=dest_path).json(),
+            )
+            if resp.ok:
+                return resp.text
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def download_file(self, dest_path: str) -> Optional[str]:
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/link/download",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=LinkUpload(object_key=dest_path).json(),
-        )
-        if resp.ok:
-            return resp.text
-        resp.raise_for_status()
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=LinkUpload(object_key=dest_path).json(),
+            )
+            if resp.ok:
+                return resp.text
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return None
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
+        return None
 
     def delete_workflow_cache(self, repo_address: RepoAddress, username: str, workflow_name: str):
         url = _url(
             url=self.url,
             project=self.project,
             additional_path=f"/workflows/{workflow_name}/cache/delete",
         )
-        resp = _make_hub_request(
-            requests.post,
-            host=self.url,
-            url=url,
-            headers=self._headers(),
-            data=UserRepoAddress(username=username, repo_address=repo_address).json(),
-        )
-        if resp.ok:
-            return
-        resp.raise_for_status()
-
-
-def _url(url: str, project: str, additional_path: str, query: dict = {}):
-    unparse_url = urlparse(url=url)
-    if additional_path.startswith("/"):
-        additional_path = additional_path[1:]
-    new_url = urlunparse(
-        (
-            unparse_url.scheme,
-            unparse_url.netloc,
-            f"/api/project/{project}/{additional_path}",
-            None,
-            urlencode(query=query),
-            unparse_url.fragment,
-        )
-    )
-    return new_url
-
-
-def _make_hub_request(request_func, host, *args, **kwargs) -> requests.Response:
-    try:
-        resp: requests.Response = request_func(*args, **kwargs)
-        if resp.status_code == 401:
-            raise BackendError(f"Invalid hub token")
-        return resp
-    except requests.ConnectionError:
-        raise BackendError(f"Cannot connect to hub at {host}")
+        try:
+            resp = requests.post(
+                url=url,
+                headers=self._headers(),
+                data=UserRepoAddress(username=username, repo_address=repo_address).json(),
+            )
+            if resp.ok:
+                return
+            elif resp.status_code == 401:
+                print("Unauthorized. Please set correct token")
+                return
+            else:
+                resp.raise_for_status()
+        except requests.ConnectionError:
+            print(f"{self.url} connection refused")
```

### Comparing `dstack-0.7.2/cli/dstack/backend/hub/config.py` & `dstack-0.7rc1/cli/dstack/backend/hub/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
     def __init__(self):
         super().__init__()
         self.url = os.getenv("DSTACK_HUB_URL") or None
         self.project = os.getenv("DSTACK_HUB_PROJECT") or None
         self.token = os.getenv("DSTACK_HUB_TOKEN") or None
 
-    def load(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def load(self, path: Path = get_config_path()):
         if path.exists():
             with path.open() as f:
                 config_data = yaml.load(f, Loader=yaml.FullLoader)
                 if config_data.get("backend") != self.NAME:
                     raise ConfigError(f"It's not HUB config")
                 if config_data.get("url") is None:
                     raise ConfigError(f"For HUB backend:the URL field is required")
@@ -38,17 +36,15 @@
                     raise ConfigError(f"For HUB backend:the project field is required")
                 self.url = config_data.get("url")
                 self.project = config_data.get("project")
                 self.token = config_data.get("token")
         else:
             raise ConfigError()
 
-    def save(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def save(self, path: Path = get_config_path()):
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
         with path.open("w") as f:
             config_data = {
                 "backend": self.NAME,
                 "url": self.url,
                 "project": self.project,
```

### Comparing `dstack-0.7.2/cli/dstack/backend/hub/storage.py` & `dstack-0.7rc1/cli/dstack/backend/hub/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/local/__init__.py` & `dstack-0.7rc1/cli/dstack/backend/local/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/local/compute.py` & `dstack-0.7rc1/cli/dstack/backend/local/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/local/config.py` & `dstack-0.7rc1/cli/dstack/backend/local/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from pathlib import Path
-from typing import Optional
 
 import yaml
 
 from dstack.core.config import BackendConfig, get_config_path, get_dstack_dir
 
 
 class LocalConfig(BackendConfig):
     def __init__(self):
         super().__init__()
         self.path = get_dstack_dir()
 
-    def load(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def load(self, path: Path = get_config_path()):
+        super().load(path=path)
         if path.exists():
             with path.open() as f:
                 config_data = yaml.load(f, Loader=yaml.FullLoader)
                 self.path = config_data.get("path") or get_dstack_dir()
 
-    def save(self, path: Optional[Path] = None):
-        if path is None:
-            path = get_config_path()
+    def save(self, path: Path = get_config_path()):
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
         with path.open("w") as f:
             config_data = {"backend": "local", "path": self.path}
             yaml.dump(config_data, f)
```

### Comparing `dstack-0.7.2/cli/dstack/backend/local/logs.py` & `dstack-0.7rc1/cli/dstack/backend/local/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/local/runners.py` & `dstack-0.7rc1/cli/dstack/backend/local/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,26 +154,26 @@
     uname = platform.uname()
     arch = _arch()
     darwin = uname.system == "Darwin"
     windows = uname.system == "Windows"
     linux = uname.system == "Linux"
     arm64 = arch == "arm64" or arch == "aarch64"
     i386 = arch == "i386"
-    amd64 = arch in ["x86_64", "AMD64"]
+    amd64 = arch == "x86_64"
     if darwin and arm64:
         filename = "dstack-runner-darwin-arm64"
     elif darwin and amd64:
         filename = "dstack-runner-darwin-amd64"
     elif linux and i386:
         filename = "dstack-runner-linux-x86"
     elif linux and amd64:
         filename = "dstack-runner-linux-amd64"
     elif windows and i386:
         filename = "dstack-runner-windows-x86.exe"
-    elif windows and amd64:
+    elif linux and amd64:
         filename = "dstack-runner-windows-amd64.exe"
     else:
         raise Exception(f"Unsupported platform: {uname}")
     return filename
 
 
 def _config_directory_path() -> Path:
```

### Comparing `dstack-0.7.2/cli/dstack/backend/local/secrets.py` & `dstack-0.7rc1/cli/dstack/backend/local/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/backend/local/storage.py` & `dstack-0.7rc1/cli/dstack/backend/local/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/config/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/cp/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/cp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from pathlib import Path
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.backend.base import Backend
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
+from dstack.cli.common import console
 from dstack.core.config import get_dstack_dir
+from dstack.core.error import BackendError, check_config, check_git
 from dstack.core.repo import RepoAddress
 
 
 class CpCommand(BasicCommand):
     NAME = "cp"
     DESCRIPTION = "Copy artifact files to a local target path"
 
@@ -38,15 +39,14 @@
             metavar="TARGET",
             type=str,
             help="A local path to download artifact file or directory into",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         repo_data = load_repo_data()
         backends = list_backends()
         run_name = None
         backend = None
         for backend in backends:
             try:
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/hub/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/init/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/init/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from argparse import Namespace
 from pathlib import Path
 from typing import Optional
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
+from dstack.cli.common import console
 from dstack.cli.config import BaseConfig
+from dstack.core.error import check_config, check_git
 from dstack.core.userconfig import RepoUserConfig
 
 
 def get_ssh_keypair(key_path: Optional[str], default: str = "~/.ssh/id_rsa") -> Optional[str]:
     """Returns path to the private key if keypair exists"""
     key_path = Path(key_path or default).expanduser().resolve()
     pub_key = (
@@ -50,15 +51,14 @@
             help="A path to the private SSH key file for SSH tunneling",
             type=str,
             dest="ssh_identity_file",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         local_repo_data = load_repo_data(args.gh_token, args.git_identity_file)
         local_repo_data.ls_remote()
         repo_credentials = local_repo_data.repo_credentials()
 
         config = BaseConfig()
         repo_user_config = RepoUserConfig(ssh_key_path=get_ssh_keypair(args.ssh_identity_file))
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/logs/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/logs/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from argparse import Namespace
 
 from dstack.api.backend import list_backends
 from dstack.api.logs import poll_logs
 from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git
+from dstack.core.error import check_config, check_git
 from dstack.utils.common import since
 
 
 class LogCommand(BasicCommand):
     NAME = "logs"
     DESCRIPTION = "Show logs"
 
@@ -36,15 +36,14 @@
             "minutes in the past.",
             type=str,
             default="1d",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         repo_data = load_repo_data()
         anyone = False
         for backend in list_backends():
             start_time = since(args.since)
             job_heads = backend.list_job_heads(repo_data, args.run_name)
             if job_heads:
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/ls/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from argparse import Namespace
+from collections import defaultdict
 from pathlib import Path
+from typing import Optional
 
 from rich.table import Table
 
 from dstack.api.artifacts import list_artifacts_with_merged_backends
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
+from dstack.cli.common import console
+from dstack.core.error import check_config, check_git
 from dstack.utils.common import sizeof_fmt
 
 
 class LsCommand(BasicCommand):
     NAME = "ls"
     DESCRIPTION = "List artifacts"
 
@@ -40,15 +43,14 @@
         )
         self._parser.add_argument(
             "-t", "--total", help="Show total folder size", action="store_true"
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         table = Table(box=None)
         table.add_column("ARTIFACT", style="bold", no_wrap=True)
         table.add_column("FILE")
         table.add_column("SIZE", style="dark_sea_green4")
         table.add_column("BACKENDS", style="bold")
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/prune/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/prune/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 from typing import List
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.backend.base import Backend
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
+from dstack.cli.common import console
+from dstack.core.error import check_config, check_git
 from dstack.core.repo import LocalRepoData
 
 
 class PruneCommand(BasicCommand):
     NAME = "prune"
     DESCRIPTION = "Prunes cache from the storage"
 
@@ -24,15 +25,14 @@
         cache_cmd.add_argument(
             "workflow", metavar="WORKFLOW", help="A workflow name to prune cache"
         )
         cache_cmd.set_defaults(prune_action=self.prune_cache)
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: argparse.Namespace):
         repo_data = load_repo_data()
         backends = list_backends()
         args.prune_action(args, backends, repo_data)
 
     @staticmethod
     def prune_cache(args: argparse.Namespace, backends: List[Backend], repo_data: LocalRepoData):
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/ps/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 from argparse import Namespace
 
 from rich.live import Live
 
 from dstack.api.backend import list_backends
 from dstack.api.run import list_runs_with_merged_backends
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import (
-    check_backend,
-    check_config,
-    check_git,
-    generate_runs_table,
-    print_runs,
-)
+from dstack.cli.common import generate_runs_table, print_runs
+from dstack.core.error import check_config, check_git
 
 LIVE_PROVISION_INTERVAL_SECS = 2
 
 REFRESH_RATE_PER_SEC = 3
 
 
 class PSCommand(BasicCommand):
@@ -42,15 +37,14 @@
             "--watch",
             help="Watch statuses of runs in realtime",
             action="store_true",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         list_runs = list_runs_with_merged_backends(list_backends(), args.run_name, args.all)
         if args.watch:
             try:
                 with Live(
                     generate_runs_table(list_runs), refresh_per_second=REFRESH_RATE_PER_SEC
                 ) as live:
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/pull/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/pull/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import Namespace
 
 from dstack.api.backend import get_current_remote_backend, get_local_backend
 from dstack.api.repo import load_repo_data
 from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
-from dstack.core.error import BackendError
+from dstack.cli.common import console
+from dstack.core.error import BackendError, check_config, check_git
 
 
 class PullCommand(BasicCommand):
     NAME = "pull"
     DESCRIPTION = "Pull artifacts of a remote run"
 
     def __init__(self, parser):
@@ -21,15 +21,14 @@
             metavar="(RUN | :TAG)",
             type=str,
             help="A name of a run or a tag",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         repo_data = load_repo_data()
         remote_backend = get_current_remote_backend()
         if remote_backend is None:
             console.print(f"No remote backend configured. Run `dstack config`.")
             exit(1)
         try:
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/push/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/push/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import os
 from argparse import Namespace
 from pathlib import Path
 
 from dstack.api.backend import get_current_remote_backend, get_local_backend
 from dstack.api.repo import load_repo_data
 from dstack.api.run import RunNotFoundError, TagNotFoundError, get_tagged_run_name
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
-from dstack.core.error import BackendError
+from dstack.cli.common import console
+from dstack.core.error import BackendError, check_config, check_git
 
 
 class PushCommand(BasicCommand):
     NAME = "push"
     DESCRIPTION = "Push artifacts of a local run"
 
     def __init__(self, parser):
@@ -22,15 +23,14 @@
             metavar="(RUN | :TAG)",
             type=str,
             help="A name of a run or a tag",
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         repo_data = load_repo_data()
         local_backend = get_local_backend()
         remote_backend = get_current_remote_backend()
         if remote_backend is None:
             console.print(f"No remote backend configured. Run `dstack config`.")
             exit(1)
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/rm/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from rich import print
 from rich.prompt import Confirm
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git
+from dstack.core.error import check_config, check_git
 
 
 class RMCommand(BasicCommand):
     NAME = "rm"
     DESCRIPTION = "Remove run(s)"
 
     def __init__(self, parser):
@@ -30,15 +30,14 @@
         )
         self._parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         if (
             args.run_name
             and (args.yes or Confirm.ask(f"[red]Delete the run '{args.run_name}'?[/]"))
         ) or (args.all and (args.yes or Confirm.ask("[red]Delete all runs?[/]"))):
             repo_data = load_repo_data()
             deleted_run = False
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/run/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/run/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 from jsonschema import ValidationError, validate
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Confirm
 from websocket import WebSocketApp
 
 from dstack import providers
 from dstack.api.backend import get_backend_by_name, get_current_remote_backend, get_local_backend
+from dstack.api.logs import poll_logs
 from dstack.api.repo import load_repo_data
 from dstack.api.run import list_runs_with_merged_backends
 from dstack.backend.base import Backend
 from dstack.backend.base.logs import fix_urls
 from dstack.cli.commands import BasicCommand
 from dstack.cli.commands.run.ssh_tunnel import allocate_local_ports, run_ssh_tunnel
-from dstack.cli.common import check_backend, check_config, check_git, console, print_runs
+from dstack.cli.common import console, print_runs
 from dstack.cli.config import BaseConfig
+from dstack.core.error import check_backend, check_config, check_git
 from dstack.core.job import Job, JobHead, JobStatus
 from dstack.core.repo import RepoAddress
 from dstack.core.request import RequestStatus
 from dstack.core.userconfig import RepoUserConfig
+from dstack.utils.common import since
 
 __all__ = "RunCommand"
 
 POLL_PROVISION_RATE_SECS = 3
 
 POLL_FINISHED_STATE_RATE_SECS = 1
 
@@ -211,16 +214,25 @@
             ssh_port = ports.get(ssh_port, ssh_port)
             ssh_key_escaped = ssh_key.replace(" ", "\\ ")
             console.print("To connect via SSH, use:")
             console.print(f"  ssh -i {ssh_key_escaped} root@localhost -p {ssh_port}")
             console.print()
 
         run = backend.list_run_heads(repo_address, run_name)[0]
-        if run.status.is_unfinished() or run.status == JobStatus.DONE:
+        if len(job_heads) == 1 and run and run.status == JobStatus.RUNNING:
             poll_logs_ws(backend, repo_address, jobs[0], ports)
+        else:
+            poll_logs(
+                backend,
+                repo_address,
+                job_heads,
+                since("1d"),
+                attach=True,
+                from_run=True,
+            )
     except KeyboardInterrupt:
         if Confirm.ask(f" [red]Abort the run '{run_name}'?[/]"):
             backend.stop_jobs(repo_address, run_name, abort=True)
             console.print(f"[grey58]OK[/]")
 
 
 class RunCommand(BasicCommand):
@@ -310,16 +322,15 @@
             repo_credentials = backend.get_repo_credentials(repo_data)
             repo_user_config = config.read(
                 config.repos / f"{repo_data.path(delimiter='.')}.yaml",
                 RepoUserConfig,
                 non_empty=False,
             )
             if not repo_credentials:
-                console.print("Call `dstack init` first")
-                exit(1)
+                sys.exit(f"Call `dstack init` first")
             if not repo_user_config.ssh_key_path:
                 if (
                     (backend.name != "local" and not args.detach)
                     or workflow_data.get("ssh", False)
                     or "--ssh" in provider_args
                 ):
                     console.print("Call `dstack init` first")
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/run/ssh_tunnel.py` & `dstack-0.7rc1/cli/dstack/cli/commands/run/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/secrets/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/secrets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rich.prompt import Confirm, Prompt
 from rich.table import Table
 from rich_argparse import RichHelpFormatter
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git
+from dstack.core.error import check_config, check_git
 from dstack.core.secret import Secret
 
 
 class SecretCommand(BasicCommand):
     NAME = "secrets"
     DESCRIPTION = "Manage secrets"
 
@@ -62,16 +62,14 @@
         delete_secrets_parser = subparsers.add_parser("delete", help="Delete a secret")
         delete_secrets_parser.add_argument(
             "secret_name", metavar="NAME", type=str, help="The name of the secret"
         )
         delete_secrets_parser.set_defaults(func=self.delete_secret)
 
     @check_config
-    @check_git
-    @check_backend
     def add_secret(self, args: Namespace):
         repo_data = load_repo_data()
         for backend in list_backends():
             if backend.get_secret(repo_data, args.secret_name):
                 if args.yes or Confirm.ask(
                     f"[red]The secret '{args.secret_name}' (backend: {backend.name}) already exists. "
                     f"Do you want to override it?[/]"
@@ -87,16 +85,14 @@
                 secret_value = args.secret_value or Prompt.ask("Value", password=True)
                 backend.add_secret(
                     repo_data, Secret(secret_name=args.secret_name, secret_value=secret_value)
                 )
                 print(f"[grey58]OK (backend: {backend.name})[/]")
 
     @check_config
-    @check_git
-    @check_backend
     def update_secret(self, args: Namespace):
         repo_data = load_repo_data()
         anyone = False
         for backend in list_backends():
             if backend.get_secret(repo_data, args.secret_name):
                 anyone = True
                 secret_value = args.secret_value or Prompt.ask("Value", password=True)
@@ -104,16 +100,14 @@
                     repo_data, Secret(secret_name=args.secret_name, secret_value=secret_value)
                 )
                 print(f"[grey58]OK (backend: {backend.name})[/]")
         if not anyone:
             sys.exit(f"The secret '{args.secret_name}' doesn't exist")
 
     @check_config
-    @check_git
-    @check_backend
     def delete_secret(self, args: Namespace):
         repo_data = load_repo_data()
         anyone = False
         for backend in list_backends():
             secret = backend.get_secret(repo_data, args.secret_name)
             if not (secret is None) and Confirm.ask(
                 f" [red]Delete the secret '{secret.secret_name}'"
@@ -123,15 +117,14 @@
                 backend.delete_secret(repo_data, secret.secret_name)
                 print(f"[grey58]OK[/]")
         if not anyone:
             sys.exit(f"The secret '{args.secret_name}' doesn't exist")
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         console = Console()
         table = Table(box=None)
         repo_data = load_repo_data()
         table.add_column("NAME", style="bold", no_wrap=True)
         table.add_column("BACKEND", style="bold", no_wrap=True)
         secrets = {}
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/stop/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from argparse import Namespace
 
 from rich.prompt import Confirm
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git, console
+from dstack.cli.common import console
+from dstack.core.error import check_config, check_git
 
 
 def _verb(abort: bool):
     if abort:
         return "Abort"
     else:
         return "Stop"
@@ -42,15 +43,14 @@
         )
         self._parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         if not args.run_name and not args.all:
             console.print("Specify a run name or use --all to stop all workflows")
             exit(1)
         if (
             args.run_name
             and (
```

### Comparing `dstack-0.7.2/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.7rc1/cli/dstack/cli/commands/tags/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from rich_argparse import RichHelpFormatter
 
 from dstack.api.backend import list_backends
 from dstack.api.repo import load_repo_data
 from dstack.api.tags import list_tag_heads_with_merged_backends
 from dstack.backend.base import BackendType
 from dstack.cli.commands import BasicCommand
-from dstack.cli.common import check_backend, check_config, check_git
-from dstack.core.error import BackendError
+from dstack.core.error import BackendError, check_config, check_git
 from dstack.utils.common import pretty_date
 
 
 class TAGCommand(BasicCommand):
     NAME = "tags"
     DESCRIPTION = "Manage tags"
 
@@ -62,15 +61,14 @@
         delete_tags_parser.add_argument(
             "-y", "--yes", help="Don't ask for confirmation", action="store_true"
         )
         delete_tags_parser.set_defaults(func=self.delete_tag)
 
     @check_config
     @check_git
-    @check_backend
     def _command(self, args: Namespace):
         repo_data = load_repo_data()
         console = Console()
         table = Table(box=None)
         table.add_column("TAG", style="bold", no_wrap=True)
         table.add_column("CREATED", style="grey58", no_wrap=True)
         table.add_column("RUN", style="grey58", no_wrap=True)
@@ -87,16 +85,14 @@
                 tag_head.run_name,
                 tag_head.local_repo_user_name or "",
                 ", ".join(b.name for b in backends),
             )
         console.print(table)
 
     @check_config
-    @check_git
-    @check_backend
     def add_tag(self, args: Namespace):
         if args.run_name or args.artifact_paths:
             repo_data = load_repo_data()
             added_tag = False
             confirmed_override = False
             for backend in list_backends():
                 tag_head = backend.get_tag_head(repo_data, args.tag_name)
@@ -137,16 +133,14 @@
                 print(f"The run '{args.run_name}' doesn't exist")
                 exit(1)
             print(f"[grey58]OK[/]")
         else:
             sys.exit("Specify -r RUN or -a PATH to create a tag")
 
     @check_config
-    @check_git
-    @check_backend
     def delete_tag(self, args: Namespace):
         repo_data = load_repo_data()
         tag_heads = []
         for backend in list_backends():
             tag_head = backend.get_tag_head(repo_data, args.tag_name)
             if tag_head is not None:
                 tag_heads.append((backend, tag_head))
```

### Comparing `dstack-0.7.2/cli/dstack/cli/common.py` & `dstack-0.7rc1/cli/dstack/cli/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import os
 from importlib.util import find_spec
 from typing import List, Optional, Tuple
 
-from git import InvalidGitRepositoryError
 from rich.console import Console
 from rich.prompt import Prompt
 from rich.table import Table
 
 from dstack.backend.base import Backend
-from dstack.core.error import BackendError, ConfigError
 from dstack.core.job import JobStatus
 from dstack.core.request import RequestStatus
 from dstack.core.run import RunHead
 from dstack.utils.common import pretty_date
 
 is_termios_available = find_spec("termios") is not None
 
@@ -101,15 +98,14 @@
 def print_runs(runs_with_backends: List[Tuple[RunHead, List[Backend]]]):
     table = generate_runs_table(runs_with_backends)
     console.print(table)
 
 
 _status_colors = {
     JobStatus.SUBMITTED: "yellow",
-    JobStatus.PENDING: "yellow",
     JobStatus.DOWNLOADING: "yellow",
     JobStatus.RUNNING: "dark_sea_green4",
     JobStatus.UPLOADING: "dark_sea_green4",
     JobStatus.DONE: "gray74",
     JobStatus.FAILED: "red",
     JobStatus.STOPPED: "grey58",
     JobStatus.STOPPING: "yellow",
@@ -134,40 +130,7 @@
     if status_column and run.has_request_status(
         [RequestStatus.TERMINATED, RequestStatus.NO_CAPACITY]
     ):
         color = "dark_orange"
     else:
         color = _status_colors.get(run.status)
     return f"[{'bold ' if run_column else ''}{color}]{val}[/]" if color is not None else val
-
-
-def check_config(func):
-    def decorator(*args, **kwargs):
-        try:
-            func(*args, **kwargs)
-        except ConfigError:
-            console.print(f"Call 'dstack config' first")
-            exit(1)
-
-    return decorator
-
-
-def check_git(func):
-    def decorator(*args, **kwargs):
-        try:
-            func(*args, **kwargs)
-        except InvalidGitRepositoryError:
-            console.print(f"{os.getcwd()} is not a Git repo")
-            exit(1)
-
-    return decorator
-
-
-def check_backend(func):
-    def decorator(*args, **kwargs):
-        try:
-            func(*args, **kwargs)
-        except BackendError as e:
-            console.print(e.message)
-            exit(1)
-
-    return decorator
```

### Comparing `dstack-0.7.2/cli/dstack/cli/config.py` & `dstack-0.7rc1/cli/dstack/cli/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/cli/handlers.py` & `dstack-0.7rc1/cli/dstack/cli/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dstack import version
 from dstack.cli.commands.config import ConfigCommand
 from dstack.cli.commands.cp import CpCommand
 from dstack.cli.commands.hub import HubCommand
 from dstack.cli.commands.init import InitCommand
 from dstack.cli.commands.logs import LogCommand
 from dstack.cli.commands.ls import LsCommand
 from dstack.cli.commands.prune import PruneCommand
@@ -25,15 +26,17 @@
     PullCommand,
     PushCommand,
     RMCommand,
     RunCommand,
     SecretCommand,
     StopCommand,
     TAGCommand,
-    HubCommand,
 ]
 
+if not version.__is_release__:
+    commands_classes.append(HubCommand)
+
 
 def cli_initialize(parser):
     commands = [cls(parser=parser) for cls in commands_classes]
     for command in commands:
         command.register()
```

### Comparing `dstack-0.7.2/cli/dstack/cli/main.py` & `dstack-0.7rc1/cli/dstack/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     parser.set_defaults(func=lambda _: parser.print_help())
     subparsers = parser.add_subparsers(metavar="COMMAND")
 
     cli_initialize(parser=subparsers)
 
     if len(sys.argv) < 2:
         parser.print_help()
-        exit(0)
+        exit(1)
     args, unknown = parser.parse_known_args()
     args.unknown = unknown
     args.func(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dstack-0.7.2/cli/dstack/cli/updates.py` & `dstack-0.7rc1/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/app.py` & `dstack-0.7rc1/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/artifact.py` & `dstack-0.7rc1/cli/dstack/core/artifact.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/config.py` & `dstack-0.7rc1/cli/dstack/core/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     return Path.joinpath(Path.home(), ".dstack")
 
 
 class BackendConfig(ABC):
     credentials: Optional[Dict] = None
 
     @abstractmethod
-    def save(self, path: Optional[Path] = None):
+    def save(self, path: Path = get_config_path()):
         pass
 
     @abstractmethod
-    def load(self, path: Optional[Path] = None):
+    def load(self, path: Path = get_config_path()):
         pass
 
 
 class Configurator(ABC):
     NAME = ""
 
     @property
```

### Comparing `dstack-0.7.2/cli/dstack/core/job.py` & `dstack-0.7rc1/cli/dstack/core/job.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/repo.py` & `dstack-0.7rc1/cli/dstack/core/repo.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/request.py` & `dstack-0.7rc1/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/run.py` & `dstack-0.7rc1/cli/dstack/core/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/runners.py` & `dstack-0.7rc1/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/core/tag.py` & `dstack-0.7rc1/cli/dstack/core/tag.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/background/tasks/resubmit_jobs.py` & `dstack-0.7rc1/cli/dstack/hub/background/tasks/resubmit_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/db/__init__.py` & `dstack-0.7rc1/cli/dstack/hub/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/db/models.py` & `dstack-0.7rc1/cli/dstack/hub/db/models.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/main.py` & `dstack-0.7rc1/cli/dstack/hub/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/migration/env.py` & `dstack-0.7rc1/cli/dstack/hub/migration/env.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/migration/versions/3b900659c822_.py` & `dstack-0.7rc1/cli/dstack/hub/migration/versions/3b900659c822_.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/models/__init__.py` & `dstack-0.7rc1/cli/dstack/hub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/repository/projects.py` & `dstack-0.7rc1/cli/dstack/hub/repository/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/repository/users.py` & `dstack-0.7rc1/cli/dstack/hub/repository/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/artifacts.py` & `dstack-0.7rc1/cli/dstack/hub/routers/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/cache.py` & `dstack-0.7rc1/cli/dstack/hub/routers/cache.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/jobs.py` & `dstack-0.7rc1/cli/dstack/hub/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/link.py` & `dstack-0.7rc1/cli/dstack/hub/routers/link.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/logs.py` & `dstack-0.7rc1/cli/dstack/hub/routers/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/projects.py` & `dstack-0.7rc1/cli/dstack/hub/routers/projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/repos.py` & `dstack-0.7rc1/cli/dstack/hub/routers/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/runners.py` & `dstack-0.7rc1/cli/dstack/hub/routers/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/runs.py` & `dstack-0.7rc1/cli/dstack/hub/routers/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/secrets.py` & `dstack-0.7rc1/cli/dstack/hub/routers/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/tags.py` & `dstack-0.7rc1/cli/dstack/hub/routers/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/users.py` & `dstack-0.7rc1/cli/dstack/hub/routers/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/util.py` & `dstack-0.7rc1/cli/dstack/hub/routers/util.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/routers/workflows.py` & `dstack-0.7rc1/cli/dstack/hub/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/hub/security/permissions.py` & `dstack-0.7rc1/cli/dstack/hub/security/permissions.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/__init__.py` & `dstack-0.7rc1/cli/dstack/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/_torchrun/main.py` & `dstack-0.7rc1/cli/dstack/providers/_torchrun/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/bash/main.py` & `dstack-0.7rc1/cli/dstack/providers/bash/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/code/main.py` & `dstack-0.7rc1/cli/dstack/providers/code/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from dstack.providers import Provider
 
 
 class CodeProvider(Provider):
     def __init__(self):
         super().__init__("code")
         self.setup = None
-        self.ports = None
         self.python = None
         self.version = None
         self.requirements = None
         self.env = None
         self.artifact_specs = None
         self.working_dir = None
         self.resources = None
@@ -32,15 +31,14 @@
         provider_args: List[str],
         workflow_name: Optional[str],
         provider_data: Dict[str, Any],
         run_name: str,
     ):
         super().load(backend, provider_args, workflow_name, provider_data, run_name)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
-        self.ports = self.provider_data.get("ports")
         self.python = self._safe_python_version("python")
         self.version = self.provider_data.get("version") or "1.74.3"
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
@@ -48,46 +46,36 @@
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
         parser = ArgumentParser(
             prog="dstack run " + (workflow_name or self.provider_name),
             formatter_class=RichHelpFormatter,
         )
         self._add_base_args(parser)
         parser.add_argument("--ssh", action="store_true", dest="openssh_server")
-        parser.add_argument("-p", "--ports", metavar="PORT_COUNT", type=int)
         return parser
 
     def parse_args(self):
         parser = self._create_parser(self.workflow_name)
         args, unknown_args = parser.parse_known_args(self.provider_args)
         self._parse_base_args(args, unknown_args)
         if args.openssh_server:
             self.openssh_server = True
-        if args.ports:
-            self.provider_data["ports"] = args.ports
 
     def create_job_specs(self) -> List[JobSpec]:
         env = {}
         connection_token = uuid.uuid4().hex
         env["CONNECTION_TOKEN"] = connection_token
         apps = [
             AppSpec(
                 port_index=0,
                 app_name="code",
                 url_query_params={
                     "tkn": connection_token,
                 },
             )
         ]
-        for i in range(self.ports or 0):
-            apps.append(
-                AppSpec(
-                    port_index=i + 1,
-                    app_name="code" + (str(i + 1)),
-                )
-            )
         if self.openssh_server:
             apps.append(AppSpec(port_index=len(apps), app_name="openssh-server"))
         return [
             JobSpec(
                 image_name=self.image_name,
                 commands=self._commands(),
                 entrypoint=["/bin/bash", "-i", "-c"],
@@ -108,21 +96,14 @@
 
     def _commands(self):
         commands = []
         if self.env:
             self._extend_commands_with_env(commands, self.env)
         if self.openssh_server:
             self._extend_commands_with_openssh_server(commands, self.ssh_key_pub, 1)
-        commands.append("export _PORT=$PORT_0")
-        if self.ports:
-            for i in range(self.ports):
-                commands.append(f"export PORT_{i}=$PORT_{i + 1}")
-                commands.append(f"echo 'export PORT_{i}=\"$PORT_{i + 1}\"' >> ~/.bashrc")
-                commands.append(f'echo "The PORT_{i} port is mapped to http://0.0.0.0:$PORT_{i}"')
-            commands.append("echo")
         commands.extend(
             [
                 "pip install ipykernel -q",
                 "mkdir -p /tmp",
                 'if [ $(uname -m) = "aarch64" ]; then arch="arm64"; else arch="x64"; fi',
                 f"wget -q https://github.com/gitpod-io/openvscode-server/releases/download/"
                 f"openvscode-server-v{self.version}/openvscode-server-v{self.version}-linux-$arch.tar.gz -O "
@@ -131,14 +112,14 @@
                 f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --install-extension ms-python.python",
                 "rm /usr/bin/python2*",
             ]
         )
         if self.setup:
             commands.extend(self.setup)
         commands.append(
-            f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --port $_PORT --host 0.0.0.0 --connection-token $CONNECTION_TOKEN --default-folder /workflow"
+            f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --port $PORT_0 --host 0.0.0.0 --connection-token $CONNECTION_TOKEN --default-folder /workflow"
         )
         return commands
 
 
 def __provider__():
     return CodeProvider()
```

### Comparing `dstack-0.7.2/cli/dstack/providers/docker/main.py` & `dstack-0.7rc1/cli/dstack/providers/docker/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/lab/main.py` & `dstack-0.7rc1/cli/dstack/providers/lab/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/providers/notebook/main.py` & `dstack-0.7rc1/cli/dstack/providers/notebook/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/utils/common.py` & `dstack-0.7rc1/cli/dstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/utils/interpolator.py` & `dstack-0.7rc1/cli/dstack/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack/utils/random_names.py` & `dstack-0.7rc1/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/dstack.egg-info/PKG-INFO` & `dstack-0.7rc1/cli/dstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstack
-Version: 0.7.2
+Version: 0.7rc1
 Summary: The hassle-free tool for managing ML workflows on any cloud platform.
 Home-page: https://dstack.ai
 Author: Andrey Cheptsov
 Author-email: andrey@dstack.ai
 License: UNKNOWN
 Project-URL: Source, https://github.com/dstackai/dstack
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dstack Version: 0.7.2 Summary: The hassle-free tool
-for managing ML workflows on any cloud platform. Home-page: https://dstack.ai
-Author: Andrey Cheptsov Author-email: andrey@dstack.ai License: UNKNOWN
-Project-URL: Source, https://github.com/dstackai/dstack Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
+Metadata-Version: 2.1 Name: dstack Version: 0.7rc1 Summary: The hassle-free
+tool for managing ML workflows on any cloud platform. Home-page: https://
+dstack.ai Author: Andrey Cheptsov Author-email: andrey@dstack.ai License:
+UNKNOWN Project-URL: Source, https://github.com/dstackai/dstack Platform:
+UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: OSI
 Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE.md
                             ****** [dstack] ******
                 *** Automate your ML workflows on any cloud ***
      The hassle-free tool for managing ML workflows on any cloud platform.
```

### Comparing `dstack-0.7.2/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.7rc1/cli/dstack.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -158,17 +158,13 @@
 cli/tests/hub/__init__.py
 cli/tests/hub/common.py
 cli/tests/hub/conftest.py
 cli/tests/hub/routers/__init__.py
 cli/tests/hub/routers/test_jobs.py
 cli/tests/hub/routers/test_projects.py
 cli/tests/hub/routers/test_users.py
-cli/tests/integration/__init__.py
-cli/tests/integration/common.py
-cli/tests/integration/conftest.py
-cli/tests/integration/test_commands.py
 cli/tests/providers/__init__.py
 cli/tests/providers/test_local_path.py
 cli/tests/providers/docker/__init__.py
 cli/tests/providers/docker/test_entrypoint.py
 cli/tests/utils/__init__.py
 cli/tests/utils/test_interpolator.py
```

### Comparing `dstack-0.7.2/cli/tests/backend/base/test_logs.py` & `dstack-0.7rc1/cli/tests/backend/base/test_logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/hub/common.py` & `dstack-0.7rc1/cli/tests/hub/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/hub/routers/test_jobs.py` & `dstack-0.7rc1/cli/tests/hub/routers/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/hub/routers/test_projects.py` & `dstack-0.7rc1/cli/tests/hub/routers/test_projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/hub/routers/test_users.py` & `dstack-0.7rc1/cli/tests/hub/routers/test_users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/providers/docker/test_entrypoint.py` & `dstack-0.7rc1/cli/tests/providers/docker/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/providers/test_local_path.py` & `dstack-0.7rc1/cli/tests/providers/test_local_path.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/cli/tests/utils/test_interpolator.py` & `dstack-0.7rc1/cli/tests/utils/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.7.2/setup.py` & `dstack-0.7rc1/setup.py`

 * *Files identical despite different names*

