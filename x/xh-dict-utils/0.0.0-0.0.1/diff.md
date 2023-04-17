# Comparing `tmp/xh-dict-utils-0.0.0.tar.gz` & `tmp/xh-dict-utils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dict-utils-0.0.0.tar", last modified: Mon Apr 17 00:48:15 2023, max compression
+gzip compressed data, was "xh-dict-utils-0.0.1.tar", last modified: Mon Apr 17 03:23:01 2023, max compression
```

## Comparing `xh-dict-utils-0.0.0.tar` & `xh-dict-utils-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/
--rw-r--r--   0 xeth      (1000) xeth      (1000)    35821 2023-01-06 15:42:35.000000 xh-dict-utils-0.0.0/LICENSE.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)      647 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      131 2023-04-17 00:37:07.000000 xh-dict-utils-0.0.0/README.md
--rw-r--r--   0 xeth      (1000) xeth      (1000)      618 2023-04-17 00:37:08.000000 xh-dict-utils-0.0.0/pyproject.toml
--rw-r--r--   0 xeth      (1000) xeth      (1000)       38 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/setup.cfg
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/src/
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/src/xh_dict_utils/
--rw-r--r--   0 xeth      (1000) xeth      (1000)    13292 2023-04-16 18:40:24.000000 xh-dict-utils-0.0.0/src/xh_dict_utils/ExtractFromFile.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     2496 2023-04-14 17:21:56.000000 xh-dict-utils-0.0.0/src/xh_dict_utils/Layer1AppEngine.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)       82 2023-04-17 00:46:25.000000 xh-dict-utils-0.0.0/src/xh_dict_utils/__init__.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     7932 2023-04-16 18:56:47.000000 xh-dict-utils-0.0.0/src/xh_dict_utils/dict_utils.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     3421 2023-04-14 13:39:15.000000 xh-dict-utils-0.0.0/src/xh_dict_utils/test_dict_utils.py
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 00:48:15.080500 xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/
--rw-r--r--   0 xeth      (1000) xeth      (1000)      647 2023-04-17 00:48:15.000000 xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      373 2023-04-17 00:48:15.000000 xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/SOURCES.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)        1 2023-04-17 00:48:15.000000 xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/dependency_links.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)       14 2023-04-17 00:48:15.000000 xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/top_level.txt
+drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/
+-rw-r--r--   0 xeth      (1000) xeth      (1000)    35821 2023-01-06 15:42:35.000000 xh-dict-utils-0.0.1/LICENSE.txt
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      695 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/PKG-INFO
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      182 2023-04-17 03:22:34.000000 xh-dict-utils-0.0.1/README.md
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      618 2023-04-17 03:22:34.000000 xh-dict-utils-0.0.1/pyproject.toml
+-rw-r--r--   0 xeth      (1000) xeth      (1000)       38 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/setup.cfg
+drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/src/
+drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/src/xh_dict_utils/
+-rw-r--r--   0 xeth      (1000) xeth      (1000)     1239 2023-04-17 00:54:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/ExtractFromFile.py
+-rw-r--r--   0 xeth      (1000) xeth      (1000)     2496 2023-04-14 17:21:56.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/Layer1AppEngine.py
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      148 2023-04-17 00:54:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/__init__.py
+-rw-r--r--   0 xeth      (1000) xeth      (1000)    12249 2023-04-17 00:54:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/app.py
+-rw-r--r--   0 xeth      (1000) xeth      (1000)     7932 2023-04-16 18:56:47.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/dict_utils.py
+-rw-r--r--   0 xeth      (1000) xeth      (1000)     3421 2023-04-14 13:39:15.000000 xh-dict-utils-0.0.1/src/xh_dict_utils/test_dict_utils.py
+drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-17 03:23:01.768840 xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      695 2023-04-17 03:23:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/PKG-INFO
+-rw-r--r--   0 xeth      (1000) xeth      (1000)      398 2023-04-17 03:23:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 xeth      (1000) xeth      (1000)        1 2023-04-17 03:23:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 xeth      (1000) xeth      (1000)       14 2023-04-17 03:23:01.000000 xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/top_level.txt
```

### Comparing `xh-dict-utils-0.0.0/LICENSE.txt` & `xh-dict-utils-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.0/PKG-INFO` & `xh-dict-utils-0.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.0
+Version: 0.0.1
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,9 +14,10 @@
 
 A dictionary utility of self dev py library
 
 ## Build
 ```shell
 rm -fr dist
 python -m build
+# automate by `-u {user} -p {token / password}`
 python -m twine upload dist/*
 ```
```

### Comparing `xh-dict-utils-0.0.0/pyproject.toml` & `xh-dict-utils-0.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xh-dict-utils"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="xethhung", email="pypi@xethh.dev" },
 ]
 description = "A dictionary utility of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `xh-dict-utils-0.0.0/src/xh_dict_utils/ExtractFromFile.py` & `xh-dict-utils-0.0.1/src/xh_dict_utils/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,64 +1,17 @@
 import argparse
-import json
-import os.path
-import re
+import os
 import sys
-from enum import Enum
-from pathlib import Path
-from typing import Generator
-
 import yaml
-
+import json
 from Layer1AppEngine import AppEngine, CommandTemplate
-from dict_utils import Selector, Entries
-
-
-class SupportedFormat(Enum):
-    JSON = "json"
-    YAML = "yaml"
-
-
-def getKey(args):
-    targetFile = Path(args.file)
-
-    if not targetFile.exists():
-        raise Exception(f'Path[{targetFile}] not exists')
-
-
-def readFromFile(filePath):
-    with open(filePath, "r") as f:
-        while True:
-            line = f.readline()
-            if line:
-                yield line
-            else:
-                break
-
-
-def traverseNode(root, nodeNotation, do=lambda parent, nodeName: (parent, nodeName)):
-    if root == None:
-        raise Exception("Node input is empty")
-
-    if nodeNotation and (not nodeNotation == ""):
-        levels = nodeNotation.split(".")
-        nodeName = levels[-1]
-
-        parent = root
-        for x in levels[:-1]:
-            if not x in parent:
-                parent[x] = dict()
-            parent = parent[x]
-
-        return True, do(parent, nodeName)
-    else:
-        return False, None, None
-
+from ExtractFromFile import SupportedFormat
+from dict_utils import Entries, Selector
 
-if __name__ == "__main__":
+def main():
     PROGRAM_NAME = "yaml-json-modification"
     DESCRIPTION = "A simple program modify yaml or json file"
     appEngine = AppEngine(
         program_name=PROGRAM_NAME,
         description=DESCRIPTION,
     )
```

### Comparing `xh-dict-utils-0.0.0/src/xh_dict_utils/Layer1AppEngine.py` & `xh-dict-utils-0.0.1/src/xh_dict_utils/Layer1AppEngine.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.0/src/xh_dict_utils/dict_utils.py` & `xh-dict-utils-0.0.1/src/xh_dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.0/src/xh_dict_utils/test_dict_utils.py` & `xh-dict-utils-0.0.1/src/xh_dict_utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.0/src/xh_dict_utils.egg-info/PKG-INFO` & `xh-dict-utils-0.0.1/src/xh_dict_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.0
+Version: 0.0.1
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,9 +14,10 @@
 
 A dictionary utility of self dev py library
 
 ## Build
 ```shell
 rm -fr dist
 python -m build
+# automate by `-u {user} -p {token / password}`
 python -m twine upload dist/*
 ```
```

