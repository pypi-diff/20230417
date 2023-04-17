# Comparing `tmp/buildbot-worker-3.7.0.tar.gz` & `tmp/buildbot-worker-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-worker-3.7.0.tar", last modified: Sun Dec  4 11:50:50 2022, max compression
+gzip compressed data, was "dist/buildbot-worker-3.8.0.tar", last modified: Mon Apr 17 01:19:59 2023, max compression
```

## Comparing `buildbot-worker-3.7.0.tar` & `buildbot-worker-3.8.0.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/COPYING
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      206 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/MANIFEST.in
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    26185 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/NEWS
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1095 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2079 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/README
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      192 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/UPGRADING
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4722 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/backports/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      911 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/backports/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11361 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      904 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/bot.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/commands/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9032 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9912 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/fs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2055 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/registry.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2188 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/shell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12685 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4122 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/commands/utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2975 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/compat.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1242 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/exceptions.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3673 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/interfaces.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/monkeypatches/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/monkeypatches/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2257 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/monkeypatches/testcase_assert.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14126 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2181 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/null.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30769 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/pb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6067 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/pbutil.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33279 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/runprocess.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1439 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7366 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/create_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/logwatcher.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1383 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/restart.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9830 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/runner.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5096 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/start.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2538 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/stop.py
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    25140 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/scripts/windows_service.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/test/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2093 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2303 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/protocolcommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6121 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/reactor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1378 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/remote.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7532 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/fake/runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1486 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/reactor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1088 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/test_extra_coverage.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7513 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/test_util_hangcheck.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3543 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/runprocess-scripts.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11652 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_bot.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10186 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_bot_Worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4979 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15776 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_fs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1506 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_registry.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2042 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_shell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16534 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5327 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21170 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35683 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4196 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30319 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_create_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3588 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_restart.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16759 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_runner.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2464 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_start.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6238 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_stop.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5341 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_util.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2835 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/unit/test_util_deferwaiter.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5077 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/command.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1066 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/compat.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8065 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/misc.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2367 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/sourcecommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18013 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/test_buffer_manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5853 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/test/util/test_lineboundaries.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4805 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/tunnel.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3581 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4189 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/_hangcheck.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/_notifier.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7025 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/buffer_manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1923 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/deferwaiter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4276 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/buildbot_worker/util/lineboundaries.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1095 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3116 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      164 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      118 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/buildbot_worker.egg-info/top_level.txt
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/docs/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3815 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/docs/buildbot-worker.1
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      110 2022-12-04 11:50:50.000000 buildbot-worker-3.7.0/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     6620 2022-12-04 11:48:49.000000 buildbot-worker-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/COPYING
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      206 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/MANIFEST.in
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28214 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/NEWS
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2079 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/README
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      192 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/UPGRADING
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4722 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11361 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      904 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/bot.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/commands/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9032 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9912 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/fs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2055 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/registry.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2188 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/shell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12685 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4122 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/commands/utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2975 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/compat.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1242 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/exceptions.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3673 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/interfaces.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/monkeypatches/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      855 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/monkeypatches/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1048 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/monkeypatches/testcase_assert.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14126 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2181 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/null.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30789 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/pb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6067 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/pbutil.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33293 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/runprocess.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1439 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7366 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/create_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/logwatcher.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1383 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/restart.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9830 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/runner.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5096 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/start.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2538 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/stop.py
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    25140 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/scripts/windows_service.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/test/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2093 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2303 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/protocolcommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6121 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/reactor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1378 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/remote.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7532 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/fake/runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1486 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/reactor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1088 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/test_extra_coverage.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7458 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/test_util_hangcheck.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3543 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/runprocess-scripts.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11652 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_bot.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10186 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_bot_Worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4979 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15776 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_fs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1506 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_registry.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2042 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_shell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16534 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5327 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21170 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35683 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4196 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    30319 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_create_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3588 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_restart.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16759 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_runner.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2464 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_start.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6238 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_stop.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5341 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_util.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2835 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/unit/test_util_deferwaiter.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5077 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/command.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1066 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/compat.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8065 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/misc.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2367 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/sourcecommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18013 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/test_buffer_manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5853 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/test/util/test_lineboundaries.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4805 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/tunnel.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3581 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4189 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/_hangcheck.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/_notifier.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7025 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/buffer_manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1923 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/deferwaiter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4276 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/buildbot_worker/util/lineboundaries.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1222 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3078 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      163 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      118 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/buildbot_worker.egg-info/top_level.txt
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/docs/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3815 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/docs/buildbot-worker.1
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      110 2023-04-17 01:19:59.000000 buildbot-worker-3.8.0/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     6732 2023-04-17 01:17:21.000000 buildbot-worker-3.8.0/setup.py
```

### Comparing `buildbot-worker-3.7.0/COPYING` & `buildbot-worker-3.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/NEWS` & `buildbot-worker-3.8.0/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,56 @@
     Buildbot uses towncrier to manage its release notes.
     towncrier helps to avoid the need for rebase when several people work at the same time on the release notes files.
 
     Each PR should come with a file in the newsfragment directory
 
 .. towncrier release notes start
 
+Buildbot ``3.8.0`` ( ``2023-04-16`` )
+=====================================
+
+Bug fixes
+---------
+
+- Fixed compatibility issues with Python 3.11.
+- Fixed compatibility with Autobahn v22.4.1 and newer.
+- Fixed issue with overriding `env` when calling `ShellMixin.makeRemoteShellCommand`
+- Buildbot will now include the previous location of moved files when evaluating a Github commit.
+  This fixes an issue where a commit that moves a file out of a folder, would not be shown in the
+  web UI for a builder that is tracking that same folder.
+- Improved reliability of Buildbot log watching to follow log files even after rotation.
+  This improves reliability of Buildbot start and restart scripts.
+- Fixed handling of occasional errors that happen when attempting to kill a master-side process that has already exited.
+- Fixed a race condition in PyLint step that may lead to step throwing exceptions.
+- Fixed compatibility with qemu 6.1 and newer when using LibVirtWorker with ``cheap_copy=True`` (default).
+- Fixed an issue with secrets provider stripping newline from ssh keys sent in git steps.
+- Fixed occasional errors that happen when killing processes on Windows. TASKKILL command may return
+  code 255 when process has already exited.
+- Fixed deleting secrets from worker that contain '~' in their destination path.
+
+Changes
+-------
+
+- Buildbot now requires NodeJS 14.18 or newer to build the frontend.
+- The URLs emitted by the Buildbot APIs have been changed to include slash after the hash (``#``)
+  symbol to be compatible with what React web UI supports.
+
+Improved Documentation
+----------------------
+
+- Replace statement "https is unsupported" with a more detailed disclaimer.
+
+Features
+--------
+
+- Add a way to disable default ``WarningCountingShellCommand`` parser.
+- Added health check API that latent workers can use to specify that a particular worker will not connect and build should not wait for it and mark itself as failure immediately.
+- Implemented a way to customize TLS setting for ``LdapUserInfo``.
+
+
 Buildbot ``3.7.0`` ( ``2022-12-04`` )
 =====================================
 
 Bug fixes
 ---------
 
 - Improved statistics capture to avoid negative build duration.
```

### Comparing `buildbot-worker-3.7.0/README` & `buildbot-worker-3.8.0/README`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/__init__.py` & `buildbot-worker-3.8.0/buildbot_worker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/backports/__init__.py` & `buildbot-worker-3.8.0/buildbot_worker/test/test_extra_coverage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # This file is part of Buildbot.  Buildbot is free software: you can
 # redistribute it and/or modify it under the terms of the GNU General Public
 # License as published by the Free Software Foundation, version 2.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
@@ -10,13 +9,18 @@
 #
 # You should have received a copy of the GNU General Public License along with
 # this program; if not, write to the Free Software Foundation, Inc., 51
 # Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 # Copyright Buildbot Team Members
 
-try:
-    from twisted.trial.unittest import SynchronousTestCase
-except ImportError:
-    from twisted.trial.unittest import TestCase as SynchronousTestCase
+# this file imports a number of source files that are not
+# included in the coverage because none of the tests import
+# them; this results in a more accurate total coverage percent.
 
-__all__ = ['SynchronousTestCase']
+from __future__ import absolute_import
+from __future__ import print_function
+
+from buildbot_worker.scripts import logwatcher
+
+modules = []  # for the benefit of pyflakes
+modules.extend([logwatcher])
```

### Comparing `buildbot-worker-3.7.0/buildbot_worker/base.py` & `buildbot-worker-3.8.0/buildbot_worker/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/bot.py` & `buildbot-worker-3.8.0/buildbot_worker/bot.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/base.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/fs.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/fs.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/registry.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/registry.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/shell.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/shell.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/transfer.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/commands/utils.py` & `buildbot-worker-3.8.0/buildbot_worker/commands/utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/compat.py` & `buildbot-worker-3.8.0/buildbot_worker/compat.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/exceptions.py` & `buildbot-worker-3.8.0/buildbot_worker/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/interfaces.py` & `buildbot-worker-3.8.0/buildbot_worker/interfaces.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/monkeypatches/__init__.py` & `buildbot-worker-3.8.0/buildbot_worker/monkeypatches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/msgpack.py` & `buildbot-worker-3.8.0/buildbot_worker/msgpack.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/null.py` & `buildbot-worker-3.8.0/buildbot_worker/null.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/pb.py` & `buildbot-worker-3.8.0/buildbot_worker/pb.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             args['path'] = os.path.join(self.basedir, args['path'])
 
         if command == "listdir":
             args['path'] = os.path.join(self.basedir, args['dir'])
             del args['dir']
 
         if command == "rmfile":
-            args['path'] = os.path.join(self.basedir, args['path'])
+            args['path'] = os.path.join(self.basedir, os.path.expanduser(args['path']))
 
         if command == "shell":
             args['workdir'] = os.path.join(self.basedir, args['workdir'])
 
         if command == "uploadFile":
             args["path"] = os.path.join(self.basedir, args['workdir'],
                                         os.path.expanduser(args['workersrc']))
```

### Comparing `buildbot-worker-3.7.0/buildbot_worker/pbutil.py` & `buildbot-worker-3.8.0/buildbot_worker/pbutil.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/runprocess.py` & `buildbot-worker-3.8.0/buildbot_worker/runprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,18 +803,18 @@
                 cmd = "TASKKILL /PID {0} /T".format(pid)
 
             log.msg("using {0} to kill pid {1}".format(cmd, pid))
             subprocess.check_call(cmd)
             log.msg("taskkill'd pid {0}".format(pid))
 
         except subprocess.CalledProcessError as e:
-            # taskkill may return 128 as exit code when the child has already exited. We can't
-            # handle this race condition in any other way than just interpreting the kill action
-            # as successful
-            if e.returncode == 128:
+            # taskkill may return 128 or 255 as exit code when the child has already exited.
+            # We can't handle this race condition in any other way than just interpreting the kill
+            # action as successful
+            if e.returncode in (128, 255):
                 log.msg("taskkill didn't find pid {0} to kill".format(pid))
             else:
                 log.msg("taskkill failed to kill process {0}: {1}".format(pid, e))
 
     def kill(self, msg):
         # This may be called by the timeout, or when the user has decided to
         # abort this build.
```

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/base.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/create_worker.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/create_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/logwatcher.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/logwatcher.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/restart.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/restart.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/runner.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/start.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/start.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/stop.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/scripts/windows_service.py` & `buildbot-worker-3.8.0/buildbot_worker/scripts/windows_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/__init__.py` & `buildbot-worker-3.8.0/buildbot_worker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/fake/protocolcommand.py` & `buildbot-worker-3.8.0/buildbot_worker/test/fake/protocolcommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/fake/reactor.py` & `buildbot-worker-3.8.0/buildbot_worker/test/fake/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/fake/remote.py` & `buildbot-worker-3.8.0/buildbot_worker/test/fake/remote.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/fake/runprocess.py` & `buildbot-worker-3.8.0/buildbot_worker/test/fake/runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/reactor.py` & `buildbot-worker-3.8.0/buildbot_worker/test/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/test_util_hangcheck.py` & `buildbot-worker-3.8.0/buildbot_worker/test/test_util_hangcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from twisted.internet.task import Clock
 from twisted.python.failure import Failure
 from twisted.spread.pb import PBClientFactory
 from twisted.trial.unittest import TestCase
 from twisted.web.server import Site
 from twisted.web.static import Data
 
-from ..backports import SynchronousTestCase
 from ..util import HangCheckFactory
 from ..util._hangcheck import HangCheckProtocol
 
 try:
     from twisted.internet.testing import AccumulatingProtocol
     from twisted.internet.testing import StringTransport
 except ImportError:
@@ -36,15 +35,15 @@
     calls.
     """
     case.assertEqual(
         clock.getDelayedCalls(), [],
     )
 
 
-class HangCheckTests(SynchronousTestCase):
+class HangCheckTests(TestCase):
     """
     Tests for HangCheckProtocol.
     """
 
     def test_disconnects(self):
         """
         When connecting to a server that doesn't send any data,
```

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/runprocess-scripts.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/runprocess-scripts.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_bot.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_bot.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_bot_Worker.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_bot_Worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_base.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_fs.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_fs.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_registry.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_registry.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_shell.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_shell.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_transfer.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_transfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_commands_utils.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_commands_utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_msgpack.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_runprocess.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_base.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_create_worker.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_create_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_restart.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_restart.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_runner.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_runner.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_start.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_start.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_scripts_stop.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_scripts_stop.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_util.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/unit/test_util_deferwaiter.py` & `buildbot-worker-3.8.0/buildbot_worker/test/unit/test_util_deferwaiter.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/command.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/command.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/compat.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/compat.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/misc.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/misc.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/sourcecommand.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/sourcecommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/test_buffer_manager.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/test_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/test/util/test_lineboundaries.py` & `buildbot-worker-3.8.0/buildbot_worker/test/util/test_lineboundaries.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/tunnel.py` & `buildbot-worker-3.8.0/buildbot_worker/tunnel.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/__init__.py` & `buildbot-worker-3.8.0/buildbot_worker/util/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/_hangcheck.py` & `buildbot-worker-3.8.0/buildbot_worker/util/_hangcheck.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/_notifier.py` & `buildbot-worker-3.8.0/buildbot_worker/util/_notifier.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/buffer_manager.py` & `buildbot-worker-3.8.0/buildbot_worker/util/buffer_manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/deferwaiter.py` & `buildbot-worker-3.8.0/buildbot_worker/util/deferwaiter.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker/util/lineboundaries.py` & `buildbot-worker-3.8.0/buildbot_worker/util/lineboundaries.py`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/buildbot_worker.egg-info/SOURCES.txt` & `buildbot-worker-3.8.0/buildbot_worker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 buildbot_worker/tunnel.py
 buildbot_worker.egg-info/PKG-INFO
 buildbot_worker.egg-info/SOURCES.txt
 buildbot_worker.egg-info/dependency_links.txt
 buildbot_worker.egg-info/entry_points.txt
 buildbot_worker.egg-info/requires.txt
 buildbot_worker.egg-info/top_level.txt
-buildbot_worker/backports/__init__.py
 buildbot_worker/commands/__init__.py
 buildbot_worker/commands/base.py
 buildbot_worker/commands/fs.py
 buildbot_worker/commands/registry.py
 buildbot_worker/commands/shell.py
 buildbot_worker/commands/transfer.py
 buildbot_worker/commands/utils.py
```

### Comparing `buildbot-worker-3.7.0/docs/buildbot-worker.1` & `buildbot-worker-3.8.0/docs/buildbot-worker.1`

 * *Files identical despite different names*

### Comparing `buildbot-worker-3.7.0/setup.py` & `buildbot-worker-3.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,20 +99,22 @@
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     'packages': [
         "buildbot_worker",
         "buildbot_worker.util",
-        "buildbot_worker.backports",
         "buildbot_worker.commands",
         "buildbot_worker.scripts",
         "buildbot_worker.monkeypatches",
     ] + ([] if BUILDING_WHEEL else [  # skip tests for wheels (save 40% of the archive)
         "buildbot_worker.test",
         "buildbot_worker.test.fake",
         "buildbot_worker.test.unit",
```

