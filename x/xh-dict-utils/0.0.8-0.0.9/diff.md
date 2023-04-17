# Comparing `tmp/xh-dict-utils-0.0.8.tar.gz` & `tmp/xh-dict-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dict-utils-0.0.8.tar", last modified: Mon Apr 17 09:09:45 2023, max compression
+gzip compressed data, was "xh-dict-utils-0.0.9.tar", last modified: Mon Apr 17 09:21:08 2023, max compression
```

## Comparing `xh-dict-utils-0.0.8.tar` & `xh-dict-utils-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/src/xh_dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/ExtractFromFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/Layer1AppEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 09:09:29.000000 xh-dict-utils-0.0.8/src/xh_dict_utils/test_dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:09:45.961836 xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 09:09:45.000000 xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 09:09:45.000000 xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:09:45.000000 xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 09:09:45.000000 xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:21:08.723527 xh-dict-utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 09:21:08.723527 xh-dict-utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:21:08.723527 xh-dict-utils-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:21:08.719527 xh-dict-utils-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:21:08.723527 xh-dict-utils-0.0.9/src/xh_dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/Layer1AppEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 09:20:54.000000 xh-dict-utils-0.0.9/src/xh_dict_utils/test_dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:21:08.723527 xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 09:21:08.000000 xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 09:21:08.000000 xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:21:08.000000 xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 09:21:08.000000 xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/top_level.txt
```

### Comparing `xh-dict-utils-0.0.8/LICENSE.txt` & `xh-dict-utils-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.8/PKG-INFO` & `xh-dict-utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dict-utils-0.0.8/pyproject.toml` & `xh-dict-utils-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-dict-utils"
-version = "0.0.8"
+version = "0.0.9"
 description = "A dictionary utility of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "xethhung"
 email = "pypi@xethh.dev"
```

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils/ExtractFromFile.py` & `xh-dict-utils-0.0.9/src/xh_dict_utils/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils/Layer1AppEngine.py` & `xh-dict-utils-0.0.9/src/xh_dict_utils/Layer1AppEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from abc import ABC, abstractmethod
-from typing import Callable
+from typing import Callable, List
 
 
 class CommandTemplate(ABC):
     def __init__(self, name: str, help: str):
         self.name = name
         self.help = help
 
@@ -37,15 +37,15 @@
         self.description = description
         self.root_parser = parser_setup(self)
         self.subparsers = sub_parser_setup(self)
         self.subCommands = dict()
         self.handlers = dict()
 
     def regSubCommand(self, key: str, help: str, parserOp: Callable[[argparse.ArgumentParser], None],
-                      handle: Callable[[[str]], None]):
+                      handle: Callable[[List[str]], None]):
         if key not in self.subCommands:
             parser = self.subparsers.add_parser(key, help=help)
             parserOp(parser)
             self.subCommands.update({key: parser})
 
             def handling(args):
                 # parsed_args = root_parser.parse_args(args)
```

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils/app.py` & `xh-dict-utils-0.0.9/src/xh_dict_utils/app.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils/dict_utils.py` & `xh-dict-utils-0.0.9/src/xh_dict_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils/test_dict_utils.py` & `xh-dict-utils-0.0.9/src/xh_dict_utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.8/src/xh_dict_utils.egg-info/PKG-INFO` & `xh-dict-utils-0.0.9/src/xh_dict_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

