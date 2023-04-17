# Comparing `tmp/fractal_server-1.2.0a4.tar.gz` & `tmp/fractal_server-1.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.0a4.tar", max compression
+gzip compressed data, was "fractal_server-1.2.0a5.tar", max compression
```

## Comparing `fractal_server-1.2.0a4.tar` & `fractal_server-1.2.0a5.tar`

### file list

```diff
@@ -1,117 +1,120 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a4/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a4/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a4/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-04-14 12:56:29.081164 fractal_server-1.2.0a4/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a4/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21983 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11794 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2724 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a4/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a4/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8144 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    20882 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     4510 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3690 2023-04-13 13:38:10.605758 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-14 08:28:41.981553 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    18410 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    40101 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9749 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a4/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a4/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a4/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a4/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a4/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a4/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a4/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    13225 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/logger.py
--rw-r--r--   0        0        0     4969 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a4/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a4/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a4/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a4/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a4/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12782 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-04-14 12:56:29.081164 fractal_server-1.2.0a4/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a4/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a5/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a5/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a5/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-17 13:34:41.336202 fractal_server-1.2.0a5/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a5/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a5/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a5/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a5/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a5/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a5/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    21983 2023-04-14 12:55:14.842206 fractal_server-1.2.0a5/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    11794 2023-04-14 12:55:14.842206 fractal_server-1.2.0a5/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2724 2023-04-14 12:55:14.842206 fractal_server-1.2.0a5/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a5/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a5/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8187 2023-04-17 11:49:54.893488 fractal_server-1.2.0a5/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19294 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5460 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3796 2023-04-17 11:49:54.893488 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-14 08:28:41.981553 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19745 2023-04-17 11:49:54.893488 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-04-14 12:55:14.842206 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    40272 2023-04-17 11:49:54.893488 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9749 2023-04-14 12:55:14.846206 fractal_server-1.2.0a5/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a5/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a5/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a5/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a5/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a5/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a5/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a5/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a5/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a5/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a5/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a5/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a5/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a5/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a5/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a5/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a5/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a5/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a5/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12079 2023-04-17 13:34:24.748408 fractal_server-1.2.0a5/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.0a5/fractal_server/logger.py
+-rw-r--r--   0        0        0     4969 2023-04-14 12:55:14.846206 fractal_server-1.2.0a5/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a5/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a5/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a5/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a5/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a5/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.0a5/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12782 2023-04-14 12:55:14.846206 fractal_server-1.2.0a5/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-04-14 12:55:14.846206 fractal_server-1.2.0a5/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-17 13:34:41.336202 fractal_server-1.2.0a5/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a5/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a5/PKG-INFO
```

### Comparing `fractal_server-1.2.0a4/LICENSE` & `fractal_server-1.2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/README.md` & `fractal_server-1.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/__main__.py` & `fractal_server-1.2.0a5/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/alembic.ini` & `fractal_server-1.2.0a5/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/api/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.0a5/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.0a5/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.0a5/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.0a5/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/db/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/job.py` & `fractal_server-1.2.0a5/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/project.py` & `fractal_server-1.2.0a5/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/security.py` & `fractal_server-1.2.0a5/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/state.py` & `fractal_server-1.2.0a5/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/task.py` & `fractal_server-1.2.0a5/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/models/workflow.py` & `fractal_server-1.2.0a5/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     try:
         output_dataset.meta = await process_workflow(
             workflow=workflow,
             input_paths=input_paths,
             output_path=output_path,
             input_metadata=input_dataset.meta,
             slurm_user=slurm_user,
+            user_cache_dir=user_cache_dir,
             workflow_dir=WORKFLOW_DIR,
             workflow_dir_user=WORKFLOW_DIR_USER,
             logger_name=logger_name,
             worker_init=worker_init,
         )
 
         logger.debug(f'END workflow "{workflow.name}"')
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_common.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 from concurrent.futures import Executor
 from concurrent.futures import Future
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
 from shlex import split as shlex_split
 from typing import Callable
-from typing import Generator
 from typing import Optional
 
-from ...config import get_settings
 from ...logger import get_logger
-from ...syringe import Inject
 from ..models import WorkflowTask
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import TaskParameters
 from .common import write_args_file
 
 
@@ -47,30 +44,14 @@
     """
     Remove {" ", "/", "."} form a string, e.g. going from
     'plate.zarr/B/03/0' to 'plate_zarr_B_03_0'.
     """
     return value.replace(" ", "_").replace("/", "_").replace(".", "_")
 
 
-def _get_list_chunks(mylist: list, *, chunksize: Optional[int]) -> Generator:
-    """
-    Split a list into several chunks of maximum size `chunksize`. If
-    `chunksize` is `None`, return a single chunk with the whole list.
-
-    Arguments:
-        mylist: The list to be splitted
-        chunksize: The maximum size of each chunk
-    """
-    if chunksize is None:
-        yield mylist
-    else:
-        for ind_chunk in range(0, len(mylist), chunksize):
-            yield mylist[ind_chunk : ind_chunk + chunksize]  # noqa: E203
-
-
 class TaskFiles:
     """
     Group all file paths pertaining to a task
 
     Attributes:
         workflow_dir:
             Server-owned directory to store all task-execution-related relevant
@@ -394,17 +375,15 @@
     submit_setup_call: Callable = no_op_submit_setup_call,
 ) -> Future:  # py3.9 Future[TaskParameters]:
     """
     Collect results from the parallel instances of a parallel task
 
     Prepare and submit for execution all the single calls of a parallel task,
     and return a single future with the TaskParameters to be passed on to the
-    next task.  Note that the configuration variable
-    [`FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW`](../../../../../configuration/#fractal_server.config.Settings.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW)
-    may affect the internal behavior of this function.
+    next task.
 
     **Note**: This function returns a future which already has
     `out_future.done()=True` (that is, this function is blocking and it
     returns only after the task is over). The reason for returning a future
     instead of a `TaskParameter` object is for compatibility with the output of
     `executor.submit(call_single_task, ...)`.
 
@@ -449,38 +428,21 @@
         call_single_parallel_task,
         wftask=wftask,
         task_pars=task_pars_depend,
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
     )
 
-    # Depending on FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW, either submit
-    # all tasks at once or in smaller chunks.  Note that `for _ in map_iter:
+    # Submit tasks for execution. Note that `for _ in map_iter:
     # pass` explicitly calls the .result() method for each future, and
     # therefore is blocking until the task are complete.
-    settings = Inject(get_settings)
-    max_parallel_tasks = None
-    if settings.FRACTAL_RUNNER_BACKEND == "local":
-        max_parallel_tasks = (
-            settings.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW
-        )
-    # Prepare generator of component chunks (this is just a single item if
-    # FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW is None)
-    component_chunks_generator = _get_list_chunks(
-        component_list,
-        chunksize=max_parallel_tasks,
-    )
-    for component_chunk in component_chunks_generator:
-        # Submit this chunk of tasks for execution
-        map_iter = executor.map(
-            partial_call_task, component_chunk, **extra_setup
-        )
-        # Wait for execution of this chunk of tasks
-        for _ in map_iter:
-            pass  # noqa: 701
+    map_iter = executor.map(partial_call_task, component_list, **extra_setup)
+    # Wait for execution of this chunk of tasks
+    for _ in map_iter:
+        pass  # noqa: 701
 
     # Assemble a Future[TaskParameter]
     history = f"{wftask.task.name}: {component_list}"
     try:
         task_pars_depend.metadata["history"].append(history)
     except KeyError:
         task_pars_depend.metadata["history"] = [history]
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_local/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,71 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
 Local Bakend
 
-This backend runs Fractal workflows using python
-[ThreadPoolExecutor](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor)
-to run tasks in several threads. Incidentally, it also represents the reference
-implementation for a backend.
+This backend runs Fractal workflows using `FractalThreadPoolExecutor` (a custom
+version of Python
+[ThreadPoolExecutor](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor))
+to run tasks in several threads.
+Incidentally, it also represents the reference implementation for a backend.
 """
-from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from typing import Any
 from typing import Optional
 
 from ...models import Workflow
 from .._common import recursive_task_submission
 from ..common import async_wrap
 from ..common import TaskParameters
+from ._submit_setup import _local_submit_setup
+from .executor import FractalThreadPoolExecutor
 
 
 def _process_workflow(
     *,
     workflow: Workflow,
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
 ) -> dict[str, Any]:
     """
     Internal processing routine
 
-    Schedules the workflow using a ThreadPoolExecutor.
+    Schedules the workflow using a `FractalThreadPoolExecutor`.
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
     for the call signature.
     """
 
-    with ThreadPoolExecutor() as executor:
+    with FractalThreadPoolExecutor() as executor:
         output_task_pars_fut = recursive_task_submission(
             executor=executor,
             task_list=workflow.task_list,
             task_pars=TaskParameters(
                 input_paths=input_paths,
                 output_path=output_path,
                 metadata=input_metadata,
             ),
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir,
             logger_name=logger_name,
+            submit_setup_call=_local_submit_setup,
         )
     output_task_pars = output_task_pars_fut.result()
     output_dataset_metadata = output_task_pars.metadata
     return output_dataset_metadata
 
 
 async def process_workflow(
@@ -59,14 +74,15 @@
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     slurm_user: Optional[str] = None,
+    user_cache_dir: Optional[str] = None,
     worker_init: Optional[str] = None,
 ) -> dict[str, Any]:
     """
     Run a workflow
 
     This function is responsible for running a workflow on some input data,
     saving the output and taking care of any exception raised during the run.
@@ -92,14 +108,18 @@
             Working directory for this run, on the user side. This argument is
             present for compatibility with the standard backend interface, but
             for the `local` backend it cannot be different from `workflow_dir`.
         slurm_user:
             Username to impersonate to run the workflow. This argument is
             present for compatibility with the standard backend interface, but
             is ignored in the `local` backend.
+        user_cache_dir:
+            Cache directory of the user who will run the workflow. This
+            argument is present for compatibility with the standard backend
+            interface, but is ignored in the `local` backend.
         worker_init:
             Any additional, usually backend specific, information to be passed
             to the backend executor. This argument is present for compatibility
             with the standard backend interface, but is ignored in the `local`
             backend.
 
     Raises:
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Path,
     slurm_user: Optional[str] = None,
+    user_cache_dir: str,
     worker_init: Optional[Union[str, list[str]]] = None,
 ) -> dict[str, Any]:
     """
     Internal processing routine for the SLURM backend
 
     This function initialises the a FractalSlurmExecutor, setting logging,
     workflow working dir and user to impersonate. It then schedules the
@@ -92,14 +93,15 @@
     workflow: Workflow,
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
+    user_cache_dir: Optional[str] = None,
     slurm_user: Optional[str] = None,
     worker_init: Optional[str] = None,
 ) -> dict[str, Any]:
     """
     Process workflow (SLURM backend public interface)
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
@@ -109,10 +111,11 @@
         input_paths=input_paths,
         output_path=output_path,
         input_metadata=input_metadata,
         logger_name=logger_name,
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         slurm_user=slurm_user,
+        user_cache_dir=user_cache_dir,
         worker_init=worker_init,
     )
     return output_dataset_metadata
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -109,32 +109,41 @@
       "batching_config": {
           "target_cpus_per_job": 1,
           "max_cpus_per_job": 1,
           "target_mem_per_job": 200,
           "max_mem_per_job": 500,
           "target_num_jobs": 2,
           "max_num_jobs": 4
+      },
+      "user_local_exports": {
+          "CELLPOSE_LOCAL_MODELS_PATH": "CELLPOSE_LOCAL_MODELS_PATH",
+          "NAPARI_CONFIG": "napari_config.json"
       }
     }
     ```
 
     See `_SlurmConfigSet` and `_BatchingConfigSet` for more details.
 
     Attributes:
         default_slurm_config:
             Common default options for all tasks.
         gpu_slurm_config:
             Default configuration for all GPU tasks.
         batching_config:
             Configuration of the batching strategy.
+        user_local_exports:
+            Key-value pairs to be included as `export`-ed variables in SLURM
+            submission script, after prepending values with the user's cache
+            directory.
     """
 
     default_slurm_config: _SlurmConfigSet
     gpu_slurm_config: Optional[_SlurmConfigSet]
     batching_config: _BatchingConfigSet
+    user_local_exports: Optional[dict[str, str]]
 
 
 def load_slurm_config_file(
     config_path: Optional[Path] = None,
 ) -> SlurmConfigFile:
     """
     Load a SLURM configuration file and validate its content with
@@ -218,14 +227,18 @@
                           SLURM job.
         target_mem_per_job: Optimal amount of memory (in MB) to be requested in
                             each SLURM job.
         max_mem_per_job: Maximum amount of memory (in MB) that can be requested
                          in each SLURM job.
         target_num_jobs: Optimal number of SLURM jobs for a given WorkflowTask.
         max_num_jobs: Maximum number of SLURM jobs for a given WorkflowTask.
+        user_local_exports:
+            Key-value pairs to be included as `export`-ed variables in SLURM
+            submission script, after prepending values with the user's cache
+            directory.
     """
 
     # Required SLURM parameters (note that the integer attributes are those
     # that will need to scale up with the number of parallel tasks per job)
     partition: str
     cpus_per_task: int
     mem_per_task_MB: int
@@ -239,14 +252,17 @@
     time: Optional[str] = None
     account: Optional[str] = None
 
     # Free-field attribute for extra lines to be added to the SLURM job
     # preamble
     extra_lines: Optional[list[str]] = Field(default_factory=list)
 
+    # Variables that will be `export`ed in the SLURM submission script
+    user_local_exports: Optional[dict[str, str]] = None
+
     # Metaparameters needed to combine multiple tasks in each SLURM job
     tasks_per_job: Optional[int] = None
     parallel_tasks_per_job: Optional[int] = None
     target_cpus_per_job: int
     max_cpus_per_job: int
     target_mem_per_job: int
     max_mem_per_job: int
@@ -285,18 +301,26 @@
             elif _line.startswith(self.prefix):
                 return 1
             else:
                 return 2
 
         return sorted(script_lines, key=_sorting_function)
 
-    def to_sbatch_preamble(self) -> list[str]:
+    def to_sbatch_preamble(
+        self,
+        user_cache_dir: Optional[str] = None,
+    ) -> list[str]:
         """
         Compile `SlurmConfig` object into the preamble of a SLURM submission
         script.
+
+        Arguments:
+            user_cache_dir:
+                Base directory for exports defined in
+                `self.user_local_exports`.
         """
         if self.parallel_tasks_per_job is None:
             raise ValueError(
                 "SlurmConfig.sbatch_preamble requires that "
                 f"{self.parallel_tasks_per_job=} is not None."
             )
         if self.extra_lines:
@@ -327,14 +351,23 @@
                 option = key.replace("_", "-")
                 lines.append(f"{self.prefix} --{option}={value}")
 
         if self.extra_lines:
             for line in self._sorted_extra_lines():
                 lines.append(line)
 
+        if self.user_local_exports:
+            if user_cache_dir is None:
+                raise ValueError(
+                    f"user_cache_dir=None but {self.user_local_exports=}"
+                )
+            for key, value in self.user_local_exports.items():
+                tmp_value = str(Path(user_cache_dir) / value)
+                lines.append(f"export {key}={tmp_value}")
+
         """
         FIXME export SRUN_CPUS_PER_TASK
         # From https://slurm.schedmd.com/sbatch.html: Beginning with 22.05,
         # srun will not inherit the --cpus-per-task value requested by salloc
         # or sbatch.  It must be requested again with the call to srun or set
         # with the SRUN_CPUS_PER_TASK environment variable if desired for the
         # task(s).
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,24 +168,26 @@
         map_jobid_to_slurm_files:
             Dictionary with paths of slurm-related files for active jobs
     """
 
     wait_thread_cls = FractalSlurmWaitThread
     slurm_user: str
     common_script_lines: list[str]
+    user_cache_dir: str
     working_dir: Path
     working_dir_user: Path
     map_jobid_to_slurm_files: dict[str, tuple[str, str, str]]
     keep_pickle_files: bool
 
     def __init__(
         self,
         slurm_user: str,
         working_dir: Optional[Path] = None,
         working_dir_user: Optional[Path] = None,
+        user_cache_dir: Optional[str] = None,
         common_script_lines: Optional[list[str]] = None,
         slurm_poll_interval: Optional[int] = None,
         keep_pickle_files: bool = False,
         *args,
         **kwargs,
     ):
         """
@@ -211,14 +213,15 @@
                 raise RuntimeError(f"{self.slurm_user=}, {working_dir_user=}")
             else:
                 working_dir_user = working_dir
         if not _path_exists_as_user(
             path=str(working_dir_user), user=self.slurm_user
         ):
             logger.info(f"Missing folder {working_dir_user=}")
+        self.user_cache_dir = user_cache_dir
 
         self.working_dir_user = working_dir_user
         self.map_jobid_to_slurm_files = {}
 
         # Set the attribute slurm_poll_interval for self.wait_thread (see
         # cfut.SlurmWaitThread)
         if not slurm_poll_interval:
@@ -1018,15 +1021,17 @@
             slurm_config.parallel_tasks_per_job = ntasks
             logger.debug(
                 f"{len(list_commands)=} is smaller than "
                 f"{num_tasks_max_running=}. Setting {ntasks=}."
             )
 
         # Prepare SLURM preamble based on SlurmConfig object
-        script_lines = slurm_config.to_sbatch_preamble()
+        script_lines = slurm_config.to_sbatch_preamble(
+            user_cache_dir=self.user_cache_dir
+        )
 
         # Extend SLURM preamble with variable which are not in SlurmConfig, and
         # fix their order
         script_lines.extend(
             [
                 f"#SBATCH --err={slurm_err_path}",
                 f"#SBATCH --out={slurm_out_path}",
```

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/runner/common.py` & `fractal_server-1.2.0a5/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/app/security/__init__.py` & `fractal_server-1.2.0a5/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.0a5/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.0a5/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/README.md` & `fractal_server-1.2.0a5/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.0a5/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/project.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/state.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/task.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/user.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.0a5/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a5/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.0a5/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/config.py` & `fractal_server-1.2.0a5/fractal_server/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,38 +242,24 @@
     """
     Logging-level threshold for logging
 
     Only logs of with this level (or higher) will appear in the console logs;
     see details [here](../internals/logs/).
     """
 
-    FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW: Optional[int] = None
+    FRACTAL_LOCAL_CONFIG_FILE: Optional[Path]
     """
-    Maximum number of components that a parallel task may process
-    simultaneously, for the [local backend](../internals/runners/local/).  If
-    `None`, no limit is set.
-
-    Intended use case: Reduce memory requirements of a workflow by capping the
-    number of tasks running in parallel.
-
-    Note: this limit concerns a single task in a single workflow execution, but
-    it does **not** limit the global (i.e. across workflow executions) number
-    of components processed simultaneously.
+    Path of JSON file with configuration for the local backend.
     """
 
     FRACTAL_SLURM_CONFIG_FILE: Optional[Path]
     """
     Path of JSON file with configuration for the SLURM backend.
     """
 
-    FRACTAL_RUNNER_DEFAULT_EXECUTOR: str = "cpu-low"
-    """
-    Used by some runner backends to configure the parameters to run jobs with.
-    """
-
     FRACTAL_SLURM_WORKER_PYTHON: Optional[str] = None
     """
     Path to Python interpreter that will run the jobs on the SLURM nodes. If
     not specified, the same interpreter that runs the server is used.
     """
 
     FRACTAL_SLURM_POLL_INTERVAL: Optional[int] = 60
@@ -338,30 +324,18 @@
             FRACTAL_RUNNER_BACKEND: str = Field()
             if FRACTAL_RUNNER_BACKEND == "slurm":
                 FRACTAL_SLURM_CONFIG_FILE: Path
 
         StrictSettings(**self.dict())
 
         # Check that some variables are allowed
-        if isinstance(self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW, int):
-            if self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW < 1:
-                raise FractalConfigurationError(
-                    f"{self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW=} "
-                    "not allowed"
-                )
-
-        if (
-            self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW
-            and self.FRACTAL_RUNNER_BACKEND != "local"
-        ):
-            logging.warning(
-                "FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW is set to "
-                f"{self.FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW}, but "
-                f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND} is "
-                "the local backend."
+        if self.FRACTAL_RUNNER_BACKEND not in ["local", "slurm"]:
+            raise FractalConfigurationError(
+                f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND}"
+                "is not allowed"
             )
 
         if self.FRACTAL_RUNNER_BACKEND == "slurm":
             info = f"FRACTAL_RUNNER_BACKEND={self.FRACTAL_RUNNER_BACKEND}"
 
             # Check that FRACTAL_SLURM_CONFIG_FILE exists
             if not self.FRACTAL_SLURM_CONFIG_FILE.exists():
```

### Comparing `fractal_server-1.2.0a4/fractal_server/logger.py` & `fractal_server-1.2.0a5/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/main.py` & `fractal_server-1.2.0a5/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/migrations/env.py` & `fractal_server-1.2.0a5/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.0a5/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.0a5/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.0a5/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.0a5/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/syringe.py` & `fractal_server-1.2.0a5/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/tasks/collection.py` & `fractal_server-1.2.0a5/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/fractal_server/utils.py` & `fractal_server-1.2.0a5/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a4/pyproject.toml` & `fractal_server-1.2.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.0a4"
+version = "1.2.0a5"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.0a4"
+current_version = "1.2.0a5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.0a4/setup.py` & `fractal_server-1.2.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.0a4',
+    'version': '1.2.0a5',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.0a4/PKG-INFO` & `fractal_server-1.2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.0a4
+Version: 1.2.0a5
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

