# Comparing `tmp/funcs-0.2.1.tar.gz` & `tmp/funcs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.2.1.tar", max compression
+gzip compressed data, was "funcs-0.2.2.tar", max compression
```

## Comparing `funcs-0.2.1.tar` & `funcs-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1092 2023-04-12 12:31:10.156600 funcs-0.2.1/LICENSE
--rw-r--r--   0        0        0     2872 2023-04-12 12:31:10.156600 funcs-0.2.1/README.md
--rw-r--r--   0        0        0     1664 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/application.py
--rw-r--r--   0        0        0      563 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/callers.py
--rw-r--r--   0        0        0     4121 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/composition.py
--rw-r--r--   0        0        0      300 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/debug.py
--rw-r--r--   0        0        0      166 2023-04-12 12:31:10.156600 funcs-0.2.1/funcs/decorators.py
--rw-r--r--   0        0        0     3595 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/flow.py
--rw-r--r--   0        0        0      899 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/getters.py
--rw-r--r--   0        0        0      264 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/py.typed
--rw-r--r--   0        0        0      492 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/reduction.py
--rw-r--r--   0        0        0      475 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/types.py
--rw-r--r--   0        0        0     2627 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/typing.py
--rw-r--r--   0        0        0     1369 2023-04-12 12:31:10.160600 funcs-0.2.1/funcs/unpacking.py
--rw-r--r--   0        0        0     3022 2023-04-12 12:31:10.160600 funcs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-17 13:12:16.876319 funcs-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2872 2023-04-17 13:12:16.876319 funcs-0.2.2/README.md
+-rw-r--r--   0        0        0     1664 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/application.py
+-rw-r--r--   0        0        0      563 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/callers.py
+-rw-r--r--   0        0        0     4121 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/composition.py
+-rw-r--r--   0        0        0      431 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/debug.py
+-rw-r--r--   0        0        0      166 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/decorators.py
+-rw-r--r--   0        0        0     3595 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/flow.py
+-rw-r--r--   0        0        0      899 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/getters.py
+-rw-r--r--   0        0        0      264 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/py.typed
+-rw-r--r--   0        0        0      492 2023-04-17 13:12:16.876319 funcs-0.2.2/funcs/reduction.py
+-rw-r--r--   0        0        0      475 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/types.py
+-rw-r--r--   0        0        0     2878 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/typing.py
+-rw-r--r--   0        0        0     1369 2023-04-17 13:12:16.880319 funcs-0.2.2/funcs/unpacking.py
+-rw-r--r--   0        0        0     3022 2023-04-17 13:12:16.880319 funcs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 funcs-0.2.2/PKG-INFO
```

### Comparing `funcs-0.2.1/LICENSE` & `funcs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/README.md` & `funcs-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.1"
+funcs = "^0.2.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.2.1/funcs/__init__.py` & `funcs-0.2.2/funcs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
```

### Comparing `funcs-0.2.1/funcs/application.py` & `funcs-0.2.2/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/funcs/callers.py` & `funcs-0.2.2/funcs/callers.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/funcs/composition.py` & `funcs-0.2.2/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/funcs/flow.py` & `funcs-0.2.2/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/funcs/functions.py` & `funcs-0.2.2/funcs/functions.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/funcs/typing.py` & `funcs-0.2.2/funcs/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,33 @@
     "DynamicCallable",
     "AnyCallable",
     "Nullary",
     "Unary",
     "Binary",
     "Ternary",
     "Quaternary",
+    "Identity",
+    "Inspect",
     "Predicate",
+    "Decorator",
+    "DecoratorIdentity",
     "GenericPredicate",
     "UnpackNullary",
     "UnpackUnary",
     "UnpackBinary",
     "UnpackTernary",
     "UnpackQuaternary",
+    "AsyncCallable",
     "AsyncNullary",
     "AsyncUnary",
     "AsyncBinary",
     "AsyncTernary",
     "AsyncQuaternary",
+    "AsyncIdentity",
+    "AsyncInspect",
     "AsyncPredicate",
     "AsyncGenericPredicate",
     "is_instance",
     "is_subclass",
     "is_none",
     "is_not_none",
 )
@@ -79,18 +86,22 @@
 
 Nullary = Callable[[], R]
 Unary = Callable[[T], R]
 Binary = Callable[[T, U], R]
 Ternary = Callable[[T, U, V], R]
 Quaternary = Callable[[T, U, V, W], R]
 
+Identity = Unary[T, T]
+
+Inspect = Unary[T, None]
+
 Predicate = Unary[T, bool]
 
 Decorator = Unary[F, G]
-DecoratorIdentity = Decorator[F, F]
+DecoratorIdentity = Identity[F]
 
 GenericPredicate = Callable[P, bool]
 
 UnpackNullary = Unary[EmptyTuple, R]
 UnpackUnary = Unary[Tuple[T], R]
 UnpackBinary = Unary[Tuple[T, U], R]
 UnpackTernary = Unary[Tuple[T, U, V], R]
@@ -100,14 +111,18 @@
 
 AsyncNullary = Nullary[Awaitable[R]]
 AsyncUnary = Unary[T, Awaitable[R]]
 AsyncBinary = Binary[T, U, Awaitable[R]]
 AsyncTernary = Ternary[T, U, V, Awaitable[R]]
 AsyncQuaternary = Quaternary[T, U, V, W, Awaitable[R]]
 
+AsyncIdentity = AsyncUnary[T, T]
+
+AsyncInspect = AsyncUnary[T, None]
+
 AsyncPredicate = AsyncUnary[T, bool]
 
 AsyncGenericPredicate = AsyncCallable[P, bool]
 
 
 def is_none(item: Optional[Any]) -> TypeGuard[None]:
     return item is None
```

### Comparing `funcs-0.2.1/funcs/unpacking.py` & `funcs-0.2.2/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.2.1/pyproject.toml` & `funcs-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.2.1"
+version = "0.2.2"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -126,15 +126,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.2.1"
+version = "0.2.2"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.2.1/PKG-INFO` & `funcs-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -70,15 +70,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.2.1"
+funcs = "^0.2.2"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

