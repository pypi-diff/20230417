# Comparing `tmp/opentaskpy-0.8.0.tar.gz` & `tmp/opentaskpy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentaskpy-0.8.0.tar", last modified: Fri Mar 31 13:56:08 2023, max compression
+gzip compressed data, was "opentaskpy-0.8.1.tar", last modified: Mon Apr 17 16:02:47 2023, max compression
```

## Comparing `opentaskpy-0.8.0.tar` & `opentaskpy-0.8.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.255920 opentaskpy-0.8.0/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       71 2023-01-27 14:31:24.000000 opentaskpy-0.8.0/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35148 2023-01-27 14:31:24.000000 opentaskpy-0.8.0/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       43 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/MANIFEST.in
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17798 2023-03-31 13:56:08.255920 opentaskpy-0.8.0/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16950 2023-03-31 12:59:03.000000 opentaskpy-0.8.0/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1838 2023-03-31 13:08:47.000000 opentaskpy-0.8.0/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-03-31 13:56:08.255920 opentaskpy-0.8.0/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.171920 opentaskpy-0.8.0/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.203920 opentaskpy-0.8.0/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.203920 opentaskpy-0.8.0/src/opentaskpy/cli/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2032 2023-01-30 12:56:01.000000 opentaskpy-0.8.0/src/opentaskpy/cli/task_run.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.203920 opentaskpy-0.8.0/src/opentaskpy/config/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-01-24 14:12:28.000000 opentaskpy-0.8.0/src/opentaskpy/config/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10322 2023-03-31 11:01:34.000000 opentaskpy-0.8.0/src/opentaskpy/config/loader.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.203920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1658 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/batch.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.175920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/execution/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.219920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/execution/ssh/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      496 2023-03-29 15:19:06.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/execution/ssh/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      460 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/execution/ssh/ssh.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.231920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.235920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/email/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      761 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/email/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      384 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/email_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.247920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      161 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      564 2023-03-29 15:19:06.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      213 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      692 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.247920 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      864 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      273 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      382 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1283 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      496 2023-03-29 15:19:06.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      690 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source.json
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9714 2023-03-31 12:06:00.000000 opentaskpy-0.8.0/src/opentaskpy/config/schemas.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/src/opentaskpy/exceptions.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5685 2023-03-02 17:46:38.000000 opentaskpy-0.8.0/src/opentaskpy/logging.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.175920 opentaskpy-0.8.0/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.251920 opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      844 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1191 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      627 2023-03-31 12:53:23.000000 opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/random.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.251920 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-01-24 14:12:28.000000 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4099 2023-03-08 13:20:16.000000 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      930 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/remotehandler.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.251920 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/scripts/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6265 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/scripts/transfer.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29670 2023-03-30 15:43:48.000000 opentaskpy-0.8.0/src/opentaskpy/remotehandlers/ssh.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2754 2023-03-30 16:02:42.000000 opentaskpy-0.8.0/src/opentaskpy/task_run.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.251920 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-01-24 14:12:28.000000 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16851 2023-03-08 13:20:16.000000 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6612 2023-03-08 13:20:16.000000 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2692 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/taskhandler.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    23016 2023-03-30 15:53:35.000000 opentaskpy-0.8.0/src/opentaskpy/taskhandlers/transfer.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.203920 opentaskpy-0.8.0/src/opentaskpy.egg-info/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17798 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2630 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       58 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      230 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2023-03-31 13:56:08.000000 opentaskpy-0.8.0/src/opentaskpy.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-03-31 13:56:08.255920 opentaskpy-0.8.0/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1463 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_batch_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13804 2023-03-31 10:58:00.000000 opentaskpy-0.8.0/tests/test_config_loader.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6939 2023-03-30 13:28:17.000000 opentaskpy-0.8.0/tests/test_docker_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      969 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_email_transfer_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      836 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/tests/test_file_helper.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7891 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/tests/test_logging.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      911 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/tests/test_plugin_file.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1126 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/tests/test_plugin_http_json.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8416 2023-02-21 17:18:29.000000 opentaskpy-0.8.0/tests/test_remote_transfer_script.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1920 2023-03-28 15:10:24.000000 opentaskpy-0.8.0/tests/test_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3535 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_ssh_dest_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_ssh_execution_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5874 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_ssh_source_schema_validate.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14719 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_task_run.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14301 2023-03-08 13:20:16.000000 opentaskpy-0.8.0/tests/test_taskhandler_batch.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4420 2023-03-08 13:20:16.000000 opentaskpy-0.8.0/tests/test_taskhandler_execution.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4205 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_taskhandler_transfer_email.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14339 2023-03-28 12:13:44.000000 opentaskpy-0.8.0/tests/test_taskhandler_transfer_ssh.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/MANIFEST.in
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17790 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16943 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1853 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/cli/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2052 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/cli/task_run.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    10322 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/loader.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1659 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/batch.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      497 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      461 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/execution/ssh/ssh.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      762 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      385 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      162 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/flags.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      212 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/permissions.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      565 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      214 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/rename.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      693 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination.json
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      865 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      274 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/fileWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      383 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/logWatch.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      497 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/protocol.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      691 2023-04-17 16:01:52.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source.json
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9714 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/config/schemas.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1236 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5685 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/logging.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.402677 opentaskpy-0.8.1/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      844 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1191 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      627 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/random.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4099 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      930 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/remotehandler.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.410678 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6265 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/transfer.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    29670 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/remotehandlers/ssh.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2754 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/task_run.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    16851 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6612 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2692 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/taskhandler.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    23016 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/src/opentaskpy/taskhandlers/transfer.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.406678 opentaskpy-0.8.1/src/opentaskpy.egg-info/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    17790 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2630 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       58 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      241 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2023-04-17 16:02:47.000000 opentaskpy-0.8.1/src/opentaskpy.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-04-17 16:02:47.414677 opentaskpy-0.8.1/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1463 2023-04-11 16:45:44.000000 opentaskpy-0.8.1/tests/test_batch_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    13804 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_config_loader.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6939 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_docker_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      969 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_email_transfer_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      836 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_file_helper.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7891 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_logging.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      911 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_plugin_file.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1126 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_plugin_http_json.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     8416 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_remote_transfer_script.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1920 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3535 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_dest_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_execution_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5874 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_ssh_source_schema_validate.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14719 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_task_run.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14301 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_batch.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4420 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_execution.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4205 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_transfer_email.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14339 2023-04-06 12:19:29.000000 opentaskpy-0.8.1/tests/test_taskhandler_transfer_ssh.py
```

### Comparing `opentaskpy-0.8.0/LICENSE` & `opentaskpy-0.8.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -667,8 +667,8 @@
 <https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `opentaskpy-0.8.0/PKG-INFO` & `opentaskpy-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentaskpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for automation execution of commands and transferring files between hosts
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
@@ -70,21 +70,21 @@
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
 
 ```shell
 docker build -t opentaskpy -f Dockerfile . # Build the image
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
-The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against. 
+The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
 # Configuration
 
-There are several ways to customise the running of tasks. 
+There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
 
 ```
 usage: task-run [-h] -t TASKID [-r RUNID] [-v VERBOSITY] [-c CONFIGDIR]
@@ -113,15 +113,15 @@
 
 There are 3 levels of logging, beyond the default INFO level. These are VERBOSE1 (1), VERBOSE2 (2), and DEBUG (3).
 
 VERBOSITY is an integer; 1, 2 or 3
 
 **-c, --configDir**
 
-The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file. 
+The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file.
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
@@ -311,15 +311,15 @@
 ```
 
 An explaination of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
-4. Transfer the files that were found to 2 destinations. 
+4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
 
 ## Executions
 
@@ -344,25 +344,25 @@
 }
 ```
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
-## Batches 
+## Batches
 
 Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
-`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined. 
+`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
 
 # Development
@@ -396,24 +396,24 @@
 Lookup plugins:
    * Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
-Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template. 
+Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
 
 3 examples are bundled by default. The simplest of which is the `random` plugin, which takes 2 numbers and returns a random number between the 2.
 
 They should either be installed as a python package and accessible to load as a module, or stored within the config directory under a `plugins` directory.
 
 They must sit under the `opentaskpy.plugins.lookup` namespace. The filename must match the name of the plugin being references from the template lookup function.
 
 ### Addons
 
 Addons allow you to write your own interfaces with other types of remote systems. This could be a custom database provider to allow you to run stored procedures on demand, or something like AWS to perform custom transfers
 
-Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception. 
+Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception.
 
 You should also ensure that you define an appropriate JSON schema, and include those under the `opentaskpy.addons.XXXX.remotehandlers.schemas` directory
 
 Addons can technically be named under any namespace, but must be referred to using the full package name in the task definition e.g. `opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution`
```

### Comparing `opentaskpy-0.8.0/README.md` & `opentaskpy-0.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
 
 ```shell
 docker build -t opentaskpy -f Dockerfile . # Build the image
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
-The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against. 
+The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
 # Configuration
 
-There are several ways to customise the running of tasks. 
+There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
 
 ```
 usage: task-run [-h] -t TASKID [-r RUNID] [-v VERBOSITY] [-c CONFIGDIR]
@@ -94,15 +94,15 @@
 
 There are 3 levels of logging, beyond the default INFO level. These are VERBOSE1 (1), VERBOSE2 (2), and DEBUG (3).
 
 VERBOSITY is an integer; 1, 2 or 3
 
 **-c, --configDir**
 
-The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file. 
+The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file.
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
@@ -292,15 +292,15 @@
 ```
 
 An explaination of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
-4. Transfer the files that were found to 2 destinations. 
+4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
 
 ## Executions
 
@@ -325,25 +325,25 @@
 }
 ```
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
-## Batches 
+## Batches
 
 Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
-`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined. 
+`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
 
 # Development
@@ -377,24 +377,24 @@
 Lookup plugins:
    * Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
-Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template. 
+Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
 
 3 examples are bundled by default. The simplest of which is the `random` plugin, which takes 2 numbers and returns a random number between the 2.
 
 They should either be installed as a python package and accessible to load as a module, or stored within the config directory under a `plugins` directory.
 
 They must sit under the `opentaskpy.plugins.lookup` namespace. The filename must match the name of the plugin being references from the template lookup function.
 
 ### Addons
 
 Addons allow you to write your own interfaces with other types of remote systems. This could be a custom database provider to allow you to run stored procedures on demand, or something like AWS to perform custom transfers
 
-Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception. 
+Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception.
 
 You should also ensure that you define an appropriate JSON schema, and include those under the `opentaskpy.addons.XXXX.remotehandlers.schemas` directory
 
-Addons can technically be named under any namespace, but must be referred to using the full package name in the task definition e.g. `opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution`
+Addons can technically be named under any namespace, but must be referred to using the full package name in the task definition e.g. `opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution`
```

### Comparing `opentaskpy-0.8.0/pyproject.toml` & `opentaskpy-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opentaskpy"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -35,30 +35,31 @@
   "flake8-use-fstring",
   "flake8-black",
   "isort",
   "flake8-isort",
   "pytest",
   "bumpver",
   "pytest-shell",
-  "lovely-pytest-docker"
+  "lovely-pytest-docker",
+  "pre-commit"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/adammcdonagh/open-task-framework"
 "Bug Tracker" = "https://github.com/adammcdonagh/open-task-framework/issues"
 "Changelog" = "https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md"
 
 [project.scripts]
 task-run = "opentaskpy.cli.task_run:main"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.8.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
@@ -69,8 +70,7 @@
 
 # Include the schema JSON files in the package
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
-
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/cli/task_run.py` & `opentaskpy-0.8.1/src/opentaskpy/cli/task_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,11 +68,12 @@
 
     try:
         task_run_obj.run()
     except Exception as e:
         logger.error(f"Error running task: {e}")
         if logger.getEffectiveLevel() <= 12:
             raise e
+        os._exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/loader.py` & `opentaskpy-0.8.1/src/opentaskpy/config/loader.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/batch.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/batch.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
 00000600: 2020 2020 2020 226d 696e 696d 756d 223a        "minimum":
 00000610: 2031 0a20 2020 2020 207d 0a20 2020 207d   1.      }.    }
 00000620: 0a20 207d 2c0a 2020 2261 6464 6974 696f  .  },.  "additio
 00000630: 6e61 6c50 726f 7065 7274 6965 7322 3a20  nalProperties": 
 00000640: 6661 6c73 652c 0a20 2022 7265 7175 6972  false,.  "requir
 00000650: 6564 223a 205b 0a20 2020 2022 6f72 6465  ed": [.    "orde
 00000660: 725f 6964 222c 0a20 2020 2022 7461 736b  r_id",.    "task
-00000670: 5f69 6422 0a20 205d 0a7d                 _id".  ].}
+00000670: 5f69 6422 0a20 205d 0a7d 0a              _id".  ].}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/email/protocol.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/email/protocol.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 13% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 00000280: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
 00000290: 6164 6469 7469 6f6e 616c 5072 6f70 6572  additionalProper
 000002a0: 7469 6573 223a 2066 616c 7365 0a20 2020  ties": false.   
 000002b0: 207d 0a20 207d 2c0a 2020 2272 6571 7569   }.  },.  "requi
 000002c0: 7265 6422 3a20 5b0a 2020 2020 226e 616d  red": [.    "nam
 000002d0: 6522 0a20 205d 2c0a 2020 2261 6464 6974  e".  ],.  "addit
 000002e0: 696f 6e61 6c50 726f 7065 7274 6965 7322  ionalProperties"
-000002f0: 3a20 6661 6c73 650a 7d                   : false.}
+000002f0: 3a20 6661 6c73 650a 7d0a                 : false.}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination/protocol.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 000001c0: 616c 5072 6f70 6572 7469 6573 223a 2066  alProperties": f
 000001d0: 616c 7365 0a20 2020 207d 0a20 207d 2c0a  alse.    }.  },.
 000001e0: 2020 2272 6571 7569 7265 6422 3a20 5b0a    "required": [.
 000001f0: 2020 2020 226e 616d 6522 2c0a 2020 2020      "name",.    
 00000200: 2263 7265 6465 6e74 6961 6c73 220a 2020  "credentials".  
 00000210: 5d2c 0a20 2022 6164 6469 7469 6f6e 616c  ],.  "additional
 00000220: 5072 6f70 6572 7469 6573 223a 2066 616c  Properties": fal
-00000230: 7365 0a7d                                se.}
+00000230: 7365 0a7d 0a                             se.}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_destination.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_destination.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 00000240: 6e22 0a20 2020 207d 0a20 207d 2c0a 2020  n".    }.  },.  
 00000250: 2261 6464 6974 696f 6e61 6c50 726f 7065  "additionalPrope
 00000260: 7274 6965 7322 3a20 6661 6c73 652c 0a20  rties": false,. 
 00000270: 2022 7265 7175 6972 6564 223a 205b 0a20   "required": [. 
 00000280: 2020 2022 686f 7374 6e61 6d65 222c 0a20     "hostname",. 
 00000290: 2020 2022 6469 7265 6374 6f72 7922 2c0a     "directory",.
 000002a0: 2020 2020 2270 726f 746f 636f 6c22 0a20      "protocol". 
-000002b0: 205d 0a7d                                 ].}
+000002b0: 205d 0a7d 0a                              ].}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/conditionals.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -48,7 +48,8 @@
 000002f0: 0a20 2020 2020 2020 2020 205d 0a20 2020  .          ].   
 00000300: 2020 2020 207d 0a20 2020 2020 205d 2c0a       }.      ],.
 00000310: 2020 2020 2020 2261 6464 6974 696f 6e61        "additiona
 00000320: 6c50 726f 7065 7274 6965 7322 3a20 6661  lProperties": fa
 00000330: 6c73 650a 2020 2020 7d0a 2020 7d2c 0a20  lse.    }.  },. 
 00000340: 2022 6164 6469 7469 6f6e 616c 5072 6f70   "additionalProp
 00000350: 6572 7469 6573 223a 2066 616c 7365 0a7d  erties": false.}
+00000360: 0a                                       .
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source/postCopyAction.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,8 @@
 00000490: 2020 2020 2020 2020 2020 2020 2273 7562              "sub
 000004a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
 000004b0: 7061 7474 6572 6e22 0a20 2020 2020 2020  pattern".       
 000004c0: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
 000004d0: 2020 2020 207d 0a20 2020 207d 0a20 205d       }.    }.  ]
 000004e0: 2c0a 2020 2261 6464 6974 696f 6e61 6c50  ,.  "additionalP
 000004f0: 726f 7065 7274 6965 7322 3a20 6661 6c73  roperties": fals
-00000500: 650a 7d                                  e.}
+00000500: 650a 7d0a                                e.}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas/transfer/ssh_source.json` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas/transfer/ssh_source.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 00000240: 0a20 2020 207d 0a20 207d 2c0a 2020 2261  .    }.  },.  "a
 00000250: 6464 6974 696f 6e61 6c50 726f 7065 7274  dditionalPropert
 00000260: 6965 7322 3a20 6661 6c73 652c 0a20 2022  ies": false,.  "
 00000270: 7265 7175 6972 6564 223a 205b 0a20 2020  required": [.   
 00000280: 2022 686f 7374 6e61 6d65 222c 0a20 2020   "hostname",.   
 00000290: 2022 6669 6c65 5265 6765 7822 2c0a 2020   "fileRegex",.  
 000002a0: 2020 2270 726f 746f 636f 6c22 0a20 205d    "protocol".  ]
-000002b0: 0a7d                                     .}
+000002b0: 0a7d 0a                                  .}.
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy/config/schemas.py` & `opentaskpy-0.8.1/src/opentaskpy/config/schemas.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/exceptions.py` & `opentaskpy-0.8.1/src/opentaskpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/logging.py` & `opentaskpy-0.8.1/src/opentaskpy/logging.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/file.py` & `opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/file.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/http_json.py` & `opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/http_json.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/plugins/lookup/random.py` & `opentaskpy-0.8.1/src/opentaskpy/plugins/lookup/random.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/remotehandlers/email.py` & `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/email.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/remotehandlers/remotehandler.py` & `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/remotehandler.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/remotehandlers/scripts/transfer.py` & `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/scripts/transfer.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/remotehandlers/ssh.py` & `opentaskpy-0.8.1/src/opentaskpy/remotehandlers/ssh.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/task_run.py` & `opentaskpy-0.8.1/src/opentaskpy/task_run.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/taskhandlers/batch.py` & `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/batch.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/taskhandlers/execution.py` & `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/execution.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/taskhandlers/taskhandler.py` & `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/taskhandler.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy/taskhandlers/transfer.py` & `opentaskpy-0.8.1/src/opentaskpy/taskhandlers/transfer.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/src/opentaskpy.egg-info/PKG-INFO` & `opentaskpy-0.8.1/src/opentaskpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentaskpy
-Version: 0.8.0
+Version: 0.8.1
 Summary: A framework for automation execution of commands and transferring files between hosts
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/open-task-framework
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/open-task-framework/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/open-task-framework/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,scheduling,ssh,sftp,remote,execution,command
@@ -70,21 +70,21 @@
 To run via docker, use the `Dockerfile` to create your own base image using just the standard opentaskpy library. However if you want to install addons, you'll need to customise this, to install the additional packages first, before bundling it as a Docker image.
 
 ```shell
 docker build -t opentaskpy -f Dockerfile . # Build the image
 docker run --rm --volume /opt/otf/cfg:/cfg --volume /var/log/otf:/logs--volume /home/<USER>/.ssh/id_rsa:/id_rsa -e OTF_SSH_KEY=/id_rsa -e OTF_LOG_DIRECTORY=/logs task-run -t <TASK NAME> -c /cfg # Run a task
 ```
 
-The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against. 
+The default `opentaskpy` library is only really designed to use SSH for executions and file transfers. To do this, you need to make sure that the host/container that is running the `task-run` script has a private RSA key, that is trusted on all remote hosts that you're running against.
 
 An environment variable `OTF_SSH_KEY` can be used to define a default SSH key to use for all SSH connectivity. This can be overridden at the transfer/execution level by specifying a `keyFile` in the `credentials` section of the protocol definition.
 
 # Configuration
 
-There are several ways to customise the running of tasks. 
+There are several ways to customise the running of tasks.
 
 ## Command Line Arguments
 
 The following details the syntax of the `task-run` command:
 
 ```
 usage: task-run [-h] -t TASKID [-r RUNID] [-v VERBOSITY] [-c CONFIGDIR]
@@ -113,15 +113,15 @@
 
 There are 3 levels of logging, beyond the default INFO level. These are VERBOSE1 (1), VERBOSE2 (2), and DEBUG (3).
 
 VERBOSITY is an integer; 1, 2 or 3
 
 **-c, --configDir**
 
-The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file. 
+The directory containing all of the config files. These are the task definition JSON files, as well as the variables Jinja2 template file.
 
 In order for the process to run, you must have at least one task, and a `variables.json.j2` file, even if it's just an empty object definition
 
 ## Environment Variables
 
 These are some environment variables that can be used to customise the behaviour of the application. There are some internally used variables too, but changing them without a full understanding of the code is not advised.
 
@@ -311,15 +311,15 @@
 ```
 
 An explaination of what's going on in the order it will handled:
 
 1. Tail the log file matching named: `/tmp/testFiles/src/log{{ YYYY }}Watch1.log` for lines matching containing the regex `someText[0-9]`, for up to 15 seconds, before giving up.
 2. Poll for a file matching the regex `/tmp/testFiles/src/fileWatch\.txt` for up to 15 seconds.
 3. Find all files matching the regex `/tmp/testFiles/src/.*\.txt`, with the conditions that the are >10B and <20B in size, as well as being older than 60 seconds, but newer than 600 seconds since last modification
-4. Transfer the files that were found to 2 destinations. 
+4. Transfer the files that were found to 2 destinations.
    1. The first destination is a simple SCP from `HOST_A` to `HOST_B` where the file is placed under `/tmp/testFiles/dest`. The group ownership of the file(s) is then set to `operator`
    2. The second destination is done via a pull from the destination server into the same directory. The SCP connects to `HOST_A` as `transferUsername`. Once the file has been retrieved, it is renamed using the following regex match `^(.*)\.txt$` and substitution `\1-2.txt`
 5. Transferred files are moved into `/tmp/testFiles/archive` on `HOST_A`
 
 
 ## Executions
 
@@ -344,25 +344,25 @@
 }
 ```
 
 The above is running the command `touch touchedFile.txt` on `{{ HOST_A }}`, from within the `/tmp/testFiles/src` directory.
 
 If multiple `hosts` are defined, a thread is spawned in parallel for each host. If the command fails on any of the hosts in the list, it will cause the task run to fail, once all processes have returned a result.
 
-## Batches 
+## Batches
 
 Batches are a little more complex. They do not contain any task definitions, only the list, and order of excecution for each task.
 
 A batch task can have multiple options set that determine the execution order and conditions, as well as how failures and task reruns are handled.
 
 Each task in a batch has an `order_id`, this is a unique ID for each task, and is primarily used to define dependencies.
 
 `dependencies` can be applied to any task, and are simply a list of other tasks that must be completed before it is triggered.
 
-`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined. 
+`continue_on_fail` is a boolean that defines whether a failure would cause the whole batch to fail immediately (after existing tasks have finished executing), or whether following steps get run. This defaults to false if not defined.
 
 `retry_on_rerun` is a boolean that determines whether a successful task is run a second time following a failed run. If a batch exits with a failure, and then the script is reun later on that same day, by default only the steps that failed will be run. All steps can be forced to run by setting this to true
 
 `timeout` specifies the number of seconds a task is allowed to be running before it gets terminated. This counts as a failure. The default timeout, if not specified is 300 seconds.
 
 
 # Development
@@ -396,24 +396,24 @@
 Lookup plugins:
    * Support for AWS SSM Parameter Store for retrieving global variables
 
 ## Developing your own addon/plugin
 
 ### Lookup Plugins
 
-Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template. 
+Plugins are very simple. They simply need a `run` function, and to return the required variable based on a list of kwargs provided within the config template.
 
 3 examples are bundled by default. The simplest of which is the `random` plugin, which takes 2 numbers and returns a random number between the 2.
 
 They should either be installed as a python package and accessible to load as a module, or stored within the config directory under a `plugins` directory.
 
 They must sit under the `opentaskpy.plugins.lookup` namespace. The filename must match the name of the plugin being references from the template lookup function.
 
 ### Addons
 
 Addons allow you to write your own interfaces with other types of remote systems. This could be a custom database provider to allow you to run stored procedures on demand, or something like AWS to perform custom transfers
 
-Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception. 
+Addons can either be a transfer type, or execution, and must follow the same rules. They should implement all of the functions in the abstract `RemoteTransferHandler` or `RemoteExecutionHandler` class, or return a `NotImplementedError` exception.
 
 You should also ensure that you define an appropriate JSON schema, and include those under the `opentaskpy.addons.XXXX.remotehandlers.schemas` directory
 
 Addons can technically be named under any namespace, but must be referred to using the full package name in the task definition e.g. `opentaskpy.addons.aws.remotehandlers.lambda.LambdaExecution`
```

### Comparing `opentaskpy-0.8.0/src/opentaskpy.egg-info/SOURCES.txt` & `opentaskpy-0.8.1/src/opentaskpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_batch_schema_validate.py` & `opentaskpy-0.8.1/tests/test_batch_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_config_loader.py` & `opentaskpy-0.8.1/tests/test_config_loader.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_docker_task_run.py` & `opentaskpy-0.8.1/tests/test_docker_task_run.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_email_transfer_schema_validate.py` & `opentaskpy-0.8.1/tests/test_email_transfer_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_file_helper.py` & `opentaskpy-0.8.1/tests/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_logging.py` & `opentaskpy-0.8.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_plugin_file.py` & `opentaskpy-0.8.1/tests/test_plugin_file.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_plugin_http_json.py` & `opentaskpy-0.8.1/tests/test_plugin_http_json.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_remote_transfer_script.py` & `opentaskpy-0.8.1/tests/test_remote_transfer_script.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_schema_validate.py` & `opentaskpy-0.8.1/tests/test_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_ssh_dest_schema_validate.py` & `opentaskpy-0.8.1/tests/test_ssh_dest_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_ssh_execution_schema_validate.py` & `opentaskpy-0.8.1/tests/test_ssh_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_ssh_source_schema_validate.py` & `opentaskpy-0.8.1/tests/test_ssh_source_schema_validate.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_task_run.py` & `opentaskpy-0.8.1/tests/test_task_run.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_taskhandler_batch.py` & `opentaskpy-0.8.1/tests/test_taskhandler_batch.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_taskhandler_execution.py` & `opentaskpy-0.8.1/tests/test_taskhandler_execution.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_taskhandler_transfer_email.py` & `opentaskpy-0.8.1/tests/test_taskhandler_transfer_email.py`

 * *Files identical despite different names*

### Comparing `opentaskpy-0.8.0/tests/test_taskhandler_transfer_ssh.py` & `opentaskpy-0.8.1/tests/test_taskhandler_transfer_ssh.py`

 * *Files identical despite different names*

