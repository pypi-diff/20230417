# Comparing `tmp/receptorctl-1.3.0.dev2.tar.gz` & `tmp/receptorctl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptorctl-1.3.0.dev2.tar", last modified: Thu Oct 13 17:08:52 2022, max compression
+gzip compressed data, was "receptorctl-1.3.1.tar", last modified: Mon Apr 17 17:29:47 2023, max compression
```

## Comparing `receptorctl-1.3.0.dev2.tar` & `receptorctl-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:08:52.396526 receptorctl-1.3.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 17:08:28.000000 receptorctl-1.3.0.dev2/.VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-13 17:08:52.396526 receptorctl-1.3.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:08:52.396526 receptorctl-1.3.0.dev2/receptorctl/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/receptorctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/receptorctl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18198 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/receptorctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9768 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/receptorctl/socket_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 17:08:52.396526 receptorctl-1.3.0.dev2/receptorctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 17:08:52.000000 receptorctl-1.3.0.dev2/receptorctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-13 17:08:52.396526 receptorctl-1.3.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-10-13 17:08:13.000000 receptorctl-1.3.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:29:47.425623 receptorctl-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:29:33.000000 receptorctl-1.3.1/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 17:29:26.000000 receptorctl-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 17:29:47.425623 receptorctl-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 17:29:26.000000 receptorctl-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-17 17:29:26.000000 receptorctl-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:29:47.425623 receptorctl-1.3.1/receptorctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 17:29:26.000000 receptorctl-1.3.1/receptorctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 17:29:26.000000 receptorctl-1.3.1/receptorctl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-04-17 17:29:26.000000 receptorctl-1.3.1/receptorctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-17 17:29:26.000000 receptorctl-1.3.1/receptorctl/socket_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:29:47.425623 receptorctl-1.3.1/receptorctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:29:47.000000 receptorctl-1.3.1/receptorctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 17:29:47.429623 receptorctl-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 17:29:26.000000 receptorctl-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:29:47.425623 receptorctl-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-17 17:29:26.000000 receptorctl-1.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-17 17:29:26.000000 receptorctl-1.3.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 17:29:26.000000 receptorctl-1.3.1/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-17 17:29:26.000000 receptorctl-1.3.1/tests/test_workunit.py
```

### Comparing `receptorctl-1.3.0.dev2/receptorctl/cli.py` & `receptorctl-1.3.1/receptorctl/cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.3.0.dev2/receptorctl/socket_interface.py` & `receptorctl-1.3.1/receptorctl/socket_interface.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.3.0.dev2/setup.cfg` & `receptorctl-1.3.1/setup.cfg`

 * *Files identical despite different names*

