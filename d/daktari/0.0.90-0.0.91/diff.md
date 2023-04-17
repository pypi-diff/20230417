# Comparing `tmp/daktari-0.0.90.tar.gz` & `tmp/daktari-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daktari-0.0.90.tar", last modified: Wed Apr  5 14:16:54 2023, max compression
+gzip compressed data, was "daktari-0.0.91.tar", last modified: Mon Apr 17 06:21:47 2023, max compression
```

## Comparing `daktari-0.0.90.tar` & `daktari-0.0.91.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:53.994417 daktari-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-05 14:16:44.000000 daktari-0.0.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-05 14:16:44.000000 daktari-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-05 14:16:53.994417 daktari-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-05 14:16:45.000000 daktari-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:53.990417 daktari-0.0.90/daktari/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 14:16:45.000000 daktari-0.0.90/daktari/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/check_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/check_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:53.994417 daktari-0.0.90/daktari/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/direnv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/flutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/intellij_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/onepassword.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/test_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/test_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/test_yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/checks/yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/os.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/resource_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:53.994417 daktari-0.0.90/daktari/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/resources/daktari-local-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/resources/mock_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/result_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_check_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/test_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-05 14:16:44.000000 daktari-0.0.90/daktari/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:16:53.990417 daktari-0.0.90/daktari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 14:16:53.000000 daktari-0.0.90/daktari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-05 14:16:44.000000 daktari-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-05 14:16:44.000000 daktari-0.0.90/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:16:53.994417 daktari-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-05 14:16:45.000000 daktari-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:47.715998 daktari-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-17 06:21:38.000000 daktari-0.0.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 06:21:38.000000 daktari-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-17 06:21:47.711998 daktari-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-17 06:21:40.000000 daktari-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:47.711998 daktari-0.0.91/daktari/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 06:21:40.000000 daktari-0.0.91/daktari/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/check_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/check_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:47.711998 daktari-0.0.91/daktari/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/flutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/intellij_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/onepassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/test_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/test_yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/checks/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/resource_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:47.711998 daktari-0.0.91/daktari/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/resources/daktari-local-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/resources/mock_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_check_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/test_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 06:21:38.000000 daktari-0.0.91/daktari/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:21:47.711998 daktari-0.0.91/daktari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 06:21:47.000000 daktari-0.0.91/daktari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-17 06:21:38.000000 daktari-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 06:21:38.000000 daktari-0.0.91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:21:47.715998 daktari-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 06:21:40.000000 daktari-0.0.91/setup.py
```

### Comparing `daktari-0.0.90/LICENSE.txt` & `daktari-0.0.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/PKG-INFO` & `daktari-0.0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.90
+Version: 0.0.91
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.90"
+version = "0.0.91"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.90/README.md` & `daktari-0.0.91/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.90"
+version = "0.0.91"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.90/daktari/__main__.py` & `daktari-0.0.91/daktari/__main__.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/check.py` & `daktari-0.0.91/daktari/check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/check_runner.py` & `daktari-0.0.91/daktari/check_runner.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/check_sorter.py` & `daktari-0.0.91/daktari/check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/check_utils.py` & `daktari-0.0.91/daktari/check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/certs.py` & `daktari-0.0.91/daktari/checks/certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/direnv.py` & `daktari-0.0.91/daktari/checks/direnv.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/docker.py` & `daktari-0.0.91/daktari/checks/docker.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/files.py` & `daktari-0.0.91/daktari/checks/files.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/flutter.py` & `daktari-0.0.91/daktari/checks/flutter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/git.py` & `daktari-0.0.91/daktari/checks/git.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/google.py` & `daktari-0.0.91/daktari/checks/google.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/intellij_idea.py` & `daktari-0.0.91/daktari/checks/intellij_idea.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/java.py` & `daktari-0.0.91/daktari/checks/java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/kubernetes.py` & `daktari-0.0.91/daktari/checks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/misc.py` & `daktari-0.0.91/daktari/checks/misc.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/nodejs.py` & `daktari-0.0.91/daktari/checks/nodejs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/onepassword.py` & `daktari-0.0.91/daktari/checks/onepassword.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/python.py` & `daktari-0.0.91/daktari/checks/python.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/ssh.py` & `daktari-0.0.91/daktari/checks/ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/terraform.py` & `daktari-0.0.91/daktari/checks/terraform.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/test_certs.py` & `daktari-0.0.91/daktari/checks/test_certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/test_java.py` & `daktari-0.0.91/daktari/checks/test_java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/test_ssh.py` & `daktari-0.0.91/daktari/checks/test_ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/test_yarn.py` & `daktari-0.0.91/daktari/checks/test_yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/xml.py` & `daktari-0.0.91/daktari/checks/xml.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/checks/yarn.py` & `daktari-0.0.91/daktari/checks/yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/command_utils.py` & `daktari-0.0.91/daktari/command_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/config.py` & `daktari-0.0.91/daktari/config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/file_utils.py` & `daktari-0.0.91/daktari/file_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/options.py` & `daktari-0.0.91/daktari/options.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/os.py` & `daktari-0.0.91/daktari/os.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/result_printer.py` & `daktari-0.0.91/daktari/result_printer.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_check.py` & `daktari-0.0.91/daktari/test_check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_check_factory.py` & `daktari-0.0.91/daktari/test_check_factory.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_check_sorter.py` & `daktari-0.0.91/daktari/test_check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_check_utils.py` & `daktari-0.0.91/daktari/test_check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_config.py` & `daktari-0.0.91/daktari/test_config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/test_version_utils.py` & `daktari-0.0.91/daktari/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari/version_utils.py` & `daktari-0.0.91/daktari/version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/daktari.egg-info/PKG-INFO` & `daktari-0.0.91/daktari.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.90
+Version: 0.0.91
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.90"
+version = "0.0.91"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.90/daktari.egg-info/SOURCES.txt` & `daktari-0.0.91/daktari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.90/requirements.txt` & `daktari-0.0.91/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 semver==3.0.0
 python-hosts==1.0.3
 tabulate==0.9.0
 types-tabulate==0.9.0.2
 PyYAML==6.0
 types-PyYAML==6.0.12.9
 pyobjc-core==9.0.1; sys_platform == 'darwin'
-pyobjc-framework-Cocoa==9.0.1; sys_platform == 'darwin'
+pyobjc-framework-Cocoa==9.1; sys_platform == 'darwin'
 requests-unixsocket==0.3.0
 dpath==2.1.5
 pyOpenSSL==23.1.1
-types-pyOpenSSL==23.1.0.1
+types-pyOpenSSL==23.1.0.2
```

### Comparing `daktari-0.0.90/setup.py` & `daktari-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="daktari",
-    version="0.0.90",
+    version="0.0.91",
     description="Assist in setting up and maintaining developer environments",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Matt Russell",
     author_email="matthew.russell@sonocent.com",
     url="https://github.com/sonocent/daktari",
```

