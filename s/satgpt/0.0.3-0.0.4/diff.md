# Comparing `tmp/satgpt-0.0.3.tar.gz` & `tmp/satgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satgpt-0.0.3.tar", last modified: Mon Apr 17 00:57:26 2023, max compression
+gzip compressed data, was "satgpt-0.0.4.tar", last modified: Mon Apr 17 01:31:55 2023, max compression
```

## Comparing `satgpt-0.0.3.tar` & `satgpt-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 00:57:17.000000 satgpt-0.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 00:57:26.874331 satgpt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 00:57:17.000000 satgpt-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 00:57:17.000000 satgpt-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 00:57:26.874331 satgpt-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-17 00:57:17.000000 satgpt-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.870331 satgpt-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/src/satgpt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/module_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 00:57:17.000000 satgpt-0.0.3/src/satgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/src/satgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 00:57:26.000000 satgpt-0.0.3/src/satgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:57:26.874331 satgpt-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-17 00:57:17.000000 satgpt-0.0.3/tests/test_module_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:31:55.916071 satgpt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 01:31:46.000000 satgpt-0.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-17 01:31:55.916071 satgpt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-17 01:31:46.000000 satgpt-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 01:31:46.000000 satgpt-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 01:31:55.916071 satgpt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 01:31:46.000000 satgpt-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:31:55.912071 satgpt-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:31:55.916071 satgpt-0.0.4/src/satgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 01:31:46.000000 satgpt-0.0.4/src/satgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-17 01:31:46.000000 satgpt-0.0.4/src/satgpt/make_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-17 01:31:46.000000 satgpt-0.0.4/src/satgpt/module_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 01:31:46.000000 satgpt-0.0.4/src/satgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:31:55.916071 satgpt-0.0.4/src/satgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-17 01:31:55.000000 satgpt-0.0.4/src/satgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-17 01:31:55.000000 satgpt-0.0.4/src/satgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 01:31:55.000000 satgpt-0.0.4/src/satgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 01:31:55.000000 satgpt-0.0.4/src/satgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 01:31:55.000000 satgpt-0.0.4/src/satgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:31:55.916071 satgpt-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-17 01:31:46.000000 satgpt-0.0.4/tests/test_module_demo.py
```

### Comparing `satgpt-0.0.3/setup.py` & `satgpt-0.0.4/src/satgpt/make_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 import json
 import os
 import platform
 from os import getenv, pathsep
 from os.path import basename
 
-from setuptools import setup
-
 
 # adapted from https://github.com/TheR1D/shell_gpt/blob/main/sgpt/role.py
 def make_satgpt_role():
     from distro import name as distro_name
 
     operating_systems = {
         "Linux": "Linux/" + distro_name(pretty=True),
@@ -54,26 +52,19 @@
         "expecting": "Command",
         "variables": {
             "shell": shell_name,
             "os": os_name,
         },
         "role": SATGPT_ROLE,
     }
-    print(satgpt_json)
+
     file_path = getenv("HOME") + "/.config/shell_gpt/roles/shell.json"
 
     # make directory if it doesn't exist
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     with open(file_path, "w") as f:
         f.write(json.dumps(satgpt_json, indent=4))
 
 
 if __name__ == "__main__":
     # setup for satgpt
-    setup(
-        # install_requires=[
-        #     "shell_gpt",
-        #     "pystac",
-        #     "distro",
-        # ],
-    )
     make_satgpt_role()
```

