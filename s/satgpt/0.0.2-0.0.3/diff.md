# Comparing `tmp/satgpt-0.0.2.tar.gz` & `tmp/satgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satgpt-0.0.2.tar", last modified: Sun Apr 16 19:27:30 2023, max compression
+gzip compressed data, was "satgpt-0.0.3.tar", last modified: Mon Apr 17 00:57:26 2023, max compression
```

## Comparing `satgpt-0.0.2.tar` & `satgpt-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:27:30.693822 satgpt-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 19:27:30.693822 satgpt-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 19:27:19.000000 satgpt-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-16 19:27:19.000000 satgpt-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-16 19:27:30.693822 satgpt-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-16 19:27:19.000000 satgpt-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:27:30.689821 satgpt-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:27:30.693822 satgpt-0.0.2/src/satgpt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-16 19:27:19.000000 satgpt-0.0.2/src/satgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-16 19:27:19.000000 satgpt-0.0.2/src/satgpt/module_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 19:27:19.000000 satgpt-0.0.2/src/satgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:27:30.693822 satgpt-0.0.2/src/satgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 19:27:30.000000 satgpt-0.0.2/src/satgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-16 19:27:30.000000 satgpt-0.0.2/src/satgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:27:30.000000 satgpt-0.0.2/src/satgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 19:27:30.000000 satgpt-0.0.2/src/satgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:27:30.693822 satgpt-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-16 19:27:19.000000 satgpt-0.0.2/tests/test_module_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 00:57:17.000000 satgpt-0.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 00:57:26.874331 satgpt-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 00:57:17.000000 satgpt-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 00:57:17.000000 satgpt-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 00:57:26.874331 satgpt-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-17 00:57:17.000000 satgpt-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.870331 satgpt-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/src/satgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/module_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/src/satgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-17 00:57:17.000000 satgpt-0.0.3/tests/test_module_demo.py
```

