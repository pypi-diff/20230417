# Comparing `tmp/globus-compute-endpoint-2.0.1a0.tar.gz` & `tmp/globus-compute-endpoint-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.1a0.tar", last modified: Fri Apr 14 15:04:24 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.1a1.tar", last modified: Mon Apr 17 19:01:13 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.1a0.tar` & `globus-compute-endpoint-2.0.1a1.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728863 globus-compute-endpoint-2.0.1a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-14 15:04:24.728943 globus-compute-endpoint-2.0.1a0/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.712566 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.723125 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24955 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724002 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724434 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724593 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.726758 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8427 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.726980 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.727456 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728325 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-14 15:02:34.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.713578 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2637 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-14 15:04:24.729232 globus-compute-endpoint-2.0.1a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3179 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728714 globus-compute-endpoint-2.0.1a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a0/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/tests/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.176264 globus-compute-endpoint-2.0.1a1/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 18:57:51.000000 globus-compute-endpoint-2.0.1a1/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     1646 2023-04-17 19:01:13.176355 globus-compute-endpoint-2.0.1a1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      871 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/PyPI.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.165547 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)      131 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    18802 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.168805 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2895 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 chris      (501) staff       (20)      772 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 chris      (501) staff       (20)    26053 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 chris      (501) staff       (20)    19658 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)    24955 2023-04-12 19:39:07.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 chris      (501) staff       (20)     2773 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.169844 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 chris      (501) staff       (20)      307 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      689 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 chris      (501) staff       (20)    11834 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 chris      (501) staff       (20)     3068 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 chris      (501) staff       (20)    14076 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 chris      (501) staff       (20)     5184 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 chris      (501) staff       (20)     7275 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.170257 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 chris      (501) staff       (20)     1017 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     6026 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 chris      (501) staff       (20)     1834 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 chris      (501) staff       (20)      220 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.170457 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/
+-rw-r--r--   0 chris      (501) staff       (20)      141 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.173398 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2104 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 chris      (501) staff       (20)    34995 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 chris      (501) staff       (20)    48886 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 chris      (501) staff       (20)     9712 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 chris      (501) staff       (20)      267 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 chris      (501) staff       (20)    35860 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     9114 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 chris      (501) staff       (20)     8401 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 chris      (501) staff       (20)    18606 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 chris      (501) staff       (20)     5433 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 chris      (501) staff       (20)     8219 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.173695 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/
+-rw-r--r--   0 chris      (501) staff       (20)      115 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.174298 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    12874 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 chris      (501) staff       (20)       50 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.175416 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/
+-rw-r--r--   0 chris      (501) staff       (20)      280 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7018 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     5106 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 chris      (501) staff       (20)     6145 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 chris      (501) staff       (20)     1610 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 chris      (501) staff       (20)      806 2023-04-17 19:00:11.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.166460 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     1646 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2657 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      359 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       30 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      282 2023-04-17 19:01:13.176709 globus-compute-endpoint-2.0.1a1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     3384 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.175990 globus-compute-endpoint-2.0.1a1/tests/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2693 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/conftest.py
+-rw-r--r--   0 chris      (501) staff       (20)     2276 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.1a0/LICENSE` & `globus-compute-endpoint-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         while True:
             log.debug("Waiting for task")
             p_task_id, p_container_id, msg = self.task_socket.recv_multipart()
             task_id: str = dill.loads(p_task_id)
             container_id: str = dill.loads(p_container_id)
             log.debug(f"Received task with task_id='{task_id}' and msg='{msg}'")
 
-            result = None
             if task_id == "KILL":
                 log.info("[KILL] -- Worker KILL message received! ")
                 # send a "worker die" message back to the manager
                 self.task_socket.send_multipart([b"WRKR_DIE", b""])
                 log.info(f"*** WORKER {self.worker_id} ABOUT TO DIE ***")
                 # Kill the worker after accepting death in message to manager.
                 sys.exit()
```

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a0"
+__version__ = "2.0.1a1"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 LICENSE
+MANIFEST.in
+PyPI.md
 setup.cfg
 setup.py
 globus_compute_endpoint/__init__.py
 globus_compute_endpoint/cli.py
 globus_compute_endpoint/exception_handling.py
 globus_compute_endpoint/exceptions.py
 globus_compute_endpoint/logging_config.py
```

### Comparing `globus-compute-endpoint-2.0.1a0/setup.py` & `globus-compute-endpoint-2.0.1a1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
     "globus-compute-sdk>=2.0.0",
@@ -47,19 +48,24 @@
 
 
 version_ns = {}
 with open(os.path.join("globus_compute_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
 
+directory = Path(__file__).parent
+long_description = (directory / "PyPI.md").read_text()
+
 setup(
     name="globus-compute-endpoint",
     version=version,
     packages=find_packages(),
     description="Globus Compute: High Performance Function Serving for Science",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     extras_require={
         "test": TEST_REQUIRES,
     },
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `globus-compute-endpoint-2.0.1a0/tests/conftest.py` & `globus-compute-endpoint-2.0.1a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a0/tests/utils.py` & `globus-compute-endpoint-2.0.1a1/tests/utils.py`

 * *Files identical despite different names*

