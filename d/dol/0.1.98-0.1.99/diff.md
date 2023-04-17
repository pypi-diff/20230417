# Comparing `tmp/dol-0.1.98.tar.gz` & `tmp/dol-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dol-0.1.98.tar", last modified: Mon Jul 25 19:58:09 2022, max compression
+gzip compressed data, was "dol-0.1.99.tar", last modified: Wed Aug  3 03:14:00 2022, max compression
```

## Comparing `dol-0.1.98.tar` & `dol-0.1.99.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:58:09.597993 dol-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-25 19:57:36.000000 dol-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17342 2022-07-25 19:58:09.601993 dol-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14481 2022-07-25 19:57:36.000000 dol-0.1.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:58:09.593993 dol-0.1.98/dol/
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-07-25 19:57:36.000000 dol-0.1.98/dol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18084 2022-07-25 19:57:36.000000 dol-0.1.98/dol/appendable.py
--rw-r--r--   0 runner    (1001) docker     (121)    36972 2022-07-25 19:57:36.000000 dol-0.1.98/dol/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    29666 2022-07-25 19:57:36.000000 dol-0.1.98/dol/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-07-25 19:57:36.000000 dol-0.1.98/dol/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2022-07-25 19:57:36.000000 dol-0.1.98/dol/dig.py
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-07-25 19:57:36.000000 dol-0.1.98/dol/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-07-25 19:57:36.000000 dol-0.1.98/dol/explicit.py
--rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-07-25 19:57:36.000000 dol-0.1.98/dol/filesys.py
--rw-r--r--   0 runner    (1001) docker     (121)     8622 2022-07-25 19:57:36.000000 dol-0.1.98/dol/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    45945 2022-07-25 19:57:36.000000 dol-0.1.98/dol/naming.py
--rw-r--r--   0 runner    (1001) docker     (121)    14995 2022-07-25 19:57:36.000000 dol-0.1.98/dol/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)   142625 2022-07-25 19:57:36.000000 dol-0.1.98/dol/signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)    19249 2022-07-25 19:58:08.000000 dol-0.1.98/dol/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:58:09.597993 dol-0.1.98/dol/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-25 19:57:36.000000 dol-0.1.98/dol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-07-25 19:57:36.000000 dol-0.1.98/dol/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-07-25 19:57:36.000000 dol-0.1.98/dol/tests/pickability_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-25 19:57:36.000000 dol-0.1.98/dol/tests/scrap.py
--rw-r--r--   0 runner    (1001) docker     (121)    13022 2022-07-25 19:57:36.000000 dol-0.1.98/dol/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    99017 2022-07-25 19:57:36.000000 dol-0.1.98/dol/trans.py
--rw-r--r--   0 runner    (1001) docker     (121)    39988 2022-07-25 19:57:36.000000 dol-0.1.98/dol/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    31607 2022-07-25 19:57:36.000000 dol-0.1.98/dol/zipfiledol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:58:09.597993 dol-0.1.98/dol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17342 2022-07-25 19:58:09.000000 dol-0.1.98/dol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-07-25 19:58:09.000000 dol-0.1.98/dol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 19:58:09.000000 dol-0.1.98/dol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 19:58:09.000000 dol-0.1.98/dol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-25 19:58:09.000000 dol-0.1.98/dol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-25 19:58:09.601993 dol-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-07-25 19:57:36.000000 dol-0.1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:00.377401 dol-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-03 03:13:26.000000 dol-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    17342 2022-08-03 03:14:00.377401 dol-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14481 2022-08-03 03:13:26.000000 dol-0.1.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:00.373401 dol-0.1.99/dol/
+-rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-08-03 03:13:26.000000 dol-0.1.99/dol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18581 2022-08-03 03:13:58.000000 dol-0.1.99/dol/appendable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36972 2022-08-03 03:13:26.000000 dol-0.1.99/dol/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29666 2022-08-03 03:13:26.000000 dol-0.1.99/dol/caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-08-03 03:13:26.000000 dol-0.1.99/dol/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6293 2022-08-03 03:13:26.000000 dol-0.1.99/dol/dig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-08-03 03:13:26.000000 dol-0.1.99/dol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-08-03 03:13:26.000000 dol-0.1.99/dol/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-08-03 03:13:26.000000 dol-0.1.99/dol/filesys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8622 2022-08-03 03:13:26.000000 dol-0.1.99/dol/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45945 2022-08-03 03:13:26.000000 dol-0.1.99/dol/naming.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14995 2022-08-03 03:13:26.000000 dol-0.1.99/dol/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)   142625 2022-08-03 03:13:26.000000 dol-0.1.99/dol/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19249 2022-08-03 03:13:26.000000 dol-0.1.99/dol/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:00.377401 dol-0.1.99/dol/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-03 03:13:26.000000 dol-0.1.99/dol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-08-03 03:13:26.000000 dol-0.1.99/dol/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-08-03 03:13:26.000000 dol-0.1.99/dol/tests/pickability_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-03 03:13:26.000000 dol-0.1.99/dol/tests/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13022 2022-08-03 03:13:26.000000 dol-0.1.99/dol/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99017 2022-08-03 03:13:26.000000 dol-0.1.99/dol/trans.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40031 2022-08-03 03:13:26.000000 dol-0.1.99/dol/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31607 2022-08-03 03:13:26.000000 dol-0.1.99/dol/zipfiledol.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-03 03:14:00.373401 dol-0.1.99/dol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17342 2022-08-03 03:14:00.000000 dol-0.1.99/dol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-08-03 03:14:00.000000 dol-0.1.99/dol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:00.000000 dol-0.1.99/dol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-03 03:14:00.000000 dol-0.1.99/dol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-08-03 03:14:00.000000 dol-0.1.99/dol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-08-03 03:14:00.377401 dol-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-03 03:13:26.000000 dol-0.1.99/setup.py
```

### Comparing `dol-0.1.98/LICENSE` & `dol-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/PKG-INFO` & `dol-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dol
-Version: 0.1.98
+Version: 0.1.99
 Summary: Base builtin tools make and transform data object layers (dols).
 Home-page: https://github.com/i2mint/dol
 Author: OtoSense
 Author-email: thorwhalen1@gmail.com
 License: mit
 Description: # dol
```

### Comparing `dol-0.1.98/README.md` & `dol-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/__init__.py` & `dol-0.1.99/dol/__init__.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/appendable.py` & `dol-0.1.99/dol/appendable.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 See add_append_functionality_to_store_cls docs for examples.
 """
 
 import time
 import types
 
 from dol.trans import store_decorator
+from dol.util import exhaust
 
 
 def define_extend_as_seq_of_appends(obj):
     """Inject an extend method in obj that will used append method.
 
     Args:
         obj: Class (type) or instance of an object that has an "append" method.
@@ -299,17 +300,15 @@
             else:
                 return key, val
 
         return item2kv
 
 
 @store_decorator
-def appendable(
-    store_cls=None, *, item2kv,
-):
+def appendable(store_cls=None, *, item2kv, return_keys=False):
     """Makes a new class with append (and consequential extend) methods
 
     Args:
         store_cls: The store class to subclass
         item2kv: The function that produces a (key, val) pair from an item
         new_store_name: The name to give the new class (default will be 'Appendable' + store_cls.__name__)
 
@@ -343,23 +342,39 @@
     Also showing here how you can decorate the instance itself.
 
     >>> item_to_kv = appendable.mk_item2kv_for.fields(['G', 'L'], key_as_tuple=True)
     >>> d = {}
     >>> s = appendable(d, item2kv=item_to_kv)
     >>> s.append({'L': 'let', 'I': 'it', 'G': 'go'}); list(s.items())
     [(('go', 'let'), {'I': 'it'})]
+
+    You can make the "append" and "extend" methods to return the new generated keys by
+    using the "return_keys" flag.
+
+    >>> d = {}
+    >>> s = appendable(d, item2kv=item_to_kv, return_keys=True)
+    >>> s.append({'L': 'let', 'I': 'it', 'G': 'go'})
+    ('go', 'let')
     """
 
     def append(self, item):
         k, v = item2kv(item)
         self[k] = v
+        if return_keys:
+            return k
 
     def extend(self, items):
-        for item in items:
-            self.append(item)
+        def gen_keys():
+            for item in items:
+                yield self.append(item)
+
+        gen = gen_keys()
+        if return_keys:
+            return list(gen)
+        exhaust(gen)
 
     return type(
         'Appendable' + store_cls.__name__,
         (store_cls,),
         {'append': append, 'extend': extend},
     )
```

### Comparing `dol-0.1.98/dol/base.py` & `dol-0.1.99/dol/base.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/caching.py` & `dol-0.1.99/dol/caching.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/core.py` & `dol-0.1.99/dol/core.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/dig.py` & `dol-0.1.99/dol/dig.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/errors.py` & `dol-0.1.99/dol/errors.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/explicit.py` & `dol-0.1.99/dol/explicit.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/filesys.py` & `dol-0.1.99/dol/filesys.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/mixins.py` & `dol-0.1.99/dol/mixins.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/naming.py` & `dol-0.1.99/dol/naming.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/paths.py` & `dol-0.1.99/dol/paths.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/signatures.py` & `dol-0.1.99/dol/signatures.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/sources.py` & `dol-0.1.99/dol/sources.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/tests/base_test.py` & `dol-0.1.99/dol/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/tests/pickability_test.py` & `dol-0.1.99/dol/tests/pickability_test.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/tools.py` & `dol-0.1.99/dol/tools.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/trans.py` & `dol-0.1.99/dol/trans.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol/util.py` & `dol-0.1.99/dol/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """General util objects"""
 import os
 import shutil
 import re
-from collections import namedtuple, defaultdict
+from collections import deque, namedtuple, defaultdict
 from warnings import warn
 from typing import Any, Hashable, Callable, Iterable, Optional, Union
 from functools import update_wrapper as _update_wrapper
 from functools import wraps as _wraps
 from functools import partialmethod, partial, WRAPPER_ASSIGNMENTS
 from types import MethodType
 from inspect import Signature, signature, Parameter
@@ -14,14 +14,16 @@
 
 # monkey patching WRAPPER_ASSIGNMENTS to get "proper" wrapping (adding defaults and kwdefaults
 wrapper_assignments = (*WRAPPER_ASSIGNMENTS, '__defaults__', '__kwdefaults__')
 
 update_wrapper = partial(_update_wrapper, assigned=wrapper_assignments)
 wraps = partial(_wraps, assigned=wrapper_assignments)
 
+exhaust = partial(deque, maxlen=0)
+
 
 class Literal:
     """An object to indicate that the value should be considered literally.
 
     >>> t = Literal(42)
     >>> t.get_val()
     42
```

### Comparing `dol-0.1.98/dol/zipfiledol.py` & `dol-0.1.99/dol/zipfiledol.py`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/dol.egg-info/PKG-INFO` & `dol-0.1.99/dol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dol
-Version: 0.1.98
+Version: 0.1.99
 Summary: Base builtin tools make and transform data object layers (dols).
 Home-page: https://github.com/i2mint/dol
 Author: OtoSense
 Author-email: thorwhalen1@gmail.com
 License: mit
 Description: # dol
```

### Comparing `dol-0.1.98/dol.egg-info/SOURCES.txt` & `dol-0.1.99/dol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dol-0.1.98/setup.cfg` & `dol-0.1.99/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dol
-version = 0.1.98
+version = 0.1.99
 url = https://github.com/i2mint/dol
 platforms = any
 description_file = README.md
 description = Base builtin tools make and transform data object layers (dols).
 root_url = https://github.com/i2mint
 license = mit
 author = OtoSense
```

