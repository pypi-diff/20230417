# Comparing `tmp/xh-dict-utils-0.0.3.tar.gz` & `tmp/xh-dict-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dict-utils-0.0.3.tar", last modified: Mon Apr 17 04:28:11 2023, max compression
+gzip compressed data, was "xh-dict-utils-0.0.4.tar", last modified: Mon Apr 17 06:04:16 2023, max compression
```

## Comparing `xh-dict-utils-0.0.3.tar` & `xh-dict-utils-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:28:11.645438 xh-dict-utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 04:28:11.645438 xh-dict-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:28:11.645438 xh-dict-utils-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:28:11.641437 xh-dict-utils-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:28:11.641437 xh-dict-utils-0.0.3/src/xh_dict_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/ExtractFromFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/Layer1AppEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 04:27:57.000000 xh-dict-utils-0.0.3/src/xh_dict_utils/test_dict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:28:11.645438 xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 04:28:11.000000 xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 04:28:11.000000 xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:28:11.000000 xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 04:28:11.000000 xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:04:16.943828 xh-dict-utils-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/xh_dict_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/Layer1AppEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-17 06:04:00.000000 xh-dict-utils-0.0.4/src/xh_dict_utils/test_dict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:04:16.939828 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 06:04:16.000000 xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/top_level.txt
```

### Comparing `xh-dict-utils-0.0.3/LICENSE.txt` & `xh-dict-utils-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.3/PKG-INFO` & `xh-dict-utils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dict-utils-0.0.3/pyproject.toml` & `xh-dict-utils-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xh-dict-utils"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="xethhung", email="pypi@xethh.dev" },
 ]
 description = "A dictionary utility of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils/ExtractFromFile.py` & `xh-dict-utils-0.0.4/src/xh_dict_utils/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils/Layer1AppEngine.py` & `xh-dict-utils-0.0.4/src/xh_dict_utils/Layer1AppEngine.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils/app.py` & `xh-dict-utils-0.0.4/src/xh_dict_utils/app.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils/dict_utils.py` & `xh-dict-utils-0.0.4/src/xh_dict_utils/dict_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def list_group(self, index: int):
         return Selector(f"{index}.[*]") if self.is_root() else Selector(f"{self.selector_str}.{index}.[*]")
 
     def pop(self):
         return self.key_and_parent()[1]
 
-    def dot_chain(self) -> list[str]:
+    def dot_chain(self) -> [str]:
         return [i for i in self.selector_str.split(".") if i != "[*]"]
     def key_and_parent(self):
         splited = self.dot_chain()
         if self.is_root():
             return Selector.root(), None
         elif len(splited) == 1:
             return splited[0], Selector.root()
```

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils/test_dict_utils.py` & `xh-dict-utils-0.0.4/src/xh_dict_utils/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `xh-dict-utils-0.0.3/src/xh_dict_utils.egg-info/PKG-INFO` & `xh-dict-utils-0.0.4/src/xh_dict_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dict-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A dictionary utility of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dict-utils
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dict-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

