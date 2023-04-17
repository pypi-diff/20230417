# Comparing `tmp/xmanager-0.3.0.tar.gz` & `tmp/xmanager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmanager-0.3.0.tar", last modified: Fri Sep 30 14:43:39 2022, max compression
+gzip compressed data, was "xmanager-0.4.0.tar", last modified: Mon Apr 17 14:54:14 2023, max compression
```

## Comparing `xmanager-0.3.0.tar` & `xmanager-0.4.0.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11358 2021-04-06 14:47:01.000000 xmanager-0.3.0/LICENSE
--rw-r-----   0 chenandrew (446784) primarygroup (89939)    11848 2022-09-30 14:43:39.643558 xmanager-0.3.0/PKG-INFO
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11477 2022-09-30 14:42:11.000000 xmanager-0.3.0/README.md
--rw-r-----   0 chenandrew (446784) primarygroup (89939)       38 2022-09-30 14:43:39.643558 xmanager-0.3.0/setup.cfg
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2103 2022-09-30 14:32:05.000000 xmanager-0.3.0/setup.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.619556 xmanager-0.3.0/setup_scripts/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      805 2022-07-22 12:42:42.000000 xmanager-0.3.0/setup_scripts/install_bazel.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      766 2022-07-22 12:42:42.000000 xmanager-0.3.0/setup_scripts/install_docker.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1100 2022-07-22 12:42:42.000000 xmanager-0.3.0/setup_scripts/install_gcloud.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      980 2022-07-22 12:42:42.000000 xmanager-0.3.0/setup_scripts/install_python.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1147 2022-09-30 14:42:11.000000 xmanager-0.3.0/setup_scripts/install_xmanager.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      878 2022-07-22 12:42:42.000000 xmanager-0.3.0/setup_scripts/setup_all.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4493 2022-09-30 14:42:11.000000 xmanager-0.3.0/setup_scripts/setup_gcp.sh
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.615556 xmanager-0.3.0/xmanager/
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.619556 xmanager-0.3.0/xmanager/bazel/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1907 2021-11-05 10:26:16.000000 xmanager-0.3.0/xmanager/bazel/client.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1067 2021-03-31 19:56:12.000000 xmanager-0.3.0/xmanager/bazel/file_utils.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.619556 xmanager-0.3.0/xmanager/cli/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2310 2021-09-29 12:38:48.000000 xmanager-0.3.0/xmanager/cli/cli.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.627556 xmanager-0.3.0/xmanager/cloud/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      594 2021-03-31 19:56:12.000000 xmanager-0.3.0/xmanager/cloud/__init__.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6147 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/auth.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9213 2022-09-06 12:53:07.000000 xmanager-0.3.0/xmanager/cloud/auth_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    13613 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/build_image.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2364 2022-05-20 02:55:36.000000 xmanager-0.3.0/xmanager/cloud/build_image_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9457 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/cloud_build.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3660 2022-05-20 02:55:36.000000 xmanager-0.3.0/xmanager/cloud/cloud_build_test.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.627556 xmanager-0.3.0/xmanager/cloud/data/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      896 2022-01-18 22:49:12.000000 xmanager-0.3.0/xmanager/cloud/data/wrapped_entrypoint.sh
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6610 2022-03-03 23:11:43.000000 xmanager-0.3.0/xmanager/cloud/docker_lib.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8917 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/kubernetes.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6978 2022-09-09 12:30:59.000000 xmanager-0.3.0/xmanager/cloud/kubernetes_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5268 2022-01-18 22:49:12.000000 xmanager-0.3.0/xmanager/cloud/utils.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2911 2021-03-31 19:56:12.000000 xmanager-0.3.0/xmanager/cloud/utils_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    14234 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/vertex.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7404 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/cloud/vertex_test.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.631557 xmanager-0.3.0/xmanager/contrib/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      594 2021-09-07 10:43:23.000000 xmanager-0.3.0/xmanager/contrib/__init__.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1409 2022-08-17 14:02:23.000000 xmanager-0.3.0/xmanager/contrib/addressing.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1125 2022-08-17 14:02:23.000000 xmanager-0.3.0/xmanager/contrib/addressing_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3081 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/copybara.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4127 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/executor_selector.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3841 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/framework_defaults.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4051 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/framework_defaults_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4566 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/gcs.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3823 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/gcs_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8501 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/parameter_controller.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3225 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/tensorboard.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4700 2022-09-29 12:15:23.000000 xmanager-0.3.0/xmanager/contrib/tensorboard_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1202 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/contrib/tpu.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7369 2022-08-17 14:05:02.000000 xmanager-0.3.0/xmanager/contrib/xm_tensorflow.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6462 2022-08-17 14:05:02.000000 xmanager-0.3.0/xmanager/contrib/xm_tensorflow_test.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.631557 xmanager-0.3.0/xmanager/docker/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5869 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/docker/docker_adapter.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.631557 xmanager-0.3.0/xmanager/generated/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    71522 2022-07-11 09:11:59.000000 xmanager-0.3.0/xmanager/generated/build_event_stream_pb2.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4621 2022-07-11 09:11:59.000000 xmanager-0.3.0/xmanager/generated/command_line_pb2.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9504 2021-09-07 18:04:29.000000 xmanager-0.3.0/xmanager/generated/data_pb2.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)   190389 2022-07-11 09:11:59.000000 xmanager-0.3.0/xmanager/generated/failure_details_pb2.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5842 2022-07-11 09:11:59.000000 xmanager-0.3.0/xmanager/generated/invocation_policy_pb2.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3416 2022-07-11 09:11:59.000000 xmanager-0.3.0/xmanager/generated/option_filters_pb2.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.615556 xmanager-0.3.0/xmanager/vizier/
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.635557 xmanager-0.3.0/xmanager/vizier/vizier_cloud/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      811 2022-03-23 19:16:10.000000 xmanager-0.3.0/xmanager/vizier/vizier_cloud/__init__.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2906 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/vizier/vizier_cloud/study_factory.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6743 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_controller.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2535 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_exploration.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2419 2022-03-23 19:16:10.000000 xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_worker.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.639557 xmanager-0.3.0/xmanager/xm/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3546 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/__init__.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3871 2022-03-29 08:33:52.000000 xmanager-0.3.0/xmanager/xm/async_packager.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2971 2021-09-28 13:29:05.000000 xmanager-0.3.0/xmanager/xm/async_packager_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      997 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/compute_units.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    32128 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/core.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11858 2022-07-14 18:31:46.000000 xmanager-0.3.0/xmanager/xm/core_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6889 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/executables.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1894 2021-11-03 11:28:47.000000 xmanager-0.3.0/xmanager/xm/executables_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3943 2021-11-30 12:26:48.000000 xmanager-0.3.0/xmanager/xm/id_predictor.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2094 2021-03-31 19:56:12.000000 xmanager-0.3.0/xmanager/xm/id_predictor_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    15225 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/job_blocks.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3323 2022-09-08 12:52:14.000000 xmanager-0.3.0/xmanager/xm/job_blocks_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4167 2022-09-12 05:14:45.000000 xmanager-0.3.0/xmanager/xm/job_operators.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2823 2022-04-25 10:01:02.000000 xmanager-0.3.0/xmanager/xm/job_operators_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1773 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/metadata_context.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11054 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/packagables.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5351 2021-11-10 14:35:43.000000 xmanager-0.3.0/xmanager/xm/packagables_generator.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1678 2021-11-04 12:19:16.000000 xmanager-0.3.0/xmanager/xm/packagables_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4236 2021-11-19 11:02:11.000000 xmanager-0.3.0/xmanager/xm/pattern_matching.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2928 2021-11-19 11:02:11.000000 xmanager-0.3.0/xmanager/xm/pattern_matching_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    15404 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/resources.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8360 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/resources_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5137 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm/utils.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1592 2022-07-22 09:58:39.000000 xmanager-0.3.0/xmanager/xm/utils_test.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.639557 xmanager-0.3.0/xmanager/xm_local/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      960 2022-05-28 00:21:12.000000 xmanager-0.3.0/xmanager/xm_local/__init__.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1404 2021-08-20 05:09:22.000000 xmanager-0.3.0/xmanager/xm_local/executables.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9332 2022-08-12 12:11:28.000000 xmanager-0.3.0/xmanager/xm_local/execution.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9215 2022-08-12 12:11:28.000000 xmanager-0.3.0/xmanager/xm_local/execution_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4662 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm_local/executors.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    15463 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm_local/experiment.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/xmanager/xm_local/packaging/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8789 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm_local/packaging/bazel_tools.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1850 2021-11-08 04:47:27.000000 xmanager-0.3.0/xmanager/xm_local/packaging/bazel_tools_test.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7507 2022-07-05 06:21:10.000000 xmanager-0.3.0/xmanager/xm_local/packaging/cloud.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5370 2021-11-05 10:46:18.000000 xmanager-0.3.0/xmanager/xm_local/packaging/local.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4105 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm_local/packaging/router.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1703 2021-09-17 21:16:26.000000 xmanager-0.3.0/xmanager/xm_local/status.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/xmanager/xm_local/storage/
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/xmanager/xm_local/storage/alembic/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2333 2022-09-22 17:33:46.000000 xmanager-0.3.0/xmanager/xm_local/storage/alembic/env.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1252 2022-09-22 17:33:46.000000 xmanager-0.3.0/xmanager/xm_local/storage/alembic/script.py.mako
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/xmanager/xm_local/storage/alembic/versions/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4930 2022-09-22 17:56:46.000000 xmanager-0.3.0/xmanager/xm_local/storage/alembic/versions/f45829405692_migrate_or_create.py
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3799 2022-09-22 17:33:46.000000 xmanager-0.3.0/xmanager/xm_local/storage/alembic.ini
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    14220 2022-09-30 14:42:11.000000 xmanager-0.3.0/xmanager/xm_local/storage/database.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.643558 xmanager-0.3.0/xmanager/xm_mock/
--rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6005 2022-06-28 23:01:41.000000 xmanager-0.3.0/xmanager/xm_mock/__init__.py
-drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2022-09-30 14:43:39.619556 xmanager-0.3.0/xmanager.egg-info/
--rw-r-----   0 chenandrew (446784) primarygroup (89939)    11848 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/PKG-INFO
--rw-r-----   0 chenandrew (446784) primarygroup (89939)     3373 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/SOURCES.txt
--rw-r-----   0 chenandrew (446784) primarygroup (89939)        1 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/dependency_links.txt
--rw-r-----   0 chenandrew (446784) primarygroup (89939)       57 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/entry_points.txt
--rw-r-----   0 chenandrew (446784) primarygroup (89939)      256 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/requires.txt
--rw-r-----   0 chenandrew (446784) primarygroup (89939)       42 2022-09-30 14:43:39.000000 xmanager-0.3.0/xmanager.egg-info/top_level.txt
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.519368 xmanager-0.4.0/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11358 2021-04-06 14:47:01.000000 xmanager-0.4.0/LICENSE
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)    11849 2023-04-17 14:54:14.519368 xmanager-0.4.0/PKG-INFO
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11477 2023-04-17 14:48:57.000000 xmanager-0.4.0/README.md
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)       38 2023-04-17 14:54:14.519368 xmanager-0.4.0/setup.cfg
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2150 2023-04-17 14:50:29.000000 xmanager-0.4.0/setup.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.499366 xmanager-0.4.0/setup_scripts/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      805 2022-07-22 12:42:42.000000 xmanager-0.4.0/setup_scripts/install_bazel.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      766 2022-07-22 12:42:42.000000 xmanager-0.4.0/setup_scripts/install_docker.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1100 2022-07-22 12:42:42.000000 xmanager-0.4.0/setup_scripts/install_gcloud.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      980 2022-07-22 12:42:42.000000 xmanager-0.4.0/setup_scripts/install_python.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1147 2023-04-17 14:48:57.000000 xmanager-0.4.0/setup_scripts/install_xmanager.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      878 2022-07-22 12:42:42.000000 xmanager-0.4.0/setup_scripts/setup_all.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4493 2023-04-17 14:48:57.000000 xmanager-0.4.0/setup_scripts/setup_gcp.sh
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.495366 xmanager-0.4.0/xmanager/
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.499366 xmanager-0.4.0/xmanager/bazel/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1897 2023-01-30 18:29:40.000000 xmanager-0.4.0/xmanager/bazel/client.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1067 2021-03-31 19:56:12.000000 xmanager-0.4.0/xmanager/bazel/file_utils.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.499366 xmanager-0.4.0/xmanager/cli/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2328 2023-01-30 18:29:40.000000 xmanager-0.4.0/xmanager/cli/cli.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.503366 xmanager-0.4.0/xmanager/cloud/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      594 2021-03-31 19:56:12.000000 xmanager-0.4.0/xmanager/cloud/__init__.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6201 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/auth.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9634 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/auth_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    13537 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/build_image.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2364 2022-05-20 02:55:36.000000 xmanager-0.4.0/xmanager/cloud/build_image_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9741 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/cloud_build.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3764 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/cloud_build_test.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.503366 xmanager-0.4.0/xmanager/cloud/data/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      896 2022-01-18 22:49:12.000000 xmanager-0.4.0/xmanager/cloud/data/wrapped_entrypoint.sh
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6475 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/docker_lib.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8970 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/kubernetes.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7069 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/kubernetes_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5261 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/utils.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2923 2023-01-30 17:14:56.000000 xmanager-0.4.0/xmanager/cloud/utils_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    13990 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/vertex.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7150 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/cloud/vertex_test.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.507367 xmanager-0.4.0/xmanager/contrib/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      594 2021-09-07 10:43:23.000000 xmanager-0.4.0/xmanager/contrib/__init__.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1362 2023-01-30 18:47:40.000000 xmanager-0.4.0/xmanager/contrib/addressing.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1137 2023-01-30 18:47:40.000000 xmanager-0.4.0/xmanager/contrib/addressing_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3061 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/copybara.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4152 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/executor_selector.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5070 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/flow.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4035 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/framework_defaults.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4082 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/framework_defaults_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4619 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/gcs.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3831 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/gcs_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8513 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/parameter_controller.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3275 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/tensorboard.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4530 2023-01-30 18:47:40.000000 xmanager-0.4.0/xmanager/contrib/tensorboard_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1254 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/contrib/tpu.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7186 2023-01-30 18:47:40.000000 xmanager-0.4.0/xmanager/contrib/xm_tensorflow.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6452 2023-01-30 18:47:40.000000 xmanager-0.4.0/xmanager/contrib/xm_tensorflow_test.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.507367 xmanager-0.4.0/xmanager/docker/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5907 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/docker/docker_adapter.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.507367 xmanager-0.4.0/xmanager/generated/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    35712 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/build_event_stream_pb2.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2990 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/command_line_pb2.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2284 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/data_pb2.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)   165371 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/failure_details_pb2.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3679 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/invocation_policy_pb2.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2753 2023-03-02 13:30:05.000000 xmanager-0.4.0/xmanager/generated/option_filters_pb2.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.495366 xmanager-0.4.0/xmanager/vizier/
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.511367 xmanager-0.4.0/xmanager/vizier/vizier_cloud/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      811 2022-03-23 19:16:10.000000 xmanager-0.4.0/xmanager/vizier/vizier_cloud/__init__.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2913 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/vizier/vizier_cloud/study_factory.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7002 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_controller.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2526 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_exploration.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2473 2023-01-30 18:29:40.000000 xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_worker.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.515368 xmanager-0.4.0/xmanager/xm/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3546 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/__init__.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4210 2023-02-23 10:40:46.000000 xmanager-0.4.0/xmanager/xm/async_packager.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3386 2023-02-23 10:40:46.000000 xmanager-0.4.0/xmanager/xm/async_packager_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      997 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/compute_units.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    32252 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/core.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11604 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/core_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     6950 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/executables.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1899 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/executables_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3961 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/id_predictor.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2094 2021-03-31 19:56:12.000000 xmanager-0.4.0/xmanager/xm/id_predictor_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    16324 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/job_blocks.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3663 2023-02-01 12:15:01.000000 xmanager-0.4.0/xmanager/xm/job_blocks_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4162 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/job_operators.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2827 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/job_operators_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1773 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/metadata_context.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    11072 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/packagables.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5397 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/packagables_generator.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1678 2021-11-04 12:19:16.000000 xmanager-0.4.0/xmanager/xm/packagables_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4224 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/pattern_matching.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2901 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/pattern_matching_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    15542 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/resources.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8408 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/resources_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5109 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm/utils.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1597 2023-01-30 19:15:49.000000 xmanager-0.4.0/xmanager/xm/utils_test.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.515368 xmanager-0.4.0/xmanager/xm_local/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)      960 2022-05-28 00:21:12.000000 xmanager-0.4.0/xmanager/xm_local/__init__.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1404 2021-08-20 05:09:22.000000 xmanager-0.4.0/xmanager/xm_local/executables.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9342 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/execution.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     9343 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/execution_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4667 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm_local/executors.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    15275 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm_local/experiment.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.515368 xmanager-0.4.0/xmanager/xm_local/packaging/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     8921 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm_local/packaging/bazel_tools.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2548 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/packaging/bazel_tools_test.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     7441 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/packaging/cloud.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5274 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/packaging/local.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4103 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm_local/packaging/router.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1683 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/status.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.519368 xmanager-0.4.0/xmanager/xm_local/storage/
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.519368 xmanager-0.4.0/xmanager/xm_local/storage/alembic/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     2181 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/storage/alembic/env.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     1252 2022-09-22 17:33:46.000000 xmanager-0.4.0/xmanager/xm_local/storage/alembic/script.py.mako
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.519368 xmanager-0.4.0/xmanager/xm_local/storage/alembic/versions/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     4987 2023-01-30 14:38:00.000000 xmanager-0.4.0/xmanager/xm_local/storage/alembic/versions/f45829405692_migrate_or_create.py
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     3297 2023-01-27 17:51:50.000000 xmanager-0.4.0/xmanager/xm_local/storage/alembic.ini
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)    14183 2023-04-17 14:48:57.000000 xmanager-0.4.0/xmanager/xm_local/storage/database.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.519368 xmanager-0.4.0/xmanager/xm_mock/
+-rw-rw-r--   0 chenandrew (446784) primarygroup (89939)     5983 2023-01-30 18:29:40.000000 xmanager-0.4.0/xmanager/xm_mock/__init__.py
+drwxr-x---   0 chenandrew (446784) primarygroup (89939)        0 2023-04-17 14:54:14.499366 xmanager-0.4.0/xmanager.egg-info/
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)    11849 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/PKG-INFO
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)     3398 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/SOURCES.txt
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)        1 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/dependency_links.txt
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)       57 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/entry_points.txt
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)      269 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/requires.txt
+-rw-r-----   0 chenandrew (446784) primarygroup (89939)       42 2023-04-17 14:54:14.000000 xmanager-0.4.0/xmanager.egg-info/top_level.txt
```

### Comparing `xmanager-0.3.0/LICENSE` & `xmanager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/PKG-INFO` & `xmanager-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xmanager
-Version: 0.3.0
+Version: 0.4.0
 Summary: A framework for managing machine learning experiments
 Author: DeepMind Technologies Limited
 Project-URL: Homepage, https://github.com/deepmind/xmanager
 Project-URL: Issue tracker, https://github.com/deepmind/xmanager/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XManager: A framework for managing machine learning experiments 🧑‍🔬
 
 <!-- Note that links in README.md have to be absolute as it also lands on PyPI. -->
```

### Comparing `xmanager-0.3.0/README.md` & `xmanager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup.py` & `xmanager-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,44 +17,47 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
   long_description = fh.read()
 
 setup(
     name='xmanager',
-    version='0.3.0',
+    version='0.4.0',
     description='A framework for managing machine learning experiments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepMind Technologies Limited',
     packages=find_namespace_packages(exclude=['examples.*']),
     package_data={'': ['*.sh', '*.sql', '*.ini', '*.mako']},
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     install_requires=[
         'absl-py',
         'alembic==1.4.3',
         'async_generator',
         'attrs',
         'cloud-sql-python-connector',
         'docker',
+        'etils[epath]',
         'google-api-core',
         'google-api-python-client',
         'google-auth',
         'google-cloud-aiplatform',
         'google-cloud-storage',
         'humanize',
         'immutabledict',
         'kubernetes',
         'pyyaml',
         'sqlalchemy==1.2.19',
         'sqlparse',
         'termcolor',
     ],
     entry_points={
-        'console_scripts': ['xmanager = xmanager.cli.cli:entrypoint',],
+        'console_scripts': [
+            'xmanager = xmanager.cli.cli:entrypoint',
+        ],
     },
     # https://github.com/pypa/warehouse/blob/de4a2e5e2ec26d01bf7813da427ebc4725dccde9/warehouse/templates/packaging/detail.html#L20-L60
     project_urls={
         'Homepage': 'https://github.com/deepmind/xmanager',
         'Issue tracker': 'https://github.com/deepmind/xmanager/issues',
     },
 )
```

### Comparing `xmanager-0.3.0/setup_scripts/install_bazel.sh` & `xmanager-0.4.0/setup_scripts/install_bazel.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/install_docker.sh` & `xmanager-0.4.0/setup_scripts/install_docker.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/install_gcloud.sh` & `xmanager-0.4.0/setup_scripts/install_gcloud.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/install_python.sh` & `xmanager-0.4.0/setup_scripts/install_python.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/install_xmanager.sh` & `xmanager-0.4.0/setup_scripts/install_xmanager.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/setup_all.sh` & `xmanager-0.4.0/setup_scripts/setup_all.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/setup_scripts/setup_gcp.sh` & `xmanager-0.4.0/setup_scripts/setup_gcp.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/bazel/client.py` & `xmanager-0.4.0/xmanager/bazel/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 
     Returns:
       A list of kinds, for example, `['py_binary rule']`.
     """
     raise NotImplementedError
 
   @abc.abstractmethod
-  def build_targets(self, labels: Sequence[str],
-                    tail_args: Sequence[str]) -> List[List[str]]:
+  def build_targets(
+      self, labels: Sequence[str], tail_args: Sequence[str]
+  ) -> List[List[str]]:
     """Builds given targets and returns paths to their important outputs.
 
     Args:
       labels: Labels of the targets to build.
       tail_args: Arguments to append to the Bazel command.
 
     Returns:
```

### Comparing `xmanager-0.3.0/xmanager/bazel/file_utils.py` & `xmanager-0.4.0/xmanager/bazel/file_utils.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/cli/cli.py` & `xmanager-0.4.0/xmanager/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,18 @@
     launch_script = argv[2]
     if not os.path.exists(launch_script):
       raise OSError(errno.ENOENT, f'File not found: {launch_script}')
     sys.path.insert(0, os.path.abspath(os.path.dirname(launch_script)))
     launch_module, _ = os.path.splitext(os.path.basename(launch_script))
     m = importlib.import_module(launch_module)
     sys.path.pop(0)
-    argv = [launch_script, '--xm_launch_script={}'.format(launch_script)
-           ] + argv[3:]
+    argv = [
+        launch_script,
+        '--xm_launch_script={}'.format(launch_script),
+    ] + argv[3:]
     app.run(m.main, argv=argv)
   elif cmd == 'cluster':
     caliban_gke = importlib.import_module('caliban.platform.gke.cli')
     caliban_gke_types = importlib.import_module('caliban.platform.gke.types')
     subcmd = argv[2]
     args = {
         'dry_run': False,
@@ -52,15 +54,16 @@
     }
     if subcmd == 'create':
       caliban_gke._cluster_create(args)  # pylint: disable=protected-access
     elif subcmd == 'delete':
       caliban_gke._cluster_delete(args)  # pylint: disable=protected-access
     else:
       raise app.UsageError(
-          f'Subcommand `{cmd} {subcmd}` is not a supported subcommand')
+          f'Subcommand `{cmd} {subcmd}` is not a supported subcommand'
+      )
   else:
     raise app.UsageError(f'Command `{cmd}` is not a supported command')
 
 
 def entrypoint():
   app.run(main)
```

### Comparing `xmanager-0.3.0/xmanager/cloud/__init__.py` & `xmanager-0.4.0/xmanager/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/cloud/auth.py` & `xmanager-0.4.0/xmanager/cloud/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,19 +21,23 @@
 from google import auth
 from googleapiclient import discovery
 from googleapiclient import errors
 
 _DEFAULT_SCOPES = ('https://www.googleapis.com/auth/cloud-platform',)
 
 _GCP_SERVICE_ACCOUNT_NAME = flags.DEFINE_string(
-    'xm_gcp_service_account_name', 'xmanager',
-    'Specifies the user-managed service account name to be used by XManager'
-    'Note that user-managed service accounts have the following format: '
-    '`{service-account-name}@{project-id}.iam.gserviceaccount.com`, so only'
-    'the part before @ is required')
+    'xm_gcp_service_account_name',
+    'xmanager',
+    (
+        'Specifies the user-managed service account name to be used by XManager'
+        'Note that user-managed service accounts have the following format: '
+        '`{service-account-name}@{project-id}.iam.gserviceaccount.com`, so only'
+        'the part before @ is required'
+    ),
+)
 
 
 def get_project_name() -> str:
   """Gets the Project ID of the GCP Project."""
   _, project = auth.default()
   return project
 
@@ -67,15 +71,16 @@
           'iam.googleapis.com',
           'logging.googleapis.com',
           'storage-api.googleapis.com',
           'tpu.googleapis.com',
       ]
   }
   resource.services().batchEnable(
-      parent=f'projects/{get_project_number()}', body=body).execute()
+      parent=f'projects/{get_project_number()}', body=body
+  ).execute()
 
 
 def get_service_account() -> str:
   """Gets or creates the service account for running XManager in GCP.
 
   The default Vertex AI Training Service Agent has limited scopes. It is more
   useful to use a custom service account that can access a greater number of
@@ -87,16 +92,17 @@
   Returns:
     The service account email.
   Raises:
     HttpError: if the response was not a 2xx or 403.
   """
 
   service_account_name = _GCP_SERVICE_ACCOUNT_NAME.value
-  service_account = (f'{service_account_name}@{get_project_name()}'
-                     '.iam.gserviceaccount.com')
+  service_account = (
+      f'{service_account_name}@{get_project_name()}.iam.gserviceaccount.com'
+  )
 
   try:
     _maybe_create_service_account(service_account)
     _maybe_grant_service_account_permissions(service_account)
   except errors.HttpError as e:
     # A 403 implies that the user is not an IAM Admin or Cloud Resource Manager
     # API is not enabled.
@@ -106,30 +112,38 @@
       raise e
   return service_account
 
 
 def _maybe_create_service_account(service_account: str) -> None:
   """Creates the default service account if it does not exist."""
   iam = discovery.build('iam', 'v1')
-  accounts = iam.projects().serviceAccounts().list(
-      name='projects/' + get_project_name()).execute()
+  accounts = (
+      iam.projects()
+      .serviceAccounts()
+      .list(name='projects/' + get_project_name())
+      .execute()
+  )
   for account in accounts.get('accounts', []):
     if account['email'] == service_account:
       return
 
   # https://cloud.google.com/iam/docs/reference/rest/v1/projects.serviceAccounts
   body = {
       'accountId': service_account.split('@')[0],
       'serviceAccount': {
           'displayName': service_account.split('@')[0],
           'description': 'XManager service account',
       },
   }
-  accounts = iam.projects().serviceAccounts().create(
-      name='projects/' + get_project_name(), body=body).execute()
+  accounts = (
+      iam.projects()
+      .serviceAccounts()
+      .create(name='projects/' + get_project_name(), body=body)
+      .execute()
+  )
 
 
 def _maybe_grant_service_account_permissions(service_account: str) -> None:
   """Grants the default service account IAM permissions if necessary."""
   rm = discovery.build('cloudresourcemanager', 'v1')
   policy = rm.projects().getIamPolicy(resource=get_project_name()).execute()
   want_roles = ['roles/aiplatform.user', 'roles/storage.admin']
@@ -143,16 +157,17 @@
   if not should_set:
     return None
 
   body = {'policy': policy}
   rm.projects().setIamPolicy(resource=get_project_name(), body=body).execute()
 
 
-def _add_member_to_iam_policy(policy: Dict[str, Any], role: str,
-                              member: str) -> bool:
+def _add_member_to_iam_policy(
+    policy: Dict[str, Any], role: str, member: str
+) -> bool:
   """Modifies the IAM policy to add the member with the role."""
   for i, binding in enumerate(policy['bindings']):
     if binding['role'] == role:
       if member in binding['members']:
         return False
       policy['bindings'][i]['members'].append(member)
       return True
@@ -166,8 +181,9 @@
   if bucket:
     return bucket
   raise ValueError(
       '$GOOGLE_CLOUD_BUCKET_NAME is undefined. Run '
       '`export GOOGLE_CLOUD_BUCKET_NAME=<bucket-name>`, '
       'replacing <bucket-name> with a Google Cloud Storage bucket. '
       'You can create a bucket with '
-      '`gsutil mb -l us-central1 gs://$GOOGLE_CLOUD_BUCKET_NAME`')
+      '`gsutil mb -l us-central1 gs://$GOOGLE_CLOUD_BUCKET_NAME`'
+  )
```

### Comparing `xmanager-0.3.0/xmanager/cloud/auth_test.py` & `xmanager-0.4.0/xmanager/cloud/auth_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,79 +8,90 @@
 from absl.testing import parameterized
 from googleapiclient import discovery
 from xmanager.cloud import auth
 
 _TEST_SERVICE_ACCOUNT_NAME = 'test-service-account'
 _DEFAULT_SERVICE_ACCOUNT_NAME = 'xmanager'
 
-_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS = [{
-    'sys_argv': sys.argv,
-    'expected_account_name': _DEFAULT_SERVICE_ACCOUNT_NAME
-}, {
-    'sys_argv': [
-        *sys.argv, f'--xm_gcp_service_account_name={_TEST_SERVICE_ACCOUNT_NAME}'
-    ],
-    'expected_account_name': _TEST_SERVICE_ACCOUNT_NAME
-}]
+_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS = [
+    {
+        'sys_argv': sys.argv,
+        'expected_account_name': _DEFAULT_SERVICE_ACCOUNT_NAME,
+    },
+    {
+        'sys_argv': [
+            *sys.argv,
+            f'--xm_gcp_service_account_name={_TEST_SERVICE_ACCOUNT_NAME}',
+        ],
+        'expected_account_name': _TEST_SERVICE_ACCOUNT_NAME,
+    },
+]
 
 
 class GetServiceAccountTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
     # Resets flags between runs
     flags.FLAGS.unparse_flags()
 
   @parameterized.parameters(_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS)
-  def test_get_service_account_existing_account(self, sys_argv,
-                                                expected_account_name):
+  def test_get_service_account_existing_account(
+      self, sys_argv, expected_account_name
+  ):
     """Tests that `get_service_account` does nothing on a properly configured account."""
 
     flags.FLAGS(sys_argv)
 
     mock_service_accounts = mock.Mock()
     mock_service_accounts.list.return_value.execute.return_value = {
-        'accounts': [{
-            'email':
-                f'{expected_account_name}@test-project.iam.gserviceaccount.com'
-        }]
+        'accounts': [
+            {
+                'email': f'{expected_account_name}@test-project.iam.gserviceaccount.com'
+            }
+        ]
     }
     mock_service_accounts.create.return_value.execute.return_value = None
 
     mock_projects = mock.Mock()
     mock_projects.serviceAccounts.return_value = mock_service_accounts
     mock_projects.getIamPolicy.return_value.execute.return_value = {
-        'bindings': [{
-            'role':
-                'roles/aiplatform.user',
-            'members': [(f'serviceAccount:{expected_account_name}'
-                         '@test-project.iam.gserviceaccount.com')]
-        }, {
-            'role':
-                'roles/storage.admin',
-            'members': [(f'serviceAccount:{expected_account_name}'
-                         '@test-project.iam.gserviceaccount.com')]
-        }]
+        'bindings': [
+            {
+                'role': 'roles/aiplatform.user',
+                'members': [
+                    f'serviceAccount:{expected_account_name}'
+                    '@test-project.iam.gserviceaccount.com'
+                ],
+            },
+            {
+                'role': 'roles/storage.admin',
+                'members': [
+                    f'serviceAccount:{expected_account_name}'
+                    '@test-project.iam.gserviceaccount.com'
+                ],
+            },
+        ]
     }
 
     mock_discovery_build = mock.Mock()
     mock_discovery_build.projects.return_value = mock_projects
 
-    with mock.patch.object(auth, 'get_project_name',
-                           return_value='test-project'), \
-         mock.patch.object(discovery, 'build',
-                           return_value=mock_discovery_build):
+    with mock.patch.object(
+        auth, 'get_project_name', return_value='test-project'
+    ), mock.patch.object(discovery, 'build', return_value=mock_discovery_build):
       auth.get_service_account()
 
     mock_service_accounts.create.assert_not_called()
     mock_projects.setIamPolicy.assert_not_called()
 
   @parameterized.parameters(_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS)
-  def test_get_service_account_new_account(self, sys_argv,
-                                           expected_account_name):
+  def test_get_service_account_new_account(
+      self, sys_argv, expected_account_name
+  ):
     """Tests if `get_service_account` creates a new account and permissions properly."""
 
     flags.FLAGS(sys_argv)
 
     mock_service_accounts = mock.Mock()
     mock_service_accounts.list.return_value.execute.return_value = {}
     mock_service_accounts.create.return_value.execute.return_value = None
@@ -90,162 +101,190 @@
     mock_projects.getIamPolicy.return_value.execute.return_value = {
         'bindings': []
     }
 
     mock_discovery_build = mock.Mock()
     mock_discovery_build.projects.return_value = mock_projects
 
-    with mock.patch.object(auth, 'get_project_name',
-                           return_value='test-project'), \
-         mock.patch.object(discovery, 'build',
-                           return_value=mock_discovery_build):
+    with mock.patch.object(
+        auth, 'get_project_name', return_value='test-project'
+    ), mock.patch.object(discovery, 'build', return_value=mock_discovery_build):
       auth.get_service_account()
 
     mock_service_accounts.create.assert_called_once_with(
         name='projects/test-project',
         body={
             'accountId': expected_account_name,
             'serviceAccount': {
                 'displayName': expected_account_name,
-                'description': 'XManager service account'
-            }
-        })
+                'description': 'XManager service account',
+            },
+        },
+    )
 
     mock_projects.setIamPolicy.assert_called_once_with(
         resource='test-project',
         body={
             'policy': {
-                'bindings': [{
-                    'role':
-                        'roles/aiplatform.user',
-                    'members': [(f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }, {
-                    'role':
-                        'roles/storage.admin',
-                    'members': [(f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }]
+                'bindings': [
+                    {
+                        'role': 'roles/aiplatform.user',
+                        'members': [
+                            f'serviceAccount:{expected_account_name}'
+                            '@test-project.iam.gserviceaccount.com'
+                        ],
+                    },
+                    {
+                        'role': 'roles/storage.admin',
+                        'members': [
+                            f'serviceAccount:{expected_account_name}'
+                            '@test-project.iam.gserviceaccount.com'
+                        ],
+                    },
+                ]
             }
-        })
+        },
+    )
 
   @parameterized.parameters(_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS)
-  def test_get_service_account_no_permissions(self, sys_argv,
-                                              expected_account_name):
+  def test_get_service_account_no_permissions(
+      self, sys_argv, expected_account_name
+  ):
     """Tests if `get_service_account` creates permissions properly for an existing account with no permissions."""
 
     flags.FLAGS(sys_argv)
 
     mock_service_accounts = mock.Mock()
     mock_service_accounts.list.return_value.execute.return_value = {
-        'accounts': [{
-            'email':
-                f'{expected_account_name}@test-project.iam.gserviceaccount.com'
-        }]
+        'accounts': [
+            {
+                'email': f'{expected_account_name}@test-project.iam.gserviceaccount.com'
+            }
+        ]
     }
     mock_service_accounts.create.return_value.execute.return_value = None
 
     mock_projects = mock.Mock()
     mock_projects.serviceAccounts.return_value = mock_service_accounts
     mock_projects.getIamPolicy.return_value.execute.return_value = {
         'bindings': []
     }
 
     mock_discovery_build = mock.Mock()
     mock_discovery_build.projects.return_value = mock_projects
 
-    with mock.patch.object(auth, 'get_project_name',
-                           return_value='test-project'), \
-         mock.patch.object(discovery, 'build',
-                           return_value=mock_discovery_build):
+    with mock.patch.object(
+        auth, 'get_project_name', return_value='test-project'
+    ), mock.patch.object(discovery, 'build', return_value=mock_discovery_build):
       auth.get_service_account()
 
     mock_service_accounts.create.assert_not_called()
 
     mock_projects.setIamPolicy.assert_called_once_with(
         resource='test-project',
         body={
             'policy': {
-                'bindings': [{
-                    'role':
-                        'roles/aiplatform.user',
-                    'members': [(f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }, {
-                    'role':
-                        'roles/storage.admin',
-                    'members': [(f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }]
+                'bindings': [
+                    {
+                        'role': 'roles/aiplatform.user',
+                        'members': [
+                            f'serviceAccount:{expected_account_name}'
+                            '@test-project.iam.gserviceaccount.com'
+                        ],
+                    },
+                    {
+                        'role': 'roles/storage.admin',
+                        'members': [
+                            f'serviceAccount:{expected_account_name}'
+                            '@test-project.iam.gserviceaccount.com'
+                        ],
+                    },
+                ]
             }
-        })
+        },
+    )
 
   @parameterized.parameters(_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS)
-  def test_get_service_account_some_permissions(self, sys_argv,
-                                                expected_account_name):
+  def test_get_service_account_some_permissions(
+      self, sys_argv, expected_account_name
+  ):
     """Tests if `get_service_account` creates permissions properly for an existing account with some permissions."""
 
     flags.FLAGS(sys_argv)
 
     mock_service_accounts = mock.Mock()
     mock_service_accounts.list.return_value.execute.return_value = {
         'accounts': [
             {
-                'email': (f'{expected_account_name}'
-                          '@test-project.iam.gserviceaccount.com')
+                'email': (
+                    f'{expected_account_name}'
+                    '@test-project.iam.gserviceaccount.com'
+                )
             },
             {
                 # Used to test that permissions of other users are not affected
                 'email': 'someone_else@test-project.iam.gserviceaccount.com'
-            }
+            },
         ]
     }
     mock_service_accounts.create.return_value.execute.return_value = None
 
     mock_projects = mock.Mock()
     mock_projects.serviceAccounts.return_value = mock_service_accounts
     mock_projects.getIamPolicy.return_value.execute.return_value = {
-        'bindings': [{
-            'role':
-                'roles/aiplatform.user',
-            'members': [(f'serviceAccount:{expected_account_name}'
-                         '@test-project.iam.gserviceaccount.com')]
-        }, {
-            'role': 'roles/storage.admin',
-            'members': ['someone-else@test-project.iam.gserviceaccount.com']
-        }]
+        'bindings': [
+            {
+                'role': 'roles/aiplatform.user',
+                'members': [
+                    f'serviceAccount:{expected_account_name}'
+                    '@test-project.iam.gserviceaccount.com'
+                ],
+            },
+            {
+                'role': 'roles/storage.admin',
+                'members': [
+                    'someone-else@test-project.iam.gserviceaccount.com'
+                ],
+            },
+        ]
     }
 
     mock_discovery_build = mock.Mock()
     mock_discovery_build.projects.return_value = mock_projects
 
-    with mock.patch.object(auth, 'get_project_name',
-                           return_value='test-project'), \
-         mock.patch.object(discovery, 'build',
-                           return_value=mock_discovery_build):
+    with mock.patch.object(
+        auth, 'get_project_name', return_value='test-project'
+    ), mock.patch.object(discovery, 'build', return_value=mock_discovery_build):
       auth.get_service_account()
 
     mock_service_accounts.create.assert_not_called()
 
     mock_projects.setIamPolicy.assert_called_once_with(
         resource='test-project',
         body={
             'policy': {
-                'bindings': [{
-                    'role':
-                        'roles/aiplatform.user',
-                    'members': [(f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }, {
-                    'role':
-                        'roles/storage.admin',
-                    'members': [('someone-else'
-                                 '@test-project.iam.gserviceaccount.com'),
-                                (f'serviceAccount:{expected_account_name}'
-                                 '@test-project.iam.gserviceaccount.com')]
-                }]
+                'bindings': [
+                    {
+                        'role': 'roles/aiplatform.user',
+                        'members': [
+                            f'serviceAccount:{expected_account_name}'
+                            '@test-project.iam.gserviceaccount.com'
+                        ],
+                    },
+                    {
+                        'role': 'roles/storage.admin',
+                        'members': [
+                            'someone-else@test-project.iam.gserviceaccount.com',
+                            (
+                                f'serviceAccount:{expected_account_name}'
+                                '@test-project.iam.gserviceaccount.com'
+                            ),
+                        ],
+                    },
+                ]
             }
-        })
+        },
+    )
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `xmanager-0.3.0/xmanager/cloud/build_image.py` & `xmanager-0.4.0/xmanager/cloud/build_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,45 @@
 from xmanager.cloud import auth
 from xmanager.cloud import cloud_build
 from xmanager.cloud import docker_lib
 from xmanager.docker import docker_adapter
 from xmanager.xm import utils
 
 _BUILD_IMAGE_LOCALLY = flags.DEFINE_boolean(
-    'xm_build_image_locally', True,
-    'Use local Docker to build images instead of remote Google Cloud Build. '
-    'This is usually a lot faster but requires docker to be installed.')
+    'xm_build_image_locally',
+    True,
+    (
+        'Use local Docker to build images instead of remote Google Cloud Build.'
+        ' This is usually a lot faster but requires docker to be installed.'
+    ),
+)
 _USE_DOCKER_COMMAND = flags.DEFINE_boolean(
-    'xm_use_docker_command', True,
-    'Call "docker build" in a subprocess rather than using Python docker '
-    'client library when building the docker image locally. This provies a '
-    'much nicer output for interactive use.')
+    'xm_use_docker_command',
+    True,
+    (
+        'Call "docker build" in a subprocess rather than using Python docker '
+        'client library when building the docker image locally. This provies a '
+        'much nicer output for interactive use.'
+    ),
+)
 _SHOW_DOCKER_COMMAND_PROGRESS = flags.DEFINE_boolean(
-    'xm_show_docker_command_progress', False,
-    'Show container output during the "docker build".')
+    'xm_show_docker_command_progress',
+    False,
+    'Show container output during the "docker build".',
+)
 _WRAP_LATE_BINDINGS = flags.DEFINE_boolean(
-    'xm_wrap_late_bindings', False,
-    'Feature flag to wrap and unwrap late bindings for network addresses. '
-    'ONLY works with PythonContainer with default instructions or simple '
-    'instructions that do not modify the file directory. '
-    'REQUIRES ./entrypoint.sh to be the ENTRYPOINT.')
+    'xm_wrap_late_bindings',
+    False,
+    (
+        'Feature flag to wrap and unwrap late bindings for network addresses. '
+        'ONLY works with PythonContainer with default instructions or simple '
+        'instructions that do not modify the file directory. '
+        'REQUIRES ./entrypoint.sh to be the ENTRYPOINT.'
+    ),
+)
 
 # TODO: Find a master image than is compatible with every
 # combination (TF, Torch, JAX) X (CPU, GPU, TPU).
 _DEFAULT_BASE_IMAGE = 'gcr.io/deeplearning-platform-release/base-cu110'
 _DOCKERFILE_TEMPLATE = """
 FROM {base_image}
 
@@ -77,21 +91,23 @@
   export XRT_TPU_CONFIG="tpu_worker;0;$TPU_IP_AND_PORT"
 fi
 
 {cmds}
 """
 
 
-def build(py_executable: xm.PythonContainer,
-          args: xm.SequentialArgs,
-          env_vars: Dict[str, str],
-          image_name: Optional[str] = None,
-          project: Optional[str] = None,
-          bucket: Optional[str] = None,
-          pull_image: bool = False) -> str:
+def build(
+    py_executable: xm.PythonContainer,
+    args: xm.SequentialArgs,
+    env_vars: Dict[str, str],
+    image_name: Optional[str] = None,
+    project: Optional[str] = None,
+    bucket: Optional[str] = None,
+    pull_image: bool = False,
+) -> str:
   """Build a Docker image from a Python project.
 
   Args:
     py_executable: The PythonContainer to build.
     args: Args to pass to the image.
     env_vars: Environment variables to set in the image.
     image_name: The image name that will be assigned to the resulting image.
@@ -112,26 +128,35 @@
   with tempfile.TemporaryDirectory() as wrapped_directory:
     if _WRAP_LATE_BINDINGS.value:
       _wrap_late_bindings(wrapped_directory, python_path, dockerfile)
       python_path = wrapped_directory
       dockerfile = os.path.join(python_path, 'Dockerfile')
 
     with tempfile.TemporaryDirectory() as staging:
-      docker_lib.prepare_directory(staging, python_path, dirname, entrypoint,
-                                   dockerfile)
-      return build_by_dockerfile(staging, os.path.join(staging, 'Dockerfile'),
-                                 image_name, project, bucket, pull_image)
+      docker_lib.prepare_directory(
+          staging, python_path, dirname, entrypoint, dockerfile
+      )
+      return build_by_dockerfile(
+          staging,
+          os.path.join(staging, 'Dockerfile'),
+          image_name,
+          project,
+          bucket,
+          pull_image,
+      )
 
 
-def build_by_dockerfile(path: str,
-                        dockerfile: str,
-                        image_name: str,
-                        project: Optional[str] = None,
-                        bucket: Optional[str] = None,
-                        pull_image: bool = False):
+def build_by_dockerfile(
+    path: str,
+    dockerfile: str,
+    image_name: str,
+    project: Optional[str] = None,
+    bucket: Optional[str] = None,
+    pull_image: bool = False,
+):
   """Build a Docker image from a Docker directory.
 
   Args:
     path: The directory to use for the Docker build context.
     dockerfile: The path of Dockerfile.
     image_name: The name to set the built image to.
     project: The project to use if CloudBuild is used.
@@ -146,15 +171,16 @@
     if docker_lib.is_docker_installed():
       # TODO: Improve out-of-disk space handling.
       return docker_lib.build_docker_image(
           image_name,
           path,
           dockerfile,
           use_docker_command=_USE_DOCKER_COMMAND.value,
-          show_docker_command_progress=_SHOW_DOCKER_COMMAND_PROGRESS.value)
+          show_docker_command_progress=_SHOW_DOCKER_COMMAND_PROGRESS.value,
+      )
     print('Falling back to CloudBuild. See INFO log for details.')
 
   # If Dockerfile is not a direct child of path, then create a temp directory
   # that contains both the contents of path and Dockerfile.
   with tempfile.TemporaryDirectory() as tempdir:
     if os.path.dirname(dockerfile) != path:
       new_path = os.path.join(tempdir, os.path.basename(path))
@@ -184,25 +210,27 @@
 
 def _get_base_image(py_executable: xm.PythonContainer) -> str:
   if py_executable.base_image:
     return py_executable.base_image
   return _DEFAULT_BASE_IMAGE
 
 
-def _create_instructions(py_executable: xm.PythonContainer,
-                         env_vars: Dict[str, str]) -> str:
+def _create_instructions(
+    py_executable: xm.PythonContainer, env_vars: Dict[str, str]
+) -> str:
   """Create Docker instructions."""
   set_env_vars = [f'ENV {key}="{value}"' for key, value in env_vars.items()]
   if py_executable.docker_instructions:
     return '\n'.join(py_executable.docker_instructions + set_env_vars)
 
   directory = os.path.basename(py_executable.path)
   return '\n'.join(
-      list(default_steps(directory, py_executable.use_deep_module)) +
-      set_env_vars)
+      list(default_steps(directory, py_executable.use_deep_module))
+      + set_env_vars
+  )
 
 
 def default_steps(directory: str, use_deep_module: bool) -> List[str]:
   """Default commands to use in the Dockerfile."""
   workdir_setup_prefix = []
   workdir_setup_suffix = []
   project_dir = f'/{directory}'
@@ -215,52 +243,54 @@
     ]
     project_dir = f'/workdir/{directory}'
   else:
     workdir_setup_suffix = [
         f'WORKDIR {directory}',
     ]
 
-  return workdir_setup_prefix + [
-      # Without setting LANG, RDL ran into an UnicodeDecodeError, similar to
-      # what is described at [1]. This seems to be good practice and not hurt so
-      # we're just always setting it.
-      # [1] https://github.com/spotDL/spotify-downloader/issues/279
-      'ENV LANG=C.UTF-8',
-      'RUN rm -f /etc/apt/sources.list.d/cuda.list',
-      'RUN curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | ' +
-      'apt-key add -',
-      # Updating and installing on the same line causes cache-busting.
-      # https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#run
-      'RUN apt-get update && apt-get install -y git netcat',
-      'RUN python -m pip install --upgrade pip',
-      f'COPY {directory}/requirements.txt {project_dir}/requirements.txt',
-      f'RUN python -m pip install -r {directory}/requirements.txt',
-      # It is best practice to copy the project directory as late as possible,
-      # rather than at the beginning. This allows Docker to reuse cached layers.
-      # If copying the project files were the first step, a tiny modification to
-      # the source code will invalidate the cache.
-      # https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#add-or-copy
-      f'COPY {directory}/ {project_dir}',
-      # Changing ownwership of project_dir, so that both users: UID 1000
-      # and root are the co-owner of it.
-      f'RUN chown -R 1000:root {project_dir} && chmod -R 775 {project_dir}',
-  ] + workdir_setup_suffix
+  return (
+      workdir_setup_prefix
+      + [
+          # Without setting LANG, RDL ran into an UnicodeDecodeError, similar to
+          # what is described at [1]. This seems to be good practice and not
+          # hurt so we're just always setting it.
+          # [1] https://github.com/spotDL/spotify-downloader/issues/279
+          'ENV LANG=C.UTF-8',
+          # Updating and installing on the same line causes cache-busting.
+          # https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#run
+          'RUN apt-get update && apt-get install -y git netcat',
+          'RUN python -m pip install --upgrade pip',
+          f'COPY {directory}/requirements.txt {project_dir}/requirements.txt',
+          f'RUN python -m pip install -r {directory}/requirements.txt',
+          # It is best practice to copy the project directory as late as
+          # possible, rather than at the beginning. This allows Docker to reuse
+          # cached layers. If copying the project files were the first step, a
+          # tiny modification to the source code will invalidate the cache.
+          # https://docs.docker.com/develop/develop-images/dockerfile_best-practices/#add-or-copy
+          f'COPY {directory}/ {project_dir}',
+          # Changing ownwership of project_dir, so that both users: UID 1000
+          # and root are the co-owner of it.
+          f'RUN chown -R 1000:root {project_dir} && chmod -R 775 {project_dir}',
+      ]
+      + workdir_setup_suffix
+  )
 
 
 def _create_dockerfile(
     py_executable: xm.PythonContainer,
     args: xm.SequentialArgs,
     env_vars: Dict[str, str],
 ) -> str:
   """Creates a Dockerfile from a project executable."""
   base_image = _get_base_image(py_executable)
   instructions = _create_instructions(py_executable, env_vars)
   entrypoint = _create_entrypoint_cmd(args)
   contents = _DOCKERFILE_TEMPLATE.format(
-      base_image=base_image, instructions=instructions, entrypoint=entrypoint)
+      base_image=base_image, instructions=instructions, entrypoint=entrypoint
+  )
   print('Dockerfile:', contents, sep='\n')
   t = tempfile.NamedTemporaryFile(delete=False)
   with open(t.name, 'w') as f:
     f.write(contents)
   return t.name
 
 
@@ -268,27 +298,29 @@
   """Given the executable, return entrypoint commands."""
   if isinstance(py_executable.entrypoint, xm.ModuleName):
     cmds = [f'python -m {py_executable.entrypoint.module_name}']
   elif isinstance(py_executable.entrypoint, xm.CommandList):
     # Commands specified by the user are passed unchanged.
     cmds = py_executable.entrypoint.commands
   else:
-    raise ValueError('Unsupported entrypoint type {}'.format(
-        type(py_executable.entrypoint)))
+    raise ValueError(
+        'Unsupported entrypoint type {}'.format(type(py_executable.entrypoint))
+    )
   cmds = '\n'.join(cmds)
   # Allow passing extra parameters to the commands.
   if not cmds.endswith(('$@', '"$@"')):
     cmds = cmds + ' "$@"'
   return cmds
 
 
 def _create_entrypoint(py_executable: xm.PythonContainer) -> str:
   """Create a bash entrypoint based on the base image."""
   contents = _ENTRYPOINT_TEMPLATE.format(
-      cmds=_get_entrypoint_commands(py_executable))
+      cmds=_get_entrypoint_commands(py_executable)
+  )
 
   t = tempfile.NamedTemporaryFile(delete=False)
   with open(t.name, 'w') as f:
     f.write(contents)
   return t.name
 
 
@@ -321,27 +353,32 @@
   shutil.rmtree(destination)
   shutil.copytree(path, destination)
 
   root_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
 
   shutil.copyfile(
       os.path.join(root_dir, 'cloud', 'data', 'wrapped_entrypoint.sh'),
-      os.path.join(destination, 'wrapped_entrypoint.sh'))
+      os.path.join(destination, 'wrapped_entrypoint.sh'),
+  )
   shutil.copyfile(
       os.path.join(root_dir, 'cloud', 'utils.py'),
-      os.path.join(destination, 'vertex_utils.py'))
+      os.path.join(destination, 'vertex_utils.py'),
+  )
   shutil.copyfile(
       os.path.join(root_dir, 'vizier', 'vizier_cloud', 'vizier_worker.py'),
-      os.path.join(destination, 'vizier_worker.py'))
+      os.path.join(destination, 'vizier_worker.py'),
+  )
 
   new_dockerfile = os.path.join(destination, 'Dockerfile')
   insert_instructions = [
       'RUN chmod +x ./wrapped_entrypoint.sh',
   ]
   with open(dockerfile) as f:
     contents = f.read()
-  contents = contents.replace('ENTRYPOINT',
-                              '\n'.join(insert_instructions + ['ENTRYPOINT']))
-  contents = contents.replace('ENTRYPOINT ["./entrypoint.sh',
-                              'ENTRYPOINT ["./wrapped_entrypoint.sh')
+  contents = contents.replace(
+      'ENTRYPOINT', '\n'.join(insert_instructions + ['ENTRYPOINT'])
+  )
+  contents = contents.replace(
+      'ENTRYPOINT ["./entrypoint.sh', 'ENTRYPOINT ["./wrapped_entrypoint.sh'
+  )
   with open(new_dockerfile, 'w') as f:
     f.write(contents)
```

### Comparing `xmanager-0.3.0/xmanager/cloud/build_image_test.py` & `xmanager-0.4.0/xmanager/cloud/build_image_test.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/cloud/cloud_build.py` & `xmanager-0.4.0/xmanager/cloud/cloud_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,52 +25,64 @@
 from google.cloud import storage
 from googleapiclient import discovery
 import termcolor
 
 from xmanager.cloud import auth
 
 _CLOUD_BUILD_TIMEOUT_SECONDS = flags.DEFINE_integer(
-    'xm_cloud_build_timeout_seconds', 1200,
-    'The amount of time that builds should be allowed to run, '
-    'to second granularity.')
+    'xm_cloud_build_timeout_seconds',
+    1200,
+    (
+        'The amount of time that builds should be allowed to run, '
+        'to second granularity.'
+    ),
+)
 _USE_CLOUD_BUILD_CACHE = flags.DEFINE_boolean(
     'xm_use_cloud_build_cache',
     False,
-    'Use Cloud Build cache to speed up the Docker build. '
-    'An image with the same name tagged as :latest should exist.'
-    'More details at https://cloud.google.com/cloud-build/docs/speeding-up-builds#using_a_cached_docker_image'  # pylint:disable=g-line-too-long
+    (  # pylint:disable=g-line-too-long
+        'Use Cloud Build cache to speed up the Docker build. '
+        'An image with the same name tagged as :latest should exist.'
+        'More details at'
+        ' https://cloud.google.com/cloud-build/docs/speeding-up-builds#using_a_cached_docker_image'
+    ),
 )
 
 _USE_KANIKO = flags.DEFINE_boolean(
-    'xm_use_kaniko', False,
-    'Use kaniko backend for Cloud Build and enable caching.')
-_KANIKO_CACHE_TTL = flags.DEFINE_string('xm_kaniko_cache_ttl', '336h',
-                                        'Cache ttl to use for kaniko builds.')
+    'xm_use_kaniko',
+    False,
+    'Use kaniko backend for Cloud Build and enable caching.',
+)
+_KANIKO_CACHE_TTL = flags.DEFINE_string(
+    'xm_kaniko_cache_ttl', '336h', 'Cache ttl to use for kaniko builds.'
+)
 
 _CLOUD_SDK_CREDENTIALS_WARNING = """\
 Your application has authenticated using end user credentials from Google \
 Cloud SDK without a quota project. You might receive a "quota exceeded" \
 or "API not enabled" error. We recommend you rerun \
 `gcloud auth application-default login` and make sure a quota project is \
 added. Or you can use service accounts instead. For more information \
 about service accounts, see https://cloud.google.com/docs/authentication/"""
 warnings.filterwarnings('ignore', _CLOUD_SDK_CREDENTIALS_WARNING)
 
 
 class Client:
   """Cloud Build Client."""
 
-  def __init__(self,
-               project: Optional[str] = None,
-               bucket: Optional[str] = None,
-               credentials=None,
-               cloud_build_timeout_seconds: Optional[int] = None,
-               use_cloud_build_cache: Optional[bool] = None,
-               use_kaniko: Optional[bool] = None,
-               kaniko_cache_ttl: Optional[str] = None):
+  def __init__(
+      self,
+      project: Optional[str] = None,
+      bucket: Optional[str] = None,
+      credentials=None,
+      cloud_build_timeout_seconds: Optional[int] = None,
+      use_cloud_build_cache: Optional[bool] = None,
+      use_kaniko: Optional[bool] = None,
+      kaniko_cache_ttl: Optional[str] = None,
+  ):
     """Create the Cloud Build Client.
 
     Args:
       project: Name of the GCP project to use for Cloud Build calls and for
         storing the data passed to Cloud Build. If not specified the project of
         the default credentials for the current environment is used.
       bucket: Bucket used to store data passed to Cloud Build. If not specified
@@ -103,21 +115,23 @@
     if kaniko_cache_ttl is None:
       kaniko_cache_ttl = _KANIKO_CACHE_TTL.value
     self.kaniko_cache_ttl = kaniko_cache_ttl
     self.cloudbuild_api = None  # discovery CloudBuild v1 client
 
   def upload_tar_to_storage(self, archive_path: str, destination_name: str):
     storage_client = storage.Client(
-        project=self.project, credentials=self.credentials)
+        project=self.project, credentials=self.credentials
+    )
     bucket = storage_client.bucket(self.bucket)
     blob = bucket.blob(destination_name)
     blob.upload_from_filename(archive_path)
 
-  def build_docker_image(self, image: str, directory: str,
-                         upload_name: str) -> str:
+  def build_docker_image(
+      self, image: str, directory: str, upload_name: str
+  ) -> str:
     """Create a Docker image via Cloud Build and push to Cloud Repository."""
     repository, tag = docker_utils.parse_repository_tag(image)
     if not tag:
       tag = datetime.datetime.now().strftime('%Y%m%d-%H%M%S_%f')
 
     _, archive_path = tempfile.mkstemp(suffix='.tar.gz')
     with tarfile.open(archive_path, 'w:gz') as tar:
@@ -128,17 +142,22 @@
     # Note: On GCP cache_discovery=True (the default) leads to ugly error
     # messages as file_cache is unavailable.
     if not self.cloudbuild_api:
       self.cloudbuild_api = discovery.build(
           'cloudbuild',
           'v1',
           credentials=self.credentials,
-          cache_discovery=False)
-    create_op = self.cloudbuild_api.projects().builds().create(
-        projectId=self.project, body=build_body).execute()
+          cache_discovery=False,
+      )
+    create_op = (
+        self.cloudbuild_api.projects()
+        .builds()
+        .create(projectId=self.project, body=build_body)
+        .execute()
+    )
     log_url = create_op['metadata']['build']['logUrl']
     print('Cloud Build link:', termcolor.colored(log_url, color='blue'))
 
     build_id = create_op['metadata']['build']['id']
     return self.wait_for_build(build_id, f'{repository}:{tag}')
 
   def _build_request_body(self, bucket_path, repository, tag) -> Dict[str, Any]:
@@ -149,72 +168,91 @@
                 'bucket': self.bucket,
                 'object': bucket_path,
             },
         },
         'timeout': str(self.cloud_build_timeout_seconds) + 's',
     }
     if self.use_kaniko:
-      body.update({
-          'steps': [{
-              'name':
-                  'gcr.io/kaniko-project/executor:latest',
-              'args': [
-                  f'--destination={repository}:{tag}',
-                  f'--destination={repository}:latest', '--cache=true',
-                  f'--cache-ttl={self.kaniko_cache_ttl}'
-              ],
-          }]
-      })
+      body.update(
+          {
+              'steps': [{
+                  'name': 'gcr.io/kaniko-project/executor:latest',
+                  'args': [
+                      f'--destination={repository}:{tag}',
+                      f'--destination={repository}:latest',
+                      '--cache=true',
+                      f'--cache-ttl={self.kaniko_cache_ttl}',
+                  ],
+              }]
+          }
+      )
     else:
-      args_for_cached_image = (['--cache-from', f'{repository}:latest']
-                               if self.use_cloud_build_cache else [])
+      args_for_cached_image = (
+          ['--cache-from', f'{repository}:latest']
+          if self.use_cloud_build_cache
+          else []
+      )
       body.update({
           'steps': [{
-              'name':
-                  'gcr.io/cloud-builders/docker',
-              'args': [
-                  'build', '-t', f'{repository}:{tag}', '-t',
-                  f'{repository}:latest'
-              ] + args_for_cached_image + ['.'],
+              'name': 'gcr.io/cloud-builders/docker',
+              'args': (
+                  [
+                      'build',
+                      '-t',
+                      f'{repository}:{tag}',
+                      '-t',
+                      f'{repository}:latest',
+                  ]
+                  + args_for_cached_image
+                  + ['.']
+              ),
           }],
-          'options': {
-              'machineType': 'E2_HIGHCPU_32'
-          },
-          'images': [repository]
+          'options': {'machineType': 'E2_HIGHCPU_32'},
+          'images': [repository],
       })
     return body
 
   def wait_for_build(self, build_id: str, kaniko_image: str) -> str:
     """Waits for build to finish and return the image URI of the result."""
     backoff = 30  # seconds
     while True:
       time.sleep(backoff)
-      result = self.cloudbuild_api.projects().builds().get(
-          projectId=self.project, id=build_id).execute()
+      result = (
+          self.cloudbuild_api.projects()
+          .builds()
+          .get(projectId=self.project, id=build_id)
+          .execute()
+      )
       status = result['status']
       print('Cloud Build status:', status)
 
       if status == 'SUCCESS':
         image_uri = kaniko_image
         if not self.use_kaniko:
           # Note: Not sure if this is needed. Could we always use the uri above?
           image = result['results']['images'][0]
           image_uri = f'{image["name"]}@{image["digest"]}'
         break
       elif status == 'FAILURE':
-        print('Build FAILED. See logs for more information:',
-              termcolor.colored(result['logUrl'], color='red'))
+        print(
+            'Build FAILED. See logs for more information:',
+            termcolor.colored(result['logUrl'], color='red'),
+        )
         raise RuntimeError('Build FAILED.')
       elif status == 'QUEUED' or status == 'WORKING':
         continue
       elif status == 'INTERNAL_ERROR' or status == 'CANCELLED':
         print('Cloud Build tool failure. Status:', status)
         raise RuntimeError('Cloud Build tool failed. Try again.')
       else:
-        print('Build not complete. See logs for more information:',
-              termcolor.colored(result['logUrl'], color='red'))
+        print(
+            'Build not complete. See logs for more information:',
+            termcolor.colored(result['logUrl'], color='red'),
+        )
         raise RuntimeError('Build FAILED.')
 
     print('Your image URI is:', termcolor.colored(image_uri, color='blue'))
-    print('You can run your image locally via:\n' +
-          termcolor.colored('docker run ' + image_uri, color='green'))
+    print(
+        'You can run your image locally via:\n'
+        + termcolor.colored('docker run ' + image_uri, color='green')
+    )
     return image_uri
```

### Comparing `xmanager-0.3.0/xmanager/cloud/cloud_build_test.py` & `xmanager-0.4.0/xmanager/cloud/cloud_build_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,47 +22,55 @@
 
   def test_build_request_body(self):
     client = cloud_build.Client(
         'my-project',
         'my-bucket',
         mock.Mock(),
         use_kaniko=False,
-        use_cloud_build_cache=False)
+        use_cloud_build_cache=False,
+    )
     image = client._build_request_body('path/to/project', 'my-image', 'live')
     self.assertEqual(
-        image, {
+        image,
+        {
             'images': ['my-image'],
-            'options': {
-                'machineType': 'E2_HIGHCPU_32'
-            },
+            'options': {'machineType': 'E2_HIGHCPU_32'},
             'source': {
                 'storageSource': {
                     'bucket': 'my-bucket',
                     'object': 'path/to/project',
                 },
             },
             'steps': [{
                 'args': [
-                    'build', '-t', 'my-image:live', '-t', 'my-image:latest', '.'
+                    'build',
+                    '-t',
+                    'my-image:live',
+                    '-t',
+                    'my-image:latest',
+                    '.',
                 ],
                 'name': 'gcr.io/cloud-builders/docker',
             }],
-            'timeout': '1200s'
-        })
+            'timeout': '1200s',
+        },
+    )
 
   def test_build_request_body_use_kaniko(self):
     client = cloud_build.Client(
         'my-project',
         'my-bucket',
         mock.Mock(),
         use_kaniko=True,
-        use_cloud_build_cache=False)
+        use_cloud_build_cache=False,
+    )
     image = client._build_request_body('path/to/project', 'my-image', 'live')
     self.assertEqual(
-        image, {
+        image,
+        {
             'source': {
                 'storageSource': {
                     'bucket': 'my-bucket',
                     'object': 'path/to/project',
                 },
             },
             'steps': [{
@@ -70,31 +78,32 @@
                     '--destination=my-image:live',
                     '--destination=my-image:latest',
                     '--cache=true',
                     '--cache-ttl=336h',
                 ],
                 'name': 'gcr.io/kaniko-project/executor:latest',
             }],
-            'timeout': '1200s'
-        })
+            'timeout': '1200s',
+        },
+    )
 
   def test_build_request_body_use_build_cache(self):
     client = cloud_build.Client(
         'my-project',
         'my-bucket',
         mock.Mock(),
         use_kaniko=False,
-        use_cloud_build_cache=True)
+        use_cloud_build_cache=True,
+    )
     image = client._build_request_body('path/to/project', 'my-image', 'live')
     self.assertEqual(
-        image, {
+        image,
+        {
             'images': ['my-image'],
-            'options': {
-                'machineType': 'E2_HIGHCPU_32'
-            },
+            'options': {'machineType': 'E2_HIGHCPU_32'},
             'source': {
                 'storageSource': {
                     'bucket': 'my-bucket',
                     'object': 'path/to/project',
                 },
             },
             'steps': [{
@@ -106,13 +115,14 @@
                     'my-image:latest',
                     '--cache-from',
                     'my-image:latest',
                     '.',
                 ],
                 'name': 'gcr.io/cloud-builders/docker',
             }],
-            'timeout': '1200s'
-        })
+            'timeout': '1200s',
+        },
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/cloud/data/wrapped_entrypoint.sh` & `xmanager-0.4.0/xmanager/cloud/data/wrapped_entrypoint.sh`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/cloud/docker_lib.py` & `xmanager-0.4.0/xmanager/cloud/docker_lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,17 +27,21 @@
 import termcolor
 
 
 def create_tag() -> str:
   return datetime.datetime.now().strftime('%Y%m%d-%H%M%S-%f')
 
 
-def prepare_directory(destination_directory: str, source_directory: str,
-                      project_name: str, entrypoint_file: str,
-                      dockerfile: str) -> None:
+def prepare_directory(
+    destination_directory: str,
+    source_directory: str,
+    project_name: str,
+    entrypoint_file: str,
+    dockerfile: str,
+) -> None:
   """Stage all inputs into the destination directory.
 
   Args:
     destination_directory: The directory to copy files to.
     source_directory: The directory to copy files from.
     project_name: The name of the folder inside destination_directory/ that
       source_directory/ files will be copied to.
@@ -46,22 +50,28 @@
   """
   source_path = pathlib.Path(source_directory)
   size = sum(f.stat().st_size for f in source_path.glob('**/*') if f.is_file())
   print(f'Size of Docker input: {humanize.naturalsize(size)}')
   if size > 200 * 10**6:
     print(
         termcolor.colored(
-            'You are trying to pack over 200MB into a Docker image. '
-            'Large images negatively impact build times',
-            color='magenta'))
-  shutil.copytree(source_directory,
-                  os.path.join(destination_directory, project_name))
+            (
+                'You are trying to pack over 200MB into a Docker image. '
+                'Large images negatively impact build times'
+            ),
+            color='magenta',
+        )
+    )
+  shutil.copytree(
+      source_directory, os.path.join(destination_directory, project_name)
+  )
   shutil.copyfile(dockerfile, os.path.join(destination_directory, 'Dockerfile'))
-  shutil.copyfile(entrypoint_file,
-                  os.path.join(destination_directory, 'entrypoint.sh'))
+  shutil.copyfile(
+      entrypoint_file, os.path.join(destination_directory, 'entrypoint.sh')
+  )
 
 
 def is_docker_installed() -> bool:
   """Checks if Docker is installed and accessible."""
   try:
     docker_client = docker.from_env()
     logging.info('Local docker: %s', docker_client.version())
@@ -71,32 +81,41 @@
       # This is the expected case when Docker is not installed, so we don't log
       # anything, and just return False. The other error branches indicate
       # something wrong with the Docker installation, so we log an error and
       # also return False.
       return False
     logging.info(e)
     if 'Permission denied' in str(e):
-      print('Looks like there is a permission problem with docker. '
-            'Did you install sudoless docker?')
+      print(
+          'Looks like there is a permission problem with docker. '
+          'Did you install sudoless docker?'
+      )
   return False
 
 
-def build_docker_image(image: str,
-                       directory: str,
-                       dockerfile: Optional[str] = None,
-                       use_docker_command: bool = True,
-                       show_docker_command_progress: bool = False) -> str:
+def build_docker_image(
+    image: str,
+    directory: str,
+    dockerfile: Optional[str] = None,
+    use_docker_command: bool = True,
+    show_docker_command_progress: bool = False,
+) -> str:
   """Builds a Docker image locally."""
   logging.info('Building Docker image')
   docker_client = docker.from_env()
   if not dockerfile:
     dockerfile = os.path.join(directory, 'Dockerfile')
   if use_docker_command:
-    _build_image_with_docker_command(docker_client, directory, image,
-                                     dockerfile, show_docker_command_progress)
+    _build_image_with_docker_command(
+        docker_client,
+        directory,
+        image,
+        dockerfile,
+        show_docker_command_progress,
+    )
   else:
     _build_image_with_python_client(docker_client, directory, image, dockerfile)
   logging.info('Building docker image: Done')
   return image
 
 
 def push_docker_image(image: str) -> str:
@@ -105,63 +124,76 @@
   repository, tag = docker_utils.parse_repository_tag(image)
   push = docker_client.images.push(repository=repository, tag=tag)
   logging.info(push)
   if not isinstance(push, str) or '"Digest":' not in push:
     raise RuntimeError(
         'Expected docker push to return a string with `status: Pushed` and a '
         'Digest. This is probably a temporary issue with '
-        '--xm_build_image_locally and you should try again')
+        '--xm_build_image_locally and you should try again'
+    )
   # If we are pushing an image, then :latest should also be present.
   docker_client.images.push(repository=repository, tag='latest')
   print('Your image URI is:', termcolor.colored(image, color='blue'))
   return image
 
 
-def _build_image_with_docker_command(client: docker.DockerClient,
-                                     path: str,
-                                     image_tag: str,
-                                     dockerfile: str,
-                                     progress: bool = False) -> None:
+def _build_image_with_docker_command(
+    client: docker.DockerClient,
+    path: str,
+    image_tag: str,
+    dockerfile: str,
+    progress: bool = False,
+) -> None:
   """Builds a Docker image by calling `docker build` within a subprocess."""
   version = client.version()['Version']
   [major, minor] = version.split('.')[:2]
   if float(f'{major}.{minor}') < 20.10:
     # docker buildx requires docker 20.10.
     raise RuntimeError('XCloud requires Docker Engine version 20.10+.')
   repository, tag = docker_utils.parse_repository_tag(image_tag)
   if not tag:
     tag = 'latest'
   command = [
-      'docker', 'buildx', 'build', '-t', f'{repository}:{tag}', '-t',
-      f'{repository}:latest', '-f', dockerfile, path
+      'docker',
+      'buildx',
+      'build',
+      '-t',
+      f'{repository}:{tag}',
+      '-t',
+      f'{repository}:latest',
+      '-f',
+      dockerfile,
+      path,
   ]
 
   # Adding flags to show progress and disabling cache.
   # Caching prevents actual commands in layer from executing.
   # This is turn makes displaying progress redundant.
   if progress:
     command[2:2] = ['--progress', 'plain', '--no-cache']
 
   subprocess.run(
-      command, check=True, env={
-          **os.environ, 'DOCKER_BUILDKIT': '1'
-      })
+      command, check=True, env={**os.environ, 'DOCKER_BUILDKIT': '1'}
+  )
 
 
-def _build_image_with_python_client(client: docker.DockerClient, path: str,
-                                    image_tag: str, dockerfile: str) -> None:
+def _build_image_with_python_client(
+    client: docker.DockerClient, path: str, image_tag: str, dockerfile: str
+) -> None:
   """Builds a Docker image by calling the Docker Python client."""
   repository, tag = docker_utils.parse_repository_tag(image_tag)
   if not tag:
     tag = 'latest'
   try:
     # The `tag=` arg refers to the full repository:tag image name.
     _, logs = client.images.build(
-        path=path, tag=f'{repository}:{tag}', dockerfile=dockerfile)
+        path=path, tag=f'{repository}:{tag}', dockerfile=dockerfile
+    )
     client.images.build(
-        path=path, tag=f'{repository}:latest', dockerfile=dockerfile)
+        path=path, tag=f'{repository}:latest', dockerfile=dockerfile
+    )
   except docker.errors.BuildError as error:
     for log in error.build_log:
       print(log.get('stream', ''), end='', file=sys.stderr)
     raise error
   for log in logs:
     print(log.get('stream', ''), end='')
```

### Comparing `xmanager-0.3.0/xmanager/cloud/kubernetes.py` & `xmanager-0.4.0/xmanager/cloud/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,21 @@
 from xmanager.xm_local import executables as local_executables
 from xmanager.xm_local import execution as local_execution
 from xmanager.xm_local import executors as local_executors
 from xmanager.xm_local import status as local_status
 
 
 _K8S_SERVICE_ACCOUNT_NAME = flags.DEFINE_string(
-    'xm_k8s_service_account_name', 'default',
-    'Specifies the Kubernetes Service Account name to be used by XManager in'
-    'the pod specifications.')
+    'xm_k8s_service_account_name',
+    'default',
+    (
+        'Specifies the Kubernetes Service Account name to be used by XManager'
+        ' inthe pod specifications.'
+    ),
+)
 
 
 @functools.lru_cache()
 def client():
   # Global singleton defers client creation until an actual launch.
   # If the user only launches local jobs, they don't need to create a client.
   return Client()
@@ -89,29 +93,35 @@
   ) -> List[k8s_client.V1Job]:
     """Launches jobs on Kubernetes."""
     batch_jobs = []
     service = 'experiments'
     for job in jobs:
       executable = job.executable
       executor = job.executor
-      if not isinstance(executable,
-                        local_executables.GoogleContainerRegistryImage):
-        raise ValueError('Executable {} has type {}. Executable must be of '
-                         'type GoogleContainerRegistryImage.'.format(
-                             executable, type(executable)))
+      if not isinstance(
+          executable, local_executables.GoogleContainerRegistryImage
+      ):
+        raise ValueError(
+            'Executable {} has type {}. Executable must be of '
+            'type GoogleContainerRegistryImage.'.format(
+                executable, type(executable)
+            )
+        )
       all_env_vars = {**executable.env_vars, **job.env_vars}
       env = [k8s_client.V1EnvVar(k, v) for k, v in all_env_vars.items()]
       job_name = convert_to_valid_label(get_full_job_name(job.name))
       container = k8s_client.V1Container(
           name=job_name,
           image=executable.image_path,
           resources=requirements_from_executor(executor),
-          args=xm.merge_args(executable.args,
-                             job.args).to_list(utils.ARG_ESCAPER),
-          env=env)
+          args=xm.merge_args(executable.args, job.args).to_list(
+              utils.ARG_ESCAPER
+          ),
+          env=env,
+      )
       k8s_job = k8s_client.V1Job()
       k8s_job.metadata = k8s_client.V1ObjectMeta(name=job_name)
       k8s_job.spec = k8s_client.V1JobSpec(
           template=k8s_client.V1PodTemplateSpec(
               metadata=k8s_client.V1ObjectMeta(
                   labels={'service': service},
                   annotations=annotations_from_executor(executor),
@@ -154,15 +164,16 @@
 
   async def wait_for_job(self, job: k8s_client.V1Job) -> None:
     batch_api = k8s_client.BatchV1Api(self.api_client)
     backoff = 5  # seconds
     while True:
       await asyncio.sleep(backoff)
       response = batch_api.read_namespaced_job_status(
-          namespace='default', name=job.metadata.name)
+          namespace='default', name=job.metadata.name
+      )
       if response.status.completion_time:
         return
 
 
 @attr.s(auto_attribs=True)
 class KubernetesHandle(local_execution.ExecutionHandle):
   """A handle for referring to the launched container."""
@@ -173,31 +184,34 @@
     await asyncio.gather(*[client().wait_for_job(job) for job in self.jobs])
 
   def get_status(self) -> local_status.LocalWorkUnitStatus:
     raise NotImplementedError
 
 
 # Must act on all jobs with `local_executors.Kubernetes` executor.
-def launch(get_full_job_name: Callable[[str], str],
-           job_group: xm.JobGroup) -> List[KubernetesHandle]:
+def launch(
+    get_full_job_name: Callable[[str], str], job_group: xm.JobGroup
+) -> List[KubernetesHandle]:
   """Launch K8s jobs in the job_group and return a handler."""
-  jobs = xm.job_operators.collect_jobs_by_filter(job_group,
-                                                 _kubernetes_job_predicate)
+  jobs = xm.job_operators.collect_jobs_by_filter(
+      job_group, _kubernetes_job_predicate
+  )
   # As client creation may throw, do not initiate it if there are no jobs.
   if not jobs:
     return []
   k8_jobs = client().launch(
       get_full_job_name=get_full_job_name,
       jobs=jobs,
   )
   return [KubernetesHandle(jobs=k8_jobs)]
 
 
 def requirements_from_executor(
-    executor: local_executors.Kubernetes) -> k8s_client.V1ResourceRequirements:
+    executor: local_executors.Kubernetes,
+) -> k8s_client.V1ResourceRequirements:
   """Get resource limits from the executor."""
   limits = {}
   for resource, value in executor.requirements.task_requirements.items():
     if resource in xm.GpuType:
       # TODO: Implement detection of whether an accelerator is an Nvidia
       # GPU. amd.com/gpu is another type of GPU that is not present in GCP.
       limits['nvidia.com/gpu'] = f'{value:g}'
@@ -209,33 +223,42 @@
       # https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/#meaning-of-memory
       limits[str(resource).lower()] = f'{value:.15g}'
 
   return k8s_client.V1ResourceRequirements(limits=limits)
 
 
 def annotations_from_executor(
-    executor: local_executors.Kubernetes) -> Dict[str, str]:
+    executor: local_executors.Kubernetes,
+) -> Dict[str, str]:
   """Get Pod annotations from the executor for TPUs."""
-  if executor.cloud_provider != local_executors.GOOGLE_KUBERNETES_ENGINE_CLOUD_PROVIDER:
+  if (
+      executor.cloud_provider
+      != local_executors.GOOGLE_KUBERNETES_ENGINE_CLOUD_PROVIDER
+  ):
     return {}
 
   if executor.requirements.accelerator in xm.TpuType:
     tpu_runtime_version = 'nightly'
     if executor.tpu_capability:
       tpu_runtime_version = executor.tpu_capability.tpu_runtime_version
     return {'tf-version.cloud-tpus.google.com': tpu_runtime_version}
   return {}
 
 
 def node_selector_from_executor(
-    executor: local_executors.Kubernetes) -> Dict[str, str]:
+    executor: local_executors.Kubernetes,
+) -> Dict[str, str]:
   """Get Pod annotations from the executor for TPUs."""
-  if executor.cloud_provider != local_executors.GOOGLE_KUBERNETES_ENGINE_CLOUD_PROVIDER:
+  if (
+      executor.cloud_provider
+      != local_executors.GOOGLE_KUBERNETES_ENGINE_CLOUD_PROVIDER
+  ):
     return {}
 
   for resource in executor.requirements.task_requirements:
     if resource in xm.GpuType:
       return {
-          'cloud.google.com/gke-accelerator':
+          'cloud.google.com/gke-accelerator': (
               'nvidia-tesla-' + str(resource).lower()
+          )
       }
   return {}
```

### Comparing `xmanager-0.3.0/xmanager/cloud/kubernetes_test.py` & `xmanager-0.4.0/xmanager/cloud/kubernetes_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 from xmanager.cloud import kubernetes
 from xmanager.xm_local import executables as local_executables
 from xmanager.xm_local import executors as local_executors
 
 _TEST_SERVICE_ACCOUNT_NAME = 'test-service-account'
 _DEFAULT_SERVICE_ACCOUNT_NAME = 'default'
 
-_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS = [{
-    'sys_argv': sys.argv,
-    'expected_account_name': _DEFAULT_SERVICE_ACCOUNT_NAME
-}, {
-    'sys_argv': [
-        *sys.argv, f'--xm_k8s_service_account_name={_TEST_SERVICE_ACCOUNT_NAME}'
-    ],
-    'expected_account_name': _TEST_SERVICE_ACCOUNT_NAME
-}]
+_SERVICE_ACCOUNT_FLAG_TEST_PARAMETERS = [
+    {
+        'sys_argv': sys.argv,
+        'expected_account_name': _DEFAULT_SERVICE_ACCOUNT_NAME,
+    },
+    {
+        'sys_argv': [
+            *sys.argv,
+            f'--xm_k8s_service_account_name={_TEST_SERVICE_ACCOUNT_NAME}',
+        ],
+        'expected_account_name': _TEST_SERVICE_ACCOUNT_NAME,
+    },
+]
 
 
 class CallAPIResponse:
   items = []
 
 
 class KubernetesTest(parameterized.TestCase):
@@ -57,19 +61,17 @@
         name='test-job',
         executable=local_executables.GoogleContainerRegistryImage(
             name='test-image',
             image_path='image-path',
             args=xm.SequentialArgs.from_collection({'a': 1}),
         ),
         executor=local_executors.Kubernetes(
-            xm.JobRequirements(cpu=1, ram=1, t4=2)),
-        args={
-            'b': 2,
-            'c': 3
-        },
+            xm.JobRequirements(cpu=1, ram=1, t4=2)
+        ),
+        args={'b': 2, 'c': 3},
     )
     expected_service = k8s_client.V1Service(
         metadata=k8s_client.V1ObjectMeta(name='experiments'),
         spec=k8s_client.V1ServiceSpec(
             selector={'service': 'experiments'},
             cluster_ip='None',
         ),
@@ -92,15 +94,16 @@
                             name='test-job',
                             image='image-path',
                             resources=k8s_client.V1ResourceRequirements(
                                 limits={
                                     'cpu': '1',
                                     'memory': '1',
                                     'nvidia.com/gpu': '2',
-                                },),
+                                },
+                            ),
                             args=['--a=1', '--b=2', '--c=3'],
                             env=[],
                         )
                     ],
                     node_selector={
                         'cloud.google.com/gke-accelerator': 'nvidia-tesla-t4',
                     },
@@ -114,66 +117,79 @@
     [_, service_call, job_call] = fake_client.call_api.call_args_list
     _, service_kwargs = service_call
     self.assertEqual(service_kwargs['body'], expected_service)
     _, job_kwargs = job_call
     self.assertEqual(job_kwargs['body'], expected_job)
 
   @parameterized.product(
-      inside_cluster=[True, False],)
+      inside_cluster=[True, False],
+  )
   def test_config_load(self, inside_cluster):
     load_incluster_side_effect = (
-        k8s_config.ConfigException() if not inside_cluster else None)
-    with mock.patch.object(k8s_client, 'ApiClient', return_value=None), \
-         mock.patch.object(k8s_config, 'load_incluster_config',
-                           side_effect=load_incluster_side_effect,
-                           return_value=None) as mock_load_incluster, \
-         mock.patch.object(k8s_config, 'load_kube_config',
-                           return_value=None) as mock_load_kube:
+        k8s_config.ConfigException() if not inside_cluster else None
+    )
+    with mock.patch.object(
+        k8s_client, 'ApiClient', return_value=None
+    ), mock.patch.object(
+        k8s_config,
+        'load_incluster_config',
+        side_effect=load_incluster_side_effect,
+        return_value=None,
+    ) as mock_load_incluster, mock.patch.object(
+        k8s_config, 'load_kube_config', return_value=None
+    ) as mock_load_kube:
       kubernetes.Client(None)
 
     if inside_cluster:
       mock_load_incluster.assert_called_once_with()
     else:
       mock_load_kube.assert_called_once_with()
 
   def test_requirements_from_executor(self):
     executor = local_executors.Kubernetes(
-        requirements=xm.JobRequirements(cpu=1, ram=1 * xm.GiB))
+        requirements=xm.JobRequirements(cpu=1, ram=1 * xm.GiB)
+    )
     requirements = kubernetes.requirements_from_executor(executor).to_dict()
-    self.assertDictEqual(requirements['limits'], {
-        'cpu': '1',
-        'memory': str(2**30),
-    })
+    self.assertDictEqual(
+        requirements['limits'],
+        {
+            'cpu': '1',
+            'memory': str(2**30),
+        },
+    )
 
   def test_requirements_from_executor_gpu(self):
     executor = local_executors.Kubernetes(
-        requirements=xm.JobRequirements(v100=4))
+        requirements=xm.JobRequirements(v100=4)
+    )
     requirements = kubernetes.requirements_from_executor(executor).to_dict()
     self.assertDictEqual(requirements['limits'], {'nvidia.com/gpu': '4'})
 
   def test_requirements_from_executor_empty(self):
     executor = local_executors.Kubernetes()
     requirements = kubernetes.requirements_from_executor(executor).to_dict()
     self.assertDictEqual(requirements['limits'], {})
 
   def test_annotations_from_executor_tpu(self):
     executor = local_executors.Kubernetes(xm.JobRequirements(tpu_v2=8))
     self.assertDictEqual(
         kubernetes.annotations_from_executor(executor),
-        {'tf-version.cloud-tpus.google.com': 'nightly'})
+        {'tf-version.cloud-tpus.google.com': 'nightly'},
+    )
 
   def test_annotations_from_executor_gpu(self):
     executor = local_executors.Kubernetes(xm.JobRequirements(v100=4))
     self.assertDictEqual(kubernetes.annotations_from_executor(executor), {})
 
   def test_node_selector_from_executor_gpu(self):
     executor = local_executors.Kubernetes(xm.JobRequirements(v100=4))
     self.assertDictEqual(
         kubernetes.node_selector_from_executor(executor),
-        {'cloud.google.com/gke-accelerator': 'nvidia-tesla-v100'})
+        {'cloud.google.com/gke-accelerator': 'nvidia-tesla-v100'},
+    )
 
   def test_node_selector_from_executor_tpu(self):
     executor = local_executors.Kubernetes(xm.JobRequirements(tpu_v2=8))
     self.assertDictEqual(kubernetes.node_selector_from_executor(executor), {})
 
   def test_node_selector_from_executor_empty(self):
     executor = local_executors.Kubernetes(xm.JobRequirements())
```

### Comparing `xmanager-0.3.0/xmanager/cloud/utils.py` & `xmanager-0.4.0/xmanager/cloud/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,18 +64,15 @@
   cluster = {}
   for i, domain in enumerate(workers):
     cluster[f'workerpool{i}'] = [domain]
   specs = []
   for i in range(len(workers)):
     spec = {
         'cluster': cluster,
-        'task': {
-            'type': f'workerpool{i}',
-            'index': i
-        },
+        'task': {'type': f'workerpool{i}', 'index': i},
     }
     specs.append(json.dumps(spec))
   return specs
 
 
 def get_workerpool_address(workerpool: str) -> str:
   """Creates a late-binding that is mapped at runtime."""
@@ -95,24 +92,28 @@
   for arg in args:
     match = late_bind_regex.search(arg)
     if match is None:
       result.append(arg)
     else:
       worker_type = match.group(1)
       result.append(
-          arg.replace(f'%objectname({worker_type})%',
-                      cluster_spec[worker_type][0]))
+          arg.replace(
+              f'%objectname({worker_type})%', cluster_spec[worker_type][0]
+          )
+      )
   return result
 
 
 def print_workerpool_address_args(argv: List[str]) -> None:
   # Note that this is method is called by
   # third_party/py/xmanager/cloud/data/wrapped_entrypoint.sh
   for arg in map_workerpool_address_args(argv[1:]):
-    print(arg,)
+    print(
+        arg,
+    )
 
 
 def create_workerpool_address_env_vars_script(path: str) -> None:
   """Create a script to map late-binding env vars to their value at runtime."""
   with open(path, 'w') as f:
     f.write('#!/bin/bash\n\n')
 
@@ -136,19 +137,20 @@
 
 
 def get_region() -> str:
   """Get the region of the current GCE VM from metadata, e.g. us-central1."""
   # Default VM instance metadata
   # https://cloud.google.com/compute/docs/metadata/default-metadata-values#vm_instance_metadata
   request = urllib.request.Request(
-      'http://metadata.google.internal/computeMetadata/v1/instance/zone')
+      'http://metadata.google.internal/computeMetadata/v1/instance/zone'
+  )
   request.add_header('Metadata-Flavor', 'Google')
   response = urllib.request.urlopen(request)
   content = str(response.read())
-  zone = content.strip('\'').split('/')[-1]
+  zone = content.strip("'").split('/')[-1]
   region = zone[:-2]
   return region
 
 
 def get_closest_bucket(bucket_names: List[str]) -> str:
   """Get the closest bucket from a list of buckets."""
   region = get_region()
```

### Comparing `xmanager-0.3.0/xmanager/cloud/utils_test.py` & `xmanager-0.4.0/xmanager/cloud/utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
   },
   "environment": "cloud",
   "task": {
     "type": "workerpool1",
     "index": 1,
     "trial": ""
   }
-}""".replace('\n', ' ')
+}""".replace(
+    '\n', ' '
+)
 
 
 class UtilsTest(unittest.TestCase):
 
   def tearDown(self):
     super(UtilsTest, self).tearDown()
     os.environ['CLUSTER_SPEC'] = ''
@@ -64,15 +66,16 @@
 
   def test_wrap_and_unwrap_addresses(self):
     arg = '--master=' + utils.get_workerpool_address('workerpool0')
     self.assertEqual(arg, '--master=%objectname(workerpool0)%')
     os.environ['CLUSTER_SPEC'] = _CLUSTER_SPEC
     self.assertEqual(
         utils.map_workerpool_address_args([arg]),
-        ['--master=cmle-training-workerpool0-ab-0:2222'])
+        ['--master=cmle-training-workerpool0-ab-0:2222'],
+    )
 
   def test_create_workerpool_address_env_vars_script(self):
     os.environ['MY_WORKER'] = utils.get_workerpool_address('workerpool0')
     os.environ['CLUSTER_SPEC'] = _CLUSTER_SPEC
     t = tempfile.NamedTemporaryFile()
     utils.create_workerpool_address_env_vars_script(t.name)
     expected = """
```

### Comparing `xmanager-0.3.0/xmanager/cloud/vertex.py` & `xmanager-0.4.0/xmanager/cloud/vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,30 +65,38 @@
 
 _CLOUD_TPU_ACCELERATOR_TYPES = {
     xm.ResourceType.TPU_V2: 'TPU_V2',
     xm.ResourceType.TPU_V3: 'TPU_V3',
 }
 
 _STATE_TO_STATUS = {
-    aip_v1.JobState.JOB_STATE_SUCCEEDED:
-        local_status.LocalWorkUnitStatusEnum.COMPLETED,
-    aip_v1.JobState.JOB_STATE_CANCELLED:
-        local_status.LocalWorkUnitStatusEnum.CANCELLED,
-    aip_v1.JobState.JOB_STATE_QUEUED:
-        local_status.LocalWorkUnitStatusEnum.RUNNING,
-    aip_v1.JobState.JOB_STATE_PENDING:
-        local_status.LocalWorkUnitStatusEnum.RUNNING,
-    aip_v1.JobState.JOB_STATE_RUNNING:
-        local_status.LocalWorkUnitStatusEnum.RUNNING,
-    aip_v1.JobState.JOB_STATE_CANCELLING:
-        local_status.LocalWorkUnitStatusEnum.RUNNING,
-    aip_v1.JobState.JOB_STATE_PAUSED:
-        local_status.LocalWorkUnitStatusEnum.RUNNING,
-    aip_v1.JobState.JOB_STATE_FAILED:
-        local_status.LocalWorkUnitStatusEnum.FAILED,
+    aip_v1.JobState.JOB_STATE_SUCCEEDED: (
+        local_status.LocalWorkUnitStatusEnum.COMPLETED
+    ),
+    aip_v1.JobState.JOB_STATE_CANCELLED: (
+        local_status.LocalWorkUnitStatusEnum.CANCELLED
+    ),
+    aip_v1.JobState.JOB_STATE_QUEUED: (
+        local_status.LocalWorkUnitStatusEnum.RUNNING
+    ),
+    aip_v1.JobState.JOB_STATE_PENDING: (
+        local_status.LocalWorkUnitStatusEnum.RUNNING
+    ),
+    aip_v1.JobState.JOB_STATE_RUNNING: (
+        local_status.LocalWorkUnitStatusEnum.RUNNING
+    ),
+    aip_v1.JobState.JOB_STATE_CANCELLING: (
+        local_status.LocalWorkUnitStatusEnum.RUNNING
+    ),
+    aip_v1.JobState.JOB_STATE_PAUSED: (
+        local_status.LocalWorkUnitStatusEnum.RUNNING
+    ),
+    aip_v1.JobState.JOB_STATE_FAILED: (
+        local_status.LocalWorkUnitStatusEnum.FAILED
+    ),
 }
 
 # Hide noisy warning regarding:
 # `file_cache is unavailable when using oauth2client >= 4.0.0 or google-auth`
 logging.getLogger('googleapiclient.discovery_cache').setLevel(logging.ERROR)
 
 _default_client = None
@@ -97,17 +105,17 @@
 def _vertex_job_predicate(job: xm.Job) -> bool:
   return isinstance(job.executor, local_executors.Vertex)
 
 
 class Client:
   """Client class for interacting with AI Platform (Unified)."""
 
-  def __init__(self,
-               project: Optional[str] = None,
-               location: str = _DEFAULT_LOCATION) -> None:
+  def __init__(
+      self, project: Optional[str] = None, location: str = _DEFAULT_LOCATION
+  ) -> None:
     """Create a client.
 
     Args:
       project: GCP project ID.
       location: Location of the API endpoint. Defaults to region us-central1.
         https://cloud.google.com/vertex-ai/docs/reference/rest#service-endpoint
     """
@@ -118,26 +126,32 @@
 
   def launch(self, name: str, jobs: Sequence[xm.Job]) -> str:
     """Launch jobs on AI Platform (Unified)."""
     pools = []
     tensorboard, output_dir = self.get_tensorboard_settings(jobs)
     for i, job in enumerate(jobs):
       executable = job.executable
-      if not isinstance(executable,
-                        local_executables.GoogleContainerRegistryImage):
-        raise ValueError('Executable {} has type {}. Executable must be of '
-                         'type GoogleContainerRegistryImage'.format(
-                             executable, type(executable)))
+      if not isinstance(
+          executable, local_executables.GoogleContainerRegistryImage
+      ):
+        raise ValueError(
+            'Executable {} has type {}. Executable must be of '
+            'type GoogleContainerRegistryImage'.format(
+                executable, type(executable)
+            )
+        )
 
       args = xm.merge_args(executable.args, job.args).to_list(utils.ARG_ESCAPER)
       env_vars = {**executable.env_vars, **job.env_vars}
       env = [{'name': k, 'value': v} for k, v in env_vars.items()]
       if i == 0 and job.executor.requirements.replicas > 1:
-        raise ValueError('The first job in a JobGroup using the Vertex AI '
-                         'executor cannot have requirements.replicas > 1.')
+        raise ValueError(
+            'The first job in a JobGroup using the Vertex AI '
+            'executor cannot have requirements.replicas > 1.'
+        )
       pool = aip_v1.WorkerPoolSpec(
           machine_spec=get_machine_spec(job),
           container_spec=aip_v1.ContainerSpec(
               image_uri=executable.image_path,
               args=args,
               env=env,
           ),
@@ -148,17 +162,18 @@
     # TOOD(chenandrew): Vertex Training only allows for 4 worker pools.
     # If Vertex does not implement more worker pools, another work-around
     # is to simply put all jobs into the same worker pool as replicas.
     # Each replica would contain the same image, but would execute different
     # modules based the replica index. A disadvantage of this implementation
     # is that every replica must have the same machine_spec.
     if len(pools) > 4:
-      raise ValueError('Cloud Job for xm jobs {} contains {} worker types. '
-                       'Only 4 worker types are supported'.format(
-                           jobs, len(pools)))
+      raise ValueError(
+          'Cloud Job for xm jobs {} contains {} worker types. '
+          'Only 4 worker types are supported'.format(jobs, len(pools))
+      )
 
     custom_job = aiplatform.CustomJob(
         project=self.project,
         location=self.location,
         display_name=name,
         worker_pool_specs=pools,
         base_output_dir=output_dir,
@@ -168,88 +183,97 @@
     # https://github.com/deepmind/xmanager/issues/11
     service_account = auth.get_service_account()
     for job in jobs:
       assert isinstance(job.executor, local_executors.Vertex)
       if job.executor.requirements.accelerator in xm.TpuType:
         service_account = None
         break
-    custom_job.run(
-        sync=False,
+    custom_job.submit(
         service_account=service_account,
         tensorboard=tensorboard,
         enable_web_access=True,
     )
-    custom_job.wait_for_resource_creation()
     print(f'Job launched at: {custom_job._dashboard_uri()}')  # pylint: disable=protected-access
     return custom_job.resource_name
 
   def get_tensorboard_settings(self, jobs: Sequence[xm.Job]) -> Tuple[str, str]:
     """Get the tensorboard settings for a sequence of Jobs."""
     executors = []
     for job in jobs:
       assert isinstance(job.executor, local_executors.Vertex)
       executors.append(job.executor)
     if all(not executor.tensorboard for executor in executors):
       return '', ''
 
     if not executors[0].tensorboard:
       raise ValueError(
-          'Jobs in this job group must have the same tensorboard settings. ' +
-          'jobs[0] has no tensorboard settings.')
+          'Jobs in this job group must have the same tensorboard settings. '
+          + 'jobs[0] has no tensorboard settings.'
+      )
     output_dir = executors[0].tensorboard.base_output_directory
     tensorboard = executors[0].tensorboard.name
     for i, executor in enumerate(executors):
       if not executor:
         raise ValueError(
-            'Jobs in this job group must have the same tensorboard settings. ' +
-            'jobs[i] has no tensorboard settings.')
-      if (executor.tensorboard.name != tensorboard or
-          executor.tensorboard.base_output_directory != output_dir):
+            'Jobs in this job group must have the same tensorboard settings. '
+            + 'jobs[i] has no tensorboard settings.'
+        )
+      if (
+          executor.tensorboard.name != tensorboard
+          or executor.tensorboard.base_output_directory != output_dir
+      ):
         raise ValueError(
-            'Jobs in this job group must have the same tensorboard settings. ' +
-            f'jobs[0] has tensorboard = {tensorboard} and output_dir =' +
-            f'{output_dir}. jobs[{i}] has tensorboard = ' +
-            f'{executor.tensorboard.name} and output_dir = '
-            f'{executor.tensorboard.base_output_directory}.')
+            'Jobs in this job group must have the same tensorboard settings. '
+            + f'jobs[0] has tensorboard = {tensorboard} and output_dir ='
+            + f'{output_dir}. jobs[{i}] has tensorboard = '
+            + f'{executor.tensorboard.name} and output_dir = '
+            f'{executor.tensorboard.base_output_directory}.'
+        )
     if output_dir and not output_dir.startswith('gs://'):
       output_dir = os.path.join('gs://', output_dir)
     return tensorboard, output_dir
 
   async def wait_for_job(self, job_name: str) -> None:
     job = aiplatform.CustomJob.get(job_name)
     loop = asyncio.get_event_loop()
     return await loop.run_in_executor(None, job._block_until_complete)  # pylint: disable=protected-access
 
   def cancel(self, job_name: str) -> None:
     aiplatform.CustomJob.get(job_name).cancel()
 
   async def get_or_create_tensorboard(self, name: str) -> str:
     """Gets or creates a Vertex Tensorboard instance."""
-    tensorboard_client = aip_v1.TensorboardServiceAsyncClient(client_options={
-        'api_endpoint': f'{self.location}-aiplatform.googleapis.com'
-    })
+    tensorboard_client = aip_v1.TensorboardServiceAsyncClient(
+        client_options={
+            'api_endpoint': f'{self.location}-aiplatform.googleapis.com'
+        }
+    )
     request = aip_v1.ListTensorboardsRequest(
-        parent=self.parent, filter=f'displayName={name}')
+        parent=self.parent, filter=f'displayName={name}'
+    )
     response = await tensorboard_client.list_tensorboards(request)
     async for page in response.pages:
       if page.tensorboards:
         return response.tensorboards[0].name
     return await self.create_tensorboard(name)
 
   async def create_tensorboard(self, name: str) -> str:
     """Creates a Vertex Tensorboard instance."""
-    tensorboard_client = aip_v1.TensorboardServiceAsyncClient(client_options={
-        'api_endpoint': f'{self.location}-aiplatform.googleapis.com'
-    })
+    tensorboard_client = aip_v1.TensorboardServiceAsyncClient(
+        client_options={
+            'api_endpoint': f'{self.location}-aiplatform.googleapis.com'
+        }
+    )
     tensorboard = aip_v1.Tensorboard(display_name=name)
     op = await tensorboard_client.create_tensorboard(
         aip_v1.CreateTensorboardRequest(
             parent=self.parent,
             tensorboard=tensorboard,
-        ))
+        )
+    )
     return (await op.result()).name
 
   def get_state(self, job_name: str) -> aip_v1.JobState:
     return aiplatform.CustomJob.get(job_name).state
 
 
 def set_default_client(client: Client) -> None:
@@ -272,39 +296,38 @@
   for resource, value in requirements.task_requirements.items():
     accelerator_type = None
     if resource in xm.GpuType:
       accelerator_type = 'NVIDIA_TESLA_' + str(resource).upper()
     elif resource in xm.TpuType:
       accelerator_type = _CLOUD_TPU_ACCELERATOR_TYPES[resource]
     if accelerator_type:
-      # TPU_V2 and TPU_V3 removed in
-      # https://github.com/googleapis/python-aiplatform/commit/f3a3d03c8509dc49c24139155a572dacbe954f66
-      # Hardcode their values until they are reintroduced.
-      if accelerator_type == 'TPU_V2':
-        spec['accelerator_type'] = 6
-      elif accelerator_type == 'TPU_V3':
-        spec['accelerator_type'] = 7
-      else:
-        spec['accelerator_type'] = aip_v1.AcceleratorType[accelerator_type]
+      spec['accelerator_type'] = aip_v1.AcceleratorType[accelerator_type]
       spec['accelerator_count'] = int(value)
   accelerator = spec.get('accelerator_type', None)
   if accelerator and accelerator == aip_v1.AcceleratorType.NVIDIA_TESLA_A100:
-    for (gpus, machine_type) in sorted(_A100_GPUS_TO_MACHINE_TYPE.items()):
+    for gpus, machine_type in sorted(_A100_GPUS_TO_MACHINE_TYPE.items()):
       if spec['accelerator_count'] <= gpus:
         spec['machine_type'] = machine_type
         break
     if not spec.get('machine_type', None):
-      raise ValueError('a100={} does not fit in any valid machine type'.format(
-          spec['accelerator_count']))
-  elif accelerator == 6 or accelerator == 7:
+      raise ValueError(
+          'a100={} does not fit in any valid machine type'.format(
+              spec['accelerator_count']
+          )
+      )
+  elif (
+      accelerator == aip_v1.AcceleratorType.TPU_V2
+      or accelerator == aip_v1.AcceleratorType.TPU_V3
+  ):
     spec['machine_type'] = 'cloud-tpu'
   else:
     spec['machine_type'] = cpu_ram_to_machine_type(
         requirements.task_requirements.get(xm.ResourceType.CPU),
-        requirements.task_requirements.get(xm.ResourceType.RAM))
+        requirements.task_requirements.get(xm.ResourceType.RAM),
+    )
   return spec
 
 
 @attr.s(auto_attribs=True)
 class VertexHandle(local_execution.ExecutionHandle):
   """A handle for referring to the launched container."""
 
@@ -319,19 +342,21 @@
   def get_status(self) -> local_status.LocalWorkUnitStatus:
     state = get_default_client().get_state(self.job_name)
     status = _STATE_TO_STATUS[state]
     return local_status.LocalWorkUnitStatus(status=status)
 
 
 # Must act on all jobs with `local_executors.Vertex` executor.
-def launch(experiment_title: str, work_unit_name: str,
-           job_group: xm.JobGroup) -> List[VertexHandle]:
+def launch(
+    experiment_title: str, work_unit_name: str, job_group: xm.JobGroup
+) -> List[VertexHandle]:
   """Launch Vertex jobs in the job_group and return a handler."""
-  jobs = xm.job_operators.collect_jobs_by_filter(job_group,
-                                                 _vertex_job_predicate)
+  jobs = xm.job_operators.collect_jobs_by_filter(
+      job_group, _vertex_job_predicate
+  )
   # As client creation may throw, do not initiate it if there are no jobs.
   if not jobs:
     return []
 
   job_name = get_default_client().launch(
       name=f'{experiment_title}_{work_unit_name}',
       jobs=jobs,
@@ -344,20 +369,22 @@
   cpu = cpu or 0
   ram = ram or 0
   if cpu + ram == 0:
     return 'n1-standard-4'
 
   optimal_machine_type = ''
   optimal_excess_resources = math.inf
-  for machine_type, (machine_cpu,
-                     machine_ram) in _MACHINE_TYPE_TO_CPU_RAM.items():
+  for machine_type, (
+      machine_cpu,
+      machine_ram,
+  ) in _MACHINE_TYPE_TO_CPU_RAM.items():
     if machine_cpu >= cpu and machine_ram >= ram:
       excess = machine_cpu + machine_ram - cpu - ram
       if excess < optimal_excess_resources:
         optimal_machine_type = machine_type
         optimal_excess_resources = excess
 
   if optimal_machine_type:
     return optimal_machine_type
   raise ValueError(
-      '(cpu={}, ram={}) does not fit in any valid machine type'.format(
-          cpu, ram))
+      '(cpu={}, ram={}) does not fit in any valid machine type'.format(cpu, ram)
+  )
```

### Comparing `xmanager-0.3.0/xmanager/cloud/vertex_test.py` & `xmanager-0.4.0/xmanager/cloud/vertex_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,141 +46,156 @@
         name='test-job',
         executable=local_executables.GoogleContainerRegistryImage(
             name='test-image',
             image_path='image-path',
             args=xm.SequentialArgs.from_collection({'a': 1}),
         ),
         executor=local_executors.Vertex(xm.JobRequirements(cpu=1, ram=1, t4=2)),
-        args={
-            'b': 2,
-            'c': 3
-        },
+        args={'b': 2, 'c': 3},
     )
 
     expected_call = {
-        'parent':
-            'projects/test-project/locations/us-central1',
-        'custom_job':
-            aip_v1.CustomJob(
-                display_name='test-experiment',
-                job_spec=aip_v1.CustomJobSpec(
-                    worker_pool_specs=[
-                        aip_v1.WorkerPoolSpec(
-                            machine_spec=aip_v1.MachineSpec(
-                                machine_type='n1-highmem-2',
-                                accelerator_type='NVIDIA_TESLA_T4',
-                                accelerator_count=2,
-                            ),
-                            replica_count=1,
-                            container_spec=aip_v1.ContainerSpec(
-                                image_uri='image-path',
-                                args=['--a=1', '--b=2', '--c=3'],
-                            ))
-                    ],
-                    service_account='test-sa',
-                    base_output_directory=aip_v1.GcsDestination(
-                        output_uri_prefix='gs://test-bucket/aiplatform-custom-job-2022-01-01-00:00:00.000',
-                    ),
-                    enable_web_access=True,
+        'parent': 'projects/test-project/locations/us-central1',
+        'custom_job': aip_v1.CustomJob(
+            display_name='test-experiment',
+            job_spec=aip_v1.CustomJobSpec(
+                worker_pool_specs=[
+                    aip_v1.WorkerPoolSpec(
+                        machine_spec=aip_v1.MachineSpec(
+                            machine_type='n1-highmem-2',
+                            accelerator_type='NVIDIA_TESLA_T4',
+                            accelerator_count=2,
+                        ),
+                        replica_count=1,
+                        container_spec=aip_v1.ContainerSpec(
+                            image_uri='image-path',
+                            args=['--a=1', '--b=2', '--c=3'],
+                        ),
+                    )
+                ],
+                service_account='test-sa',
+                base_output_directory=aip_v1.GcsDestination(
+                    output_uri_prefix='gs://test-bucket/aiplatform-custom-job-2022-01-01-00:00:00.000',
                 ),
+                enable_web_access=True,
             ),
-        'timeout':
-            None,
+        ),
+        'timeout': None,
     }
 
     timestamp = datetime.datetime.strptime('2022/1/1', '%Y/%m/%d')
-    with mock.patch.object(datetime, 'datetime') as mock_timestamp, \
-         mock.patch.object(aip_utils.ClientWithOverride, 'WrappedClient') as job_client, \
-         mock.patch.object(aiplatform.CustomJob, 'resource_name', new_callable=mock.PropertyMock) as name, \
-         mock.patch.object(aiplatform.CustomJob, '_dashboard_uri'):
+    with mock.patch.object(
+        datetime, 'datetime'
+    ) as mock_timestamp, mock.patch.object(
+        aip_utils.ClientWithOverride, 'WrappedClient'
+    ) as job_client, mock.patch.object(
+        aiplatform.CustomJob, 'resource_name', new_callable=mock.PropertyMock
+    ) as name, mock.patch.object(
+        aiplatform.CustomJob, '_dashboard_uri'
+    ):
       mock_timestamp.now.return_value = timestamp
       name.return_value = 'test-resource-name'
       client.launch('test-experiment', [job])
       job_client.return_value.create_custom_job.assert_called_once_with(  # pytype: disable=attribute-error  # py39-upgrade
-          **expected_call)
+          **expected_call
+      )
 
   def test_get_machine_spec_default(self):
     job = xm.Job(
         executable=local_executables.GoogleContainerRegistryImage('name', ''),
         executor=local_executors.Vertex(),
-        args={})
+        args={},
+    )
     machine_spec = vertex.get_machine_spec(job)
     self.assertDictEqual(machine_spec, {'machine_type': 'n1-standard-4'})
 
   def test_get_machine_spec_cpu(self):
     job = xm.Job(
         executable=local_executables.GoogleContainerRegistryImage('name', ''),
         executor=local_executors.Vertex(
-            requirements=xm.JobRequirements(cpu=20, ram=40 * xm.GiB)),
-        args={})
+            requirements=xm.JobRequirements(cpu=20, ram=40 * xm.GiB)
+        ),
+        args={},
+    )
     machine_spec = vertex.get_machine_spec(job)
     self.assertDictEqual(machine_spec, {'machine_type': 'n1-highcpu-64'})
 
   def test_get_machine_spec_gpu(self):
     job = xm.Job(
         executable=local_executables.GoogleContainerRegistryImage('name', ''),
         executor=local_executors.Vertex(
-            requirements=xm.JobRequirements(p100=2)),
-        args={})
+            requirements=xm.JobRequirements(p100=2)
+        ),
+        args={},
+    )
     machine_spec = vertex.get_machine_spec(job)
     self.assertDictEqual(
-        machine_spec, {
+        machine_spec,
+        {
             'machine_type': 'n1-standard-4',
             'accelerator_type': vertex.aip_v1.AcceleratorType.NVIDIA_TESLA_P100,
             'accelerator_count': 2,
-        })
+        },
+    )
 
   def test_get_machine_spec_a100(self):
     job = xm.Job(
         executable=local_executables.GoogleContainerRegistryImage('name', ''),
         executor=local_executors.Vertex(
-            requirements=xm.JobRequirements(a100=2)),
-        args={})
+            requirements=xm.JobRequirements(a100=2)
+        ),
+        args={},
+    )
     machine_spec = vertex.get_machine_spec(job)
     self.assertDictEqual(
-        machine_spec, {
+        machine_spec,
+        {
             'machine_type': 'a2-highgpu-2g',
             'accelerator_type': vertex.aip_v1.AcceleratorType.NVIDIA_TESLA_A100,
             'accelerator_count': 2,
-        })
+        },
+    )
 
   def test_get_machine_spec_tpu(self):
     job = xm.Job(
         executable=local_executables.GoogleContainerRegistryImage('name', ''),
         executor=local_executors.Vertex(
-            requirements=xm.JobRequirements(tpu_v3=8)),
-        args={})
+            requirements=xm.JobRequirements(tpu_v3=8)
+        ),
+        args={},
+    )
     machine_spec = vertex.get_machine_spec(job)
-    # TPU_V2 and TPU_V3 removed in
-    # https://github.com/googleapis/python-aiplatform/commit/f3a3d03c8509dc49c24139155a572dacbe954f66
-    # When TPU enums are restored, replace
-    #   'accelerator_type': 7,
-    # with
-    #   'accelerator_type': vertex.aip_v1.AcceleratorType.TPU_V3,
-    self.assertDictEqual(machine_spec, {
-        'machine_type': 'cloud-tpu',
-        'accelerator_type': 7,
-        'accelerator_count': 8,
-    })
+    self.assertDictEqual(
+        machine_spec,
+        {
+            'machine_type': 'cloud-tpu',
+            'accelerator_type': vertex.aip_v1.AcceleratorType.TPU_V3,
+            'accelerator_count': 8,
+        },
+    )
 
   def test_cpu_ram_to_machine_type_exact(self):
-    self.assertEqual('n1-standard-16',
-                     vertex.cpu_ram_to_machine_type(16, 60 * xm.GiB))
+    self.assertEqual(
+        'n1-standard-16', vertex.cpu_ram_to_machine_type(16, 60 * xm.GiB)
+    )
 
   def test_cpu_ram_to_machine_type_highmem(self):
-    self.assertEqual('n1-highmem-64',
-                     vertex.cpu_ram_to_machine_type(1, 415 * xm.GiB))
+    self.assertEqual(
+        'n1-highmem-64', vertex.cpu_ram_to_machine_type(1, 415 * xm.GiB)
+    )
 
   def test_cpu_ram_to_machine_type_mem_only(self):
-    self.assertEqual('n1-highmem-64',
-                     vertex.cpu_ram_to_machine_type(None, 415 * xm.GiB))
+    self.assertEqual(
+        'n1-highmem-64', vertex.cpu_ram_to_machine_type(None, 415 * xm.GiB)
+    )
 
   def test_cpu_ram_to_machine_type_highcpu(self):
-    self.assertEqual('n1-highcpu-64',
-                     vertex.cpu_ram_to_machine_type(63, 1 * xm.GiB))
+    self.assertEqual(
+        'n1-highcpu-64', vertex.cpu_ram_to_machine_type(63, 1 * xm.GiB)
+    )
 
   def test_cpu_ram_to_machine_type_cpu_only(self):
     self.assertEqual('n1-highcpu-64', vertex.cpu_ram_to_machine_type(63, None))
 
   def test_cpu_ram_to_machine_type_too_high(self):
     with self.assertRaises(ValueError):
       vertex.cpu_ram_to_machine_type(1000, 1000)
```

### Comparing `xmanager-0.3.0/xmanager/contrib/__init__.py` & `xmanager-0.4.0/xmanager/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/contrib/addressing.py` & `xmanager-0.4.0/xmanager/contrib/addressing.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 """Module for getting the address of XManager jobs.
 
 Addresses in XManager can be statically evaluated because the experiment ID is
 known. Addressing should not involve tokens or late-bindings.
 """
 
 
-def k8s_pod_domain(job_name: str,
-                   experiment_id: int,
-                   work_unit_id: int,
-                   service: str = 'experiments',
-                   namespace: str = 'default') -> str:
+def k8s_pod_domain(
+    job_name: str,
+    experiment_id: int,
+    work_unit_id: int,
+    service: str = 'experiments',
+    namespace: str = 'default',
+) -> str:
   """Returns the Kubernetes pod address of a job.
 
   Args:
     job_name: Job name.
     experiment_id: Experiment ID.
     work_unit_id: Work unit ID
     service: Name of the service for the job. Defaults to 'experiments'
     namespace: Namespace of the job. Defaults to 'default'
   """
-  return (f'{experiment_id}-{work_unit_id}-{job_name}'
-          f'.{service}.{namespace}.svc.cluster.local:2222')
+  return (
+      f'{experiment_id}-{work_unit_id}-{job_name}'
+      f'.{service}.{namespace}.svc.cluster.local:2222'
+  )
```

### Comparing `xmanager-0.3.0/xmanager/contrib/addressing_test.py` & `xmanager-0.4.0/xmanager/contrib/addressing_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
   def test_k8s_pod_domain(self):
     address = addressing.k8s_pod_domain(
         job_name='cifar10',
         experiment_id=123,
         work_unit_id=4,
         service='best_service',
-        namespace='best_namespace')
+        namespace='best_namespace',
+    )
 
     self.assertEqual(
         address,
-        '123-4-cifar10.best_service.best_namespace.svc.cluster.local:2222')
+        '123-4-cifar10.best_service.best_namespace.svc.cluster.local:2222',
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/contrib/copybara.py` & `xmanager-0.4.0/xmanager/contrib/copybara.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,19 +50,21 @@
 from typing import Optional
 
 # Set with the compiled path to copybara e.g.
 # COPYBARA_BIN = 'bazel-bin/java/com/google/copybara/copybara_deploy.jar'
 COPYBARA_BIN = 'copybara'
 
 
-def run_workflow(config: str,
-                 workflow: str,
-                 origin_folder: str,
-                 destination_folder: Optional[str] = None,
-                 config_root: Optional[str] = None) -> str:
+def run_workflow(
+    config: str,
+    workflow: str,
+    origin_folder: str,
+    destination_folder: Optional[str] = None,
+    config_root: Optional[str] = None,
+) -> str:
   """Run a workflow in a copybara config to transform origin to destination.
 
   Args:
     config: Path to the Copybara config.
     workflow: Name of a workflow in copybara config.
     origin_folder: The origin folder to use as input. This will passed to
       Copybara via the source_ref argument.
@@ -73,15 +75,19 @@
   Returns:
     The output destination folder.
   """
   origin_folder = os.path.abspath(origin_folder)
   if not destination_folder:
     destination_folder = tempfile.mkdtemp()
   command = [
-      COPYBARA_BIN, config, workflow, '--ignore-noop', origin_folder,
-      '--folder-dir=' + destination_folder
+      COPYBARA_BIN,
+      config,
+      workflow,
+      '--ignore-noop',
+      origin_folder,
+      '--folder-dir=' + destination_folder,
   ]
   if config_root:
     command += ['--config-root=' + config_root]
   print('Copybara command: ', command)
   subprocess.run(command, check=True)
   return destination_folder
```

### Comparing `xmanager-0.3.0/xmanager/contrib/executor_selector.py` & `xmanager-0.4.0/xmanager/contrib/executor_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,35 +53,39 @@
 from absl import flags
 from xmanager import xm
 from xmanager import xm_local
 
 
 class XMLaunchMode(enum.Enum):
   """Specifies an executor to run an experiment."""
+
   VERTEX = 'vertex'
   LOCAL = 'local'
   INTERACTIVE = 'interactive'
 
 
 _XM_LAUNCH_MODE = flags.DEFINE_enum_class(
     'xm_launch_mode',
     XMLaunchMode.VERTEX,
     XMLaunchMode,
-    'How to launch the experiment. Supports local and interactive execution, ' +
-    'launch on ' +
-    'Vertex.')
+    'How to launch the experiment. Supports local and interactive execution, '
+    + 'launch on '
+    +
+    'Vertex.',
+)
 
 
 def launch_mode() -> XMLaunchMode:
   return _XM_LAUNCH_MODE.value
 
 
 def create_experiment(
     experiment_title: Optional[str] = None,
-    mode: Optional[XMLaunchMode] = None) -> xm.Experiment:
+    mode: Optional[XMLaunchMode] = None,
+) -> xm.Experiment:
   """Creates an experiment depending on the launch mode.
 
   Args:
     experiment_title: Title of an experiment
     mode: Specifies which experiment to create. If None, the '--xm_launch_mode'
       flag value is used.
 
@@ -90,41 +94,46 @@
 
   Raises:
     ValueError: if provided `mode` is unknown.
   """
   if mode is None:
     mode = launch_mode()
 
-  if mode in (XMLaunchMode.LOCAL, XMLaunchMode.INTERACTIVE,
-              XMLaunchMode.VERTEX):
+  if mode in (
+      XMLaunchMode.LOCAL,
+      XMLaunchMode.INTERACTIVE,
+      XMLaunchMode.VERTEX,
+  ):
     # TODO: add import here?
     return xm_local.create_experiment(experiment_title)
   raise ValueError(f'Unknown launch mode: {mode}')
 
 
 def _local_executor(interactive: bool) -> Callable[..., xm.Executor]:
   """Helper to provide a local executor with appropriate `interactive` flag."""
 
   def setup_local(*args, **kwargs_in) -> xm_local.Local:
     kwargs = {}
     # Copy supported arguments.
     if 'experimental_stream_output' in kwargs_in:
       kwargs['experimental_stream_output'] = kwargs_in[
-          'experimental_stream_output']
+          'experimental_stream_output'
+      ]
     # Set the specified value of `interactive`.
     docker_options = kwargs_in.get('docker_options', xm_local.DockerOptions())
     setattr(docker_options, 'interactive', interactive)
     kwargs['docker_options'] = docker_options
     return xm_local.Local(*args, **kwargs)
 
   return setup_local
 
 
 def get_executor(
-    mode: Optional[XMLaunchMode] = None) -> Callable[..., xm.Executor]:
+    mode: Optional[XMLaunchMode] = None,
+) -> Callable[..., xm.Executor]:
   """Select an `xm.Executor` specialization depending on the launch mode.
 
   Args:
     mode: Specifies which class to select. If None, the '--xm_launch_mode' flag
       value is used.
 
   Returns:
@@ -134,10 +143,10 @@
     ValueError: if provided `mode` is unknown.
   """
   if mode is None:
     mode = launch_mode()
 
   if mode == XMLaunchMode.VERTEX:
     return xm_local.Caip
-  if (mode == XMLaunchMode.LOCAL or mode == XMLaunchMode.INTERACTIVE):
+  if mode == XMLaunchMode.LOCAL or mode == XMLaunchMode.INTERACTIVE:
     return _local_executor(mode == XMLaunchMode.INTERACTIVE)
   raise ValueError(f'Unknown launch mode: {mode}')
```

### Comparing `xmanager-0.3.0/xmanager/contrib/framework_defaults.py` & `xmanager-0.4.0/xmanager/contrib/framework_defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,68 +31,74 @@
 
 from absl import logging
 from xmanager import xm
 
 
 class MLFramework(enum.Enum):
   """ML Framework used in the experiment code."""
+
   UNKNOWN = 0
   JAX = 1
   PYTORCH = 2
   TF2 = 3
   TF1 = 4  # Unsupported
 
 
 FrameworkSpec = Union[str, MLFramework]
 
 
 def _get_framework(framework: str) -> MLFramework:
   """Given a framework name in a loose form, returns the most suitable enum."""
-  if (framework == 'jax' or framework == 'flax'):
+  if framework == 'jax' or framework == 'flax':
     return MLFramework.JAX
   if 'torch' in framework:
     return MLFramework.PYTORCH
   if 'tf' in framework or 'tensorflow' in framework:
     # A variant of a Tensorflow.
     return MLFramework.TF1 if '1' in framework else MLFramework.TF2
   # Framework not recognized.
   logging.error('Unrecognized framework "%s"', framework)
   return MLFramework.UNKNOWN
 
 
-def base_image(framework: FrameworkSpec,
-               accelerator: Optional[xm.ResourceType]) -> str:
+def base_image(
+    framework: FrameworkSpec, accelerator: Optional[xm.ResourceType]
+) -> str:
   """Returns a base image recommendation depending on the input.
 
   Please note that the recommendations can change as we are trying to recommend
-  the latest supported images for all frameworks.
+  the latest supported images for all frameworks. Currently most of the images
+  are taken from
+  https://cloud.google.com/deep-learning-containers/docs/choosing-container.
 
   Args:
     framework: a free-text framework name. Recognized options are `jax`,
       `pytorch`, `tf`, `tensorflow`. The enum value is also accepted.
     accelerator: Accelerator specification from xm.JobRequirements. If None,
       then execution on CPU is assumed.
 
   Returns:
     a name of a base image to pass to e.g. xm.python_container.
   """
   if isinstance(framework, str):
     framework = _get_framework(framework)
+  # LINT.IfChange(base_image_version)
   if framework == MLFramework.JAX:
     # JAX-based experiment use the same base image for all accelerators.
     return 'gcr.io/deeplearning-platform-release/base-cu113'
   elif framework == MLFramework.TF2:
     # TF experiments use the same base image for all accelerators.
     return 'gcr.io/deeplearning-platform-release/tf2-gpu.2-6'
   elif framework == MLFramework.PYTORCH:
     if accelerator in xm.TpuType:
       # Base image is taken from pytorch / XLA documentation.
       # https://github.com/pytorch/xla#-available-images-and-wheels
       return 'gcr.io/tpu-pytorch/xla:nightly_3.8_tpuvm_20220819'
     else:
-      return 'gcr.io/deeplearning-platform-release/pytorch-gpu.1-9'
+      return 'gcr.io/deeplearning-platform-release/pytorch-gpu.1-12'
+  # LINT.ThenChange(:tpu_runtime_version)
   elif framework == MLFramework.TF1:
     logging.warning('Tensorflow 1.x is not supported')
     return 'gcr.io/deeplearning-platform-release/tf-gpu.1-15'
   else:
     # Unrecognized framework: use the default CUDA image.
     return 'gcr.io/deeplearning-platform-release/base-cu113'
```

### Comparing `xmanager-0.3.0/xmanager/contrib/framework_defaults_test.py` & `xmanager-0.4.0/xmanager/contrib/framework_defaults_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,39 @@
 MLFramework = framework_defaults.MLFramework
 
 
 class FrameworkDefaultsTest(parameterized.TestCase):
 
   def test_known_frameworks(self):
     self.assertEqual(
-        framework_defaults._get_framework('torch'), MLFramework.PYTORCH)
+        framework_defaults._get_framework('torch'), MLFramework.PYTORCH
+    )
     self.assertEqual(
-        framework_defaults._get_framework('pytorch'), MLFramework.PYTORCH)
+        framework_defaults._get_framework('pytorch'), MLFramework.PYTORCH
+    )
     self.assertEqual(framework_defaults._get_framework('tf'), MLFramework.TF2)
     self.assertEqual(framework_defaults._get_framework('tf1'), MLFramework.TF1)
     self.assertEqual(framework_defaults._get_framework('tf2'), MLFramework.TF2)
     self.assertEqual(
-        framework_defaults._get_framework('tensorflow 2.x'), MLFramework.TF2)
+        framework_defaults._get_framework('tensorflow 2.x'), MLFramework.TF2
+    )
     self.assertEqual(framework_defaults._get_framework('jax'), MLFramework.JAX)
     self.assertEqual(framework_defaults._get_framework('flax'), MLFramework.JAX)
 
   def test_unknown_frameworks(self):
     self.assertEqual(
-        framework_defaults._get_framework('huggingface'), MLFramework.UNKNOWN)
+        framework_defaults._get_framework('huggingface'), MLFramework.UNKNOWN
+    )
     self.assertEqual(
-        framework_defaults._get_framework('objax'), MLFramework.UNKNOWN)
+        framework_defaults._get_framework('objax'), MLFramework.UNKNOWN
+    )
     self.assertEqual(
         framework_defaults._get_framework('not a framework name'),
-        MLFramework.UNKNOWN)
+        MLFramework.UNKNOWN,
+    )
 
   @parameterized.named_parameters(
       ('cpu', None),
       ('gpu', xm.ResourceType.V100),
       ('tpu', xm.ResourceType.TPU_V3),
   )
   def test_jax_base_image(self, accelerator):
@@ -71,15 +77,15 @@
       ('tpu', xm.ResourceType.TPU_V3),
   )
   def test_torch_base_image(self, accelerator):
     base_image = framework_defaults.base_image(MLFramework.PYTORCH, accelerator)
     self.assertStartsWith(base_image, 'gcr.io/')
     self.assertContainsSubsequence(base_image, 'pytorch')
     if accelerator in xm.TpuType:
-      self.assertContainsSubsequence(base_image, 'xla')
+      self.assertContainsSubsequence(base_image, 'tpu')
 
   @parameterized.named_parameters(
       ('cpu', None),
       ('gpu', xm.ResourceType.V100),
       ('tpu', xm.ResourceType.TPU_V3),
   )
   def test_unsupported_tf1_base_image(self, accelerator):
```

### Comparing `xmanager-0.3.0/xmanager/contrib/gcs.py` & `xmanager-0.4.0/xmanager/contrib/gcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,48 +25,59 @@
 import getpass
 import os
 
 from absl import app
 from absl import flags
 
 _GCS_PATH = flags.DEFINE_string(
-    'xm_gcs_path', None, 'A GCS directory within a bucket to store output '
-    '(in gs://bucket/directory format).')
+    'xm_gcs_path',
+    None,
+    (
+        'A GCS directory within a bucket to store output '
+        '(in gs://bucket/directory format).'
+    ),
+)
 
 _GS_PREFIX = 'gs://'
 _GCS_PREFIX = '/gcs/'
 
 
 _default_bucket_name = '<Your bucket>'
 
 
 def suggestion(project_name: str) -> str:
   """Returns a suggested GCS dir name for the given @project_name."""
   return os.path.join(
-      _GS_PREFIX, _default_bucket_name, getpass.getuser(),
-      project_name + '-' + datetime.datetime.now().strftime('%Y%m%d-%H%M%S'))
+      _GS_PREFIX,
+      _default_bucket_name,
+      getpass.getuser(),
+      project_name + '-' + datetime.datetime.now().strftime('%Y%m%d-%H%M%S'),
+  )
 
 
 def get_gcs_path_or_fail(project_name: str) -> str:
   """Returns value passed in the --xm_gcs_path flag; fails if nothing is passed.
 
   Args:
     project_name: a project name used to generate suggested GCS path.
 
   Returns:
     If the --xm_gcs_path flag is empty, or contains invalid value, raise an
     error. Otherwise, returns a flag value.
   """
   if not _GCS_PATH.value:
-    raise app.UsageError('--xm_gcs_path is missing. Suggestion: ' +
-                         f'--xm_gcs_path={suggestion(project_name)}')
+    raise app.UsageError(
+        '--xm_gcs_path is missing. Suggestion: '
+        + f'--xm_gcs_path={suggestion(project_name)}'
+    )
   elif not is_gcs_path(_GCS_PATH.value):
     raise app.UsageError(
-        '--xm_gcs_path not in gs://bucket/directory or /gcs/path format. ' +
-        f'Suggestion: --xm_gcs_path={suggestion(project_name)}')
+        '--xm_gcs_path not in gs://bucket/directory or /gcs/path format. '
+        + f'Suggestion: --xm_gcs_path={suggestion(project_name)}'
+    )
   return str(_GCS_PATH.value)
 
 
 def is_gs_path(path: str) -> bool:
   """Given the path, checks whether it is a valid Google Storage URL.
 
   Args:
@@ -108,19 +119,20 @@
   Args:
     path: GCS path in gs://bucket/directory format.
 
   Returns:
     Path without 'gs://' prefix.
   """
   if is_gs_path(path):
-    return path[len(_GS_PREFIX):]
+    return path[len(_GS_PREFIX) :]
   if is_gcs_fuse_path(path):
-    return path[len(_GCS_PREFIX):]
+    return path[len(_GCS_PREFIX) :]
   raise ValueError(
-      f'Path not in gs://bucket/directory or /gcs/path format: {path}')
+      f'Path not in gs://bucket/directory or /gcs/path format: {path}'
+  )
 
 
 # Exposed for testing.
 gcp_website_url = 'https://console.cloud.google.com'
 
 
 def get_gcs_url(path: str) -> str:
```

### Comparing `xmanager-0.3.0/xmanager/contrib/gcs_test.py` & `xmanager-0.4.0/xmanager/contrib/gcs_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from absl import app
 from absl.testing import absltest
 from absl.testing import flagsaver
 from absl.testing import parameterized
 from xmanager.contrib import gcs
 
 # Error patterns.
-_GCS_PATH_ERROR = ('--xm_gcs_path not in gs://bucket/directory or /gcs/path '
-                   'format.')
+_GCS_PATH_ERROR = (
+    '--xm_gcs_path not in gs://bucket/directory or /gcs/path format.'
+)
 _PATH_ERROR = 'Path not in gs://bucket/directory or /gcs/path format'
 
 
 class GcsTest(parameterized.TestCase):
 
   def test_gcs_path_empty_flag(self):
     with self.assertRaisesRegex(app.UsageError, '--xm_gcs_path is missing'):
@@ -57,24 +58,28 @@
     self.assertEqual(gcs.is_gs_path(path), expected_gs)
     self.assertEqual(gcs.is_gcs_fuse_path(path), expected_fuse)
     self.assertEqual(gcs.is_gcs_path(path), expected_gcs)
 
   def test_get_gcs_url(self):
     self.assertEqual(
         gcs.get_gcs_url('gs://a/b/c'),
-        f'{gcs.gcp_website_url}/storage/browser/a/b/c')
+        f'{gcs.gcp_website_url}/storage/browser/a/b/c',
+    )
     self.assertEqual(
         gcs.get_gcs_url('gs://d/e'),
-        f'{gcs.gcp_website_url}/storage/browser/d/e')
+        f'{gcs.gcp_website_url}/storage/browser/d/e',
+    )
     self.assertEqual(
         gcs.get_gcs_url('/gcs/a/b/c'),
-        f'{gcs.gcp_website_url}/storage/browser/a/b/c')
+        f'{gcs.gcp_website_url}/storage/browser/a/b/c',
+    )
     self.assertEqual(
         gcs.get_gcs_url('/gcs/d/e'),
-        f'{gcs.gcp_website_url}/storage/browser/d/e')
+        f'{gcs.gcp_website_url}/storage/browser/d/e',
+    )
     with self.assertRaisesRegex(ValueError, _PATH_ERROR):
       gcs.get_gcs_url('a/b/f')
 
   def test_get_gcs_fuse_path(self):
     self.assertEqual(gcs.get_gcs_fuse_path('gs://a/b/c'), '/gcs/a/b/c')
     self.assertEqual(gcs.get_gcs_fuse_path('gs://d/e'), '/gcs/d/e')
     self.assertEqual(gcs.get_gcs_fuse_path('/gcs/a/b/c'), '/gcs/a/b/c')
```

### Comparing `xmanager-0.3.0/xmanager/contrib/parameter_controller.py` & `xmanager-0.4.0/xmanager/contrib/parameter_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 import launchpad as lp
 import launchpad.nodes.python.xm_docker as lp_docker
 from xmanager import xm
 from xmanager import xm_local
 
 
 def _parameter_controller_job_args(
-    controller_args: Dict[str, Any]) -> Dict[str, Any]:
+    controller_args: Dict[str, Any]
+) -> Dict[str, Any]:
   """Converts given XM flags to coresponding Launchpad's `process_entry` flags.
 
   The XM client runs inside `process_entry`, but flags are not defined yet.
   The `flags_to_populate` flag in `process_entry` is used to define the
   given flags before calling `app.run()`. This function converts XM flags
   to the format desired by `process_entry`.
 
@@ -52,26 +53,27 @@
     controller_args: XM flags to be passed.
 
   Returns:
     Flags used to populate XM flags in `process_entry`
   """
   args = {
       'lp_task_id': 0,
-      'flags_to_populate': xm.ShellSafeArg(json.dumps(controller_args))
+      'flags_to_populate': xm.ShellSafeArg(json.dumps(controller_args)),
   }
 
   return args
 
 
-def _to_python_container(node: lp.PyNode, label: str,
-                         docker_config: lp.DockerConfig) -> xm.PythonContainer:
+def _to_python_container(
+    node: lp.PyNode, label: str, docker_config: lp.DockerConfig
+) -> xm.PythonContainer:
   """Returns xm.PythonContainer embedding a lp.PyNode."""
-  return lp_docker.to_docker_executables([node],
-                                         label=label,
-                                         docker_config=docker_config)[0][0]
+  return lp_docker.to_docker_executables(
+      [node], label=label, docker_config=docker_config
+  )[0][0]
 
 
 def _use_host_db_config(
     package_path: str,
     controller_args: Dict[str, Any],
 ) -> None:
   """Make DB config file used by host available to controller job.
@@ -88,20 +90,23 @@
   Raises:
     RuntimeError: The `--xm_db_yaml_config` flag will be overriden by this
       function. To avoid confusion about this behavior, an exception is thrown
       if it's already set.
   """
 
   if 'xm_db_yaml_config_path' in controller_args:
-    raise RuntimeError('Parameter controller can\'t use host DB config '
-                       'and also use `--xm_db_yaml_config_path` flag. Use '
-                       '`use_host_db_config=False` or remove the flag.')
+    raise RuntimeError(
+        "Parameter controller can't use host DB config "
+        'and also use `--xm_db_yaml_config_path` flag. Use '
+        '`use_host_db_config=False` or remove the flag.'
+    )
 
   config_path = xm.utils.resolve_path_relative_to_launcher(
-      flags.FLAGS.xm_db_yaml_config_path)
+      flags.FLAGS.xm_db_yaml_config_path
+  )
 
   if not os.path.isfile(os.path.join(package_path, config_path)):
     shutil.copy(config_path, package_path)
 
   controller_args['xm_db_yaml_config_path'] = os.path.basename(config_path)
 
 
@@ -122,30 +127,35 @@
   if use_host_db_config:
     _use_host_db_config(package_path, controller_args)
 
   docker_requirements = os.path.join(package_path, 'requirements.txt')
   docker_config = lp.DockerConfig(package_path, docker_requirements)
 
   executable_spec = _to_python_container(
-      node, f'{aux_unit.experiment_unit_name}_{function_label}', docker_config)
+      node, f'{aux_unit.experiment_unit_name}_{function_label}', docker_config
+  )
 
   [executable] = await asyncio.get_running_loop().run_in_executor(
-      None, aux_unit.experiment.package, [
+      None,
+      aux_unit.experiment.package,
+      [
           xm.Packageable(
               executable_spec=executable_spec,
               executor_spec=executor.Spec(),
           )
-      ])
+      ],
+  )
 
   controller_job = xm.Job(
       name=controller_name,
       executable=executable,
       executor=executor,
       args=_parameter_controller_job_args(controller_args) or {},
-      env_vars=controller_env_vars or {})
+      env_vars=controller_env_vars or {},
+  )
 
   aux_unit.add(controller_job)
 
 
 def _populate_flags(controller_args: Dict[str, Any]) -> None:
   """Sets flag values at runtime.
 
@@ -157,16 +167,17 @@
   Args:
     controller_args: Mapping of flag names and values to be set.
   """
   for name, value in controller_args.items():
     flags.FLAGS[name].value = value
 
 
-async def _controller_body(experiment_id, f, controller_args, *args,
-                           **kwargs) -> None:
+async def _controller_body(
+    experiment_id, f, controller_args, *args, **kwargs
+) -> None:
   _populate_flags(controller_args)
 
   async with xm_local.get_experiment(experiment_id) as experiment:
     await f(experiment, *args, **kwargs)
 
 
 def controller(
@@ -200,39 +211,44 @@
       controller job.
 
   Returns:
     A decorator to be applied to the function.
   """
 
   def wrap(f: Callable[..., None]) -> Callable[..., xm.JobGeneratorType]:
-
     def make_controller(*args, **kwargs) -> xm.JobType:
-
       async def job_generator(aux_unit: xm.ExperimentUnit) -> None:
         experiment_id = aux_unit.experiment.experiment_id
 
         remote_controller = asyncio.create_task(
             _launch_remote_controller(
                 aux_unit,
                 lp.PyNode(
-                    xm.run_in_asyncio_loop(_controller_body), experiment_id, f,
-                    controller_args, *args, **kwargs),
+                    xm.run_in_asyncio_loop(_controller_body),
+                    experiment_id,
+                    f,
+                    controller_args,
+                    *args,
+                    **kwargs,
+                ),
                 function_label=f.__name__,
                 executor=executor,
                 controller_name=controller_name,
                 controller_args=controller_args,
                 controller_env_vars=controller_env_vars,
                 package_path=package_path,
                 use_host_db_config=use_host_db_config,
-            ))
+            )
+        )
 
         await remote_controller
 
       return xm.AuxiliaryUnitJob(
           job_generator,
           importance=xm.Importance.HIGH,
           # TODO: Add support for `termination_delay_secs`.
-          termination_delay_secs=0)
+          termination_delay_secs=0,
+      )
 
     return make_controller
 
   return wrap
```

### Comparing `xmanager-0.3.0/xmanager/contrib/tensorboard.py` & `xmanager-0.4.0/xmanager/contrib/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Any, Mapping, Optional
 
 from xmanager import xm
 
 
 class TensorboardProvider:
   """A class to generate package and job/args to Tensorboard jobs."""
+
   DEFAULT_TENSORBOARD_PORT = 6006
 
   @staticmethod
   def get_tensorboard_packageable(timeout_secs: int) -> xm.PythonContainer:
     """Creates container spec running TensorBoard server.
 
     Args:
@@ -38,15 +39,16 @@
       period of time.
     """
     if timeout_secs < 0:
       raise RuntimeError('`timeout_secs` must be a nonnegative number')
 
     return xm.PythonContainer(
         base_image='tensorflow/tensorflow',
-        entrypoint=xm.CommandList([f'timeout {timeout_secs}s tensorboard']))
+        entrypoint=xm.CommandList([f'timeout {timeout_secs}s tensorboard']),
+    )
 
   @staticmethod
   def get_tensorboard_job_args(
       log_dir: str,
       port: Optional[int] = None,
       additional_args: Optional[Mapping[str, Any]] = None,
   ) -> Mapping[str, Any]:
@@ -58,15 +60,15 @@
         'host': '0.0.0.0',
         # This is set to true by default when running Tensorboard.
         # Since it doesn't seem to be working well with GKE Workload Identity,
         # we set it to false for now. Can be overriden through the
         # `additional_args` param.
         #
         # https://github.com/tensorflow/tensorboard/issues/4784#issuecomment-868945650
-        'load_fast': 'false'
+        'load_fast': 'false',
     }
     if additional_args:
       args.update(additional_args)
 
     return args
 
 
@@ -75,21 +77,25 @@
     logdir: str,
     executor: xm.Executor,
     timeout_secs: int = 60 * 60 * 24,
     args: Optional[Mapping[str, Any]] = None,
 ) -> None:
   """Self-contained function which adds a Tensorboard auxiliary job to @experiment."""
   provider = TensorboardProvider
-  [executable] = experiment.package([
-      xm.Packageable(
-          provider.get_tensorboard_packageable(timeout_secs=timeout_secs),
-          executor.Spec())
-  ])
+  [executable] = experiment.package(
+      [
+          xm.Packageable(
+              provider.get_tensorboard_packageable(timeout_secs=timeout_secs),
+              executor.Spec(),
+          )
+      ]
+  )
 
   job = xm.Job(
       executable,
       executor,
       args=provider.get_tensorboard_job_args(logdir, additional_args=args),
-      name='tensorboard')
+      name='tensorboard',
+  )
 
   # TODO: Add support for `termination_delay_secs`.
   experiment.add(xm.AuxiliaryUnitJob(job, termination_delay_secs=0))
```

### Comparing `xmanager-0.3.0/xmanager/contrib/tensorboard_test.py` & `xmanager-0.4.0/xmanager/contrib/tensorboard_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,75 +21,81 @@
 from xmanager import xm_local
 from xmanager.contrib import tensorboard
 
 
 class TensorboardTest(parameterized.TestCase):
 
   @parameterized.product(
-      executor=[xm_local.Vertex(),
-                xm_local.Kubernetes(),
-                xm_local.Local()],
+      executor=[xm_local.Vertex(), xm_local.Kubernetes(), xm_local.Local()],
       logdir=['logs'],
-      args=[{}, None, {
-          'new': 0
-      }])
-  def test_add_tensorboard_negative_timeout(self, executor: xm.Executor,
-                                            logdir: str, args: Mapping[str,
-                                                                       Any]):
+      args=[{}, None, {'new': 0}],
+  )
+  def test_add_tensorboard_negative_timeout(
+      self, executor: xm.Executor, logdir: str, args: Mapping[str, Any]
+  ):
     mock_experiment = absltest.mock.Mock()
     mock_experiment.add.return_value = None
     mock_executable = absltest.mock.Mock()
     mock_experiment.package.return_value = [mock_executable]
 
     with self.assertRaises(RuntimeError):
       tensorboard.add_tensorboard(
           mock_experiment,
           logdir=logdir,
           executor=executor,
           timeout_secs=-5,
-          args=args)
+          args=args,
+      )
 
   @parameterized.product(
-      executor=[xm_local.Vertex(),
-                xm_local.Kubernetes(),
-                xm_local.Local()],
+      executor=[xm_local.Vertex(), xm_local.Kubernetes(), xm_local.Local()],
       logdir=['logs'],
       timeout_secs=[0, 5],
-      args=[{}, None, {
-          'new': 0
-      }])
-  def test_add_tensorboard(self, executor: xm.Executor, logdir: str,
-                           timeout_secs: int, args: Mapping[str, Any]):
+      args=[{}, None, {'new': 0}],
+  )
+  def test_add_tensorboard(
+      self,
+      executor: xm.Executor,
+      logdir: str,
+      timeout_secs: int,
+      args: Mapping[str, Any],
+  ):
     mock_experiment = absltest.mock.Mock()
     mock_experiment.add.return_value = None
     mock_executable = absltest.mock.Mock()
     mock_experiment.package.return_value = [mock_executable]
 
     tensorboard.add_tensorboard(
         mock_experiment,
         logdir=logdir,
         executor=executor,
         timeout_secs=timeout_secs,
-        args=args)
+        args=args,
+    )
 
     expected_packageable_spec_arg = (
         tensorboard.TensorboardProvider.get_tensorboard_packageable(
-            timeout_secs=timeout_secs))
+            timeout_secs=timeout_secs
+        )
+    )
     mock_experiment.package.assert_called_once()
     packageable_arg = mock_experiment.package.call_args[0][0][0]
-    self.assertEqual(packageable_arg.executable_spec,
-                     expected_packageable_spec_arg)
+    self.assertEqual(
+        packageable_arg.executable_spec, expected_packageable_spec_arg
+    )
     self.assertEqual(packageable_arg.executor_spec, executor.Spec())
 
     expected_job = xm.Job(
         executable=mock_executable,
         executor=executor,
         args=tensorboard.TensorboardProvider.get_tensorboard_job_args(
-            logdir, additional_args=args),
-        name='tensorboard')
+            logdir, additional_args=args
+        ),
+        name='tensorboard',
+    )
     mock_experiment.add.assert_called_once()
     auxiliary_job_arg = mock_experiment.add.call_args[0][0]
     self.assertIsInstance(auxiliary_job_arg, xm.AuxiliaryUnitJob)
     self.assertEqual(auxiliary_job_arg._job, expected_job)
 
   def test_get_tensorboard_packageable_negative_timeout(self):
     provider = tensorboard.TensorboardProvider
@@ -97,35 +103,38 @@
       provider.get_tensorboard_packageable(timeout_secs=-5)
 
   @parameterized.product(timeout_secs=[0, 5])
   def test_get_tensorboard_packageable(self, timeout_secs: int):
     provider = tensorboard.TensorboardProvider
 
     packageable = provider.get_tensorboard_packageable(
-        timeout_secs=timeout_secs)
+        timeout_secs=timeout_secs
+    )
 
     self.assertIsInstance(packageable, xm.PythonContainer)
     self.assertEqual(packageable.base_image, 'tensorflow/tensorflow')
 
   @parameterized.product(
       log_dir=['logs'],
       port=[None, 6006, 2002],
-      additional_args=[{}, None, {
-          'logdir': 'logs_v2'
-      }, {
-          'new': 0
-      }])
-  def test_get_tensorboard_job_args(self, log_dir: str, port: int,
-                                    additional_args: Mapping[str, Any]):
+      additional_args=[{}, None, {'logdir': 'logs_v2'}, {'new': 0}],
+  )
+  def test_get_tensorboard_job_args(
+      self, log_dir: str, port: int, additional_args: Mapping[str, Any]
+  ):
     provider = tensorboard.TensorboardProvider
 
     args = provider.get_tensorboard_job_args(log_dir, port, additional_args)
     self.assertDictContainsSubset(
         dict(
             {
                 'logdir': log_dir,
                 'port': port or provider.DEFAULT_TENSORBOARD_PORT,
-            }, **(additional_args if additional_args else {})), args)
+            },
+            **(additional_args if additional_args else {}),
+        ),
+        args,
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/contrib/tpu.py` & `xmanager-0.4.0/xmanager/contrib/tpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 """Helper module for using TPUs."""
 from typing import List
 
 
 # pylint: disable=line-too-long
 def tpuvm_docker_instructions() -> List[str]:
   return [
-      'RUN wget '
-      'https://storage.googleapis.com/cloud-tpu-tpuvm-artifacts/libtpu/20210525/libtpu.so'
-      ' -O /lib/libtpu.so',
+      (
+          'RUN wget'
+          ' https://storage.googleapis.com/cloud-tpu-tpuvm-artifacts/libtpu/20210525/libtpu.so'
+          ' -O /lib/libtpu.so'
+      ),
       'RUN chmod 700 /lib/libtpu.so',
-      'RUN wget '
-      'https://storage.googleapis.com/cloud-tpu-tpuvm-artifacts/tensorflow/20210525/tf_nightly-2.6.0-cp38-cp38-linux_x86_64.whl',
+      (
+          'RUN wget '
+          'https://storage.googleapis.com/cloud-tpu-tpuvm-artifacts/tensorflow/20210525/tf_nightly-2.6.0-cp38-cp38-linux_x86_64.whl'
+      ),
       'RUN pip3 install tf_nightly-2.6.0-cp38-cp38-linux_x86_64.whl',
       'RUN rm tf_nightly-2.6.0-cp38-cp38-linux_x86_64.whl',
   ]
```

### Comparing `xmanager-0.3.0/xmanager/contrib/xm_tensorflow.py` & `xmanager-0.4.0/xmanager/contrib/xm_tensorflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,66 +43,67 @@
 
   experiment: xm.Experiment
   worker_executable: xm.Executable
   worker_executor: xm.Executor
   worker_name: str = 'worker'
   num_workers: int = 1
 
-  def create_job_group(self, work_unit: xm.WorkUnit,
-                       hparams: xm.UserArgs) -> xm.JobGroup:
+  def create_job_group(
+      self, work_unit: xm.WorkUnit, hparams: xm.UserArgs
+  ) -> xm.JobGroup:
     if isinstance(self.worker_executor, xm_local.Kubernetes):
       return self.create_kubernetes_job_group(work_unit, hparams)
 
     raise NotImplementedError(
         'MultiWorkerMirrored is not supported for executor_type '
-        f'`{type(self.worker_executor)}`')
+        f'`{type(self.worker_executor)}`'
+    )
 
   def gen_job_group(self) -> Callable[[xm.WorkUnit], Awaitable[None]]:
     """Create a generator that can be be used with experiment.add(generator)."""
 
-    async def _gen_job_group(work_unit: xm.WorkUnit,
-                             **hparams) -> Awaitable[None]:
+    async def _gen_job_group(
+        work_unit: xm.WorkUnit, **hparams
+    ) -> Awaitable[None]:
       job = self.create_job_group(work_unit, hparams)
       return work_unit.add(job)
 
     return _gen_job_group
 
-  def create_kubernetes_job_group(self, work_unit: xm.WorkUnit,
-                                  hparams: xm.UserArgs) -> xm.JobGroup:
+  def create_kubernetes_job_group(
+      self, work_unit: xm.WorkUnit, hparams: xm.UserArgs
+  ) -> xm.JobGroup:
     """Builds a Kubernetes job group that can be added to an experiment."""
     assert isinstance(self.worker_executor, xm_local.Kubernetes)
 
     worker_job_domains = {}
     for i in range(self.num_workers):
       job_name = f'{self.worker_name}-{i}'
 
       worker_job_domains[job_name] = addressing.k8s_pod_domain(
           job_name=job_name,
           experiment_id=self.experiment.experiment_id,
-          work_unit_id=work_unit.work_unit_id)
+          work_unit_id=work_unit.work_unit_id,
+      )
 
     jobs = {}
     for i, worker_job_name in enumerate(worker_job_domains):
       tf_config = {
-          'cluster': {
-              'worker': list(worker_job_domains.values())
-          },
-          'task': {
-              'type': 'worker',
-              'index': i
-          },
+          'cluster': {'worker': list(worker_job_domains.values())},
+          'task': {'type': 'worker', 'index': i},
       }
 
       jobs[worker_job_name] = xm.Job(
           executable=self.worker_executable,
           executor=self.worker_executor,
           args=hparams,
           env_vars={
               'TF_CONFIG': json.dumps(tf_config),
-          })
+          },
+      )
 
     return xm.JobGroup(**jobs)
 
 
 @attr.s(auto_attribs=True)
 class ParameterServerStrategyBuilder:
   """Builds a Tensorflow ParameterServer experiment in XManager.
@@ -124,96 +125,108 @@
   ps_executor: xm.Executor
   chief_name: str = 'chief'
   worker_name: str = 'worker'
   ps_name: str = 'ps'
   num_workers: int = 1
   num_ps: int = 1
 
-  def create_job_group(self, work_unit: xm.WorkUnit,
-                       hparams: xm.UserArgs) -> xm.JobGroup:
+  def create_job_group(
+      self, work_unit: xm.WorkUnit, hparams: xm.UserArgs
+  ) -> xm.JobGroup:
     if isinstance(self.worker_executor, xm_local.Kubernetes):
       return self.create_kubernetes_job_group(work_unit, hparams)
 
     raise NotImplementedError(
         'ParameterServerStrategy is not supported for executor_type '
-        f'`{type(self.worker_executor)}`')
+        f'`{type(self.worker_executor)}`'
+    )
 
   def gen_job_group(self) -> Callable[[xm.WorkUnit], Awaitable[None]]:
     """Create a generator that can be be used with experiment.add(generator)."""
 
-    async def _gen_job_group(work_unit: xm.WorkUnit,
-                             **hparams) -> Awaitable[None]:
+    async def _gen_job_group(
+        work_unit: xm.WorkUnit, **hparams
+    ) -> Awaitable[None]:
       job = self.create_job_group(work_unit, hparams)
       return work_unit.add(job)
 
     return _gen_job_group
 
-  def create_kubernetes_job_group(self, work_unit: xm.WorkUnit,
-                                  hparams: xm.UserArgs) -> xm.JobGroup:
+  def create_kubernetes_job_group(
+      self, work_unit: xm.WorkUnit, hparams: xm.UserArgs
+  ) -> xm.JobGroup:
     """Builds a Kubernetes job group that can be added to an experiment."""
     assert isinstance(self.chief_executor, xm_local.Kubernetes)
     assert isinstance(self.worker_executor, xm_local.Kubernetes)
     assert isinstance(self.ps_executor, xm_local.Kubernetes)
 
     def _k8s_pod_domain(job_name: str) -> str:
-      return addressing.k8s_pod_domain(job_name, self.experiment.experiment_id,
-                                       work_unit.work_unit_id)
+      return addressing.k8s_pod_domain(
+          job_name, self.experiment.experiment_id, work_unit.work_unit_id
+      )
 
     chief_domain = _k8s_pod_domain(self.chief_name)
     # pylint: disable=g-complex-comprehension
     worker_domains = [
-        addressing.k8s_pod_domain(f'{self.worker_name}-{i}',
-                                  self.experiment.experiment_id,
-                                  work_unit.work_unit_id)
+        addressing.k8s_pod_domain(
+            f'{self.worker_name}-{i}',
+            self.experiment.experiment_id,
+            work_unit.work_unit_id,
+        )
         for i in range(self.num_workers)
     ]
     ps_domains = [
-        addressing.k8s_pod_domain(f'{self.ps_name}-{i}',
-                                  self.experiment.experiment_id,
-                                  work_unit.work_unit_id)
+        addressing.k8s_pod_domain(
+            f'{self.ps_name}-{i}',
+            self.experiment.experiment_id,
+            work_unit.work_unit_id,
+        )
         for i in range(self.num_ps)
     ]
 
     # pylint: enable=g-complex-comprehension
 
     def _create_tf_config(task_type, task_index):
       return {
           'cluster': {
               'chief': [chief_domain],
               'worker': worker_domains,
-              'ps': ps_domains
+              'ps': ps_domains,
           },
           'task': {
               'type': task_type,
               'index': task_index,
-          }
+          },
       }
 
     jobs = {}
     jobs[self.chief_name] = xm.Job(
         executable=self.chief_executable,
         executor=self.chief_executor,
-        env_vars={'TF_CONFIG': json.dumps(_create_tf_config('chief', 0))})
+        env_vars={'TF_CONFIG': json.dumps(_create_tf_config('chief', 0))},
+    )
 
     for i in range(self.num_ps):
       ps_job_name = f'{self.ps_name}-{i}'
 
       jobs[ps_job_name] = xm.Job(
           executable=self.ps_executable,
           executor=self.ps_executor,
           args=hparams,
           env_vars={
               'TF_CONFIG': json.dumps(_create_tf_config('ps', i)),
-          })
+          },
+      )
 
     for i in range(self.num_workers):
       worker_job_name = f'{self.worker_name}-{i}'
 
       jobs[worker_job_name] = xm.Job(
           executable=self.worker_executable,
           executor=self.worker_executor,
           args=hparams,
           env_vars={
               'TF_CONFIG': json.dumps(_create_tf_config('worker', i)),
-          })
+          },
+      )
 
     return xm.JobGroup(**jobs)
```

### Comparing `xmanager-0.3.0/xmanager/contrib/xm_tensorflow_test.py` & `xmanager-0.4.0/xmanager/contrib/xm_tensorflow_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,63 +26,62 @@
 
 class XmTensorflowTest(parameterized.TestCase):
 
   @parameterized.product(num_workers=[0, 2, 4])
   def test_kubernetes_multiworker_strategy(self, num_workers):
     experiment = absltest.mock.MagicMock()
     type(experiment).experiment_id = absltest.mock.PropertyMock(
-        return_value=123)
+        return_value=123
+    )
     work_unit = absltest.mock.MagicMock()
     type(work_unit).work_unit_id = absltest.mock.PropertyMock(return_value=42)
     executable = absltest.mock.MagicMock()
     executor = absltest.mock.MagicMock(spec=xm_local.Kubernetes)
     hparams = xm.SequentialArgs.from_collection({'a': 'b'})
     worker_name = 'best_worker'
 
     builder = xm_tensorflow.MultiWorkerMirroredStrategyBuilder(
         experiment=experiment,
         worker_executable=executable,
         worker_executor=executor,
         num_workers=num_workers,
-        worker_name=worker_name)
+        worker_name=worker_name,
+    )
     job_group = builder.create_job_group(hparams=hparams, work_unit=work_unit)
 
     expected_job_names = [f'{worker_name}-{i}' for i in range(num_workers)]
     expected_worker_domains = [
         addressing.k8s_pod_domain(
-            job_name=job_name, experiment_id=123, work_unit_id=42)
+            job_name=job_name, experiment_id=123, work_unit_id=42
+        )
         for job_name in expected_job_names
     ]
 
     self.assertSameElements(expected_job_names, list(job_group.jobs.keys()))
 
     for i, job_name in enumerate(expected_job_names):
       self.assertIsInstance(job_group.jobs[job_name], xm.Job)
       job = cast(xm.Job, job_group.jobs[job_name])
 
       self.assertEqual(job.executable, executable)
       self.assertEqual(job.executor, executor)
       self.assertEqual(job.args, xm.SequentialArgs.from_collection(hparams))
 
       tf_config = {
-          'cluster': {
-              'worker': expected_worker_domains
-          },
-          'task': {
-              'type': 'worker',
-              'index': i
-          }
+          'cluster': {'worker': expected_worker_domains},
+          'task': {'type': 'worker', 'index': i},
       }
       self.assertEqual(job.env_vars, {'TF_CONFIG': json.dumps(tf_config)})
 
   @parameterized.product(num_workers=[0, 2], num_ps=[0, 2])
   def test_kubernetes_parameter_server_strategy(self, num_workers, num_ps):
     experiment = absltest.mock.MagicMock()
     type(experiment).experiment_id = absltest.mock.PropertyMock(
-        return_value=123)
+        return_value=123
+    )
     work_unit = absltest.mock.MagicMock()
     type(work_unit).work_unit_id = absltest.mock.PropertyMock(return_value=42)
 
     chief_executable = absltest.mock.MagicMock()
     chief_executor = absltest.mock.MagicMock(spec=xm_local.Kubernetes)
     worker_executable = absltest.mock.MagicMock()
     worker_executor = absltest.mock.MagicMock(spec=xm_local.Kubernetes)
@@ -102,26 +101,30 @@
         worker_executor,
         ps_executable,
         ps_executor,
         chief_name=chief_name,
         worker_name=worker_name,
         ps_name=ps_name,
         num_workers=num_workers,
-        num_ps=num_ps)
+        num_ps=num_ps,
+    )
     job_group = builder.create_job_group(work_unit=work_unit, hparams=hparams)
 
     expected_worker_job_names = [
         f'{worker_name}-{i}' for i in range(num_workers)
     ]
     expected_ps_job_names = [f'{ps_name}-{i}' for i in range(num_ps)]
-    self.assertSameElements([chief_name] + expected_worker_job_names +
-                            expected_ps_job_names, list(job_group.jobs.keys()))
+    self.assertSameElements(
+        [chief_name] + expected_worker_job_names + expected_ps_job_names,
+        list(job_group.jobs.keys()),
+    )
 
     expected_chief_domain = addressing.k8s_pod_domain(
-        chief_name, experiment_id=123, work_unit_id=42)
+        chief_name, experiment_id=123, work_unit_id=42
+    )
     expected_worker_domains = [
         addressing.k8s_pod_domain(worker_name, 123, 42)
         for worker_name in expected_worker_job_names
     ]
     expected_ps_domains = [
         addressing.k8s_pod_domain(ps_name, 123, 42)
         for ps_name in expected_ps_job_names
@@ -134,47 +137,50 @@
     job = cast(xm.Job, job_group.jobs[chief_name])
 
     def _create_expected_tf_config(task_type, task_index):
       return {
           'cluster': {
               'chief': [expected_chief_domain],
               'worker': expected_worker_domains,
-              'ps': expected_ps_domains
+              'ps': expected_ps_domains,
           },
           'task': {
               'type': task_type,
               'index': task_index,
-          }
+          },
       }
 
     self.assertEqual(job.executable, chief_executable)
     self.assertEqual(job.executor, chief_executor)
     self.assertEqual(
         job.env_vars,
-        {'TF_CONFIG': json.dumps(_create_expected_tf_config('chief', 0))})
+        {'TF_CONFIG': json.dumps(_create_expected_tf_config('chief', 0))},
+    )
 
     # Test workers
     for i in range(num_workers):
       worker_job_name = expected_worker_job_names[i]
       job = cast(xm.Job, job_group.jobs[worker_job_name])
 
       self.assertEqual(job.executable, worker_executable)
       self.assertEqual(job.executor, worker_executor)
       self.assertEqual(job.args, xm.SequentialArgs.from_collection(hparams))
       self.assertEqual(
           job.env_vars,
-          {'TF_CONFIG': json.dumps(_create_expected_tf_config('worker', i))})
+          {'TF_CONFIG': json.dumps(_create_expected_tf_config('worker', i))},
+      )
 
     # Test parameter servers
     for i in range(num_ps):
       ps_job_name = expected_ps_job_names[i]
       job = cast(xm.Job, job_group.jobs[ps_job_name])
 
       self.assertEqual(job.executable, ps_executable)
       self.assertEqual(job.executor, ps_executor)
       self.assertEqual(
           job.env_vars,
-          {'TF_CONFIG': json.dumps(_create_expected_tf_config('ps', i))})
+          {'TF_CONFIG': json.dumps(_create_expected_tf_config('ps', i))},
+      )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/docker/docker_adapter.py` & `xmanager-0.4.0/xmanager/docker/docker_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 import docker
 from docker import errors
 from docker import types
 from docker.models import containers
 from docker.utils import utils
 
 _USE_SUBPROCESS = flags.DEFINE_bool(
-    'xm_subprocess_docker_impl', False,
-    'Launch docker using `subprocess` command.')
+    'xm_subprocess_docker_impl',
+    False,
+    'Launch docker using `subprocess` command.',
+)
 
 Ports = Dict[Union[int, str], Union[None, int, Tuple[str, int], List[int]]]
 
 
 @functools.lru_cache()
 def instance() -> 'DockerAdapter':
   """Returns a thread-safe singleton adapter derived from the environment.
@@ -91,20 +93,28 @@
       ports: Ports,
       volumes: Dict[str, str],
       gpu_count: int,
       interactive: bool = False,
   ) -> Optional[containers.Container]:
     """Runs a given container image."""
     if _USE_SUBPROCESS.value or interactive:
-      return self.run_container_subprocess(image_id, args, env_vars, network,
-                                           ports, volumes, gpu_count,
-                                           interactive)
+      return self.run_container_subprocess(
+          image_id,
+          args,
+          env_vars,
+          network,
+          ports,
+          volumes,
+          gpu_count,
+          interactive,
+      )
     else:
-      return self.run_container_client(name, image_id, args, env_vars, network,
-                                       ports, volumes, gpu_count)
+      return self.run_container_client(
+          name, image_id, args, env_vars, network, ports, volumes, gpu_count
+      )
 
   def run_container_client(
       self,
       name: str,
       image_id: str,
       args: Sequence[str],
       env_vars: Mapping[str, str],
@@ -168,9 +178,13 @@
     return None
 
   def stop_container(self, container_id: str) -> None:
     try:
       self._client.containers.get(container_id).stop()
     except docker.errors.NotFound:
       logging.warning(
-          'Container %s could not be stopped as it was not found '
-          '(it may already have been stopped)', container_id)
+          (
+              'Container %s could not be stopped as it was not found '
+              '(it may already have been stopped)'
+          ),
+          container_id,
+      )
```

### Comparing `xmanager-0.3.0/xmanager/generated/failure_details_pb2.py` & `xmanager-0.4.0/xmanager/generated/failure_details_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,606 +13,30 @@
 # limitations under the License.
 
 # pyformat: disable
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # pylint: skip-file
 # source: src/main/protobuf/failure_details.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'src/main/protobuf/failure_details.proto\x12\x0f\x66\x61ilure_details\x1a google/protobuf/descriptor.proto\"*\n\x15\x46\x61ilureDetailMetadata\x12\x11\n\texit_code\x18\x01 \x01(\r\"\xaa\x1c\n\rFailureDetail\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x33\n\x0binterrupted\x18\x65 \x01(\x0b\x32\x1c.failure_details.InterruptedH\x00\x12\x42\n\x13\x65xternal_repository\x18g \x01(\x0b\x32#.failure_details.ExternalRepositoryH\x00\x12\x38\n\x0e\x62uild_progress\x18h \x01(\x0b\x32\x1e.failure_details.BuildProgressH\x00\x12\x38\n\x0eremote_options\x18j \x01(\x0b\x32\x1e.failure_details.RemoteOptionsH\x00\x12@\n\x12\x63lient_environment\x18k \x01(\x0b\x32\".failure_details.ClientEnvironmentH\x00\x12\'\n\x05\x63rash\x18l \x01(\x0b\x32\x16.failure_details.CrashH\x00\x12\x38\n\x0esymlink_forest\x18n \x01(\x0b\x32\x1e.failure_details.SymlinkForestH\x00\x12:\n\x0fpackage_options\x18r \x01(\x0b\x32\x1f.failure_details.PackageOptionsH\x00\x12<\n\x10remote_execution\x18s \x01(\x0b\x32 .failure_details.RemoteExecutionH\x00\x12/\n\texecution\x18t \x01(\x0b\x32\x1a.failure_details.ExecutionH\x00\x12\x31\n\nworkspaces\x18u \x01(\x0b\x32\x1b.failure_details.WorkspacesH\x00\x12\x36\n\rcrash_options\x18v \x01(\x0b\x32\x1d.failure_details.CrashOptionsH\x00\x12\x31\n\nfilesystem\x18w \x01(\x0b\x32\x1b.failure_details.FilesystemH\x00\x12>\n\x11\x65xecution_options\x18y \x01(\x0b\x32!.failure_details.ExecutionOptionsH\x00\x12+\n\x07\x63ommand\x18z \x01(\x0b\x32\x18.failure_details.CommandH\x00\x12\'\n\x05spawn\x18{ \x01(\x0b\x32\x16.failure_details.SpawnH\x00\x12\x32\n\x0bgrpc_server\x18| \x01(\x0b\x32\x1b.failure_details.GrpcServerH\x00\x12@\n\x12\x63\x61nonicalize_flags\x18} \x01(\x0b\x32\".failure_details.CanonicalizeFlagsH\x00\x12\x42\n\x13\x62uild_configuration\x18~ \x01(\x0b\x32#.failure_details.BuildConfigurationH\x00\x12\x34\n\x0cinfo_command\x18\x7f \x01(\x0b\x32\x1c.failure_details.InfoCommandH\x00\x12\x39\n\x0ememory_options\x18\x81\x01 \x01(\x0b\x32\x1e.failure_details.MemoryOptionsH\x00\x12(\n\x05query\x18\x82\x01 \x01(\x0b\x32\x16.failure_details.QueryH\x00\x12;\n\x0flocal_execution\x18\x84\x01 \x01(\x0b\x32\x1f.failure_details.LocalExecutionH\x00\x12\x35\n\x0c\x61\x63tion_cache\x18\x86\x01 \x01(\x0b\x32\x1c.failure_details.ActionCacheH\x00\x12\x37\n\rfetch_command\x18\x87\x01 \x01(\x0b\x32\x1d.failure_details.FetchCommandH\x00\x12\x35\n\x0csync_command\x18\x88\x01 \x01(\x0b\x32\x1c.failure_details.SyncCommandH\x00\x12,\n\x07sandbox\x18\x89\x01 \x01(\x0b\x32\x18.failure_details.SandboxH\x00\x12=\n\x10include_scanning\x18\x8b\x01 \x01(\x0b\x32 .failure_details.IncludeScanningH\x00\x12\x35\n\x0ctest_command\x18\x8c\x01 \x01(\x0b\x32\x1c.failure_details.TestCommandH\x00\x12\x35\n\x0c\x61\x63tion_query\x18\x8d\x01 \x01(\x0b\x32\x1c.failure_details.ActionQueryH\x00\x12;\n\x0ftarget_patterns\x18\x8e\x01 \x01(\x0b\x32\x1f.failure_details.TargetPatternsH\x00\x12\x37\n\rclean_command\x18\x90\x01 \x01(\x0b\x32\x1d.failure_details.CleanCommandH\x00\x12\x39\n\x0e\x63onfig_command\x18\x91\x01 \x01(\x0b\x32\x1e.failure_details.ConfigCommandH\x00\x12\x41\n\x12\x63onfigurable_query\x18\x92\x01 \x01(\x0b\x32\".failure_details.ConfigurableQueryH\x00\x12\x35\n\x0c\x64ump_command\x18\x93\x01 \x01(\x0b\x32\x1c.failure_details.DumpCommandH\x00\x12\x35\n\x0chelp_command\x18\x94\x01 \x01(\x0b\x32\x1c.failure_details.HelpCommandH\x00\x12\x39\n\x0emobile_install\x18\x96\x01 \x01(\x0b\x32\x1e.failure_details.MobileInstallH\x00\x12;\n\x0fprofile_command\x18\x97\x01 \x01(\x0b\x32\x1f.failure_details.ProfileCommandH\x00\x12\x33\n\x0brun_command\x18\x98\x01 \x01(\x0b\x32\x1b.failure_details.RunCommandH\x00\x12;\n\x0fversion_command\x18\x99\x01 \x01(\x0b\x32\x1f.failure_details.VersionCommandH\x00\x12\x44\n\x14print_action_command\x18\x9a\x01 \x01(\x0b\x32#.failure_details.PrintActionCommandH\x00\x12=\n\x10workspace_status\x18\x9e\x01 \x01(\x0b\x32 .failure_details.WorkspaceStatusH\x00\x12\x35\n\x0cjava_compile\x18\x9f\x01 \x01(\x0b\x32\x1c.failure_details.JavaCompileH\x00\x12=\n\x10\x61\x63tion_rewinding\x18\xa0\x01 \x01(\x0b\x32 .failure_details.ActionRewindingH\x00\x12\x33\n\x0b\x63pp_compile\x18\xa1\x01 \x01(\x0b\x32\x1b.failure_details.CppCompileH\x00\x12;\n\x0fstarlark_action\x18\xa2\x01 \x01(\x0b\x32\x1f.failure_details.StarlarkActionH\x00\x12\x35\n\x0cninja_action\x18\xa3\x01 \x01(\x0b\x32\x1c.failure_details.NinjaActionH\x00\x12?\n\x11\x64ynamic_execution\x18\xa4\x01 \x01(\x0b\x32!.failure_details.DynamicExecutionH\x00\x12\x33\n\x0b\x66\x61il_action\x18\xa6\x01 \x01(\x0b\x32\x1b.failure_details.FailActionH\x00\x12\x39\n\x0esymlink_action\x18\xa7\x01 \x01(\x0b\x32\x1e.failure_details.SymlinkActionH\x00\x12-\n\x08\x63pp_link\x18\xa8\x01 \x01(\x0b\x32\x18.failure_details.CppLinkH\x00\x12\x31\n\nlto_action\x18\xa9\x01 \x01(\x0b\x32\x1a.failure_details.LtoActionH\x00\x12\x33\n\x0btest_action\x18\xac\x01 \x01(\x0b\x32\x1b.failure_details.TestActionH\x00\x12*\n\x06worker\x18\xad\x01 \x01(\x0b\x32\x17.failure_details.WorkerH\x00\x12.\n\x08\x61nalysis\x18\xae\x01 \x01(\x0b\x32\x19.failure_details.AnalysisH\x00\x12;\n\x0fpackage_loading\x18\xaf\x01 \x01(\x0b\x32\x1f.failure_details.PackageLoadingH\x00\x12\x30\n\ttoolchain\x18\xb1\x01 \x01(\x0b\x32\x1a.failure_details.ToolchainH\x00\x12=\n\x10starlark_loading\x18\xb3\x01 \x01(\x0b\x32 .failure_details.StarlarkLoadingH\x00\x12\x37\n\rexternal_deps\x18\xb5\x01 \x01(\x0b\x32\x1d.failure_details.ExternalDepsH\x00\x12\x39\n\x0e\x64iff_awareness\x18\xb6\x01 \x01(\x0b\x32\x1e.failure_details.DiffAwarenessH\x00\x12=\n\x10modquery_command\x18\xb7\x01 \x01(\x0b\x32 .failure_details.ModqueryCommandH\x00\x42\n\n\x08\x63\x61tegoryJ\x04\x08\x02\x10\x65J\x04\x08\x66\x10gJ\x04\x08i\x10jJ\x04\x08m\x10nJ\x04\x08o\x10rJ\x04\x08x\x10yJ\x06\x08\x80\x01\x10\x81\x01J\x06\x08\x83\x01\x10\x84\x01J\x06\x08\x85\x01\x10\x86\x01J\x06\x08\x8a\x01\x10\x8b\x01J\x06\x08\x8f\x01\x10\x90\x01J\x06\x08\x95\x01\x10\x96\x01J\x06\x08\x9b\x01\x10\x9e\x01J\x06\x08\xa5\x01\x10\xa6\x01J\x06\x08\xaa\x01\x10\xac\x01J\x06\x08\xb0\x01\x10\xb1\x01J\x06\x08\xb2\x01\x10\xb3\x01J\x06\x08\xb4\x01\x10\xb5\x01\"\xa2\x05\n\x0bInterrupted\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.Interrupted.Code\"\xe1\x04\n\x04\x43ode\x12\x1e\n\x13INTERRUPTED_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08\x08\x12\x16\n\x0bINTERRUPTED\x10\x1c\x1a\x05\xb2\x43\x02\x08\x08\x12\x1b\n\x10\x44\x45PRECATED_BUILD\x10\x04\x1a\x05\xb2\x43\x02\x08\x08\x12&\n\x1b\x44\x45PRECATED_BUILD_COMPLETION\x10\x05\x1a\x05\xb2\x43\x02\x08\x08\x12*\n\x1f\x44\x45PRECATED_PACKAGE_LOADING_SYNC\x10\x06\x1a\x05\xb2\x43\x02\x08\x08\x12)\n\x1e\x44\x45PRECATED_EXECUTOR_COMPLETION\x10\x07\x1a\x05\xb2\x43\x02\x08\x08\x12&\n\x1b\x44\x45PRECATED_COMMAND_DISPATCH\x10\x08\x1a\x05\xb2\x43\x02\x08\x08\x12\x1f\n\x14\x44\x45PRECATED_INFO_ITEM\x10\t\x1a\x05\xb2\x43\x02\x08\x08\x12!\n\x16\x44\x45PRECATED_AFTER_QUERY\x10\n\x1a\x05\xb2\x43\x02\x08\x08\x12#\n\x18\x44\x45PRECATED_FETCH_COMMAND\x10\x11\x1a\x05\xb2\x43\x02\x08\x08\x12\"\n\x17\x44\x45PRECATED_SYNC_COMMAND\x10\x12\x1a\x05\xb2\x43\x02\x08\x08\x12#\n\x18\x44\x45PRECATED_CLEAN_COMMAND\x10\x14\x1a\x05\xb2\x43\x02\x08\x08\x12,\n!DEPRECATED_MOBILE_INSTALL_COMMAND\x10\x15\x1a\x05\xb2\x43\x02\x08\x08\x12\x1b\n\x10\x44\x45PRECATED_QUERY\x10\x16\x1a\x05\xb2\x43\x02\x08\x08\x12!\n\x16\x44\x45PRECATED_RUN_COMMAND\x10\x17\x1a\x05\xb2\x43\x02\x08\x08\x12%\n\x1a\x44\x45PRECATED_OPTIONS_PARSING\x10\x1b\x1a\x05\xb2\x43\x02\x08\x08\"\x04\x08\x01\x10\x03\"\x04\x08\x0b\x10\x10\"\x04\x08\x13\x10\x13\"\x04\x08\x18\x10\x1a\"\xa6\x04\n\x05Spawn\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Spawn.Code\x12\x14\n\x0c\x63\x61tastrophic\x18\x02 \x01(\x08\x12\x17\n\x0fspawn_exit_code\x18\x03 \x01(\x05\"\xc2\x03\n\x04\x43ode\x12\x18\n\rSPAWN_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNON_ZERO_EXIT\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x12\n\x07TIMEOUT\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rOUT_OF_MEMORY\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10\x45XECUTION_FAILED\x10\x04\x1a\x05\xb2\x43\x02\x08\"\x12\x1b\n\x10\x45XECUTION_DENIED\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13REMOTE_CACHE_FAILED\x10\x06\x1a\x05\xb2\x43\x02\x08\"\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x45XEC_IO_EXCEPTION\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0fINVALID_TIMEOUT\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#INVALID_REMOTE_EXECUTION_PROPERTIES\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NO_USABLE_STRATEGY_FOUND\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dUNSPECIFIED_EXECUTION_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\"\xd3\x01\n\x12\x45xternalRepository\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.ExternalRepository.Code\"\x84\x01\n\x04\x43ode\x12&\n\x1b\x45XTERNAL_REPOSITORY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x32\n\'OVERRIDE_DISALLOWED_MANAGED_DIRECTORIES\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x42\x41\x44_DOWNLOADER_CONFIG\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xa7\x06\n\rBuildProgress\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.BuildProgress.Code\"\xe2\x05\n\x04\x43ode\x12!\n\x16\x42UILD_PROGRESS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12 \n\x15OUTPUT_INITIALIZATION\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12.\n#BES_RUNS_PER_TEST_LIMIT_UNSUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x42\x45S_LOCAL_WRITE_ERROR\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18\x42\x45S_INITIALIZATION_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18\x42\x45S_UPLOAD_TIMEOUT_ERROR\x10\x07\x1a\x05\xb2\x43\x02\x08&\x12!\n\x16\x42\x45S_FILE_WRITE_TIMEOUT\x10\x08\x1a\x05\xb2\x43\x02\x08&\x12\"\n\x17\x42\x45S_FILE_WRITE_IO_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08&\x12%\n\x1a\x42\x45S_FILE_WRITE_INTERRUPTED\x10\n\x1a\x05\xb2\x43\x02\x08&\x12\"\n\x17\x42\x45S_FILE_WRITE_CANCELED\x10\x0b\x1a\x05\xb2\x43\x02\x08&\x12\'\n\x1c\x42\x45S_FILE_WRITE_UNKNOWN_ERROR\x10\x0c\x1a\x05\xb2\x43\x02\x08&\x12&\n\x1b\x42\x45S_UPLOAD_LOCAL_FILE_ERROR\x10\r\x1a\x05\xb2\x43\x02\x08&\x12*\n\x1f\x42\x45S_STREAM_NOT_RETRYING_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08-\x12\x37\n,BES_STREAM_COMPLETED_WITH_UNACK_EVENTS_ERROR\x10\x0f\x1a\x05\xb2\x43\x02\x08-\x12\x38\n-BES_STREAM_COMPLETED_WITH_UNSENT_EVENTS_ERROR\x10\x10\x1a\x05\xb2\x43\x02\x08-\x12\x31\n&BES_STREAM_COMPLETED_WITH_REMOTE_ERROR\x10\x13\x1a\x05\xb2\x43\x02\x08-\x12\x32\n\'BES_UPLOAD_RETRY_LIMIT_EXCEEDED_FAILURE\x10\x11\x1a\x05\xb2\x43\x02\x08&\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x04\x08\x12\x10\x12\"\xc3\x02\n\rRemoteOptions\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.RemoteOptions.Code\"\xfe\x01\n\x04\x43ode\x12!\n\x16REMOTE_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x35\n*REMOTE_DEFAULT_EXEC_PROPERTIES_LOGIC_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x43REDENTIALS_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19\x43REDENTIALS_WRITE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1d\x44OWNLOADER_WITHOUT_GRPC_CACHE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1c\x45XECUTION_WITH_INVALID_CACHE\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\"\x9a\x01\n\x11\x43lientEnvironment\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.ClientEnvironment.Code\"N\n\x04\x43ode\x12%\n\x1a\x43LIENT_ENVIRONMENT_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14\x43LIENT_CWD_MALFORMED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x96\x01\n\x05\x43rash\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Crash.Code\x12*\n\x06\x63\x61uses\x18\x02 \x03(\x0b\x32\x1a.failure_details.Throwable\"6\n\x04\x43ode\x12\x18\n\rCRASH_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x14\n\tCRASH_OOM\x10\x01\x1a\x05\xb2\x43\x02\x08!\"J\n\tThrowable\x12\x17\n\x0fthrowable_class\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x13\n\x0bstack_trace\x18\x03 \x03(\t\"\xe7\x01\n\rSymlinkForest\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.SymlinkForest.Code\"\xa2\x01\n\x04\x43ode\x12!\n\x16SYMLINK_FOREST_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%TOPLEVEL_OUTDIR_PACKAGE_PATH_CONFLICT\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eTOPLEVEL_OUTDIR_USED_AS_SOURCE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0f\x43REATION_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\"\x9d\x01\n\x0ePackageOptions\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.PackageOptions.Code\"W\n\x04\x43ode\x12\"\n\x17PACKAGE_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14PACKAGE_PATH_INVALID\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x02\x10\x02\"\x04\x08\x03\x10\x03\"\xb3\x06\n\x0fRemoteExecution\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.RemoteExecution.Code\"\xea\x05\n\x04\x43ode\x12#\n\x18REMOTE_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1a\x43\x41PABILITIES_QUERY_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\"\x12#\n\x18\x43REDENTIALS_INIT_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12\x43\x41\x43HE_INIT_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0fRPC_LOG_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19\x45XEC_CHANNEL_INIT_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1a\x43\x41\x43HE_CHANNEL_INIT_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1f\x44OWNLOADER_CHANNEL_INIT_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17LOG_DIR_CLEANUP_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x43LIENT_SERVER_INCOMPATIBLE\x10\t\x1a\x05\xb2\x43\x02\x08\"\x12-\n\"DOWNLOADED_INPUTS_DELETION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\"\x12@\n5REMOTE_DOWNLOAD_OUTPUTS_MINIMAL_WITHOUT_INMEMORY_DOTD\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x41\n6REMOTE_DOWNLOAD_OUTPUTS_MINIMAL_WITHOUT_INMEMORY_JDEPS\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\x12\x35\n*INCOMPLETE_OUTPUT_DOWNLOAD_CLEANUP_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12;\n0REMOTE_DEFAULT_PLATFORM_PROPERTIES_PARSE_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0eILLEGAL_OUTPUT\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12/\n$INVALID_EXEC_AND_PLATFORM_PROPERTIES\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\"\xd8\r\n\tExecution\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.Execution.Code\"\x9b\r\n\x04\x43ode\x12\x1c\n\x11\x45XECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12/\n$EXECUTION_LOG_INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12&\n\x1b\x45XECUTION_LOG_WRITE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19\x45XECROOT_CREATION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-TEMP_ACTION_OUTPUT_DIRECTORY_DELETION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-TEMP_ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12>\n3PERSISTENT_ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x31\n&LOCAL_OUTPUT_DIRECTORY_SYMLINK_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12+\n LOCAL_TEMPLATE_EXPANSION_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08$\x12-\n\"INPUT_DIRECTORY_CHECK_IO_EXCEPTION\x10\n\x1a\x05\xb2\x43\x02\x08$\x12/\n$EXTRA_ACTION_OUTPUT_CREATION_FAILURE\x10\x0b\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18TEST_RUNNER_IO_EXCEPTION\x10\x0c\x1a\x05\xb2\x43\x02\x08$\x12\"\n\x17\x46ILE_WRITE_IO_EXCEPTION\x10\r\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19TEST_OUT_ERR_IO_EXCEPTION\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_MANIFEST_COPY_IO_EXCEPTION\x10\x0f\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_MANIFEST_LINK_IO_EXCEPTION\x10\x10\x1a\x05\xb2\x43\x02\x08$\x12-\n\"SYMLINK_TREE_CREATION_IO_EXCEPTION\x10\x11\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_CREATION_COMMAND_EXCEPTION\x10\x12\x1a\x05\xb2\x43\x02\x08$\x12)\n\x1e\x41\x43TION_INPUT_READ_IO_EXCEPTION\x10\x13\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15\x41\x43TION_NOT_UP_TO_DATE\x10\x14\x1a\x05\xb2\x43\x02\x08\x01\x12-\n\"PSEUDO_ACTION_EXECUTION_PROHIBITED\x10\x15\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x44ISCOVERED_INPUT_DOES_NOT_EXIST\x10\x16\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1f\x41\x43TION_OUTPUTS_DELETION_FAILURE\x10\x17\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x41\x43TION_OUTPUTS_NOT_CREATED\x10\x18\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x41\x43TION_FINALIZATION_FAILURE\x10\x19\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x41\x43TION_INPUT_LOST\x10\x1a\x1a\x05\xb2\x43\x02\x08\x01\x12,\n!FILESYSTEM_CONTEXT_UPDATE_FAILURE\x10\x1b\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x41\x43TION_OUTPUT_CLOSE_FAILURE\x10\x1c\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cINPUT_DISCOVERY_IO_EXCEPTION\x10\x1d\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(TREE_ARTIFACT_DIRECTORY_CREATION_FAILURE\x10\x1e\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x1f\x1a\x05\xb2\x43\x02\x08\x01\x12\x36\n+ACTION_FS_OUTPUT_DIRECTORY_CREATION_FAILURE\x10 \x1a\x05\xb2\x43\x02\x08\x01\x12\x37\n,ACTION_FS_OUT_ERR_DIRECTORY_CREATION_FAILURE\x10!\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cNON_ACTION_EXECUTION_FAILURE\x10\"\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10#\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14SOURCE_INPUT_MISSING\x10$\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14UNEXPECTED_EXCEPTION\x10%\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19SOURCE_INPUT_IO_EXCEPTION\x10\'\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x08\x10\x08\"\x04\x08&\x10&\"\xc4\x02\n\nWorkspaces\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.Workspaces.Code\"\x85\x02\n\x04\x43ode\x12\x1d\n\x12WORKSPACES_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%WORKSPACES_LOG_INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cWORKSPACES_LOG_WRITE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12\x42\n7ILLEGAL_WORKSPACE_FILE_SYMLINK_WITH_MANAGED_DIRECTORIES\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12?\n4WORKSPACE_FILE_READ_FAILURE_WITH_MANAGED_DIRECTORIES\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\"p\n\x0c\x43rashOptions\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.CrashOptions.Code\".\n\x04\x43ode\x12 \n\x15\x43RASH_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\"\x04\x08\x01\x10\x01\"\xb2\x02\n\nFilesystem\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.Filesystem.Code\"\xf3\x01\n\x04\x43ode\x12\x1d\n\x12\x46ILESYSTEM_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%EMBEDDED_BINARIES_ENUMERATION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12+\n SERVER_PID_TXT_FILE_READ_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19SERVER_FILE_WRITE_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x35\n*DEFAULT_DIGEST_HASH_FUNCTION_INVALID_VALUE\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x04\x08\x07\x10\x07\"\xea\x03\n\x10\x45xecutionOptions\x12\x34\n\x04\x63ode\x18\x01 \x01(\x0e\x32&.failure_details.ExecutionOptions.Code\"\x9f\x03\n\x04\x43ode\x12$\n\x19\x45XECUTION_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10INVALID_STRATEGY\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12:\n/REQUESTED_STRATEGY_INCOMPATIBLE_WITH_SANDBOXING\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1f\x44\x45PRECATED_LOCAL_RESOURCES_USED\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1fINVALID_CYCLIC_DYNAMIC_STRATEGY\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'RESTRICTION_UNMATCHED_TO_ACTION_CONTEXT\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+REMOTE_FALLBACK_STRATEGY_NOT_ABSTRACT_SPAWN\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12STRATEGY_NOT_FOUND\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1e\x44YNAMIC_STRATEGY_NOT_SANDBOXED\x10\n\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x96\x05\n\x07\x43ommand\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.Command.Code\"\xdd\x04\n\x04\x43ode\x12\"\n\x17\x43OMMAND_FAILURE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1c\n\x11\x43OMMAND_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17\x41NOTHER_COMMAND_RUNNING\x10\x02\x1a\x05\xb2\x43\x02\x08\t\x12\x1e\n\x13PREVIOUSLY_SHUTDOWN\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12;\n0STARLARK_CPU_PROFILE_FILE_INITIALIZATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-STARLARK_CPU_PROFILING_INITIALIZATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'STARLARK_CPU_PROFILE_FILE_WRITE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1fINVOCATION_POLICY_PARSE_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19INVOCATION_POLICY_INVALID\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15OPTIONS_PARSE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eSTARLARK_OPTIONS_PARSE_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x41RGUMENTS_NOT_RECOGNIZED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10NOT_IN_WORKSPACE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18SPACES_IN_WORKSPACE_PATH\x10\r\x1a\x05\xb2\x43\x02\x08$\x12\x1e\n\x13IN_OUTPUT_DIRECTORY\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\"\xec\x01\n\nGrpcServer\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.GrpcServer.Code\"\xad\x01\n\x04\x43ode\x12\x1e\n\x13GRPC_SERVER_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12&\n\x1bGRPC_SERVER_NOT_COMPILED_IN\x10\x01\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13SERVER_BIND_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x15\n\nBAD_COOKIE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15NO_CLIENT_DESCRIPTION\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\x04\x08\x05\x10\x05\"\x99\x01\n\x11\x43\x61nonicalizeFlags\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.CanonicalizeFlags.Code\"M\n\x04\x43ode\x12%\n\x1a\x43\x41NONICALIZE_FLAGS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13\x46OR_COMMAND_INVALID\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\xc2\x04\n\x12\x42uildConfiguration\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.BuildConfiguration.Code\"\xf3\x03\n\x04\x43ode\x12&\n\x1b\x42UILD_CONFIGURATION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12.\n#PLATFORM_MAPPING_EVALUATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12.\n#PLATFORM_MAPPINGS_FILE_IS_DIRECTORY\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12+\n PLATFORM_MAPPINGS_FILE_NOT_FOUND\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(TOP_LEVEL_CONFIGURATION_CREATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15INVALID_CONFIGURATION\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15INVALID_BUILD_OPTIONS\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16MULTI_CPU_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\x33\n(HEURISTIC_INSTRUMENTATION_FILTER_INVALID\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x10\n\x05\x43YCLE\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1a\x43ONFLICTING_CONFIGURATIONS\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12,\n!INVALID_OUTPUT_DIRECTORY_MNEMONIC\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\"\xe9\x01\n\x0bInfoCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.InfoCommand.Code\"\xa8\x01\n\x04\x43ode\x12\x1f\n\x14INFO_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rTOO_MANY_KEYS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12KEY_NOT_RECOGNIZED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18INFO_BLOCK_WRITE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12!\n\x16\x41LL_INFO_WRITE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\xf6\x01\n\rMemoryOptions\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.MemoryOptions.Code\"\xb1\x01\n\x04\x43ode\x12!\n\x16MEMORY_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12@\n5EXPERIMENTAL_OOM_MORE_EAGERLY_THRESHOLD_INVALID_VALUE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x44\n9EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xf2\x0b\n\x05Query\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Query.Code\"\xbd\x0b\n\x04\x43ode\x12\x18\n\rQUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x32\n\'QUERY_FILE_WITH_COMMAND_LINE_EXPRESSION\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17QUERY_FILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15OUTPUT_FORMAT_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16GRAPHLESS_PREREQ_UNMET\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aQUERY_OUTPUT_WRITE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aQUERY_STDOUT_FLUSH_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12&\n\x1b\x41NALYSIS_QUERY_PREREQ_UNMET\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\x12&\n\x1bQUERY_RESULTS_FLUSH_FAILURE\x10\x0f\x1a\x05\xb2\x43\x02\x08$\x12\x39\n.DEPRECATED_UNCLOSED_QUOTATION_EXPRESSION_ERROR\x10\x10\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15VARIABLE_NAME_INVALID\x10\x11\x1a\x05\xb2\x43\x02\x08\x07\x12\x1d\n\x12VARIABLE_UNDEFINED\x10\x12\x1a\x05\xb2\x43\x02\x08\x07\x12\x44\n9BUILDFILES_AND_LOADFILES_CANNOT_USE_OUTPUT_LOCATION_ERROR\x10\x13\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10\x42UILD_FILE_ERROR\x10\x14\x1a\x05\xb2\x43\x02\x08\x07\x12\x10\n\x05\x43YCLE\x10\x15\x1a\x05\xb2\x43\x02\x08\x07\x12+\n UNIQUE_SKYKEY_THRESHOLD_EXCEEDED\x10\x16\x1a\x05\xb2\x43\x02\x08\x07\x12\'\n\x1cTARGET_NOT_IN_UNIVERSE_SCOPE\x10\x17\x1a\x05\xb2\x43\x02\x08\x02\x12+\n INVALID_FULL_UNIVERSE_EXPRESSION\x10\x18\x1a\x05\xb2\x43\x02\x08\x07\x12(\n\x1dUNIVERSE_SCOPE_LIMIT_EXCEEDED\x10\x19\x1a\x05\xb2\x43\x02\x08\x07\x12&\n\x1bINVALIDATION_LIMIT_EXCEEDED\x10\x1a\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1aOUTPUT_FORMAT_PREREQ_UNMET\x10\x1b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x41RGUMENTS_MISSING\x10\x1c\x1a\x05\xb2\x43\x02\x08\x07\x12\x31\n&RBUILDFILES_FUNCTION_REQUIRES_SKYQUERY\x10\x1d\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1a\x46ULL_TARGETS_NOT_SUPPORTED\x10\x1e\x1a\x05\xb2\x43\x02\x08\x07\x12,\n!DEPRECATED_UNEXPECTED_TOKEN_ERROR\x10\x1f\x1a\x05\xb2\x43\x02\x08\x02\x12-\n\"DEPRECATED_INTEGER_LITERAL_MISSING\x10 \x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+DEPRECATED_INVALID_STARTING_CHARACTER_ERROR\x10!\x1a\x05\xb2\x43\x02\x08\x02\x12\x32\n\'DEPRECATED_PREMATURE_END_OF_INPUT_ERROR\x10\"\x1a\x05\xb2\x43\x02\x08\x02\x12\x17\n\x0cSYNTAX_ERROR\x10#\x1a\x05\xb2\x43\x02\x08\x02\x12(\n\x1dOUTPUT_FORMATTER_IO_EXCEPTION\x10$\x1a\x05\xb2\x43\x02\x08$\x12+\n SKYQUERY_TRANSITIVE_TARGET_ERROR\x10%\x1a\x05\xb2\x43\x02\x08\x07\x12$\n\x19SKYQUERY_TARGET_EXCEPTION\x10&\x1a\x05\xb2\x43\x02\x08\x07\x12&\n\x1bINVALID_LABEL_IN_TEST_SUITE\x10\'\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18ILLEGAL_FLAG_COMBINATION\x10(\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12NON_DETAILED_ERROR\x10)\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x07\x10\x0c\"\x99\x01\n\x0eLocalExecution\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.LocalExecution.Code\"S\n\x04\x43ode\x12\"\n\x17LOCAL_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\'\n\x1cLOCKFREE_OUTPUT_PREREQ_UNMET\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x8a\x01\n\x0b\x41\x63tionCache\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.ActionCache.Code\"J\n\x04\x43ode\x12\x1f\n\x14\x41\x43TION_CACHE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12!\n\x16INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\"\xe7\x01\n\x0c\x46\x65tchCommand\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.FetchCommand.Code\"\xa4\x01\n\x04\x43ode\x12 \n\x15\x46\x45TCH_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1d\n\x12\x45XPRESSION_MISSING\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0fOPTIONS_INVALID\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11QUERY_PARSE_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16QUERY_EVALUATION_ERROR\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\"\xf8\x01\n\x0bSyncCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.SyncCommand.Code\"\xb7\x01\n\x04\x43ode\x12\x1f\n\x14SYNC_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14PACKAGE_LOOKUP_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1aWORKSPACE_EVALUATION_ERROR\x10\x02\x1a\x05\xb2\x43\x02\x08\x07\x12\"\n\x17REPOSITORY_FETCH_ERRORS\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12\"\n\x17REPOSITORY_NAME_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x07\"\xfb\x03\n\x07Sandbox\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.Sandbox.Code\"\xc2\x03\n\x04\x43ode\x12\"\n\x17SANDBOX_FAILURE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12!\n\x16INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12!\n\x16\x45XECUTION_IO_EXCEPTION\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12!\n\x16\x44OCKER_COMMAND_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fNO_DOCKER_IMAGE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12+\n DOCKER_IMAGE_PREPARATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x42IND_MOUNT_ANALYSIS_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bMOUNT_SOURCE_DOES_NOT_EXIST\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12,\n!MOUNT_SOURCE_TARGET_TYPE_MISMATCH\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bMOUNT_TARGET_DOES_NOT_EXIST\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17SUBPROCESS_START_FAILED\x10\n\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\"\x9d\x04\n\x0fIncludeScanning\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.IncludeScanning.Code\x12\x42\n\x14package_loading_code\x18\x02 \x01(\x0e\x32$.failure_details.PackageLoading.Code\"\x90\x03\n\x04\x43ode\x12#\n\x18INCLUDE_SCANNING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1eINITIALIZE_INCLUDE_HINTS_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15SCANNING_IO_EXCEPTION\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12,\n!INCLUDE_HINTS_FILE_NOT_IN_PACKAGE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aINCLUDE_HINTS_READ_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15ILLEGAL_ABSOLUTE_PATH\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_LOAD_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19USER_PACKAGE_LOAD_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bSYSTEM_PACKAGE_LOAD_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12\x30\n%UNDIFFERENTIATED_PACKAGE_LOAD_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\"\xbc\x01\n\x0bTestCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.TestCommand.Code\"|\n\x04\x43ode\x12\x1f\n\x14TEST_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1a\n\x0fNO_TEST_TARGETS\x10\x01\x1a\x05\xb2\x43\x02\x08\x04\x12\x1e\n\x13TEST_WITH_NOANALYZE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x17\n\x0cTESTS_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x03\"\xa6\x05\n\x0b\x41\x63tionQuery\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.ActionQuery.Code\"\xe5\x04\n\x04\x43ode\x12\x1f\n\x14\x41\x43TION_QUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x19\n\x0eOUTPUT_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x06\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x45XPRESSION_PARSE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+SKYFRAME_STATE_WITH_COMMAND_LINE_EXPRESSION\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19INVALID_AQUERY_EXPRESSION\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bSKYFRAME_STATE_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x41QUERY_OUTPUT_TOO_BIG\x10\x08\x1a\x05\xb2\x43\x02\x08\x07\x12!\n\x16ILLEGAL_PATTERN_SYNTAX\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13INCORRECT_ARGUMENTS\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12>\n3TOP_LEVEL_TARGETS_WITH_SKYFRAME_STATE_NOT_SUPPORTED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eSKYFRAME_STATE_AFTER_EXECUTION\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dLABELS_FUNCTION_NOT_SUPPORTED\x10\r\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aTEMPLATE_EXPANSION_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\"\xd7\x06\n\x0eTargetPatterns\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.TargetPatterns.Code\"\x90\x06\n\x04\x43ode\x12\"\n\x17TARGET_PATTERNS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x38\n-TARGET_PATTERN_FILE_WITH_COMMAND_LINE_PATTERN\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12+\n TARGET_PATTERN_FILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cTARGET_PATTERN_PARSE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11PACKAGE_NOT_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15TARGET_FORMAT_INVALID\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x41\x42SOLUTE_TARGET_PATTERN_INVALID\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%CANNOT_DETERMINE_TARGET_FROM_FILENAME\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12LABEL_SYNTAX_ERROR\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dTARGET_CANNOT_BE_EMPTY_STRING\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12+\n PACKAGE_PART_CANNOT_END_IN_SLASH\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15\x43\x41NNOT_PRELOAD_TARGET\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fTARGETS_MISSING\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%RECURSIVE_TARGET_PATTERNS_NOT_ALLOWED\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1fUP_LEVEL_REFERENCES_NOT_ALLOWED\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#NEGATIVE_TARGET_PATTERN_NOT_ALLOWED\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15TARGET_MUST_BE_A_FILE\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x44\x45PENDENCY_NOT_FOUND\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_NAME_INVALID\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\"\xf5\x03\n\x0c\x43leanCommand\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.CleanCommand.Code\"\xb2\x03\n\x04\x43ode\x12 \n\x15\x43LEAN_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\'\n\x1cOUTPUT_SERVICE_CLEAN_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x06\x12%\n\x1a\x41\x43TION_CACHE_CLEAN_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15OUT_ERR_CLOSE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aOUTPUT_BASE_DELETE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1dOUTPUT_BASE_TEMP_MOVE_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12+\n ASYNC_OUTPUT_BASE_DELETE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x06\x12\"\n\x17\x45XECROOT_DELETE_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x45XECROOT_TEMP_MOVE_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1d\x41SYNC_EXECROOT_DELETE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x06\x12#\n\x18\x41RGUMENTS_NOT_RECOGNIZED\x10\n\x1a\x05\xb2\x43\x02\x08\x02\"\xb1\x01\n\rConfigCommand\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.ConfigCommand.Code\"m\n\x04\x43ode\x12!\n\x16\x43ONFIG_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13TOO_MANY_CONFIG_IDS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17\x43ONFIGURATION_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xbb\x04\n\x11\x43onfigurableQuery\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.ConfigurableQuery.Code\"\xee\x03\n\x04\x43ode\x12%\n\x1a\x43ONFIGURABLE_QUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x45XPRESSION_PARSE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x46ILTERS_NOT_SUPPORTED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12,\n!BUILDFILES_FUNCTION_NOT_SUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1fSIBLINGS_FUNCTION_NOT_SUPPORTED\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eVISIBLE_FUNCTION_NOT_SUPPORTED\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x41TTRIBUTE_MISSING\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1fINCORRECT_CONFIG_ARGUMENT_ERROR\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x19\n\x0eTARGET_MISSING\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15STARLARK_SYNTAX_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13STARLARK_EVAL_ERROR\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x46ORMAT_FUNCTION_ERROR\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\"\xa9\x02\n\x0b\x44umpCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.DumpCommand.Code\"\xe8\x01\n\x04\x43ode\x12\x1f\n\x14\x44UMP_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13NO_OUTPUT_SPECIFIED\x10\x01\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18\x41\x43TION_CACHE_DUMP_FAILED\x10\x02\x1a\x05\xb2\x43\x02\x08\x07\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18\x41\x43TION_GRAPH_DUMP_FAILED\x10\x04\x1a\x05\xb2\x43\x02\x08\x07\x12$\n\x19STARLARK_HEAP_DUMP_FAILED\x10\x05\x1a\x05\xb2\x43\x02\x08\x08\"\x04\x08\x06\x10\x06\"\xa2\x01\n\x0bHelpCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.HelpCommand.Code\"b\n\x04\x43ode\x12\x1f\n\x14HELP_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MISSING_ARGUMENT\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x43OMMAND_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xb1\x02\n\rMobileInstall\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.MobileInstall.Code\"\xec\x01\n\x04\x43ode\x12!\n\x16MOBILE_INSTALL_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13\x43LASSIC_UNSUPPORTED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13NO_TARGET_SPECIFIED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aMULTIPLE_TARGETS_SPECIFIED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13TARGET_TYPE_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x06\x12\x18\n\rNON_ZERO_EXIT\x10\x05\x1a\x05\xb2\x43\x02\x08\x06\x12 \n\x15\x45RROR_RUNNING_PROGRAM\x10\x06\x1a\x05\xb2\x43\x02\x08\x06\"\xb8\x01\n\x0eProfileCommand\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.ProfileCommand.Code\"r\n\x04\x43ode\x12\"\n\x17PROFILE_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12(\n\x1dOLD_BINARY_FORMAT_UNSUPPORTED\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x46ILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xc6\x05\n\nRunCommand\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.RunCommand.Code\"\x87\x05\n\x04\x43ode\x12\x1e\n\x13RUN_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13NO_TARGET_SPECIFIED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aTOO_MANY_TARGETS_SPECIFIED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15TARGET_NOT_EXECUTABLE\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12/\n$TARGET_BUILT_BUT_PATH_NOT_EXECUTABLE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x32\n\'TARGET_BUILT_BUT_PATH_VALIDATION_FAILED\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aRUN_UNDER_TARGET_NOT_BUILT\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10RUN_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cTOO_MANY_TEST_SHARDS_OR_RUNS\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eTEST_ENVIRONMENT_SETUP_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08$\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08$\x12\x1d\n\x12NO_SHELL_SPECIFIED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1f\n\x14SCRIPT_WRITE_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x06\x12\x30\n%RUNFILES_DIRECTORIES_CREATION_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12-\n\"RUNFILES_SYMLINKS_CREATION_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12-\n\"TEST_ENVIRONMENT_SETUP_INTERRUPTED\x10\x0f\x1a\x05\xb2\x43\x02\x08\x08\"\x8a\x01\n\x0eVersionCommand\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.VersionCommand.Code\"D\n\x04\x43ode\x12\"\n\x17VERSION_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNOT_AVAILABLE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x88\x02\n\x12PrintActionCommand\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.PrintActionCommand.Code\"\xb9\x01\n\x04\x43ode\x12\'\n\x1cPRINT_ACTION_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10TARGET_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17TARGET_KIND_UNSUPPORTED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x41\x43TIONS_NOT_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\"\xc8\x02\n\x0fWorkspaceStatus\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.WorkspaceStatus.Code\"\xff\x01\n\x04\x43ode\x12#\n\x18WORKSPACE_STATUS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNON_ZERO_EXIT\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x41\x42NORMAL_TERMINATION\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0b\x45XEC_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rPARSE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x1d\n\x12VALIDATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x43ONTENT_UPDATE_IO_EXCEPTION\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13STDERR_IO_EXCEPTION\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\"\x94\x02\n\x0bJavaCompile\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.JavaCompile.Code\"\xd3\x01\n\x04\x43ode\x12\x1f\n\x14JAVA_COMPILE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19REDUCED_CLASSPATH_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17JDEPS_READ_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12\x35\n*REDUCED_CLASSPATH_FALLBACK_CLEANUP_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\xba\x01\n\x0f\x41\x63tionRewinding\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.ActionRewinding.Code\"r\n\x04\x43ode\x12#\n\x18\x41\x43TION_REWINDING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19LOST_INPUT_TOO_MANY_TIMES\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14LOST_INPUT_IS_SOURCE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\x8d\x04\n\nCppCompile\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.CppCompile.Code\"\xce\x03\n\x04\x43ode\x12\x1e\n\x13\x43PP_COMPILE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1e\x46IND_USED_HEADERS_IO_EXCEPTION\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\x1f\n\x14\x43OPY_OUT_ERR_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12\x1e\n\x13\x44_FILE_READ_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x43OMMAND_GENERATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18MODULE_EXPANSION_TIMEOUT\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eINCLUDE_PATH_OUTSIDE_EXEC_ROOT\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x46\x41KE_COMMAND_GENERATION_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15UNDECLARED_INCLUSIONS\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x44_FILE_PARSE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x43OVERAGE_NOTES_CREATION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dMODULE_EXPANSION_MISSING_DATA\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\"\xc9\x01\n\x0eStarlarkAction\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.StarlarkAction.Code\"\x82\x01\n\x04\x43ode\x12\"\n\x17STARLARK_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1eUNUSED_INPUT_LIST_READ_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12+\n UNUSED_INPUT_LIST_FILE_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xb8\x01\n\x0bNinjaAction\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.NinjaAction.Code\"x\n\x04\x43ode\x12\x1f\n\x14NINJA_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12.\n#INVALID_DEPFILE_DECLARED_DEPENDENCY\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\x1f\n\x14\x44_FILE_PARSE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\"\xff\x01\n\x10\x44ynamicExecution\x12\x34\n\x04\x63ode\x18\x01 \x01(\x0e\x32&.failure_details.DynamicExecution.Code\"\xb4\x01\n\x04\x43ode\x12$\n\x19\x44YNAMIC_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1aXCODE_RELATED_PREREQ_UNMET\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\"\n\x17\x41\x43TION_LOG_MOVE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bRUN_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NO_USABLE_STRATEGY_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\"\x92\x03\n\nFailAction\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.FailAction.Code\"\xd3\x02\n\x04\x43ode\x12\x1e\n\x13\x46\x41IL_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13INTENTIONAL_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18INCORRECT_PYTHON_VERSION\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16PROGUARD_SPECS_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1d\x44YNAMIC_LINKING_NOT_SUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14SOURCE_FILES_MISSING\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13INCORRECT_TOOLCHAIN\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16\x46RAGMENT_CLASS_MISSING\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43\x41NT_BUILD_INCOMPATIBLE_TARGET\x10\n\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x08\x10\x08\"\x04\x08\t\x10\t\"\xb3\x02\n\rSymlinkAction\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.SymlinkAction.Code\"\xee\x01\n\x04\x43ode\x12!\n\x16SYMLINK_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19\x45XECUTABLE_INPUT_NOT_FILE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17\x45XECUTABLE_INPUT_IS_NOT\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#EXECUTABLE_INPUT_CHECK_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aLINK_CREATION_IO_EXCEPTION\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17LINK_TOUCH_IO_EXCEPTION\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\"\xae\x01\n\x07\x43ppLink\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.CppLink.Code\"v\n\x04\x43ode\x12\x1b\n\x10\x43PP_LINK_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1a\x43OMMAND_GENERATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x46\x41KE_COMMAND_GENERATION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xd7\x01\n\tLtoAction\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.LtoAction.Code\"\x9a\x01\n\x04\x43ode\x12\x1d\n\x12LTO_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12+\n INVALID_ABSOLUTE_PATH_IN_IMPORTS\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15MISSING_BITCODE_FILES\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19IMPORTS_READ_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\"\x96\x02\n\nTestAction\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.TestAction.Code\"\xd7\x01\n\x04\x43ode\x12\x1e\n\x13TEST_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1aNO_KEEP_GOING_TEST_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17LOCAL_TEST_PREREQ_UNMET\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x44UPLICATE_CPU_TAGS\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fINVALID_CPU_TAG\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\"\xf1\x03\n\x06Worker\x12*\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1c.failure_details.Worker.Code\"\xba\x03\n\x04\x43ode\x12\x19\n\x0eWORKER_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12/\n$MULTIPLEXER_INSTANCE_REMOVAL_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aMULTIPLEXER_DOES_NOT_EXIST\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x13\n\x08NO_TOOLS\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bNO_FLAGFILE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%VIRTUAL_INPUT_MATERIALIZATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x42ORROW_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10PREFETCH_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0fPREPARE_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fREQUEST_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16PARSE_RESPONSE_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bNO_RESPONSE\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x46INISH_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\"\x8e\x06\n\x08\x41nalysis\x12,\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1e.failure_details.Analysis.Code\"\xd3\x05\n\x04\x43ode\x12\x1b\n\x10\x41NALYSIS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x17\n\x0cLOAD_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dGENERIC_LOADING_PHASE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NOT_ALL_TARGETS_ANALYZED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x31\n&PARAMETERIZED_TOP_LEVEL_ASPECT_INVALID\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19\x41SPECT_LABEL_SYNTAX_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13\x41SPECT_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10\x41SPECT_NOT_FOUND\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x41\x43TION_CONFLICT\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x41RTIFACT_PREFIX_CONFLICT\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dUNEXPECTED_ANALYSIS_EXCEPTION\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cTARGETS_MISSING_ENVIRONMENTS\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13INVALID_ENVIRONMENT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x45NVIRONMENT_MISSING_FROM_GROUPS\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x45XEC_GROUP_MISSING\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aINVALID_EXECUTION_PLATFORM\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16\x41SPECT_CREATION_FAILED\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12+\n CONFIGURED_VALUE_CREATION_FAILED\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dINCOMPATIBLE_TARGET_REQUESTED\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\"\xb8\t\n\x0ePackageLoading\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.PackageLoading.Code\"\xf1\x08\n\x04\x43ode\x12\"\n\x17PACKAGE_LOADING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14WORKSPACE_FILE_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eMAX_COMPUTATION_STEPS_EXCEEDED\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x42UILD_FILE_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12REPOSITORY_MISSING\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(PERSISTENT_INCONSISTENT_FILESYSTEM_ERROR\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'TRANSIENT_INCONSISTENT_FILESYSTEM_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x17\n\x0cINVALID_NAME\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x45VAL_GLOBS_SYMLINK_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aIMPORT_STARLARK_FILE_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fPACKAGE_MISSING\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0eTARGET_MISSING\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rNO_SUCH_THING\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11GLOB_IO_EXCEPTION\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0f\x44UPLICATE_LABEL\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dINVALID_PACKAGE_SPECIFICATION\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12\x17\n\x0cSYNTAX_ERROR\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12+\n ENVIRONMENT_IN_DIFFERENT_PACKAGE\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x44\x45\x46\x41ULT_ENVIRONMENT_UNDECLARED\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x45NVIRONMENT_IN_MULTIPLE_GROUPS\x10\x14\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x45NVIRONMENT_DOES_NOT_EXIST\x10\x15\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13\x45NVIRONMENT_INVALID\x10\x16\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x45NVIRONMENT_NOT_IN_GROUP\x10\x17\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_NAME_INVALID\x10\x18\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13STARLARK_EVAL_ERROR\x10\x19\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15LICENSE_PARSE_FAILURE\x10\x1a\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x44ISTRIBUTIONS_PARSE_FAILURE\x10\x1b\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eLABEL_CROSSES_PACKAGE_BOUNDARY\x10\x1c\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x42UILTINS_INJECTION_FAILURE\x10\x1d\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#SYMLINK_CYCLE_OR_INFINITE_EXPANSION\x10\x1e\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12OTHER_IO_EXCEPTION\x10\x1f\x1a\x05\xb2\x43\x02\x08$\"\x04\x08\x08\x10\x08\"\xd4\x02\n\tToolchain\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.Toolchain.Code\"\x97\x02\n\x04\x43ode\x12\x1c\n\x11TOOLCHAIN_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MISSING_PROVIDER\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18INVALID_CONSTRAINT_VALUE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16INVALID_PLATFORM_VALUE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11INVALID_TOOLCHAIN\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eNO_MATCHING_EXECUTION_PLATFORM\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15NO_MATCHING_TOOLCHAIN\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16INVALID_TOOLCHAIN_TYPE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\"\x8e\x03\n\x0fStarlarkLoading\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.StarlarkLoading.Code\"\xc5\x02\n\x04\x43ode\x12#\n\x18STARLARK_LOADING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x10\n\x05\x43YCLE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rCOMPILE_ERROR\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bPARSE_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x15\n\nEVAL_ERROR\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1c\x43ONTAINING_PACKAGE_NOT_FOUND\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11PACKAGE_NOT_FOUND\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x13\n\x08IO_ERROR\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eLABEL_CROSSES_PACKAGE_BOUNDARY\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x42UILTINS_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10VISIBILITY_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x01\"\x8a\x02\n\x0c\x45xternalDeps\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.ExternalDeps.Code\"\xc7\x01\n\x04\x43ode\x12 \n\x15\x45XTERNAL_DEPS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MODULE_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x30\x12\x15\n\nBAD_MODULE\x10\x02\x1a\x05\xb2\x43\x02\x08\x30\x12#\n\x18VERSION_RESOLUTION_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x30\x12\x1f\n\x14INVALID_REGISTRY_URL\x10\x04\x1a\x05\xb2\x43\x02\x08\x30\x12#\n\x18\x45RROR_ACCESSING_REGISTRY\x10\x05\x1a\x05\xb2\x43\x02\x08 \"\x8a\x01\n\rDiffAwareness\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.DiffAwareness.Code\"F\n\x04\x43ode\x12!\n\x16\x44IFF_AWARENESS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10\x44IFF_STAT_FAILED\x10\x01\x1a\x05\xb2\x43\x02\x08$\"\xcf\x01\n\x0fModqueryCommand\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.ModqueryCommand.Code\"\x86\x01\n\x04\x43ode\x12#\n\x18MODQUERY_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1c\n\x11MISSING_ARGUMENTS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12TOO_MANY_ARGUMENTS\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11INVALID_ARGUMENTS\x10\x03\x1a\x05\xb2\x43\x02\x08\x02:\\\n\x08metadata\x12!.google.protobuf.EnumValueOptions\x18\xb6\x08 \x01(\x0b\x32&.failure_details.FailureDetailMetadataB&\n$com.google.devtools.build.lib.serverb\x06proto3')
-
-
-METADATA_FIELD_NUMBER = 1078
-metadata = DESCRIPTOR.extensions_by_name['metadata']
-
-_FAILUREDETAILMETADATA = DESCRIPTOR.message_types_by_name['FailureDetailMetadata']
-_FAILUREDETAIL = DESCRIPTOR.message_types_by_name['FailureDetail']
-_INTERRUPTED = DESCRIPTOR.message_types_by_name['Interrupted']
-_SPAWN = DESCRIPTOR.message_types_by_name['Spawn']
-_EXTERNALREPOSITORY = DESCRIPTOR.message_types_by_name['ExternalRepository']
-_BUILDPROGRESS = DESCRIPTOR.message_types_by_name['BuildProgress']
-_REMOTEOPTIONS = DESCRIPTOR.message_types_by_name['RemoteOptions']
-_CLIENTENVIRONMENT = DESCRIPTOR.message_types_by_name['ClientEnvironment']
-_CRASH = DESCRIPTOR.message_types_by_name['Crash']
-_THROWABLE = DESCRIPTOR.message_types_by_name['Throwable']
-_SYMLINKFOREST = DESCRIPTOR.message_types_by_name['SymlinkForest']
-_PACKAGEOPTIONS = DESCRIPTOR.message_types_by_name['PackageOptions']
-_REMOTEEXECUTION = DESCRIPTOR.message_types_by_name['RemoteExecution']
-_EXECUTION = DESCRIPTOR.message_types_by_name['Execution']
-_WORKSPACES = DESCRIPTOR.message_types_by_name['Workspaces']
-_CRASHOPTIONS = DESCRIPTOR.message_types_by_name['CrashOptions']
-_FILESYSTEM = DESCRIPTOR.message_types_by_name['Filesystem']
-_EXECUTIONOPTIONS = DESCRIPTOR.message_types_by_name['ExecutionOptions']
-_COMMAND = DESCRIPTOR.message_types_by_name['Command']
-_GRPCSERVER = DESCRIPTOR.message_types_by_name['GrpcServer']
-_CANONICALIZEFLAGS = DESCRIPTOR.message_types_by_name['CanonicalizeFlags']
-_BUILDCONFIGURATION = DESCRIPTOR.message_types_by_name['BuildConfiguration']
-_INFOCOMMAND = DESCRIPTOR.message_types_by_name['InfoCommand']
-_MEMORYOPTIONS = DESCRIPTOR.message_types_by_name['MemoryOptions']
-_QUERY = DESCRIPTOR.message_types_by_name['Query']
-_LOCALEXECUTION = DESCRIPTOR.message_types_by_name['LocalExecution']
-_ACTIONCACHE = DESCRIPTOR.message_types_by_name['ActionCache']
-_FETCHCOMMAND = DESCRIPTOR.message_types_by_name['FetchCommand']
-_SYNCCOMMAND = DESCRIPTOR.message_types_by_name['SyncCommand']
-_SANDBOX = DESCRIPTOR.message_types_by_name['Sandbox']
-_INCLUDESCANNING = DESCRIPTOR.message_types_by_name['IncludeScanning']
-_TESTCOMMAND = DESCRIPTOR.message_types_by_name['TestCommand']
-_ACTIONQUERY = DESCRIPTOR.message_types_by_name['ActionQuery']
-_TARGETPATTERNS = DESCRIPTOR.message_types_by_name['TargetPatterns']
-_CLEANCOMMAND = DESCRIPTOR.message_types_by_name['CleanCommand']
-_CONFIGCOMMAND = DESCRIPTOR.message_types_by_name['ConfigCommand']
-_CONFIGURABLEQUERY = DESCRIPTOR.message_types_by_name['ConfigurableQuery']
-_DUMPCOMMAND = DESCRIPTOR.message_types_by_name['DumpCommand']
-_HELPCOMMAND = DESCRIPTOR.message_types_by_name['HelpCommand']
-_MOBILEINSTALL = DESCRIPTOR.message_types_by_name['MobileInstall']
-_PROFILECOMMAND = DESCRIPTOR.message_types_by_name['ProfileCommand']
-_RUNCOMMAND = DESCRIPTOR.message_types_by_name['RunCommand']
-_VERSIONCOMMAND = DESCRIPTOR.message_types_by_name['VersionCommand']
-_PRINTACTIONCOMMAND = DESCRIPTOR.message_types_by_name['PrintActionCommand']
-_WORKSPACESTATUS = DESCRIPTOR.message_types_by_name['WorkspaceStatus']
-_JAVACOMPILE = DESCRIPTOR.message_types_by_name['JavaCompile']
-_ACTIONREWINDING = DESCRIPTOR.message_types_by_name['ActionRewinding']
-_CPPCOMPILE = DESCRIPTOR.message_types_by_name['CppCompile']
-_STARLARKACTION = DESCRIPTOR.message_types_by_name['StarlarkAction']
-_NINJAACTION = DESCRIPTOR.message_types_by_name['NinjaAction']
-_DYNAMICEXECUTION = DESCRIPTOR.message_types_by_name['DynamicExecution']
-_FAILACTION = DESCRIPTOR.message_types_by_name['FailAction']
-_SYMLINKACTION = DESCRIPTOR.message_types_by_name['SymlinkAction']
-_CPPLINK = DESCRIPTOR.message_types_by_name['CppLink']
-_LTOACTION = DESCRIPTOR.message_types_by_name['LtoAction']
-_TESTACTION = DESCRIPTOR.message_types_by_name['TestAction']
-_WORKER = DESCRIPTOR.message_types_by_name['Worker']
-_ANALYSIS = DESCRIPTOR.message_types_by_name['Analysis']
-_PACKAGELOADING = DESCRIPTOR.message_types_by_name['PackageLoading']
-_TOOLCHAIN = DESCRIPTOR.message_types_by_name['Toolchain']
-_STARLARKLOADING = DESCRIPTOR.message_types_by_name['StarlarkLoading']
-_EXTERNALDEPS = DESCRIPTOR.message_types_by_name['ExternalDeps']
-_DIFFAWARENESS = DESCRIPTOR.message_types_by_name['DiffAwareness']
-_MODQUERYCOMMAND = DESCRIPTOR.message_types_by_name['ModqueryCommand']
-_INTERRUPTED_CODE = _INTERRUPTED.enum_types_by_name['Code']
-_SPAWN_CODE = _SPAWN.enum_types_by_name['Code']
-_EXTERNALREPOSITORY_CODE = _EXTERNALREPOSITORY.enum_types_by_name['Code']
-_BUILDPROGRESS_CODE = _BUILDPROGRESS.enum_types_by_name['Code']
-_REMOTEOPTIONS_CODE = _REMOTEOPTIONS.enum_types_by_name['Code']
-_CLIENTENVIRONMENT_CODE = _CLIENTENVIRONMENT.enum_types_by_name['Code']
-_CRASH_CODE = _CRASH.enum_types_by_name['Code']
-_SYMLINKFOREST_CODE = _SYMLINKFOREST.enum_types_by_name['Code']
-_PACKAGEOPTIONS_CODE = _PACKAGEOPTIONS.enum_types_by_name['Code']
-_REMOTEEXECUTION_CODE = _REMOTEEXECUTION.enum_types_by_name['Code']
-_EXECUTION_CODE = _EXECUTION.enum_types_by_name['Code']
-_WORKSPACES_CODE = _WORKSPACES.enum_types_by_name['Code']
-_CRASHOPTIONS_CODE = _CRASHOPTIONS.enum_types_by_name['Code']
-_FILESYSTEM_CODE = _FILESYSTEM.enum_types_by_name['Code']
-_EXECUTIONOPTIONS_CODE = _EXECUTIONOPTIONS.enum_types_by_name['Code']
-_COMMAND_CODE = _COMMAND.enum_types_by_name['Code']
-_GRPCSERVER_CODE = _GRPCSERVER.enum_types_by_name['Code']
-_CANONICALIZEFLAGS_CODE = _CANONICALIZEFLAGS.enum_types_by_name['Code']
-_BUILDCONFIGURATION_CODE = _BUILDCONFIGURATION.enum_types_by_name['Code']
-_INFOCOMMAND_CODE = _INFOCOMMAND.enum_types_by_name['Code']
-_MEMORYOPTIONS_CODE = _MEMORYOPTIONS.enum_types_by_name['Code']
-_QUERY_CODE = _QUERY.enum_types_by_name['Code']
-_LOCALEXECUTION_CODE = _LOCALEXECUTION.enum_types_by_name['Code']
-_ACTIONCACHE_CODE = _ACTIONCACHE.enum_types_by_name['Code']
-_FETCHCOMMAND_CODE = _FETCHCOMMAND.enum_types_by_name['Code']
-_SYNCCOMMAND_CODE = _SYNCCOMMAND.enum_types_by_name['Code']
-_SANDBOX_CODE = _SANDBOX.enum_types_by_name['Code']
-_INCLUDESCANNING_CODE = _INCLUDESCANNING.enum_types_by_name['Code']
-_TESTCOMMAND_CODE = _TESTCOMMAND.enum_types_by_name['Code']
-_ACTIONQUERY_CODE = _ACTIONQUERY.enum_types_by_name['Code']
-_TARGETPATTERNS_CODE = _TARGETPATTERNS.enum_types_by_name['Code']
-_CLEANCOMMAND_CODE = _CLEANCOMMAND.enum_types_by_name['Code']
-_CONFIGCOMMAND_CODE = _CONFIGCOMMAND.enum_types_by_name['Code']
-_CONFIGURABLEQUERY_CODE = _CONFIGURABLEQUERY.enum_types_by_name['Code']
-_DUMPCOMMAND_CODE = _DUMPCOMMAND.enum_types_by_name['Code']
-_HELPCOMMAND_CODE = _HELPCOMMAND.enum_types_by_name['Code']
-_MOBILEINSTALL_CODE = _MOBILEINSTALL.enum_types_by_name['Code']
-_PROFILECOMMAND_CODE = _PROFILECOMMAND.enum_types_by_name['Code']
-_RUNCOMMAND_CODE = _RUNCOMMAND.enum_types_by_name['Code']
-_VERSIONCOMMAND_CODE = _VERSIONCOMMAND.enum_types_by_name['Code']
-_PRINTACTIONCOMMAND_CODE = _PRINTACTIONCOMMAND.enum_types_by_name['Code']
-_WORKSPACESTATUS_CODE = _WORKSPACESTATUS.enum_types_by_name['Code']
-_JAVACOMPILE_CODE = _JAVACOMPILE.enum_types_by_name['Code']
-_ACTIONREWINDING_CODE = _ACTIONREWINDING.enum_types_by_name['Code']
-_CPPCOMPILE_CODE = _CPPCOMPILE.enum_types_by_name['Code']
-_STARLARKACTION_CODE = _STARLARKACTION.enum_types_by_name['Code']
-_NINJAACTION_CODE = _NINJAACTION.enum_types_by_name['Code']
-_DYNAMICEXECUTION_CODE = _DYNAMICEXECUTION.enum_types_by_name['Code']
-_FAILACTION_CODE = _FAILACTION.enum_types_by_name['Code']
-_SYMLINKACTION_CODE = _SYMLINKACTION.enum_types_by_name['Code']
-_CPPLINK_CODE = _CPPLINK.enum_types_by_name['Code']
-_LTOACTION_CODE = _LTOACTION.enum_types_by_name['Code']
-_TESTACTION_CODE = _TESTACTION.enum_types_by_name['Code']
-_WORKER_CODE = _WORKER.enum_types_by_name['Code']
-_ANALYSIS_CODE = _ANALYSIS.enum_types_by_name['Code']
-_PACKAGELOADING_CODE = _PACKAGELOADING.enum_types_by_name['Code']
-_TOOLCHAIN_CODE = _TOOLCHAIN.enum_types_by_name['Code']
-_STARLARKLOADING_CODE = _STARLARKLOADING.enum_types_by_name['Code']
-_EXTERNALDEPS_CODE = _EXTERNALDEPS.enum_types_by_name['Code']
-_DIFFAWARENESS_CODE = _DIFFAWARENESS.enum_types_by_name['Code']
-_MODQUERYCOMMAND_CODE = _MODQUERYCOMMAND.enum_types_by_name['Code']
-FailureDetailMetadata = _reflection.GeneratedProtocolMessageType('FailureDetailMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _FAILUREDETAILMETADATA,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.FailureDetailMetadata)
-  })
-_sym_db.RegisterMessage(FailureDetailMetadata)
-
-FailureDetail = _reflection.GeneratedProtocolMessageType('FailureDetail', (_message.Message,), {
-  'DESCRIPTOR' : _FAILUREDETAIL,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.FailureDetail)
-  })
-_sym_db.RegisterMessage(FailureDetail)
-
-Interrupted = _reflection.GeneratedProtocolMessageType('Interrupted', (_message.Message,), {
-  'DESCRIPTOR' : _INTERRUPTED,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Interrupted)
-  })
-_sym_db.RegisterMessage(Interrupted)
-
-Spawn = _reflection.GeneratedProtocolMessageType('Spawn', (_message.Message,), {
-  'DESCRIPTOR' : _SPAWN,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Spawn)
-  })
-_sym_db.RegisterMessage(Spawn)
-
-ExternalRepository = _reflection.GeneratedProtocolMessageType('ExternalRepository', (_message.Message,), {
-  'DESCRIPTOR' : _EXTERNALREPOSITORY,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ExternalRepository)
-  })
-_sym_db.RegisterMessage(ExternalRepository)
-
-BuildProgress = _reflection.GeneratedProtocolMessageType('BuildProgress', (_message.Message,), {
-  'DESCRIPTOR' : _BUILDPROGRESS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.BuildProgress)
-  })
-_sym_db.RegisterMessage(BuildProgress)
-
-RemoteOptions = _reflection.GeneratedProtocolMessageType('RemoteOptions', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTEOPTIONS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.RemoteOptions)
-  })
-_sym_db.RegisterMessage(RemoteOptions)
-
-ClientEnvironment = _reflection.GeneratedProtocolMessageType('ClientEnvironment', (_message.Message,), {
-  'DESCRIPTOR' : _CLIENTENVIRONMENT,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ClientEnvironment)
-  })
-_sym_db.RegisterMessage(ClientEnvironment)
-
-Crash = _reflection.GeneratedProtocolMessageType('Crash', (_message.Message,), {
-  'DESCRIPTOR' : _CRASH,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Crash)
-  })
-_sym_db.RegisterMessage(Crash)
-
-Throwable = _reflection.GeneratedProtocolMessageType('Throwable', (_message.Message,), {
-  'DESCRIPTOR' : _THROWABLE,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Throwable)
-  })
-_sym_db.RegisterMessage(Throwable)
-
-SymlinkForest = _reflection.GeneratedProtocolMessageType('SymlinkForest', (_message.Message,), {
-  'DESCRIPTOR' : _SYMLINKFOREST,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.SymlinkForest)
-  })
-_sym_db.RegisterMessage(SymlinkForest)
-
-PackageOptions = _reflection.GeneratedProtocolMessageType('PackageOptions', (_message.Message,), {
-  'DESCRIPTOR' : _PACKAGEOPTIONS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.PackageOptions)
-  })
-_sym_db.RegisterMessage(PackageOptions)
-
-RemoteExecution = _reflection.GeneratedProtocolMessageType('RemoteExecution', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTEEXECUTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.RemoteExecution)
-  })
-_sym_db.RegisterMessage(RemoteExecution)
-
-Execution = _reflection.GeneratedProtocolMessageType('Execution', (_message.Message,), {
-  'DESCRIPTOR' : _EXECUTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Execution)
-  })
-_sym_db.RegisterMessage(Execution)
-
-Workspaces = _reflection.GeneratedProtocolMessageType('Workspaces', (_message.Message,), {
-  'DESCRIPTOR' : _WORKSPACES,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Workspaces)
-  })
-_sym_db.RegisterMessage(Workspaces)
-
-CrashOptions = _reflection.GeneratedProtocolMessageType('CrashOptions', (_message.Message,), {
-  'DESCRIPTOR' : _CRASHOPTIONS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.CrashOptions)
-  })
-_sym_db.RegisterMessage(CrashOptions)
-
-Filesystem = _reflection.GeneratedProtocolMessageType('Filesystem', (_message.Message,), {
-  'DESCRIPTOR' : _FILESYSTEM,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Filesystem)
-  })
-_sym_db.RegisterMessage(Filesystem)
-
-ExecutionOptions = _reflection.GeneratedProtocolMessageType('ExecutionOptions', (_message.Message,), {
-  'DESCRIPTOR' : _EXECUTIONOPTIONS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ExecutionOptions)
-  })
-_sym_db.RegisterMessage(ExecutionOptions)
-
-Command = _reflection.GeneratedProtocolMessageType('Command', (_message.Message,), {
-  'DESCRIPTOR' : _COMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Command)
-  })
-_sym_db.RegisterMessage(Command)
-
-GrpcServer = _reflection.GeneratedProtocolMessageType('GrpcServer', (_message.Message,), {
-  'DESCRIPTOR' : _GRPCSERVER,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.GrpcServer)
-  })
-_sym_db.RegisterMessage(GrpcServer)
-
-CanonicalizeFlags = _reflection.GeneratedProtocolMessageType('CanonicalizeFlags', (_message.Message,), {
-  'DESCRIPTOR' : _CANONICALIZEFLAGS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.CanonicalizeFlags)
-  })
-_sym_db.RegisterMessage(CanonicalizeFlags)
-
-BuildConfiguration = _reflection.GeneratedProtocolMessageType('BuildConfiguration', (_message.Message,), {
-  'DESCRIPTOR' : _BUILDCONFIGURATION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.BuildConfiguration)
-  })
-_sym_db.RegisterMessage(BuildConfiguration)
-
-InfoCommand = _reflection.GeneratedProtocolMessageType('InfoCommand', (_message.Message,), {
-  'DESCRIPTOR' : _INFOCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.InfoCommand)
-  })
-_sym_db.RegisterMessage(InfoCommand)
-
-MemoryOptions = _reflection.GeneratedProtocolMessageType('MemoryOptions', (_message.Message,), {
-  'DESCRIPTOR' : _MEMORYOPTIONS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.MemoryOptions)
-  })
-_sym_db.RegisterMessage(MemoryOptions)
-
-Query = _reflection.GeneratedProtocolMessageType('Query', (_message.Message,), {
-  'DESCRIPTOR' : _QUERY,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Query)
-  })
-_sym_db.RegisterMessage(Query)
-
-LocalExecution = _reflection.GeneratedProtocolMessageType('LocalExecution', (_message.Message,), {
-  'DESCRIPTOR' : _LOCALEXECUTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.LocalExecution)
-  })
-_sym_db.RegisterMessage(LocalExecution)
-
-ActionCache = _reflection.GeneratedProtocolMessageType('ActionCache', (_message.Message,), {
-  'DESCRIPTOR' : _ACTIONCACHE,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ActionCache)
-  })
-_sym_db.RegisterMessage(ActionCache)
-
-FetchCommand = _reflection.GeneratedProtocolMessageType('FetchCommand', (_message.Message,), {
-  'DESCRIPTOR' : _FETCHCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.FetchCommand)
-  })
-_sym_db.RegisterMessage(FetchCommand)
-
-SyncCommand = _reflection.GeneratedProtocolMessageType('SyncCommand', (_message.Message,), {
-  'DESCRIPTOR' : _SYNCCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.SyncCommand)
-  })
-_sym_db.RegisterMessage(SyncCommand)
-
-Sandbox = _reflection.GeneratedProtocolMessageType('Sandbox', (_message.Message,), {
-  'DESCRIPTOR' : _SANDBOX,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Sandbox)
-  })
-_sym_db.RegisterMessage(Sandbox)
-
-IncludeScanning = _reflection.GeneratedProtocolMessageType('IncludeScanning', (_message.Message,), {
-  'DESCRIPTOR' : _INCLUDESCANNING,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.IncludeScanning)
-  })
-_sym_db.RegisterMessage(IncludeScanning)
-
-TestCommand = _reflection.GeneratedProtocolMessageType('TestCommand', (_message.Message,), {
-  'DESCRIPTOR' : _TESTCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.TestCommand)
-  })
-_sym_db.RegisterMessage(TestCommand)
-
-ActionQuery = _reflection.GeneratedProtocolMessageType('ActionQuery', (_message.Message,), {
-  'DESCRIPTOR' : _ACTIONQUERY,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ActionQuery)
-  })
-_sym_db.RegisterMessage(ActionQuery)
-
-TargetPatterns = _reflection.GeneratedProtocolMessageType('TargetPatterns', (_message.Message,), {
-  'DESCRIPTOR' : _TARGETPATTERNS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.TargetPatterns)
-  })
-_sym_db.RegisterMessage(TargetPatterns)
-
-CleanCommand = _reflection.GeneratedProtocolMessageType('CleanCommand', (_message.Message,), {
-  'DESCRIPTOR' : _CLEANCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.CleanCommand)
-  })
-_sym_db.RegisterMessage(CleanCommand)
-
-ConfigCommand = _reflection.GeneratedProtocolMessageType('ConfigCommand', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ConfigCommand)
-  })
-_sym_db.RegisterMessage(ConfigCommand)
-
-ConfigurableQuery = _reflection.GeneratedProtocolMessageType('ConfigurableQuery', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGURABLEQUERY,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ConfigurableQuery)
-  })
-_sym_db.RegisterMessage(ConfigurableQuery)
-
-DumpCommand = _reflection.GeneratedProtocolMessageType('DumpCommand', (_message.Message,), {
-  'DESCRIPTOR' : _DUMPCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.DumpCommand)
-  })
-_sym_db.RegisterMessage(DumpCommand)
-
-HelpCommand = _reflection.GeneratedProtocolMessageType('HelpCommand', (_message.Message,), {
-  'DESCRIPTOR' : _HELPCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.HelpCommand)
-  })
-_sym_db.RegisterMessage(HelpCommand)
-
-MobileInstall = _reflection.GeneratedProtocolMessageType('MobileInstall', (_message.Message,), {
-  'DESCRIPTOR' : _MOBILEINSTALL,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.MobileInstall)
-  })
-_sym_db.RegisterMessage(MobileInstall)
-
-ProfileCommand = _reflection.GeneratedProtocolMessageType('ProfileCommand', (_message.Message,), {
-  'DESCRIPTOR' : _PROFILECOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ProfileCommand)
-  })
-_sym_db.RegisterMessage(ProfileCommand)
-
-RunCommand = _reflection.GeneratedProtocolMessageType('RunCommand', (_message.Message,), {
-  'DESCRIPTOR' : _RUNCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.RunCommand)
-  })
-_sym_db.RegisterMessage(RunCommand)
-
-VersionCommand = _reflection.GeneratedProtocolMessageType('VersionCommand', (_message.Message,), {
-  'DESCRIPTOR' : _VERSIONCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.VersionCommand)
-  })
-_sym_db.RegisterMessage(VersionCommand)
-
-PrintActionCommand = _reflection.GeneratedProtocolMessageType('PrintActionCommand', (_message.Message,), {
-  'DESCRIPTOR' : _PRINTACTIONCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.PrintActionCommand)
-  })
-_sym_db.RegisterMessage(PrintActionCommand)
-
-WorkspaceStatus = _reflection.GeneratedProtocolMessageType('WorkspaceStatus', (_message.Message,), {
-  'DESCRIPTOR' : _WORKSPACESTATUS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.WorkspaceStatus)
-  })
-_sym_db.RegisterMessage(WorkspaceStatus)
-
-JavaCompile = _reflection.GeneratedProtocolMessageType('JavaCompile', (_message.Message,), {
-  'DESCRIPTOR' : _JAVACOMPILE,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.JavaCompile)
-  })
-_sym_db.RegisterMessage(JavaCompile)
-
-ActionRewinding = _reflection.GeneratedProtocolMessageType('ActionRewinding', (_message.Message,), {
-  'DESCRIPTOR' : _ACTIONREWINDING,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ActionRewinding)
-  })
-_sym_db.RegisterMessage(ActionRewinding)
-
-CppCompile = _reflection.GeneratedProtocolMessageType('CppCompile', (_message.Message,), {
-  'DESCRIPTOR' : _CPPCOMPILE,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.CppCompile)
-  })
-_sym_db.RegisterMessage(CppCompile)
-
-StarlarkAction = _reflection.GeneratedProtocolMessageType('StarlarkAction', (_message.Message,), {
-  'DESCRIPTOR' : _STARLARKACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.StarlarkAction)
-  })
-_sym_db.RegisterMessage(StarlarkAction)
-
-NinjaAction = _reflection.GeneratedProtocolMessageType('NinjaAction', (_message.Message,), {
-  'DESCRIPTOR' : _NINJAACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.NinjaAction)
-  })
-_sym_db.RegisterMessage(NinjaAction)
-
-DynamicExecution = _reflection.GeneratedProtocolMessageType('DynamicExecution', (_message.Message,), {
-  'DESCRIPTOR' : _DYNAMICEXECUTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.DynamicExecution)
-  })
-_sym_db.RegisterMessage(DynamicExecution)
-
-FailAction = _reflection.GeneratedProtocolMessageType('FailAction', (_message.Message,), {
-  'DESCRIPTOR' : _FAILACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.FailAction)
-  })
-_sym_db.RegisterMessage(FailAction)
-
-SymlinkAction = _reflection.GeneratedProtocolMessageType('SymlinkAction', (_message.Message,), {
-  'DESCRIPTOR' : _SYMLINKACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.SymlinkAction)
-  })
-_sym_db.RegisterMessage(SymlinkAction)
-
-CppLink = _reflection.GeneratedProtocolMessageType('CppLink', (_message.Message,), {
-  'DESCRIPTOR' : _CPPLINK,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.CppLink)
-  })
-_sym_db.RegisterMessage(CppLink)
-
-LtoAction = _reflection.GeneratedProtocolMessageType('LtoAction', (_message.Message,), {
-  'DESCRIPTOR' : _LTOACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.LtoAction)
-  })
-_sym_db.RegisterMessage(LtoAction)
-
-TestAction = _reflection.GeneratedProtocolMessageType('TestAction', (_message.Message,), {
-  'DESCRIPTOR' : _TESTACTION,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.TestAction)
-  })
-_sym_db.RegisterMessage(TestAction)
-
-Worker = _reflection.GeneratedProtocolMessageType('Worker', (_message.Message,), {
-  'DESCRIPTOR' : _WORKER,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Worker)
-  })
-_sym_db.RegisterMessage(Worker)
-
-Analysis = _reflection.GeneratedProtocolMessageType('Analysis', (_message.Message,), {
-  'DESCRIPTOR' : _ANALYSIS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Analysis)
-  })
-_sym_db.RegisterMessage(Analysis)
-
-PackageLoading = _reflection.GeneratedProtocolMessageType('PackageLoading', (_message.Message,), {
-  'DESCRIPTOR' : _PACKAGELOADING,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.PackageLoading)
-  })
-_sym_db.RegisterMessage(PackageLoading)
-
-Toolchain = _reflection.GeneratedProtocolMessageType('Toolchain', (_message.Message,), {
-  'DESCRIPTOR' : _TOOLCHAIN,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.Toolchain)
-  })
-_sym_db.RegisterMessage(Toolchain)
-
-StarlarkLoading = _reflection.GeneratedProtocolMessageType('StarlarkLoading', (_message.Message,), {
-  'DESCRIPTOR' : _STARLARKLOADING,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.StarlarkLoading)
-  })
-_sym_db.RegisterMessage(StarlarkLoading)
-
-ExternalDeps = _reflection.GeneratedProtocolMessageType('ExternalDeps', (_message.Message,), {
-  'DESCRIPTOR' : _EXTERNALDEPS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ExternalDeps)
-  })
-_sym_db.RegisterMessage(ExternalDeps)
-
-DiffAwareness = _reflection.GeneratedProtocolMessageType('DiffAwareness', (_message.Message,), {
-  'DESCRIPTOR' : _DIFFAWARENESS,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.DiffAwareness)
-  })
-_sym_db.RegisterMessage(DiffAwareness)
-
-ModqueryCommand = _reflection.GeneratedProtocolMessageType('ModqueryCommand', (_message.Message,), {
-  'DESCRIPTOR' : _MODQUERYCOMMAND,
-  '__module__' : 'src.main.protobuf.failure_details_pb2'
-  # @@protoc_insertion_point(class_scope:failure_details.ModqueryCommand)
-  })
-_sym_db.RegisterMessage(ModqueryCommand)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'src/main/protobuf/failure_details.proto\x12\x0f\x66\x61ilure_details\x1a google/protobuf/descriptor.proto\"*\n\x15\x46\x61ilureDetailMetadata\x12\x11\n\texit_code\x18\x01 \x01(\r\"\xe1\x1c\n\rFailureDetail\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x33\n\x0binterrupted\x18\x65 \x01(\x0b\x32\x1c.failure_details.InterruptedH\x00\x12\x42\n\x13\x65xternal_repository\x18g \x01(\x0b\x32#.failure_details.ExternalRepositoryH\x00\x12\x38\n\x0e\x62uild_progress\x18h \x01(\x0b\x32\x1e.failure_details.BuildProgressH\x00\x12\x38\n\x0eremote_options\x18j \x01(\x0b\x32\x1e.failure_details.RemoteOptionsH\x00\x12@\n\x12\x63lient_environment\x18k \x01(\x0b\x32\".failure_details.ClientEnvironmentH\x00\x12\'\n\x05\x63rash\x18l \x01(\x0b\x32\x16.failure_details.CrashH\x00\x12\x38\n\x0esymlink_forest\x18n \x01(\x0b\x32\x1e.failure_details.SymlinkForestH\x00\x12:\n\x0fpackage_options\x18r \x01(\x0b\x32\x1f.failure_details.PackageOptionsH\x00\x12<\n\x10remote_execution\x18s \x01(\x0b\x32 .failure_details.RemoteExecutionH\x00\x12/\n\texecution\x18t \x01(\x0b\x32\x1a.failure_details.ExecutionH\x00\x12\x31\n\nworkspaces\x18u \x01(\x0b\x32\x1b.failure_details.WorkspacesH\x00\x12\x36\n\rcrash_options\x18v \x01(\x0b\x32\x1d.failure_details.CrashOptionsH\x00\x12\x31\n\nfilesystem\x18w \x01(\x0b\x32\x1b.failure_details.FilesystemH\x00\x12>\n\x11\x65xecution_options\x18y \x01(\x0b\x32!.failure_details.ExecutionOptionsH\x00\x12+\n\x07\x63ommand\x18z \x01(\x0b\x32\x18.failure_details.CommandH\x00\x12\'\n\x05spawn\x18{ \x01(\x0b\x32\x16.failure_details.SpawnH\x00\x12\x32\n\x0bgrpc_server\x18| \x01(\x0b\x32\x1b.failure_details.GrpcServerH\x00\x12@\n\x12\x63\x61nonicalize_flags\x18} \x01(\x0b\x32\".failure_details.CanonicalizeFlagsH\x00\x12\x42\n\x13\x62uild_configuration\x18~ \x01(\x0b\x32#.failure_details.BuildConfigurationH\x00\x12\x34\n\x0cinfo_command\x18\x7f \x01(\x0b\x32\x1c.failure_details.InfoCommandH\x00\x12\x39\n\x0ememory_options\x18\x81\x01 \x01(\x0b\x32\x1e.failure_details.MemoryOptionsH\x00\x12(\n\x05query\x18\x82\x01 \x01(\x0b\x32\x16.failure_details.QueryH\x00\x12;\n\x0flocal_execution\x18\x84\x01 \x01(\x0b\x32\x1f.failure_details.LocalExecutionH\x00\x12\x35\n\x0c\x61\x63tion_cache\x18\x86\x01 \x01(\x0b\x32\x1c.failure_details.ActionCacheH\x00\x12\x37\n\rfetch_command\x18\x87\x01 \x01(\x0b\x32\x1d.failure_details.FetchCommandH\x00\x12\x35\n\x0csync_command\x18\x88\x01 \x01(\x0b\x32\x1c.failure_details.SyncCommandH\x00\x12,\n\x07sandbox\x18\x89\x01 \x01(\x0b\x32\x18.failure_details.SandboxH\x00\x12=\n\x10include_scanning\x18\x8b\x01 \x01(\x0b\x32 .failure_details.IncludeScanningH\x00\x12\x35\n\x0ctest_command\x18\x8c\x01 \x01(\x0b\x32\x1c.failure_details.TestCommandH\x00\x12\x35\n\x0c\x61\x63tion_query\x18\x8d\x01 \x01(\x0b\x32\x1c.failure_details.ActionQueryH\x00\x12;\n\x0ftarget_patterns\x18\x8e\x01 \x01(\x0b\x32\x1f.failure_details.TargetPatternsH\x00\x12\x37\n\rclean_command\x18\x90\x01 \x01(\x0b\x32\x1d.failure_details.CleanCommandH\x00\x12\x39\n\x0e\x63onfig_command\x18\x91\x01 \x01(\x0b\x32\x1e.failure_details.ConfigCommandH\x00\x12\x41\n\x12\x63onfigurable_query\x18\x92\x01 \x01(\x0b\x32\".failure_details.ConfigurableQueryH\x00\x12\x35\n\x0c\x64ump_command\x18\x93\x01 \x01(\x0b\x32\x1c.failure_details.DumpCommandH\x00\x12\x35\n\x0chelp_command\x18\x94\x01 \x01(\x0b\x32\x1c.failure_details.HelpCommandH\x00\x12\x39\n\x0emobile_install\x18\x96\x01 \x01(\x0b\x32\x1e.failure_details.MobileInstallH\x00\x12;\n\x0fprofile_command\x18\x97\x01 \x01(\x0b\x32\x1f.failure_details.ProfileCommandH\x00\x12\x33\n\x0brun_command\x18\x98\x01 \x01(\x0b\x32\x1b.failure_details.RunCommandH\x00\x12;\n\x0fversion_command\x18\x99\x01 \x01(\x0b\x32\x1f.failure_details.VersionCommandH\x00\x12\x44\n\x14print_action_command\x18\x9a\x01 \x01(\x0b\x32#.failure_details.PrintActionCommandH\x00\x12=\n\x10workspace_status\x18\x9e\x01 \x01(\x0b\x32 .failure_details.WorkspaceStatusH\x00\x12\x35\n\x0cjava_compile\x18\x9f\x01 \x01(\x0b\x32\x1c.failure_details.JavaCompileH\x00\x12=\n\x10\x61\x63tion_rewinding\x18\xa0\x01 \x01(\x0b\x32 .failure_details.ActionRewindingH\x00\x12\x33\n\x0b\x63pp_compile\x18\xa1\x01 \x01(\x0b\x32\x1b.failure_details.CppCompileH\x00\x12;\n\x0fstarlark_action\x18\xa2\x01 \x01(\x0b\x32\x1f.failure_details.StarlarkActionH\x00\x12\x35\n\x0cninja_action\x18\xa3\x01 \x01(\x0b\x32\x1c.failure_details.NinjaActionH\x00\x12?\n\x11\x64ynamic_execution\x18\xa4\x01 \x01(\x0b\x32!.failure_details.DynamicExecutionH\x00\x12\x33\n\x0b\x66\x61il_action\x18\xa6\x01 \x01(\x0b\x32\x1b.failure_details.FailActionH\x00\x12\x39\n\x0esymlink_action\x18\xa7\x01 \x01(\x0b\x32\x1e.failure_details.SymlinkActionH\x00\x12-\n\x08\x63pp_link\x18\xa8\x01 \x01(\x0b\x32\x18.failure_details.CppLinkH\x00\x12\x31\n\nlto_action\x18\xa9\x01 \x01(\x0b\x32\x1a.failure_details.LtoActionH\x00\x12\x33\n\x0btest_action\x18\xac\x01 \x01(\x0b\x32\x1b.failure_details.TestActionH\x00\x12*\n\x06worker\x18\xad\x01 \x01(\x0b\x32\x17.failure_details.WorkerH\x00\x12.\n\x08\x61nalysis\x18\xae\x01 \x01(\x0b\x32\x19.failure_details.AnalysisH\x00\x12;\n\x0fpackage_loading\x18\xaf\x01 \x01(\x0b\x32\x1f.failure_details.PackageLoadingH\x00\x12\x30\n\ttoolchain\x18\xb1\x01 \x01(\x0b\x32\x1a.failure_details.ToolchainH\x00\x12=\n\x10starlark_loading\x18\xb3\x01 \x01(\x0b\x32 .failure_details.StarlarkLoadingH\x00\x12\x37\n\rexternal_deps\x18\xb5\x01 \x01(\x0b\x32\x1d.failure_details.ExternalDepsH\x00\x12\x39\n\x0e\x64iff_awareness\x18\xb6\x01 \x01(\x0b\x32\x1e.failure_details.DiffAwarenessH\x00\x12=\n\x10modquery_command\x18\xb7\x01 \x01(\x0b\x32 .failure_details.ModqueryCommandH\x00\x12\x35\n\x0c\x62uild_report\x18\xb8\x01 \x01(\x0b\x32\x1c.failure_details.BuildReportH\x00\x42\n\n\x08\x63\x61tegoryJ\x04\x08\x02\x10\x65J\x04\x08\x66\x10gJ\x04\x08i\x10jJ\x04\x08m\x10nJ\x04\x08o\x10rJ\x04\x08x\x10yJ\x06\x08\x80\x01\x10\x81\x01J\x06\x08\x83\x01\x10\x84\x01J\x06\x08\x85\x01\x10\x86\x01J\x06\x08\x8a\x01\x10\x8b\x01J\x06\x08\x8f\x01\x10\x90\x01J\x06\x08\x95\x01\x10\x96\x01J\x06\x08\x9b\x01\x10\x9e\x01J\x06\x08\xa5\x01\x10\xa6\x01J\x06\x08\xaa\x01\x10\xac\x01J\x06\x08\xb0\x01\x10\xb1\x01J\x06\x08\xb2\x01\x10\xb3\x01J\x06\x08\xb4\x01\x10\xb5\x01\"\xa2\x05\n\x0bInterrupted\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.Interrupted.Code\"\xe1\x04\n\x04\x43ode\x12\x1e\n\x13INTERRUPTED_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08\x08\x12\x16\n\x0bINTERRUPTED\x10\x1c\x1a\x05\xb2\x43\x02\x08\x08\x12\x1b\n\x10\x44\x45PRECATED_BUILD\x10\x04\x1a\x05\xb2\x43\x02\x08\x08\x12&\n\x1b\x44\x45PRECATED_BUILD_COMPLETION\x10\x05\x1a\x05\xb2\x43\x02\x08\x08\x12*\n\x1f\x44\x45PRECATED_PACKAGE_LOADING_SYNC\x10\x06\x1a\x05\xb2\x43\x02\x08\x08\x12)\n\x1e\x44\x45PRECATED_EXECUTOR_COMPLETION\x10\x07\x1a\x05\xb2\x43\x02\x08\x08\x12&\n\x1b\x44\x45PRECATED_COMMAND_DISPATCH\x10\x08\x1a\x05\xb2\x43\x02\x08\x08\x12\x1f\n\x14\x44\x45PRECATED_INFO_ITEM\x10\t\x1a\x05\xb2\x43\x02\x08\x08\x12!\n\x16\x44\x45PRECATED_AFTER_QUERY\x10\n\x1a\x05\xb2\x43\x02\x08\x08\x12#\n\x18\x44\x45PRECATED_FETCH_COMMAND\x10\x11\x1a\x05\xb2\x43\x02\x08\x08\x12\"\n\x17\x44\x45PRECATED_SYNC_COMMAND\x10\x12\x1a\x05\xb2\x43\x02\x08\x08\x12#\n\x18\x44\x45PRECATED_CLEAN_COMMAND\x10\x14\x1a\x05\xb2\x43\x02\x08\x08\x12,\n!DEPRECATED_MOBILE_INSTALL_COMMAND\x10\x15\x1a\x05\xb2\x43\x02\x08\x08\x12\x1b\n\x10\x44\x45PRECATED_QUERY\x10\x16\x1a\x05\xb2\x43\x02\x08\x08\x12!\n\x16\x44\x45PRECATED_RUN_COMMAND\x10\x17\x1a\x05\xb2\x43\x02\x08\x08\x12%\n\x1a\x44\x45PRECATED_OPTIONS_PARSING\x10\x1b\x1a\x05\xb2\x43\x02\x08\x08\"\x04\x08\x01\x10\x03\"\x04\x08\x0b\x10\x10\"\x04\x08\x13\x10\x13\"\x04\x08\x18\x10\x1a\"\xc7\x04\n\x05Spawn\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Spawn.Code\x12\x14\n\x0c\x63\x61tastrophic\x18\x02 \x01(\x08\x12\x17\n\x0fspawn_exit_code\x18\x03 \x01(\x05\"\xe3\x03\n\x04\x43ode\x12\x18\n\rSPAWN_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNON_ZERO_EXIT\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x12\n\x07TIMEOUT\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rOUT_OF_MEMORY\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10\x45XECUTION_FAILED\x10\x04\x1a\x05\xb2\x43\x02\x08\"\x12\x1b\n\x10\x45XECUTION_DENIED\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13REMOTE_CACHE_FAILED\x10\x06\x1a\x05\xb2\x43\x02\x08\"\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x45XEC_IO_EXCEPTION\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0fINVALID_TIMEOUT\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#INVALID_REMOTE_EXECUTION_PROPERTIES\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NO_USABLE_STRATEGY_FOUND\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dUNSPECIFIED_EXECUTION_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14REMOTE_CACHE_EVICTED\x10\x0e\x1a\x05\xb2\x43\x02\x08\'\"\x84\x02\n\x12\x45xternalRepository\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.ExternalRepository.Code\"\xb5\x01\n\x04\x43ode\x12&\n\x1b\x45XTERNAL_REPOSITORY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x32\n\'OVERRIDE_DISALLOWED_MANAGED_DIRECTORIES\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x42\x41\x44_DOWNLOADER_CONFIG\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12/\n$REPOSITORY_MAPPING_RESOLUTION_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08%\"\xa7\x06\n\rBuildProgress\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.BuildProgress.Code\"\xe2\x05\n\x04\x43ode\x12!\n\x16\x42UILD_PROGRESS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12 \n\x15OUTPUT_INITIALIZATION\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12.\n#BES_RUNS_PER_TEST_LIMIT_UNSUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x42\x45S_LOCAL_WRITE_ERROR\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18\x42\x45S_INITIALIZATION_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18\x42\x45S_UPLOAD_TIMEOUT_ERROR\x10\x07\x1a\x05\xb2\x43\x02\x08&\x12!\n\x16\x42\x45S_FILE_WRITE_TIMEOUT\x10\x08\x1a\x05\xb2\x43\x02\x08&\x12\"\n\x17\x42\x45S_FILE_WRITE_IO_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08&\x12%\n\x1a\x42\x45S_FILE_WRITE_INTERRUPTED\x10\n\x1a\x05\xb2\x43\x02\x08&\x12\"\n\x17\x42\x45S_FILE_WRITE_CANCELED\x10\x0b\x1a\x05\xb2\x43\x02\x08&\x12\'\n\x1c\x42\x45S_FILE_WRITE_UNKNOWN_ERROR\x10\x0c\x1a\x05\xb2\x43\x02\x08&\x12&\n\x1b\x42\x45S_UPLOAD_LOCAL_FILE_ERROR\x10\r\x1a\x05\xb2\x43\x02\x08&\x12*\n\x1f\x42\x45S_STREAM_NOT_RETRYING_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08-\x12\x37\n,BES_STREAM_COMPLETED_WITH_UNACK_EVENTS_ERROR\x10\x0f\x1a\x05\xb2\x43\x02\x08-\x12\x38\n-BES_STREAM_COMPLETED_WITH_UNSENT_EVENTS_ERROR\x10\x10\x1a\x05\xb2\x43\x02\x08-\x12\x31\n&BES_STREAM_COMPLETED_WITH_REMOTE_ERROR\x10\x13\x1a\x05\xb2\x43\x02\x08-\x12\x32\n\'BES_UPLOAD_RETRY_LIMIT_EXCEEDED_FAILURE\x10\x11\x1a\x05\xb2\x43\x02\x08&\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x04\x08\x12\x10\x12\"\xc3\x02\n\rRemoteOptions\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.RemoteOptions.Code\"\xfe\x01\n\x04\x43ode\x12!\n\x16REMOTE_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x35\n*REMOTE_DEFAULT_EXEC_PROPERTIES_LOGIC_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x43REDENTIALS_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19\x43REDENTIALS_WRITE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1d\x44OWNLOADER_WITHOUT_GRPC_CACHE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1c\x45XECUTION_WITH_INVALID_CACHE\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\"\x9a\x01\n\x11\x43lientEnvironment\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.ClientEnvironment.Code\"N\n\x04\x43ode\x12%\n\x1a\x43LIENT_ENVIRONMENT_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14\x43LIENT_CWD_MALFORMED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\xb5\x01\n\x05\x43rash\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Crash.Code\x12*\n\x06\x63\x61uses\x18\x02 \x03(\x0b\x32\x1a.failure_details.Throwable\x12\x1d\n\x15oom_detector_override\x18\x03 \x01(\x08\"6\n\x04\x43ode\x12\x18\n\rCRASH_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x14\n\tCRASH_OOM\x10\x01\x1a\x05\xb2\x43\x02\x08!\"J\n\tThrowable\x12\x17\n\x0fthrowable_class\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x13\n\x0bstack_trace\x18\x03 \x03(\t\"\xe7\x01\n\rSymlinkForest\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.SymlinkForest.Code\"\xa2\x01\n\x04\x43ode\x12!\n\x16SYMLINK_FOREST_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%TOPLEVEL_OUTDIR_PACKAGE_PATH_CONFLICT\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eTOPLEVEL_OUTDIR_USED_AS_SOURCE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0f\x43REATION_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\"\xc4\x01\n\x0b\x42uildReport\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.BuildReport.Code\"\x83\x01\n\x04\x43ode\x12\x1f\n\x14\x42UILD_REPORT_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x34\n)BUILD_REPORT_UPLOADER_NEEDS_PACKAGE_PATHS\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19\x42UILD_REPORT_WRITE_FAILED\x10\x02\x1a\x05\xb2\x43\x02\x08$\"\x9d\x01\n\x0ePackageOptions\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.PackageOptions.Code\"W\n\x04\x43ode\x12\"\n\x17PACKAGE_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14PACKAGE_PATH_INVALID\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x02\x10\x02\"\x04\x08\x03\x10\x03\"\xb3\x06\n\x0fRemoteExecution\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.RemoteExecution.Code\"\xea\x05\n\x04\x43ode\x12#\n\x18REMOTE_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1a\x43\x41PABILITIES_QUERY_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\"\x12#\n\x18\x43REDENTIALS_INIT_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12\x43\x41\x43HE_INIT_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0fRPC_LOG_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19\x45XEC_CHANNEL_INIT_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1a\x43\x41\x43HE_CHANNEL_INIT_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1f\x44OWNLOADER_CHANNEL_INIT_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17LOG_DIR_CLEANUP_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x43LIENT_SERVER_INCOMPATIBLE\x10\t\x1a\x05\xb2\x43\x02\x08\"\x12-\n\"DOWNLOADED_INPUTS_DELETION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\"\x12@\n5REMOTE_DOWNLOAD_OUTPUTS_MINIMAL_WITHOUT_INMEMORY_DOTD\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x41\n6REMOTE_DOWNLOAD_OUTPUTS_MINIMAL_WITHOUT_INMEMORY_JDEPS\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\x12\x35\n*INCOMPLETE_OUTPUT_DOWNLOAD_CLEANUP_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12;\n0REMOTE_DEFAULT_PLATFORM_PROPERTIES_PARSE_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0eILLEGAL_OUTPUT\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12/\n$INVALID_EXEC_AND_PLATFORM_PROPERTIES\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\"\xd8\r\n\tExecution\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.Execution.Code\"\x9b\r\n\x04\x43ode\x12\x1c\n\x11\x45XECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12/\n$EXECUTION_LOG_INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12&\n\x1b\x45XECUTION_LOG_WRITE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19\x45XECROOT_CREATION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-TEMP_ACTION_OUTPUT_DIRECTORY_DELETION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-TEMP_ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12>\n3PERSISTENT_ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x31\n&LOCAL_OUTPUT_DIRECTORY_SYMLINK_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12+\n LOCAL_TEMPLATE_EXPANSION_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08$\x12-\n\"INPUT_DIRECTORY_CHECK_IO_EXCEPTION\x10\n\x1a\x05\xb2\x43\x02\x08$\x12/\n$EXTRA_ACTION_OUTPUT_CREATION_FAILURE\x10\x0b\x1a\x05\xb2\x43\x02\x08$\x12#\n\x18TEST_RUNNER_IO_EXCEPTION\x10\x0c\x1a\x05\xb2\x43\x02\x08$\x12\"\n\x17\x46ILE_WRITE_IO_EXCEPTION\x10\r\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19TEST_OUT_ERR_IO_EXCEPTION\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_MANIFEST_COPY_IO_EXCEPTION\x10\x0f\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_MANIFEST_LINK_IO_EXCEPTION\x10\x10\x1a\x05\xb2\x43\x02\x08$\x12-\n\"SYMLINK_TREE_CREATION_IO_EXCEPTION\x10\x11\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'SYMLINK_TREE_CREATION_COMMAND_EXCEPTION\x10\x12\x1a\x05\xb2\x43\x02\x08$\x12)\n\x1e\x41\x43TION_INPUT_READ_IO_EXCEPTION\x10\x13\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15\x41\x43TION_NOT_UP_TO_DATE\x10\x14\x1a\x05\xb2\x43\x02\x08\x01\x12-\n\"PSEUDO_ACTION_EXECUTION_PROHIBITED\x10\x15\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x44ISCOVERED_INPUT_DOES_NOT_EXIST\x10\x16\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1f\x41\x43TION_OUTPUTS_DELETION_FAILURE\x10\x17\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x41\x43TION_OUTPUTS_NOT_CREATED\x10\x18\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x41\x43TION_FINALIZATION_FAILURE\x10\x19\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x41\x43TION_INPUT_LOST\x10\x1a\x1a\x05\xb2\x43\x02\x08\x01\x12,\n!FILESYSTEM_CONTEXT_UPDATE_FAILURE\x10\x1b\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x41\x43TION_OUTPUT_CLOSE_FAILURE\x10\x1c\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cINPUT_DISCOVERY_IO_EXCEPTION\x10\x1d\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(TREE_ARTIFACT_DIRECTORY_CREATION_FAILURE\x10\x1e\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(ACTION_OUTPUT_DIRECTORY_CREATION_FAILURE\x10\x1f\x1a\x05\xb2\x43\x02\x08\x01\x12\x36\n+ACTION_FS_OUTPUT_DIRECTORY_CREATION_FAILURE\x10 \x1a\x05\xb2\x43\x02\x08\x01\x12\x37\n,ACTION_FS_OUT_ERR_DIRECTORY_CREATION_FAILURE\x10!\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cNON_ACTION_EXECUTION_FAILURE\x10\"\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10#\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14SOURCE_INPUT_MISSING\x10$\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14UNEXPECTED_EXCEPTION\x10%\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19SOURCE_INPUT_IO_EXCEPTION\x10\'\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x08\x10\x08\"\x04\x08&\x10&\"\xc4\x02\n\nWorkspaces\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.Workspaces.Code\"\x85\x02\n\x04\x43ode\x12\x1d\n\x12WORKSPACES_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%WORKSPACES_LOG_INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cWORKSPACES_LOG_WRITE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12\x42\n7ILLEGAL_WORKSPACE_FILE_SYMLINK_WITH_MANAGED_DIRECTORIES\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12?\n4WORKSPACE_FILE_READ_FAILURE_WITH_MANAGED_DIRECTORIES\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\"p\n\x0c\x43rashOptions\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.CrashOptions.Code\".\n\x04\x43ode\x12 \n\x15\x43RASH_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\"\x04\x08\x01\x10\x01\"\xb2\x02\n\nFilesystem\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.Filesystem.Code\"\xf3\x01\n\x04\x43ode\x12\x1d\n\x12\x46ILESYSTEM_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x30\n%EMBEDDED_BINARIES_ENUMERATION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12+\n SERVER_PID_TXT_FILE_READ_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12$\n\x19SERVER_FILE_WRITE_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x35\n*DEFAULT_DIGEST_HASH_FUNCTION_INVALID_VALUE\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x04\x08\x07\x10\x07\"\xea\x03\n\x10\x45xecutionOptions\x12\x34\n\x04\x63ode\x18\x01 \x01(\x0e\x32&.failure_details.ExecutionOptions.Code\"\x9f\x03\n\x04\x43ode\x12$\n\x19\x45XECUTION_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10INVALID_STRATEGY\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12:\n/REQUESTED_STRATEGY_INCOMPATIBLE_WITH_SANDBOXING\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1f\x44\x45PRECATED_LOCAL_RESOURCES_USED\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1fINVALID_CYCLIC_DYNAMIC_STRATEGY\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'RESTRICTION_UNMATCHED_TO_ACTION_CONTEXT\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+REMOTE_FALLBACK_STRATEGY_NOT_ABSTRACT_SPAWN\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12STRATEGY_NOT_FOUND\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1e\x44YNAMIC_STRATEGY_NOT_SANDBOXED\x10\n\x1a\x05\xb2\x43\x02\x08\x02\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02\"\x96\x05\n\x07\x43ommand\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.Command.Code\"\xdd\x04\n\x04\x43ode\x12\"\n\x17\x43OMMAND_FAILURE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1c\n\x11\x43OMMAND_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17\x41NOTHER_COMMAND_RUNNING\x10\x02\x1a\x05\xb2\x43\x02\x08\t\x12\x1e\n\x13PREVIOUSLY_SHUTDOWN\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12;\n0STARLARK_CPU_PROFILE_FILE_INITIALIZATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x38\n-STARLARK_CPU_PROFILING_INITIALIZATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'STARLARK_CPU_PROFILE_FILE_WRITE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12*\n\x1fINVOCATION_POLICY_PARSE_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19INVOCATION_POLICY_INVALID\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15OPTIONS_PARSE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eSTARLARK_OPTIONS_PARSE_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x41RGUMENTS_NOT_RECOGNIZED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10NOT_IN_WORKSPACE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18SPACES_IN_WORKSPACE_PATH\x10\r\x1a\x05\xb2\x43\x02\x08$\x12\x1e\n\x13IN_OUTPUT_DIRECTORY\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\"\xec\x01\n\nGrpcServer\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.GrpcServer.Code\"\xad\x01\n\x04\x43ode\x12\x1e\n\x13GRPC_SERVER_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12&\n\x1bGRPC_SERVER_NOT_COMPILED_IN\x10\x01\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13SERVER_BIND_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x15\n\nBAD_COOKIE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15NO_CLIENT_DESCRIPTION\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\x04\x08\x05\x10\x05\"\x99\x01\n\x11\x43\x61nonicalizeFlags\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.CanonicalizeFlags.Code\"M\n\x04\x43ode\x12%\n\x1a\x43\x41NONICALIZE_FLAGS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13\x46OR_COMMAND_INVALID\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\xc2\x04\n\x12\x42uildConfiguration\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.BuildConfiguration.Code\"\xf3\x03\n\x04\x43ode\x12&\n\x1b\x42UILD_CONFIGURATION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12.\n#PLATFORM_MAPPING_EVALUATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12.\n#PLATFORM_MAPPINGS_FILE_IS_DIRECTORY\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12+\n PLATFORM_MAPPINGS_FILE_NOT_FOUND\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(TOP_LEVEL_CONFIGURATION_CREATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15INVALID_CONFIGURATION\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15INVALID_BUILD_OPTIONS\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16MULTI_CPU_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\x33\n(HEURISTIC_INSTRUMENTATION_FILTER_INVALID\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x10\n\x05\x43YCLE\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1a\x43ONFLICTING_CONFIGURATIONS\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12,\n!INVALID_OUTPUT_DIRECTORY_MNEMONIC\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\"\xe9\x01\n\x0bInfoCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.InfoCommand.Code\"\xa8\x01\n\x04\x43ode\x12\x1f\n\x14INFO_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rTOO_MANY_KEYS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12KEY_NOT_RECOGNIZED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18INFO_BLOCK_WRITE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12!\n\x16\x41LL_INFO_WRITE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\x83\x02\n\rMemoryOptions\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.MemoryOptions.Code\"\xbe\x01\n\x04\x43ode\x12!\n\x16MEMORY_OPTIONS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12@\n5EXPERIMENTAL_OOM_MORE_EAGERLY_THRESHOLD_INVALID_VALUE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12Q\nDDEPRECATED_EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND\x10\x02\x1a\x07\x08\x01\xb2\x43\x02\x08\x02\"\xf2\x0b\n\x05Query\x12)\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1b.failure_details.Query.Code\"\xbd\x0b\n\x04\x43ode\x12\x18\n\rQUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x32\n\'QUERY_FILE_WITH_COMMAND_LINE_EXPRESSION\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17QUERY_FILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15OUTPUT_FORMAT_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16GRAPHLESS_PREREQ_UNMET\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aQUERY_OUTPUT_WRITE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aQUERY_STDOUT_FLUSH_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12&\n\x1b\x41NALYSIS_QUERY_PREREQ_UNMET\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\x12&\n\x1bQUERY_RESULTS_FLUSH_FAILURE\x10\x0f\x1a\x05\xb2\x43\x02\x08$\x12\x39\n.DEPRECATED_UNCLOSED_QUOTATION_EXPRESSION_ERROR\x10\x10\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15VARIABLE_NAME_INVALID\x10\x11\x1a\x05\xb2\x43\x02\x08\x07\x12\x1d\n\x12VARIABLE_UNDEFINED\x10\x12\x1a\x05\xb2\x43\x02\x08\x07\x12\x44\n9BUILDFILES_AND_LOADFILES_CANNOT_USE_OUTPUT_LOCATION_ERROR\x10\x13\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10\x42UILD_FILE_ERROR\x10\x14\x1a\x05\xb2\x43\x02\x08\x07\x12\x10\n\x05\x43YCLE\x10\x15\x1a\x05\xb2\x43\x02\x08\x07\x12+\n UNIQUE_SKYKEY_THRESHOLD_EXCEEDED\x10\x16\x1a\x05\xb2\x43\x02\x08\x07\x12\'\n\x1cTARGET_NOT_IN_UNIVERSE_SCOPE\x10\x17\x1a\x05\xb2\x43\x02\x08\x02\x12+\n INVALID_FULL_UNIVERSE_EXPRESSION\x10\x18\x1a\x05\xb2\x43\x02\x08\x07\x12(\n\x1dUNIVERSE_SCOPE_LIMIT_EXCEEDED\x10\x19\x1a\x05\xb2\x43\x02\x08\x07\x12&\n\x1bINVALIDATION_LIMIT_EXCEEDED\x10\x1a\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1aOUTPUT_FORMAT_PREREQ_UNMET\x10\x1b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x41RGUMENTS_MISSING\x10\x1c\x1a\x05\xb2\x43\x02\x08\x07\x12\x31\n&RBUILDFILES_FUNCTION_REQUIRES_SKYQUERY\x10\x1d\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1a\x46ULL_TARGETS_NOT_SUPPORTED\x10\x1e\x1a\x05\xb2\x43\x02\x08\x07\x12,\n!DEPRECATED_UNEXPECTED_TOKEN_ERROR\x10\x1f\x1a\x05\xb2\x43\x02\x08\x02\x12-\n\"DEPRECATED_INTEGER_LITERAL_MISSING\x10 \x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+DEPRECATED_INVALID_STARTING_CHARACTER_ERROR\x10!\x1a\x05\xb2\x43\x02\x08\x02\x12\x32\n\'DEPRECATED_PREMATURE_END_OF_INPUT_ERROR\x10\"\x1a\x05\xb2\x43\x02\x08\x02\x12\x17\n\x0cSYNTAX_ERROR\x10#\x1a\x05\xb2\x43\x02\x08\x02\x12(\n\x1dOUTPUT_FORMATTER_IO_EXCEPTION\x10$\x1a\x05\xb2\x43\x02\x08$\x12+\n SKYQUERY_TRANSITIVE_TARGET_ERROR\x10%\x1a\x05\xb2\x43\x02\x08\x07\x12$\n\x19SKYQUERY_TARGET_EXCEPTION\x10&\x1a\x05\xb2\x43\x02\x08\x07\x12&\n\x1bINVALID_LABEL_IN_TEST_SUITE\x10\'\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18ILLEGAL_FLAG_COMBINATION\x10(\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12NON_DETAILED_ERROR\x10)\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x07\x10\x0c\"\x99\x01\n\x0eLocalExecution\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.LocalExecution.Code\"S\n\x04\x43ode\x12\"\n\x17LOCAL_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\'\n\x1cLOCKFREE_OUTPUT_PREREQ_UNMET\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x8a\x01\n\x0b\x41\x63tionCache\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.ActionCache.Code\"J\n\x04\x43ode\x12\x1f\n\x14\x41\x43TION_CACHE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12!\n\x16INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\"\xe7\x01\n\x0c\x46\x65tchCommand\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.FetchCommand.Code\"\xa4\x01\n\x04\x43ode\x12 \n\x15\x46\x45TCH_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1d\n\x12\x45XPRESSION_MISSING\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1a\n\x0fOPTIONS_INVALID\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11QUERY_PARSE_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12!\n\x16QUERY_EVALUATION_ERROR\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\"\xf8\x01\n\x0bSyncCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.SyncCommand.Code\"\xb7\x01\n\x04\x43ode\x12\x1f\n\x14SYNC_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14PACKAGE_LOOKUP_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x07\x12%\n\x1aWORKSPACE_EVALUATION_ERROR\x10\x02\x1a\x05\xb2\x43\x02\x08\x07\x12\"\n\x17REPOSITORY_FETCH_ERRORS\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12\"\n\x17REPOSITORY_NAME_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x07\"\xfb\x03\n\x07Sandbox\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.Sandbox.Code\"\xc2\x03\n\x04\x43ode\x12\"\n\x17SANDBOX_FAILURE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12!\n\x16INITIALIZATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12!\n\x16\x45XECUTION_IO_EXCEPTION\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12!\n\x16\x44OCKER_COMMAND_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fNO_DOCKER_IMAGE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12+\n DOCKER_IMAGE_PREPARATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x42IND_MOUNT_ANALYSIS_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bMOUNT_SOURCE_DOES_NOT_EXIST\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12,\n!MOUNT_SOURCE_TARGET_TYPE_MISMATCH\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bMOUNT_TARGET_DOES_NOT_EXIST\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17SUBPROCESS_START_FAILED\x10\n\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\"\x9d\x04\n\x0fIncludeScanning\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.IncludeScanning.Code\x12\x42\n\x14package_loading_code\x18\x02 \x01(\x0e\x32$.failure_details.PackageLoading.Code\"\x90\x03\n\x04\x43ode\x12#\n\x18INCLUDE_SCANNING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1eINITIALIZE_INCLUDE_HINTS_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15SCANNING_IO_EXCEPTION\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12,\n!INCLUDE_HINTS_FILE_NOT_IN_PACKAGE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aINCLUDE_HINTS_READ_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15ILLEGAL_ABSOLUTE_PATH\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_LOAD_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19USER_PACKAGE_LOAD_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bSYSTEM_PACKAGE_LOAD_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12\x30\n%UNDIFFERENTIATED_PACKAGE_LOAD_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\"\xbc\x01\n\x0bTestCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.TestCommand.Code\"|\n\x04\x43ode\x12\x1f\n\x14TEST_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1a\n\x0fNO_TEST_TARGETS\x10\x01\x1a\x05\xb2\x43\x02\x08\x04\x12\x1e\n\x13TEST_WITH_NOANALYZE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x17\n\x0cTESTS_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x03\"\xa6\x05\n\x0b\x41\x63tionQuery\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.ActionQuery.Code\"\xe5\x04\n\x04\x43ode\x12\x1f\n\x14\x41\x43TION_QUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x19\n\x0eOUTPUT_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x06\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x45XPRESSION_PARSE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12\x36\n+SKYFRAME_STATE_WITH_COMMAND_LINE_EXPRESSION\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12$\n\x19INVALID_AQUERY_EXPRESSION\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1bSKYFRAME_STATE_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x41QUERY_OUTPUT_TOO_BIG\x10\x08\x1a\x05\xb2\x43\x02\x08\x07\x12!\n\x16ILLEGAL_PATTERN_SYNTAX\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13INCORRECT_ARGUMENTS\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12>\n3TOP_LEVEL_TARGETS_WITH_SKYFRAME_STATE_NOT_SUPPORTED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eSKYFRAME_STATE_AFTER_EXECUTION\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dLABELS_FUNCTION_NOT_SUPPORTED\x10\r\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aTEMPLATE_EXPANSION_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08\x02\"\xd7\x06\n\x0eTargetPatterns\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.TargetPatterns.Code\"\x90\x06\n\x04\x43ode\x12\"\n\x17TARGET_PATTERNS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x38\n-TARGET_PATTERN_FILE_WITH_COMMAND_LINE_PATTERN\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12+\n TARGET_PATTERN_FILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cTARGET_PATTERN_PARSE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11PACKAGE_NOT_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15TARGET_FORMAT_INVALID\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x41\x42SOLUTE_TARGET_PATTERN_INVALID\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%CANNOT_DETERMINE_TARGET_FROM_FILENAME\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12LABEL_SYNTAX_ERROR\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dTARGET_CANNOT_BE_EMPTY_STRING\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12+\n PACKAGE_PART_CANNOT_END_IN_SLASH\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15\x43\x41NNOT_PRELOAD_TARGET\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fTARGETS_MISSING\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%RECURSIVE_TARGET_PATTERNS_NOT_ALLOWED\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1fUP_LEVEL_REFERENCES_NOT_ALLOWED\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#NEGATIVE_TARGET_PATTERN_NOT_ALLOWED\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15TARGET_MUST_BE_A_FILE\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x44\x45PENDENCY_NOT_FOUND\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_NAME_INVALID\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\"\xf5\x03\n\x0c\x43leanCommand\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.CleanCommand.Code\"\xb2\x03\n\x04\x43ode\x12 \n\x15\x43LEAN_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\'\n\x1cOUTPUT_SERVICE_CLEAN_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x06\x12%\n\x1a\x41\x43TION_CACHE_CLEAN_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12 \n\x15OUT_ERR_CLOSE_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aOUTPUT_BASE_DELETE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1dOUTPUT_BASE_TEMP_MOVE_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12+\n ASYNC_OUTPUT_BASE_DELETE_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x06\x12\"\n\x17\x45XECROOT_DELETE_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x45XECROOT_TEMP_MOVE_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08$\x12(\n\x1d\x41SYNC_EXECROOT_DELETE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x06\x12#\n\x18\x41RGUMENTS_NOT_RECOGNIZED\x10\n\x1a\x05\xb2\x43\x02\x08\x02\"\xb1\x01\n\rConfigCommand\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.ConfigCommand.Code\"m\n\x04\x43ode\x12!\n\x16\x43ONFIG_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13TOO_MANY_CONFIG_IDS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\"\n\x17\x43ONFIGURATION_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xbb\x04\n\x11\x43onfigurableQuery\x12\x35\n\x04\x63ode\x18\x01 \x01(\x0e\x32\'.failure_details.ConfigurableQuery.Code\"\xee\x03\n\x04\x43ode\x12%\n\x1a\x43ONFIGURABLE_QUERY_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12*\n\x1f\x43OMMAND_LINE_EXPRESSION_MISSING\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12#\n\x18\x45XPRESSION_PARSE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x46ILTERS_NOT_SUPPORTED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12,\n!BUILDFILES_FUNCTION_NOT_SUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1fSIBLINGS_FUNCTION_NOT_SUPPORTED\x10\x05\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eVISIBLE_FUNCTION_NOT_SUPPORTED\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x41TTRIBUTE_MISSING\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12*\n\x1fINCORRECT_CONFIG_ARGUMENT_ERROR\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12\x19\n\x0eTARGET_MISSING\x10\t\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15STARLARK_SYNTAX_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13STARLARK_EVAL_ERROR\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15\x46ORMAT_FUNCTION_ERROR\x10\x0c\x1a\x05\xb2\x43\x02\x08\x02\"\xa9\x02\n\x0b\x44umpCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.DumpCommand.Code\"\xe8\x01\n\x04\x43ode\x12\x1f\n\x14\x44UMP_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13NO_OUTPUT_SPECIFIED\x10\x01\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18\x41\x43TION_CACHE_DUMP_FAILED\x10\x02\x1a\x05\xb2\x43\x02\x08\x07\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x07\x12#\n\x18\x41\x43TION_GRAPH_DUMP_FAILED\x10\x04\x1a\x05\xb2\x43\x02\x08\x07\x12$\n\x19STARLARK_HEAP_DUMP_FAILED\x10\x05\x1a\x05\xb2\x43\x02\x08\x08\"\x04\x08\x06\x10\x06\"\xa2\x01\n\x0bHelpCommand\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.HelpCommand.Code\"b\n\x04\x43ode\x12\x1f\n\x14HELP_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MISSING_ARGUMENT\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11\x43OMMAND_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\"\xb1\x02\n\rMobileInstall\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.MobileInstall.Code\"\xec\x01\n\x04\x43ode\x12!\n\x16MOBILE_INSTALL_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13\x43LASSIC_UNSUPPORTED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13NO_TARGET_SPECIFIED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aMULTIPLE_TARGETS_SPECIFIED\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12\x1e\n\x13TARGET_TYPE_INVALID\x10\x04\x1a\x05\xb2\x43\x02\x08\x06\x12\x18\n\rNON_ZERO_EXIT\x10\x05\x1a\x05\xb2\x43\x02\x08\x06\x12 \n\x15\x45RROR_RUNNING_PROGRAM\x10\x06\x1a\x05\xb2\x43\x02\x08\x06\"\xb8\x01\n\x0eProfileCommand\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.ProfileCommand.Code\"r\n\x04\x43ode\x12\"\n\x17PROFILE_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12(\n\x1dOLD_BINARY_FORMAT_UNSUPPORTED\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x46ILE_READ_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xc6\x05\n\nRunCommand\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.RunCommand.Code\"\x87\x05\n\x04\x43ode\x12\x1e\n\x13RUN_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13NO_TARGET_SPECIFIED\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12%\n\x1aTOO_MANY_TARGETS_SPECIFIED\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12 \n\x15TARGET_NOT_EXECUTABLE\x10\x03\x1a\x05\xb2\x43\x02\x08\x02\x12/\n$TARGET_BUILT_BUT_PATH_NOT_EXECUTABLE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x32\n\'TARGET_BUILT_BUT_PATH_VALIDATION_FAILED\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1aRUN_UNDER_TARGET_NOT_BUILT\x10\x06\x1a\x05\xb2\x43\x02\x08\x02\x12\x1b\n\x10RUN_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x02\x12\'\n\x1cTOO_MANY_TEST_SHARDS_OR_RUNS\x10\x08\x1a\x05\xb2\x43\x02\x08\x02\x12)\n\x1eTEST_ENVIRONMENT_SETUP_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08$\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08$\x12\x1d\n\x12NO_SHELL_SPECIFIED\x10\x0b\x1a\x05\xb2\x43\x02\x08\x02\x12\x1f\n\x14SCRIPT_WRITE_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x06\x12\x30\n%RUNFILES_DIRECTORIES_CREATION_FAILURE\x10\r\x1a\x05\xb2\x43\x02\x08$\x12-\n\"RUNFILES_SYMLINKS_CREATION_FAILURE\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12-\n\"TEST_ENVIRONMENT_SETUP_INTERRUPTED\x10\x0f\x1a\x05\xb2\x43\x02\x08\x08\"\x8a\x01\n\x0eVersionCommand\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.VersionCommand.Code\"D\n\x04\x43ode\x12\"\n\x17VERSION_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNOT_AVAILABLE\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\"\x88\x02\n\x12PrintActionCommand\x12\x36\n\x04\x63ode\x18\x01 \x01(\x0e\x32(.failure_details.PrintActionCommand.Code\"\xb9\x01\n\x04\x43ode\x12\'\n\x1cPRINT_ACTION_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10TARGET_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17TARGET_KIND_UNSUPPORTED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11\x41\x43TIONS_NOT_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\"\xc8\x02\n\x0fWorkspaceStatus\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.WorkspaceStatus.Code\"\xff\x01\n\x04\x43ode\x12#\n\x18WORKSPACE_STATUS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x18\n\rNON_ZERO_EXIT\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x41\x42NORMAL_TERMINATION\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0b\x45XEC_FAILED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rPARSE_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\x12\x1d\n\x12VALIDATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x43ONTENT_UPDATE_IO_EXCEPTION\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13STDERR_IO_EXCEPTION\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\"\x94\x02\n\x0bJavaCompile\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.JavaCompile.Code\"\xd3\x01\n\x04\x43ode\x12\x1f\n\x14JAVA_COMPILE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19REDUCED_CLASSPATH_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17JDEPS_READ_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12\x35\n*REDUCED_CLASSPATH_FALLBACK_CLEANUP_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08$\"\xba\x01\n\x0f\x41\x63tionRewinding\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.ActionRewinding.Code\"r\n\x04\x43ode\x12#\n\x18\x41\x43TION_REWINDING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19LOST_INPUT_TOO_MANY_TIMES\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14LOST_INPUT_IS_SOURCE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\x8d\x04\n\nCppCompile\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.CppCompile.Code\"\xce\x03\n\x04\x43ode\x12\x1e\n\x13\x43PP_COMPILE_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1e\x46IND_USED_HEADERS_IO_EXCEPTION\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\x1f\n\x14\x43OPY_OUT_ERR_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\x12\x1e\n\x13\x44_FILE_READ_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08$\x12%\n\x1a\x43OMMAND_GENERATION_FAILURE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18MODULE_EXPANSION_TIMEOUT\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eINCLUDE_PATH_OUTSIDE_EXEC_ROOT\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x46\x41KE_COMMAND_GENERATION_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15UNDECLARED_INCLUSIONS\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14\x44_FILE_PARSE_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x43OVERAGE_NOTES_CREATION_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dMODULE_EXPANSION_MISSING_DATA\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\"\xc9\x01\n\x0eStarlarkAction\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.StarlarkAction.Code\"\x82\x01\n\x04\x43ode\x12\"\n\x17STARLARK_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12)\n\x1eUNUSED_INPUT_LIST_READ_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12+\n UNUSED_INPUT_LIST_FILE_NOT_FOUND\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xb8\x01\n\x0bNinjaAction\x12/\n\x04\x63ode\x18\x01 \x01(\x0e\x32!.failure_details.NinjaAction.Code\"x\n\x04\x43ode\x12\x1f\n\x14NINJA_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12.\n#INVALID_DEPFILE_DECLARED_DEPENDENCY\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\x1f\n\x14\x44_FILE_PARSE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08$\"\xff\x01\n\x10\x44ynamicExecution\x12\x34\n\x04\x63ode\x18\x01 \x01(\x0e\x32&.failure_details.DynamicExecution.Code\"\xb4\x01\n\x04\x43ode\x12$\n\x19\x44YNAMIC_EXECUTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1aXCODE_RELATED_PREREQ_UNMET\x10\x01\x1a\x05\xb2\x43\x02\x08$\x12\"\n\x17\x41\x43TION_LOG_MOVE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bRUN_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NO_USABLE_STRATEGY_FOUND\x10\x04\x1a\x05\xb2\x43\x02\x08\x02\"\x92\x03\n\nFailAction\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.FailAction.Code\"\xd3\x02\n\x04\x43ode\x12\x1e\n\x13\x46\x41IL_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1e\n\x13INTENTIONAL_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18INCORRECT_PYTHON_VERSION\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16PROGUARD_SPECS_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1d\x44YNAMIC_LINKING_NOT_SUPPORTED\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14SOURCE_FILES_MISSING\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13INCORRECT_TOOLCHAIN\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16\x46RAGMENT_CLASS_MISSING\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43\x41NT_BUILD_INCOMPATIBLE_TARGET\x10\n\x1a\x05\xb2\x43\x02\x08\x01\"\x04\x08\x08\x10\x08\"\x04\x08\t\x10\t\"\xb3\x02\n\rSymlinkAction\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.SymlinkAction.Code\"\xee\x01\n\x04\x43ode\x12!\n\x16SYMLINK_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12$\n\x19\x45XECUTABLE_INPUT_NOT_FILE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17\x45XECUTABLE_INPUT_IS_NOT\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#EXECUTABLE_INPUT_CHECK_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aLINK_CREATION_IO_EXCEPTION\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17LINK_TOUCH_IO_EXCEPTION\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\"\xae\x01\n\x07\x43ppLink\x12+\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1d.failure_details.CppLink.Code\"v\n\x04\x43ode\x12\x1b\n\x10\x43PP_LINK_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1a\x43OMMAND_GENERATION_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x46\x41KE_COMMAND_GENERATION_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\"\xd7\x01\n\tLtoAction\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.LtoAction.Code\"\x9a\x01\n\x04\x43ode\x12\x1d\n\x12LTO_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12+\n INVALID_ABSOLUTE_PATH_IN_IMPORTS\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15MISSING_BITCODE_FILES\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19IMPORTS_READ_IO_EXCEPTION\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\"\x96\x02\n\nTestAction\x12.\n\x04\x63ode\x18\x01 \x01(\x0e\x32 .failure_details.TestAction.Code\"\xd7\x01\n\x04\x43ode\x12\x1e\n\x13TEST_ACTION_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12%\n\x1aNO_KEEP_GOING_TEST_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\"\n\x17LOCAL_TEST_PREREQ_UNMET\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x43OMMAND_LINE_EXPANSION_FAILURE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x44UPLICATE_CPU_TAGS\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fINVALID_CPU_TAG\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\"\xf1\x03\n\x06Worker\x12*\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1c.failure_details.Worker.Code\"\xba\x03\n\x04\x43ode\x12\x19\n\x0eWORKER_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12/\n$MULTIPLEXER_INSTANCE_REMOVAL_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aMULTIPLEXER_DOES_NOT_EXIST\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x13\n\x08NO_TOOLS\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bNO_FLAGFILE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x30\n%VIRTUAL_INPUT_MATERIALIZATION_FAILURE\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x42ORROW_FAILURE\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10PREFETCH_FAILURE\x10\x07\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0fPREPARE_FAILURE\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fREQUEST_FAILURE\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16PARSE_RESPONSE_FAILURE\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bNO_RESPONSE\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x46INISH_FAILURE\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x46ORBIDDEN_INPUT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\"\xbe\x06\n\x08\x41nalysis\x12,\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1e.failure_details.Analysis.Code\"\x83\x06\n\x04\x43ode\x12\x1b\n\x10\x41NALYSIS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x17\n\x0cLOAD_FAILURE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dGENERIC_LOADING_PHASE_FAILURE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18NOT_ALL_TARGETS_ANALYZED\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x10\n\x05\x43YCLE\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x31\n&PARAMETERIZED_TOP_LEVEL_ASPECT_INVALID\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12$\n\x19\x41SPECT_LABEL_SYNTAX_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13\x41SPECT_PREREQ_UNMET\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10\x41SPECT_NOT_FOUND\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0f\x41\x43TION_CONFLICT\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x41RTIFACT_PREFIX_CONFLICT\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dUNEXPECTED_ANALYSIS_EXCEPTION\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1cTARGETS_MISSING_ENVIRONMENTS\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13INVALID_ENVIRONMENT\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12*\n\x1f\x45NVIRONMENT_MISSING_FROM_GROUPS\x10\x0e\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x45XEC_GROUP_MISSING\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aINVALID_EXECUTION_PLATFORM\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16\x41SPECT_CREATION_FAILED\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12+\n CONFIGURED_VALUE_CREATION_FAILED\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dINCOMPATIBLE_TARGET_REQUESTED\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#ANALYSIS_FAILURE_PROPAGATION_FAILED\x10\x14\x1a\x05\xb2\x43\x02\x08\x01\"\xb8\t\n\x0ePackageLoading\x12\x32\n\x04\x63ode\x18\x01 \x01(\x0e\x32$.failure_details.PackageLoading.Code\"\xf1\x08\n\x04\x43ode\x12\"\n\x17PACKAGE_LOADING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1f\n\x14WORKSPACE_FILE_ERROR\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eMAX_COMPUTATION_STEPS_EXCEEDED\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12\x42UILD_FILE_MISSING\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12REPOSITORY_MISSING\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\x33\n(PERSISTENT_INCONSISTENT_FILESYSTEM_ERROR\x10\x05\x1a\x05\xb2\x43\x02\x08$\x12\x32\n\'TRANSIENT_INCONSISTENT_FILESYSTEM_ERROR\x10\x06\x1a\x05\xb2\x43\x02\x08$\x12\x17\n\x0cINVALID_NAME\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x45VAL_GLOBS_SYMLINK_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1aIMPORT_STARLARK_FILE_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x01\x12\x1a\n\x0fPACKAGE_MISSING\x10\x0b\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0eTARGET_MISSING\x10\x0c\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rNO_SUCH_THING\x10\r\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11GLOB_IO_EXCEPTION\x10\x0e\x1a\x05\xb2\x43\x02\x08$\x12\x1a\n\x0f\x44UPLICATE_LABEL\x10\x0f\x1a\x05\xb2\x43\x02\x08\x01\x12(\n\x1dINVALID_PACKAGE_SPECIFICATION\x10\x10\x1a\x05\xb2\x43\x02\x08\x01\x12\x17\n\x0cSYNTAX_ERROR\x10\x11\x1a\x05\xb2\x43\x02\x08\x01\x12+\n ENVIRONMENT_IN_DIFFERENT_PACKAGE\x10\x12\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x44\x45\x46\x41ULT_ENVIRONMENT_UNDECLARED\x10\x13\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1e\x45NVIRONMENT_IN_MULTIPLE_GROUPS\x10\x14\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x45NVIRONMENT_DOES_NOT_EXIST\x10\x15\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13\x45NVIRONMENT_INVALID\x10\x16\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18\x45NVIRONMENT_NOT_IN_GROUP\x10\x17\x1a\x05\xb2\x43\x02\x08\x01\x12\x1f\n\x14PACKAGE_NAME_INVALID\x10\x18\x1a\x05\xb2\x43\x02\x08\x01\x12\x1e\n\x13STARLARK_EVAL_ERROR\x10\x19\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15LICENSE_PARSE_FAILURE\x10\x1a\x1a\x05\xb2\x43\x02\x08\x01\x12&\n\x1b\x44ISTRIBUTIONS_PARSE_FAILURE\x10\x1b\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eLABEL_CROSSES_PACKAGE_BOUNDARY\x10\x1c\x1a\x05\xb2\x43\x02\x08\x01\x12%\n\x1a\x42UILTINS_INJECTION_FAILURE\x10\x1d\x1a\x05\xb2\x43\x02\x08\x01\x12.\n#SYMLINK_CYCLE_OR_INFINITE_EXPANSION\x10\x1e\x1a\x05\xb2\x43\x02\x08\x01\x12\x1d\n\x12OTHER_IO_EXCEPTION\x10\x1f\x1a\x05\xb2\x43\x02\x08$\"\x04\x08\x08\x10\x08\"\xd4\x02\n\tToolchain\x12-\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1f.failure_details.Toolchain.Code\"\x97\x02\n\x04\x43ode\x12\x1c\n\x11TOOLCHAIN_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MISSING_PROVIDER\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12#\n\x18INVALID_CONSTRAINT_VALUE\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16INVALID_PLATFORM_VALUE\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11INVALID_TOOLCHAIN\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eNO_MATCHING_EXECUTION_PLATFORM\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12 \n\x15NO_MATCHING_TOOLCHAIN\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12!\n\x16INVALID_TOOLCHAIN_TYPE\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\"\x8e\x03\n\x0fStarlarkLoading\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.StarlarkLoading.Code\"\xc5\x02\n\x04\x43ode\x12#\n\x18STARLARK_LOADING_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x10\n\x05\x43YCLE\x10\x01\x1a\x05\xb2\x43\x02\x08\x01\x12\x18\n\rCOMPILE_ERROR\x10\x02\x1a\x05\xb2\x43\x02\x08\x01\x12\x16\n\x0bPARSE_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x01\x12\x15\n\nEVAL_ERROR\x10\x04\x1a\x05\xb2\x43\x02\x08\x01\x12\'\n\x1c\x43ONTAINING_PACKAGE_NOT_FOUND\x10\x05\x1a\x05\xb2\x43\x02\x08\x01\x12\x1c\n\x11PACKAGE_NOT_FOUND\x10\x06\x1a\x05\xb2\x43\x02\x08\x01\x12\x13\n\x08IO_ERROR\x10\x07\x1a\x05\xb2\x43\x02\x08\x01\x12)\n\x1eLABEL_CROSSES_PACKAGE_BOUNDARY\x10\x08\x1a\x05\xb2\x43\x02\x08\x01\x12\x19\n\x0e\x42UILTINS_ERROR\x10\t\x1a\x05\xb2\x43\x02\x08\x01\x12\x1b\n\x10VISIBILITY_ERROR\x10\n\x1a\x05\xb2\x43\x02\x08\x01\"\x8a\x02\n\x0c\x45xternalDeps\x12\x30\n\x04\x63ode\x18\x01 \x01(\x0e\x32\".failure_details.ExternalDeps.Code\"\xc7\x01\n\x04\x43ode\x12 \n\x15\x45XTERNAL_DEPS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10MODULE_NOT_FOUND\x10\x01\x1a\x05\xb2\x43\x02\x08\x30\x12\x15\n\nBAD_MODULE\x10\x02\x1a\x05\xb2\x43\x02\x08\x30\x12#\n\x18VERSION_RESOLUTION_ERROR\x10\x03\x1a\x05\xb2\x43\x02\x08\x30\x12\x1f\n\x14INVALID_REGISTRY_URL\x10\x04\x1a\x05\xb2\x43\x02\x08\x30\x12#\n\x18\x45RROR_ACCESSING_REGISTRY\x10\x05\x1a\x05\xb2\x43\x02\x08 \"\x8a\x01\n\rDiffAwareness\x12\x31\n\x04\x63ode\x18\x01 \x01(\x0e\x32#.failure_details.DiffAwareness.Code\"F\n\x04\x43ode\x12!\n\x16\x44IFF_AWARENESS_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1b\n\x10\x44IFF_STAT_FAILED\x10\x01\x1a\x05\xb2\x43\x02\x08$\"\xcf\x01\n\x0fModqueryCommand\x12\x33\n\x04\x63ode\x18\x01 \x01(\x0e\x32%.failure_details.ModqueryCommand.Code\"\x86\x01\n\x04\x43ode\x12#\n\x18MODQUERY_COMMAND_UNKNOWN\x10\x00\x1a\x05\xb2\x43\x02\x08%\x12\x1c\n\x11MISSING_ARGUMENTS\x10\x01\x1a\x05\xb2\x43\x02\x08\x02\x12\x1d\n\x12TOO_MANY_ARGUMENTS\x10\x02\x1a\x05\xb2\x43\x02\x08\x02\x12\x1c\n\x11INVALID_ARGUMENTS\x10\x03\x1a\x05\xb2\x43\x02\x08\x02:\\\n\x08metadata\x12!.google.protobuf.EnumValueOptions\x18\xb6\x08 \x01(\x0b\x32&.failure_details.FailureDetailMetadataB&\n$com.google.devtools.build.lib.serverb\x06proto3')
 
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.main.protobuf.failure_details_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.EnumValueOptions.RegisterExtension(metadata)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n$com.google.devtools.build.lib.server'
   _INTERRUPTED_CODE.values_by_name["INTERRUPTED_UNKNOWN"]._options = None
   _INTERRUPTED_CODE.values_by_name["INTERRUPTED_UNKNOWN"]._serialized_options = b'\262C\002\010\010'
@@ -670,20 +94,24 @@
   _SPAWN_CODE.values_by_name["INVALID_REMOTE_EXECUTION_PROPERTIES"]._serialized_options = b'\262C\002\010\001'
   _SPAWN_CODE.values_by_name["NO_USABLE_STRATEGY_FOUND"]._options = None
   _SPAWN_CODE.values_by_name["NO_USABLE_STRATEGY_FOUND"]._serialized_options = b'\262C\002\010\001'
   _SPAWN_CODE.values_by_name["UNSPECIFIED_EXECUTION_FAILURE"]._options = None
   _SPAWN_CODE.values_by_name["UNSPECIFIED_EXECUTION_FAILURE"]._serialized_options = b'\262C\002\010\001'
   _SPAWN_CODE.values_by_name["FORBIDDEN_INPUT"]._options = None
   _SPAWN_CODE.values_by_name["FORBIDDEN_INPUT"]._serialized_options = b'\262C\002\010\001'
+  _SPAWN_CODE.values_by_name["REMOTE_CACHE_EVICTED"]._options = None
+  _SPAWN_CODE.values_by_name["REMOTE_CACHE_EVICTED"]._serialized_options = b'\262C\002\010\''
   _EXTERNALREPOSITORY_CODE.values_by_name["EXTERNAL_REPOSITORY_UNKNOWN"]._options = None
   _EXTERNALREPOSITORY_CODE.values_by_name["EXTERNAL_REPOSITORY_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _EXTERNALREPOSITORY_CODE.values_by_name["OVERRIDE_DISALLOWED_MANAGED_DIRECTORIES"]._options = None
   _EXTERNALREPOSITORY_CODE.values_by_name["OVERRIDE_DISALLOWED_MANAGED_DIRECTORIES"]._serialized_options = b'\262C\002\010\002'
   _EXTERNALREPOSITORY_CODE.values_by_name["BAD_DOWNLOADER_CONFIG"]._options = None
   _EXTERNALREPOSITORY_CODE.values_by_name["BAD_DOWNLOADER_CONFIG"]._serialized_options = b'\262C\002\010\002'
+  _EXTERNALREPOSITORY_CODE.values_by_name["REPOSITORY_MAPPING_RESOLUTION_FAILED"]._options = None
+  _EXTERNALREPOSITORY_CODE.values_by_name["REPOSITORY_MAPPING_RESOLUTION_FAILED"]._serialized_options = b'\262C\002\010%'
   _BUILDPROGRESS_CODE.values_by_name["BUILD_PROGRESS_UNKNOWN"]._options = None
   _BUILDPROGRESS_CODE.values_by_name["BUILD_PROGRESS_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _BUILDPROGRESS_CODE.values_by_name["OUTPUT_INITIALIZATION"]._options = None
   _BUILDPROGRESS_CODE.values_by_name["OUTPUT_INITIALIZATION"]._serialized_options = b'\262C\002\010$'
   _BUILDPROGRESS_CODE.values_by_name["BES_RUNS_PER_TEST_LIMIT_UNSUPPORTED"]._options = None
   _BUILDPROGRESS_CODE.values_by_name["BES_RUNS_PER_TEST_LIMIT_UNSUPPORTED"]._serialized_options = b'\262C\002\010\002'
   _BUILDPROGRESS_CODE.values_by_name["BES_LOCAL_WRITE_ERROR"]._options = None
@@ -738,14 +166,20 @@
   _SYMLINKFOREST_CODE.values_by_name["SYMLINK_FOREST_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _SYMLINKFOREST_CODE.values_by_name["TOPLEVEL_OUTDIR_PACKAGE_PATH_CONFLICT"]._options = None
   _SYMLINKFOREST_CODE.values_by_name["TOPLEVEL_OUTDIR_PACKAGE_PATH_CONFLICT"]._serialized_options = b'\262C\002\010\002'
   _SYMLINKFOREST_CODE.values_by_name["TOPLEVEL_OUTDIR_USED_AS_SOURCE"]._options = None
   _SYMLINKFOREST_CODE.values_by_name["TOPLEVEL_OUTDIR_USED_AS_SOURCE"]._serialized_options = b'\262C\002\010\002'
   _SYMLINKFOREST_CODE.values_by_name["CREATION_FAILED"]._options = None
   _SYMLINKFOREST_CODE.values_by_name["CREATION_FAILED"]._serialized_options = b'\262C\002\010\002'
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_UNKNOWN"]._options = None
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_UNKNOWN"]._serialized_options = b'\262C\002\010%'
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_UPLOADER_NEEDS_PACKAGE_PATHS"]._options = None
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_UPLOADER_NEEDS_PACKAGE_PATHS"]._serialized_options = b'\262C\002\010$'
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_WRITE_FAILED"]._options = None
+  _BUILDREPORT_CODE.values_by_name["BUILD_REPORT_WRITE_FAILED"]._serialized_options = b'\262C\002\010$'
   _PACKAGEOPTIONS_CODE.values_by_name["PACKAGE_OPTIONS_UNKNOWN"]._options = None
   _PACKAGEOPTIONS_CODE.values_by_name["PACKAGE_OPTIONS_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _PACKAGEOPTIONS_CODE.values_by_name["PACKAGE_PATH_INVALID"]._options = None
   _PACKAGEOPTIONS_CODE.values_by_name["PACKAGE_PATH_INVALID"]._serialized_options = b'\262C\002\010\002'
   _REMOTEEXECUTION_CODE.values_by_name["REMOTE_EXECUTION_UNKNOWN"]._options = None
   _REMOTEEXECUTION_CODE.values_by_name["REMOTE_EXECUTION_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _REMOTEEXECUTION_CODE.values_by_name["CAPABILITIES_QUERY_FAILURE"]._options = None
@@ -974,16 +408,16 @@
   _INFOCOMMAND_CODE.values_by_name["INFO_BLOCK_WRITE_FAILURE"]._serialized_options = b'\262C\002\010\007'
   _INFOCOMMAND_CODE.values_by_name["ALL_INFO_WRITE_FAILURE"]._options = None
   _INFOCOMMAND_CODE.values_by_name["ALL_INFO_WRITE_FAILURE"]._serialized_options = b'\262C\002\010$'
   _MEMORYOPTIONS_CODE.values_by_name["MEMORY_OPTIONS_UNKNOWN"]._options = None
   _MEMORYOPTIONS_CODE.values_by_name["MEMORY_OPTIONS_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _MEMORYOPTIONS_CODE.values_by_name["EXPERIMENTAL_OOM_MORE_EAGERLY_THRESHOLD_INVALID_VALUE"]._options = None
   _MEMORYOPTIONS_CODE.values_by_name["EXPERIMENTAL_OOM_MORE_EAGERLY_THRESHOLD_INVALID_VALUE"]._serialized_options = b'\262C\002\010\002'
-  _MEMORYOPTIONS_CODE.values_by_name["EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND"]._options = None
-  _MEMORYOPTIONS_CODE.values_by_name["EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND"]._serialized_options = b'\262C\002\010\002'
+  _MEMORYOPTIONS_CODE.values_by_name["DEPRECATED_EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND"]._options = None
+  _MEMORYOPTIONS_CODE.values_by_name["DEPRECATED_EXPERIMENTAL_OOM_MORE_EAGERLY_NO_TENURED_COLLECTORS_FOUND"]._serialized_options = b'\010\001\262C\002\010\002'
   _QUERY_CODE.values_by_name["QUERY_UNKNOWN"]._options = None
   _QUERY_CODE.values_by_name["QUERY_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _QUERY_CODE.values_by_name["QUERY_FILE_WITH_COMMAND_LINE_EXPRESSION"]._options = None
   _QUERY_CODE.values_by_name["QUERY_FILE_WITH_COMMAND_LINE_EXPRESSION"]._serialized_options = b'\262C\002\010\002'
   _QUERY_CODE.values_by_name["QUERY_FILE_READ_FAILURE"]._options = None
   _QUERY_CODE.values_by_name["QUERY_FILE_READ_FAILURE"]._serialized_options = b'\262C\002\010\002'
   _QUERY_CODE.values_by_name["COMMAND_LINE_EXPRESSION_MISSING"]._options = None
@@ -1538,14 +972,16 @@
   _ANALYSIS_CODE.values_by_name["INVALID_EXECUTION_PLATFORM"]._serialized_options = b'\262C\002\010\001'
   _ANALYSIS_CODE.values_by_name["ASPECT_CREATION_FAILED"]._options = None
   _ANALYSIS_CODE.values_by_name["ASPECT_CREATION_FAILED"]._serialized_options = b'\262C\002\010\001'
   _ANALYSIS_CODE.values_by_name["CONFIGURED_VALUE_CREATION_FAILED"]._options = None
   _ANALYSIS_CODE.values_by_name["CONFIGURED_VALUE_CREATION_FAILED"]._serialized_options = b'\262C\002\010\001'
   _ANALYSIS_CODE.values_by_name["INCOMPATIBLE_TARGET_REQUESTED"]._options = None
   _ANALYSIS_CODE.values_by_name["INCOMPATIBLE_TARGET_REQUESTED"]._serialized_options = b'\262C\002\010\001'
+  _ANALYSIS_CODE.values_by_name["ANALYSIS_FAILURE_PROPAGATION_FAILED"]._options = None
+  _ANALYSIS_CODE.values_by_name["ANALYSIS_FAILURE_PROPAGATION_FAILED"]._serialized_options = b'\262C\002\010\001'
   _PACKAGELOADING_CODE.values_by_name["PACKAGE_LOADING_UNKNOWN"]._options = None
   _PACKAGELOADING_CODE.values_by_name["PACKAGE_LOADING_UNKNOWN"]._serialized_options = b'\262C\002\010%'
   _PACKAGELOADING_CODE.values_by_name["WORKSPACE_FILE_ERROR"]._options = None
   _PACKAGELOADING_CODE.values_by_name["WORKSPACE_FILE_ERROR"]._serialized_options = b'\262C\002\010\001'
   _PACKAGELOADING_CODE.values_by_name["MAX_COMPUTATION_STEPS_EXCEEDED"]._options = None
   _PACKAGELOADING_CODE.values_by_name["MAX_COMPUTATION_STEPS_EXCEEDED"]._serialized_options = b'\262C\002\010\001'
   _PACKAGELOADING_CODE.values_by_name["BUILD_FILE_MISSING"]._options = None
@@ -1665,255 +1101,259 @@
   _MODQUERYCOMMAND_CODE.values_by_name["TOO_MANY_ARGUMENTS"]._options = None
   _MODQUERYCOMMAND_CODE.values_by_name["TOO_MANY_ARGUMENTS"]._serialized_options = b'\262C\002\010\002'
   _MODQUERYCOMMAND_CODE.values_by_name["INVALID_ARGUMENTS"]._options = None
   _MODQUERYCOMMAND_CODE.values_by_name["INVALID_ARGUMENTS"]._serialized_options = b'\262C\002\010\002'
   _FAILUREDETAILMETADATA._serialized_start=94
   _FAILUREDETAILMETADATA._serialized_end=136
   _FAILUREDETAIL._serialized_start=139
-  _FAILUREDETAIL._serialized_end=3765
-  _INTERRUPTED._serialized_start=3768
-  _INTERRUPTED._serialized_end=4442
-  _INTERRUPTED_CODE._serialized_start=3833
-  _INTERRUPTED_CODE._serialized_end=4442
-  _SPAWN._serialized_start=4445
-  _SPAWN._serialized_end=4995
-  _SPAWN_CODE._serialized_start=4545
-  _SPAWN_CODE._serialized_end=4995
-  _EXTERNALREPOSITORY._serialized_start=4998
-  _EXTERNALREPOSITORY._serialized_end=5209
-  _EXTERNALREPOSITORY_CODE._serialized_start=5077
-  _EXTERNALREPOSITORY_CODE._serialized_end=5209
-  _BUILDPROGRESS._serialized_start=5212
-  _BUILDPROGRESS._serialized_end=6019
-  _BUILDPROGRESS_CODE._serialized_start=5281
-  _BUILDPROGRESS_CODE._serialized_end=6019
-  _REMOTEOPTIONS._serialized_start=6022
-  _REMOTEOPTIONS._serialized_end=6345
-  _REMOTEOPTIONS_CODE._serialized_start=6091
-  _REMOTEOPTIONS_CODE._serialized_end=6345
-  _CLIENTENVIRONMENT._serialized_start=6348
-  _CLIENTENVIRONMENT._serialized_end=6502
-  _CLIENTENVIRONMENT_CODE._serialized_start=6424
-  _CLIENTENVIRONMENT_CODE._serialized_end=6502
-  _CRASH._serialized_start=6505
-  _CRASH._serialized_end=6655
-  _CRASH_CODE._serialized_start=6601
-  _CRASH_CODE._serialized_end=6655
-  _THROWABLE._serialized_start=6657
-  _THROWABLE._serialized_end=6731
-  _SYMLINKFOREST._serialized_start=6734
-  _SYMLINKFOREST._serialized_end=6965
-  _SYMLINKFOREST_CODE._serialized_start=6803
-  _SYMLINKFOREST_CODE._serialized_end=6965
-  _PACKAGEOPTIONS._serialized_start=6968
-  _PACKAGEOPTIONS._serialized_end=7125
-  _PACKAGEOPTIONS_CODE._serialized_start=7038
-  _PACKAGEOPTIONS_CODE._serialized_end=7125
-  _REMOTEEXECUTION._serialized_start=7128
-  _REMOTEEXECUTION._serialized_end=7947
-  _REMOTEEXECUTION_CODE._serialized_start=7201
-  _REMOTEEXECUTION_CODE._serialized_end=7947
-  _EXECUTION._serialized_start=7950
-  _EXECUTION._serialized_end=9702
-  _EXECUTION_CODE._serialized_start=8011
-  _EXECUTION_CODE._serialized_end=9702
-  _WORKSPACES._serialized_start=9705
-  _WORKSPACES._serialized_end=10029
-  _WORKSPACES_CODE._serialized_start=9768
-  _WORKSPACES_CODE._serialized_end=10029
-  _CRASHOPTIONS._serialized_start=10031
-  _CRASHOPTIONS._serialized_end=10143
-  _CRASHOPTIONS_CODE._serialized_start=10097
-  _CRASHOPTIONS_CODE._serialized_end=10143
-  _FILESYSTEM._serialized_start=10146
-  _FILESYSTEM._serialized_end=10452
-  _FILESYSTEM_CODE._serialized_start=10209
-  _FILESYSTEM_CODE._serialized_end=10452
-  _EXECUTIONOPTIONS._serialized_start=10455
-  _EXECUTIONOPTIONS._serialized_end=10945
-  _EXECUTIONOPTIONS_CODE._serialized_start=10530
-  _EXECUTIONOPTIONS_CODE._serialized_end=10945
-  _COMMAND._serialized_start=10948
-  _COMMAND._serialized_end=11610
-  _COMMAND_CODE._serialized_start=11005
-  _COMMAND_CODE._serialized_end=11610
-  _GRPCSERVER._serialized_start=11613
-  _GRPCSERVER._serialized_end=11849
-  _GRPCSERVER_CODE._serialized_start=11676
-  _GRPCSERVER_CODE._serialized_end=11849
-  _CANONICALIZEFLAGS._serialized_start=11852
-  _CANONICALIZEFLAGS._serialized_end=12005
-  _CANONICALIZEFLAGS_CODE._serialized_start=11928
-  _CANONICALIZEFLAGS_CODE._serialized_end=12005
-  _BUILDCONFIGURATION._serialized_start=12008
-  _BUILDCONFIGURATION._serialized_end=12586
-  _BUILDCONFIGURATION_CODE._serialized_start=12087
-  _BUILDCONFIGURATION_CODE._serialized_end=12586
-  _INFOCOMMAND._serialized_start=12589
-  _INFOCOMMAND._serialized_end=12822
-  _INFOCOMMAND_CODE._serialized_start=12654
-  _INFOCOMMAND_CODE._serialized_end=12822
-  _MEMORYOPTIONS._serialized_start=12825
-  _MEMORYOPTIONS._serialized_end=13071
-  _MEMORYOPTIONS_CODE._serialized_start=12894
-  _MEMORYOPTIONS_CODE._serialized_end=13071
-  _QUERY._serialized_start=13074
-  _QUERY._serialized_end=14596
-  _QUERY_CODE._serialized_start=13127
-  _QUERY_CODE._serialized_end=14596
-  _LOCALEXECUTION._serialized_start=14599
-  _LOCALEXECUTION._serialized_end=14752
-  _LOCALEXECUTION_CODE._serialized_start=14669
-  _LOCALEXECUTION_CODE._serialized_end=14752
-  _ACTIONCACHE._serialized_start=14755
-  _ACTIONCACHE._serialized_end=14893
-  _ACTIONCACHE_CODE._serialized_start=14819
-  _ACTIONCACHE_CODE._serialized_end=14893
-  _FETCHCOMMAND._serialized_start=14896
-  _FETCHCOMMAND._serialized_end=15127
-  _FETCHCOMMAND_CODE._serialized_start=14963
-  _FETCHCOMMAND_CODE._serialized_end=15127
-  _SYNCCOMMAND._serialized_start=15130
-  _SYNCCOMMAND._serialized_end=15378
-  _SYNCCOMMAND_CODE._serialized_start=15195
-  _SYNCCOMMAND_CODE._serialized_end=15378
-  _SANDBOX._serialized_start=15381
-  _SANDBOX._serialized_end=15888
-  _SANDBOX_CODE._serialized_start=15438
-  _SANDBOX_CODE._serialized_end=15888
-  _INCLUDESCANNING._serialized_start=15891
-  _INCLUDESCANNING._serialized_end=16432
-  _INCLUDESCANNING_CODE._serialized_start=16032
-  _INCLUDESCANNING_CODE._serialized_end=16432
-  _TESTCOMMAND._serialized_start=16435
-  _TESTCOMMAND._serialized_end=16623
-  _TESTCOMMAND_CODE._serialized_start=16499
-  _TESTCOMMAND_CODE._serialized_end=16623
-  _ACTIONQUERY._serialized_start=16626
-  _ACTIONQUERY._serialized_end=17304
-  _ACTIONQUERY_CODE._serialized_start=16691
-  _ACTIONQUERY_CODE._serialized_end=17304
-  _TARGETPATTERNS._serialized_start=17307
-  _TARGETPATTERNS._serialized_end=18162
-  _TARGETPATTERNS_CODE._serialized_start=17378
-  _TARGETPATTERNS_CODE._serialized_end=18162
-  _CLEANCOMMAND._serialized_start=18165
-  _CLEANCOMMAND._serialized_end=18666
-  _CLEANCOMMAND_CODE._serialized_start=18232
-  _CLEANCOMMAND_CODE._serialized_end=18666
-  _CONFIGCOMMAND._serialized_start=18669
-  _CONFIGCOMMAND._serialized_end=18846
-  _CONFIGCOMMAND_CODE._serialized_start=18737
-  _CONFIGCOMMAND_CODE._serialized_end=18846
-  _CONFIGURABLEQUERY._serialized_start=18849
-  _CONFIGURABLEQUERY._serialized_end=19420
-  _CONFIGURABLEQUERY_CODE._serialized_start=18926
-  _CONFIGURABLEQUERY_CODE._serialized_end=19420
-  _DUMPCOMMAND._serialized_start=19423
-  _DUMPCOMMAND._serialized_end=19720
-  _DUMPCOMMAND_CODE._serialized_start=19488
-  _DUMPCOMMAND_CODE._serialized_end=19720
-  _HELPCOMMAND._serialized_start=19723
-  _HELPCOMMAND._serialized_end=19885
-  _HELPCOMMAND_CODE._serialized_start=19787
-  _HELPCOMMAND_CODE._serialized_end=19885
-  _MOBILEINSTALL._serialized_start=19888
-  _MOBILEINSTALL._serialized_end=20193
-  _MOBILEINSTALL_CODE._serialized_start=19957
-  _MOBILEINSTALL_CODE._serialized_end=20193
-  _PROFILECOMMAND._serialized_start=20196
-  _PROFILECOMMAND._serialized_end=20380
-  _PROFILECOMMAND_CODE._serialized_start=20266
-  _PROFILECOMMAND_CODE._serialized_end=20380
-  _RUNCOMMAND._serialized_start=20383
-  _RUNCOMMAND._serialized_end=21093
-  _RUNCOMMAND_CODE._serialized_start=20446
-  _RUNCOMMAND_CODE._serialized_end=21093
-  _VERSIONCOMMAND._serialized_start=21096
-  _VERSIONCOMMAND._serialized_end=21234
-  _VERSIONCOMMAND_CODE._serialized_start=21166
-  _VERSIONCOMMAND_CODE._serialized_end=21234
-  _PRINTACTIONCOMMAND._serialized_start=21237
-  _PRINTACTIONCOMMAND._serialized_end=21501
-  _PRINTACTIONCOMMAND_CODE._serialized_start=21316
-  _PRINTACTIONCOMMAND_CODE._serialized_end=21501
-  _WORKSPACESTATUS._serialized_start=21504
-  _WORKSPACESTATUS._serialized_end=21832
-  _WORKSPACESTATUS_CODE._serialized_start=21577
-  _WORKSPACESTATUS_CODE._serialized_end=21832
-  _JAVACOMPILE._serialized_start=21835
-  _JAVACOMPILE._serialized_end=22111
-  _JAVACOMPILE_CODE._serialized_start=21900
-  _JAVACOMPILE_CODE._serialized_end=22111
-  _ACTIONREWINDING._serialized_start=22114
-  _ACTIONREWINDING._serialized_end=22300
-  _ACTIONREWINDING_CODE._serialized_start=22186
-  _ACTIONREWINDING_CODE._serialized_end=22300
-  _CPPCOMPILE._serialized_start=22303
-  _CPPCOMPILE._serialized_end=22828
-  _CPPCOMPILE_CODE._serialized_start=22366
-  _CPPCOMPILE_CODE._serialized_end=22828
-  _STARLARKACTION._serialized_start=22831
-  _STARLARKACTION._serialized_end=23032
-  _STARLARKACTION_CODE._serialized_start=22902
-  _STARLARKACTION_CODE._serialized_end=23032
-  _NINJAACTION._serialized_start=23035
-  _NINJAACTION._serialized_end=23219
-  _NINJAACTION_CODE._serialized_start=23099
-  _NINJAACTION_CODE._serialized_end=23219
-  _DYNAMICEXECUTION._serialized_start=23222
-  _DYNAMICEXECUTION._serialized_end=23477
-  _DYNAMICEXECUTION_CODE._serialized_start=23297
-  _DYNAMICEXECUTION_CODE._serialized_end=23477
-  _FAILACTION._serialized_start=23480
-  _FAILACTION._serialized_end=23882
-  _FAILACTION_CODE._serialized_start=23543
-  _FAILACTION_CODE._serialized_end=23882
-  _SYMLINKACTION._serialized_start=23885
-  _SYMLINKACTION._serialized_end=24192
-  _SYMLINKACTION_CODE._serialized_start=23954
-  _SYMLINKACTION_CODE._serialized_end=24192
-  _CPPLINK._serialized_start=24195
-  _CPPLINK._serialized_end=24369
-  _CPPLINK_CODE._serialized_start=24251
-  _CPPLINK_CODE._serialized_end=24369
-  _LTOACTION._serialized_start=24372
-  _LTOACTION._serialized_end=24587
-  _LTOACTION_CODE._serialized_start=24433
-  _LTOACTION_CODE._serialized_end=24587
-  _TESTACTION._serialized_start=24590
-  _TESTACTION._serialized_end=24868
-  _TESTACTION_CODE._serialized_start=24653
-  _TESTACTION_CODE._serialized_end=24868
-  _WORKER._serialized_start=24871
-  _WORKER._serialized_end=25368
-  _WORKER_CODE._serialized_start=24926
-  _WORKER_CODE._serialized_end=25368
-  _ANALYSIS._serialized_start=25371
-  _ANALYSIS._serialized_end=26153
-  _ANALYSIS_CODE._serialized_start=25430
-  _ANALYSIS_CODE._serialized_end=26153
-  _PACKAGELOADING._serialized_start=26156
-  _PACKAGELOADING._serialized_end=27364
-  _PACKAGELOADING_CODE._serialized_start=26227
-  _PACKAGELOADING_CODE._serialized_end=27364
-  _TOOLCHAIN._serialized_start=27367
-  _TOOLCHAIN._serialized_end=27707
-  _TOOLCHAIN_CODE._serialized_start=27428
-  _TOOLCHAIN_CODE._serialized_end=27707
-  _STARLARKLOADING._serialized_start=27710
-  _STARLARKLOADING._serialized_end=28108
-  _STARLARKLOADING_CODE._serialized_start=27783
-  _STARLARKLOADING_CODE._serialized_end=28108
-  _EXTERNALDEPS._serialized_start=28111
-  _EXTERNALDEPS._serialized_end=28377
-  _EXTERNALDEPS_CODE._serialized_start=28178
-  _EXTERNALDEPS_CODE._serialized_end=28377
-  _DIFFAWARENESS._serialized_start=28380
-  _DIFFAWARENESS._serialized_end=28518
-  _DIFFAWARENESS_CODE._serialized_start=28448
-  _DIFFAWARENESS_CODE._serialized_end=28518
-  _MODQUERYCOMMAND._serialized_start=28521
-  _MODQUERYCOMMAND._serialized_end=28728
-  _MODQUERYCOMMAND_CODE._serialized_start=28594
-  _MODQUERYCOMMAND_CODE._serialized_end=28728
+  _FAILUREDETAIL._serialized_end=3820
+  _INTERRUPTED._serialized_start=3823
+  _INTERRUPTED._serialized_end=4497
+  _INTERRUPTED_CODE._serialized_start=3888
+  _INTERRUPTED_CODE._serialized_end=4497
+  _SPAWN._serialized_start=4500
+  _SPAWN._serialized_end=5083
+  _SPAWN_CODE._serialized_start=4600
+  _SPAWN_CODE._serialized_end=5083
+  _EXTERNALREPOSITORY._serialized_start=5086
+  _EXTERNALREPOSITORY._serialized_end=5346
+  _EXTERNALREPOSITORY_CODE._serialized_start=5165
+  _EXTERNALREPOSITORY_CODE._serialized_end=5346
+  _BUILDPROGRESS._serialized_start=5349
+  _BUILDPROGRESS._serialized_end=6156
+  _BUILDPROGRESS_CODE._serialized_start=5418
+  _BUILDPROGRESS_CODE._serialized_end=6156
+  _REMOTEOPTIONS._serialized_start=6159
+  _REMOTEOPTIONS._serialized_end=6482
+  _REMOTEOPTIONS_CODE._serialized_start=6228
+  _REMOTEOPTIONS_CODE._serialized_end=6482
+  _CLIENTENVIRONMENT._serialized_start=6485
+  _CLIENTENVIRONMENT._serialized_end=6639
+  _CLIENTENVIRONMENT_CODE._serialized_start=6561
+  _CLIENTENVIRONMENT_CODE._serialized_end=6639
+  _CRASH._serialized_start=6642
+  _CRASH._serialized_end=6823
+  _CRASH_CODE._serialized_start=6769
+  _CRASH_CODE._serialized_end=6823
+  _THROWABLE._serialized_start=6825
+  _THROWABLE._serialized_end=6899
+  _SYMLINKFOREST._serialized_start=6902
+  _SYMLINKFOREST._serialized_end=7133
+  _SYMLINKFOREST_CODE._serialized_start=6971
+  _SYMLINKFOREST_CODE._serialized_end=7133
+  _BUILDREPORT._serialized_start=7136
+  _BUILDREPORT._serialized_end=7332
+  _BUILDREPORT_CODE._serialized_start=7201
+  _BUILDREPORT_CODE._serialized_end=7332
+  _PACKAGEOPTIONS._serialized_start=7335
+  _PACKAGEOPTIONS._serialized_end=7492
+  _PACKAGEOPTIONS_CODE._serialized_start=7405
+  _PACKAGEOPTIONS_CODE._serialized_end=7492
+  _REMOTEEXECUTION._serialized_start=7495
+  _REMOTEEXECUTION._serialized_end=8314
+  _REMOTEEXECUTION_CODE._serialized_start=7568
+  _REMOTEEXECUTION_CODE._serialized_end=8314
+  _EXECUTION._serialized_start=8317
+  _EXECUTION._serialized_end=10069
+  _EXECUTION_CODE._serialized_start=8378
+  _EXECUTION_CODE._serialized_end=10069
+  _WORKSPACES._serialized_start=10072
+  _WORKSPACES._serialized_end=10396
+  _WORKSPACES_CODE._serialized_start=10135
+  _WORKSPACES_CODE._serialized_end=10396
+  _CRASHOPTIONS._serialized_start=10398
+  _CRASHOPTIONS._serialized_end=10510
+  _CRASHOPTIONS_CODE._serialized_start=10464
+  _CRASHOPTIONS_CODE._serialized_end=10510
+  _FILESYSTEM._serialized_start=10513
+  _FILESYSTEM._serialized_end=10819
+  _FILESYSTEM_CODE._serialized_start=10576
+  _FILESYSTEM_CODE._serialized_end=10819
+  _EXECUTIONOPTIONS._serialized_start=10822
+  _EXECUTIONOPTIONS._serialized_end=11312
+  _EXECUTIONOPTIONS_CODE._serialized_start=10897
+  _EXECUTIONOPTIONS_CODE._serialized_end=11312
+  _COMMAND._serialized_start=11315
+  _COMMAND._serialized_end=11977
+  _COMMAND_CODE._serialized_start=11372
+  _COMMAND_CODE._serialized_end=11977
+  _GRPCSERVER._serialized_start=11980
+  _GRPCSERVER._serialized_end=12216
+  _GRPCSERVER_CODE._serialized_start=12043
+  _GRPCSERVER_CODE._serialized_end=12216
+  _CANONICALIZEFLAGS._serialized_start=12219
+  _CANONICALIZEFLAGS._serialized_end=12372
+  _CANONICALIZEFLAGS_CODE._serialized_start=12295
+  _CANONICALIZEFLAGS_CODE._serialized_end=12372
+  _BUILDCONFIGURATION._serialized_start=12375
+  _BUILDCONFIGURATION._serialized_end=12953
+  _BUILDCONFIGURATION_CODE._serialized_start=12454
+  _BUILDCONFIGURATION_CODE._serialized_end=12953
+  _INFOCOMMAND._serialized_start=12956
+  _INFOCOMMAND._serialized_end=13189
+  _INFOCOMMAND_CODE._serialized_start=13021
+  _INFOCOMMAND_CODE._serialized_end=13189
+  _MEMORYOPTIONS._serialized_start=13192
+  _MEMORYOPTIONS._serialized_end=13451
+  _MEMORYOPTIONS_CODE._serialized_start=13261
+  _MEMORYOPTIONS_CODE._serialized_end=13451
+  _QUERY._serialized_start=13454
+  _QUERY._serialized_end=14976
+  _QUERY_CODE._serialized_start=13507
+  _QUERY_CODE._serialized_end=14976
+  _LOCALEXECUTION._serialized_start=14979
+  _LOCALEXECUTION._serialized_end=15132
+  _LOCALEXECUTION_CODE._serialized_start=15049
+  _LOCALEXECUTION_CODE._serialized_end=15132
+  _ACTIONCACHE._serialized_start=15135
+  _ACTIONCACHE._serialized_end=15273
+  _ACTIONCACHE_CODE._serialized_start=15199
+  _ACTIONCACHE_CODE._serialized_end=15273
+  _FETCHCOMMAND._serialized_start=15276
+  _FETCHCOMMAND._serialized_end=15507
+  _FETCHCOMMAND_CODE._serialized_start=15343
+  _FETCHCOMMAND_CODE._serialized_end=15507
+  _SYNCCOMMAND._serialized_start=15510
+  _SYNCCOMMAND._serialized_end=15758
+  _SYNCCOMMAND_CODE._serialized_start=15575
+  _SYNCCOMMAND_CODE._serialized_end=15758
+  _SANDBOX._serialized_start=15761
+  _SANDBOX._serialized_end=16268
+  _SANDBOX_CODE._serialized_start=15818
+  _SANDBOX_CODE._serialized_end=16268
+  _INCLUDESCANNING._serialized_start=16271
+  _INCLUDESCANNING._serialized_end=16812
+  _INCLUDESCANNING_CODE._serialized_start=16412
+  _INCLUDESCANNING_CODE._serialized_end=16812
+  _TESTCOMMAND._serialized_start=16815
+  _TESTCOMMAND._serialized_end=17003
+  _TESTCOMMAND_CODE._serialized_start=16879
+  _TESTCOMMAND_CODE._serialized_end=17003
+  _ACTIONQUERY._serialized_start=17006
+  _ACTIONQUERY._serialized_end=17684
+  _ACTIONQUERY_CODE._serialized_start=17071
+  _ACTIONQUERY_CODE._serialized_end=17684
+  _TARGETPATTERNS._serialized_start=17687
+  _TARGETPATTERNS._serialized_end=18542
+  _TARGETPATTERNS_CODE._serialized_start=17758
+  _TARGETPATTERNS_CODE._serialized_end=18542
+  _CLEANCOMMAND._serialized_start=18545
+  _CLEANCOMMAND._serialized_end=19046
+  _CLEANCOMMAND_CODE._serialized_start=18612
+  _CLEANCOMMAND_CODE._serialized_end=19046
+  _CONFIGCOMMAND._serialized_start=19049
+  _CONFIGCOMMAND._serialized_end=19226
+  _CONFIGCOMMAND_CODE._serialized_start=19117
+  _CONFIGCOMMAND_CODE._serialized_end=19226
+  _CONFIGURABLEQUERY._serialized_start=19229
+  _CONFIGURABLEQUERY._serialized_end=19800
+  _CONFIGURABLEQUERY_CODE._serialized_start=19306
+  _CONFIGURABLEQUERY_CODE._serialized_end=19800
+  _DUMPCOMMAND._serialized_start=19803
+  _DUMPCOMMAND._serialized_end=20100
+  _DUMPCOMMAND_CODE._serialized_start=19868
+  _DUMPCOMMAND_CODE._serialized_end=20100
+  _HELPCOMMAND._serialized_start=20103
+  _HELPCOMMAND._serialized_end=20265
+  _HELPCOMMAND_CODE._serialized_start=20167
+  _HELPCOMMAND_CODE._serialized_end=20265
+  _MOBILEINSTALL._serialized_start=20268
+  _MOBILEINSTALL._serialized_end=20573
+  _MOBILEINSTALL_CODE._serialized_start=20337
+  _MOBILEINSTALL_CODE._serialized_end=20573
+  _PROFILECOMMAND._serialized_start=20576
+  _PROFILECOMMAND._serialized_end=20760
+  _PROFILECOMMAND_CODE._serialized_start=20646
+  _PROFILECOMMAND_CODE._serialized_end=20760
+  _RUNCOMMAND._serialized_start=20763
+  _RUNCOMMAND._serialized_end=21473
+  _RUNCOMMAND_CODE._serialized_start=20826
+  _RUNCOMMAND_CODE._serialized_end=21473
+  _VERSIONCOMMAND._serialized_start=21476
+  _VERSIONCOMMAND._serialized_end=21614
+  _VERSIONCOMMAND_CODE._serialized_start=21546
+  _VERSIONCOMMAND_CODE._serialized_end=21614
+  _PRINTACTIONCOMMAND._serialized_start=21617
+  _PRINTACTIONCOMMAND._serialized_end=21881
+  _PRINTACTIONCOMMAND_CODE._serialized_start=21696
+  _PRINTACTIONCOMMAND_CODE._serialized_end=21881
+  _WORKSPACESTATUS._serialized_start=21884
+  _WORKSPACESTATUS._serialized_end=22212
+  _WORKSPACESTATUS_CODE._serialized_start=21957
+  _WORKSPACESTATUS_CODE._serialized_end=22212
+  _JAVACOMPILE._serialized_start=22215
+  _JAVACOMPILE._serialized_end=22491
+  _JAVACOMPILE_CODE._serialized_start=22280
+  _JAVACOMPILE_CODE._serialized_end=22491
+  _ACTIONREWINDING._serialized_start=22494
+  _ACTIONREWINDING._serialized_end=22680
+  _ACTIONREWINDING_CODE._serialized_start=22566
+  _ACTIONREWINDING_CODE._serialized_end=22680
+  _CPPCOMPILE._serialized_start=22683
+  _CPPCOMPILE._serialized_end=23208
+  _CPPCOMPILE_CODE._serialized_start=22746
+  _CPPCOMPILE_CODE._serialized_end=23208
+  _STARLARKACTION._serialized_start=23211
+  _STARLARKACTION._serialized_end=23412
+  _STARLARKACTION_CODE._serialized_start=23282
+  _STARLARKACTION_CODE._serialized_end=23412
+  _NINJAACTION._serialized_start=23415
+  _NINJAACTION._serialized_end=23599
+  _NINJAACTION_CODE._serialized_start=23479
+  _NINJAACTION_CODE._serialized_end=23599
+  _DYNAMICEXECUTION._serialized_start=23602
+  _DYNAMICEXECUTION._serialized_end=23857
+  _DYNAMICEXECUTION_CODE._serialized_start=23677
+  _DYNAMICEXECUTION_CODE._serialized_end=23857
+  _FAILACTION._serialized_start=23860
+  _FAILACTION._serialized_end=24262
+  _FAILACTION_CODE._serialized_start=23923
+  _FAILACTION_CODE._serialized_end=24262
+  _SYMLINKACTION._serialized_start=24265
+  _SYMLINKACTION._serialized_end=24572
+  _SYMLINKACTION_CODE._serialized_start=24334
+  _SYMLINKACTION_CODE._serialized_end=24572
+  _CPPLINK._serialized_start=24575
+  _CPPLINK._serialized_end=24749
+  _CPPLINK_CODE._serialized_start=24631
+  _CPPLINK_CODE._serialized_end=24749
+  _LTOACTION._serialized_start=24752
+  _LTOACTION._serialized_end=24967
+  _LTOACTION_CODE._serialized_start=24813
+  _LTOACTION_CODE._serialized_end=24967
+  _TESTACTION._serialized_start=24970
+  _TESTACTION._serialized_end=25248
+  _TESTACTION_CODE._serialized_start=25033
+  _TESTACTION_CODE._serialized_end=25248
+  _WORKER._serialized_start=25251
+  _WORKER._serialized_end=25748
+  _WORKER_CODE._serialized_start=25306
+  _WORKER_CODE._serialized_end=25748
+  _ANALYSIS._serialized_start=25751
+  _ANALYSIS._serialized_end=26581
+  _ANALYSIS_CODE._serialized_start=25810
+  _ANALYSIS_CODE._serialized_end=26581
+  _PACKAGELOADING._serialized_start=26584
+  _PACKAGELOADING._serialized_end=27792
+  _PACKAGELOADING_CODE._serialized_start=26655
+  _PACKAGELOADING_CODE._serialized_end=27792
+  _TOOLCHAIN._serialized_start=27795
+  _TOOLCHAIN._serialized_end=28135
+  _TOOLCHAIN_CODE._serialized_start=27856
+  _TOOLCHAIN_CODE._serialized_end=28135
+  _STARLARKLOADING._serialized_start=28138
+  _STARLARKLOADING._serialized_end=28536
+  _STARLARKLOADING_CODE._serialized_start=28211
+  _STARLARKLOADING_CODE._serialized_end=28536
+  _EXTERNALDEPS._serialized_start=28539
+  _EXTERNALDEPS._serialized_end=28805
+  _EXTERNALDEPS_CODE._serialized_start=28606
+  _EXTERNALDEPS_CODE._serialized_end=28805
+  _DIFFAWARENESS._serialized_start=28808
+  _DIFFAWARENESS._serialized_end=28946
+  _DIFFAWARENESS_CODE._serialized_start=28876
+  _DIFFAWARENESS_CODE._serialized_end=28946
+  _MODQUERYCOMMAND._serialized_start=28949
+  _MODQUERYCOMMAND._serialized_end=29156
+  _MODQUERYCOMMAND_CODE._serialized_start=29022
+  _MODQUERYCOMMAND_CODE._serialized_end=29156
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xmanager-0.3.0/xmanager/generated/option_filters_pb2.py` & `xmanager-0.4.0/xmanager/generated/option_filters_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,56 +13,29 @@
 # limitations under the License.
 
 # pyformat: disable
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # pylint: skip-file
 # source: src/main/protobuf/option_filters.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&src/main/protobuf/option_filters.proto\x12\x07options*\xea\x02\n\x0fOptionEffectTag\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05NO_OP\x10\x01\x12\x1b\n\x17LOSES_INCREMENTAL_STATE\x10\x02\x12\x12\n\x0e\x43HANGES_INPUTS\x10\x03\x12\x13\n\x0f\x41\x46\x46\x45\x43TS_OUTPUTS\x10\x04\x12\x18\n\x14\x42UILD_FILE_SEMANTICS\x10\x05\x12 \n\x1c\x42\x41ZEL_INTERNAL_CONFIGURATION\x10\x06\x12\x18\n\x14LOADING_AND_ANALYSIS\x10\x07\x12\r\n\tEXECUTION\x10\x08\x12\'\n#HOST_MACHINE_RESOURCE_OPTIMIZATIONS\x10\t\x12\x15\n\x11\x45\x41GERNESS_TO_EXIT\x10\n\x12\x14\n\x10\x42\x41ZEL_MONITORING\x10\x0b\x12\x13\n\x0fTERMINAL_OUTPUT\x10\x0c\x12\x18\n\x14\x41\x43TION_COMMAND_LINES\x10\r\x12\x0f\n\x0bTEST_RUNNER\x10\x0e*\xb2\x01\n\x11OptionMetadataTag\x12\x10\n\x0c\x45XPERIMENTAL\x10\x00\x12\x17\n\x13INCOMPATIBLE_CHANGE\x10\x01\x12\x0e\n\nDEPRECATED\x10\x02\x12\n\n\x06HIDDEN\x10\x03\x12\x0c\n\x08INTERNAL\x10\x04\x12\x1b\n\x17\x45XPLICIT_IN_OUTPUT_PATH\x10\x06\"\x04\x08\x05\x10\x05*%TRIGGERED_BY_ALL_INCOMPATIBLE_CHANGESB*\n(com.google.devtools.common.options.protob\x06proto3')
 
-_OPTIONEFFECTTAG = DESCRIPTOR.enum_types_by_name['OptionEffectTag']
-OptionEffectTag = enum_type_wrapper.EnumTypeWrapper(_OPTIONEFFECTTAG)
-_OPTIONMETADATATAG = DESCRIPTOR.enum_types_by_name['OptionMetadataTag']
-OptionMetadataTag = enum_type_wrapper.EnumTypeWrapper(_OPTIONMETADATATAG)
-UNKNOWN = 0
-NO_OP = 1
-LOSES_INCREMENTAL_STATE = 2
-CHANGES_INPUTS = 3
-AFFECTS_OUTPUTS = 4
-BUILD_FILE_SEMANTICS = 5
-BAZEL_INTERNAL_CONFIGURATION = 6
-LOADING_AND_ANALYSIS = 7
-EXECUTION = 8
-HOST_MACHINE_RESOURCE_OPTIMIZATIONS = 9
-EAGERNESS_TO_EXIT = 10
-BAZEL_MONITORING = 11
-TERMINAL_OUTPUT = 12
-ACTION_COMMAND_LINES = 13
-TEST_RUNNER = 14
-EXPERIMENTAL = 0
-INCOMPATIBLE_CHANGE = 1
-DEPRECATED = 2
-HIDDEN = 3
-INTERNAL = 4
-EXPLICIT_IN_OUTPUT_PATH = 6
-
-
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.main.protobuf.option_filters_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n(com.google.devtools.common.options.proto'
   _OPTIONEFFECTTAG._serialized_start=52
   _OPTIONEFFECTTAG._serialized_end=414
   _OPTIONMETADATATAG._serialized_start=417
```

### Comparing `xmanager-0.3.0/xmanager/vizier/vizier_cloud/__init__.py` & `xmanager-0.4.0/xmanager/vizier/vizier_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/vizier/vizier_cloud/study_factory.py` & `xmanager-0.4.0/xmanager/vizier/vizier_cloud/study_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,23 +32,30 @@
   display_name: str
 
   # TODO: Once vertex pyvizier is available, we should replace
   # aip.StudySpec with it.
   # display_name and num_trials_total are supposed to be set into the study
   # config, which is not supported by aip.StudySpec currently. But should be
   # settable when pyvizier.StudyConfig is available.
-  def __init__(self, study_config: aip.StudySpec, num_trials_total: int,
-               display_name: str, location: str) -> None:
+  def __init__(
+      self,
+      study_config: aip.StudySpec,
+      num_trials_total: int,
+      display_name: str,
+      location: str,
+  ) -> None:
     super().__init__()
     self.study_config = study_config
     self.num_trials_total = num_trials_total
     self.display_name = display_name
     self.vz_client = aip.VizierServiceClient(
         client_options=dict(
-            api_endpoint=f'{location}-aiplatform.googleapis.com'))
+            api_endpoint=f'{location}-aiplatform.googleapis.com'
+        )
+    )
 
   @abc.abstractmethod
   def study(self) -> str:
     raise NotImplementedError
 
 
 class NewStudy(StudyFactory):
@@ -57,25 +64,29 @@
   project: str
   location: str
 
   # `num_trials_total` is a required field. Default it to 0 to unbreak the
   # soon-to-deprecate VizierExploration users.
   # `display_name` is optional for user to customize, if not set, XM will
   # set it with experiment information
-  def __init__(self,
-               study_config: aip.StudySpec,
-               num_trials_total: int = 0,
-               display_name: Optional[str] = None,
-               project: Optional[str] = None,
-               location: Optional[str] = None) -> None:
-
+  def __init__(
+      self,
+      study_config: aip.StudySpec,
+      num_trials_total: int = 0,
+      display_name: Optional[str] = None,
+      project: Optional[str] = None,
+      location: Optional[str] = None,
+  ) -> None:
     self.project = project or auth.get_project_name()
     self.location = location or _DEFAULT_LOCATION
 
-    super().__init__(study_config, num_trials_total, display_name or '',
-                     self.location)
+    super().__init__(
+        study_config, num_trials_total, display_name or '', self.location
+    )
 
   def study(self) -> str:
     return self.vz_client.create_study(
         parent=f'projects/{self.project}/locations/{self.location}',
         study=aip.Study(
-            display_name=self.display_name, study_spec=self.study_config)).name
+            display_name=self.display_name, study_spec=self.study_config
+        ),
+    ).name
```

### Comparing `xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_controller.py` & `xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 
 from xmanager import xm
 
 
 class VizierController:
   """A Controller that runs Vizier suggested hyperparameters in multiple work units."""
 
-  def __init__(self, experiment: xm.Experiment,
-               work_unit_generator: Callable[[xm.WorkUnit, Dict[str, Any]],
-                                             Any],
-               vz_client: aip.VizierServiceClient, study_name: str,
-               num_work_units_total: int, num_parallel_work_units: int) -> None:
+  def __init__(
+      self,
+      experiment: xm.Experiment,
+      work_unit_generator: Callable[[xm.WorkUnit, Dict[str, Any]], Any],
+      vz_client: aip.VizierServiceClient,
+      study_name: str,
+      num_work_units_total: int,
+      num_parallel_work_units: int,
+  ) -> None:
     """Create a VizierController.
 
     Args:
       experiment: XM experiment.
       work_unit_generator: the function that generates WorkUnit from
         hyperparameters.
       vz_client: the Vizier Client used for interacting with Vizier.
@@ -59,108 +63,140 @@
         if not work_unit_updater.completed:
           work_unit_updater.check_for_completion()
 
       # 2. TODO: Return by Vizier's indication that study is done
       # when such API is ready on Vizier side.
       num_exisiting_work_units = len(self._work_unit_updaters)
       num_completed_work_units = sum(
-          [wuu.completed for wuu in self._work_unit_updaters])
-      if num_exisiting_work_units == self._num_work_units_total and num_completed_work_units == self._num_work_units_total:
+          [wuu.completed for wuu in self._work_unit_updaters]
+      )
+      if (
+          num_exisiting_work_units == self._num_work_units_total
+          and num_completed_work_units == self._num_work_units_total
+      ):
         print('All done! Exiting VizierController... \n')
         return
 
       # 3. Get new trials and assign to new work units.
       self._launch_new_work_units()
 
       time.sleep(poll_frequency_in_sec)
 
   def _launch_new_work_units(self) -> None:
     """Get hyperparmeter suggestions from Vizier and assign to new work units to run."""
     # 1. Compute num of work units to create next.
     num_existing_work_units = len(self._work_unit_updaters)
-    num_running_work_units = len([
-        wuu for wuu in self._work_unit_updaters
-        if wuu.work_unit_status().is_active
-    ])
-    num_work_units_to_create_total = self._num_work_units_total - num_existing_work_units
+    num_running_work_units = len(
+        [
+            wuu
+            for wuu in self._work_unit_updaters
+            if wuu.work_unit_status().is_active
+        ]
+    )
+    num_work_units_to_create_total = (
+        self._num_work_units_total - num_existing_work_units
+    )
     num_work_units_to_create_next = min(
         self._num_parallel_work_units - num_running_work_units,
-        num_work_units_to_create_total)
+        num_work_units_to_create_total,
+    )
 
     # 2. Create the work units.
     start_index = num_existing_work_units + 1
     for i in range(start_index, start_index + num_work_units_to_create_next):
-      trial = self._vz_client.suggest_trials(
-          request=aip.SuggestTrialsRequest(
-              parent=self._study_name,
-              suggestion_count=1,
-              client_id=f'work unit {i}')).result().trials[0]
+      trial = (
+          self._vz_client.suggest_trials(
+              request=aip.SuggestTrialsRequest(
+                  parent=self._study_name,
+                  suggestion_count=1,
+                  client_id=f'work unit {i}',
+              )
+          )
+          .result()
+          .trials[0]
+      )
       print(f'Trial for work unit (index: {i}) is retrieved：\n{trial}')
 
       print(f'Creating work unit (index: {i})... \n')
 
       def create_gen(index: int, trial: aip.Trial) -> xm.JobGeneratorType:
-
         async def gen_work_unit(work_unit: xm.WorkUnit, **kwargs):
           await self._work_unit_generator(work_unit, kwargs)
 
           # TODO: Add an utility to handle logging conditionally
           # (use print when run local otherwise logging.info.)
-          print(f'Work unit (index: {index}, '
-                f'id: {work_unit.work_unit_id}) created. \n')
+          print(
+              f'Work unit (index: {index}, '
+              f'id: {work_unit.work_unit_id}) created. \n'
+          )
           self._work_unit_updaters.append(
               WorkUnitVizierUpdater(
-                  vz_client=self._vz_client, work_unit=work_unit, trial=trial))
+                  vz_client=self._vz_client, work_unit=work_unit, trial=trial
+              )
+          )
 
         return gen_work_unit
 
       args = {
           'trial_name': trial.name,
-          **{p.parameter_id: p.value for p in trial.parameters}
+          **{p.parameter_id: p.value for p in trial.parameters},
       }
       self._experiment.add(create_gen(i, trial), args)
 
 
 class WorkUnitVizierUpdater:
   """An updater for syncing completion state between work unit and vizier trial."""
 
-  def __init__(self, vz_client: aip.VizierServiceClient, work_unit: xm.WorkUnit,
-               trial: aip.Trial) -> None:
+  def __init__(
+      self,
+      vz_client: aip.VizierServiceClient,
+      work_unit: xm.WorkUnit,
+      trial: aip.Trial,
+  ) -> None:
     self.completed = False
     self._vz_client = vz_client
     self._work_unit = work_unit
     self._trial = trial
 
   def work_unit_status(self) -> xm.ExperimentUnitStatus:
     return self._work_unit.get_status()
 
   def check_for_completion(self) -> None:
     """Sync the completion status between WorkUnit and Vizier Trial if needed."""
     if self.completed:
       return
 
     print(
-        f'Start completion check for work unit {self._work_unit.work_unit_id}.\n'
+        'Start completion check for work unit'
+        f' {self._work_unit.work_unit_id}.\n'
     )
 
     # TODO: Add infeasible_reason when available.
     if not self.work_unit_status().is_active:
       self._complete_trial(self._trial)
       self.completed = True
-    elif self._vz_client.check_trial_early_stopping_state(
-        request=aip.CheckTrialEarlyStoppingStateRequest(
-            trial_name=self._trial.name)).result().should_stop:
+    elif (
+        self._vz_client.check_trial_early_stopping_state(
+            request=aip.CheckTrialEarlyStoppingStateRequest(
+                trial_name=self._trial.name
+            )
+        )
+        .result()
+        .should_stop
+    ):
       print(f'Early stopping work unit {self._work_unit.work_unit_id}.\n')
       self._work_unit.stop()
     else:
       print(f'Work unit {self._work_unit.work_unit_id} is still running.\n')
 
-  def _complete_trial(self,
-                      trial: aip.Trial,
-                      infeasible_reason: Optional[str] = None) -> None:
+  def _complete_trial(
+      self, trial: aip.Trial, infeasible_reason: Optional[str] = None
+  ) -> None:
     """Complete a trial."""
     self._vz_client.complete_trial(
         request=aip.CompleteTrialRequest(
             name=trial.name,
             trial_infeasible=infeasible_reason is not None,
-            infeasible_reason=infeasible_reason))
+            infeasible_reason=infeasible_reason,
+        )
+    )
     print(f'Trial {trial.name} is completed\n')
```

### Comparing `xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_exploration.py` & `xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_exploration.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,35 @@
 _DEFAULT_LOCATION = 'us-central1'
 
 
 # TODO: Add vizier_controller as auxiliary Job generator.
 class VizierExploration:
   """An API for launching experiment as a Vizier-based Exploration."""
 
-  def __init__(self, experiment: xm.Experiment, job: xm.JobType,
-               study_factory: sf.StudyFactory, num_trials_total: int,
-               num_parallel_trial_runs: int) -> None:
+  def __init__(
+      self,
+      experiment: xm.Experiment,
+      job: xm.JobType,
+      study_factory: sf.StudyFactory,
+      num_trials_total: int,
+      num_parallel_trial_runs: int,
+  ) -> None:
     """Create a VizierExploration.
 
     Args:
       experiment: the experiment who does the exploration.
       job: a job to run.
       study_factory: the VizierStudyFactory used to create or load the study.
       num_trials_total: total number of trials the experiment want to explore.
       num_parallel_trial_runs: number of parallel runs evaluating the trials.
     """
 
-    async def work_unit_generator(work_unit: xm.WorkUnit,
-                                  vizier_params: Dict[str, Any]):
+    async def work_unit_generator(
+        work_unit: xm.WorkUnit, vizier_params: Dict[str, Any]
+    ):
       work_unit.add(job, self._to_job_params(vizier_params))
 
     if not study_factory.display_name:
       study_factory.display_name = f'X{experiment.experiment_id}'
 
     self._controller = vizier_controller.VizierController(
         experiment,
```

### Comparing `xmanager-0.3.0/xmanager/vizier/vizier_cloud/vizier_worker.py` & `xmanager-0.4.0/xmanager/vizier/vizier_cloud/vizier_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,48 +14,58 @@
 """Run Job as a Vizier worker to manager WorkUnit Vizier interaction."""
 import re
 from typing import Dict, Optional
 
 from absl import logging
 from google.cloud import aiplatform_v1beta1 as aip
 
-_TRIAL_NAME_REGEX = r'projects\/[^\/]+\/locations\/[^\/]+\/studies\/[^\/]+\/trials\/[^\/]+'
+_TRIAL_NAME_REGEX = (
+    r'projects\/[^\/]+\/locations\/[^\/]+\/studies\/[^\/]+\/trials\/[^\/]+'
+)
 
 
 class VizierWorker:
   """Worker that manage interaction between job and Vizier."""
 
   def __init__(self, trial_name: str) -> None:
     if not re.match(_TRIAL_NAME_REGEX, trial_name):
-      raise Exception('The trial_name must be in the form: '
-                      'projects/{project}/locations/{location}/'
-                      'studies/{study}/trials/{trial}')
+      raise Exception(
+          'The trial_name must be in the form: '
+          'projects/{project}/locations/{location}/'
+          'studies/{study}/trials/{trial}'
+      )
 
     self._trial_name = trial_name
 
     location = trial_name.split('/')[3]
-    self._vz_client = aip.VizierServiceClient(client_options={
-        'api_endpoint': f'{location}-aiplatform.googleapis.com',
-    })
+    self._vz_client = aip.VizierServiceClient(
+        client_options={
+            'api_endpoint': f'{location}-aiplatform.googleapis.com',
+        }
+    )
 
   def add_trial_measurement(self, step: int, metrics: Dict[str, float]) -> None:
     """Add trial measurements to Vizier."""
     self._vz_client.add_trial_measurement(
         request=aip.AddTrialMeasurementRequest(
             trial_name=self._trial_name,
             measurement=aip.Measurement(
                 step_count=step,
                 metrics=[
                     aip.Measurement.Metric(metric_id=k, value=v)
                     for k, v in metrics.items()
                 ],
-            )))
+            ),
+        )
+    )
     logging.info('Step %d Metric %s is reported', step, metrics)
 
   def complete_trial(self, infeasible_reason: Optional[str] = None) -> None:
     """Complete a trial."""
     self._vz_client.complete_trial(
         request=aip.CompleteTrialRequest(
             name=self._trial_name,
             trial_infeasible=infeasible_reason is not None,
-            infeasible_reason=infeasible_reason))
+            infeasible_reason=infeasible_reason,
+        )
+    )
     logging.info('Trial %s is completed', self._trial_name)
```

### Comparing `xmanager-0.3.0/xmanager/xm/__init__.py` & `xmanager-0.4.0/xmanager/xm/__init__.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm/async_packager.py` & `xmanager-0.4.0/xmanager/xm/async_packager.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,86 +12,106 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """An utility to batch Packageables together and build them in one go."""
 
 import asyncio
 import concurrent.futures as concurrent_futures
 import threading
-from typing import Awaitable, Callable, Sequence
+from typing import Awaitable, Callable, Sequence, TypeVar
 
 from xmanager.xm import job_blocks
 
 
 class PackageHasNotBeenCalledError(RuntimeError):
   """Access to package_async() awaitable prior to calling .package()."""
 
 
-def _return_executable(
-    executable: job_blocks.Executable) -> Awaitable[job_blocks.Executable]:
-  """Returns an awaitable for an already known executable."""
-  future = asyncio.Future()
-  future.set_result(executable)
-  return future
+Awaited = TypeVar('Awaited')
+
+
+class PicklableAwaitableImpl:
+  """Awaitable type with known value which can be pickled."""
+
+  def __init__(
+      self,
+      get_future: Callable[
+          [], asyncio.Future[Awaited] | concurrent_futures.Future[Awaited]
+      ],
+  ):
+    self._get_future = get_future
+
+  def __await__(self):
+    return asyncio.wrap_future(self._get_future()).__await__()
+
+  def __reduce__(self):
+    return _return_awaited, (self._get_future().result(),)
+
+
+def _return_awaited(
+    awaited: Awaited,
+) -> Awaitable[Awaited]:
+  """Returns a picklable awaitable for an already known value."""
+
+  def get_future() -> asyncio.Future[Awaited]:
+    future = asyncio.Future()
+    future.set_result(awaited)
+    return future
+
+  return PicklableAwaitableImpl(get_future)
 
 
 class AsyncPackager:
   """An utility to batch Packageables together and build them in one go.
 
   Attributes:
     _lock: A Lock() object used to make the class threadsafe.
     _package_batch: A function which packages a batch of Packageables.
     _packageables: Packageables queued to be packaged.
     _futures: Corresponding futures where packaging results should be written.
   """
 
   def __init__(
-      self, package_batch: Callable[[Sequence[job_blocks.Packageable]],
-                                    Sequence[job_blocks.Executable]]
+      self,
+      package_batch: Callable[
+          [Sequence[job_blocks.Packageable]], Sequence[job_blocks.Executable]
+      ],
   ) -> None:
     """Creates the async packager.
 
     Args:
       package_batch: A function which packages a batch of Packageables.
     """
     super().__init__()
     self._lock = threading.Lock()
     self._package_batch = package_batch
     self._packageables = []
     self._futures = []
 
   def add(
-      self,
-      packageable: job_blocks.Packageable) -> Awaitable[job_blocks.Executable]:
+      self, packageable: job_blocks.Packageable
+  ) -> Awaitable[job_blocks.Executable]:
     """Adds new packageable to the batch."""
     with self._lock:
       future = concurrent_futures.Future()
       self._packageables.append(packageable)
       self._futures.append(future)
 
     def check_is_packaged() -> None:
       with self._lock:
         if packageable in self._packageables:
           raise PackageHasNotBeenCalledError(
               '.package() must be called before awaiting on the packaging '
-              'result')
+              'result'
+          )
 
-    async def package_impl() -> job_blocks.Executable:
+    def get_future() -> concurrent_futures.Future[job_blocks.Executable]:
       check_is_packaged()
-      return await asyncio.wrap_future(future)
-
-    class PicklablePackageImpl:
-
-      def __await__(self):
-        return package_impl().__await__()
-
-      def __reduce__(self):
-        check_is_packaged()
-        return (_return_executable, (future.result(),))
+      return future
 
-    return PicklablePackageImpl()
+    return PicklableAwaitableImpl(get_future)
 
   def package(
       self, extra_packageables: Sequence[job_blocks.Packageable] = ()
   ) -> Sequence[job_blocks.Executable]:
     """Triggers the packaging of previously added packageables.
 
     Args:
@@ -110,12 +130,12 @@
     if not packageables:
       return []
 
     try:
       executables = self._package_batch(packageables)
       for executable, future in zip(executables, futures):
         future.set_result(executable)
-      return executables[len(futures):]
+      return executables[len(futures) :]
     except Exception as e:
       for future in futures:
         future.set_exception(e)
       raise
```

### Comparing `xmanager-0.3.0/xmanager/xm/async_packager_test.py` & `xmanager-0.4.0/xmanager/xm/async_packager_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from xmanager.xm import async_packager
 from xmanager.xm import job_blocks
 from xmanager.xm import utils
 
 
 def _package_batch(
-    packageables: Sequence[job_blocks.Packageable]
+    packageables: Sequence[job_blocks.Packageable],
 ) -> Sequence[job_blocks.Executable]:
   return [
       job_blocks.Executable(name=packageable.executable_spec.name)
       for packageable in packageables
   ]
 
 
@@ -39,15 +39,16 @@
   def name(self) -> str:
     return self._name
 
 
 def _make_packageable(name: str) -> job_blocks.Packageable:
   return job_blocks.Packageable(
       executable_spec=_TestExecutableSpec(name),
-      executor_spec=job_blocks.ExecutorSpec())
+      executor_spec=job_blocks.ExecutorSpec(),
+  )
 
 
 class AsyncPackagerTest(unittest.TestCase):
 
   @utils.run_in_asyncio_loop
   async def test_async_packager_end_to_end(self):
     packager = async_packager.AsyncPackager(_package_batch)
@@ -82,10 +83,19 @@
     # when we requested packaging.
     @utils.run_in_asyncio_loop
     async def wait_for_it():
       await pickle.loads(executable_str)
 
     wait_for_it()
 
+  def test_awaitable_is_repeatedly_picklable(self):
+    packager = async_packager.AsyncPackager(_package_batch)
+    executable = packager.add(_make_packageable(''))
+    packager.package()
+    executable_str = pickle.dumps(executable)
+    executable_reconstructed = pickle.loads(executable_str)
+    executable_str2 = pickle.dumps(executable_reconstructed)
+    self.assertEqual(executable_str, executable_str2)
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `xmanager-0.3.0/xmanager/xm/compute_units.py` & `xmanager-0.4.0/xmanager/xm/compute_units.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm/core.py` & `xmanager-0.4.0/xmanager/xm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,55 +42,66 @@
 from xmanager.xm import job_operators
 from xmanager.xm import metadata_context
 from xmanager.xm import pattern_matching
 
 # ContextVars holding the current experiment (when within an Experiment context)
 # and current experiment unit (when inside a JobGenerator).
 _current_experiment: contextvars.ContextVar['Experiment'] = (
-    contextvars.ContextVar('_xm_current_experiment'))
+    contextvars.ContextVar('_xm_current_experiment')
+)
 _current_experiment_unit: contextvars.ContextVar['ExperimentUnit'] = (
-    contextvars.ContextVar('_xm_current_experiment_unit'))
+    contextvars.ContextVar('_xm_current_experiment_unit')
+)
 
 
-def _check_if_unsupported_args_are_present(args: Mapping[str, Any],
-                                           supported_args: Collection[str],
-                                           job_type: str) -> None:
+def _check_if_unsupported_args_are_present(
+    args: Mapping[str, Any], supported_args: Collection[str], job_type: str
+) -> None:
   supported_args = set(supported_args)
   unsupported_args = set(args.keys()) - supported_args
   if unsupported_args:
     raise ValueError(
         f'Arguments {unsupported_args!r} are not supported by {job_type}. Only '
-        f'{supported_args!r} are allowed.')
+        f'{supported_args!r} are allowed.'
+    )
 
 
 def _apply_args_to_job(job: job_blocks.Job, args: Mapping[str, Any]) -> None:
   """Overrides job properties."""
   _check_if_unsupported_args_are_present(args, ('args', 'env_vars'), 'xm.Job')
 
   if 'args' in args:
     job.args = job_blocks.merge_args(job.args, args['args'])
   if 'env_vars' in args:
     job.env_vars = job.env_vars.copy()
     job.env_vars.update(args['env_vars'])
 
 
-def _apply_args_to_job_group(job_group: job_blocks.JobGroup,
-                             args: Mapping[str, Any]) -> None:
+def _apply_args_to_job_group(
+    job_group: job_blocks.JobGroup, args: Mapping[str, Any]
+) -> None:
   """Recursively overrides job group properties."""
   if args:
-    _check_if_unsupported_args_are_present(args, job_group.jobs.keys(),
-                                           'xm.JobGroup')
+    _check_if_unsupported_args_are_present(
+        args, job_group.jobs.keys(), 'xm.JobGroup'
+    )
     for key, job in job_group.jobs.items():
       _apply_args(job, args.get(key, {}))
 
 
 _apply_args = pattern_matching.match(
-    _apply_args_to_job, _apply_args_to_job_group,
-    pattern_matching.Case([job_blocks.JobGeneratorType, Any],
-                          lambda other, args: None))
+    _apply_args_to_job,
+    _apply_args_to_job_group,
+    pattern_matching.Case(
+        [job_blocks.JobGeneratorType, Any], lambda other, args: None
+    ),
+    pattern_matching.Case(
+        [job_blocks.JobConfig, Any], lambda other, args: None
+    ),
+)
 
 
 class ExperimentUnitStatus(abc.ABC):
   """The status of an experiment unit."""
 
   @property
   @abc.abstractmethod
@@ -139,14 +150,15 @@
 
 class ExperimentUnitError(RuntimeError):
   """Experiment unit could not be completed.
 
   Attrs:
     work_unit: The work unit in which the error occured, if available.
   """
+
   work_unit: Optional['WorkUnit'] = None
 
   def __init__(self, message: Any, *, work_unit: Optional['WorkUnit'] = None):
     super().__init__(message)
     self.work_unit = work_unit
 
 
@@ -193,30 +205,33 @@
     # In order to give users control on what is shown as work unit arguments we
     # don't alter them if a value is given.
     return args
 
   def deduce_args_for_job(job: job_blocks.Job) -> Dict[str, Any]:
     args = {
         'args': job.args.to_dict(kwargs_only=True),
-        'env_vars': job.env_vars
+        'env_vars': job.env_vars,
     }
     return {key: value for key, value in args.items() if value}
 
   def deduce_args_for_job_group(group: job_blocks.JobGroup) -> Dict[str, Any]:
     args = {}
     for job_name, job in group.jobs.items():
       job_args = deduce_args(job)
       if job_args:
         args[job_name] = job_args
     return args
 
   deduce_args = pattern_matching.match(
-      deduce_args_for_job, deduce_args_for_job_group,
-      pattern_matching.Case([job_blocks.JobGeneratorType],
-                            lambda generator: {}))
+      deduce_args_for_job,
+      deduce_args_for_job_group,
+      pattern_matching.Case(
+          [job_blocks.JobGeneratorType], lambda generator: {}
+      ),
+  )
 
   return deduce_args(job)
 
 
 @attr.s(auto_attribs=True, kw_only=True)
 class LaunchedJob:
   """A read-only view of a launched job.
@@ -234,14 +249,15 @@
   launched jobs as the generator adds.
 
   Attributes:
     name: Name of the job corresponding to this launched job.
     address: The job's address.
     logs: A URL to this job's logs.
   """
+
   name: str
   address: Optional[str] = None
   logs: Optional[str] = None
 
 
 class Importance(enum.Enum):
   """How important it is to schedule particular Experiment or ExperimentUnit.
@@ -269,26 +285,30 @@
 class ExperimentUnitRole(abc.ABC):
   """The role of an experiment unit within the experiment structure.
 
   Attributes:
     importance: how important it is to schedule this executable unit comparing
       to all your executable units (from all your experiments).
   """
+
   importance: Importance = Importance.NORMAL
 
 
 class ExperimentUnit(abc.ABC):
   """ExperimentUnit is a collection of semantically associated `Job`s."""
 
   experiment: 'Experiment'
 
-  def __init__(self, experiment: 'Experiment',
-               create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
-               args: Optional[Mapping[str,
-                                      Any]], role: ExperimentUnitRole) -> None:
+  def __init__(
+      self,
+      experiment: 'Experiment',
+      create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
+      args: Optional[Mapping[str, Any]],
+      role: ExperimentUnitRole,
+  ) -> None:
     """Initializes an `ExperimentUnit` instance.
 
     Args:
       experiment: An experiment this unit belongs to.
       create_task: A callback to register a new asynchronous task.
       args: Arguments to this experiment unit. Most commonly used to represent
         the hyperparameter sweep trial corresponding to a work unit.
@@ -302,19 +322,21 @@
     self._launch_tasks: List[futures.Future[Any]] = []
 
   @property
   def experiment_id(self) -> int:
     """Returns a unique ID assigned to the experiment."""
     return self.experiment.experiment_id
 
-  def add(self,
-          job: job_blocks.JobType,
-          args: Optional[Mapping[str, Any]] = None,
-          *,
-          identity: str = '') -> Awaitable[None]:
+  def add(
+      self,
+      job: job_blocks.JobType,
+      args: Optional[Mapping[str, Any]] = None,
+      *,
+      identity: str = '',
+  ) -> Awaitable[None]:
     # pyformat: disable
     """Adds a Job / JobGroup to the experiment unit.
 
     Only one JobGroup can be added to an ExperimentUnit. This limitation may be
     lifted in future versions.
 
     Args:
@@ -343,30 +365,35 @@
     job_operators.populate_job_names(job)
 
     def launch_job(job: job_blocks.Job) -> Awaitable[None]:
       _current_experiment.set(self.experiment)
       _current_experiment_unit.set(self)
       return self._launch_job_group(
           job_blocks.JobGroup(**{job.name: job}),
-          _work_unit_arguments(job, self._args), identity)
+          _work_unit_arguments(job, self._args),
+          identity,
+      )
 
     def launch_job_group(group: job_blocks.JobGroup) -> Awaitable[None]:
       _current_experiment.set(self.experiment)
       _current_experiment_unit.set(self)
-      return self._launch_job_group(group,
-                                    _work_unit_arguments(group, self._args),
-                                    identity)
+      return self._launch_job_group(
+          group, _work_unit_arguments(group, self._args), identity
+      )
 
     def launch_job_generator(
-        job_generator: job_blocks.JobGeneratorType) -> Awaitable[None]:
-      if (not inspect.iscoroutinefunction(job_generator) and
-          not inspect.iscoroutinefunction(job_generator.__call__)):
+        job_generator: job_blocks.JobGeneratorType,
+    ) -> Awaitable[None]:
+      if not inspect.iscoroutinefunction(
+          job_generator
+      ) and not inspect.iscoroutinefunction(job_generator.__call__):
         raise ValueError(
             'Job generator must be an async function. Signature needs to be '
-            '`async def job_generator(work_unit: xm.WorkUnit) -> None:`')
+            '`async def job_generator(work_unit: xm.WorkUnit) -> None:`'
+        )
       _current_experiment.set(self.experiment)
       _current_experiment_unit.set(self)
       coroutine = job_generator(self, **(args or {}))
       assert coroutine is not None
       return coroutine
 
     def launch_job_config(job_config: job_blocks.JobConfig) -> Awaitable[None]:
@@ -375,16 +402,15 @@
       return self._launch_job_config(job_config, args or {}, identity)
 
     job_awaitable = pattern_matching.match(
         launch_job,
         launch_job_group,
         launch_job_generator,
         launch_job_config,
-    )(
-        job)
+    )(job)
     launch_task = self._create_task(job_awaitable)
     self._launch_tasks.append(launch_task)
     return asyncio.wrap_future(launch_task)
 
   async def _wait_until_complete_impl(self) -> 'ExperimentUnit':
     try:
       for task in self._launch_tasks:
@@ -429,19 +455,21 @@
 
     Unlike wait_until_complete this method asumes that unit has been fully
     created. This method is only invoked if somebody has requested to monitor
     unit.
     """
     raise NotImplementedError
 
-  def stop(self,
-           *,
-           mark_as_failed: bool = False,
-           mark_as_completed: bool = False,
-           message: Optional[str] = None) -> None:
+  def stop(
+      self,
+      *,
+      mark_as_failed: bool = False,
+      mark_as_completed: bool = False,
+      message: Optional[str] = None,
+  ) -> None:
     """Initiate the process to stop the unit from running.
 
     This method will synchronously make a request for the unit to stop.
     However, the method does not actually wait for the unit to be in a
     terminal state.
 
     Use self.wait_until_complete() after self.stop() to guarantee the unit
@@ -478,15 +506,16 @@
     return f'{self.experiment_unit_name}_{job_name}'
 
   @property
   def context(self) -> metadata_context.MetadataContext:
     """Returns metadata context for a unit."""
     return metadata_context.MetadataContext(
         creator=getpass.getuser(),
-        annotations=metadata_context.ContextAnnotations())
+        annotations=metadata_context.ContextAnnotations(),
+    )
 
   @property
   def launched_jobs(self) -> List[LaunchedJob]:
     """Gets a representation for each individual job that was added.
 
     Each added Job should produce a LaunchedJob.
     Each added JobGroup will produce a LaunchedJob for each leaf Job.
@@ -517,16 +546,17 @@
         try:
           await event
           print(f'Wor unit {wid} completed successfully.')
         except xm.ExperimentUnitError as e:
           print(f'Wor unit {wid} failed: {e}.')
   """
 
-  def __init__(self, work_unit: 'WorkUnit', awaitable: Callable[[],
-                                                                Any]) -> None:
+  def __init__(
+      self, work_unit: 'WorkUnit', awaitable: Callable[[], Any]
+  ) -> None:
     self.work_unit = work_unit
     self._awaitable = awaitable
     self._wait_coro = self._wait()
 
   async def _wait(self) -> 'WorkUnit':
     # Coroutine must be created inside of async function to avoid
     # "coroutine ... was never awaited" runtime warning.
@@ -588,29 +618,32 @@
   result in AUX units once added to the expetiment.
   Note that this class conforms to xm.JobGenerator interface.
   """
 
   role: AuxiliaryUnitRole
   _job: job_blocks.JobType
 
-  def __init__(self,
-               job: job_blocks.JobType,
-               *,
-               importance: Importance = Importance.NORMAL,
-               termination_delay_secs: int) -> None:
+  def __init__(
+      self,
+      job: job_blocks.JobType,
+      *,
+      importance: Importance = Importance.NORMAL,
+      termination_delay_secs: int,
+  ) -> None:
     self.role = AuxiliaryUnitRole(
         importance=importance,
         termination_delay_secs=termination_delay_secs,
     )
     self._job = job
 
   async def __call__(self, aux_unit: ExperimentUnit, **kwargs):
 
     async def launch_generator(
-        job_generator: job_blocks.JobGeneratorType) -> None:
+        job_generator: job_blocks.JobGeneratorType,
+    ) -> None:
       coroutine = job_generator(aux_unit, **kwargs)
       assert coroutine is not None
       await coroutine
 
     async def launch_job(job: Any) -> None:
       aux_unit.add(job, args=kwargs)
 
@@ -663,54 +696,67 @@
     is_coro_context = False
     try:
       asyncio.get_running_loop()
       is_coro_context = True
     except RuntimeError:
       pass
     if is_coro_context:
-      raise RuntimeError('When using Experiment from a coroutine please use '
-                         '`async with` syntax')
+      raise RuntimeError(
+          'When using Experiment from a coroutine please use '
+          '`async with` syntax'
+      )
 
     self._current_experiment_token = _current_experiment.set(self)
     self._event_loop = asyncio.new_event_loop()
     asyncio.get_child_watcher().attach_loop(self._event_loop)
     self._event_loop_thread = threading.Thread(
-        target=self._event_loop.run_forever, daemon=True)
+        target=self._event_loop.run_forever, daemon=True
+    )
     self._event_loop_thread.start()
 
     # asyncio.run_coroutine_threadsafe doesn't accept class method and wants it
     # wrapped in a function.
     async def async_enter():
       await self.__aenter__()
 
     asyncio.run_coroutine_threadsafe(
-        async_enter(), loop=self._event_loop).result()
+        async_enter(), loop=self._event_loop
+    ).result()
 
     return self
 
   def _wait_for_tasks(self):
+    """Waits for pending tasks to complete, raising the first error."""
+    exception = None
     while not self._running_tasks.empty():
       try:
         self._running_tasks.get_nowait().result()
       except futures.CancelledError:
         # Ignore cancelled tasks.
         pass
+      except Exception as e:  # pylint: disable=broad-except
+        # Allow remaining tasks to complete before raising the first exception.
+        if not exception:
+          exception = e
+    if exception:
+      raise exception
 
   def __exit__(self, exc_type, exc_value, traceback):  # pylint:disable=redefined-outer-name
     _current_experiment.reset(self._current_experiment_token)
     self._wait_for_tasks()
     self._event_loop.call_soon_threadsafe(self._event_loop.stop)
     self._event_loop_thread.join()
 
   async def __aenter__(self):
     self._current_async_experiment_token = _current_experiment.set(self)
     self._event_loop = asyncio.get_event_loop()
     self._running_tasks = queue.Queue()
-    self._work_unit_id_predictor = id_predictor.Predictor(1 +
-                                                          self.work_unit_count)
+    self._work_unit_id_predictor = id_predictor.Predictor(
+        1 + self.work_unit_count
+    )
     return self
 
   async def _await_for_tasks(self):
     while not self._running_tasks.empty():
       await asyncio.wrap_future(self._running_tasks.get_nowait())
 
   async def __aexit__(self, exc_type, exc_value, traceback):  # pylint:disable=redefined-outer-name
@@ -735,16 +781,16 @@
     Returns:
       A sequence of packaging results associated to `packageables` (same order).
     """
     return cls._async_packager.package(packageables)
 
   @classmethod
   def package_async(
-      cls,
-      packageable: job_blocks.Packageable) -> Awaitable[job_blocks.Executable]:
+      cls, packageable: job_blocks.Packageable
+  ) -> Awaitable[job_blocks.Executable]:
     """Queues executable spec to be packaged into executable.
 
     If gathering all packageables for a single `package()` call is inconvenient,
     one may request packaging with `package_async` and later trigger the build
     for the whole batch with `package()`.
 
     Usage:
@@ -772,46 +818,49 @@
 
   @overload
   def add(
       self,
       job: AuxiliaryUnitJob,
       args: Optional[Mapping[str, Any]] = ...,
       *,  # parameters after “*” are keyword-only parameters
-      identity: str = ''
+      identity: str = '',
   ) -> asyncio.Future[ExperimentUnit]:
     ...
 
   @overload
   def add(
       self,
       job: job_blocks.JobType,
       args: Optional[Mapping[str, Any]] = ...,
       *,  # parameters after “*” are keyword-only parameters
       role: WorkUnitRole = ...,
-      identity: str = '') -> asyncio.Future[WorkUnit]:
+      identity: str = '',
+  ) -> asyncio.Future[WorkUnit]:
     ...
 
   @overload
   def add(
       self,
       job: job_blocks.JobType,
       args: Optional[Mapping[str, Any]],
       *,  # parameters after “*” are keyword-only parameters
       role: ExperimentUnitRole,
-      identity: str = '') -> asyncio.Future[ExperimentUnit]:
+      identity: str = '',
+  ) -> asyncio.Future[ExperimentUnit]:
     ...
 
   @overload
   def add(
       self,
       job: job_blocks.JobType,
       args: Optional[Mapping[str, Any]] = ...,
       *,  # parameters after “*” are keyword-only parameters
       role: ExperimentUnitRole,
-      identity: str = '') -> asyncio.Future[ExperimentUnit]:
+      identity: str = '',
+  ) -> asyncio.Future[ExperimentUnit]:
     ...
 
   # The ExperimentUnit return type is determined by the role.
   def add(self, job, args=None, *, role=WorkUnitRole(), identity: str = ''):
     # pyformat: disable
     """Adds a Job / JobGroup to the experiment.
 
@@ -840,39 +889,43 @@
     Returns:
       An awaitable that would be fulfilled when the job is launched.
     """
     # pyformat: enable
     role = pattern_matching.match(
         pattern_matching.Case([AuxiliaryUnitJob], lambda job: job.role),
         pattern_matching.Case([Any], lambda job: role),
-    )(
-        job)
+    )(job)
     experiment_unit_future = self._create_experiment_unit(args, role, identity)
 
     async def launch():
       experiment_unit = await experiment_unit_future
       try:
         await experiment_unit.add(job, args, identity=identity)
       except Exception:
         try:
           experiment_unit.stop(
               mark_as_failed=True,
-              message=f'Work unit creation failed. {traceback.format_exc()}')
+              message=f'Work unit creation failed. {traceback.format_exc()}',
+          )
         except Exception as stop_exception:  # pylint: disable=broad-except
           logging.error("Couldn't stop experiment unit: %s", stop_exception)
         raise
       return experiment_unit
 
     return asyncio.wrap_future(
-        self._create_task(launch()), loop=self._event_loop)
+        self._create_task(launch()), loop=self._event_loop
+    )
 
   @abc.abstractmethod
-  def _create_experiment_unit(self, args: Optional[Mapping[str, Any]],
-                              role: ExperimentUnitRole,
-                              identity: str) -> Awaitable[ExperimentUnit]:
+  def _create_experiment_unit(
+      self,
+      args: Optional[Mapping[str, Any]],
+      role: ExperimentUnitRole,
+      identity: str,
+  ) -> Awaitable[ExperimentUnit]:
     """Creates a new experiment unit.
 
     Synchronously starts the experiment unit creation, ensuring that IDs would
     be assigned in invocation order. The operation itself may run asynchronously
     in background.
 
     Args:
@@ -886,15 +939,16 @@
     """
     raise NotImplementedError
 
   def _create_task(self, task: Awaitable[Any]) -> futures.Future[Any]:
     if not self._event_loop.is_running():
       raise RuntimeError(
           'Event loop is not running. Have you entered Experiment context '
-          'manager (e.g. with xm.create-experiment() as experiment:)?')
+          'manager (e.g. with xm.create-experiment() as experiment:)?'
+      )
     future = asyncio.run_coroutine_threadsafe(task, loop=self._event_loop)
     self._running_tasks.put_nowait(future)
     return future
 
   @property
   def work_unit_count(self) -> int:
     """Returns how many work units the experiment has."""
@@ -906,15 +960,16 @@
     raise NotImplementedError
 
   @property
   def context(self) -> metadata_context.MetadataContext:
     """Returns metadata context for the experiment."""
     return metadata_context.MetadataContext(
         creator=getpass.getuser(),
-        annotations=metadata_context.ContextAnnotations())
+        annotations=metadata_context.ContextAnnotations(),
+    )
 
 
 @abc.abstractmethod
 def create_experiment(experiment_title: Optional[str] = None) -> Experiment:
   """Returns a concrete Experiment instance."""
   raise NotImplementedError
```

### Comparing `xmanager-0.3.0/xmanager/xm/core_test.py` & `xmanager-0.4.0/xmanager/xm/core_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,69 +33,68 @@
 
 class ApplyArgsTest(unittest.TestCase):
 
   def test_wrong_job_args(self):
     with self.assertRaises(ValueError):
       core._apply_args(
           job_blocks.Job(
-              job_blocks.Executable(name=''), xm_mock.MockExecutor()),
-          {'abra': 'kadabra'})
+              job_blocks.Executable(name=''), xm_mock.MockExecutor()
+          ),
+          {'abra': 'kadabra'},
+      )
 
   def test_wrong_job_group_args(self):
     with self.assertRaises(ValueError):
       core._apply_args(
           job_blocks.JobGroup(
               learner=job_blocks.Job(
-                  job_blocks.Executable(name=''), xm_mock.MockExecutor())),
-          {'eval': {
-              'args': {
-                  'batch_size': 32
-              }
-          }})
+                  job_blocks.Executable(name=''), xm_mock.MockExecutor()
+              )
+          ),
+          {'eval': {'args': {'batch_size': 32}}},
+      )
 
 
 class ExperimentTest(unittest.TestCase):
 
   def test_single_job_launch(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
       job = job_blocks.Job(
-          xm_mock.MockExecutable(),
-          xm_mock.MockExecutor(),
-          args={},
-          name='name')
+          xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}, name='name'
+      )
       experiment.add(job)
 
     self.assertEqual(experiment.launched_jobs, [job])
 
   def test_job_group_launch(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
       foo_job = job_blocks.Job(
           xm_mock.MockExecutable(),
           xm_mock.MockExecutor(),
           args={'foo': 1},
-          name='1')
+          name='1',
+      )
       bar_job = job_blocks.Job(
           xm_mock.MockExecutable(),
           xm_mock.MockExecutor(),
           args={'bar': 2},
-          name='2')
+          name='2',
+      )
       experiment.add(job_blocks.JobGroup(foo=foo_job, bar=bar_job))
 
     self.assertEqual(experiment.launched_jobs, [foo_job, bar_job])
 
   def test_job_generator_launch(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
       job = job_blocks.Job(
-          xm_mock.MockExecutable(),
-          xm_mock.MockExecutor(),
-          args={},
-          name='name')
+          xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}, name='name'
+      )
 
       async def job_generator(work_unit: core.WorkUnit, use_magic: bool):
         self.assertEqual(use_magic, True)
         work_unit.add(job)
 
       experiment.add(job_generator, args={'use_magic': True})
 
@@ -117,83 +116,70 @@
 
         experiment.add(job_generator)
 
   def test_auxiliary_unit_job(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
       job = job_blocks.Job(
-          xm_mock.MockExecutable(),
-          xm_mock.MockExecutor(),
-          args={},
-          name='name')
+          xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}, name='name'
+      )
       experiment.add(core.AuxiliaryUnitJob(job, termination_delay_secs=600))
 
     self.assertEqual(len(experiment.auxiliary_units), 1)
 
   def test_auxiliary_unit_job_generator(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
 
       async def make_job(aux_unit: core.ExperimentUnit):
         aux_unit.add(
             job_blocks.Job(
                 xm_mock.MockExecutable(),
                 xm_mock.MockExecutor(),
                 args={},
-                name='name'))
+                name='name',
+            )
+        )
 
       experiment.add(
-          core.AuxiliaryUnitJob(make_job, termination_delay_secs=600))
+          core.AuxiliaryUnitJob(make_job, termination_delay_secs=600)
+      )
 
     self.assertEqual(len(experiment.auxiliary_units), 1)
 
   def test_launch_with_args(self):
     experiment = xm_mock.MockExperiment()
     with experiment:
       experiment.add(
           job_blocks.JobGroup(
               foo=job_blocks.Job(
                   xm_mock.MockExecutable(),
                   xm_mock.MockExecutor(),
-                  args={
-                      'x': 1,
-                      'y': 2
-                  },
-                  env_vars={'EDITOR': 'vi'}),
+                  args={'x': 1, 'y': 2},
+                  env_vars={'EDITOR': 'vi'},
+              ),
               bar=job_blocks.Job(
                   xm_mock.MockExecutable(),
                   xm_mock.MockExecutor(),
-                  args=['--bar=1'])),
+                  args=['--bar=1'],
+              ),
+          ),
           args={
-              'foo': {
-                  'args': {
-                      'x': 3,
-                      'z': 4
-                  },
-                  'env_vars': {
-                      'TURBO': 'ON'
-                  }
-              },
-              'bar': {
-                  'args': ['--spacebar']
-              },
-          })
+              'foo': {'args': {'x': 3, 'z': 4}, 'env_vars': {'TURBO': 'ON'}},
+              'bar': {'args': ['--spacebar']},
+          },
+      )
 
     self.assertEqual(
         experiment.launched_jobs[0].args,
-        job_blocks.SequentialArgs.from_collection({
-            'x': 3,
-            'y': 2,
-            'z': 4
-        }),
+        job_blocks.SequentialArgs.from_collection({'x': 3, 'y': 2, 'z': 4}),
+    )
+    self.assertEqual(
+        experiment.launched_jobs[0].env_vars, {'TURBO': 'ON', 'EDITOR': 'vi'}
     )
-    self.assertEqual(experiment.launched_jobs[0].env_vars, {
-        'TURBO': 'ON',
-        'EDITOR': 'vi'
-    })
     self.assertEqual(
         experiment.launched_jobs[1].args,
         job_blocks.SequentialArgs.from_collection(['--bar=1', '--spacebar']),
     )
 
   def test_launch_with_different_args(self):
     experiment = xm_mock.MockExperiment()
@@ -247,26 +233,30 @@
     # There would be no Asyncio even loop thread attahched if running from a
     # worker thread. We ensure that the API still works.
     def launch_experiment():
       experiment = xm_mock.MockExperiment()
       with experiment:
         experiment.add(
             job_blocks.Job(
-                xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}))
+                xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}
+            )
+        )
 
     with futures.ThreadPoolExecutor() as executor:
       executor.submit(launch_experiment).result()
 
   @utils.run_in_asyncio_loop
   async def test_work_unit_wait_until_complete(self):
     experiment = xm_mock.MockExperiment()
     async with experiment:
       experiment.add(
           job_blocks.Job(
-              xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}))
+              xm_mock.MockExecutable(), xm_mock.MockExecutor(), args={}
+          )
+      )
       completion_future = experiment.work_units[0].wait_until_complete()
       self.assertEqual(completion_future.work_unit.work_unit_id, 1)
       await completion_future
 
   @utils.run_in_asyncio_loop
   async def test_work_unit_wait_until_complete_exception(self):
     experiment = xm_mock.MockExperiment()
@@ -274,15 +264,14 @@
       async with experiment:
         experiment.add(failing_job_generator)
         with self.assertRaises(core.ExperimentUnitError):
           await experiment.work_units[0].wait_until_complete()
 
   @utils.run_in_asyncio_loop
   async def test_get_full_job_name(self):
-
     async def generator(work_unit):
       self.assertEqual(work_unit.get_full_job_name('name'), '1_1_name')
 
     async with xm_mock.MockExperiment() as experiment:
       experiment.add(generator)
 
 
@@ -316,43 +305,38 @@
 
       experiment.add(job_generator)
 
     self.assertIsNone(core._current_experiment.get(None))
     self.assertIsNone(core._current_experiment_unit.get(None))
 
   def test_contextvars_async_job_generator_launch(self):
-
     async def make_experiment():
       async with xm_mock.MockExperiment() as experiment:
 
         async def job_generator(work_unit: core.WorkUnit):
-
           self.assertEqual(core._current_experiment_unit.get(), work_unit)
           self.assertEqual(core._current_experiment.get(), work_unit.experiment)
 
         experiment.add(job_generator)
         self.assertEqual(core._current_experiment.get(), experiment)
 
       asyncio.run(make_experiment())
 
     self.assertIsNone(core._current_experiment.get(None))
     self.assertIsNone(core._current_experiment_unit.get(None))
 
   def test_contextvars_nested_async_job_generator_launch(self):
-
     async def job_generator(work_unit: core.WorkUnit):
-
       self.assertEqual(core._current_experiment.get(), work_unit.experiment)
       self.assertEqual(core._current_experiment_unit.get(), work_unit)
 
     with xm_mock.MockExperiment() as outer_exp:
 
       async def make_inner_exp():
         async with xm_mock.MockExperiment() as experiment:
-
           experiment.add(job_generator)
           outer_exp.add(job_generator)
           self.assertEqual(core._current_experiment.get(), experiment)
 
       asyncio.run(make_inner_exp())
       self.assertEqual(core._current_experiment.get(), outer_exp)
```

### Comparing `xmanager-0.3.0/xmanager/xm/executables.py` & `xmanager-0.4.0/xmanager/xm/executables.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 def name_from_path(path: str) -> str:
   """Returns a safe to use executable name based on a filesystem path."""
   return re.sub('\\W', '_', os.path.basename(path.rstrip(os.sep)))
 
 
 class ModuleName(NamedTuple):
   """Name of python module to execute when entering this project."""
+
   module_name: str
 
 
 class CommandList(NamedTuple):
   """List of commands to execute when entering this project."""
+
   commands: List[str]
 
 
 @attr.s(auto_attribs=True)
 class Dockerfile(job_blocks.ExecutableSpec):
   """Dockerfile describes a Dockerfile for generating a docker image.
 
@@ -50,21 +52,23 @@
     dockerfile: The file that will be used for build instructions. Otherwise,
       {path}/Dockerfile will be used. Equivalent to `docker build -f`. A
       relative path will use a Dockerfile that is relative to the launcher
       script.
   """
 
   path: str = attr.ib(
-      converter=utils.resolve_path_relative_to_launcher, default='.')
+      converter=utils.resolve_path_relative_to_launcher, default='.'
+  )
   dockerfile: str = attr.ib(
       # This field is always set once the object is initialized, so we use str
       # as type annotation. But the default value depends on another property
       # and is set in __attrs_post_init__, so we temporary convert None to ''.
       converter=lambda dockerfile: dockerfile or '',
-      default=None)
+      default=None,
+  )
 
   def __attrs_post_init__(self):
     if not self.dockerfile:
       self.dockerfile = os.path.join(self.path, 'Dockerfile')
     self.dockerfile = utils.resolve_path_relative_to_launcher(self.dockerfile)
 
   @property
@@ -114,15 +118,16 @@
           'WORKDIR /workdir',
           'COPY cifar10/ /workdir/cifar10',
         ]
   """
 
   entrypoint: Union[ModuleName, CommandList]
   path: str = attr.ib(
-      converter=utils.resolve_path_relative_to_launcher, default='.')
+      converter=utils.resolve_path_relative_to_launcher, default='.'
+  )
   base_image: Optional[str] = None
   docker_instructions: Optional[List[str]] = None
   use_deep_module: bool = False
 
   @property
   def name(self) -> str:
     return name_from_path(self.path)
@@ -163,15 +168,16 @@
     path: Path to a prebuilt binary.
     dependencies: A list of data dependencies to be packaged together with the
       binary.
   """
 
   path: str
   dependencies: List[BinaryDependency] = attr.ib(
-      converter=list, default=attr.Factory(list))
+      converter=list, default=attr.Factory(list)
+  )
 
   @property
   def name(self) -> str:
     return name_from_path(self.path)
 
 
 @attr.s(auto_attribs=True)
@@ -192,27 +198,30 @@
   @property
   def name(self) -> str:
     return name_from_path(self.label)
 
 
 @attr.s(auto_attribs=True)
 class BazelBinary(job_blocks.ExecutableSpec):
+  # pyformat: disable
   """A Bazel target that produces a self-contained binary.
 
   Note that for Python targets based on https://github.com/google/subpar
   a self-contained '.par' binary would be built.
 
   Attributes:
     label: The Bazel target to be built.
-    dependencies: A list of data dependencies to be packaged together with
-      the binary.
+    dependencies: A list of data dependencies to be packaged together with the
+      binary.
     bazel_args: Bazel command line arguments.
   """
+  # pyformat: enable
 
   label: str
   dependencies: List[BinaryDependency] = attr.ib(
-      converter=list, default=attr.Factory(list))
+      converter=list, default=attr.Factory(list)
+  )
   bazel_args: List[str] = attr.ib(converter=list, default=attr.Factory(list))
 
   @property
   def name(self) -> str:
     return name_from_path(self.label)
```

### Comparing `xmanager-0.3.0/xmanager/xm/executables_test.py` & `xmanager-0.4.0/xmanager/xm/executables_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         path='/home/user/project/',
     )
 
     self.assertEqual(executable.name, 'project')
 
   def test_container_name(self):
     executable = executables.Container(
-        image_path='/home/user/project/image.tar')
+        image_path='/home/user/project/image.tar'
+    )
 
     self.assertEqual(executable.name, 'image_tar')
 
   def test_binary_name(self):
     executable = executables.Binary(path='./binary')
 
     self.assertEqual(executable.name, 'binary')
```

### Comparing `xmanager-0.3.0/xmanager/xm/id_predictor.py` & `xmanager-0.4.0/xmanager/xm/id_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,23 @@
       id_to_submit: The id to be submitted.
 
     Yields:
       Yields when it is time to send the request to the backend.
     """
     async with self._last_created_id_condition:
       await self._last_created_id_condition.wait_for(
-          lambda: self._is_broken or self._last_created_id == id_to_submit - 1)
+          lambda: self._is_broken or self._last_created_id == id_to_submit - 1
+      )
 
       try:
         if self._is_broken:
           raise BrokenSequenceError(
               f'Id {id} would never be ready to submit as'
-              ' submission of the previous one has failed')
+              ' submission of the previous one has failed'
+          )
         yield
         self._last_created_id = id_to_submit
       except:
         self._is_broken = True
         raise
       finally:
         self._last_created_id_condition.notify_all()
```

### Comparing `xmanager-0.3.0/xmanager/xm/id_predictor_test.py` & `xmanager-0.4.0/xmanager/xm/id_predictor_test.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm/job_blocks.py` & `xmanager-0.4.0/xmanager/xm/job_blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Data classes for job-related abstractions."""
 
 import abc
+import functools
+import itertools
 import re
 from typing import Any, Awaitable, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, TypeVar, Union
 
 import attr
-
 from xmanager.xm import pattern_matching
 from xmanager.xm import utils
 
 UserArgs = Union[Mapping, Sequence, 'SequentialArgs']
 
 
+@functools.cache
+def print_none_warning(key: str) -> None:
+  print(
+      f'WARNING: Setting `{key}=None` will exclude the flag. To pass the '
+      f'actual value, pass the string literal `{key}="None"` instead'
+  )
+
+
+def _is_nested_structure(structure: Union[List[Any], Tuple[Any]]) -> bool:
+  """Returns true if a list or tuple contains a list or tuple."""
+  return any(type(element) in (list, tuple) for element in structure)
+
+
 class SequentialArgs:
   """A sequence of positional and keyword arguments for a binary.
 
   Unix command line arguments are just a list of strings. But it is very common
   to simulate keyword arguments in a --key=value form. It is not uncommon to
   only have keyword arguments. Therefore we allow providing args as:
 
@@ -64,16 +78,17 @@
     name: str
 
   def __init__(self) -> None:
     """Constucts an empty SequentialArgs.
 
     Prefer using xm.merge_args to construct SequentialArgs objects.
     """
-    self._items: List[Union[SequentialArgs._RegularItem,
-                            SequentialArgs._KeywordItem]] = []
+    self._items: List[
+        Union[SequentialArgs._RegularItem, SequentialArgs._KeywordItem]
+    ] = []
     self._kwvalues: Dict[str, Any] = {}
 
   def _ingest_regular_item(self, value: Any) -> None:
     self._items.append(SequentialArgs._RegularItem(value))
 
   def _ingest_keyword_item(self, name: str, value: Any) -> None:
     if name not in self._kwvalues:
@@ -102,29 +117,34 @@
     result = SequentialArgs()
     if collection is None:
       return result
 
     def check_for_string(args: str) -> None:
       raise ValueError(
           f'Tried to construct xm.SequentialArgs from a string: {args!r}. '
-          f'Wrap it in a list: [{args!r}] to make it a single argument.')
+          f'Wrap it in a list: [{args!r}] to make it a single argument.'
+      )
 
     def import_sequential_args(args: SequentialArgs) -> None:
       result._merge_from(args)  # pylint: disable=protected-access
 
     def import_mapping(collection: Mapping[Any, Any]) -> None:
       for key, value in collection.items():
         result._ingest_keyword_item(str(key), value)  # pylint: disable=protected-access
 
     def import_sequence(collection: Sequence[Any]) -> None:
       for value in collection:
         result._ingest_regular_item(value)  # pylint: disable=protected-access
 
-    matcher = pattern_matching.match(check_for_string, import_sequential_args,
-                                     import_mapping, import_sequence)
+    matcher = pattern_matching.match(
+        check_for_string,
+        import_sequential_args,
+        import_mapping,
+        import_sequence,
+    )
     matcher(collection)
     return result
 
   def rewrite_args(self, rewrite: Callable[[str], str]) -> 'SequentialArgs':
     """Applies the rewrite function to all args and returns the result."""
     result = SequentialArgs()
 
@@ -147,38 +167,52 @@
     for item in self._items:
       matcher(item)
 
     return result
 
   def to_list(
       self,
-      escaper: Callable[[Any], str],
-      kwargs_joiner: Callable[[str, str], str] = utils.trivial_kwargs_joiner
+      escaper: Callable[[Any], str] = utils.ARG_ESCAPER,
+      kwargs_joiner: Callable[[str, str], str] = utils.trivial_kwargs_joiner,
   ) -> List[str]:
     """Exports items as a list ready to be passed into the command line."""
 
-    def export_regular_item(item: SequentialArgs._RegularItem) -> Optional[str]:
-      return escaper(item.value)
+    def export_regular_item(
+        item: SequentialArgs._RegularItem,
+    ) -> List[Optional[str]]:
+      return [escaper(item.value)]
 
-    def export_keyword_item(item: SequentialArgs._KeywordItem) -> Optional[str]:
+    def export_keyword_item(
+        item: SequentialArgs._KeywordItem,
+    ) -> List[Optional[str]]:
       value = self._kwvalues[item.name]
       if value is None:
         # We skip flags with None value, allowing the binary to use defaults.
         # A string can be used if a literal "None" value needs to be assigned.
-        return None
+        print_none_warning(item.name)
+        return [None]
       elif isinstance(value, bool):
-        return escaper(f"--{'' if value else 'no'}{item.name}")
+        return [escaper(f"--{'' if value else 'no'}{item.name}")]
+      elif type(value) in (list, tuple) and not _is_nested_structure(value):
+        # Pass sequence of arguments in by repeating the flag for each
+        # element to be consistent with absl's handling of multiple flags.
+        # We do not do this for nested sequences, which absl cannot handle,
+        # and instead fallback to quoting the sequence and leaving parsing of
+        # the nested structure to the executable being called.
+        return [
+            kwargs_joiner(escaper(f'--{item.name}'), escaper(v)) for v in value
+        ]
       else:
-        return kwargs_joiner(escaper(f'--{item.name}'), escaper(value))
+        return [kwargs_joiner(escaper(f'--{item.name}'), escaper(value))]
 
     matcher = pattern_matching.match(
         export_regular_item,
         export_keyword_item,
     )
-    flags = [matcher(item) for item in self._items]
+    flags = itertools.chain.from_iterable(matcher(item) for item in self._items)
     return [f for f in flags if f is not None]
 
   def to_dict(self, kwargs_only: bool = False) -> Dict[str, Any]:
     """Exports items as a dictionary.
 
     Args:
       kwargs_only: Whether to skip positional arguments.
@@ -186,19 +220,21 @@
     Returns:
       The sought dictionary.
     """
     if kwargs_only:
       return self._kwvalues
 
     def export_regular_item(
-        item: SequentialArgs._RegularItem) -> Tuple[str, Any]:
+        item: SequentialArgs._RegularItem,
+    ) -> Tuple[str, Any]:
       return (str(item.value), True)
 
     def export_keyword_item(
-        item: SequentialArgs._KeywordItem) -> Tuple[str, Any]:
+        item: SequentialArgs._KeywordItem,
+    ) -> Tuple[str, Any]:
       return (item.name, self._kwvalues[item.name])
 
     matcher = pattern_matching.match(
         export_regular_item,
         export_keyword_item,
     )
     return dict([matcher(item) for item in self._items])
@@ -281,34 +317,39 @@
 
   @classmethod
   @abc.abstractmethod
   def Spec(cls) -> ExecutorSpec:  # pylint: disable=invalid-name
     raise NotImplementedError
 
 
-def _validate_env_vars(self: Any, attribute: Any, env_vars: Dict[str,
-                                                                 str]) -> None:
+def _validate_env_vars(
+    self: Any, attribute: Any, env_vars: Dict[str, str]
+) -> None:
   del self  # Unused.
   del attribute  # Unused.
   for key in env_vars.keys():
     if not re.fullmatch('[a-zA-Z_][a-zA-Z0-9_]*', key):
-      raise ValueError('Environment variables names must conform to '
-                       f'[a-zA-Z_][a-zA-Z0-9_]*. Got {key!r}.')
+      raise ValueError(
+          'Environment variables names must conform to '
+          f'[a-zA-Z_][a-zA-Z0-9_]*. Got {key!r}.'
+      )
 
 
 @attr.s(auto_attribs=True)
 class Packageable:
   """Packageable describes what to build and its static parameters."""
 
   executable_spec: ExecutableSpec
   executor_spec: ExecutorSpec
   args: SequentialArgs = attr.ib(
-      factory=list, converter=SequentialArgs.from_collection)  # pytype: disable=annotation-type-mismatch
+      factory=list, converter=SequentialArgs.from_collection
+  )  # pytype: disable=annotation-type-mismatch
   env_vars: Dict[str, str] = attr.ib(
-      converter=dict, default=attr.Factory(dict), validator=_validate_env_vars)
+      converter=dict, default=attr.Factory(dict), validator=_validate_env_vars
+  )
 
 
 class Constraint(abc.ABC):
   """Constraint describes the requirements for where a job group can run.
 
   Some examples of constraints include:
 
@@ -343,17 +384,19 @@
     env_vars: Environment variables to apply.
   """
 
   executable: Executable
   executor: Executor
   name: Optional[str] = None
   args: SequentialArgs = attr.ib(
-      factory=list, converter=SequentialArgs.from_collection)  # pytype: disable=annotation-type-mismatch
+      factory=list, converter=SequentialArgs.from_collection
+  )  # pytype: disable=annotation-type-mismatch
   env_vars: Dict[str, str] = attr.ib(
-      converter=dict, default=attr.Factory(dict), validator=_validate_env_vars)
+      converter=dict, default=attr.Factory(dict), validator=_validate_env_vars
+  )
 
 
 class JobGroup:
   """JobGroup describes a set of jobs that run under shared constraints.
 
   Use named arguments to give jobs meaningful names:
 
@@ -395,18 +438,20 @@
     jobs: A mapping of names to jobs.
     constraints: A list of additional scheduling constraints.
   """
 
   jobs: Dict[str, JobType]
   constraints: List[Constraint]
 
-  def __init__(self,
-               *,
-               constraints: Optional[Sequence[Constraint]] = None,
-               **jobs: JobType) -> None:
+  def __init__(
+      self,
+      *,
+      constraints: Optional[Sequence[Constraint]] = None,
+      **jobs: JobType,
+  ) -> None:
     """Builds a JobGroup.
 
     Args:
       constraints: List of additional scheduling constraints. Keyword only arg.
       **jobs: Jobs / job groups that constitute the group passed as kwargs.
     """
     self.jobs = jobs
```

### Comparing `xmanager-0.3.0/xmanager/xm/job_blocks_test.py` & `xmanager-0.4.0/xmanager/xm/job_blocks_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
+from unittest import mock
 
-import mock
+from absl.testing import absltest
 from xmanager.xm import job_blocks
 
 
 class JobBlocksTest(unittest.TestCase):
 
   def test_from_mapping(self):
     args = job_blocks.SequentialArgs.from_collection({
         'a': 1,
         'b': 2,
         'c': 3,
     })
 
     self.assertEqual(args.to_list(str), ['--a=1', '--b=2', '--c=3'])
 
+  def test_from_mapping_multi(self):
+    args = job_blocks.SequentialArgs.from_collection({
+        'a': 1,
+        'c': [3, '4'],
+    })
+
+    self.assertEqual(args.to_list(str), ['--a=1', '--c=3', '--c=4'])
+
+  def test_from_mapping_nested_multi(self):
+    args = job_blocks.SequentialArgs.from_collection({'a': [[1, 2, 3]]})
+
+    self.assertEqual(args.to_list(str), ['--a=[[1, 2, 3]]'])
+
   def test_from_sequence(self):
     args = job_blocks.SequentialArgs.from_collection([1, 2, 3])
 
     self.assertEqual(args.to_list(str), ['1', '2', '3'])
 
   def test_from_none(self):
     args = job_blocks.SequentialArgs.from_collection(None)
@@ -50,39 +64,42 @@
             'b': 'x',
             'c': 't',
         },
         [3],
     )
 
     self.assertEqual(
-        args.to_list(str), ['1', '--a=z', '--b=x', '2', '--c=t', '3'])
+        args.to_list(str), ['1', '--a=z', '--b=x', '2', '--c=t', '3']
+    )
 
   def test_to_dict(self):
     args = job_blocks.merge_args(['--knob'], {1: False})
 
     self.assertEqual(args.to_dict(), {'--knob': True, '1': False})
 
   def test_to_list_bool(self):
     args = job_blocks.SequentialArgs.from_collection({'yes': True, 'no': False})
 
     self.assertEqual(args.to_list(str), ['--yes', '--nono'])
 
   def test_to_list_none(self):
-    args = job_blocks.SequentialArgs.from_collection({
-        'skip_me': None,
-        'pass_me': 'None'
-    })
+    args = job_blocks.SequentialArgs.from_collection(
+        {'skip_me': None, 'pass_me': 'None'}
+    )
 
     self.assertEqual(args.to_list(str), ['--pass_me=None'])
 
   def test_sequential_args_from_string(self):
     with self.assertRaisesRegex(
         ValueError,
-        "Tried to construct xm.SequentialArgs from a string: '--foo'. "
-        "Wrap it in a list: \\['--foo'\\] to make it a single argument."):
+        (
+            "Tried to construct xm.SequentialArgs from a string: '--foo'. "
+            "Wrap it in a list: \\['--foo'\\] to make it a single argument."
+        ),
+    ):
       job_blocks.SequentialArgs.from_collection('--foo')
 
   def test_get_args_for_all_jobs(self):
     group = job_blocks.JobGroup(
         a=job_blocks.Job(mock.Mock(), mock.Mock()),
         b=job_blocks.JobGroup(
             b1=job_blocks.JobGroup(
@@ -90,30 +107,22 @@
                 b1ii=job_blocks.Job(mock.Mock(), mock.Mock()),
             ),
             b2=job_blocks.Job(mock.Mock(), mock.Mock()),
         ),
     )
     logdir = {'logdir': '/logdir/1'}
     expected = {
-        'a': {
-            'args': logdir
-        },
+        'a': {'args': logdir},
         'b': {
             'b1': {
-                'b1i': {
-                    'args': logdir
-                },
-                'b1ii': {
-                    'args': logdir
-                },
-            },
-            'b2': {
-                'args': logdir
+                'b1i': {'args': logdir},
+                'b1ii': {'args': logdir},
             },
+            'b2': {'args': logdir},
         },
     }
     args = job_blocks.get_args_for_all_jobs(group, logdir)
     self.assertDictEqual(expected, args)
 
 
 if __name__ == '__main__':
-  unittest.main()
+  absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/xm/job_operators.py` & `xmanager-0.4.0/xmanager/xm/job_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,41 +19,44 @@
 
 import attr
 from xmanager.xm import job_blocks
 from xmanager.xm import pattern_matching
 
 
 def shallow_copy_job_type(
-    job_type: job_blocks.JobTypeVar) -> job_blocks.JobTypeVar:
+    job_type: job_blocks.JobTypeVar,
+) -> job_blocks.JobTypeVar:
   """Creates a shallow copy of the job structure."""
 
   def apply_to_job_group(job_group: job_blocks.JobGroup) -> job_blocks.JobGroup:
     job_group = copy.copy(job_group)
     job_group.jobs = {key: matcher(job) for key, job in job_group.jobs.items()}
     return job_group
 
   matcher = pattern_matching.match(
       pattern_matching.Case([job_blocks.Job], copy.copy),
       apply_to_job_group,
-      pattern_matching.Case([job_blocks.JobGeneratorType],
-                            lambda generator: generator),
+      pattern_matching.Case(
+          [job_blocks.JobGeneratorType], lambda generator: generator
+      ),
       pattern_matching.Case([job_blocks.JobConfig], copy.copy),
   )
   return matcher(job_type)
 
 
 def populate_job_names(job_type: job_blocks.JobTypeVar) -> None:
   """Assigns default names to the given jobs."""
 
   def apply_to_job(prefix: Sequence[str], target: job_blocks.Job) -> None:
     if target.name is None:
       target.name = '_'.join(prefix) if prefix else target.executable.name
 
-  def apply_to_job_group(prefix: Sequence[str],
-                         target: job_blocks.JobGroup) -> None:
+  def apply_to_job_group(
+      prefix: Sequence[str], target: job_blocks.JobGroup
+  ) -> None:
     for key, job in target.jobs.items():
       matcher([*prefix, key], job)
 
   def ignore_unknown(_: Sequence[str], target: Any) -> None:
     return target
 
   matcher = pattern_matching.match(
@@ -72,48 +75,51 @@
 
   def match_job(job: job_blocks.Job) -> List[job_blocks.Job]:
     return [job] if predicate(job) else []
 
   def match_job_group(job_group: job_blocks.JobGroup) -> List[job_blocks.Job]:
     return list(
         itertools.chain.from_iterable(
-            [job_collector(job) for job in job_group.jobs.values()]))
+            [job_collector(job) for job in job_group.jobs.values()]
+        )
+    )
 
   job_collector = pattern_matching.match(match_job_group, match_job)
   return job_collector(job_group)
 
 
 @attr.s(auto_attribs=True)
 class ConstraintClique:
   """A constraint with the list of jobs it applies to."""
 
   constraint: job_blocks.Constraint
   jobs: List[job_blocks.Job]
 
 
 def aggregate_constraint_cliques(
-    job_group: job_blocks.JobGroup) -> List[ConstraintClique]:
+    job_group: job_blocks.JobGroup,
+) -> List[ConstraintClique]:
   """Forms constraint cliques.
 
   For each constraint met, collects all jobs it applies to.
 
   Args:
     job_group: A job group to aggregate on.
 
   Returns:
     A set of cliques.
   """
 
   def match_job(
-      job: job_blocks.Job
+      job: job_blocks.Job,
   ) -> Tuple[List[ConstraintClique], List[job_blocks.Job]]:
     return [], [job]
 
   def match_job_group(
-      job_group: job_blocks.JobGroup
+      job_group: job_blocks.JobGroup,
   ) -> Tuple[List[ConstraintClique], List[job_blocks.Job]]:
     cliques: List[ConstraintClique] = []
     jobs: List[job_blocks.Job] = []
     for job in job_group.jobs.values():
       subcliques, subjobs = matcher(job)
       cliques += subcliques
       jobs += subjobs
```

### Comparing `xmanager-0.3.0/xmanager/xm/job_operators_test.py` & `xmanager-0.4.0/xmanager/xm/job_operators_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from xmanager.xm import job_operators
 
 
 def construct_job(name=None):
   return job_blocks.Job(
       name=name,
       executable=xm_mock.MockExecutable(),
-      executor=xm_mock.MockExecutor())
+      executor=xm_mock.MockExecutor(),
+  )
 
 
 class JobOperatorsTest(unittest.TestCase):
 
   def test_collect_jobs_by_filter_gathers_matches(self):
     job_group = job_blocks.JobGroup(
         foo=construct_job('foo'),
```

### Comparing `xmanager-0.3.0/xmanager/xm/metadata_context.py` & `xmanager-0.4.0/xmanager/xm/metadata_context.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm/packagables.py` & `xmanager-0.4.0/xmanager/xm/packagables.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,17 @@
 
   Returns:
     A packageable object which can be turned into an executable with
     Experiment.package or Experiment.package_async.
   """
   # pyformat: enable
   return job_blocks.Packageable(
-      executable_spec=executables.Container(image_path=image_path,),
+      executable_spec=executables.Container(
+          image_path=image_path,
+      ),
       executor_spec=executor_spec,
       args=args,
       env_vars=env_vars,
   )
 
 
 def bazel_container(
```

### Comparing `xmanager-0.3.0/xmanager/xm/packagables_generator.py` & `xmanager-0.4.0/xmanager/xm/packagables_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
 
 def generate_docstring(executable: Type[job_blocks.ExecutableSpec]) -> str:
   """Returns a docstring for a ExecutableSpec factory method."""
   docstring = executable.__doc__
   if _ATTRIBUTES_SECTION_HEADER not in docstring:
     raise Exception(
-        f'Please add Attributes: section to {executable.__name__} docstring.')
+        f'Please add Attributes: section to {executable.__name__} docstring.'
+    )
   docstring = re.sub(_ATTRIBUTES_SECTION_HEADER, _ARGS_DOCSTRING, docstring)
   docstring = docstring.rstrip() + _DOCSTRING_SUFFIX.rstrip()
   return docstring
 
 
 def generate_factory_parameters(parameters: List[inspect.Parameter]) -> str:
   """Returns ExecutableSpec factory method parameters definition.
@@ -87,22 +88,26 @@
   Returns:
     Python source code.
   """
   source = '    executor_spec: job_blocks.ExecutorSpec,\n'
 
   keyword_args_started = False
   for parameter in parameters:
-    if (parameter.kind == inspect.Parameter.KEYWORD_ONLY and
-        not keyword_args_started):
+    if (
+        parameter.kind == inspect.Parameter.KEYWORD_ONLY
+        and not keyword_args_started
+    ):
       keyword_args_started = True
       source += '    *,\n'
 
     parameter_source = _KNOWN_ARGS_DICT[parameter.name]
-    if (parameter.default != inspect.Parameter.empty and
-        '=' not in parameter_source):
+    if (
+        parameter.default != inspect.Parameter.empty
+        and '=' not in parameter_source
+    ):
       parameter_source += f' = {parameter.default!r}'
 
     source += f'    {parameter_source},\n'
 
   if not keyword_args_started:
     source += '    *,\n'
 
@@ -120,15 +125,16 @@
     factory_name = 'dockerfile_container'
 
   signature = inspect.signature(executable.__init__)
   # Skip the `self` parameter.
   parameters = list(signature.parameters.values())[1:]
 
   executable_args = '\n'.join(
-      f'          {p.name}={p.name},' for p in parameters)
+      f'          {p.name}={p.name},' for p in parameters
+  )
 
   return f'''
 def {factory_name}(
 {generate_factory_parameters(parameters)}
 ) -> job_blocks.Packageable:
   # pyformat: disable
   """{generate_docstring(executable)}
@@ -137,15 +143,17 @@
   return job_blocks.Packageable(
       executable_spec=executables.{executable.__name__}(
 {executable_args}
       ),
       executor_spec=executor_spec,
       args=args,
       env_vars=env_vars,
-  )'''.strip('\n')
+  )'''.strip(
+      '\n'
+  )
 
 
 def main(argv: Sequence[str]) -> None:
   if len(argv) > 1:
     raise app.UsageError('Too many command-line arguments.')
 
   for spec in _EXECUTABLES_SPECS:
```

### Comparing `xmanager-0.3.0/xmanager/xm/packagables_test.py` & `xmanager-0.4.0/xmanager/xm/packagables_test.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm/pattern_matching.py` & `xmanager-0.4.0/xmanager/xm/pattern_matching.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,36 +44,39 @@
     """Constructs a handler for given types.
 
     Args:
       kind: A tuple of types to match. One for each callable argument.
       handler: A handler to be called in case of a match.
     """
     self.kind = tuple(
-        getattr(arg_type, '__origin__', arg_type) for arg_type in kind)
+        getattr(arg_type, '__origin__', arg_type) for arg_type in kind
+    )
     self.handle = handler
 
   def matches(self, *values: Any) -> bool:
     """Checks if *values match the types."""
     if len(values) != len(self.kind):
       return False
 
     return all(
         expected_type is Any or isinstance(value, expected_type)
-        for expected_type, value in zip(self.kind, values))
+        for expected_type, value in zip(self.kind, values)
+    )
 
 
 def _deduce_types(handler: Callable[..., Any]) -> Tuple[Type[Any]]:
   """Returns callable's argument types."""
   argspec = inspect.getfullargspec(handler)
 
   def get_arg_type(arg: str):
     """Returns argument type or raises a user-friendly exception."""
     if arg not in argspec.annotations:
       raise ValueError(
-          f'{arg} argument of a {handler} is missing a type annotation.')
+          f'{arg} argument of a {handler} is missing a type annotation.'
+      )
     return argspec.annotations[arg]
 
   return tuple(map(get_arg_type, argspec.args))
 
 
 def match(*handlers: Union[Case[R], Callable[..., R]]) -> Callable[..., R]:
   """Creates a router applying appropriate function based on value's type.
@@ -99,30 +102,34 @@
       Case([int], lambda i: str(i)),
     )
     matcher(0)
     ```
   """
 
   cases = [
-      handler if isinstance(handler, Case) else Case(
-          _deduce_types(handler), handler) for handler in handlers
+      handler
+      if isinstance(handler, Case)
+      else Case(_deduce_types(handler), handler)
+      for handler in handlers
   ]
 
   def apply(*values: Any) -> R:
     for case in cases:
       if case.matches(*values):
         return case.handle(*values)
 
     value_types = tuple(type(value) for value in values)
     known_types = '\n'.join(str(case.kind) for case in cases)
-    raise TypeError(f'{values} did not match any type pattern. Values have '
-                    f'following types:\n'
-                    f'{value_types}\n'
-                    f'Which does not match any of:\n'
-                    f'{known_types}')
+    raise TypeError(
+        f'{values} did not match any type pattern. Values have '
+        'following types:\n'
+        f'{value_types}\n'
+        'Which does not match any of:\n'
+        f'{known_types}'
+    )
 
   return apply
 
 
 def async_match(*handlers: Callable[..., R]) -> Callable[..., Awaitable[R]]:
   """`match` for async functions."""
   # Python type system doesn't differentiate regular and async functions enough.
```

### Comparing `xmanager-0.3.0/xmanager/xm/pattern_matching_test.py` & `xmanager-0.4.0/xmanager/xm/pattern_matching_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,54 +32,52 @@
   def testMatch_throwsWhenNoneFit(self):
     matcher = pattern_matching.match()
 
     with self.assertRaises(TypeError):
       matcher(0)
 
   def testMatch_earlierOptionWins(self):
-
     class P:
       pass
 
     class C(P):
       pass
 
     matcher = pattern_matching.match(
         pattern_matching.Case([P], lambda _: 'P'),
         pattern_matching.Case([C], lambda _: 'C'),
     )
 
     self.assertEqual(matcher(C()), 'P')
 
   def testMatch_asVisitor(self):
-
     def visit_int(n: int):
       return n * 2
 
     def visit_str(s: str):
       return len(s)
 
     matcher = pattern_matching.match(visit_int, visit_str)
 
     self.assertEqual(matcher(1), 2)
     self.assertEqual(matcher('zzz'), 3)
 
   def testMatch_multipleArguments(self):
-
     def visit_just_one(k: int):
       return k * 2
 
     def visit_too_many(k: int, l: int, m: int):
       return k * l * m
 
     def visit_just_right(k: int, l: int):
       return k * l
 
-    matcher = pattern_matching.match(visit_just_one, visit_too_many,
-                                     visit_just_right)
+    matcher = pattern_matching.match(
+        visit_just_one, visit_too_many, visit_just_right
+    )
 
     self.assertEqual(matcher(2, 3), 6)
 
   def testMatch_parameterizedGenerics(self):
     """Test that generics parameters don't confuse isinstance.
 
     Note that the parameters don't participate in matching. We can't distinguish
@@ -93,15 +91,14 @@
 
   def testMatch_missingAnnotation(self):
     with self.assertRaises(ValueError):
       pattern_matching.match(lambda x: x)
 
   @utils.run_in_asyncio_loop
   async def testMatch_async(self):
-
     async def visit_int(n: int):
       return n * 2
 
     async def visit_str(s: str):
       return len(s)
 
     matcher = pattern_matching.async_match(visit_int, visit_str)
```

### Comparing `xmanager-0.3.0/xmanager/xm/resources.py` & `xmanager-0.4.0/xmanager/xm/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import functools
 import itertools
 import operator
 import re
 from typing import Any, Iterable, Iterator, Dict, Mapping, MutableMapping, Optional, Tuple, Union
 
 import immutabledict
-import termcolor
 from xmanager.xm import pattern_matching as pm
 
 
 class _CaseInsensetiveResourceTypeMeta(enum.EnumMeta):
   """Metaclass which allows case-insensetive enum lookup.
 
   Enum keys are upper case, but we allow other cases for the input. For
@@ -62,14 +61,15 @@
   # GPUs
   LOCAL_GPU = 100006
   P4 = 21
   T4 = 22
   P100 = 14
   V100 = 17
   A100 = 46
+  A100_80GIB = 66
 
   # TPUs
   TPU_V2 = 3
   TPU_V3 = 16
 
   # TODO: do we need V2_DONUT and V3_DONUT?
 
@@ -142,15 +142,16 @@
 
       return super().__new__(cls, class_name, bases, dct)
 
     def __getitem__(cls, item: str) -> ResourceType:
       result = ResourceType[item]
       if result not in cls:  # pylint: disable=unsupported-membership-test
         raise AttributeError(
-            f"type object '{cls.__name__}' has no attribute '{item}'")
+            f"type object '{cls.__name__}' has no attribute '{item}'"
+        )
       return result
 
     def __iter__(cls) -> Iterator[ResourceType]:
       return iter(values)
 
     def contains(cls, value: ResourceType) -> bool:
       return value in values
@@ -181,17 +182,19 @@
     [
         # LOCAL_GPU is missing as only specific GPU types should be added.
         ResourceType.P4,
         ResourceType.T4,
         ResourceType.P100,
         ResourceType.V100,
         ResourceType.A100,
+        ResourceType.A100_80GIB,
     ],
 )
 
+
 _AcceleratorType = _enum_subset(
     '_AcceleratorType',
     [
         ResourceType.LOCAL_GPU,
         *list(TpuType),
         *list(GpuType),
     ],
@@ -241,15 +244,16 @@
     """Returns user-readable text representation.
 
     Such as "V100: 8, CPU: 1.2, MEMORY: 5.4GiB".
     """
     # TODO: We do not aggregate memory yet, update this method to be more
     # user-friendly.
     return ', '.join(
-        sorted([f'{key}: {value}' for (key, value) in self.items()]))
+        sorted([f'{key}: {value}' for (key, value) in self.items()])
+    )
 
   def __add__(self: 'ResourceDict', rhs: 'ResourceDict') -> 'ResourceDict':
     """Returns a sum of two ResourceDicts."""
     result = ResourceDict()
     for key in [*self.keys(), *rhs.keys()]:
       result[key] = self.get(key, 0) + rhs.get(key, 0)
     return result
@@ -313,16 +317,16 @@
     return hash(self.name)
 
 
 ResourceQuantity = Union[int, float, str, Topology]
 
 
 def _parse_resource_quantity(
-    resource_name: str,
-    value: ResourceQuantity) -> Tuple[float, Optional[Topology]]:
+    resource_name: str, value: ResourceQuantity
+) -> Tuple[float, Optional[Topology]]:
   """Parses a string representation of a resource quantity."""
 
   def parse_string(value: str):
     if 'x' in value:
       topology = Topology(value)
       return topology.chip_count, topology
     else:
@@ -334,105 +338,119 @@
 
   def parse_number(value: Any):
     return float(value), None
 
   try:
     return pm.match(parse_string, parse_topology, parse_number)(value)
   except Exception as e:
-    raise ValueError(f"Couldn't parse resource quantity for {resource_name}. "
-                     f'{value!r} was given.') from e
+    raise ValueError(
+        f"Couldn't parse resource quantity for {resource_name}. "
+        f'{value!r} was given.'
+    ) from e
 
 
 class JobRequirements:
+  # pyformat: disable
   """Describes the resource requirements of a Job.
 
   Attributes:
     task_requirements: Amount of resources needed for a single task within a
       job.
     accelerator: The accelerator the jobs uses, if there is one. Jobs using
       multiple accelerators are not supported because different kinds of
       accelerators are usually not installed on the same host.
     topology: Accelerator topology, if an accelerator is used.
-    location: Place where the job should run. For example a cluster name or
-      a Borg cell.
+    location: Place where the job should run. For example a cluster name or a
+      Borg cell.
     service_tier: A service tier at which the job should run.
     replicas: Number of identical tasks to run within a job
   """
+  # pyformat:enable
 
   task_requirements: ResourceDict
   accelerator: Optional[ResourceType]
   topology: Optional[Topology]
 
   location: Optional[str]
   _service_tier: ServiceTier
 
   def __init__(
       self,
-      resources: Mapping[Union[ResourceType, str],
-                         ResourceQuantity] = immutabledict.immutabledict(),
+      resources: Mapping[
+          Union[ResourceType, str], ResourceQuantity
+      ] = immutabledict.immutabledict(),
       *,
       location: Optional[str] = None,
       replicas: Optional[int] = None,
       service_tier: Optional[ServiceTier] = None,
-      **kw_resources: ResourceQuantity) -> None:
+      **kw_resources: ResourceQuantity,
+  ) -> None:
+    # pyformat: disable
     """Define a set of resources.
 
     Args:
-      resources: resource amounts as a dictionary,
-        for example {xm.ResourceType.V100: 2}.
+      resources: resource amounts as a dictionary, for example
+        {xm.ResourceType.V100: 2}.
       location: Place where the job should run. For example a cluster name or a
         Borg cell.
       replicas: Number of identical tasks to run within a job. 1 by default.
       service_tier: A service tier at which the job should run.
       **kw_resources: resource amounts as a kwargs, for example `v100=2` or
         `ram=1 * xm.GiB`. See xm.ResourceType enum for the list of supported
         types and aliases.
 
     Raises:
       ValueError:
         If several accelerator resources are supplied (i.e. GPU and TPU).
         If the same resource is passed in a `resources` dictionary and as
           a command line argument.
-        If topology is supplied for a non acceelerator resource.
+        If topology is supplied for a non accelerator resource.
     """
+    # pyformat: enable
     self.location = location
     self._service_tier = service_tier or ServiceTier.PROD
 
     self.task_requirements = ResourceDict()
     self.accelerator = None
     self.topology = None
 
-    for resource_name, value in itertools.chain(resources.items(),
-                                                kw_resources.items()):
+    for resource_name, value in itertools.chain(
+        resources.items(), kw_resources.items()
+    ):
       scalar, topology = _parse_resource_quantity(resource_name, value)
       resource = pm.match(
           pm.Case([str], lambda r: ResourceType[r]),
-          pm.Case([ResourceType], lambda r: r))(
-              resource_name)
+          pm.Case([ResourceType], lambda r: r),
+      )(resource_name)
 
       if resource in _AcceleratorType:
         if self.accelerator is not None:
           raise ValueError('Accelerator already set.')
         self.accelerator = resource
         self.topology = topology or Topology(f'{scalar:g}')
       elif topology is not None:
         raise ValueError(
-            f'A topology specified for non accelerator resource {resource}.')
+            f'A topology specified for non accelerator resource {resource}.'
+        )
 
       if resource in self.task_requirements:
         raise ValueError(f'{resource} has been specified twice.')
       self.task_requirements[resource] = scalar
 
-    if (self.accelerator in GpuType and self.topology and
-        len(self.topology.dimensions) == 2):
+    if (
+        self.accelerator in GpuType
+        and self.topology
+        and len(self.topology.dimensions) == 2
+    ):
       if replicas is not None and replicas != self.topology.dimensions[1]:
         raise ValueError(
             f'For multihost GPUs with topology {self.topology}, replicas should'
             f'be either None or {self.topology.dimensions[1]}. Found: '
-            f'{replicas}')
+            f'{replicas}'
+        )
       replicas = self.topology.dimensions[1]
 
     self.replicas = replicas or 1
     self._validate_replicas()
 
   @property
   def service_tier(self):
@@ -442,15 +460,16 @@
   def service_tier(self, new_service_tier):
     self._service_tier = new_service_tier
 
   def _validate_replicas(self) -> None:
     """Raises ValueError if replication is not supported."""
     if self.replicas > 1 and self.accelerator in TpuType:
       raise ValueError(
-          f'Replicated jobs are not supported for {self.accelerator}.')
+          f'Replicated jobs are not supported for {self.accelerator}.'
+      )
 
   def __repr__(self) -> str:
     """Returns string representation of the requirements."""
     args = []
 
     for resource, value in self.task_requirements.items():
       if resource in TpuType:
```

### Comparing `xmanager-0.3.0/xmanager/xm/resources_test.py` & `xmanager-0.4.0/xmanager/xm/resources_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for xmanager.xm.resources."""
 
-import unittest
+from absl.testing import absltest
 from absl.testing import parameterized
 
 from xmanager import xm
 from xmanager.xm import resources
 from xmanager.xm.resources import JobRequirements
 from xmanager.xm.resources import ResourceType
 
 
-class ResourceDictTest(unittest.TestCase):
+class ResourceDictTest(absltest.TestCase):
 
   def test_resource_type_by_name(self):
     self.assertEqual(ResourceType['cpu'], ResourceType.CPU)
     self.assertEqual(ResourceType['Cpu'], ResourceType.CPU)
     self.assertEqual(ResourceType['CPU'], ResourceType.CPU)
     with self.assertRaises(KeyError):
       ResourceType['UPC']  # pylint: disable=pointless-statement
@@ -34,15 +34,16 @@
   def test_resource_dict_to_string(self):
     resource_dict = resources.ResourceDict()
     resource_dict[ResourceType.V100] = 8
     resource_dict[ResourceType.CPU] = 4.2 * xm.vCPU
     resource_dict[ResourceType.MEMORY] = 16.5 * xm.GiB
 
     self.assertEqual(
-        str(resource_dict), 'CPU: 4.2, MEMORY: 17716740096.0, V100: 8')
+        str(resource_dict), 'CPU: 4.2, MEMORY: 17716740096.0, V100: 8'
+    )
 
   def test_resource_dict_from_job_requirements(self):
     requirements = JobRequirements(cpu=0.5 * xm.vCPU, memory=2 * xm.MiB, v100=8)
     resource_dict = requirements.task_requirements
     self.assertEqual(resource_dict[ResourceType.CPU], 0.5)
     self.assertEqual(resource_dict[ResourceType.MEMORY], 2097152)
     self.assertEqual(resource_dict[ResourceType.V100], 8)
@@ -51,25 +52,27 @@
     with self.assertRaises(KeyError):
       JobRequirements(cpu=0.5 * xm.vCPU, upc=2)
 
   def test_requirements_summation(self):
     first = resources.JobRequirements(cpu=1, tpu_v2='2x2')
     second = resources.JobRequirements(ram=4 * xm.GiB, replicas=10)
     total = (
-        first.replicas * first.task_requirements +
-        second.replicas * second.task_requirements)
+        first.replicas * first.task_requirements
+        + second.replicas * second.task_requirements
+    )
     self.assertEqual(total[ResourceType.CPU], 1)
     self.assertEqual(total[ResourceType.RAM], 40 * xm.GiB)
     self.assertEqual(total[ResourceType.TPU_V2], 4)
 
 
 class TopologyTest(parameterized.TestCase):
 
-  @parameterized.parameters(('2', 2), ('4x4', 16), ('2x3x5', 30),
-                            ('4x4_twisted', 16))
+  @parameterized.parameters(
+      ('2', 2), ('4x4', 16), ('2x3x5', 30), ('4x4_twisted', 16)
+  )
   def test_resource_type_by_name(self, topology, chip_count):
     self.assertEqual(resources.Topology(topology).chip_count, chip_count)
 
   def test_invalid_topology(self):
     with self.assertRaises(resources.InvalidTpuTopologyError):
       resources.Topology('euclidian')
 
@@ -77,32 +80,36 @@
     self.assertEqual(repr(resources.Topology('4x4')), "xm.Topology('4x4')")
 
   def test_topology_eq(self):
     self.assertEqual(resources.Topology('4x4'), resources.Topology('4x4'))
     self.assertNotEqual(resources.Topology('2x2'), resources.Topology('4x4'))
 
     self.assertEqual(
-        hash(resources.Topology('4x4')), hash(resources.Topology('4x4')))
+        hash(resources.Topology('4x4')), hash(resources.Topology('4x4'))
+    )
 
 
 class JobRequirementsTest(parameterized.TestCase):
 
   def test_cpu_job(self):
     requirements = resources.JobRequirements(cpu=1.2, ram=1 * xm.GiB)
-    self.assertEqual(requirements.task_requirements[resources.ResourceType.CPU],
-                     1.2)
-    self.assertEqual(requirements.task_requirements[resources.ResourceType.RAM],
-                     1 * xm.GiB)
+    self.assertEqual(
+        requirements.task_requirements[resources.ResourceType.CPU], 1.2
+    )
+    self.assertEqual(
+        requirements.task_requirements[resources.ResourceType.RAM], 1 * xm.GiB
+    )
     self.assertIsNone(requirements.accelerator)
     self.assertIsNone(requirements.topology)
     self.assertEqual(requirements.replicas, 1)
 
   def test_construct_requirements(self):
-    requirements = resources.JobRequirements({resources.ResourceType.CPU: 4},
-                                             v100=1)
+    requirements = resources.JobRequirements(
+        {resources.ResourceType.CPU: 4}, v100=1
+    )
     task_requirements = requirements.task_requirements
     self.assertEqual(task_requirements[resources.ResourceType.CPU], 4)
     self.assertEqual(task_requirements[resources.ResourceType.V100], 1)
     self.assertEqual(requirements.replicas, 1)
 
   def test_resource_specified_twice(self):
     with self.assertRaises(ValueError):
@@ -131,20 +138,22 @@
 
   def test_location(self):
     requirements = resources.JobRequirements(location='lon_r7')
     self.assertEqual(requirements.location, 'lon_r7')
 
   def test_service_tier(self):
     requirements = resources.JobRequirements(
-        service_tier=resources.ServiceTier.PROD)
+        service_tier=resources.ServiceTier.PROD
+    )
     self.assertEqual(requirements.service_tier, resources.ServiceTier.PROD)
 
   def test_service_tier_mutable(self):
     requirements = resources.JobRequirements(
-        service_tier=resources.ServiceTier.PROD)
+        service_tier=resources.ServiceTier.PROD
+    )
     requirements.service_tier = resources.ServiceTier.BATCH
     self.assertEqual(requirements.service_tier, resources.ServiceTier.BATCH)
 
   def test_replicas(self):
     requirements = resources.JobRequirements(replicas=2)
     self.assertEqual(requirements.replicas, 2)
 
@@ -159,21 +168,27 @@
   def test_str(self):
     self.assertEqual(
         repr(
             resources.JobRequirements(
                 cpu=1,
                 location='lon_r7',
                 service_tier=resources.ServiceTier.BATCH,
-                replicas=2)),
-        "xm.JobRequirements(cpu=1.0, location='lon_r7', service_tier=xm.ServiceTier.BATCH, replicas=2)"
+                replicas=2,
+            )
+        ),
+        (
+            "xm.JobRequirements(cpu=1.0, location='lon_r7',"
+            ' service_tier=xm.ServiceTier.BATCH, replicas=2)'
+        ),
     )
 
   def test_str_omits_empty_fields(self):
     self.assertEqual(
-        repr(resources.JobRequirements(cpu=1)), 'xm.JobRequirements(cpu=1.0)')
+        repr(resources.JobRequirements(cpu=1)), 'xm.JobRequirements(cpu=1.0)'
+    )
 
   def test_is_gpu_tpu_given_cpu(self):
     requirements = resources.JobRequirements(cpu=1, ram=4 * xm.GiB)
     self.assertNotIn(requirements.accelerator, xm.GpuType)
     self.assertNotIn(requirements.accelerator, xm.TpuType)
 
   def test_is_gpu_tpu_given_gpu(self):
@@ -206,8 +221,8 @@
 
   def test_contains(self):
     self.assertIn(resources.ResourceType.V100, resources.GpuType)
     self.assertNotIn(resources.ResourceType.TPU_V3, resources.GpuType)
 
 
 if __name__ == '__main__':
-  unittest.main()
+  absltest.main()
```

### Comparing `xmanager-0.3.0/xmanager/xm/utils.py` & `xmanager-0.4.0/xmanager/xm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utility functions needed for XManager API implementation.
 
 This module is private and can only be used by the API itself, but not by users.
+
 """
 
 import abc
 import asyncio
 import enum
 import functools
 import os
@@ -51,15 +52,16 @@
   """
 
   arg: str
 
   def __str__(self) -> str:
     """Prevents ShellSafeArg from being used in f-strings."""
     raise RuntimeError(
-        f'Converting {self!r} to a string would strip the ShellSafe semantics.')
+        f'Converting {self!r} to a string would strip the ShellSafe semantics.'
+    )
 
 
 ARG_ESCAPER = pattern_matching.match(
     pattern_matching.Case([ShellSafeArg], lambda v: v.arg),
     pattern_matching.Case([enum.Enum], lambda v: shlex.quote(str(v.name))),
     pattern_matching.Case([Any], lambda v: shlex.quote(str(v))),
 )
@@ -119,15 +121,15 @@
   launch_script_path = sys.argv[0]
   if hasattr(FLAGS, 'xm_launch_script') and FLAGS.xm_launch_script:
     launch_script_path = FLAGS.xm_launch_script
   if not launch_script_path.endswith('.py'):
     # If the launch script is built with subpar we are interested in the name
     # of the main module, rather than subpar binary.
     main_file_path = getattr(sys.modules['__main__'], '__file__', None)
-    if (main_file_path and os.access(main_file_path, os.R_OK)):
+    if main_file_path and os.access(main_file_path, os.R_OK):
       launch_script_path = main_file_path
 
   if not launch_script_path:
     return ''
 
   # The path may be relative, especially if it comes from sys.argv[0].
   return os.path.abspath(launch_script_path)
@@ -149,14 +151,16 @@
     RuntimeError: If unable to determine the launch script path.
   """
   if os.path.isabs(path):
     return path
 
   launch_script_path = find_launch_script_path()
   if not os.access(launch_script_path, os.R_OK):
-    raise RuntimeError(f'Unable to determine launch script path. '
-                       f'The script is not present at {launch_script_path!r}. '
-                       'This may happen if launch script changes the '
-                       'working directory.')
+    raise RuntimeError(
+        'Unable to determine launch script path. '
+        f'The script is not present at {launch_script_path!r}. '
+        'This may happen if launch script changes the '
+        'working directory.'
+    )
   caller_file_path = os.path.realpath(launch_script_path)
   caller_dir = os.path.dirname(caller_file_path)
   return os.path.realpath(os.path.join(caller_dir, path))
```

### Comparing `xmanager-0.3.0/xmanager/xm/utils_test.py` & `xmanager-0.4.0/xmanager/xm/utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
   @utils.run_in_asyncio_loop
   async def test_run_in_asyncio_loop(self):
     self.assertEqual(await make_me_a_sandwich(), 'sandwich')
 
   def test_run_in_asyncio_loop_returns_value(self):
     self.assertEqual(
-        utils.run_in_asyncio_loop(make_me_a_sandwich)(), 'sandwich')
+        utils.run_in_asyncio_loop(make_me_a_sandwich)(), 'sandwich'
+    )
 
   def test_arg_escaper(self):
     self.assertEqual(utils.ARG_ESCAPER(1.0), '1.0')
     self.assertEqual(utils.ARG_ESCAPER('Jonny Droptable'), "'Jonny Droptable'")
     self.assertEqual(utils.ARG_ESCAPER(ResourceType.VESPEN), 'VESPEN')
 
   def test_shell_safe_arg_in_f_string(self):
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/__init__.py` & `xmanager-0.4.0/xmanager/xm_local/__init__.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm_local/executables.py` & `xmanager-0.4.0/xmanager/xm_local/executables.py`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm_local/execution.py` & `xmanager-0.4.0/xmanager/xm_local/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,19 +85,21 @@
   futures_executor: futures.Executor = attr.Factory(futures.ThreadPoolExecutor)
 
   async def wait(self) -> None:
     if self.model is None:
       return
 
     response = await asyncio.wrap_future(
-        self.futures_executor.submit(self.model.wait))
+        self.futures_executor.submit(self.model.wait)
+    )
     status_code = response['StatusCode']
     if status_code != 0:
       raise RuntimeError(
-          f'Container {self.model!r} returned non-zero status: {status_code}')
+          f'Container {self.model!r} returned non-zero status: {status_code}'
+      )
 
   def get_status(self) -> status.LocalWorkUnitStatus:
     raise NotImplementedError
 
   def terminate(self) -> None:
     if self.model is None:
       return
@@ -128,22 +130,24 @@
   executor = cast(executors.Local, job.executor)
   instance = docker_adapter.instance()
 
   if not instance.has_network(_BRIDGE_NETWORK_NAME):
     instance.create_network(_BRIDGE_NETWORK_NAME)
 
   gpu_count = int(
-      executor.requirements.task_requirements.get(xm.ResourceType.LOCAL_GPU, 0))
+      executor.requirements.task_requirements.get(xm.ResourceType.LOCAL_GPU, 0)
+  )
 
   if gpu_count > 0:
     try:
       subprocess.check_output('nvidia-smi')
     except Exception as exception:
-      raise RuntimeError('No NVIDIA devices detected. Only NVIDIA '
-                         'GPUs are currently supported') from exception
+      raise RuntimeError(
+          'No NVIDIA devices detected. Only NVIDIA GPUs are currently supported'
+      ) from exception
 
   args = xm.merge_args(executable.args, job.args).to_list(utils.ARG_ESCAPER)
   env_vars = {**executable.env_vars, **job.env_vars}
   options = executor.docker_options or executors.DockerOptions()
 
   volumes = options.volumes or {}
   # Add GCP credentials to Local Executor.
@@ -155,16 +159,20 @@
     local_gcs_path = os.path.expanduser('~/gcs')
     image_gcs_path = '/gcs'
 
     if local_gcs_path not in volumes:
       volumes[local_gcs_path] = image_gcs_path
     else:
       logging.warning(
-          'Default GCS path inside container overwritten by'
-          '`volumes` parameter to %s', volumes[local_gcs_path])
+          (
+              'Default GCS path inside container overwritten by'
+              '`volumes` parameter to %s'
+          ),
+          volumes[local_gcs_path],
+      )
 
   container = instance.run_container(
       name=get_full_job_name(job.name),
       image_id=executable.image_id,
       network=_BRIDGE_NETWORK_NAME,
       args=args,
       env_vars=env_vars,
@@ -188,15 +196,16 @@
   process: asyncio.subprocess.Process  # pytype: disable=module-attr
   stream_output: bool
 
   async def wait(self) -> None:
     return_code = await self.process.wait()
     if return_code != 0:
       raise RuntimeError(
-          f'Process {self.process!r} returned non-zero code: {return_code}')
+          f'Process {self.process!r} returned non-zero code: {return_code}'
+      )
 
   def get_status(self) -> status.LocalWorkUnitStatus:
     raise NotImplementedError
 
   def terminate(self) -> None:
     self.process.terminate()
 
@@ -223,30 +232,33 @@
   env_vars = {**executable.env_vars, **job.env_vars}
   process = await asyncio.create_subprocess_exec(
       executable.path,
       *args,
       env=env_vars,
       start_new_session=True,
       stdout=asyncio.subprocess.PIPE
-      if job.executor.experimental_stream_output else None,
+      if job.executor.experimental_stream_output
+      else None,
       stderr=asyncio.subprocess.STDOUT
-      if job.executor.experimental_stream_output else None,
+      if job.executor.experimental_stream_output
+      else None,
   )
   return BinaryHandle(
       name=job.name,
       process=process,
       stream_output=job.executor.experimental_stream_output,
   )
 
 
 # PyType infers the return type of `async` functions without wrapping them with
 # `Awaitable`, so we are overriding the type of `_LOCAL_EXECUTION_ROUTER` to
 # make it right.
-_LocalExecutionRouter = Callable[[Callable[[str], str], xm.Job, Any],
-                                 Awaitable[LocalExecutionHandle]]
+_LocalExecutionRouter = Callable[
+    [Callable[[str], str], xm.Job, Any], Awaitable[LocalExecutionHandle]
+]
 _LOCAL_EXECUTION_ROUTER: _LocalExecutionRouter = pattern_matching.match(
     _launch_loaded_container_image,
     _launch_local_binary,
     _throw_on_unknown_executable,  # pytype: disable=annotation-type-mismatch
 )
 
 # Note that currently handles are never removed from the list. We can consider
@@ -256,33 +268,37 @@
 
 
 @atexit.register
 def _terminate_local_jobs():
   """Terminates local jobs that were launched during the current session."""
   with _local_jobs_lock:
     if _local_jobs:
-      print(f'Terminating {len(_local_jobs)} local job(s)'
-            ' that may still be running...')
+      print(
+          f'Terminating {len(_local_jobs)} local job(s)'
+          ' that may still be running...'
+      )
     for local_job in _local_jobs:
       try:
         local_job.terminate()
       except Exception:  # pylint: disable=broad-except
         logging.warning('Unable to terminate %s', repr(local_job))
 
 
 def _local_job_predicate(job: xm.Job) -> bool:
   return isinstance(job.executor, executors.Local)
 
 
-async def launch(get_full_job_name: Callable[[str], str],
-                 job_group: xm.JobGroup) -> List[LocalExecutionHandle]:
+async def launch(
+    get_full_job_name: Callable[[str], str], job_group: xm.JobGroup
+) -> List[LocalExecutionHandle]:
   """Launches jobs with `xm_local.Local` executor."""
   # Must act on all jobs with `Local` executor.
-  local_jobs = job_operators.collect_jobs_by_filter(job_group,
-                                                    _local_job_predicate)
+  local_jobs = job_operators.collect_jobs_by_filter(
+      job_group, _local_job_predicate
+  )
   handles: List[LocalExecutionHandle] = [
       await _LOCAL_EXECUTION_ROUTER(get_full_job_name, job, job.executable)
       for job in local_jobs
   ]
   with _local_jobs_lock:
     _local_jobs.extend(handles)
   return handles
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/execution_test.py` & `xmanager-0.4.0/xmanager/xm_local/execution_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,201 +25,251 @@
 from xmanager import xm
 from xmanager.docker import docker_adapter
 from xmanager.xm_local import executables as local_executables
 from xmanager.xm_local import execution
 from xmanager.xm_local import executors as local_executors
 
 
-def create_test_job(gpu_count: int,
-                    interactive: bool = False,
-                    mount_gcs_path: bool = True) -> xm.Job:
+def create_test_job(
+    gpu_count: int, interactive: bool = False, mount_gcs_path: bool = True
+) -> xm.Job:
   return xm.Job(
       name='test-job',
       executable=local_executables.LoadedContainerImage(
           name='test',
           image_id='test-image',
           args=xm.SequentialArgs.from_collection({'a': 1}),
-          env_vars={'c': '0'}),
+          env_vars={'c': '0'},
+      ),
       executor=local_executors.Local(
           requirements=xm.JobRequirements(local_gpu=gpu_count),
           docker_options=local_executors.DockerOptions(
               ports={8080: 8080},
               volumes={'a': 'b'},
               interactive=interactive,
-              mount_gcs_path=mount_gcs_path)))
+              mount_gcs_path=mount_gcs_path,
+          ),
+      ),
+  )
 
 
 class ExecutionTest(unittest.IsolatedAsyncioTestCase, parameterized.TestCase):
   """Tests for xm_local.execution (currently only for container launches)."""
 
   async def asyncSetUp(self):
     # Force flag initialization to avoid errors
     flags.FLAGS(sys.argv)
 
   @parameterized.product(
       interactive=[True, False],
       mount_gcs_path=[True, False],
       gcs_dir_exists=[True, False],
-      gpu_count=[0, 1, 4])
+      gpu_count=[0, 1, 4],
+  )
   @mock.patch.object(
-      docker_adapter.DockerAdapter, 'run_container', return_value=None)
-  async def test_container_launch_dispatcher(self, mock_run_container,
-                                             interactive, mount_gcs_path,
-                                             gcs_dir_exists, gpu_count):
+      docker_adapter.DockerAdapter, 'run_container', return_value=None
+  )
+  async def test_container_launch_dispatcher(
+      self,
+      mock_run_container,
+      interactive,
+      mount_gcs_path,
+      gcs_dir_exists,
+      gpu_count,
+  ):
     """Tests if the container launch dispatcher is called correctly when using `xm_local.execution.launch`."""
 
     mock_docker_client = mock.Mock()
     mock_docker_client.has_network.return_value = True
 
     job = create_test_job(
         interactive=interactive,
         mount_gcs_path=mount_gcs_path,
-        gpu_count=gpu_count)
-
-    mock_gcs_dir_existence = (
-        lambda path: gcs_dir_exists and path.endswith('/gcs'))
+        gpu_count=gpu_count,
+    )
 
-    with mock.patch.object(docker, 'from_env',
-                           return_value=mock_docker_client), \
-         mock.patch.object(os.path, 'isdir',
-                           side_effect=mock_gcs_dir_existence), \
-         mock.patch.object(subprocess, 'check_output', return_value=True):
+    mock_gcs_dir_existence = lambda path: (  # pylint:disable=g-long-lambda
+        gcs_dir_exists and path.endswith('/gcs')
+    )
+
+    with mock.patch.object(
+        docker, 'from_env', return_value=mock_docker_client
+    ), mock.patch.object(
+        os.path, 'isdir', side_effect=mock_gcs_dir_existence
+    ), mock.patch.object(
+        subprocess, 'check_output', return_value=True
+    ):
       await execution.launch(lambda x: x, job_group=xm.JobGroup(test_job=job))
 
     expected_gcs_volume = {os.path.expanduser('~/gcs'): '/gcs'}
     mock_run_container.assert_called_once_with(
         name='test-job',
         image_id='test-image',
         network='xmanager',
         args=['--a=1'],
         env_vars={'c': '0'},
         ports={8080: 8080},
-        volumes=({
-            'a': 'b',
-            os.path.expanduser('~/.config/gcloud'): '/root/.config/gcloud'
-        } | (expected_gcs_volume if mount_gcs_path and gcs_dir_exists else {})),
+        volumes=(
+            {
+                'a': 'b',
+                os.path.expanduser('~/.config/gcloud'): '/root/.config/gcloud',
+            }
+            | (expected_gcs_volume if mount_gcs_path and gcs_dir_exists else {})
+        ),
         gpu_count=gpu_count,
-        interactive=interactive)
+        interactive=interactive,
+    )
 
   @parameterized.product(
       mount_gcs_path=[True, False],
       gcs_dir_exists=[True, False],
-      gpu_count=[0, 1, 4])
+      gpu_count=[0, 1, 4],
+  )
   @mock.patch.object(
-      docker.models.containers.ContainerCollection, 'run', return_value=None)
-  async def test_container_launch_by_client(self, mock_client_run,
-                                            mount_gcs_path, gcs_dir_exists,
-                                            gpu_count):
+      docker.models.containers.ContainerCollection, 'run', return_value=None
+  )
+  async def test_container_launch_by_client(
+      self, mock_client_run, mount_gcs_path, gcs_dir_exists, gpu_count
+  ):
     """Tests if the Docker Python client launches containers correctly when using `xm_local.execution.launch`."""
 
     mock_docker_client = mock.Mock()
     mock_docker_client.has_network.return_value = True
     mock_docker_client.containers = (
-        docker.models.containers.ContainerCollection(None))
+        docker.models.containers.ContainerCollection(None)
+    )
 
     job = create_test_job(
-        interactive=False, mount_gcs_path=mount_gcs_path, gpu_count=gpu_count)
-    mock_gcs_dir_existence = (
-        lambda path: gcs_dir_exists and path.endswith('/gcs'))
-
-    with mock.patch.object(docker, 'from_env',
-                           return_value=mock_docker_client), \
-         mock.patch.object(os.path, 'isdir',
-                           side_effect=mock_gcs_dir_existence), \
-         mock.patch.object(subprocess, 'check_output', return_value=True):
+        interactive=False, mount_gcs_path=mount_gcs_path, gpu_count=gpu_count
+    )
+    mock_gcs_dir_existence = lambda path: (  # pylint:disable=g-long-lambda
+        gcs_dir_exists and path.endswith('/gcs')
+    )
+
+    with mock.patch.object(
+        docker, 'from_env', return_value=mock_docker_client
+    ), mock.patch.object(
+        os.path, 'isdir', side_effect=mock_gcs_dir_existence
+    ), mock.patch.object(
+        subprocess, 'check_output', return_value=True
+    ):
       await execution.launch(lambda x: x, job_group=xm.JobGroup(test_job=job))
 
     expected_gcs_volume = {
-        os.path.expanduser('~/gcs'): {
-            'bind': '/gcs',
-            'mode': 'rw'
-        }
+        os.path.expanduser('~/gcs'): {'bind': '/gcs', 'mode': 'rw'}
     }
     mock_client_run.assert_called_once_with(
         'test-image',
         name='test-job',
         hostname='test-job',
         network='xmanager',
         detach=True,
         remove=True,
         command=['--a=1'],
         environment={'c': '0'},
         ports={8080: 8080},
-        volumes=({
-            'a': {
-                'bind': 'b',
-                'mode': 'rw'
-            },
-            os.path.expanduser('~/.config/gcloud'): {
-                'bind': '/root/.config/gcloud',
-                'mode': 'rw'
+        volumes=(
+            {
+                'a': {'bind': 'b', 'mode': 'rw'},
+                os.path.expanduser('~/.config/gcloud'): {
+                    'bind': '/root/.config/gcloud',
+                    'mode': 'rw',
+                },
             }
-        } | (expected_gcs_volume if mount_gcs_path and gcs_dir_exists else {})),
+            | (expected_gcs_volume if mount_gcs_path and gcs_dir_exists else {})
+        ),
         runtime='nvidia' if gpu_count > 0 else None,
-        device_requests=[
+        device_requests=[  # pylint:disable=g-long-ternary
             docker.types.DeviceRequest(count=gpu_count, capabilities=[['gpu']])
-        ] if gpu_count > 0 else None)
+        ]
+        if gpu_count > 0
+        else None,
+    )
 
   @parameterized.product(
       mount_gcs_path=[True, False],
       gcs_dir_exists=[True, False],
-      gpu_count=[0, 1, 4])
+      gpu_count=[0, 1, 4],
+  )
   @mock.patch.object(subprocess, 'run', return_value=None)
   async def test_container_launch_by_subprocess(
-      self, mock_container_launch_by_subprocess, mount_gcs_path, gcs_dir_exists,
-      gpu_count):
+      self,
+      mock_container_launch_by_subprocess,
+      mount_gcs_path,
+      gcs_dir_exists,
+      gpu_count,
+  ):
     """Tests if the Docker subprocesses are created correctly when using `xm_local.execution.launch."""
 
     mock_docker_client = mock.Mock()
     mock_docker_client.has_network.return_value = True
 
     job = create_test_job(
-        interactive=True, mount_gcs_path=mount_gcs_path, gpu_count=gpu_count)
-    mock_gcs_dir_existence = (
-        lambda path: gcs_dir_exists and path.endswith('/gcs'))
-
-    with mock.patch.object(docker, 'from_env',
-                           return_value=mock_docker_client), \
-         mock.patch.object(os.path, 'isdir',
-                           side_effect=mock_gcs_dir_existence), \
-         mock.patch.object(subprocess, 'check_output', return_value=True):
+        interactive=True, mount_gcs_path=mount_gcs_path, gpu_count=gpu_count
+    )
+    mock_gcs_dir_existence = lambda path: (  # pylint:disable=g-long-lambda
+        gcs_dir_exists and path.endswith('/gcs')
+    )
+
+    with mock.patch.object(
+        docker, 'from_env', return_value=mock_docker_client
+    ), mock.patch.object(
+        os.path, 'isdir', side_effect=mock_gcs_dir_existence
+    ), mock.patch.object(
+        subprocess, 'check_output', return_value=True
+    ):
       await execution.launch(lambda x: x, job_group=xm.JobGroup(test_job=job))
 
     expected_gcs_path_args = []
     if mount_gcs_path and gcs_dir_exists:
       expected_gcs_path_args = ['-v', '%s:/gcs' % os.path.expanduser('~/gcs')]
 
     expected_gpu_args = []
     if gpu_count > 0:
       expected_gpu_args = ['--gpus', str(gpu_count), '--runtime', 'nvidia']
 
     mock_container_launch_by_subprocess.assert_called_once_with(
         args=[
-            'docker', 'run', '--network', 'xmanager', '-p', '8080:8080', '-e',
-            'c=0', '-v', 'a:b', '-v',
-            '%s:/root/.config/gcloud' % os.path.expanduser('~/.config/gcloud')
-        ] + expected_gcs_path_args + expected_gpu_args +
-        ['-it', '--entrypoint', 'bash', 'test-image'],
-        check=True)
+            'docker',
+            'run',
+            '--network',
+            'xmanager',
+            '-p',
+            '8080:8080',
+            '-e',
+            'c=0',
+            '-v',
+            'a:b',
+            '-v',
+            '%s:/root/.config/gcloud' % os.path.expanduser('~/.config/gcloud'),
+        ]
+        + expected_gcs_path_args
+        + expected_gpu_args
+        + ['-it', '--entrypoint', 'bash', 'test-image'],
+        check=True,
+    )
 
   @parameterized.product(interactive=[True, False], gpu_count=[0, 1, 4])
   @mock.patch.object(
-      docker_adapter.DockerAdapter, 'run_container', return_value=None)
-  async def test_no_nvidia_smi_launch(self, mock_run_container, interactive,
-                                      gpu_count):
+      docker_adapter.DockerAdapter, 'run_container', return_value=None
+  )
+  async def test_no_nvidia_smi_launch(
+      self, mock_run_container, interactive, gpu_count
+  ):
     mock_docker_client = mock.Mock()
     mock_docker_client.has_network.return_value = True
 
     job = create_test_job(
-        interactive=interactive, mount_gcs_path=True, gpu_count=gpu_count)
+        interactive=interactive, mount_gcs_path=True, gpu_count=gpu_count
+    )
 
     if gpu_count > 0:
-      with mock.patch.object(subprocess, 'check_output',
-                             side_effect=Exception()), \
-        self.assertRaises(RuntimeError):
+      with mock.patch.object(
+          subprocess, 'check_output', side_effect=Exception()
+      ), self.assertRaises(RuntimeError):
         await execution.launch(lambda x: x, job_group=xm.JobGroup(test_job=job))
 
       mock_run_container.assert_not_called()
     else:
       await execution.launch(lambda x: x, job_group=xm.JobGroup(test_job=job))
 
       mock_run_container.assert_called_once_with(
@@ -227,15 +277,16 @@
           image_id='test-image',
           network='xmanager',
           args=['--a=1'],
           env_vars={'c': '0'},
           ports={8080: 8080},
           volumes={
               'a': 'b',
-              os.path.expanduser('~/.config/gcloud'): '/root/.config/gcloud'
+              os.path.expanduser('~/.config/gcloud'): '/root/.config/gcloud',
           },
           gpu_count=gpu_count,
-          interactive=interactive)
+          interactive=interactive,
+      )
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/executors.py` & `xmanager-0.4.0/xmanager/xm_local/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,33 +35,34 @@
       ports: In the simplest form -- a dictionary from `int` to `int`, where the
         keys represent the ports inside the container and the values represent
         the ports of the host to bind. See the specification at
         https://docker-py.readthedocs.io/en/stable/containers.html.
       volumes: A dictionary from `str` to `str`, where the keys represent paths
         inside the host to mount and the values represent paths in the
         container.
-      mount_gcs_path: If True, checks for the `~/gcs` directory on the host
-        and mounts it (if found) at `/gcs` in the container. Defaults to True.
+      mount_gcs_path: If True, checks for the `~/gcs` directory on the host and
+        mounts it (if found) at `/gcs` in the container. Defaults to True.
       interactive: If True, requests a run with interactive shell.
   """
+
   ports: Optional[docker_adapter.Ports] = None
   volumes: Optional[Dict[str, str]] = None
   mount_gcs_path: bool = True
   interactive: bool = False
 
 
 @attr.s(auto_attribs=True)
 class Local(xm.Executor):
   """Current machine executor.
 
   Attributes:
     requirements: Resources to be requested from the host.
-      Note: Currently, only the `local_gpu` resource is
-      supported (and only with a container-based executable).
-      Any other resource requirement will be ignored.
+      Note: Currently, only the `local_gpu` resource is supported (and only with
+        a container-based executable). Any other resource requirement will be
+        ignored.
     docker_options: Options applied if the job is a container-based executable.
     experimental_stream_output: Whether to pipe the job's stdout and stderr to
       the terminal. Might be removed once we decide on the logging design.
   """
 
   requirements: xm.JobRequirements = attr.Factory(xm.JobRequirements)
   docker_options: Optional[DockerOptions] = None
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/experiment.py` & `xmanager-0.4.0/xmanager/xm_local/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 def _throw_on_unknown_executor(job: xm.Job, executor: Any):
   raise TypeError(f'Unsupported executor: {executor!r}. Job: {job!r}')
 
 
 _EXECUTOR_VALIDATOR = pattern_matching.match(
     pattern_matching.Case([xm.Job, local_executors.Local], lambda *_: None),
     pattern_matching.Case([xm.Job, local_executors.Vertex], lambda *_: None),
-    pattern_matching.Case([xm.Job, local_executors.Kubernetes],
-                          lambda *_: None),
+    pattern_matching.Case(
+        [xm.Job, local_executors.Kubernetes], lambda *_: None
+    ),
     _throw_on_unknown_executor,
 )
 
 
 def _validate_job_group(job_group: xm.JobGroup) -> None:
   all_jobs = job_operators.flatten_jobs(job_group)
   for job in all_jobs:
@@ -60,73 +61,90 @@
   k8s_handles: List[kubernetes.KubernetesHandle]
   local_handles: List[local_execution.LocalExecutionHandle]
 
 
 class LocalExperimentUnit(xm.ExperimentUnit):
   """Experiment unit operated by the local backend."""
 
-  def __init__(self, experiment: 'LocalExperiment', experiment_title: str,
-               create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
-               args: Optional[Mapping[str, Any]],
-               role: xm.ExperimentUnitRole) -> None:
+  def __init__(
+      self,
+      experiment: 'LocalExperiment',
+      experiment_title: str,
+      create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
+      args: Optional[Mapping[str, Any]],
+      role: xm.ExperimentUnitRole,
+  ) -> None:
     super().__init__(experiment, create_task, args, role)
     self._experiment_title = experiment_title
     self._local_execution_handles: List[
-        local_execution.LocalExecutionHandle] = []
-    self._non_local_execution_handles: List[
-        local_execution.ExecutionHandle] = []
+        local_execution.LocalExecutionHandle
+    ] = []
+    self._non_local_execution_handles: List[local_execution.ExecutionHandle] = (
+        []
+    )
 
-  async def _submit_jobs_for_execution(self,
-                                       job_group: xm.JobGroup) -> _LaunchResult:
+  async def _submit_jobs_for_execution(
+      self, job_group: xm.JobGroup
+  ) -> _LaunchResult:
     # We are delegating the traversal of the job group to modules.
     # That improves modularity, but sacrifices the ability to make
     # cross-executor decisions.
-    vertex_handles = vertex.launch(self._experiment_title,
-                                   self.experiment_unit_name, job_group)
+    vertex_handles = vertex.launch(
+        self._experiment_title, self.experiment_unit_name, job_group
+    )
     k8s_handles = kubernetes.launch(self.get_full_job_name, job_group)
-    local_handles = await local_execution.launch(self.get_full_job_name,
-                                                 job_group)
+    local_handles = await local_execution.launch(
+        self.get_full_job_name, job_group
+    )
     return _LaunchResult(
         vertex_handles=vertex_handles,
         k8s_handles=k8s_handles,
         local_handles=local_handles,
     )
 
   def _ingest_execution_handles(self, launch_result: _LaunchResult) -> None:
-    self._non_local_execution_handles.extend(launch_result.vertex_handles +
-                                             launch_result.k8s_handles)
+    self._non_local_execution_handles.extend(
+        launch_result.vertex_handles + launch_result.k8s_handles
+    )
     self._local_execution_handles.extend(launch_result.local_handles)
 
   def _monitor_local_jobs(
       self,
-      local_execution_handles: Sequence[local_execution.LocalExecutionHandle]
+      local_execution_handles: Sequence[local_execution.LocalExecutionHandle],
   ) -> None:
     for handle in local_execution_handles:
       self._create_task(handle.monitor())
 
   async def _wait_until_complete(self) -> None:
     try:
-      await asyncio.gather(*[
-          handle.wait() for handle in self._local_execution_handles +
-          self._non_local_execution_handles
-      ])
+      await asyncio.gather(
+          *[
+              handle.wait()
+              for handle in self._local_execution_handles
+              + self._non_local_execution_handles
+          ]
+      )
     except RuntimeError as error:
       raise xm.ExperimentUnitFailedError(
-          error, work_unit=self if isinstance(self, LocalWorkUnit) else None)
+          error, work_unit=self if isinstance(self, LocalWorkUnit) else None
+      )
 
   async def wait_for_local_jobs(self, is_exit_abrupt: bool):
     if not is_exit_abrupt:
       await asyncio.gather(
-          *[handle.wait() for handle in self._local_execution_handles])
+          *[handle.wait() for handle in self._local_execution_handles]
+      )
 
-  def stop(self,
-           *,
-           mark_as_failed: bool = False,
-           mark_as_completed: bool = False,
-           message: Optional[str] = None) -> None:
+  def stop(
+      self,
+      *,
+      mark_as_failed: bool = False,
+      mark_as_completed: bool = False,
+      message: Optional[str] = None,
+  ) -> None:
     """Initiate the process to stop the work unit from running.
 
     This method will synchronously make a request for the work unit to stop.
     However, the method does not actually wait for the work unit to be in a
     terminal state.
 
     Use self.wait_until_complete() after self.stop() to guarantee the work unit
@@ -158,44 +176,51 @@
   def get_status(self) -> local_status.LocalWorkUnitStatus:
     """Gets the current status of the work unit."""
     handles = self._non_local_execution_handles + self._local_execution_handles
     if len(handles) == 1:
       return handles[0].get_status()
     raise NotImplementedError(
         'Status aggregation for work units with multiple jobs is not '
-        'implemented yet.')
+        'implemented yet.'
+    )
 
 
 class LocalWorkUnit(LocalExperimentUnit):
   """A work unit operated by the local backend."""
 
-  def __init__(self, experiment: 'LocalExperiment', experiment_title: str,
-               create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
-               args: Mapping[str, Any], role: xm.ExperimentUnitRole,
-               work_unit_id_predictor: id_predictor.Predictor) -> None:
+  def __init__(
+      self,
+      experiment: 'LocalExperiment',
+      experiment_title: str,
+      create_task: Callable[[Awaitable[Any]], futures.Future[Any]],
+      args: Mapping[str, Any],
+      role: xm.ExperimentUnitRole,
+      work_unit_id_predictor: id_predictor.Predictor,
+  ) -> None:
     super().__init__(experiment, experiment_title, create_task, args, role)
     self._work_unit_id_predictor = work_unit_id_predictor
     self._work_unit_id = self._work_unit_id_predictor.reserve_id()
 
   def _save_handles_to_storage(
-      self, handles: Sequence[local_execution.ExecutionHandle]) -> None:
+      self, handles: Sequence[local_execution.ExecutionHandle]
+  ) -> None:
     """Saves jobs present in the handlers."""
 
     def save_vertex_handle(vertex_handle: vertex.VertexHandle) -> None:
-      database.database().insert_vertex_job(self.experiment_id,
-                                            self.work_unit_id,
-                                            vertex_handle.job_name)
+      database.database().insert_vertex_job(
+          self.experiment_id, self.work_unit_id, vertex_handle.job_name
+      )
 
     def save_k8s_handle(k8s_handle: kubernetes.KubernetesHandle) -> None:
       for job in k8s_handle.jobs:
         namespace = job.metadata.namespace or 'default'
         name = job.metadata.name
-        database.database().insert_kubernetes_job(self.experiment_id,
-                                                  self.work_unit_id, namespace,
-                                                  name)
+        database.database().insert_kubernetes_job(
+            self.experiment_id, self.work_unit_id, namespace, name
+        )
 
     def throw_on_unknown_handle(handle: Any) -> None:
       raise TypeError(f'Unsupported handle: {handle!r}')
 
     handle_saver = pattern_matching.match(
         save_vertex_handle,
         save_k8s_handle,
@@ -210,23 +235,26 @@
       args_view: Mapping[str, Any],
       identity: str,
   ) -> None:
     del args_view  # Unused.
     _validate_job_group(job_group)
 
     if identity:
-      raise ValueError('LocalExperiment does not support idempotent experiment '
-                       'unit creation.')
+      raise ValueError(
+          'LocalExperiment does not support idempotent experiment '
+          'unit creation.'
+      )
 
     async with self._work_unit_id_predictor.submit_id(self.work_unit_id):
       launch_result = await self._submit_jobs_for_execution(job_group)
       self._ingest_execution_handles(launch_result)
       # TODO: Save the local jobs to the database as well.
-      self._save_handles_to_storage(launch_result.vertex_handles +
-                                    launch_result.k8s_handles)
+      self._save_handles_to_storage(
+          launch_result.vertex_handles + launch_result.k8s_handles
+      )
       self._monitor_local_jobs(launch_result.local_handles)
 
   @property
   def experiment_unit_name(self) -> str:
     return f'{self.experiment_id}_{self._work_unit_id}'
 
   @property
@@ -243,16 +271,18 @@
       args_view: Mapping[str, Any],
       identity: str,
   ) -> None:
     del args_view  # Unused.
     _validate_job_group(job_group)
 
     if identity:
-      raise ValueError('LocalExperiment does not support idempotent experiment '
-                       'unit creation.')
+      raise ValueError(
+          'LocalExperiment does not support idempotent experiment '
+          'unit creation.'
+      )
 
     launch_result = await self._submit_jobs_for_execution(job_group)
     self._ingest_execution_handles(launch_result)
     self._monitor_local_jobs(launch_result.local_handles)
 
   @property
   def experiment_unit_name(self) -> str:
@@ -272,21 +302,26 @@
     super().__init__()
     # To distinguish local job names until we use a local database generator.
     self._id = int(time.time() * 10**3)
     self._experiment_title = experiment_title
     self._experiment_units = []
     self._work_unit_count = 0
 
-  def _create_experiment_unit(self, args: Optional[Mapping[str, Any]],
-                              role: xm.ExperimentUnitRole,
-                              identity: str) -> Awaitable[xm.ExperimentUnit]:
+  def _create_experiment_unit(
+      self,
+      args: Optional[Mapping[str, Any]],
+      role: xm.ExperimentUnitRole,
+      identity: str,
+  ) -> Awaitable[xm.ExperimentUnit]:
     """Creates a new WorkUnit instance for the experiment."""
     if identity:
-      raise ValueError('LocalExperiment does not support idempotent experiment '
-                       'unit creation.')
+      raise ValueError(
+          'LocalExperiment does not support idempotent experiment '
+          'unit creation.'
+      )
 
     def create_work_unit(role: xm.WorkUnitRole) -> Awaitable[xm.ExperimentUnit]:
       work_unit = LocalWorkUnit(
           self,
           self._experiment_title,
           self._create_task,
           args,
@@ -301,15 +336,16 @@
       )
       future = asyncio.Future()
       future.set_result(work_unit)
       return future
 
     # TODO: Support `role.termination_delay_secs`.
     def create_auxiliary_unit(
-        role: xm.AuxiliaryUnitRole) -> Awaitable[xm.ExperimentUnit]:
+        role: xm.AuxiliaryUnitRole,
+    ) -> Awaitable[xm.ExperimentUnit]:
       auxiliary_unit = LocalAuxiliaryUnit(
           self,
           self._experiment_title,
           self._create_task,
           args,
           role,
       )
@@ -318,16 +354,18 @@
       future.set_result(auxiliary_unit)
       return future
 
     return pattern_matching.match(create_work_unit, create_auxiliary_unit)(role)
 
   def _wait_for_local_jobs(self, is_exit_abrupt: bool):
     if self._experiment_units:
-      print('Waiting for local jobs to complete. '
-            'Press Ctrl+C to terminate them and exit')
+      print(
+          'Waiting for local jobs to complete. '
+          'Press Ctrl+C to terminate them and exit'
+      )
     for unit in self._experiment_units:
       self._create_task(unit.wait_for_local_jobs(is_exit_abrupt))
 
   def __exit__(self, exc_type, exc_value, traceback):
     # Flush `.add` calls.
     self._wait_for_tasks()
     self._wait_for_local_jobs(exc_value is not None)
@@ -352,46 +390,57 @@
     """Gets work units created via self.add()."""
     raise NotImplementedError
 
 
 def create_experiment(experiment_title: str) -> xm.Experiment:
   """Create Experiment."""
   experiment = LocalExperiment(experiment_title)
-  database.database().insert_experiment(experiment.experiment_id,
-                                        experiment._experiment_title)  # pylint: disable=protected-access
+  database.database().insert_experiment(
+      experiment.experiment_id, experiment._experiment_title  # pylint: disable=protected-access
+  )
   return experiment
 
 
 def get_experiment(experiment_id: int) -> xm.Experiment:
   """Returns an Experiment instance associated with this experiment id."""
   # pylint: disable=protected-access
   experiment_result = database.database().get_experiment(experiment_id)
   experiment = LocalExperiment(experiment_result.experiment_title)
   experiment._id = experiment_id
   experiment._work_unit_id_predictor = id_predictor.Predictor(1)
   for work_unit_result in experiment_result.work_units:
-    work_unit = LocalWorkUnit(experiment, experiment_result.experiment_title,
-                              lambda _: None, {}, xm.WorkUnitRole(),
-                              experiment._work_unit_id_predictor)
+    work_unit = LocalWorkUnit(
+        experiment,
+        experiment_result.experiment_title,
+        lambda _: None,
+        {},
+        xm.WorkUnitRole(),
+        experiment._work_unit_id_predictor,
+    )
     work_unit._work_unit_id = work_unit_result.work_unit_id
     non_local_handles = []
     kubernetes_jobs = []
     for _, data in work_unit_result.jobs.items():
       if data.HasField('local'):
         logging.warning(
-            '[Experiment id: %s, work unit id: %s] '
-            'Loading local experiment units from storage is not implemented.',
-            experiment_id, work_unit_result.work_unit_id)
+            (
+                '[Experiment id: %s, work unit id: %s] Loading local experiment'
+                ' units from storage is not implemented.'
+            ),
+            experiment_id,
+            work_unit_result.work_unit_id,
+        )
       # "caip" is the legacy field name of vertex inside the proto.
       elif data.HasField('caip'):
         non_local_handles = [vertex.VertexHandle(data.caip.resource_name)]
       elif data.HasField('kubernetes'):
         job = k8s_client.V1Job()
         job.metadata = k8s_client.V1ObjectMeta(
-            namespace=data.kubernetes.namespace, name=data.kubernetes.job_name)
+            namespace=data.kubernetes.namespace, name=data.kubernetes.job_name
+        )
         kubernetes_jobs.append(job)
         non_local_handles = [kubernetes.KubernetesHandle(kubernetes_jobs)]
     work_unit._non_local_execution_handles = non_local_handles
     experiment._experiment_units.append(work_unit)
     experiment._work_unit_count += 1
   return experiment
   # pylint: enable=protected-access
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/packaging/bazel_tools.py` & `xmanager-0.4.0/xmanager/xm_local/packaging/bazel_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,38 +25,43 @@
 from xmanager.bazel import client
 from xmanager.bazel import file_utils
 from xmanager.xm import pattern_matching
 
 from google.protobuf.internal.decoder import _DecodeVarint32
 from xmanager.generated import build_event_stream_pb2 as bes_pb2
 
-_BAZEL_COMMAND = flags.DEFINE_string('xm_bazel_command', 'bazel',
-                                     'A command that runs Bazel.')
+_BAZEL_COMMAND = flags.DEFINE_string(
+    'xm_bazel_command', 'bazel', 'A command that runs Bazel.'
+)
 
 
-def _get_important_outputs(events: Sequence[bes_pb2.BuildEvent],
-                           labels: Sequence[str]) -> List[List[bes_pb2.File]]:
+def _get_important_outputs(
+    events: Sequence[bes_pb2.BuildEvent], labels: Sequence[str]
+) -> List[List[bes_pb2.File]]:
   label_to_output: Dict[str, List[bes_pb2.File]] = {}
   for event in events:
     if event.id.HasField('target_completed'):
       # Note that we ignore `event.id.target_completed.aspect`.
       label_to_output[event.id.target_completed.label] = list(
-          event.completed.important_output)
+          event.completed.important_output
+      )
   return [label_to_output[label] for label in labels]
 
 
-def _get_normalized_labels(events: Sequence[bes_pb2.BuildEvent],
-                           labels: Sequence[str]) -> List[str]:
+def _get_normalized_labels(
+    events: Sequence[bes_pb2.BuildEvent], labels: Sequence[str]
+) -> List[str]:
   label_to_expansion: Dict[str, str] = {}
   for event in events:
     if event.id.HasField('pattern'):
       for index, pattern in enumerate(event.id.pattern.pattern):
         # Note that we ignore `event.children.target_configured.aspect`.
         label_to_expansion[pattern] = event.children[
-            index].target_configured.label
+            index
+        ].target_configured.label
   return [label_to_expansion[label] for label in labels]
 
 
 def _get_workspace_directory(events: Sequence[bes_pb2.BuildEvent]) -> str:
   for event in events:
     if event.id.HasField('started'):
       return event.started.workspace_directory
@@ -82,35 +87,39 @@
     events = []
     position = 0
     while position < len(buffer):
       # Reimplementation of Java's `AbstractParser.parseDelimitedFrom` for
       # protobufs, which is not available in Python.
       size, start = _DecodeVarint32(buffer, position)
       event = bes_pb2.BuildEvent()
-      event.ParseFromString(buffer[start:start + size])
+      event.ParseFromString(buffer[start : start + size])
       events.append(event)
       position = start + size
     return events
 
 
 def _root_absolute_path() -> str:
   # If the launch script is run with Bazel, use `BUILD_WORKSPACE_DIRECTORY` to
   # get the root of the workspace where the build was initiated. If the launch
   # script is run with the CLI, query Bazel to find out.
-  return os.getenv('BUILD_WORKSPACE_DIRECTORY') or subprocess.run(
-      [_BAZEL_COMMAND.value, 'info', 'workspace'],
-      check=True,
-      stdout=subprocess.PIPE,
-      stderr=subprocess.PIPE,
-      universal_newlines=True,
-  ).stdout.strip()
+  return (
+      os.getenv('BUILD_WORKSPACE_DIRECTORY')
+      or subprocess.run(
+          [_BAZEL_COMMAND.value, 'info', 'workspace'],
+          check=True,
+          stdout=subprocess.PIPE,
+          stderr=subprocess.PIPE,
+          universal_newlines=True,
+      ).stdout.strip()
+  )
 
 
 def _build_multiple_targets(
-    labels: Sequence[str], bazel_args: Sequence[str] = ()) -> List[List[str]]:
+    labels: Sequence[str], bazel_args: Sequence[str] = ()
+) -> List[List[str]]:
   """Builds the targets and returns paths to their important outputs.
 
   The definition of 'important artifacts in an output group' can be found at
   https://github.com/bazelbuild/bazel/blob/8346ea4cfdd9fbd170d51a528fee26f912dad2d5/src/main/java/com/google/devtools/build/lib/analysis/TopLevelArtifactHelper.java#L223-L224.
 
   Args:
     labels: Labels of the targets to build.
@@ -135,38 +144,43 @@
     )
     events = _read_build_events(bep_path)
     normalized_labels = _get_normalized_labels(events, labels)
     output_lists = _get_important_outputs(events, normalized_labels)
     workspace = _get_workspace_directory(events)
     results: List[List[str]] = []
     for files in output_lists:
-      results.append([
-          os.path.join(workspace, *file.path_prefix, file.name)
-          for file in files
-      ])
+      results.append(
+          [
+              os.path.join(workspace, *file.path_prefix, file.name)
+              for file in files
+          ]
+      )
     return results
 
 
 # Expansions (`...`, `*`) are not allowed.
-_NAME_RE = '[^:/.*]+'
+_NAME_RE = r'(?:[^.*:/]|\.(?!\.\.))+'
 _LABEL_LEXER = re.compile(
-    f'^//(?P<packages>{_NAME_RE}(/{_NAME_RE})*)?(?P<target>:{_NAME_RE})?$')
+    f'^//(?P<packages>{_NAME_RE}(/{_NAME_RE})*)?(?P<target>:{_NAME_RE})?$'
+)
 _LexedLabel = Tuple[List[str], str]
 
 
 def _lex_label(label: str) -> _LexedLabel:
   """Splits the label into packages and target."""
   match = _LABEL_LEXER.match(label)
   if match is None:
     raise ValueError(f'{label} is not an absolute Bazel label')
   groups = match.groupdict()
   packages: Optional[str] = groups['packages']
   target: Optional[str] = groups['target']
-  if packages is None and target is None:
+  if not packages and not target:
     raise ValueError(f'{label} cannot be empty')
+  if target == ':all':
+    raise ValueError('`:all` is not a valid target')
   init = packages.split('/') if packages else []
   last = target[1:] if target else init[-1]
   return init, last
 
 
 def _assemble_label(parts: _LexedLabel) -> str:
   init, last = parts
@@ -201,37 +215,40 @@
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         cwd=_root_absolute_path(),
     ).stdout.decode('utf-8')
     label_kinds = _label_kind_lines_to_dict(stdout.strip().split(os.linesep))
     return [label_kinds[label] for label in labels]
 
-  def build_targets(self, labels: Sequence[str],
-                    bazel_args: Sequence[str]) -> List[List[str]]:
+  def build_targets(
+      self, labels: Sequence[str], bazel_args: Sequence[str]
+  ) -> List[List[str]]:
     return _build_multiple_targets(labels, bazel_args)
 
 
 @functools.lru_cache()
 def local_bazel_service() -> LocalBazelService:
   """Returns a singleton instance of `LocalBazelService`."""
   return LocalBazelService()
 
 
 def _collect_bazel_binary(
-    executable: xm.BazelBinary) -> List[client.BazelTarget]:
+    executable: xm.BazelBinary,
+) -> List[client.BazelTarget]:
   return [
       client.BazelTarget(
           label=executable.label,
           bazel_args=executable.bazel_args,
       ),
   ]
 
 
 def _collect_bazel_container(
-    executable: xm.BazelContainer) -> List[client.BazelTarget]:
+    executable: xm.BazelContainer,
+) -> List[client.BazelTarget]:
   return [
       client.BazelTarget(
           label=executable.label,
           bazel_args=executable.bazel_args,
       ),
   ]
 
@@ -244,17 +261,21 @@
     _collect_bazel_binary,
     _collect_bazel_container,
     _return_empty_list,
 )
 
 
 def collect_bazel_targets(
-    packageables: Sequence[xm.Packageable]) -> List[client.BazelTarget]:
+    packageables: Sequence[xm.Packageable],
+) -> List[client.BazelTarget]:
   """Extracts Bazel targets to package from a sequence of `Packageable`s."""
   return list(
-      itertools.chain(*[
-          _EXECUTABLE_COLLECTOR(packageable.executable_spec)
-          for packageable in packageables
-      ]))
+      itertools.chain(
+          *[
+              _EXECUTABLE_COLLECTOR(packageable.executable_spec)
+              for packageable in packageables
+          ]
+      )
+  )
 
 
 TargetOutputs = Dict[client.BazelTarget, List[str]]
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/packaging/cloud.py` & `xmanager-0.4.0/xmanager/xm_local/packaging/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,22 @@
   def _throw_on_unknown_executor(executor: Any):
     raise TypeError(f'Unsupported executor specification: {executor!r}. ')
 
   return pattern_matching.match(
       _get_push_image_tag_caip,
       _get_push_image_tag_kubernetes,
       _throw_on_unknown_executor,
-  )(
-      executor_spec)
+  )(executor_spec)
 
 
-def _package_container(bazel_outputs: bazel_tools.TargetOutputs,
-                       packageable: xm.Packageable,
-                       container: xm.Container) -> xm.Executable:
+def _package_container(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    container: xm.Container,
+) -> xm.Executable:
   """Matcher method for packaging `xm.Container`.
 
   If the user builds an image with the same repository name as an image in a
   remote Cloud registry, the user should push the image before running XManager,
   because XManager will not push a local image in the packaging step.
 
   Unless the container's image path already matches the GCR project prefix, we
@@ -68,16 +69,18 @@
     container: Container specifying image path.
 
   Returns:
     GoogleContainerRegistryImage Executable.
   """
   del bazel_outputs
   gcr_project_prefix = 'gcr.io/' + auth.get_project_name()
-  if container.image_path.startswith(
-      gcr_project_prefix) or not docker_lib.is_docker_installed():
+  if (
+      container.image_path.startswith(gcr_project_prefix)
+      or not docker_lib.is_docker_installed()
+  ):
     return local_executables.GoogleContainerRegistryImage(
         name=packageable.executable_spec.name,
         image_path=container.image_path,
         args=packageable.args,
         env_vars=packageable.env_vars,
     )
 
@@ -103,67 +106,78 @@
       name=packageable.executable_spec.name,
       image_path=push_image_tag,
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
-def _package_dockerfile(bazel_outputs: bazel_tools.TargetOutputs,
-                        packageable: xm.Packageable, dockerfile: xm.Dockerfile):
+def _package_dockerfile(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    dockerfile: xm.Dockerfile,
+):
   """Matcher method for packaging `xm.Dockerfile`."""
   del bazel_outputs
   push_image_tag = _get_push_image_tag(packageable.executor_spec)
   if not push_image_tag:
     gcr_project_prefix = 'gcr.io/' + auth.get_project_name()
     tag = docker_lib.create_tag()
     push_image_tag = f'{gcr_project_prefix}/{dockerfile.name}:{tag}'
 
   image = build_image.build_by_dockerfile(
       dockerfile.path,
       dockerfile.dockerfile,
       push_image_tag,
-      pull_image=docker_lib.is_docker_installed())
+      pull_image=docker_lib.is_docker_installed(),
+  )
   if docker_lib.is_docker_installed():
     build_image.push(image)
   return local_executables.GoogleContainerRegistryImage(
       name=packageable.executable_spec.name,
       image_path=push_image_tag,
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
 def _package_python_container(
-    bazel_outputs: bazel_tools.TargetOutputs, packageable: xm.Packageable,
-    python_container: xm.PythonContainer) -> xm.Executable:
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    python_container: xm.PythonContainer,
+) -> xm.Executable:
   """Matcher method for packaging `xm.PythonContainer`."""
   del bazel_outputs
   push_image_tag = _get_push_image_tag(packageable.executor_spec)
   image = build_image.build(
       python_container,
       packageable.args,
       packageable.env_vars,
       push_image_tag,
-      pull_image=docker_lib.is_docker_installed())
+      pull_image=docker_lib.is_docker_installed(),
+  )
   if docker_lib.is_docker_installed():
     build_image.push(image)
   return local_executables.GoogleContainerRegistryImage(
       name=packageable.executable_spec.name,
       image_path=image,
   )
 
 
-def _package_bazel_container(bazel_outputs: bazel_tools.TargetOutputs,
-                             packageable: xm.Packageable,
-                             bazel_container: xm.BazelContainer):
+def _package_bazel_container(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    bazel_container: xm.BazelContainer,
+):
   """Matcher method for packaging `xm.BazelContainer`."""
-  paths = bazel_outputs[bazel_client.BazelTarget(
-      label=bazel_container.label,
-      bazel_args=bazel_container.bazel_args,
-  )]
+  paths = bazel_outputs[
+      bazel_client.BazelTarget(
+          label=bazel_container.label,
+          bazel_args=bazel_container.bazel_args,
+      )
+  ]
 
   instance = docker_adapter.instance()
   client = instance.get_client()
 
   push_image_tag = _get_push_image_tag(packageable.executor_spec)
   print(f'Loading {bazel_container.label}...')
   loaded_image_id = instance.load_image(paths[0])
@@ -175,26 +189,31 @@
 
   return local_executables.GoogleContainerRegistryImage(
       name=packageable.executable_spec.name,
       image_path=push_image_tag,
   )
 
 
-def _throw_on_unknown_executable(packageable: xm.Packageable,
-                                 executable: xm.ExecutableSpec):
-  raise TypeError('Unsupported executable specification '
-                  f'for Cloud packaging: {executable!r}')
+def _throw_on_unknown_executable(
+    packageable: xm.Packageable, executable: xm.ExecutableSpec
+):
+  raise TypeError(
+      'Unsupported executable specification '
+      f'for Cloud packaging: {executable!r}'
+  )
 
 
 _CLOUD_PACKAGING_ROUTER = pattern_matching.match(
     _package_container,
     _package_dockerfile,
     _package_python_container,
     _package_bazel_container,
     _throw_on_unknown_executable,
 )
 
 
 def package_cloud_executable(
-    bazel_outputs: bazel_tools.TargetOutputs, packageable: xm.Packageable,
-    executable_spec: xm.ExecutableSpec) -> xm.Executable:
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    executable_spec: xm.ExecutableSpec,
+) -> xm.Executable:
   return _CLOUD_PACKAGING_ROUTER(bazel_outputs, packageable, executable_spec)
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/packaging/local.py` & `xmanager-0.4.0/xmanager/xm_local/packaging/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 from xmanager.docker import docker_adapter
 from xmanager.xm import executables
 from xmanager.xm import pattern_matching
 from xmanager.xm_local import executables as local_executables
 from xmanager.xm_local.packaging import bazel_tools
 
 
-def _package_container(bazel_outputs: bazel_tools.TargetOutputs,
-                       packageable: xm.Packageable,
-                       container: executables.Container) -> xm.Executable:
+def _package_container(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    container: executables.Container,
+) -> xm.Executable:
   """Packages a container for local execution."""
   del bazel_outputs
   instance = docker_adapter.instance()
   image_id = None
   if os.path.exists(container.image_path):
     image_id = instance.load_image(container.image_path)
   elif instance.is_registry_label(container.image_path):
@@ -43,104 +45,132 @@
         name=packageable.executable_spec.name,
         image_id=image_id,
         args=packageable.args,
         env_vars=packageable.env_vars,
     )
   else:
     raise ValueError(
-        f'{container.image_path} is found neither locally nor remotely')
+        f'{container.image_path} is found neither locally nor remotely'
+    )
 
 
-def _package_binary(bazel_outputs: bazel_tools.TargetOutputs,
-                    packageable: xm.Packageable, binary: executables.Binary):
+def _package_binary(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    binary: executables.Binary,
+):
   del bazel_outputs
   if not os.path.exists(binary.path):
     raise ValueError(f'{binary.path} does not exist on this machine')
   return local_executables.LocalBinary(
       name=packageable.executable_spec.name,
       path=binary.path,
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
-def _package_dockerfile(bazel_outputs: bazel_tools.TargetOutputs,
-                        packageable: xm.Packageable,
-                        dockerfile: executables.Dockerfile):
+def _package_dockerfile(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    dockerfile: executables.Dockerfile,
+):
   del bazel_outputs
-  image_id = docker_lib.build_docker_image(dockerfile.name, dockerfile.path,
-                                           dockerfile.dockerfile)
+  image_id = docker_lib.build_docker_image(
+      dockerfile.name, dockerfile.path, dockerfile.dockerfile
+  )
   return local_executables.LoadedContainerImage(
       name=packageable.executable_spec.name,
       image_id=image_id,
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
-def _package_python_container(bazel_outputs: bazel_tools.TargetOutputs,
-                              packageable: xm.Packageable,
-                              py_executable: executables.PythonContainer):
+def _package_python_container(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    py_executable: executables.PythonContainer,
+):
   del bazel_outputs
   # Use the directory as the image name.
   image_name = os.path.basename(py_executable.path)
-  image_id = build_image.build(py_executable, packageable.args,
-                               packageable.env_vars, image_name)
+  image_id = build_image.build(
+      py_executable, packageable.args, packageable.env_vars, image_name
+  )
   return local_executables.LoadedContainerImage(
-      name=packageable.executable_spec.name, image_id=image_id)
+      name=packageable.executable_spec.name, image_id=image_id
+  )
 
 
 def _package_bazel_container(
-    bazel_outputs: bazel_tools.TargetOutputs, packageable: xm.Packageable,
-    container: executables.BazelContainer) -> xm.Executable:
-  paths = bazel_outputs[bazel_client.BazelTarget(
-      label=container.label,
-      bazel_args=container.bazel_args,
-  )]
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    container: executables.BazelContainer,
+) -> xm.Executable:
+  """Matcher to package BazelContainer."""
+  paths = bazel_outputs[
+      bazel_client.BazelTarget(
+          label=container.label,
+          bazel_args=container.bazel_args,
+      )
+  ]
   assert len(paths) == 1
   image_id = docker_adapter.instance().load_image(paths[0])
   return local_executables.LoadedContainerImage(
       name=packageable.executable_spec.name,
       image_id=image_id,
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
-def _package_bazel_binary(bazel_outputs: bazel_tools.TargetOutputs,
-                          packageable: xm.Packageable,
-                          binary: executables.BazelBinary) -> xm.Executable:
-  paths = bazel_outputs[bazel_client.BazelTarget(
-      label=binary.label,
-      bazel_args=binary.bazel_args,
-  )]
+def _package_bazel_binary(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    binary: executables.BazelBinary,
+) -> xm.Executable:
+  """Matcher to package BazelBinary."""
+  paths = bazel_outputs[
+      bazel_client.BazelTarget(
+          label=binary.label,
+          bazel_args=binary.bazel_args,
+      )
+  ]
   assert len(paths) == 1
   return local_executables.LocalBinary(
       name=packageable.executable_spec.name,
       path=paths[0],
       args=packageable.args,
       env_vars=packageable.env_vars,
   )
 
 
-def _throw_on_unknown_executable(bazel_outputs: bazel_tools.TargetOutputs,
-                                 packageable: xm.Packageable, executable: Any):
+def _throw_on_unknown_executable(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,  # pylint: disable=unused-argument
+    executable: Any,
+):
   del bazel_outputs
-  raise TypeError('Unsupported executable specification '
-                  f'for local packaging: {executable!r}')
+  raise TypeError(
+      'Unsupported executable specification '
+      f'for local packaging: {executable!r}'
+  )
 
 
 _LOCAL_PACKAGING_ROUTER = pattern_matching.match(
     _package_bazel_binary,
     _package_bazel_container,
     _package_binary,
     _package_container,
     _package_dockerfile,
     _package_python_container,
     _throw_on_unknown_executable,
 )
 
 
-def package_for_local_executor(bazel_outputs: bazel_tools.TargetOutputs,
-                               packageable: xm.Packageable,
-                               executable_spec: xm.ExecutableSpec):
+def package_for_local_executor(
+    bazel_outputs: bazel_tools.TargetOutputs,
+    packageable: xm.Packageable,
+    executable_spec: xm.ExecutableSpec,
+):
   return _LOCAL_PACKAGING_ROUTER(bazel_outputs, packageable, executable_spec)
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/packaging/router.py` & `xmanager-0.4.0/xmanager/xm_local/packaging/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,18 @@
 
 
 def _throw_on_unknown_executor(
     bazel_outputs: bazel_tools.TargetOutputs,
     packageable: xm.Packageable,
     executor: Any,
 ):
-  raise TypeError(f'Unsupported executor specification: {executor!r}. '
-                  f'Packageable: {packageable!r}')
+  raise TypeError(
+      f'Unsupported executor specification: {executor!r}. '
+      f'Packageable: {packageable!r}'
+  )
 
 
 _PACKAGING_ROUTER = pattern_matching.match(
     _visit_vertex_spec,
     _visit_local_spec,
     _visit_kubernetes_spec,
     _throw_on_unknown_executor,
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/status.py` & `xmanager-0.4.0/xmanager/xm_local/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
   # Work unit terminated because it was cancelled by the user.
   CANCELLED = 4
 
 
 class LocalWorkUnitStatus(xm.ExperimentUnitStatus):
   """Status of a local experiment job."""
 
-  def __init__(self,
-               status: LocalWorkUnitStatusEnum,
-               message: str = '') -> None:
+  def __init__(
+      self, status: LocalWorkUnitStatusEnum, message: str = ''
+  ) -> None:
     super().__init__()
     self._status = status
     self._message = message
 
   @property
   def is_active(self) -> bool:
     return self._status == LocalWorkUnitStatusEnum.RUNNING
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/storage/alembic/env.py` & `xmanager-0.4.0/xmanager/xm_local/storage/alembic/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,35 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Alembic env.py."""
 
-from logging import config as logging_config
-
 from alembic import context
 from sqlalchemy import engine_from_config
 from sqlalchemy import pool
 
 config = context.config
 
-if config.config_file_name is not None:
-  logging_config.fileConfig(config.config_file_name)
-
 target_metadata = None
 
 
 def run_migrations_offline() -> None:
   """Run migrations in 'offline' mode.
 
-    This configures the context with just a URL
-    and not an Engine, though an Engine is acceptable
-    here as well.  By skipping the Engine creation
-    we don't even need a DBAPI to be available.
+  This configures the context with just a URL
+  and not an Engine, though an Engine is acceptable
+  here as well.  By skipping the Engine creation
+  we don't even need a DBAPI to be available.
   """
   url = config.get_main_option('sqlalchemy.url')
   context.configure(
       url=url,
       target_metadata=target_metadata,
       literal_binds=True,
       dialect_opts={'paramstyle': 'named'},
@@ -46,16 +41,16 @@
   with context.begin_transaction():
     context.run_migrations()
 
 
 def run_migrations_online() -> None:
   """Run migrations in 'online' mode.
 
-    In this scenario we need to create an Engine
-    and associate a connection with the context.
+  In this scenario we need to create an Engine
+  and associate a connection with the context.
   """
   connectable = config.attributes.get('connection', None)
 
   if connectable is None:
     connectable = engine_from_config(
         config.get_section(config.config_ini_section),
         prefix='sqlalchemy.',
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/storage/alembic/script.py.mako` & `xmanager-0.4.0/xmanager/xm_local/storage/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `xmanager-0.3.0/xmanager/xm_local/storage/alembic/versions/f45829405692_migrate_or_create.py` & `xmanager-0.4.0/xmanager/xm_local/storage/alembic/versions/f45829405692_migrate_or_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
   2. It's a new database with no tables.
     => Create tables
 
 Revision ID: f45829405692
 Revises:
 Create Date: 2022-09-16 10:50:41.096403
-
 """
 from alembic import op
 import sqlalchemy as sa
 from sqlalchemy.engine.reflection import Inspector
 
 # revision identifiers, used by Alembic.
 revision = 'f45829405692'
@@ -57,60 +56,66 @@
   table name is required.
   """
   with op.batch_alter_table('Experiment') as batch_op:
     batch_op.alter_column(
         column_name='Id',
         new_column_name='experiment_id',
         existing_type=sa.Integer(),
-        type_=sa.BigInteger())
+        type_=sa.BigInteger(),
+    )
 
     batch_op.alter_column(
         column_name='Title',
         new_column_name='experiment_title',
         existing_type=sa.TEXT,
-        type_=sa.String(255))
+        type_=sa.String(255),
+    )
   op.rename_table('Experiment', 'tmp_experiment')
   op.rename_table('tmp_experiment', 'experiment')
 
   with op.batch_alter_table('WorkUnit') as batch_op:
     batch_op.alter_column(
         column_name='ExperimentId',
         new_column_name='experiment_id',
         existing_type=sa.Integer(),
-        type_=sa.BigInteger())
+        type_=sa.BigInteger(),
+    )
 
     batch_op.alter_column(
         column_name='WorkUnitId',
         new_column_name='work_unit_id',
     )
   op.rename_table('WorkUnit', 'work_unit')
 
   with op.batch_alter_table('Job') as batch_op:
     batch_op.alter_column(
         column_name='ExperimentId',
         new_column_name='experiment_id',
         existing_type=sa.Integer(),
-        type_=sa.BigInteger())
+        type_=sa.BigInteger(),
+    )
 
     batch_op.alter_column(
         column_name='WorkUnitId',
         new_column_name='work_unit_id',
     )
 
     batch_op.alter_column(
         column_name='Name',
         new_column_name='job_name',
         existing_type=sa.TEXT,
-        type_=sa.String(255))
+        type_=sa.String(255),
+    )
 
     batch_op.alter_column(
         column_name='Data',
         new_column_name='job_data',
         existing_type=sa.TEXT,
-        type_=sa.String(255))
+        type_=sa.String(255),
+    )
   op.rename_table('Job', 'tmp_job')
   op.rename_table('tmp_job', 'job')
 
 
 def create_new_tables() -> None:
   """Creates tables for new database.
 
@@ -119,45 +124,54 @@
   """
   op.create_table(
       'experiment',
       sa.Column(
           'experiment_id',
           sa.BigInteger(),
           primary_key=True,
-          autoincrement=False), sa.Column('experiment_title', sa.String(255)))
+          autoincrement=False,
+      ),
+      sa.Column('experiment_title', sa.String(255)),
+  )
 
   op.create_table(
       'work_unit',
       sa.Column(
           'experiment_id',
           sa.BigInteger(),
           primary_key=True,
-          autoincrement=False),
-      sa.Column('work_unit_id', sa.Integer(), primary_key=True))
+          autoincrement=False,
+      ),
+      sa.Column('work_unit_id', sa.Integer(), primary_key=True),
+  )
 
   op.create_table(
       'job',
       sa.Column(
           'experiment_id',
           sa.BigInteger(),
           primary_key=True,
-          autoincrement=False),
+          autoincrement=False,
+      ),
       sa.Column('work_unit_id', sa.Integer(), primary_key=True),
       sa.Column('job_name', sa.String(255), primary_key=True),
-      sa.Column('job_data', sa.String(255)))
+      sa.Column('job_data', sa.String(255)),
+  )
 
 
 def upgrade() -> None:
   """Upgrades DB."""
   if using_legacy_sqlite_db():
     op.drop_table('VersionHistory')
 
     update_columns()
   else:
     create_new_tables()
 
 
 def downgrade() -> None:
   """Downgrades DB."""
-  raise RuntimeError('Downgrade operation is not supported: would downgrade '
-                     'to legacy SQLite schema using `VersionHistory` or to '
-                     ' empty database.')
+  raise RuntimeError(
+      'Downgrade operation is not supported: would downgrade '
+      'to legacy SQLite schema using `VersionHistory` or to '
+      ' empty database.'
+  )
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/storage/alembic.ini` & `xmanager-0.4.0/xmanager/xm_local/storage/alembic.ini`

 * *Files 18% similar despite different names*

```diff
@@ -78,42 +78,7 @@
 # detail and examples
 
 # format using "black" - use the console_scripts runner, against the "black" entrypoint
 # hooks = black
 # black.type = console_scripts
 # black.entrypoint = black
 # black.options = -l 79 REVISION_SCRIPT_FILENAME
-
-# Logging configuration
-[loggers]
-keys = root,sqlalchemy,alembic
-
-[handlers]
-keys = console
-
-[formatters]
-keys = generic
-
-[logger_root]
-level = WARN
-handlers = console
-qualname =
-
-[logger_sqlalchemy]
-level = WARN
-handlers =
-qualname = sqlalchemy.engine
-
-[logger_alembic]
-level = INFO
-handlers =
-qualname = alembic
-
-[handler_console]
-class = StreamHandler
-args = (sys.stderr,)
-level = NOTSET
-formatter = generic
-
-[formatter_generic]
-format = %(levelname)-5.5s [%(name)s] %(message)s
-datefmt = %H:%M:%S
```

### Comparing `xmanager-0.3.0/xmanager/xm_local/storage/database.py` & `xmanager-0.4.0/xmanager/xm_local/storage/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import yaml
 
 from google.protobuf import text_format
 
 from google.cloud.sql.connector import Connector, IPTypes
 
 _DB_YAML_CONFIG_PATH = flags.DEFINE_string(
-    'xm_db_yaml_config_path', None, """
+    'xm_db_yaml_config_path',
+    None,
+    """
     Path of YAML config file containing DB connection details.
 
     A valid config file contains two main entries:
       `sql_connector`: must be one of [`sqlite`, `generic`, `cloudsql`]
 
       `sql_connection_settings`: contains details about the connection URL.
         These match the interface of `SqlConnectionSettings` and their
@@ -44,48 +46,55 @@
           - backend, e.g. 'mysql', 'postgresql'
           - db_name
           - driver, e.g. 'pymysql', 'pg8000'
           - username
           - password
           - host (instance connection name when using CloudSql)
           - port
-    """)
+    """,
+)
 
 _UPGRADE_DB = flags.DEFINE_boolean(
-    'xm_upgrade_db', False, """
+    'xm_upgrade_db',
+    False,
+    """
     Specifies if XManager should update the database to the latest version.
     It's recommended to take a back-up of the database before updating, since
     migrations can fail/have errors. This is especially true
     for non-transactional DDLs, where partial migrations can occur on
     failure, leaving the database in a not well-defined state.
-    """)
+    """,
+)
 
 
 @attr.s(auto_attribs=True)
 class WorkUnitResult:
   """Result of a WorkUnit database query."""
+
   work_unit_id: int
   jobs: Dict[str, data_pb2.Job]
 
 
 @attr.s(auto_attribs=True)
 class ExperimentResult:
   """Result of an Experiment database query."""
+
   experiment_id: int
   experiment_title: str
   work_units: List[WorkUnitResult]
 
 
 Engine = sqlalchemy.engine.Engine
 text = sqlalchemy.sql.text
 
 
 @attr.s(auto_attribs=True)
 class SqlConnectionSettings:
   """Settings for a generic SQL connection."""
+
   backend: str
   db_name: str
   driver: Optional[str] = None
   username: Optional[str] = None
   password: Optional[str] = None
   host: Optional[str] = None
   port: Optional[int] = None
@@ -104,40 +113,43 @@
 
 
 class GenericSqlConnector(SqlConnector):
   """Generic way of connecting to SQL databases using an URL."""
 
   @staticmethod
   def create_engine(settings: SqlConnectionSettings) -> Engine:
-    driver_name = settings.backend + (f'+{settings.driver}'
-                                      if settings.driver else '')
+    driver_name = settings.backend + (
+        f'+{settings.driver}' if settings.driver else ''
+    )
 
     url = sqlalchemy.engine.url.URL(
         drivername=driver_name,
         username=settings.username,
         password=settings.password,
         host=settings.host,
         port=settings.port,
-        database=settings.db_name)
+        database=settings.db_name,
+    )
 
     return sqlalchemy.engine.create_engine(url)
 
 
 class SqliteConnector(SqlConnector):
   """Provides way of connecting to a SQLite database.
 
   The database used at the file path pointed to by the `database` field
   in the settings used. The database is created if it doesn't exist.
   """
 
   @staticmethod
   def create_engine(settings: SqlConnectionSettings) -> Engine:
     if settings.backend and settings.backend != 'sqlite':
-      raise RuntimeError('Can\'t use SqliteConnector with a backend'
-                         'other than `sqlite`')
+      raise RuntimeError(
+          "Can't use SqliteConnector with a backendother than `sqlite`"
+      )
 
     if not os.path.isdir(os.path.dirname(settings.db_name)):
       os.makedirs(os.path.dirname(settings.db_name))
 
     return GenericSqlConnector.create_engine(settings)
 
 
@@ -178,26 +190,28 @@
                                     host='localhost')
     return sqlalchemy.create_engine(url, creator=get_connection)
 
 
 class Database:
   """Database object with interacting with experiment metadata storage."""
 
-  def __init__(self, connector: Type[TSqlConnector],
-               settings: SqlConnectionSettings):
+  def __init__(
+      self, connector: Type[TSqlConnector], settings: SqlConnectionSettings
+  ):
     self.settings = settings
     self.engine: Engine = connector.create_engine(settings)
     # https://github.com/sqlalchemy/sqlalchemy/issues/5645
     # TODO: Remove this line after using sqlalchemy>=1.14.
     self.engine.dialect.description_encoding = None
     storage_dir = os.path.dirname(__file__)
     self.alembic_cfg = Config(os.path.join(storage_dir, 'alembic.ini'))
     self.alembic_cfg.set_main_option('sqlalchemy.url', str(self.engine.url))
-    self.alembic_cfg.set_main_option('script_location',
-                                     os.path.join(storage_dir, 'alembic'))
+    self.alembic_cfg.set_main_option(
+        'script_location', os.path.join(storage_dir, 'alembic')
+    )
 
     self.maybe_migrate_database_version()
 
   def upgrade_database(self, revision: str = 'head') -> None:
     """Upgrades database to given revision."""
     with self.engine.begin() as connection:
       # https://alembic.sqlalchemy.org/en/latest/cookbook.html#sharing-a-connection-across-one-or-more-programmatic-migration-commands
@@ -205,156 +219,192 @@
       self.alembic_cfg.attributes['connection'] = connection
       try:
         alembic.command.upgrade(self.alembic_cfg, revision)
       except Exception as e:
         raise RuntimeError(
             'Database upgrade failed. The DB may be in an undefined state or '
             'data may have been lost. Revert to the previous state using your '
-            'backup or proceed with caution.') from e
+            'backup or proceed with caution.'
+        ) from e
       finally:
         self.alembic_cfg.attributes['connection'] = None
 
   def database_version(self) -> str:
     with self.engine.begin() as connection:
       context = alembic.migration.MigrationContext.configure(connection)
       return context.get_current_revision()
 
   def latest_version_available(self) -> str:
     script_directory = alembic.script.ScriptDirectory.from_config(
-        self.alembic_cfg)
+        self.alembic_cfg
+    )
     return script_directory.get_current_head()
 
   def maybe_migrate_database_version(self):
     """Enforces the latest version of the database to be used."""
     db_version = self.database_version()
-    legacy_sqlite_db = self.engine.dialect.has_table(self.engine,
-                                                     'VersionHistory')
-
-    need_to_update = (db_version != self.latest_version_available() and
-                      db_version) or legacy_sqlite_db
+    legacy_sqlite_db = self.engine.dialect.has_table(
+        self.engine, 'VersionHistory'
+    )
+
+    need_to_update = (
+        db_version != self.latest_version_available() and db_version
+    ) or legacy_sqlite_db
     if need_to_update and not _UPGRADE_DB.value:
       raise RuntimeError(
           f'Database is not up to date: current={self.database_version()}, '
           f'latest={self.latest_version_available()}. Take a backup of the '
           'database and then launch using the `--xm_upgrade_db` flag '
-          'to update to the the latest version.')
+          'to update to the the latest version.'
+      )
     self.upgrade_database()
 
-  def insert_experiment(self, experiment_id: int,
-                        experiment_title: str) -> None:
-    query = text('INSERT INTO experiment (experiment_id, experiment_title) '
-                 'VALUES (:experiment_id, :experiment_title)')
+  def insert_experiment(
+      self, experiment_id: int, experiment_title: str
+  ) -> None:
+    query = text(
+        'INSERT INTO experiment (experiment_id, experiment_title) '
+        'VALUES (:experiment_id, :experiment_title)'
+    )
     self.engine.execute(
-        query, experiment_id=experiment_id, experiment_title=experiment_title)
+        query, experiment_id=experiment_id, experiment_title=experiment_title
+    )
 
   def insert_work_unit(self, experiment_id: int, work_unit_id: int) -> None:
-    query = text('INSERT INTO work_unit (experiment_id, work_unit_id) '
-                 'VALUES (:experiment_id, :work_unit_id)')
+    query = text(
+        'INSERT INTO work_unit (experiment_id, work_unit_id) '
+        'VALUES (:experiment_id, :work_unit_id)'
+    )
     self.engine.execute(
-        query, experiment_id=experiment_id, work_unit_id=work_unit_id)
+        query, experiment_id=experiment_id, work_unit_id=work_unit_id
+    )
 
-  def insert_vertex_job(self, experiment_id: int, work_unit_id: int,
-                        vertex_job_id: str) -> None:
+  def insert_vertex_job(
+      self, experiment_id: int, work_unit_id: int, vertex_job_id: str
+  ) -> None:
     job = data_pb2.Job(caip=data_pb2.AIPlatformJob(resource_name=vertex_job_id))
     data = text_format.MessageToBytes(job)
-    query = text('INSERT INTO '
-                 'job (experiment_id, work_unit_id, job_name, job_data) '
-                 'VALUES (:experiment_id, :work_unit_id, :job_name, :job_data)')
+    query = text(
+        'INSERT INTO '
+        'job (experiment_id, work_unit_id, job_name, job_data) '
+        'VALUES (:experiment_id, :work_unit_id, :job_name, :job_data)'
+    )
     self.engine.execute(
         query,
         experiment_id=experiment_id,
         work_unit_id=work_unit_id,
         job_name=vertex_job_id,
-        job_data=data)
+        job_data=data,
+    )
 
-  def insert_kubernetes_job(self, experiment_id: int, work_unit_id: int,
-                            namespace: str, job_name: str) -> None:
+  def insert_kubernetes_job(
+      self, experiment_id: int, work_unit_id: int, namespace: str, job_name: str
+  ) -> None:
+    """Insert a Kubernetes job into the database."""
     job = data_pb2.Job(
         kubernetes=data_pb2.KubernetesJob(
-            namespace=namespace, job_name=job_name))
+            namespace=namespace, job_name=job_name
+        )
+    )
     data = text_format.MessageToString(job)
-    query = text('INSERT INTO '
-                 'job (experiment_id, work_unit_id, job_name, job_data) '
-                 'VALUES (:experiment_id, :work_unit_id, :job_name, :job_data)')
+    query = text(
+        'INSERT INTO '
+        'job (experiment_id, work_unit_id, job_name, job_data) '
+        'VALUES (:experiment_id, :work_unit_id, :job_name, :job_data)'
+    )
     self.engine.execute(
         query,
         experiment_id=experiment_id,
         work_unit_id=work_unit_id,
         job_name=job_name,
-        job_data=data)
+        job_data=data,
+    )
 
   def list_experiment_ids(self) -> List[int]:
     """Lists all the experiment ids from local database."""
     query = text('SELECT experiment_id FROM experiment')
     rows = self.engine.execute(query)
     return [r['experiment_id'] for r in rows]
 
   def get_experiment(self, experiment_id: int) -> ExperimentResult:
     """Gets an experiment from local database."""
-    query = text('SELECT experiment_title FROM experiment '
-                 'WHERE experiment_id=:experiment_id')
+    query = text(
+        'SELECT experiment_title FROM experiment '
+        'WHERE experiment_id=:experiment_id'
+    )
     rows = self.engine.execute(query, experiment_id=experiment_id)
     title = None
     for r in rows:
       title = r['experiment_title']
       break
     if title is None:
-      raise ValueError(f'Experiment Id {experiment_id} doesn\'t exist.')
-    return ExperimentResult(experiment_id, title,
-                            self.list_work_units(experiment_id))
+      raise ValueError(f"Experiment Id {experiment_id} doesn't exist.")
+    return ExperimentResult(
+        experiment_id, title, self.list_work_units(experiment_id)
+    )
 
   def list_work_units(self, experiment_id: int) -> List[WorkUnitResult]:
     """Lists an experiment's work unit ids from local database."""
-    query = text('SELECT work_unit_id '
-                 'FROM work_unit WHERE experiment_id=:experiment_id')
+    query = text(
+        'SELECT work_unit_id FROM work_unit WHERE experiment_id=:experiment_id'
+    )
     rows = self.engine.execute(query, experiment_id=experiment_id)
     return [self.get_work_unit(experiment_id, r['work_unit_id']) for r in rows]
 
-  def get_work_unit(self, experiment_id: int,
-                    work_unit_id: int) -> WorkUnitResult:
+  def get_work_unit(
+      self, experiment_id: int, work_unit_id: int
+  ) -> WorkUnitResult:
     """Gets a work unit from local database."""
-    query = text('SELECT job_name, job_data FROM job '
-                 'WHERE experiment_id=:experiment_id '
-                 'AND work_unit_id=:work_unit_id')
+    query = text(
+        'SELECT job_name, job_data FROM job '
+        'WHERE experiment_id=:experiment_id '
+        'AND work_unit_id=:work_unit_id'
+    )
     rows = self.engine.execute(
-        query, experiment_id=experiment_id, work_unit_id=work_unit_id)
+        query, experiment_id=experiment_id, work_unit_id=work_unit_id
+    )
     jobs = {}
     for r in rows:
       job = data_pb2.Job()
       jobs[r['job_name']] = text_format.Parse(r['job_data'], job)
     return WorkUnitResult(work_unit_id, jobs)
 
 
 def sqlite_settings(
-    db_file='~/.xmanager/experiments.sqlite3') -> SqlConnectionSettings:
+    db_file='~/.xmanager/experiments.sqlite3',
+) -> SqlConnectionSettings:
   return SqlConnectionSettings(
-      backend='sqlite', db_name=os.path.expanduser(db_file))
+      backend='sqlite', db_name=os.path.expanduser(db_file)
+  )
 
 
 _SUPPORTED_CONNECTORS = ['sqlite', 'generic', 'cloudsql']
 
 
 def _validate_db_config(config: Dict[str, Any]) -> None:
   if 'sql_connector' not in config:
     raise RuntimeError('DB YAML config must contain `sql_connector` entry')
   if config['sql_connector'] not in _SUPPORTED_CONNECTORS:
     raise RuntimeError(
-        f'`sql_connector` must be one of: {_SUPPORTED_CONNECTORS}')
+        f'`sql_connector` must be one of: {_SUPPORTED_CONNECTORS}'
+    )
 
   if 'sql_connection_settings' not in config:
-    raise RuntimeError('DB YAML config must contain '
-                       '`sql_connection_settings` entry')
+    raise RuntimeError(
+        'DB YAML config must contain `sql_connection_settings` entry'
+    )
 
 
 @functools.lru_cache()
 def _db_config() -> Dict[str, Any]:
   """Parses and validates YAML DB config file to a dict."""
   if _DB_YAML_CONFIG_PATH.value is not None:
     db_config_file = xm.utils.resolve_path_relative_to_launcher(
-        _DB_YAML_CONFIG_PATH.value)
+        _DB_YAML_CONFIG_PATH.value
+    )
     with open(db_config_file, 'r') as f:
       config = yaml.safe_load(f)
       _validate_db_config(config)
       return config
 
   return {}
```

### Comparing `xmanager-0.3.0/xmanager/xm_mock/__init__.py` & `xmanager-0.4.0/xmanager/xm_mock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,17 +93,20 @@
     self._launched_jobs = launched_jobs
     self._launched_jobs_args = launched_jobs_args
     self._work_unit_id = work_unit_id_predictor.reserve_id()
 
   async def _wait_until_complete(self) -> None:
     """Mock work unit is immediately complete."""
 
-  async def _launch_job_group(self, job_group: job_blocks.JobGroup,
-                              args: Optional[Mapping[str, Any]],
-                              identity: str) -> None:
+  async def _launch_job_group(
+      self,
+      job_group: job_blocks.JobGroup,
+      args: Optional[Mapping[str, Any]],
+      identity: str,
+  ) -> None:
     """Appends the job group to the launched_jobs list."""
     self._launched_jobs.extend(job_group.jobs.values())
     self._launched_jobs_args.append(args)
 
   @property
   def work_unit_id(self) -> int:
     return self._work_unit_id
@@ -129,27 +132,38 @@
 
     self._context = MockMetadataContext()
 
   def _create_experiment_unit(
       self,
       args: Optional[Mapping[str, Any]],
       role: core.ExperimentUnitRole = core.WorkUnitRole(),
-      identity: str = '') -> Awaitable[MockExperimentUnit]:
+      identity: str = '',
+  ) -> Awaitable[MockExperimentUnit]:
     """Creates a new WorkUnit instance for the experiment."""
     del identity  # Unused.
     future = asyncio.Future(loop=self._event_loop)
-    experiment_unit = MockExperimentUnit(self, self._work_unit_id_predictor,
-                                         self._create_task, self.launched_jobs,
-                                         self.launched_jobs_args, args, role)
+    experiment_unit = MockExperimentUnit(
+        self,
+        self._work_unit_id_predictor,
+        self._create_task,
+        self.launched_jobs,
+        self.launched_jobs_args,
+        args,
+        role,
+    )
     pm.match(
-        pm.Case([core.WorkUnitRole],
-                lambda _: self._work_units.append(experiment_unit)),
-        pm.Case([core.AuxiliaryUnitRole],
-                lambda _: self._auxiliary_units.append(experiment_unit)))(
-                    role)
+        pm.Case(
+            [core.WorkUnitRole],
+            lambda _: self._work_units.append(experiment_unit),
+        ),
+        pm.Case(
+            [core.AuxiliaryUnitRole],
+            lambda _: self._auxiliary_units.append(experiment_unit),
+        ),
+    )(role)
 
     future.set_result(experiment_unit)
     return future
 
   @property
   def work_unit_count(self) -> int:
     return len(self.work_units)
@@ -170,14 +184,15 @@
   def context(self) -> MockMetadataContext:
     """Returns metadata context for the experiment."""
     return self._context
 
 
 class MockExecutable(job_blocks.Executable):
   """A mock version of Executable with abstract methods implemented."""
+
   counter = 0
 
   def __init__(self):
     super().__init__(name=f'{MockExecutable.counter}')
     MockExecutable.counter += 1
```

### Comparing `xmanager-0.3.0/xmanager.egg-info/PKG-INFO` & `xmanager-0.4.0/xmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xmanager
-Version: 0.3.0
+Version: 0.4.0
 Summary: A framework for managing machine learning experiments
 Author: DeepMind Technologies Limited
 Project-URL: Homepage, https://github.com/deepmind/xmanager
 Project-URL: Issue tracker, https://github.com/deepmind/xmanager/issues
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XManager: A framework for managing machine learning experiments 🧑‍🔬
 
 <!-- Note that links in README.md have to be absolute as it also lands on PyPI. -->
```

### Comparing `xmanager-0.3.0/xmanager.egg-info/SOURCES.txt` & `xmanager-0.4.0/xmanager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 xmanager/cloud/vertex_test.py
 xmanager/cloud/data/wrapped_entrypoint.sh
 xmanager/contrib/__init__.py
 xmanager/contrib/addressing.py
 xmanager/contrib/addressing_test.py
 xmanager/contrib/copybara.py
 xmanager/contrib/executor_selector.py
+xmanager/contrib/flow.py
 xmanager/contrib/framework_defaults.py
 xmanager/contrib/framework_defaults_test.py
 xmanager/contrib/gcs.py
 xmanager/contrib/gcs_test.py
 xmanager/contrib/parameter_controller.py
 xmanager/contrib/tensorboard.py
 xmanager/contrib/tensorboard_test.py
```

