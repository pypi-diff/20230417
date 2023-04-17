# Comparing `tmp/fa_purity-1.8.0.tar.gz` & `tmp/fa_purity-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa_purity-1.8.0.tar", max compression
+gzip compressed data, was "fa_purity-1.9.0.tar", max compression
```

## Comparing `fa_purity-1.8.0.tar` & `fa_purity-1.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      585 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/__init__.py
--rw-r--r--   0        0        0     1151 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/_iter_factory.py
--rw-r--r--   0        0        0      373 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/_patch.py
--rw-r--r--   0        0        0      110 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/cmd/__init__.py
--rw-r--r--   0        0        0     1686 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/cmd/core.py
--rw-r--r--   0        0        0      628 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/cmd/transform.py
--rw-r--r--   0        0        0      707 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/flatten.py
--rw-r--r--   0        0        0     1670 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/frozen.py
--rw-r--r--   0        0        0      166 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/__init__.py
--rw-r--r--   0        0        0        0 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/errors/__init__.py
--rw-r--r--   0        0        0      406 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/errors/invalid_type.py
--rw-r--r--   0        0        0     2150 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/factory.py
--rw-r--r--   0        0        0      283 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/primitive/__init__.py
--rw-r--r--   0        0        0      798 2022-03-31 20:29:15.223772 fa_purity-1.8.0/fa_purity/json/primitive/core.py
--rw-r--r--   0        0        0      919 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/primitive/factory.py
--rw-r--r--   0        0        0      981 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/transform.py
--rw-r--r--   0        0        0      107 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/value/__init__.py
--rw-r--r--   0        0        0      491 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/value/core.py
--rw-r--r--   0        0        0     1958 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/value/factory.py
--rw-r--r--   0        0        0     3582 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/json/value/transform.py
--rw-r--r--   0        0        0     1929 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/maybe.py
--rw-r--r--   0        0        0       67 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/pure_iter/__init__.py
--rw-r--r--   0        0        0      390 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/pure_iter/_inner.py
--rw-r--r--   0        0        0     1398 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/pure_iter/core.py
--rw-r--r--   0        0        0     2330 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/pure_iter/factory.py
--rw-r--r--   0        0        0     1236 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/pure_iter/transform.py
--rw-r--r--   0        0        0        0 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/py.typed
--rw-r--r--   0        0        0     2880 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/result.py
--rw-r--r--   0        0        0       63 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/stream/__init__.py
--rw-r--r--   0        0        0     1276 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/stream/core.py
--rw-r--r--   0        0        0      412 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/stream/factory.py
--rw-r--r--   0        0        0     1398 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/stream/transform.py
--rw-r--r--   0        0        0      283 2022-03-31 20:29:15.224772 fa_purity-1.8.0/fa_purity/union.py
--rw-r--r--   0        0        0      102 2022-03-31 20:29:15.225772 fa_purity-1.8.0/fa_purity/utils.py
--rw-r--r--   0        0        0      505 2022-03-31 20:29:15.225772 fa_purity-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      970 2022-03-31 20:29:16.584132 fa_purity-1.8.0/setup.py
--rw-r--r--   0        0        0      739 2022-03-31 20:29:16.584492 fa_purity-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2022-04-07 14:15:45.402444 fa_purity-1.9.0/fa_purity/__init__.py
+-rw-r--r--   0        0        0     1151 2022-04-07 14:15:45.402444 fa_purity-1.9.0/fa_purity/_iter_factory.py
+-rw-r--r--   0        0        0      373 2022-04-07 14:15:45.402444 fa_purity-1.9.0/fa_purity/_patch.py
+-rw-r--r--   0        0        0      110 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/cmd/__init__.py
+-rw-r--r--   0        0        0     1686 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/cmd/core.py
+-rw-r--r--   0        0        0      628 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/cmd/transform.py
+-rw-r--r--   0        0        0      707 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/flatten.py
+-rw-r--r--   0        0        0     1670 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/frozen.py
+-rw-r--r--   0        0        0      166 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/errors/__init__.py
+-rw-r--r--   0        0        0      406 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/errors/invalid_type.py
+-rw-r--r--   0        0        0     2150 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/factory.py
+-rw-r--r--   0        0        0      283 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/primitive/__init__.py
+-rw-r--r--   0        0        0      798 2022-04-07 14:15:45.406444 fa_purity-1.9.0/fa_purity/json/primitive/core.py
+-rw-r--r--   0        0        0      919 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/primitive/factory.py
+-rw-r--r--   0        0        0      981 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/transform.py
+-rw-r--r--   0        0        0      107 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/value/__init__.py
+-rw-r--r--   0        0        0      491 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/value/core.py
+-rw-r--r--   0        0        0     1958 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/value/factory.py
+-rw-r--r--   0        0        0     3582 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/json/value/transform.py
+-rw-r--r--   0        0        0     1929 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/maybe.py
+-rw-r--r--   0        0        0       67 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/pure_iter/__init__.py
+-rw-r--r--   0        0        0      390 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/pure_iter/_inner.py
+-rw-r--r--   0        0        0     1855 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/pure_iter/core.py
+-rw-r--r--   0        0        0     2330 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/pure_iter/factory.py
+-rw-r--r--   0        0        0     1236 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/pure_iter/transform.py
+-rw-r--r--   0        0        0        0 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/py.typed
+-rw-r--r--   0        0        0     2880 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/result.py
+-rw-r--r--   0        0        0       63 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/stream/__init__.py
+-rw-r--r--   0        0        0     1675 2022-04-07 14:15:45.408445 fa_purity-1.9.0/fa_purity/stream/core.py
+-rw-r--r--   0        0        0      412 2022-04-07 14:15:45.410445 fa_purity-1.9.0/fa_purity/stream/factory.py
+-rw-r--r--   0        0        0     1398 2022-04-07 14:15:45.410445 fa_purity-1.9.0/fa_purity/stream/transform.py
+-rw-r--r--   0        0        0      283 2022-04-07 14:15:45.410445 fa_purity-1.9.0/fa_purity/union.py
+-rw-r--r--   0        0        0      102 2022-04-07 14:15:45.410445 fa_purity-1.9.0/fa_purity/utils.py
+-rw-r--r--   0        0        0      505 2022-04-07 14:15:45.410445 fa_purity-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      970 2022-04-07 14:15:46.738448 fa_purity-1.9.0/setup.py
+-rw-r--r--   0        0        0      739 2022-04-07 14:15:46.738998 fa_purity-1.9.0/PKG-INFO
```

### Comparing `fa_purity-1.8.0/fa_purity/__init__.py` & `fa_purity-1.9.0/fa_purity/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Result,
     ResultE,
 )
 from fa_purity.stream import (
     Stream,
 )
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __all__ = [
     "PureIter",
     "Stream",
     "JsonObj",
     "JsonValue",
     "UnfoldedJVal",
     "Cmd",
```

### Comparing `fa_purity-1.8.0/fa_purity/_iter_factory.py` & `fa_purity-1.9.0/fa_purity/_iter_factory.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/cmd/core.py` & `fa_purity-1.9.0/fa_purity/cmd/core.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/cmd/transform.py` & `fa_purity-1.9.0/fa_purity/cmd/transform.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/flatten.py` & `fa_purity-1.9.0/fa_purity/flatten.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/frozen.py` & `fa_purity-1.9.0/fa_purity/frozen.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/factory.py` & `fa_purity-1.9.0/fa_purity/json/factory.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/primitive/core.py` & `fa_purity-1.9.0/fa_purity/json/primitive/core.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/primitive/factory.py` & `fa_purity-1.9.0/fa_purity/json/primitive/factory.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/transform.py` & `fa_purity-1.9.0/fa_purity/json/transform.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/value/factory.py` & `fa_purity-1.9.0/fa_purity/json/value/factory.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/json/value/transform.py` & `fa_purity-1.9.0/fa_purity/json/value/transform.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/maybe.py` & `fa_purity-1.9.0/fa_purity/maybe.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/pure_iter/core.py` & `fa_purity-1.9.0/fa_purity/pure_iter/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from fa_purity.frozen import (
     freeze,
     FrozenList,
 )
 from fa_purity.pure_iter._inner import (
     InnerPureIter,
 )
+import functools
 import more_itertools
 from typing import (
     Callable,
     Generic,
     Iterable,
     Iterator,
     TypeVar,
@@ -30,30 +31,43 @@
 
 def _chunked(items: Iterable[_T], size: int) -> Iterator[FrozenList[_T]]:
     return iter(map(freeze, more_itertools.chunked(items, size)))
 
 
 @dataclass(frozen=True)
 class PureIter(Generic[_T]):
+    # unsafe_unwrap use is safe due to iters equivalence
     _inner: InnerPureIter[_T]
 
     def map(self, function: Callable[[_T], _R]) -> PureIter[_R]:
         draft: InnerPureIter[_R] = InnerPureIter(
             self._inner.new_iter.map(lambda i: iter(map(function, i)))
         )
         return PureIter(draft)
 
+    def reduce(self, function: Callable[[_R, _T], _R], init: _R) -> _R:
+        return unsafe_unwrap(
+            self._inner.new_iter.map(
+                lambda i: functools.reduce(function, i, init)
+            )
+        )
+
+    def filter(self, function: Callable[[_T], bool]) -> PureIter[_T]:
+        draft = InnerPureIter(
+            self._inner.new_iter.map(lambda i: iter(filter(function, i)))
+        )
+        return PureIter(draft)
+
     def chunked(self, size: int) -> PureIter[FrozenList[_T]]:
         draft = InnerPureIter(
             self._inner.new_iter.map(lambda i: _chunked(i, size))
         )
         return PureIter(draft)
 
     def to_list(self) -> FrozenList[_T]:
         return tuple(self)
 
     def transform(self, function: Callable[[PureIter[_T]], _R]) -> _R:
         return function(self)
 
     def __iter__(self) -> Iterator[_T]:
-        # all cmds will result in an equivalent new iterator
         return iter(unsafe_unwrap(self._inner.new_iter))
```

### Comparing `fa_purity-1.8.0/fa_purity/pure_iter/factory.py` & `fa_purity-1.9.0/fa_purity/pure_iter/factory.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/pure_iter/transform.py` & `fa_purity-1.9.0/fa_purity/pure_iter/transform.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/result.py` & `fa_purity-1.9.0/fa_purity/result.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/fa_purity/stream/core.py` & `fa_purity-1.9.0/fa_purity/stream/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 from fa_purity.cmd import (
     Cmd,
 )
 from fa_purity.frozen import (
     FrozenList,
 )
+import functools
 from typing import (
     Callable,
     Generic,
     Iterable,
     TypeVar,
 )
 
@@ -38,14 +39,25 @@
 
     def map(self, function: Callable[[_T], _R]) -> Stream[_R]:
         draft: _Stream[_R] = _Stream(
             self._new_iter.map(lambda i: iter(map(function, i)))
         )
         return Stream(draft)
 
+    def reduce(self, function: Callable[[_R, _T], _R], init: _R) -> Cmd[_R]:
+        return self._new_iter.map(
+            lambda i: functools.reduce(function, i, init)
+        )
+
+    def filter(self, function: Callable[[_T], bool]) -> Stream[_T]:
+        draft = _Stream(
+            self._new_iter.map(lambda i: iter(filter(function, i)))
+        )
+        return Stream(draft)
+
     def chunked(self, size: int) -> Stream[FrozenList[_T]]:
         draft = _Stream(
             self._new_iter.map(lambda i: _iter_factory.chunked(i, size))
         )
         return Stream(draft)
 
     def transform(self, function: Callable[[Stream[_T]], _R]) -> _R:
```

### Comparing `fa_purity-1.8.0/fa_purity/stream/transform.py` & `fa_purity-1.9.0/fa_purity/stream/transform.py`

 * *Files identical despite different names*

### Comparing `fa_purity-1.8.0/setup.py` & `fa_purity-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'simplejson>=3.17.6,<4.0.0',
  'types-Deprecated>=1.2.1,<2.0.0',
  'types-simplejson>=3.17.2,<4.0.0',
  'typing-extensions>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'fa-purity',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Pure functional and typing utilities',
     'long_description': None,
     'author': 'Product Team',
     'author_email': 'development@fluidattacks.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `fa_purity-1.8.0/PKG-INFO` & `fa_purity-1.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-purity
-Version: 1.8.0
+Version: 1.9.0
 Summary: Pure functional and typing utilities
 License: MIT
 Author: Product Team
 Author-email: development@fluidattacks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

