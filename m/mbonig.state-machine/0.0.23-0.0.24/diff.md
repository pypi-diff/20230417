# Comparing `tmp/mbonig.state-machine-0.0.23.tar.gz` & `tmp/mbonig.state-machine-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbonig.state-machine-0.0.23.tar", last modified: Mon Apr 17 13:48:10 2023, max compression
+gzip compressed data, was "mbonig.state-machine-0.0.24.tar", last modified: Mon Apr 17 14:32:30 2023, max compression
```

## Comparing `mbonig.state-machine-0.0.23.tar` & `mbonig.state-machine-0.0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.684103 mbonig.state-machine-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:48:10.684103 mbonig.state-machine-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/state_machine/
--rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   203418 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/_jsii/state-machine@0.0.23.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:47:57.000000 mbonig.state-machine-0.0.23/src/mbonig/state_machine/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:48:10.680103 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:48:10.000000 mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.485350 mbonig.state-machine-0.0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.485350 mbonig.state-machine-0.0.24/src/mbonig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/src/mbonig/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/src/mbonig/state_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/src/mbonig/state_machine/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/src/mbonig/state_machine/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199094 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/src/mbonig/state_machine/_jsii/state-machine@0.0.24.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:32:16.000000 mbonig.state-machine-0.0.24/src/mbonig/state_machine/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:32:30.489350 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-17 14:32:29.000000 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 14:32:30.000000 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:32:29.000000 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 14:32:30.000000 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 14:32:30.000000 mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/top_level.txt
```

### Comparing `mbonig.state-machine-0.0.23/LICENSE` & `mbonig.state-machine-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `mbonig.state-machine-0.0.23/PKG-INFO` & `mbonig.state-machine-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.state-machine
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Step Function state machine construct focused on working well with the Workflow Studio
 Home-page: https://github.com/mbonig/state-machine.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/mbonig/state-machine.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mbonig.state-machine-0.0.23/README.md` & `mbonig.state-machine-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `mbonig.state-machine-0.0.23/setup.py` & `mbonig.state-machine-0.0.24/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mbonig.state-machine",
-    "version": "0.0.23",
+    "version": "0.0.24",
     "description": "A Step Function state machine construct focused on working well with the Workflow Studio",
     "license": "Apache-2.0",
     "url": "https://github.com/mbonig/state-machine.git",
     "long_description_content_type": "text/markdown",
     "author": "Matthew Bonig<matthew.bonig@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "mbonig.state_machine",
         "mbonig.state_machine._jsii"
     ],
     "package_data": {
         "mbonig.state_machine._jsii": [
-            "state-machine@0.0.23.jsii.tgz"
+            "state-machine@0.0.24.jsii.tgz"
         ],
         "mbonig.state_machine": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `mbonig.state-machine-0.0.23/src/mbonig/state_machine/__init__.py` & `mbonig.state-machine-0.0.24/src/mbonig/state_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `mbonig.state-machine-0.0.23/src/mbonig.state_machine.egg-info/PKG-INFO` & `mbonig.state-machine-0.0.24/src/mbonig.state_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbonig.state-machine
-Version: 0.0.23
+Version: 0.0.24
 Summary: A Step Function state machine construct focused on working well with the Workflow Studio
 Home-page: https://github.com/mbonig/state-machine.git
 Author: Matthew Bonig<matthew.bonig@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/mbonig/state-machine.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

