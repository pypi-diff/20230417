# Comparing `tmp/i2-0.0.98.tar.gz` & `tmp/i2-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2-0.0.98.tar", last modified: Tue Apr  5 21:04:05 2022, max compression
+gzip compressed data, was "i2-0.0.99.tar", last modified: Wed Apr  6 00:38:10 2022, max compression
```

## Comparing `i2-0.0.98.tar` & `i2-0.0.99.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.782151 i2-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-05 21:03:33.000000 i2-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-04-05 21:04:05.782151 i2-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-04-05 21:03:33.000000 i2-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.778151 i2-0.0.98/i2/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-04-05 21:03:33.000000 i2-0.0.98/i2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6998 2022-04-05 21:03:33.000000 i2-0.0.98/i2/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)    16178 2022-04-05 21:03:33.000000 i2-0.0.98/i2/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-04-05 21:03:33.000000 i2-0.0.98/i2/chain_map.py
--rw-r--r--   0 runner    (1001) docker     (121)    47729 2022-04-05 21:03:33.000000 i2-0.0.98/i2/deco.py
--rw-r--r--   0 runner    (1001) docker     (121)     7926 2022-04-05 21:03:33.000000 i2-0.0.98/i2/doc_mint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-04-05 21:03:33.000000 i2-0.0.98/i2/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.778151 i2-0.0.98/i2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-05 21:03:33.000000 i2-0.0.98/i2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-04-05 21:03:33.000000 i2-0.0.98/i2/examples/signature_calculus.py
--rw-r--r--   0 runner    (1001) docker     (121)    10088 2022-04-05 21:03:33.000000 i2-0.0.98/i2/footprints.py
--rw-r--r--   0 runner    (1001) docker     (121)     9541 2022-04-05 21:03:33.000000 i2-0.0.98/i2/io_trans.py
--rw-r--r--   0 runner    (1001) docker     (121)     6085 2022-04-05 21:03:33.000000 i2-0.0.98/i2/itypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    20818 2022-04-05 21:03:33.000000 i2-0.0.98/i2/key_path.py
--rw-r--r--   0 runner    (1001) docker     (121)    24414 2022-04-05 21:03:33.000000 i2-0.0.98/i2/multi_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    12320 2022-04-05 21:03:33.000000 i2-0.0.98/i2/routing_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.778151 i2-0.0.98/i2/scrap/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-05 21:03:33.000000 i2-0.0.98/i2/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-04-05 21:03:33.000000 i2-0.0.98/i2/scrap/scrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-04-05 21:03:33.000000 i2-0.0.98/i2/scrap/simple_pymint.py
--rw-r--r--   0 runner    (1001) docker     (121)   130972 2022-04-05 21:03:33.000000 i2-0.0.98/i2/signatures.py
--rw-r--r--   0 runner    (1001) docker     (121)     8944 2022-04-05 21:03:33.000000 i2-0.0.98/i2/switch_case_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.782151 i2-0.0.98/i2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/footprints_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/objects_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    19362 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/signatures_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    15322 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-04-05 21:03:33.000000 i2-0.0.98/i2/tests/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    21667 2022-04-05 21:03:33.000000 i2-0.0.98/i2/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    64709 2022-04-05 21:04:04.000000 i2-0.0.98/i2/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 21:04:05.778151 i2-0.0.98/i2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-04-05 21:04:05.000000 i2-0.0.98/i2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-04-05 21:04:05.000000 i2-0.0.98/i2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 21:04:05.000000 i2-0.0.98/i2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 21:04:05.000000 i2-0.0.98/i2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-04-05 21:04:05.000000 i2-0.0.98/i2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-04-05 21:04:05.782151 i2-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-05 21:03:33.000000 i2-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-06 00:37:43.000000 i2-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-04-06 00:38:10.446031 i2-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-04-06 00:37:43.000000 i2-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/i2/
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-04-06 00:37:43.000000 i2-0.0.99/i2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6998 2022-04-06 00:37:43.000000 i2-0.0.99/i2/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16178 2022-04-06 00:37:43.000000 i2-0.0.99/i2/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7340 2022-04-06 00:37:43.000000 i2-0.0.99/i2/chain_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47729 2022-04-06 00:37:43.000000 i2-0.0.99/i2/deco.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7926 2022-04-06 00:37:43.000000 i2-0.0.99/i2/doc_mint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6098 2022-04-06 00:37:43.000000 i2-0.0.99/i2/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/i2/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-06 00:37:43.000000 i2-0.0.99/i2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-04-06 00:37:43.000000 i2-0.0.99/i2/examples/signature_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10088 2022-04-06 00:37:43.000000 i2-0.0.99/i2/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9541 2022-04-06 00:37:43.000000 i2-0.0.99/i2/io_trans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6085 2022-04-06 00:37:43.000000 i2-0.0.99/i2/itypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20818 2022-04-06 00:37:43.000000 i2-0.0.99/i2/key_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24414 2022-04-06 00:37:43.000000 i2-0.0.99/i2/multi_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12320 2022-04-06 00:37:43.000000 i2-0.0.99/i2/routing_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/i2/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-06 00:37:43.000000 i2-0.0.99/i2/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-04-06 00:37:43.000000 i2-0.0.99/i2/scrap/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-04-06 00:37:43.000000 i2-0.0.99/i2/scrap/simple_pymint.py
+-rw-r--r--   0 runner    (1001) docker     (121)   130972 2022-04-06 00:37:43.000000 i2-0.0.99/i2/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8944 2022-04-06 00:37:43.000000 i2-0.0.99/i2/switch_case_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/i2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/footprints_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/objects_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19362 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/signatures_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15322 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-04-06 00:37:43.000000 i2-0.0.99/i2/tests/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21667 2022-04-06 00:37:43.000000 i2-0.0.99/i2/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66196 2022-04-06 00:38:09.000000 i2-0.0.99/i2/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 00:38:10.446031 i2-0.0.99/i2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-04-06 00:38:10.000000 i2-0.0.99/i2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-04-06 00:38:10.000000 i2-0.0.99/i2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 00:38:10.000000 i2-0.0.99/i2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 00:38:10.000000 i2-0.0.99/i2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-04-06 00:38:10.000000 i2-0.0.99/i2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-04-06 00:38:10.446031 i2-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-06 00:37:43.000000 i2-0.0.99/setup.py
```

### Comparing `i2-0.0.98/LICENSE` & `i2-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/PKG-INFO` & `i2-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2
-Version: 0.0.98
+Version: 0.0.99
 Summary:  Creating manipulating and applying mint (Meta-INTerface)
 Home-page: https://github.com/i2mint/i2
 Author: Otosense
 License: Apache Software License
 Description: # i2
         
         Core tools for minting code.
```

### Comparing `i2-0.0.98/README.md` & `i2-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/__init__.py` & `i2-0.0.99/i2/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,8 +27,19 @@
 )
 
 from i2.errors import (
     InterruptWithBlock,
     HandleExceptions,
 )
 
-from i2.wrapper import wrap, Wrap, Wrapx, Ingress, include_exclude, rm_params, partialx
+from i2.wrapper import (
+    wrap,
+    Wrap,
+    Wrapx,
+    Ingress,
+    include_exclude,
+    rm_params,
+    partialx,
+    map_names,
+    func_to_method_func,
+    bind_funcs_object_attrs,
+)
```

### Comparing `i2-0.0.98/i2/_deprecated.py` & `i2-0.0.99/i2/_deprecated.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/base.py` & `i2-0.0.99/i2/base.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/chain_map.py` & `i2-0.0.99/i2/chain_map.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/deco.py` & `i2-0.0.99/i2/deco.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/doc_mint.py` & `i2-0.0.99/i2/doc_mint.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/errors.py` & `i2-0.0.99/i2/errors.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/examples/signature_calculus.py` & `i2-0.0.99/i2/examples/signature_calculus.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/footprints.py` & `i2-0.0.99/i2/footprints.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/io_trans.py` & `i2-0.0.99/i2/io_trans.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/itypes.py` & `i2-0.0.99/i2/itypes.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/key_path.py` & `i2-0.0.99/i2/key_path.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/multi_object.py` & `i2-0.0.99/i2/multi_object.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/routing_forest.py` & `i2-0.0.99/i2/routing_forest.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/scrap/scrap.py` & `i2-0.0.99/i2/scrap/scrap.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/scrap/simple_pymint.py` & `i2-0.0.99/i2/scrap/simple_pymint.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/signatures.py` & `i2-0.0.99/i2/signatures.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/switch_case_tree.py` & `i2-0.0.99/i2/switch_case_tree.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/tests/footprints_test.py` & `i2-0.0.99/i2/tests/footprints_test.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/tests/objects_for_testing.py` & `i2-0.0.99/i2/tests/objects_for_testing.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/tests/signatures_test.py` & `i2-0.0.99/i2/tests/signatures_test.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/tests/util.py` & `i2-0.0.99/i2/tests/util.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/tests/wrapper_test.py` & `i2-0.0.99/i2/tests/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/util.py` & `i2-0.0.99/i2/util.py`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/i2/wrapper.py` & `i2-0.0.99/i2/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,17 @@
         """reduce is meant to control how things are pickled/unpickled"""
         return type(self), self._init_args, dict(self._init_kwargs)
 
     def __get__(self, instance, owner):
         """This method allows things to work well when we use Wrap object as method"""
         return MethodType(self, instance)
 
+    # def __set_name__(self, owner, name):
+    #     self.name = owner.__name__
+
     def __repr__(self):
         # TODO: Replace i2.Wrap with dynamic (Wrap or Wrapx)
         name = getattr(self, '__name__', None) or 'Wrap'
         return f'<i2.Wrap {name}{signature(self)}>'
 
 
 class Wrap(_Wrap):
@@ -1222,15 +1225,15 @@
     func,
     instance_params=(),
     *,
     method_name=None,
     method_params=None,
     instance_arg_name='self',
 ) -> MethodFunc:
-    """Get a 'method function' from a 'normal function'.
+    """Get a 'method function' from a 'normal function'. Also known as "methodize".
 
     That is, get a function that gives the same outputs as the 'normal function',
     except that some of the arguments are sourced from the attributes of the first
     argument.
 
     The intended use case is when you want to inject one or several methods in a class
     or instance, sourcing some of the arguments of the underlying function from a
@@ -1256,25 +1259,57 @@
     that ``a`` and ``c`` are not there, but that the two remaining parameters,
     ``b`` and ``d`` are present, in the same order, and with the same annotations and
     parameter kind (the ``d`` is still keyword-only).
 
     Now let's make a dummy object that has attributes ``a`` and a ``c``, and use it to
     call ``method_func``:
 
-    >>> class Klass:
-    ...     a = 1
-    ...     c = 3
-    >>> instance = Klass()
+    >>> from collections import namedtuple
+    >>> instance = namedtuple('FakeInstance', 'a c')(1, 3)
     >>> method_func(instance, 2, d='hello')
     'hello: 9'
 
     Which is:
 
     >>> assert method_func(instance, 2, d='hello') == func(1, 2, c=3, d='hello')
 
+    Often, though, what you'll want is to include this method function directly in
+    a class, as you're making that class "normally". That works too:
+
+    >>> from dataclasses import dataclass
+    >>> @dataclass
+    ... class Klass:
+    ...     a : int = 1
+    ...     c : int = 3
+    ...     method_func = func_to_method_func(func, 'a c')
+    >>> instance = Klass(1, 3)
+    >>> instance.method_func(2, d='hello')
+    'hello: 9'
+
+    What if your function has argument names that don't correspond to the names you
+    have, or want, as attributes of the class? Or even, you have several functions that
+    share an argument name that need to be bound to a different attribute?
+
+    For that, just use ``map_names`` to wrap the function, giving it the names that
+    you need to give it to have the effect you want (the binding of those arguments
+    to attributes of the instance):
+
+    >>> from i2.wrapper import map_names
+    >>> def func(x, y: int, z=2, *, d='bar'):
+    ...     return f"{d}: {(x + y) * z}"
+    >>> from dataclasses import dataclass
+    >>> @dataclass
+    ... class Klass:
+    ...     a : int = 1
+    ...     c : int = 3
+    ...     method_func = func_to_method_func(map_names(func, x='a', z='c'), 'a c')
+    >>> instance = Klass(1, 3)
+    >>> instance.method_func(2, d='hello')
+    'hello: 9'
+
     """
     # get a signature object for func
     sig = Sig(func)
     # if method_name not give, use the function's name
     method_name = method_name or sig.name
     # if params expressed as string, split it into a list of parameter (names)
     if isinstance(instance_params, str):
@@ -1301,26 +1336,28 @@
     )
     # wrap the function, name it and return it
     method_func = wrap(func, ingress=ingress)
     method_func.__name__ = method_name
     return method_func
 
 
-def make_funcs_binding_class(
-    funcs, init_params=(), cls_name=None,
+def bind_funcs_object_attrs(
+    funcs, init_params=(), *, cls=None,
 ):
     """Transform one or several functions into a class that contains them as methods
     sourcing specific arguments from the instance's attributes.
 
     >>> from inspect import signature
+    >>> from dataclasses import dataclass
+    >>>
     >>> def foo(a, b, c=2, *, d='bar'):
     ...     return f"{d}: {(a + b) * c}"
     >>> foo(1, 2)
     'bar: 6'
-    >>> Klass = make_funcs_binding_class(foo, init_params='a c')
+    >>> Klass = bind_funcs_object_attrs(foo, init_params='a c')
     >>> Klass.__name__
     'Foo'
     >>> instance = Klass(a=1, c=3)
     >>> assert instance.foo(2, d='hello') == 'hello: 9' == foo(
     ...     a=1, b=2, c=3, d='hello')
     >>> str(signature(Klass))
     "(a: 'typing.Any', c: 'typing.Any' = 2) -> None"
@@ -1330,79 +1367,85 @@
     'Foo(a=1, c=3)'
     >>> str(signature(instance.foo))
     "(b, *, d='bar')"
     >>> instance.foo(2, d='hello')
     'hello: 9'
     >>> instance.foo(10, d='goodbye')
     'goodbye: 33'
+
+    >>> def foo(a, b, c):
+    ...     return a + b * c
+    ...
+    >>> def bar(d, e):
+    ...     return f"{d=}, {e=}"
+    ...
+    >>> @dataclass
+    ... class K:
+    ...     a: int
+    ...     e: int
+    ...
+    >>> C = bind_funcs_object_attrs([foo, bar], 'a e', cls=K)
+    >>> str(signature(C))
+    '(a: int, e: int) -> None'
+    >>> c = C(1,2)
+    >>> assert str(signature(c.foo)) == '(b, c)'
+    >>> c.foo(3,4)
+    13
+    >>> assert str(signature(c.bar)) == '(d)'
+    >>> c.bar(5)
+    'd=5, e=2'
     """
 
+    if isinstance(init_params, str):
+        init_params = init_params.split()
+
     dflt_cls_name = 'FuncsUnion'
     if callable(funcs) and not isinstance(funcs, Iterable):
         single_func = funcs
         dflt_cls_name = camelize(getattr(single_func, '__name__', dflt_cls_name))
         funcs = [single_func]
 
-    cls_name = cls_name or dflt_cls_name
-    if isinstance(init_params, str):
-        init_params = init_params.split()
+    if not isinstance(cls, type):
+        # if the class is not given, we need to make one
+        if isinstance(cls, str):
+            cls_name = cls
+        else:
+            cls_name = dflt_cls_name
 
-    # init_parameter_objects = Sig(func)[init_params].params
-    class_init_sig = Sig()
-    for func in funcs:
-        class_init_sig = class_init_sig.merge_with_sig(func)[init_params]
-    dataclass_fields = list(map(param_to_dataclass_field_tuple, class_init_sig.params))
-    Klass = make_dataclass(cls_name, dataclass_fields)
+        # init_parameter_objects = Sig(func)[init_params].params
+        # Make the signature for the init
+        class_init_sig = Sig()
+        for func in funcs:
+            class_init_sig = class_init_sig.merge_with_sig(func)[init_params]
+
+        dataclass_fields = list(
+            map(param_to_dataclass_field_tuple, class_init_sig.params)
+        )
+        cls = make_dataclass(cls_name, dataclass_fields)
 
     for func in funcs:
         method_func = func_to_method_func(func, init_params)
-        setattr(Klass, method_func.__name__, method_func)
-    return Klass
+        setattr(cls, method_func.__name__, method_func)
+    return cls
 
 
-#
-# # TODO: Make a type where ``isinstance(s, Identifier) == s.isidentifier()``
-# Identifier = NewType('Identifier', str)  # + should satisfy str.isidentifier
-# Bind = NewType(
-#     'Bind',
-#     Union[
-#         str,  # Identifier or ' '.join(Iterable[Identifier])
-#         Dict[Identifier, Identifier],
-#         Sequence[Union[Identifier, Tuple[Identifier, Identifier]]],
-#     ],
-# )
-# IdentifierMapping = Dict[Identifier, Identifier]
-#
-#
-# def identifier_mapping(x: Bind) -> IdentifierMapping:
-#     """
-#
-#     >>> identifier_mapping('x a_b yz')
-#     {'x': 'x', 'a_b': 'a_b', 'yz': 'yz'}
-#     >>> identifier_mapping(['foo', ('bar', 'mitzvah')])
-#     {'foo': 'foo', 'bar': 'mitzvah'}
-#     >>> identifier_mapping({'x': 'y', 'a': 'b'})
-#     {'x': 'y', 'a': 'b'}
-#     """
-#     if isinstance(x, str):
-#         x = x.split()
-#     if not isinstance(x, Mapping):
-#
-#         def gen():
-#             for item in x:
-#                 if isinstance(item, str):
-#                     yield item, item
-#                 else:
-#                     yield item
-#
-#         return dict(gen())
-#     else:
-#         return dict(**x)
-#
-#
+def _items_filt(d: dict, keys):
+    for k, v in d.items():
+        if k in keys:
+            yield k, v
+
+
+def _mk_sig_from_params_and_funcs(params, funcs):
+    def gen():
+        for param in params:
+            pass
+
+
+## An attempt to redo a func_to_method_func because I forgot func_to_method_func existed
+## Has some different ideas, so keeping around until I decide it's time to let go.
 # NoSuchKey = type('NoSuchKey', (), {})
 # _instance_extractor: KwargsTrans
 #
 # # TODO: Add more (possibly optional) bind validation to fail early.
 # def _instance_extractor(
 #     outer_kwargs, bind: IdentifierMapping = (), instance_param: Identifier = 'self'
 # ):
@@ -1431,15 +1474,15 @@
 #                 # the instance's attribute
 #                 yield inner_param, getattr(instance, outer_val)
 #             else:
 #                 # take the arg name and val as is
 #                 yield outer_param, outer_val
 #
 #     return dict(gen())
-#
+
 #
 # def methodize(func, bind: Bind = ()):
 #     bind = identifier_mapping(bind)
 #     ingress = Ingress(
 #         outer_sig=Sig(func),
 #         kwargs_trans=partial(_instance_extractor, bind=bind),
 #         inner_sig=Sig('self') + Sig(func) - Sig(list(bind)),  # TODO: solve type or lint
```

### Comparing `i2-0.0.98/i2.egg-info/PKG-INFO` & `i2-0.0.99/i2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2
-Version: 0.0.98
+Version: 0.0.99
 Summary:  Creating manipulating and applying mint (Meta-INTerface)
 Home-page: https://github.com/i2mint/i2
 Author: Otosense
 License: Apache Software License
 Description: # i2
         
         Core tools for minting code.
```

### Comparing `i2-0.0.98/i2.egg-info/SOURCES.txt` & `i2-0.0.99/i2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i2-0.0.98/setup.cfg` & `i2-0.0.99/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = i2
-version = 0.0.98
+version = 0.0.99
 url = https://github.com/i2mint/i2
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint
 description = 
 	Creating
 	manipulating
```

