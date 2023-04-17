# Comparing `tmp/xh-dict-utils-0.0.5.tar.gz` & `tmp/xh-dict-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dict-utils-0.0.5.tar", last modified: Mon Apr 17 08:17:38 2023, max compression
+gzip compressed data, was "xh-dict-utils-0.0.6.tar", last modified: Mon Apr 17 08:33:07 2023, max compression
```

## Comparing `xh-dict-utils-0.0.5.tar` & `xh-dict-utils-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/xh_dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/ExtractFromFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/Layer1AppEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 08:17:27.000000 xh-dict-utils-0.0.5/src/xh_dict_utils/test_dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:17:38.056219 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 08:17:38.000000 xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/src/xh_dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/Layer1AppEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 08:32:54.000000 xh-dict-utils-0.0.6/src/xh_dict_utils/test_dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:33:07.635086 xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 08:33:07.000000 xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 08:33:07.000000 xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:33:07.000000 xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 08:33:07.000000 xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/top_level.txt
```

### Comparing `xh-dict-utils-0.0.5/LICENSE.txt` & `xh-dict-utils-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.5/PKG-INFO` & `xh-dict-utils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dict-utils-0.0.5/pyproject.toml` & `xh-dict-utils-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-dict-utils"
-version = "0.0.5"
+version = "0.0.6"
 description = "A dictionary utility of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "xethhung"
 email = "pypi@xethh.dev"
```

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils/ExtractFromFile.py` & `xh-dict-utils-0.0.6/src/xh_dict_utils/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils/Layer1AppEngine.py` & `xh-dict-utils-0.0.6/src/xh_dict_utils/Layer1AppEngine.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils/app.py` & `xh-dict-utils-0.0.6/src/xh_dict_utils/app.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils/dict_utils.py` & `xh-dict-utils-0.0.6/src/xh_dict_utils/dict_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from dataclasses import dataclass
 from enum import Enum
-from typing import Generator, Callable, Union
+from typing import Generator, Callable, Union, Tuple
 
 
 class EntryType(Enum):
     DICT = 0
     LIST = 1
     LIST_ITEM = 2
     VALUE = 3
@@ -183,15 +183,15 @@
 
     def asList(self) -> Generator[Entry, None, None]:
         yield from self.entries
 
     def size(self):
         return len(self.entries)
 
-    def head_and_tail(self) -> tuple[Entry, "Entries"]:
+    def head_and_tail(self) -> Tuple[Entry, "Entries"]:
         head = self.entries[0] if len(self.entries) > 0 else None
         tail = Entries(self.entries[1:] if len(self.entries) > 1 else [])
         return head, tail
 
     def head(self):
         head, _ = self.head_and_tail()
         return head
```

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils/test_dict_utils.py` & `xh-dict-utils-0.0.6/src/xh_dict_utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.5/src/xh_dict_utils.egg-info/PKG-INFO` & `xh-dict-utils-0.0.6/src/xh_dict_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

