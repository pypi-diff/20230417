# Comparing `tmp/binsync-3.6.0.tar.gz` & `tmp/binsync-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsync-3.6.0.tar", last modified: Sat Apr  8 23:09:33 2023, max compression
+gzip compressed data, was "binsync-3.9.0.tar", last modified: Mon Apr 17 06:10:06 2023, max compression
```

## Comparing `binsync-3.6.0.tar` & `binsync-3.9.0.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-08 23:09:21.000000 binsync-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 23:09:21.000000 binsync-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-08 23:09:33.022079 binsync-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-08 23:09:21.000000 binsync-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync/common/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)    37358 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/control_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/force_push/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/force_push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/force_push/panels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/force_push/panels/global_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/magic_sync_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.010079 binsync-3.6.0/binsync/common/ui/panel_tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/activity_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/ctx_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/panel_tabs/util_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/qt_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/common/ui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/core/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24708 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/core/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/data/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/global_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/stack_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20455 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/data/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.014079 binsync-3.6.0/binsync/decompilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/angr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/control_panel_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/angr/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/binja/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/binja_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/binja/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/ghidra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.018079 binsync-3.6.0/binsync/decompilers/ghidra/server/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/control_panel_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ghidra/server/ghidra_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/binsync/decompilers/ida/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/artifact_lifter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22352 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10336 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/oneliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/decompilers/ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-08 23:09:21.000000 binsync-3.6.0/binsync/loggercfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.006079 binsync-3.6.0/binsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 23:09:32.000000 binsync-3.6.0/binsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/angr_binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/angr_binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/angr_binsync/plugin.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/decompiler_stubs/binja_binsync/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/binja_binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/binja_binsync/plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/ghidra_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-08 23:09:21.000000 binsync-3.6.0/decompiler_stubs/ida_binsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-08 23:09:33.022079 binsync-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-08 23:09:21.000000 binsync-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:09:33.022079 binsync-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_angr_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-08 23:09:21.000000 binsync-3.6.0/tests/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.433547 binsync-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-17 06:09:57.000000 binsync-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 06:09:57.000000 binsync-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-04-17 06:10:06.433547 binsync-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-04-17 06:09:57.000000 binsync-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.417547 binsync-3.9.0/binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.417547 binsync-3.9.0/binsync/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/api/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/api/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/api/type_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.417547 binsync-3.9.0/binsync/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/core/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24758 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/core/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.421547 binsync-3.9.0/binsync/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/global_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/stack_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20793 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/data/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.421547 binsync-3.9.0/binsync/decompiler_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompiler_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.421547 binsync-3.9.0/binsync/decompiler_stubs/angr_binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompiler_stubs/angr_binsync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.421547 binsync-3.9.0/binsync/decompiler_stubs/binja_binsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompiler_stubs/binja_binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompiler_stubs/ghidra_binsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompiler_stubs/ida_binsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.421547 binsync-3.9.0/binsync/decompilers/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/decompilers/angr/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/angr/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/angr/control_panel_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/angr/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/angr/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/decompilers/binja/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/binja/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/binja/binja_binsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/binja/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/binja/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/decompilers/ghidra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/decompilers/ghidra/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/server/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/server/control_panel_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/server/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ghidra/server/ghidra_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/decompilers/ida/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/artifact_lifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10388 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/oneliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/decompilers/ida/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.425547 binsync-3.9.0/binsync/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.429547 binsync-3.9.0/binsync/extras/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/extras/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/extras/ai/ai_user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/extras/ai/openai_bs_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/loggercfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.429547 binsync-3.9.0/binsync/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/control_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.429547 binsync-3.9.0/binsync/ui/force_push/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/force_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/force_push/force_push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.429547 binsync-3.9.0/binsync/ui/force_push/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/force_push/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/force_push/panels/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/force_push/panels/global_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/magic_sync_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.429547 binsync-3.9.0/binsync/ui/panel_tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/activity_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/ctx_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/panel_tabs/util_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/qt_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-17 06:09:57.000000 binsync-3.9.0/binsync/ui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.417547 binsync-3.9.0/binsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 06:10:06.000000 binsync-3.9.0/binsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 06:10:06.433547 binsync-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 06:09:57.000000 binsync-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:10:06.433547 binsync-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16153 2023-04-17 06:09:57.000000 binsync-3.9.0/tests/test_angr_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-17 06:09:57.000000 binsync-3.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-17 06:09:57.000000 binsync-3.9.0/tests/test_state.py
```

### Comparing `binsync-3.6.0/LICENSE` & `binsync-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/common/artifact_lifter.py` & `binsync-3.9.0/binsync/api/artifact_lifter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from binsync.data import StackVariable, Artifact
-from binsync.data.type_parser import BSTypeParser, BSType
+from binsync.api.type_parser import BSTypeParser
 
 _l = logging.getLogger(name=__name__)
 
 
-class ArtifactLifter:
+class BSArtifactLifter:
     def __init__(self, controller, types=None):
         self.controller = controller
         self.type_parser = BSTypeParser(extra_types=types)
 
     #
     # Public API
     #
```

### Comparing `binsync-3.6.0/binsync/common/controller.py` & `binsync-3.9.0/binsync/api/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import threading
 import datetime
 import time
 from functools import wraps
-from typing import Dict, Iterable, Optional, Union
+from typing import Dict, Iterable, Optional, Union, TypeVar, Callable
 
 import binsync.data
 from binsync.data import ProjectConfig
-from binsync.common.artifact_lifter import ArtifactLifter
+from binsync.api.artifact_lifter import BSArtifactLifter
 from binsync.core.client import Client, SchedSpeed, Scheduler, Job
-from binsync.data.type_parser import BSTypeParser, BSType
+from binsync.api.type_parser import BSTypeParser, BSType
 from binsync.data import (
     State, User, Artifact,
     Function, FunctionHeader, StackVariable,
     Comment, GlobalVariable, Patch,
     Enum, Struct
 )
 
@@ -29,30 +29,33 @@
     def _init_check(self, *args, **kwargs):
         if not self.check_client():
             raise RuntimeError("Please connect to a repo first.")
         return f(self, *args, **kwargs)
 
     return _init_check
 
+
 def fill_event(f):
     @wraps(f)
-    def _fill_event(self: "BinSyncController", *args, **kwargs):
+    def _fill_event(self: "BSController", *args, **kwargs):
         return self.fill_event_handler(f, *args, **kwargs)
 
     return _fill_event
 
 #
 # Description Constants
 #
 
+
 # https://stackoverflow.com/questions/10926328
 BUSY_LOOP_COOLDOWN = 0.5
 GET_MANY = True
 FILL_MANY = True
 
+
 class SyncControlStatus:
     CONNECTED = 0
     CONNECTED_NO_REMOTE = 1
     DISCONNECTED = 2
 
 
 class MergeLevel:
@@ -69,15 +72,15 @@
         pass
 
 
 #
 #   Controller
 #
 
-class BinSyncController:
+class BSController:
 
     ARTIFACT_SET_MAP = {
         Function: State.set_function,
         FunctionHeader: State.set_function_header,
         StackVariable: State.set_stack_variable,
         Comment: State.set_comment,
         GlobalVariable: State.set_global_var,
@@ -110,15 +113,15 @@
     All class properties that have a "= None" means they must be set during runtime by an outside process.
     The client will be set on connection. The ctx_change_callback will be set by an outside UI
 
     """
     def __init__(self, artifact_lifter=None, headless=False, reload_time=10):
         self.headless = headless
         self.reload_time = reload_time
-        self.artifact_lifer: ArtifactLifter = artifact_lifter
+        self.artifact_lifer: BSArtifactLifter = artifact_lifter
 
         # client created on connection
         self.client = None  # type: Optional[Client]
 
         # ui callback created on UI init
         self.ui_callback = None  # func(states: List[State])
         self.ctx_change_callback = None  # func()
@@ -139,28 +142,33 @@
 
         # create a pulling thread, but start on connection
         self._run_updater_threads = False
         self.user_states_update_thread = threading.Thread(target=self.updater_routine)
 
         # TODO: make the initialization of this with types of decompiler
         self.type_parser = BSTypeParser()
+        if self.headless:
+            self._init_headless_components()
+
+    def _init_headless_components(self):
+        pass
 
     #
     #   Multithreading updaters, locks, and evaluators
     #
 
     def _init_ui_components(self):
         if self.headless:
             return
 
         # after this point you can import anything from UI and it is safe!
-        from binsync.common.ui.qt_objects import (
+        from binsync.ui.qt_objects import (
             QThread
         )
-        from binsync.common.ui.utils import BSUIScheduler
+        from binsync.ui.utils import BSUIScheduler
         # spawns a qthread/worker
         self._ui_updater_thread = QThread()
         self._ui_updater_worker = BSUIScheduler()
         self._ui_updater_worker.moveToThread(self._ui_updater_thread)
         self._ui_updater_thread.started.connect(self._ui_updater_worker.run)
         self._ui_updater_thread.finished.connect(self._ui_updater_thread.deleteLater)
         self._ui_updater_thread.start()
@@ -255,21 +263,23 @@
         self.push_job_scheduler.stop_worker_thread()
         self._stop_ui_components()
 
     #
     # Client Interaction Functions
     #
 
-    def connect(self, user, path, init_repo=False, remote_url=None, **kwargs):
+    def connect(self, user, path, init_repo=False, remote_url=None, single_thread=False, **kwargs):
         binary_hash = self.binary_hash()
         self.client = Client(
             user, path, binary_hash, init_repo=init_repo, remote_url=remote_url, **kwargs
         )
 
-        self.start_worker_routines()
+        if not single_thread:
+            self.start_worker_routines()
+
         return self.client.connection_warnings
 
     def check_client(self):
         return self.client is not None
 
     def status(self):
         if self.check_client():
@@ -458,14 +468,139 @@
                 return artifact
 
             artifact = self.enum(lookup_item)
             return artifact
 
         return None
 
+    def decompile(self, addr: int) -> Optional[str]:
+        if not self.decompiler_available:
+            return None
+
+        # TODO: make this a function call after transitioning decompiler artifacts to LiveState
+        for search_addr in (addr, self.artifact_lifer.lower_addr(addr)):
+            func_found = False
+            for func_addr, func in self.functions().items():
+                if func.addr <= search_addr < (func.addr + func.size):
+                    func_found = True
+                    break
+            else:
+                func = None
+
+            if func_found:
+                break
+        else:
+            return None
+
+        return self._decompile(func)
+
+    def _decompile(self, function: Function) -> Optional[str]:
+        return None
+
+    #
+    # Setters:
+    # Work like Fillers, except can function without a BS Client. In effect, this allows you to
+    # change the decompilers objects using BinSync objects.
+    # TODO: all the code in this category set_* is experimental and not ready for production use
+    # all this code should be implemented in the other decompilers or moved to a different project
+    #
+
+    def set_artifact(self, artifact: Artifact, lower=True, **kwargs) -> bool:
+        """
+        Sets a BinSync Artifact into the decompilers local database. This operations allows you to change
+        what the native decompiler sees with BinSync Artifacts. This is different from opertions on a BinSync State,
+        since this is native to the decompiler
+
+        >>> func = Function(0xdeadbeef, 0x800)
+        >>> func.name = "main"
+        >>> controller.set_artifact(func)
+
+        @param artifact:
+        @param lower:       Wether to convert the Artifacts types and offset into the local decompilers format
+        @return:            True if the Artifact was succesfuly set into the decompiler
+        """
+        set_map = {
+            Function: self.set_function,
+            FunctionHeader: self.set_function_header,
+            StackVariable: self.set_stack_variable,
+            Comment: self.set_comment,
+            GlobalVariable: self.set_global_var,
+            Struct: self.set_struct,
+            Enum: self.set_enum,
+            Patch: self.set_patch,
+            Artifact: None,
+        }
+
+        if lower:
+            artifact = self.lower_artifact(artifact)
+
+        setter = set_map.get(type(artifact), None)
+        if setter is None:
+            _l.critical(f"Unsupported object is attempting to be set, please check your object: {artifact}")
+            return False
+
+        return setter(artifact, **kwargs)
+
+    def set_function(self, func: Function, **kwargs) -> bool:
+        update = False
+        header = func.header
+        if header is not None:
+            update = self.set_function_header(header, **kwargs)
+
+        if func.stack_vars:
+            for variable in func.stack_vars.values():
+                update |= self.set_stack_variable(variable, **kwargs)
+
+        return update
+
+    def set_function_header(self, fheader: FunctionHeader, **kwargs) -> bool:
+        return False
+
+    def set_stack_variable(self, svar: StackVariable, **kwargs) -> bool:
+        return False
+
+    def set_comment(self, comment: Comment, **kwargs) -> bool:
+        return False
+
+    def set_global_var(self, gvar: GlobalVariable, **kwargs) -> bool:
+        return False
+
+    def set_struct(self, struct: Struct, header=True, members=True, **kwargs) -> bool:
+        return False
+
+    def set_enum(self, enum: Enum, **kwargs) -> bool:
+        return False
+
+    def set_patch(self, path: Patch, **kwargs) -> bool:
+        return False
+
+    #
+    # Change Callback API
+    # TODO: all the code in this category on_* is experimental and not ready for production use
+    # all this code should be implemented in the other decompilers or moved to a different project
+    #
+
+    def on_function_header_changed(self, fheader: FunctionHeader):
+        pass
+
+    def on_stack_variable_changed(self, svar: StackVariable):
+        pass
+
+    def on_comment_changed(self, comment: Comment):
+        pass
+
+    def on_struct_changed(self, struct: Struct):
+        pass
+
+    def on_enum_changed(self, enum: Enum):
+        pass
+
+    def on_global_variable_changed(self, gvar: GlobalVariable):
+        pass
+
     #
     # Client API & Shortcuts
     #
 
     def lift_artifact(self, artifact: Artifact) -> Artifact:
         return self.artifact_lifer.lift(artifact)
 
@@ -533,15 +668,15 @@
                 self.push_artifact(Function(func_addr, self.get_func_size(func_addr)), state=state, set_last_change=set_last_change)
 
         # lift artifact into standard BinSync format
         artifact = self.lift_artifact(artifact)
 
         # set the artifact in the target state, likely master
         _l.debug(f"Setting an artifact now into {state} as {artifact}")
-        was_set = set_artifact_func(state, artifact, set_last_change=set_last_change)
+        was_set = set_artifact_func(state, artifact, set_last_change=set_last_change, **kwargs)
 
         # TODO: make was_set reliable
         _l.debug(f"{state} committing now with {commit_msg or artifact.commit_msg}")
         self.client.commit_state(state, msg=commit_msg or artifact.commit_msg)
 
         return was_set
 
@@ -623,46 +758,41 @@
                 state=master_state,
                 set_last_change=False,
                 commit_msg=commit_msg
             )
 
         return fill_changes
 
-
-    @init_checker
     @fill_event
     def fill_struct(self, struct_name, header=True, members=True, artifact=None, **kwargs):
         """
 
         @param struct_name:
         @param user:
         @param state:
         @param header:
         @param members:
         @return:
         """
         _l.debug(f"Fill Struct is not implemented in your decompiler.")
         return False
 
-    @init_checker
     @fill_event
     def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
         """
         Grab a global variable for a specified address and fill it locally
 
         @param var_addr:
         @param user:
         @param state:
         @return:
         """
         _l.debug(f"Fill Global Var is not implemented in your decompiler.")
         return False
 
-
-    @init_checker
     @fill_event
     def fill_enum(self, enum_name, user=None, artifact=None, **kwargs):
         """
         Grab an enum and fill it locally
 
         @param enum_name:
         @param user:
@@ -683,15 +813,14 @@
         return False
 
     @fill_event
     def fill_comment(self, addr, user=None, artifact=None, **kwargs):
         _l.debug(f"Fill Comments is not implemented in your decompiler.")
         return False
 
-    @init_checker
     @fill_event
     def fill_function(self, func_addr, user=None, artifact=None, **kwargs):
         """
         Grab all relevant information from the specified user and fill the @func_addr.
         """
         dec_func: Function = self.function(func_addr, **kwargs)
         if not dec_func:
@@ -723,24 +852,22 @@
 
         # comments
         for addr, cmt in kwargs['state'].get_func_comments(func_addr).items():
             changes |= self.fill_comment(addr, artifact=cmt, **kwargs)
 
         return changes
 
-    @init_checker
     def fill_functions(self, user=None, **kwargs):
         change = False
         master_state, state = self.get_master_and_user_state(user=user, **kwargs)
         for addr, func in state.functions.items():
             change |= self.fill_function(addr, state=state, master_state=master_state)
 
         return change
 
-    @init_checker
     def fill_structs(self, user=None, **kwargs):
         """
         Grab all the structs from a specified user, then fill them locally
 
         @param user:
         @param state:
         @return:
@@ -752,15 +879,14 @@
             changes |= self.fill_struct(name, user=user, state=state, master_state=master_state, members=False)
 
         for name, struct in state.structs.items():
             changes |= self.fill_struct(name, user=user, state=state, master_state=master_state, header=False)
 
         return changes
 
-    @init_checker
     def fill_enums(self, user=None, **kwargs):
         """
         Grab all enums and fill it locally
 
         @param user:
         @param state:
         @return:
@@ -768,24 +894,22 @@
         changes = False
         master_state, state = self.get_master_and_user_state(user=user, **kwargs)
         for name, enum in state.enums.items():
             changes |= self.fill_enum(name, user=user, state=state, master_state=master_state)
 
         return changes
 
-    @init_checker
     def fill_global_vars(self, user=None, **kwargs):
         changes = False
         master_state, state = self.get_master_and_user_state(user=user, **kwargs)
         for off, gvar in state.global_vars.items():
             changes |= self.fill_global_var(off, user=user, state=state, master_state=master_state)
 
         return changes
 
-    @init_checker
     def fill_all(self, user=None, **kwargs):
         """
         Connected to the Sync All action:
         syncs in all the data from the targeted user
 
         @param user:
         @param state:
```

### Comparing `binsync-3.6.0/binsync/common/ui/config_dialog.py` & `binsync-3.9.0/binsync/ui/config_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import time
 from pathlib import Path
 from typing import Optional
 
 from binsync.core.client import ConnectionWarnings, BINSYNC_ROOT_BRANCH
 from binsync.data.configuration import ProjectConfig
-from binsync.common.ui.qt_objects import (
+from binsync.ui.qt_objects import (
     QCheckBox,
     QDialog,
     QDir,
     QFileDialog,
     QGridLayout,
     QHBoxLayout,
     QLabel,
@@ -19,15 +19,15 @@
     QMessageBox,
     QPushButton,
     QVBoxLayout,
     QTableWidget,
     QTableWidgetItem,
     QHeaderView
 )
-from binsync.common.ui.utils import QCollapsibleBox
+from binsync.ui.utils import QCollapsibleBox
 
 l = logging.getLogger(__name__)
 
 
 class BSProjectDialog(QDialog):
     TITLE = "BS Project Dialog"
```

### Comparing `binsync-3.6.0/binsync/common/ui/control_panel.py` & `binsync-3.9.0/binsync/ui/control_panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import logging
-import time
 
 import binsync.data
-from binsync.common.ui.force_push.force_push import ForcePushUI
-from binsync.common.ui.panel_tabs.activity_table import QActivityTable
-from binsync.common.ui.panel_tabs.ctx_table import QCTXTable
-from binsync.common.ui.panel_tabs.functions_table import QFunctionTable
-from binsync.common.ui.panel_tabs.globals_table import QGlobalsTable
-from binsync.common.ui.panel_tabs.util_panel import QUtilPanel
-from binsync.common.ui.qt_objects import (
+from binsync.ui.panel_tabs.activity_table import QActivityTable
+from binsync.ui.panel_tabs.ctx_table import QCTXTable
+from binsync.ui.panel_tabs.functions_table import QFunctionTable
+from binsync.ui.panel_tabs.globals_table import QGlobalsTable
+from binsync.ui.panel_tabs.util_panel import QUtilPanel
+from binsync.ui.qt_objects import (
     QLabel,
     QMenu,
-    QPushButton,
     QStatusBar,
     QTabWidget,
     QVBoxLayout,
     QWidget,
     Signal,
     Slot
 )
```

### Comparing `binsync-3.6.0/binsync/common/ui/force_push/force_push.py` & `binsync-3.9.0/binsync/ui/force_push/force_push.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
-from binsync.common.ui.force_push.panels.functions_table import QFunctionTable
-from binsync.common.ui.force_push.panels.global_panel import QGlobalsTable
-from binsync.common.ui.qt_objects import (
+from binsync.ui.force_push.panels.functions_table import QFunctionTable
+from binsync.ui.force_push.panels.global_panel import QGlobalsTable
+from binsync.ui.qt_objects import (
     QTabWidget,
     QVBoxLayout,
     QWidget,
     Signal
 )
 
 l = logging.getLogger(__name__)
```

### Comparing `binsync-3.6.0/binsync/common/ui/force_push/panels/functions_table.py` & `binsync-3.9.0/binsync/ui/force_push/panels/functions_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from datetime import datetime
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.qt_objects import (
     QAbstractItemView,
     QAbstractTableModel,
     QHeaderView,
     Qt,
     QModelIndex,
     QSortFilterProxyModel,
     QFocusEvent,
@@ -16,15 +16,15 @@
     QFontDatabase,
     QWidget,
     QVBoxLayout,
     QPushButton,
     QPersistentModelIndex,
     QCheckBox
 )
-from binsync.common.ui.utils import friendly_datetime
+from binsync.ui.utils import friendly_datetime
 from binsync.data.state import State
 from binsync.core.scheduler import SchedSpeed
 
 l = logging.getLogger(__name__)
 
 
 class FunctionTableModel(QAbstractTableModel):
@@ -39,15 +39,15 @@
     # This is *most likely* alright, definitely works on linux, could use a macos/windows pass.
     # Custom defined role for sorting (since we shouldn't sort hex numbers alphabetically)
     SortRole = Qt.UserRole + 1000
 
     # Color for most recently updated, the alpha value decreases linearly over controller.table_coloring_window
     ACTIVE_FUNCTION_COLOR = (100, 255, 100, 70)
 
-    def __init__(self, controller: BinSyncController, data=None, parent=None):
+    def __init__(self, controller: BSController, data=None, parent=None):
         super().__init__(parent)
         self.controller = controller
         self.row_data = data if data else []
         
         self.checks = [False for _ in self.row_data]
         self.HEADER[1] = 'Name'
 
@@ -185,15 +185,15 @@
             self.user_unfocused = True
         super(FunctionTableFilterLineEdit, self).focusOutEvent(event)
 
 
 class FunctionTableView(QTableView):
     """ Table view for the data, this is the front end "container" for our model. """
 
-    def __init__(self, controller: BinSyncController, filteredit: FunctionTableFilterLineEdit, parent=None):
+    def __init__(self, controller: BSController, filteredit: FunctionTableFilterLineEdit, parent=None):
         super().__init__(parent=parent)
         self.controller = controller
 
         self.filteredit = filteredit
         self.filteredit.textChanged.connect(self.handle_filteredit_change)
 
         # Create a SortFilterProxyModel to allow for sorting/filtering
@@ -315,15 +315,15 @@
         for i in range(self.proxymodel.rowCount()):
             proxyIndex = self.proxymodel.index(i, 0, QModelIndex())
             mappedIndex = self.proxymodel.mapToSource(proxyIndex)
             self.model.setData(mappedIndex, False, Qt.CheckStateRole)
 
 class QFunctionTable(QWidget):
     """ Wrapper widget to contain the function table classes in one file (prevents bulking up control_panel.py) """
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def toggle_select_all(self):
         if self.checkbox.isChecked():
             self.table.check_all()
```

### Comparing `binsync-3.6.0/binsync/common/ui/force_push/panels/global_panel.py` & `binsync-3.9.0/binsync/ui/force_push/panels/global_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import logging
 from datetime import datetime
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.qt_objects import (
     QAbstractItemView,
     QAbstractTableModel,
     QHeaderView,
     Qt,
     QModelIndex,
     QSortFilterProxyModel,
     QFocusEvent,
     QKeyEvent,
     QLineEdit,
     QTableView,
     QFontDatabase,
     QWidget,
     QVBoxLayout,
-    QPersistentModelIndex,
     QCheckBox,
     QPushButton
 )
-from binsync.common.ui.utils import friendly_datetime
+from binsync.ui.utils import friendly_datetime
 
 l = logging.getLogger(__name__)
 
 
 class GlobalTableModel(QAbstractTableModel):
     """Table model that controls backend behavior of the global table"""
     HEADER = [
@@ -37,15 +36,15 @@
     # This is *most likely* alright, definitely works on linux, could use a macos/windows pass.
     # Custom defined role for sorting (since we shouldn't sort hex numbers alphabetically)
     SortRole = Qt.UserRole + 1000
 
     # Color for most recently updated, the alpha value decreases linearly over controller.table_coloring_window
     ACTIVE_GLOBAL_COLOR = (100, 255, 100, 70)
 
-    def __init__(self, controller: BinSyncController, data=None, parent=None):
+    def __init__(self, controller: BSController, data=None, parent=None):
         super().__init__(parent)
         self.controller = controller
         # holds sublists of form: (type, remote name, user, last push)
         self.row_data = data if data else []
         self.checks = [False for _ in self.row_data]
         self.gvar_name_to_addr_map = {}
 
@@ -193,15 +192,15 @@
             self.user_unfocused = True
         super(GlobalTableFilterLineEdit, self).focusOutEvent(event)
 
 
 class GlobalTableView(QTableView):
     """ Table view for the data, this is the front end "container" for our model. """
 
-    def __init__(self, controller: BinSyncController, filteredit: GlobalTableFilterLineEdit, parent=None):
+    def __init__(self, controller: BSController, filteredit: GlobalTableFilterLineEdit, parent=None):
         super().__init__(parent=parent)
         self.controller = controller
 
         self.filteredit = filteredit
         self.filteredit.textChanged.connect(self.handle_filteredit_change)
 
         # Create a SortFilterProxyModel to allow for sorting/filtering
@@ -306,15 +305,15 @@
             mappedIndex = self.proxymodel.mapToSource(proxyIndex)
             self.model.setData(mappedIndex, False, Qt.CheckStateRole)
 
 
 class QGlobalsTable(QWidget):
     """ Wrapper widget to contain the globals table classes in one file (prevents bulking up control_panel.py) """
 
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def toggle_select_all(self):
         if self.checkbox.isChecked():
             self.table.check_all()
```

### Comparing `binsync-3.6.0/binsync/common/ui/magic_sync_dialog.py` & `binsync-3.9.0/binsync/ui/magic_sync_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from binsync.common.ui.qt_objects import (
+from .qt_objects import (
     QDialog,
     QDialogButtonBox,
     QGridLayout,
     QVBoxLayout,
     QLabel,
     QComboBox,
     Qt
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/activity_table.py` & `binsync-3.9.0/binsync/ui/panel_tabs/activity_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import logging
-import time
 from collections import defaultdict
 from typing import Dict
-import datetime
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
+from binsync.ui.qt_objects import (
     QMenu,
     QAction,
     QWidget,
     QVBoxLayout,
-    QColor,
     Qt
 )
-from binsync.common.ui.utils import friendly_datetime
+from binsync.ui.utils import friendly_datetime
 from binsync.core.scheduler import SchedSpeed
 from binsync.data import Function
 
 l = logging.getLogger(__name__)
 
 
 class ActivityTableModel(BinsyncTableModel):
-    def __init__(self, controller: BinSyncController, col_headers=None, filter_cols=None, time_col=None,
+    def __init__(self, controller: BSController, col_headers=None, filter_cols=None, time_col=None,
                  addr_col=None, parent=None):
         super().__init__(controller, col_headers, filter_cols, time_col, addr_col, parent)
         self.data_dict = {}
         self.saved_color_window = self.controller.table_coloring_window
         self.context_menu_cache = {}
 
     def data(self, index, role=Qt.DisplayRole):
@@ -92,15 +89,15 @@
         self.context_menu_cache = cmenu_cache
         self._update_changed_rows(self.data_dict, updated_row_keys)
         self.refresh_time_cells()
 
 class ActivityTableView(BinsyncTableView):
     HEADER = ['User', 'Activity', 'Last Push']
 
-    def __init__(self, controller: BinSyncController, filteredit: BinsyncTableFilterLineEdit=None, stretch_col=None,
+    def __init__(self, controller: BSController, filteredit: BinsyncTableFilterLineEdit=None, stretch_col=None,
                  col_count=None, parent=None):
         super().__init__(controller, filteredit, stretch_col, col_count, parent)
 
         self.model = ActivityTableModel(controller, self.HEADER, filter_cols=[0, 1], time_col=2,
                                         parent=parent)
         self.proxymodel.setSourceModel(self.model)
         self.setModel(self.proxymodel)
@@ -167,15 +164,15 @@
 
         menu.popup(self.mapToGlobal(event.pos()))
 
 
 class QActivityTable(QWidget):
     """ Wrapper widget to contain the function table classes in one file (prevents bulking up control_panel.py) """
 
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def _init_widgets(self):
         self.table = ActivityTableView(self.controller, filteredit=None, stretch_col=1, col_count=3)
         layout = QVBoxLayout()
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/ctx_table.py` & `binsync-3.9.0/binsync/ui/panel_tabs/ctx_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import logging
-import time
-from functools import partial
-from typing import Dict
-import datetime
-
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
-from binsync.common.ui.qt_objects import (
+
+from binsync.api.controller import BSController
+from binsync.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableView
+from binsync.ui.qt_objects import (
     QMenu,
     QAction,
     Qt
 )
-from binsync.common.ui.utils import friendly_datetime
-from binsync.core.scheduler import SchedSpeed
-from binsync.data import Function
+from binsync.ui.utils import friendly_datetime
 
 l = logging.getLogger(__name__)
 
 
 class CTXTableModel(BinsyncTableModel):
-    def __init__(self, controller: BinSyncController, col_headers=None, filter_cols=None, time_col=None,
+    def __init__(self, controller: BSController, col_headers=None, filter_cols=None, time_col=None,
                  addr_col=None, parent=None):
         super().__init__(controller, col_headers, filter_cols, time_col, addr_col, parent)
         self.data_dict = {}
         self.saved_color_window = self.controller.table_coloring_window
 
         self.saved_ctx = None
 
@@ -77,15 +71,15 @@
             self._update_changed_rows(self.data_dict, updated_row_keys)
         self.refresh_time_cells()
 
 
 class QCTXTable(BinsyncTableView):
     HEADER = ['User', 'Remote Name', 'Last Push']
 
-    def __init__(self, controller: BinSyncController, stretch_col=None,
+    def __init__(self, controller: BSController, stretch_col=None,
                  col_count=None, parent=None):
         super().__init__(controller, None, 1, 3, parent)
 
         self.model = CTXTableModel(controller, self.HEADER, filter_cols=[0, 1], time_col=2,
                                         parent=parent)
         self.proxymodel.setSourceModel(self.model)
         self.setModel(self.proxymodel)
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/functions_table.py` & `binsync-3.9.0/binsync/ui/panel_tabs/functions_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import datetime
 import logging
 import time
 from typing import Dict
 from collections import defaultdict
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
+from binsync.ui.qt_objects import (
     QMenu,
     QAction,
     QWidget,
     QVBoxLayout,
     QColor,
     Qt
 )
-from binsync.common.ui.utils import friendly_datetime
+from binsync.ui.utils import friendly_datetime
 from binsync.core.scheduler import SchedSpeed
 from binsync.data import Function
 
 l = logging.getLogger(__name__)
 
 
 class FunctionTableModel(BinsyncTableModel):
-    def __init__(self, controller: BinSyncController, col_headers=None, filter_cols=None, time_col=None,
+    def __init__(self, controller: BSController, col_headers=None, filter_cols=None, time_col=None,
                  addr_col=None, parent=None):
         super().__init__(controller, col_headers, filter_cols, time_col, addr_col, parent)
         self.data_dict = {}
         self.context_menu_cache = {}
 
     def data(self, index, role=Qt.DisplayRole):
         if not index.isValid():
@@ -81,15 +81,15 @@
         self.context_menu_cache = cmenu_cache
         self._update_changed_rows(self.data_dict, updated_row_keys)
         self.refresh_time_cells()
 
 class FunctionTableView(BinsyncTableView):
     HEADER = ['Addr', 'Remote Name', 'User', 'Last Push']
 
-    def __init__(self, controller: BinSyncController, filteredit: BinsyncTableFilterLineEdit, stretch_col=None,
+    def __init__(self, controller: BSController, filteredit: BinsyncTableFilterLineEdit, stretch_col=None,
                  col_count=None, parent=None):
         super().__init__(controller, filteredit, stretch_col, col_count, parent)
 
         self.model = FunctionTableModel(controller, self.HEADER, filter_cols=[0, 1], time_col=3, addr_col=0,
                                         parent=parent)
         self.proxymodel.setSourceModel(self.model)
         self.setModel(self.proxymodel)
@@ -159,15 +159,15 @@
                     lambda checked=False, name=username: self.controller.fill_function(func_addr, user=name))
         menu.popup(self.mapToGlobal(event.pos()))
 
 
 class QFunctionTable(QWidget):
     """ Wrapper widget to contain the function table classes in one file (prevents bulking up control_panel.py) """
 
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def _init_widgets(self):
         self.filteredit = BinsyncTableFilterLineEdit(parent=self)
         self.table = FunctionTableView(self.controller, self.filteredit, stretch_col=1, col_count=4)
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/globals_table.py` & `binsync-3.9.0/binsync/ui/panel_tabs/globals_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import logging
-import time
 from collections import defaultdict
-from typing import Dict
 import re
-import datetime
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.panel_tabs.table_model import BinsyncTableModel, BinsyncTableFilterLineEdit, BinsyncTableView
+from binsync.ui.qt_objects import (
     QMenu,
     QAction,
     QWidget,
     QVBoxLayout,
-    QColor,
     Qt
 )
-from binsync.common.ui.utils import friendly_datetime
+from binsync.ui.utils import friendly_datetime
 from binsync.core.scheduler import SchedSpeed
-from binsync.data import Function
 
 l = logging.getLogger(__name__)
 
 
 class GlobalsTableModel(BinsyncTableModel):
-    def __init__(self, controller: BinSyncController, col_headers=None, filter_cols=None, time_col=None,
+    def __init__(self, controller: BSController, col_headers=None, filter_cols=None, time_col=None,
                  addr_col=None, parent=None):
         super().__init__(controller, col_headers, filter_cols, time_col, addr_col, parent)
         self.data_dict = {}
         self.saved_color_window = self.controller.table_coloring_window
         self.context_menu_cache = {}
 
     def data(self, index, role=Qt.DisplayRole):
@@ -96,15 +91,15 @@
         self.context_menu_cache = cmenu_cache
         self._update_changed_rows(self.data_dict, updated_row_keys)
         self.refresh_time_cells()
 
 
 class GlobalsTableView(BinsyncTableView):
     HEADER = ['T', 'Name', 'User', 'Last Push']
-    def __init__(self, controller: BinSyncController, filteredit: BinsyncTableFilterLineEdit, stretch_col=None,
+    def __init__(self, controller: BSController, filteredit: BinsyncTableFilterLineEdit, stretch_col=None,
                  col_count=None, parent=None):
         super().__init__(controller, filteredit, stretch_col, col_count, parent)
 
         self.model = GlobalsTableModel(controller, self.HEADER, filter_cols=[0, 1, 2], time_col=3,
                                         parent=parent)
         self.proxymodel.setSourceModel(self.model)
         self.setModel(self.proxymodel)
@@ -200,15 +195,15 @@
                 action.triggered.connect(filler_func(username))
 
         menu.popup(self.mapToGlobal(event.pos()))
 
 class QGlobalsTable(QWidget):
     """ Wrapper widget to contain the function table classes in one file (prevents bulking up control_panel.py) """
 
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def _init_widgets(self):
         self.filteredit = BinsyncTableFilterLineEdit(parent=self)
         self.table = GlobalsTableView(self.controller, self.filteredit, stretch_col=1, col_count=4)
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/table_model.py` & `binsync-3.9.0/binsync/ui/panel_tabs/table_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import datetime
-from typing import List, Dict, Set
+from typing import Dict, Set
 
-from binsync.common.controller import BinSyncController
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController
+from binsync.ui.qt_objects import (
     QAbstractItemView,
     QAbstractTableModel,
     QHeaderView,
     Qt,
     QModelIndex,
     QSortFilterProxyModel,
     QColor,
@@ -15,29 +15,29 @@
     QKeyEvent,
     QLineEdit,
     QTableView,
     QFontDatabase,
     Signal,
     Slot,
 )
-from binsync.common.ui.utils import friendly_datetime
+
 l = logging.getLogger(__name__)
 
 
 class BinsyncTableModel(QAbstractTableModel):
     # Custom defined role for sorting/filtering (since we shouldn't sort hex numbers alphabetically)
     SortRole = Qt.UserRole + 1000
     FilterRole = Qt.UserRole + 1001
 
     # Color for most recently updated, the alpha value decreases linearly over controller.table_coloring_window
     ACTIVE_FUNCTION_COLOR = (100, 255, 100, 70)
 
     update_signal = Signal(list, list)
 
-    def __init__(self, controller: BinSyncController, col_headers=None, filter_cols=None, time_col=None, addr_col=None, parent=None):
+    def __init__(self, controller: BSController, col_headers=None, filter_cols=None, time_col=None, addr_col=None, parent=None):
         """
         Template class for a Binsync Table
 
         :param controller:    BinSyncController instance
         :param col_headers:   List of column header names
         :param col_dtypes:    List of data types (corresponding to the header names), supported
                               dtypes are {str, int, "time", "hex"}.
@@ -224,15 +224,15 @@
             self.user_unfocused = True
         super(BinsyncTableFilterLineEdit, self).focusOutEvent(event)
 
 
 class BinsyncTableView(QTableView):
     """ Table view for the data, this is the front end "container" for our model. """
 
-    def __init__(self, controller: BinSyncController, filteredit: BinsyncTableFilterLineEdit=None, stretch_col=None, col_count=None, parent=None):
+    def __init__(self, controller: BSController, filteredit: BinsyncTableFilterLineEdit=None, stretch_col=None, col_count=None, parent=None):
         """
         Template class for a Binsync Table View, required to create and set the model (extend BinsyncTableModel)
 
         :param controller:    BinSyncController instance
         :param filteredit:    An instance of BinsyncTableFilterLineEdit
         :param stretch_col:   Column to stretch (resize) when table is resized
         :param col_count:     Number of columns this table will have
```

### Comparing `binsync-3.6.0/binsync/common/ui/panel_tabs/util_panel.py` & `binsync-3.9.0/binsync/ui/panel_tabs/util_panel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 
-from binsync.common.controller import BinSyncController, MergeLevel
-from binsync.common.ui.qt_objects import (
+from binsync.api.controller import BSController, MergeLevel
+from binsync.ui.qt_objects import (
     QCheckBox,
     QComboBox,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
     Qt,
     QVBoxLayout,
     QWidget,
     QLineEdit,
     QIntValidator
 )
-from binsync.common.ui.magic_sync_dialog import MagicSyncDialog
-from binsync.common.ui.force_push import ForcePushUI
-from binsync.common.controller import BinSyncController
-from binsync.core.scheduler import SchedSpeed
+from binsync.ui.magic_sync_dialog import MagicSyncDialog
+from binsync.ui.force_push import ForcePushUI
+from binsync.api.controller import BSController
+from binsync.extras import EXTRAS_AVAILABLE
 
 l = logging.getLogger(__name__)
 
 
 class QUtilPanel(QWidget):
-    def __init__(self, controller: BinSyncController, parent=None):
+    def __init__(self, controller: BSController, parent=None):
         super().__init__(parent)
         self.controller = controller
         self._init_widgets()
 
     def _init_widgets(self):
 
         #
@@ -128,20 +128,49 @@
         main_layout = QVBoxLayout()
         main_layout.setContentsMargins(10, 20, 10, 20)
         main_layout.setSpacing(18)
         main_layout.setAlignment(Qt.AlignTop)
         main_layout.addWidget(sync_options_group)
         main_layout.addWidget(dev_options_group)
         main_layout.addWidget(ui_options_group)
+        if EXTRAS_AVAILABLE:
+            main_layout.addWidget(self._create_extras_group())
         main_layout.addWidget(self._save_apply_config_option)
         self.setLayout(main_layout)
 
     #
+    # Extras GUI (only available if extras are installed)
+    #
+
+    def _create_extras_group(self):
+        extras_group = QGroupBox()
+        extras_layout = QVBoxLayout()
+        extras_group.setTitle("BS Extras")
+
+        #
+        # AI Extras
+        #
+
+        ai_button = QPushButton("Add AI User...")
+        ai_button.clicked.connect(self._handle_add_ai_user)
+        extras_layout.addWidget(ai_button)
+
+        extras_group.setLayout(extras_layout)
+        return extras_group
+
+    def _handle_add_ai_user(self):
+        from binsync.extras.ai.ai_user_config import AIUserConfigDialog
+        dialog = AIUserConfigDialog(self.controller)
+        dialog.exec_()
+
+
+    #
     # Event Handlers
     #
+
     def _handle_table_coloring_change(self):
         try:
             val = int(self._table_coloring_window_lineedit.text())
             self.controller.table_coloring_window = val
         except ValueError:
             pass
```

### Comparing `binsync-3.6.0/binsync/common/ui/qt_objects.py` & `binsync-3.9.0/binsync/ui/qt_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from binsync.common.ui.version import ui_version
+from binsync.ui.version import ui_version
 
 if ui_version == "PySide2":
     from PySide2.QtCore import (
         QDir, Qt, Signal, QAbstractTableModel, QModelIndex, QSortFilterProxyModel, QPersistentModelIndex,
         QEvent, QThread, Slot, QObject, QPropertyAnimation, QAbstractAnimation, QParallelAnimationGroup
     )
     from PySide2.QtWidgets import (
```

### Comparing `binsync-3.6.0/binsync/common/ui/utils.py` & `binsync-3.9.0/binsync/ui/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import logging
 
-from binsync.common.ui.qt_objects import (
+from binsync.ui.qt_objects import (
     QFrame,
     QWidget,
     QScrollArea,
     QSizePolicy,
     Qt,
     QPropertyAnimation,
     QAbstractAnimation,
```

### Comparing `binsync-3.6.0/binsync/core/cache.py` & `binsync-3.9.0/binsync/core/cache.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/core/client.py` & `binsync-3.9.0/binsync/core/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from binsync.core.cache import Cache
 
 
 l = logging.getLogger(__name__)
 BINSYNC_BRANCH_PREFIX = 'binsync'
 BINSYNC_ROOT_BRANCH = f'{BINSYNC_BRANCH_PREFIX}/__root__'
 
+logging.getLogger("git").setLevel(logging.ERROR)
+
 
 class ConnectionWarnings:
     HASH_MISMATCH = 0
 
 
 def atomic_git_action(f):
     """
```

### Comparing `binsync-3.6.0/binsync/core/scheduler.py` & `binsync-3.9.0/binsync/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/__init__.py` & `binsync-3.9.0/binsync/data/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,8 +5,7 @@
 from binsync.data.patch import Patch
 from binsync.data.stack_variable import StackVariable
 from binsync.data.struct import StructMember, Struct
 from binsync.data.global_variable import GlobalVariable
 from binsync.data.enum import Enum
 from binsync.data.state import State, ArtifactType
 from binsync.data.configuration import ProjectConfig, GlobalConfig
-from binsync.data.type_parser import BSType, BSTypeParser
```

### Comparing `binsync-3.6.0/binsync/data/artifact.py` & `binsync-3.9.0/binsync/data/artifact.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/comment.py` & `binsync-3.9.0/binsync/data/comment.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,46 @@
         "comment",
         "decompiled",
 
     )
 
     def __init__(self, addr, comment,  func_addr=None, decompiled=False, last_change=None):
         super(Comment, self).__init__(last_change=last_change)
-        self.comment = comment  # type: str
-        self.decompiled = decompiled  # TODO: use this in other places!
+        if comment:
+            self.comment = self.linewrap_comment(comment)
+
+        self.decompiled = decompiled
         self.addr = addr  # type: int
         self.func_addr = func_addr
 
     def __str__(self):
         return f"<Comment: @{hex(self.addr)} len={len(self.comment)}>"
 
     def __repr__(self):
         return self.__str__()
 
+    @staticmethod
+    def linewrap_comment(comment: str, width=80):
+        lines = comment.splitlines()
+        final_comment = ""
+
+        for line in lines:
+            if len(line) < width:
+                final_comment += line + "\n"
+                continue
+
+            for i, c in enumerate(line):
+                if i % width == 0 and i != 0:
+                    final_comment += "\n"
+                final_comment += c
+
+            final_comment += "\n"
+
+        return final_comment
+
     @classmethod
     def parse(cls, s):
         comm = Comment(None, None)
         comm.__setstate__(toml.loads(s))
         return comm
 
     @classmethod
```

### Comparing `binsync-3.6.0/binsync/data/configuration.py` & `binsync-3.9.0/binsync/data/configuration.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/enum.py` & `binsync-3.9.0/binsync/data/enum.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/func.py` & `binsync-3.9.0/binsync/data/func.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/global_variable.py` & `binsync-3.9.0/binsync/data/global_variable.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/patch.py` & `binsync-3.9.0/binsync/data/patch.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/stack_variable.py` & `binsync-3.9.0/binsync/data/stack_variable.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/state.py` & `binsync-3.9.0/binsync/data/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,50 +369,55 @@
 
     #
     # Setters
     #
 
     @dirty_checker
     @update_last_change
-    def set_function(self, function: Function, set_last_change=True):
+    def set_function(self, function: Function, set_last_change=True, **kwargs):
         if function.addr in self.functions and self.functions[function.addr] == function:
             return False
 
         self.functions[function.addr] = function
         return True
 
     @dirty_checker
     @update_last_change
-    def set_function_header(self, func_header: FunctionHeader, set_last_change=True):
+    def set_function_header(self, func_header: FunctionHeader, set_last_change=True, **kwargs):
         if func_header.addr in self.functions and self.functions[func_header.addr] == func_header:
             return False
 
         self.functions[func_header.addr].header = func_header
         return True
 
     @dirty_checker
     @update_last_change
-    def set_comment(self, comment: Comment, set_last_change=True):
+    def set_comment(self, comment: Comment, append=False, set_last_change=True, **kwargs):
         if not comment:
             return False
 
         try:
             old_cmt = self.comments[comment.addr]
         except KeyError:
             old_cmt = None
 
         if old_cmt != comment:
+            if old_cmt is not None and append:
+                comment.comment = old_cmt.comment + "\n" + comment.comment
+                if set_last_change:
+                    comment.last_change = comment.last_change or old_cmt.last_change
+
             self.comments[comment.addr] = comment
             return True
 
         return False
 
     @dirty_checker
     @update_last_change
-    def set_patch(self, patch, addr, set_last_change=True):
+    def set_patch(self, patch, addr, set_last_change=True, **kwargs):
         if not patch:
             return False
 
         try:
             old_patch = self.patches[addr]
         except KeyError:
             old_patch = None
@@ -421,15 +426,15 @@
             self.patches[addr] = patch
             return True
 
         return False
 
     @dirty_checker
     @update_last_change
-    def set_stack_variable(self, variable: StackVariable, set_last_change=True):
+    def set_stack_variable(self, variable: StackVariable, set_last_change=True, **kwargs):
         if not variable:
             return False
 
         func = self.get_function(variable.addr)
         if not func:
             return False
 
@@ -442,15 +447,15 @@
             func.stack_vars[variable.offset] = variable
             return True
 
         return False
 
     @dirty_checker
     @update_last_change
-    def set_struct(self, struct: Struct, old_name=None, set_last_change=True):
+    def set_struct(self, struct: Struct, old_name=None, set_last_change=True, **kwargs):
         """
         Sets a struct in the current state. If old_name is not defined (None), then
         this indicates that the struct has not changed names. In that case, simply overwrite the
         internal representation of the struct.
 
         If the old_name is defined, than a struct has changed names. In that case, delete
         the internal struct data and delete the related .toml file.
@@ -478,29 +483,29 @@
             self.structs[struct.name] = struct
             return True
 
         return False
 
     @dirty_checker
     @update_last_change
-    def set_global_var(self, gloabl_var: GlobalVariable, set_last_change=True):
+    def set_global_var(self, gloabl_var: GlobalVariable, set_last_change=True, **kwargs):
         try:
             old_gvar = self.global_vars[gloabl_var.addr]
         except KeyError:
             old_gvar = None
 
         if old_gvar != gloabl_var:
             self.global_vars[gloabl_var.addr] = gloabl_var
             return True
 
         return False
 
     @dirty_checker
     @update_last_change
-    def set_enum(self, enum: Enum, set_last_change=True):
+    def set_enum(self, enum: Enum, set_last_change=True, **kwargs):
         try:
             old_enum = self.enums[enum.name]
         except KeyError:
             old_enum = None
 
         if old_enum != enum:
             self.enums[enum.name] = enum
```

### Comparing `binsync-3.6.0/binsync/data/struct.py` & `binsync-3.9.0/binsync/data/struct.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/type_parser.py` & `binsync-3.9.0/binsync/api/type_parser.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/data/user.py` & `binsync-3.9.0/binsync/data/user.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/decompilers/angr/artifact_lifter.py` & `binsync-3.9.0/binsync/decompilers/angr/artifact_lifter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from binsync.common import ArtifactLifter
+from binsync.api import BSArtifactLifter
 
 
-class AngrArtifactLifter(ArtifactLifter):
+class AngrArtifactLifter(BSArtifactLifter):
     """
     TODO: fix me
     """
     def __init__(self, controller):
         super(AngrArtifactLifter, self).__init__(controller)
 
     def lift_addr(self, addr: int) -> int:
```

### Comparing `binsync-3.6.0/binsync/decompilers/angr/control_panel_view.py` & `binsync-3.9.0/binsync/decompilers/angr/control_panel_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
 from angrmanagement.ui.views.view import BaseView
-from binsync.common.ui.version import set_ui_version
+from binsync.ui.version import set_ui_version
 
 set_ui_version("PySide6")
-from binsync.common.ui.control_panel import ControlPanel
-from binsync.common.ui.qt_objects import QVBoxLayout
+from binsync.ui.control_panel import ControlPanel
+from binsync.ui.qt_objects import QVBoxLayout
 
-from .controller import AngrBinSyncController
+from .controller import AngrBSController
 
 
 l = logging.getLogger(__name__)
 
 
 class ControlPanelView(BaseView):
     """
@@ -20,15 +20,15 @@
     """
 
     def __init__(self, instance, default_docking_position, controller, *args, **kwargs):
         super().__init__('sync', instance, instance.workspace, default_docking_position, *args, **kwargs)
 
         self.base_caption = "BinSync: Control Panel"
 
-        self.controller: AngrBinSyncController = controller
+        self.controller: AngrBSController = controller
         self.control_panel = ControlPanel(self.controller)
         self._init_widgets()
 
         self.width_hint = 300
 
     def reload(self):
         pass
```

### Comparing `binsync-3.6.0/binsync/decompilers/angr/plugin.py` & `binsync-3.9.0/binsync/decompilers/angr/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # pylint: disable=wrong-import-position,wrong-import-order
 import logging
 
 import binsync
 from angrmanagement.plugins import BasePlugin
 from angrmanagement.ui.workspace import Workspace
-from binsync.common.ui.version import set_ui_version
+from binsync.ui.version import set_ui_version
 
 set_ui_version("PySide6")
-from binsync.common.ui.config_dialog import ConfigureBSDialog
+from binsync.ui.config_dialog import ConfigureBSDialog
 from .control_panel_view import ControlPanelView
-from .controller import AngrBinSyncController
+from .controller import AngrBSController
 
 from binsync.data import (
     StackVariable, Function, FunctionHeader, Comment
 )
 
 l = logging.getLogger(__name__)
 
@@ -28,15 +28,15 @@
         that pushes and pulls changes every so many seconds.
 
         @param workspace:   an AM _workspace (usually found in _instance)
         """
         super().__init__(workspace)
 
         # init the Sync View on load
-        self.controller = AngrBinSyncController(self.workspace)
+        self.controller = AngrBSController(workspace=self.workspace)
         self.control_panel_view = ControlPanelView(workspace.main_instance, 'right', self.controller)
 
         self.controller.control_panel = self.control_panel_view
 
         self.sync_menu = None
         self.selected_funcs = []
 
@@ -101,15 +101,15 @@
     # pylint: disable=unused-argument
     def handle_stack_var_renamed(self, func, offset, old_name, new_name):
         if func is None:
             return False
 
         decompilation = self.controller.decompile_function(func)
         stack_var = self.controller.find_stack_var_in_codegen(decompilation, offset)
-        var_type = AngrBinSyncController.stack_var_type_str(decompilation, stack_var)
+        var_type = AngrBSController.stack_var_type_str(decompilation, stack_var)
 
         self.controller.schedule_job(
             self.controller.push_artifact,
             StackVariable(offset, new_name, var_type, stack_var.size, func.addr)
         )
         return False
 
@@ -123,40 +123,30 @@
             StackVariable(offset, stack_var.name, new_type, stack_var.size, func.addr),
         )
         return False
 
     # pylint: disable=unused-argument
     def handle_func_arg_renamed(self, func, offset, old_name, new_name):
         decompilation = self.controller.decompile_function(func)
-        func_args = AngrBinSyncController.get_func_args(decompilation)
+        func_args = AngrBSController.func_args_as_bs_args(decompilation)
         func_type = decompilation.cfunc.functy.returnty.c_repr()
-        bs_args = {
-            i: binsync.FunctionArgument(i, var_info[0].name, var_info[1], var_info[0].size)
-            for i, var_info in func_args.items()
-        }
-
         self.controller.schedule_job(
             self.controller.push_artifact,
-            FunctionHeader(func.name, func.addr, type_=func_type, args=bs_args)
+            FunctionHeader(func.name, func.addr, type_=func_type, args=func_args)
         )
         return False
 
     # pylint: disable=unused-argument
     def handle_func_arg_retyped(self, func, offset, old_type, new_type):
         decompilation = self.controller.decompile_function(func)
-        func_args = AngrBinSyncController.get_func_args(decompilation)
+        func_args = AngrBSController.func_args_as_bs_args(decompilation)
         func_type = decompilation.cfunc.functy.returnty.c_repr()
-        bs_args = {
-            i: binsync.FunctionArgument(i, var_info[0].name, var_info[1], var_info[0].size)
-            for i, var_info in func_args.items()
-        }
-
         self.controller.schedule_job(
             self.controller.push_artifact,
-            FunctionHeader(func.name, func.addr, type_=func_type, args=bs_args)
+            FunctionHeader(func.name, func.addr, type_=func_type, args=func_args)
         )
         return False
 
     # pylint: disable=unused-argument,no-self-use
     def handle_global_var_renamed(self, address, old_name, new_name):
         return False
 
@@ -174,13 +164,13 @@
 
     # pylint: disable=unused-argument,no-self-use
     def handle_function_retyped(self, func, old_type, new_type):
         return False
 
     # pylint: disable=unused-argument
     def handle_comment_changed(self, address, old_cmt, new_cmt, created: bool, decomp: bool):
-        func_addr = self.controller.get_func_addr_from_addr(address)
+        func_addr = self.controller.get_closest_function(address)
         self.controller.schedule_job(
             self.controller.push_artifact,
             Comment(address, new_cmt, func_addr=func_addr, decompiled=decomp)
         )
         return False
```

### Comparing `binsync-3.6.0/binsync/decompilers/binja/artifact_lifter.py` & `binsync-3.9.0/binsync/decompilers/binja/artifact_lifter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from binsync.common import ArtifactLifter
+from binsync.api import BSArtifactLifter
 
 
-class BinjaArtifactLifter(ArtifactLifter):
+class BinjaArtifactLifter(BSArtifactLifter):
     lift_map = {
         "int64_t": "long",
         "uint64_t": "unsigned long",
         "int32_t": "int",
         "uint32_t": "unsigned int",
         "int16_t": "short",
         "uint16_t": "unsigned short",
```

### Comparing `binsync-3.6.0/binsync/decompilers/binja/binja_binsync.py` & `binsync-3.9.0/binsync/decompilers/binja/binja_binsync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-import threading
 import re
 
 from PySide6.QtWidgets import QVBoxLayout
 from PySide6.QtCore import Qt
 from binaryninjaui import (
     UIContext,
     DockHandler,
     DockContextHandler,
     UIAction,
     UIActionHandler,
     Menu,
 )
 import binaryninja
 from binaryninja.types import StructureType, EnumerationType
-from binaryninja import PluginCommand, BinaryView, SymbolType
+from binaryninja import SymbolType
 from binaryninja.interaction import show_message_box
-from binaryninja.enums import MessageBoxButtonSet, MessageBoxIcon, VariableSourceType
 from binaryninja.binaryview import BinaryDataNotification
 
 from collections import defaultdict
 import logging
 
-from binsync.common.ui.version import set_ui_version
+from binsync.ui.version import set_ui_version
 set_ui_version("PySide6")
-from binsync.common.ui.config_dialog import ConfigureBSDialog
-from binsync.common.ui.control_panel import ControlPanel
+from binsync.ui.config_dialog import ConfigureBSDialog
+from binsync.ui.control_panel import ControlPanel
 from .compat import bn_enum_to_bs, find_main_window, BinjaDockWidget, create_widget, bn_struct_to_bs, bn_func_to_bs
-from .controller import BinjaBinSyncController
+from .controller import BinjaBSController
 from binsync.data import (
-    State, User, Artifact,
-    Function, FunctionHeader, FunctionArgument, StackVariable,
-    Comment, GlobalVariable, Patch,
-    Enum, Struct, StructMember
+    Artifact,
+    Function, FunctionHeader, FunctionArgument, Comment, GlobalVariable, Enum, StructMember
 )
 
 l = logging.getLogger(__name__)
 
 #
 # Binja UI
 #
@@ -179,15 +175,15 @@
     notification = DataMonitor(view, controller)
     view.register_notification(notification)
 
 
 class BinjaPlugin:
     def __init__(self):
         # controller stored by a binary view
-        self.controllers = defaultdict(BinjaBinSyncController)
+        self.controllers = defaultdict(BinjaBSController)
         self._init_ui()
 
     def _init_ui(self):
         # config dialog
         configure_binsync_id = "BinSync: Configure..."
         UIAction.registerAction(configure_binsync_id)
         UIActionHandler.globalActions().bindAction(
```

### Comparing `binsync-3.6.0/binsync/decompilers/binja/compat.py` & `binsync-3.9.0/binsync/decompilers/binja/compat.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/decompilers/binja/controller.py` & `binsync-3.9.0/binsync/decompilers/binja/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,34 @@
 # runnable actions that are queued from inside the hooks.py file.
 # Essentially, every change that happens in IDA from the main user triggers
 # a hook which will push an action to be preformed onto the command queue;
 # Causing a "git push" on every change.
 #
 # ----------------------------------------------------------------------------
 
-import re
 import threading
 import functools
-from typing import Dict, List, Tuple, Optional, Iterable, Any
+from typing import Dict, Tuple, Optional, Iterable, Any
 import hashlib
 import logging
 
 from binaryninja import SymbolType
 from binaryninjaui import (
     UIContext,
-    DockHandler,
     DockContextHandler,
-    UIAction,
     UIActionHandler,
     Menu,
 )
 import binaryninja
-from binaryninja.enums import MessageBoxButtonSet, MessageBoxIcon, VariableSourceType
-from binaryninja.mainthread import execute_on_main_thread, is_main_thread
+from binaryninja.enums import VariableSourceType
 from binaryninja.types import StructureType, EnumerationType
 
-from binsync.common.controller import BinSyncController, fill_event, init_checker
+from binsync.api.controller import BSController, fill_event, init_checker
 from binsync.data import (
-    State, User, Artifact,
-    Function, FunctionHeader, FunctionArgument, StackVariable,
+    State, Function, FunctionHeader, StackVariable,
     Comment, GlobalVariable, Patch,
     Enum, Struct
 )
 import binsync
 
 from .artifact_lifter import BinjaArtifactLifter
 from .compat import bn_enum_to_bs, bn_func_to_bs, bn_struct_to_bs
@@ -75,18 +70,18 @@
     return wrapper
 
 
 #
 # Controller
 #
 
-class BinjaBinSyncController(BinSyncController):
-    def __init__(self):
-        super(BinjaBinSyncController, self).__init__(artifact_lifter=BinjaArtifactLifter(self))
-        self.bv: binaryninja.BinaryView = None
+class BinjaBSController(BSController):
+    def __init__(self, bv=None):
+        super(BinjaBSController, self).__init__(artifact_lifter=BinjaArtifactLifter(self))
+        self.bv: binaryninja.BinaryView = bv
 
     def binary_hash(self) -> str:
         hash_ = ""
         try:
             hash_ = hashlib.md5(self.bv.file.raw[:]).hexdigest()
         except Exception:
             pass
@@ -128,15 +123,14 @@
     def goto_address(self, func_addr) -> None:
         self.bv.offset = func_addr
 
     #
     # Fillers
     #
 
-    @init_checker
     @fill_event
     def fill_struct(self, struct_name, header=True, members=True, artifact=None, **kwargs):
         bs_struct: Struct = artifact
         if not bs_struct:
             l.warning(f"Unable to find the struct: {struct_name} in requested user.")
             return False
 
@@ -160,15 +154,14 @@
 
                     members.append((bn_type, bs_memb.name))
 
                 s.members = members
 
         return True
 
-    @init_checker
     @fill_event
     def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
         changed = False
         bs_global_var: GlobalVariable = artifact
         bn_global_var: binaryninja.DataVariable = self.bv.get_data_var_at(var_addr)
         global_type = self.bv.parse_type_string(bs_global_var.type)
         
@@ -179,31 +172,29 @@
         
             if bn_global_var.name != bs_global_var.name or bn_global_var.type != global_type:
                 bn_global_var = self.bv.define_user_data_var(bs_global_var.addr, global_type, bs_global_var.name)
                 changed = True
 
         return changed
 
-    @init_checker
     @background_and_wait
     @fill_event
     def fill_function(self, func_addr, user=None, artifact=None, **kwargs):
         """
         Grab all relevant information from the specified user and fill the @bn_func.
         """
         bs_func: Function = artifact
         bn_func = self.bv.get_function_at(bs_func.addr)
 
-        changes = super(BinjaBinSyncController, self).fill_function(
+        changes = super(BinjaBSController, self).fill_function(
             func_addr, user=user, artifact=artifact, bn_func=bn_func, **kwargs
         )
         bn_func.reanalyze()
         return changes
 
-    @init_checker
     @fill_event
     def fill_function_header(self, func_addr, user=None, artifact=None, bn_func=None, **kwargs):
         updates = False
         bs_func_header: FunctionHeader = artifact
 
         if bs_func_header:
             # func name
@@ -251,15 +242,14 @@
 
                 if valid_type:
                     bn_func.type = bn_prototype
                     updates |= True
 
         return updates
 
-    @init_checker
     @fill_event
     def fill_stack_variable(self, func_addr, offset, user=None, artifact=None, bn_func=None, **kwargs):
         updates = False
         bs_stack_var: StackVariable = artifact
 
         existing_stack_vars: Dict[int, Any] = {
             v.storage: v for v in bn_func.stack_layout
@@ -287,24 +277,22 @@
                 except Exception as e:
                     l.warning(f"BinSync could not sync stack variable at offset {bn_offset}: {e}")
 
                 updates |= True
 
         return updates
 
-    @init_checker
     @fill_event
     def fill_comment(self, addr, user=None, artifact=None, bn_func=None, **kwargs):
         # TODO: check if the comment changed when set!
         comment: Comment = artifact
         bn_func.set_comment_at(comment.addr, comment.comment)
 
         return True
     
-    @init_checker
     @fill_event
     def fill_enum(self, name, user=None, artifact=None, ida_code_view=None, **kwargs):
         bs_enum: Enum = artifact
         bn_enum: binaryninja.EnumerationType = self.bv.types.get(name)
         
         bn_members = []
         
@@ -381,7 +369,14 @@
         except KeyError:
             return None 
             
         gvar = GlobalVariable(
             addr, self.bv.get_symbol_at(addr) or f"data_{addr:x}", type_=str(var.type) if var.type is not None else None, size=var.type.width
         )
         return gvar
+
+    def _decompile(self, function: Function) -> Optional[str]:
+        funcs = self.bv.get_functions_containing(function.addr)
+        if not funcs:
+            return None
+        func = funcs[0]
+        return str(func.hlil)
```

### Comparing `binsync-3.6.0/binsync/decompilers/ghidra/server/artifact_lifter.py` & `binsync-3.9.0/binsync/decompilers/ghidra/server/artifact_lifter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
-from binsync.common import ArtifactLifter
+from binsync.api import BSArtifactLifter
 
 l = logging.getLogger(name=__name__)
 
 
-class GhidraArtifactLifter(ArtifactLifter):
+class GhidraArtifactLifter(BSArtifactLifter):
     lift_map = {}
 
     def __init__(self, controller):
         super(GhidraArtifactLifter, self).__init__(controller)
 
     def lift_addr(self, addr: int) -> int:
         #return self.controller.rebase_addr(addr)
```

### Comparing `binsync-3.6.0/binsync/decompilers/ghidra/server/control_panel_window.py` & `binsync-3.9.0/binsync/decompilers/ghidra/server/control_panel_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 
-from binsync.common.ui.qt_objects import QVBoxLayout, QMainWindow, QApplication
-from binsync.common.ui.control_panel import ControlPanel
-from binsync.common.ui.config_dialog import ConfigureBSDialog
+from binsync.ui.qt_objects import QVBoxLayout, QMainWindow, QApplication
+from binsync.ui.control_panel import ControlPanel
+from binsync.ui.config_dialog import ConfigureBSDialog
 
-from .controller import GhidraBinSyncController
+from .controller import GhidraBSController
 
 
 l = logging.getLogger(__name__)
 
 
 class ControlPanelWindow(QMainWindow):
     """
@@ -18,15 +18,15 @@
     """
 
     def __init__(self):
         super(ControlPanelWindow, self).__init__()
         self.setWindowTitle("BinSync")
         self.width_hint = 300
 
-        self.controller: GhidraBinSyncController = GhidraBinSyncController()
+        self.controller: GhidraBSController = GhidraBSController()
         self.control_panel = ControlPanel(self.controller)
 
         self._init_widgets()
 
     #
     # Private methods
     #
```

### Comparing `binsync-3.6.0/binsync/decompilers/ghidra/server/controller.py` & `binsync-3.9.0/binsync/decompilers/ghidra/server/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional
 import logging
 
-from binsync.common.controller import BinSyncController, init_checker, fill_event
+from binsync.api.controller import BSController, init_checker, fill_event
 from binsync.data import (
     Function, FunctionHeader, StackVariable, Comment
 )
 
 from .ghidra_client import BSGhidraClient
 from .artifact_lifter import GhidraArtifactLifter
 
 l = logging.getLogger(__name__)
 
 
-class GhidraBinSyncController(BinSyncController):
+class GhidraBSController(BSController):
     def __init__(self):
-        super(GhidraBinSyncController, self).__init__(GhidraArtifactLifter(self))
+        super(GhidraBSController, self).__init__(GhidraArtifactLifter(self))
         self.ghidra = BSGhidraClient()
         self.base_addr = None
 
     def binary_hash(self) -> str:
         return self.ghidra.binary_hash
 
     def active_context(self):
@@ -40,14 +40,17 @@
             return addr + self.base_addr
         elif addr > self.base_addr:
             return addr - self.base_addr
 
     def goto_address(self, func_addr) -> None:
         self.ghidra.goto_address(func_addr)
 
+    def _decompile(self, function: Function) -> Optional[str]:
+        return self.ghidra.decompile(function.addr)
+
     #
     # Ghidra Specific
     #
 
     def connect_ghidra_client(self):
         return self.ghidra.connect()
 
@@ -90,10 +93,17 @@
         if comment.comment:
             update |= self.ghidra.set_comment(comment.addr, comment.comment, comment.decompiled)
 
         return update
 
     @init_checker
     def magic_fill(self, preference_user=None):
-        super(GhidraBinSyncController, self).magic_fill(
+        super(GhidraBSController, self).magic_fill(
             preference_user=preference_user, target_artifacts={Function: self.fill_function}
         )
+
+    #
+    # Artifact API
+    #
+
+    def _decompile(self, function: Function) -> Optional[str]:
+        return None
```

### Comparing `binsync-3.6.0/binsync/decompilers/ghidra/server/ghidra_client.py` & `binsync-3.9.0/binsync/decompilers/ghidra/server/ghidra_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,18 @@
     def binary_path(self) -> Optional[str]:
         return self.server.binaryPath()
 
     @stringify_args
     def goto_address(self, addr) -> bool:
         return self.server.gotoAddress(addr)
 
+    @stringify_args
+    def decomiple(self, addr) -> str:
+        return self.server.decompile(addr)
+
     #
     # Function Operations
     #
 
     @stringify_args
     def set_func_name(self, addr: int, name: str) -> bool:
         return self.server.setFunctionName(addr, name)
```

### Comparing `binsync-3.6.0/binsync/decompilers/ida/artifact_lifter.py` & `binsync-3.9.0/binsync/decompilers/ida/artifact_lifter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 
-from binsync.common import ArtifactLifter
+from binsync.api import BSArtifactLifter
 
 from . import compat
 
 l = logging.getLogger(name=__name__)
 
 
-class IDAArtifactLifter(ArtifactLifter):
+class IDAArtifactLifter(BSArtifactLifter):
     lift_map = {
         "__int64": "long",
         "__int32": "int",
         "__int16": "short",
         "__int8": "char",
     }
```

### Comparing `binsync-3.6.0/binsync/decompilers/ida/compat.py` & `binsync-3.9.0/binsync/decompilers/ida/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import idc, idaapi, ida_kernwin, ida_hexrays, ida_funcs, \
     ida_bytes, ida_struct, ida_idaapi, ida_typeinf, idautils, ida_enum
 
 import binsync
 from binsync.data import (
     Struct, FunctionHeader, FunctionArgument, StackVariable, Function, GlobalVariable, Enum
 )
-from .controller import IDABinSyncController
+from .controller import IDABSController
 
 l = logging.getLogger(__name__)
 
 #
 # Wrappers for IDA Main thread r/w operations
 # a special note about these functions:
 # Any operation that needs to do some type of write to the ida db (idb), needs to be in the main thread due to
@@ -63,14 +63,17 @@
 
 #
 #   Data Type Converters
 #
 
 @execute_write
 def convert_type_str_to_ida_type(type_str) -> typing.Optional['ida_typeinf']:
+    if type_str is None or not isinstance(type_str, str):
+        return None
+
     ida_type_str = type_str + ";"
     tif = ida_typeinf.tinfo_t()
     valid_parse = ida_typeinf.parse_decl(tif, None, ida_type_str, 1)
 
     return tif if valid_parse is not None else None
 
 
@@ -407,15 +410,15 @@
             ida_offset, name, type_str, size, func_addr
         )
 
     return stack_var_info
 
 
 @execute_write
-def set_stack_vars_types(var_type_dict, code_view, controller: "IDABinSyncController") -> bool:
+def set_stack_vars_types(var_type_dict, code_view, controller: "IDABSController") -> bool:
     """
     Sets the type of a stack variable, which should be a local variable.
     Take special note of the types of first two parameters used here:
     var_type_dict is a dictionary of the offsets and the new proposed type info for each offset.
     This typeinfo should be gotten either by manully making a new typeinfo object or using the
     parse_decl function. code_view is a _instance of vdui_t, which should be gotten through
     open_pseudocode() from ida_hexrays.
```

### Comparing `binsync-3.6.0/binsync/decompilers/ida/controller.py` & `binsync-3.9.0/binsync/decompilers/ida/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 
 import idc
 import idaapi
 import ida_struct
 import ida_hexrays
 
 import binsync
-from binsync.common.controller import BinSyncController, init_checker, fill_event
+from binsync.api.controller import BSController, init_checker, fill_event
 from binsync.data import (
     StackVariable, Function, FunctionHeader, Struct, Comment, GlobalVariable, Enum
 )
 from . import compat
 from .artifact_lifter import IDAArtifactLifter
 
 _l = logging.getLogger(name=__name__)
 
 
 def update_on_view(f):
     wraps(f)
-    def _update_on_view(self: IDABinSyncController, func_addr, *args, **kwargs):
+    def _update_on_view(self: IDABSController, func_addr, *args, **kwargs):
         # always execute something we are looking at
         active_ctx = self.active_context()
         if active_ctx and active_ctx.addr == func_addr:
             return f(self, func_addr, *args, **kwargs)
 
         # otherwise, execute next time we look at it through the hooks
         task = UpdateTask(f, self, func_addr, *args, **kwargs)
@@ -120,17 +120,17 @@
                     del self.update_tasks[update_task]
 
 
 #
 #   Controller
 #
 
-class IDABinSyncController(BinSyncController):
+class IDABSController(BSController):
     def __init__(self):
-        super(IDABinSyncController, self).__init__(artifact_lifter=IDAArtifactLifter(self))
+        super(IDABSController, self).__init__(artifact_lifter=IDAArtifactLifter(self))
 
         # view change callback
         self._updated_ctx = None
         self._decompiler_available = None
         self._crashing_version = False
 
         # update state for only updating when needed
@@ -175,15 +175,14 @@
 
         return self._decompiler_available
 
     #
     # IDA DataBase Fillers
     #
 
-    @init_checker
     @fill_event
     def fill_struct(self, struct_name, user=None, header=True, members=True, artifact=None, **kwargs):
         data_changed = False
         struct: Struct = artifact
         
         if not struct:
             _l.warning(f"Unable to find the struct: {struct_name} in requested user.")
@@ -197,58 +196,54 @@
             data_changed |= compat.set_ida_struct(struct)
 
         if members:
             data_changed |= compat.set_ida_struct_member_types(struct)
 
         return data_changed
 
-    @init_checker
     @fill_event
     def fill_global_var(self, var_addr, user=None, artifact=None, **kwargs):
         changed = False
         global_var: GlobalVariable = artifact
         if global_var and global_var.name:
             changed = compat.set_global_var_name(var_addr, global_var.name)
 
         if changed:
             ctx = self.active_context()
             if ctx:
                 compat.refresh_pseudocode_view(ctx.addr)
 
         return changed
 
-    @init_checker
     @fill_event
     def fill_function(self, func_addr, user=None, artifact=None, **kwargs):
         func: Function = artifact
         try:
             ida_code_view = compat.acquire_pseudocode_vdui(func.addr)
         except Exception:
             ida_code_view = None
 
-        changes = super(IDABinSyncController, self).fill_function(
+        changes = super(IDABSController, self).fill_function(
             func_addr, user=user, artifact=artifact, ida_code_view=ida_code_view, **kwargs
         )
         if ida_code_view is not None and changes:
             ida_code_view.cfunc.refresh_func_ctext()
 
         return changes
 
-    @init_checker
     @fill_event
     def fill_comment(self, addr, user=None, artifact=None, **kwargs):
         cmt: Comment = artifact
         _l.debug(f"Filling comment {cmt} now...")
         res = compat.set_ida_comment(addr, cmt.comment, decompiled=cmt.decompiled)
         if not res:
             _l.warning(f"Failed to sync comment at <{hex(addr)}>: \'{cmt.comment}\'")
 
         return res
 
-    @init_checker
     @fill_event
     def fill_stack_variable(self, func_addr, offset, user=None, artifact=None, ida_code_view=None, **kwargs):
         if ida_code_view is None:
             return False
 
         stack_var: StackVariable = artifact
         _l.debug(f"Filling stack var {stack_var} now...")
@@ -265,27 +260,25 @@
         if ida_type is None:
             _l.warning(f"IDA Failed to parse type for stack var {stack_var}")
             return changes
 
         changes |= compat.set_stack_vars_types({offset: ida_type}, ida_code_view, self)
         return changes
 
-    @init_checker
     @fill_event
     def fill_function_header(self, func_addr, user=None, artifact=None, ida_code_view=None, **kwargs):
         func_header: FunctionHeader = artifact
         _l.debug(f"Filling header {func_header} now...")
         if ida_code_view is None:
             compat.set_ida_func_name(func_addr, func_header.name)
             return False
 
         updated_header = compat.set_function_header(ida_code_view, func_header)
         return updated_header
 
-    @init_checker
     @fill_event
     def fill_enum(self, name, user=None, artifact=None, ida_code_view=None, **kwargs):
         enum: Enum = artifact
         updated_enum = compat.set_enum(enum)
         return updated_enum
 
     #
@@ -311,7 +304,15 @@
         return compat.struct(name)
 
     def enums(self) -> Dict[str, Enum]:
         return compat.enums()
 
     def enum(self, name) -> Optional[Enum]:
         return compat.enum(name)
+
+    def _decompile(self, function: Function) -> Optional[str]:
+        try:
+            cfunc = ida_hexrays.decompile(function.addr)
+        except Exception:
+            return None
+
+        return str(cfunc)
```

### Comparing `binsync-3.6.0/binsync/decompilers/ida/hooks.py` & `binsync-3.9.0/binsync/decompilers/ida/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import ida_enum
 import idaapi
 import idc
 
 from PyQt5 import QtCore
 
 from . import compat
-from .controller import IDABinSyncController
+from .controller import IDABSController
 from binsync.data import (
     FunctionHeader, FunctionArgument, StackVariable,
     Comment, GlobalVariable, Enum, Struct
 )
 from PyQt5.QtGui import QKeyEvent
 
 l = logging.getLogger(__name__)
@@ -75,15 +75,15 @@
 #   IDA Change Hooks
 #
 
 
 class IDBHooks(ida_idp.IDB_Hooks):
     def __init__(self, controller):
         ida_idp.IDB_Hooks.__init__(self)
-        self.controller: IDABinSyncController = controller
+        self.controller: IDABSController = controller
         self.last_local_type = None
 
     @quite_init_checker
     @stop_if_syncing
     def local_types_changed(self):
         #print("local type changed")
         return 0
@@ -510,15 +510,15 @@
 class FakeIDACodeView:
     def __init__(self, cfunc):
         self.cfunc = cfunc
 
 
 class HexRaysHooks:
     def __init__(self, controller):
-        self.controller: IDABinSyncController = controller
+        self.controller: IDABSController = controller
         super(HexRaysHooks, self).__init__()
         self._available = None
         self._installed = False
         self._cached_funcs = {}
         self.updating_states = threading.Lock()
 
     def hook(self):
```

### Comparing `binsync-3.6.0/binsync/decompilers/ida/oneliner.py` & `binsync-3.9.0/binsync/decompilers/ida/oneliner.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/decompilers/ida/plugin.py` & `binsync-3.9.0/binsync/decompilers/ida/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 import ida_kernwin
 import idc
 import ida_hexrays
 import idautils
 from PyQt5.QtWidgets import QWidget, QVBoxLayout
 from PyQt5.QtCore import Qt
 
-from binsync.common.ui.version import set_ui_version
+from binsync.ui.version import set_ui_version
 set_ui_version("PyQt5")
-from binsync.common.ui.config_dialog import ConfigureBSDialog
-from binsync.common.ui.control_panel import ControlPanel
+from binsync.ui.config_dialog import ConfigureBSDialog
+from binsync.ui.control_panel import ControlPanel
 from binsync import __version__ as VERSION
 
 from .hooks import MasterHook, IdaHotkeyHook
-from .controller import IDABinSyncController
+from .controller import IDABSController
 from . import compat
 
 l = logging.getLogger(__name__)
-controller = IDABinSyncController()
+controller = IDABSController()
 
 # disable the annoying "Running Python script" wait box that freezes IDA at times
 idaapi.set_script_timeout(0)
 
 
 #
 #   UI Hook, placed here for convenience of reading UI implementation
```

### Comparing `binsync-3.6.0/binsync/installer.py` & `binsync-3.9.0/binsync/installer.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync/loggercfg.py` & `binsync-3.9.0/binsync/loggercfg.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/binsync.egg-info/SOURCES.txt` & `binsync-3.9.0/binsync.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,36 +9,18 @@
 binsync/loggercfg.py
 binsync.egg-info/PKG-INFO
 binsync.egg-info/SOURCES.txt
 binsync.egg-info/dependency_links.txt
 binsync.egg-info/entry_points.txt
 binsync.egg-info/requires.txt
 binsync.egg-info/top_level.txt
-binsync/common/__init__.py
-binsync/common/artifact_lifter.py
-binsync/common/controller.py
-binsync/common/ui/__init__.py
-binsync/common/ui/config_dialog.py
-binsync/common/ui/control_panel.py
-binsync/common/ui/magic_sync_dialog.py
-binsync/common/ui/qt_objects.py
-binsync/common/ui/utils.py
-binsync/common/ui/version.py
-binsync/common/ui/force_push/__init__.py
-binsync/common/ui/force_push/force_push.py
-binsync/common/ui/force_push/panels/__init__.py
-binsync/common/ui/force_push/panels/functions_table.py
-binsync/common/ui/force_push/panels/global_panel.py
-binsync/common/ui/panel_tabs/__init__.py
-binsync/common/ui/panel_tabs/activity_table.py
-binsync/common/ui/panel_tabs/ctx_table.py
-binsync/common/ui/panel_tabs/functions_table.py
-binsync/common/ui/panel_tabs/globals_table.py
-binsync/common/ui/panel_tabs/table_model.py
-binsync/common/ui/panel_tabs/util_panel.py
+binsync/api/__init__.py
+binsync/api/artifact_lifter.py
+binsync/api/controller.py
+binsync/api/type_parser.py
 binsync/core/__init__.py
 binsync/core/cache.py
 binsync/core/client.py
 binsync/core/errors.py
 binsync/core/scheduler.py
 binsync/data/__init__.py
 binsync/data/artifact.py
@@ -47,16 +29,20 @@
 binsync/data/enum.py
 binsync/data/func.py
 binsync/data/global_variable.py
 binsync/data/patch.py
 binsync/data/stack_variable.py
 binsync/data/state.py
 binsync/data/struct.py
-binsync/data/type_parser.py
 binsync/data/user.py
+binsync/decompiler_stubs/__init__.py
+binsync/decompiler_stubs/ghidra_binsync.py
+binsync/decompiler_stubs/ida_binsync.py
+binsync/decompiler_stubs/angr_binsync/__init__.py
+binsync/decompiler_stubs/binja_binsync/__init__.py
 binsync/decompilers/__init__.py
 binsync/decompilers/angr/__init__.py
 binsync/decompilers/angr/artifact_lifter.py
 binsync/decompilers/angr/control_panel_view.py
 binsync/decompilers/angr/controller.py
 binsync/decompilers/angr/plugin.py
 binsync/decompilers/binja/__init__.py
@@ -73,16 +59,33 @@
 binsync/decompilers/ida/__init__.py
 binsync/decompilers/ida/artifact_lifter.py
 binsync/decompilers/ida/compat.py
 binsync/decompilers/ida/controller.py
 binsync/decompilers/ida/hooks.py
 binsync/decompilers/ida/oneliner.py
 binsync/decompilers/ida/plugin.py
-decompiler_stubs/ghidra_binsync.py
-decompiler_stubs/ida_binsync.py
-decompiler_stubs/angr_binsync/__init__.py
-decompiler_stubs/angr_binsync/plugin.toml
-decompiler_stubs/binja_binsync/__init__.py
-decompiler_stubs/binja_binsync/plugin.json
+binsync/extras/__init__.py
+binsync/extras/ai/__init__.py
+binsync/extras/ai/ai_user_config.py
+binsync/extras/ai/openai_bs_user.py
+binsync/ui/__init__.py
+binsync/ui/config_dialog.py
+binsync/ui/control_panel.py
+binsync/ui/magic_sync_dialog.py
+binsync/ui/qt_objects.py
+binsync/ui/utils.py
+binsync/ui/version.py
+binsync/ui/force_push/__init__.py
+binsync/ui/force_push/force_push.py
+binsync/ui/force_push/panels/__init__.py
+binsync/ui/force_push/panels/functions_table.py
+binsync/ui/force_push/panels/global_panel.py
+binsync/ui/panel_tabs/__init__.py
+binsync/ui/panel_tabs/activity_table.py
+binsync/ui/panel_tabs/ctx_table.py
+binsync/ui/panel_tabs/functions_table.py
+binsync/ui/panel_tabs/globals_table.py
+binsync/ui/panel_tabs/table_model.py
+binsync/ui/panel_tabs/util_panel.py
 tests/test_angr_gui.py
 tests/test_client.py
 tests/test_state.py
```

### Comparing `binsync-3.6.0/tests/test_angr_gui.py` & `binsync-3.9.0/tests/test_angr_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 import tempfile
 
 import time
 import logging
 from datetime import datetime as datetime_, timedelta
 
 from PySide6 import QtWidgets
-from PySide6.QtCore import Qt, QPoint
 from PySide6.QtGui import QContextMenuEvent
-from PySide6.QtTest import QTest
-from PySide6.QtCore import Qt, QPoint, QTimer
+from PySide6.QtCore import Qt, QPoint
 from PySide6.QtWidgets import QApplication, QMenu
 from angrmanagement.ui.views import CodeView, DisassemblyView
 from pytestqt.qtbot import QtBot
 import pytest
 
 import angr
 from angrmanagement.ui.dialogs.rename_node import RenameNode
 from angrmanagement.ui.main_window import MainWindow
 
-from binsync.common.ui.version import set_ui_version
+from binsync.ui.version import set_ui_version
 set_ui_version("PySide6")
-from binsync.common.controller import SyncControlStatus
-from binsync.common.ui.config_dialog import ConfigureBSDialog
+from binsync.api.controller import SyncControlStatus
+from binsync.ui.config_dialog import ConfigureBSDialog
 
 
 test_location = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'binaries')
 logging.disable(logging.CRITICAL)
 
 BINSYNC_RELOAD_TIME = 10000
```

### Comparing `binsync-3.6.0/tests/test_client.py` & `binsync-3.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `binsync-3.6.0/tests/test_state.py` & `binsync-3.9.0/tests/test_state.py`

 * *Files identical despite different names*

