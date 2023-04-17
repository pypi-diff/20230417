# Comparing `tmp/zict-2.2.0.tar.gz` & `tmp/zict-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zict-2.2.0.tar", last modified: Thu Apr 28 14:19:06 2022, max compression
+gzip compressed data, was "zict-3.0.0.tar", last modified: Mon Apr 17 21:39:50 2023, max compression
```

## Comparing `zict-2.2.0.tar` & `zict-3.0.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-04-28 14:19:06.318472 zict-2.2.0/
--rw-r--r--   0 james      (501) staff       (20)     1507 2021-12-03 20:15:47.000000 zict-2.2.0/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      200 2022-04-28 14:06:51.000000 zict-2.2.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)      898 2022-04-28 14:19:06.318620 zict-2.2.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      466 2022-04-28 14:06:51.000000 zict-2.2.0/README.rst
--rw-r--r--   0 james      (501) staff       (20)        9 2021-05-04 19:37:47.000000 zict-2.2.0/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)     1577 2022-04-28 14:19:06.319346 zict-2.2.0/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)       61 2022-04-28 14:06:51.000000 zict-2.2.0/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-04-28 14:19:06.311788 zict-2.2.0/zict/
--rw-r--r--   0 james      (501) staff       (20)      299 2022-04-28 14:13:12.000000 zict-2.2.0/zict/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5309 2022-04-28 14:06:51.000000 zict-2.2.0/zict/buffer.py
--rw-r--r--   0 james      (501) staff       (20)     3464 2022-04-28 14:06:51.000000 zict-2.2.0/zict/cache.py
--rw-r--r--   0 james      (501) staff       (20)     2139 2022-04-28 14:06:51.000000 zict-2.2.0/zict/common.py
--rw-r--r--   0 james      (501) staff       (20)     3267 2022-04-28 14:06:51.000000 zict-2.2.0/zict/file.py
--rw-r--r--   0 james      (501) staff       (20)     2714 2022-04-28 14:06:51.000000 zict-2.2.0/zict/func.py
--rw-r--r--   0 james      (501) staff       (20)     3119 2022-04-28 14:06:51.000000 zict-2.2.0/zict/lmdb.py
--rw-r--r--   0 james      (501) staff       (20)     4765 2022-04-28 14:06:51.000000 zict-2.2.0/zict/lru.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-04-28 14:06:51.000000 zict-2.2.0/zict/py.typed
--rw-r--r--   0 james      (501) staff       (20)     3989 2022-04-28 14:06:51.000000 zict-2.2.0/zict/sieve.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-04-28 14:19:06.318237 zict-2.2.0/zict/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-05-04 19:37:47.000000 zict-2.2.0/zict/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3998 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_buffer.py
--rw-r--r--   0 james      (501) staff       (20)     3073 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_cache.py
--rw-r--r--   0 james      (501) staff       (20)     2508 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_file.py
--rw-r--r--   0 james      (501) staff       (20)     1855 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_func.py
--rw-r--r--   0 james      (501) staff       (20)     1141 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_lmdb.py
--rw-r--r--   0 james      (501) staff       (20)     4309 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_lru.py
--rw-r--r--   0 james      (501) staff       (20)     1739 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_sieve.py
--rw-r--r--   0 james      (501) staff       (20)     1541 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/test_zip.py
--rw-r--r--   0 james      (501) staff       (20)     2964 2022-04-28 14:06:51.000000 zict-2.2.0/zict/tests/utils_test.py
--rw-r--r--   0 james      (501) staff       (20)     2677 2022-04-28 14:06:51.000000 zict-2.2.0/zict/zip.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-04-28 14:19:06.315108 zict-2.2.0/zict.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      898 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      630 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)        9 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        5 2022-04-28 14:19:06.000000 zict-2.2.0/zict.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-17 21:39:50.544210 zict-3.0.0/
+-rw-r--r--   0 james      (501) staff       (20)     1507 2021-12-03 20:15:47.000000 zict-3.0.0/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      200 2022-04-28 14:06:51.000000 zict-3.0.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)      899 2023-04-17 21:39:50.544549 zict-3.0.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      466 2022-04-28 14:06:51.000000 zict-3.0.0/README.rst
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-04-17 21:35:32.000000 zict-3.0.0/requirements.txt
+-rw-r--r--   0 james      (501) staff       (20)     2029 2023-04-17 21:39:50.546258 zict-3.0.0/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)       61 2022-04-28 14:06:51.000000 zict-3.0.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-17 21:39:50.526916 zict-3.0.0/zict/
+-rw-r--r--   0 james      (501) staff       (20)      528 2023-04-17 21:35:32.000000 zict-3.0.0/zict/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6565 2023-04-17 21:35:32.000000 zict-3.0.0/zict/async_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)     9624 2023-04-17 21:35:32.000000 zict-3.0.0/zict/buffer.py
+-rw-r--r--   0 james      (501) staff       (20)     4857 2023-04-17 21:35:32.000000 zict-3.0.0/zict/cache.py
+-rw-r--r--   0 james      (501) staff       (20)     3335 2023-04-17 21:35:32.000000 zict-3.0.0/zict/common.py
+-rw-r--r--   0 james      (501) staff       (20)     5244 2023-04-17 21:35:32.000000 zict-3.0.0/zict/file.py
+-rw-r--r--   0 james      (501) staff       (20)     2196 2023-04-17 21:35:32.000000 zict-3.0.0/zict/func.py
+-rw-r--r--   0 james      (501) staff       (20)     4707 2023-04-17 21:35:32.000000 zict-3.0.0/zict/lmdb.py
+-rw-r--r--   0 james      (501) staff       (20)    10032 2023-04-17 21:35:32.000000 zict-3.0.0/zict/lru.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-04-28 14:06:51.000000 zict-3.0.0/zict/py.typed
+-rw-r--r--   0 james      (501) staff       (20)     4310 2023-04-17 21:35:32.000000 zict-3.0.0/zict/sieve.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-17 21:39:50.543462 zict-3.0.0/zict/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2021-05-04 19:37:47.000000 zict-3.0.0/zict/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1201 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/conftest.py
+-rw-r--r--   0 james      (501) staff       (20)     8626 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_async_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)    10214 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)    11922 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_cache.py
+-rw-r--r--   0 james      (501) staff       (20)     2239 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_common.py
+-rw-r--r--   0 james      (501) staff       (20)     3708 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_file.py
+-rw-r--r--   0 james      (501) staff       (20)     1851 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_func.py
+-rw-r--r--   0 james      (501) staff       (20)     1432 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_lmdb.py
+-rw-r--r--   0 james      (501) staff       (20)    10582 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_lru.py
+-rw-r--r--   0 james      (501) staff       (20)     6674 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_sieve.py
+-rw-r--r--   0 james      (501) staff       (20)     2912 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     2704 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/test_zip.py
+-rw-r--r--   0 james      (501) staff       (20)     8098 2023-04-17 21:35:32.000000 zict-3.0.0/zict/tests/utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)     1927 2023-04-17 21:35:32.000000 zict-3.0.0/zict/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     3012 2023-04-17 21:35:32.000000 zict-3.0.0/zict/zip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-17 21:39:50.529948 zict-3.0.0/zict.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      899 2023-04-17 21:39:50.000000 zict-3.0.0/zict.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      744 2023-04-17 21:39:50.000000 zict-3.0.0/zict.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-04-17 21:39:50.000000 zict-3.0.0/zict.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-04-17 21:39:50.000000 zict-3.0.0/zict.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)        5 2023-04-17 21:39:50.000000 zict-3.0.0/zict.egg-info/top_level.txt
```

### Comparing `zict-2.2.0/LICENSE.txt` & `zict-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zict-2.2.0/PKG-INFO` & `zict-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: zict
-Version: 2.2.0
+Version: 3.0.0
 Summary: Mutable mapping tools
 Home-page: http://zict.readthedocs.io/en/latest/
 Maintainer: Matthew Rocklin
 Maintainer-email: mrocklin@coiled.io
 License: BSD
 Keywords: mutable mapping,dict,dask
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 
 Mutable Mapping tools. See `documentation`_.
 
 .. _documentation: http://zict.readthedocs.io/en/latest/
```

### Comparing `zict-2.2.0/zict/func.py` & `zict-3.0.0/zict/func.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Callable, Iterable, Iterator, KeysView, MutableMapping
+from collections.abc import Callable, Iterable, Iterator, MutableMapping
 from typing import Generic, TypeVar
 
 from zict.common import KT, VT, ZictBase, close, flush
 
 WT = TypeVar("WT")
 
 
@@ -23,15 +23,15 @@
     --------
     >>> def double(x):
     ...     return x * 2
 
     >>> def halve(x):
     ...     return x / 2
 
-    >>> d = dict()
+    >>> d = {}
     >>> f = Func(double, halve, d)
     >>> f['x'] = 10
     >>> d
     {'x': 20}
     >>> f['x']
     10.0
     """
@@ -42,43 +42,33 @@
 
     def __init__(
         self,
         dump: Callable[[VT], WT],
         load: Callable[[WT], VT],
         d: MutableMapping[KT, WT],
     ):
-        # FIXME https://github.com/python/mypy/issues/708
-        self.dump = dump  # type: ignore
-        self.load = load  # type: ignore
+        super().__init__()
+        self.dump = dump
+        self.load = load
         self.d = d
 
     def __getitem__(self, key: KT) -> VT:
-        return self.load(self.d[key])  # type: ignore
+        return self.load(self.d[key])
 
     def __setitem__(self, key: KT, value: VT) -> None:
-        self.d[key] = self.dump(value)  # type: ignore
+        self.d[key] = self.dump(value)
 
     def __contains__(self, key: object) -> bool:
         return key in self.d
 
     def __delitem__(self, key: KT) -> None:
         del self.d[key]
 
-    def keys(self) -> KeysView[KT]:
-        return self.d.keys()
-
-    # FIXME dictionary views https://github.com/dask/zict/issues/61
-    def values(self) -> Iterator[VT]:  # type: ignore
-        return (self.load(v) for v in self.d.values())  # type: ignore
-
-    def items(self) -> Iterator[tuple[KT, VT]]:  # type: ignore
-        return ((k, self.load(v)) for k, v in self.d.items())  # type: ignore
-
     def _do_update(self, items: Iterable[tuple[KT, VT]]) -> None:
-        it = ((k, self.dump(v)) for k, v in items)  # type: ignore
+        it = ((k, self.dump(v)) for k, v in items)
         self.d.update(it)
 
     def __iter__(self) -> Iterator[KT]:
         return iter(self.d)
 
     def __len__(self) -> int:
         return len(self.d)
@@ -91,15 +81,15 @@
     def flush(self) -> None:
         flush(self.d)
 
     def close(self) -> None:
         close(self.d)
 
 
-def funcname(func) -> str:
+def funcname(func: Callable) -> str:
     """Get the name of a function."""
     while hasattr(func, "func"):
         func = func.func
     try:
         return func.__name__
     except Exception:
         return str(func)
```

### Comparing `zict-2.2.0/zict/lmdb.py` & `zict-3.0.0/zict/zip.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,104 @@
 from __future__ import annotations
 
-import sys
-from collections.abc import Iterable, Iterator
+import zipfile
+from collections.abc import Iterator
+from typing import MutableMapping  # TODO move to collections.abc (needs Python >=3.9)
+from typing import TYPE_CHECKING, Any, Literal
 
-from zict.common import ZictBase
+if TYPE_CHECKING:
+    # TODO: import from typing (needs Python >=3.10)
+    from typing_extensions import TypeAlias
 
+FileMode: TypeAlias = Literal["r", "w", "x", "a"]
 
-def _encode_key(key: str) -> bytes:
-    return key.encode("utf-8")
 
-
-def _decode_key(key: bytes) -> str:
-    return key.decode("utf-8")
-
-
-class LMDB(ZictBase[str, bytes]):
-    """Mutable Mapping interface to a LMDB database.
+class Zip(MutableMapping[str, bytes]):
+    """Mutable Mapping interface to a Zip file
 
     Keys must be strings, values must be bytes
 
     Parameters
     ----------
-    directory: string
+    filename: string
+    mode: string, ('r', 'w', 'a'), defaults to 'a'
+
+    Notes
+    -----
+    None of this class is thread-safe - not even normally trivial methods such as
+    ``__len__ `` or ``__contains__``.
 
     Examples
     --------
-    >>> z = LMDB('/tmp/somedir/')  # doctest: +SKIP
+    >>> z = Zip('myfile.zip')  # doctest: +SKIP
     >>> z['x'] = b'123'  # doctest: +SKIP
     >>> z['x']  # doctest: +SKIP
     b'123'
+    >>> z.flush()  # flush and write metadata to disk  # doctest: +SKIP
     """
 
-    def __init__(self, directory: str):
-        import lmdb
-
-        # map_size is the maximum database size but shouldn't fill up the
-        # virtual address space
-        map_size = 1 << 40 if sys.maxsize >= 2**32 else 1 << 28
-        # writemap requires sparse file support otherwise the whole
-        # `map_size` may be reserved up front on disk
-        writemap = sys.platform.startswith("linux")
-        self.db = lmdb.open(
-            directory,
-            subdir=True,
-            map_size=map_size,
-            sync=False,
-            writemap=writemap,
-        )
+    filename: str
+    mode: FileMode | Literal["closed"]
+    _file: zipfile.ZipFile | None
+
+    def __init__(self, filename: str, mode: FileMode = "a"):
+        super().__init__()
+        self.filename = filename
+        self.mode = mode
+        self._file = None
+
+    @property
+    def file(self) -> zipfile.ZipFile:
+        if self.mode == "closed":
+            raise OSError("File closed")
+        if not self._file or not self._file.fp:
+            self._file = zipfile.ZipFile(self.filename, mode=self.mode)
+        return self._file
 
     def __getitem__(self, key: str) -> bytes:
-        with self.db.begin() as txn:
-            value = txn.get(_encode_key(key))
-        if value is None:
+        if not isinstance(key, str):
             raise KeyError(key)
-        return value
+        return self.file.read(key)
+
+    def __setitem__(self, key: str, value: bytes | bytearray | memoryview) -> None:
+        if not isinstance(key, str):
+            raise TypeError(key)
+        if not isinstance(value, (bytes, bytearray, memoryview)):
+            raise TypeError(value)
+        if key in self:
+            raise NotImplementedError("Not supported by stdlib zipfile")
+        self.file.writestr(key, value)
 
-    def __setitem__(self, key: str, value: bytes) -> None:
-        with self.db.begin(write=True) as txn:
-            txn.put(_encode_key(key), value)
+    def __iter__(self) -> Iterator[str]:
+        return (zi.filename for zi in self.file.filelist)
 
     def __contains__(self, key: object) -> bool:
         if not isinstance(key, str):
             return False
-        with self.db.begin() as txn:
-            return txn.cursor().set_key(_encode_key(key))
-
-    # FIXME dictionary views https://github.com/dask/zict/issues/61
-    def items(self) -> Iterator[tuple[str, bytes]]:  # type: ignore
-        cursor = self.db.begin().cursor()
-        return ((_decode_key(k), v) for k, v in cursor.iternext(keys=True, values=True))
-
-    def keys(self) -> Iterator[str]:  # type: ignore
-        cursor = self.db.begin().cursor()
-        return (_decode_key(k) for k in cursor.iternext(keys=True, values=False))
-
-    def values(self) -> Iterator[bytes]:  # type: ignore
-        cursor = self.db.begin().cursor()
-        return cursor.iternext(keys=False, values=True)
-
-    def _do_update(self, items: Iterable[tuple[str, bytes]]) -> None:
-        # Optimized version of update() using a single putmulti() call.
-        items_enc = [(_encode_key(k), v) for k, v in items]
-        with self.db.begin(write=True) as txn:
-            consumed, added = txn.cursor().putmulti(items_enc)
-            assert consumed == added == len(items_enc)
-
-    def __iter__(self) -> Iterator[str]:
-        return self.keys()
+        try:
+            self.file.getinfo(key)
+            return True
+        except KeyError:
+            return False
 
-    def __delitem__(self, key: str) -> None:
-        with self.db.begin(write=True) as txn:
-            if not txn.delete(_encode_key(key)):
-                raise KeyError(key)
+    def __delitem__(self, key: str) -> None:  # pragma: nocover
+        raise NotImplementedError("Not supported by stdlib zipfile")
 
     def __len__(self) -> int:
-        return self.db.stat()["entries"]
+        return len(self.file.filelist)
+
+    def flush(self) -> None:
+        if self._file:
+            if self._file.fp:
+                self._file.fp.flush()
+            self._file.close()
+            self._file = None
 
     def close(self) -> None:
-        self.db.close()
+        self.flush()
+        self.mode = "closed"
+
+    def __enter__(self) -> Zip:
+        return self
+
+    def __exit__(self, *args: Any) -> None:
+        self.close()
```

### Comparing `zict-2.2.0/zict/lru.py` & `zict-3.0.0/zict/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,169 +1,148 @@
 from __future__ import annotations
 
-from collections.abc import (
-    Callable,
-    ItemsView,
-    Iterator,
-    KeysView,
-    MutableMapping,
-    ValuesView,
-)
+import weakref
+from collections.abc import Iterator, MutableMapping
+from typing import TYPE_CHECKING
 
-from heapdict import heapdict
+from zict.common import KT, VT, ZictBase, close, discard, flush, locked
 
-from zict.common import KT, VT, ZictBase, close, flush
 
-
-class LRU(ZictBase[KT, VT]):
-    """Evict Least Recently Used Elements.
+class Cache(ZictBase[KT, VT]):
+    """Transparent write-through cache around a MutableMapping with an expensive
+    __getitem__ method.
 
     Parameters
     ----------
-    n: int or float
-        Number of elements to keep, or total weight if weight= is used
-    d: MutableMapping
-        Dict-like in which to hold elements
-    on_evict: list of callables
-        Function:: k, v -> action to call on key value pairs prior to eviction
-        If an exception occurs during an on_evict callback (e.g a callback tried
-        storing to disk and raised a disk full error) the key will remain in the LRU.
-    weight: callable
-        Function:: k, v -> number to determine the size of keeping the item in
-        the mapping.  Defaults to ``(k, v) -> 1``
+    data: MutableMapping
+        Persistent, slow to read mapping to be cached
+    cache: MutableMapping
+        Fast cache for reads from data. This mapping may lose keys on its own; e.g. it
+        could be a LRU.
+    update_on_set: bool, optional
+        If True (default), the cache will be updated both when writing and reading.
+        If False, update the cache when reading, but just invalidate it when writing.
+
+    Notes
+    -----
+    If you call methods of this class from multiple threads, access will be fast as long
+    as all methods of ``cache``, plus ``data.__delitem__``, are fast. Other methods of
+    ``data`` are not protected by locks.
 
     Examples
     --------
-    >>> lru = LRU(2, {}, on_evict=lambda k, v: print("Lost", k, v))
-    >>> lru['x'] = 1
-    >>> lru['y'] = 2
-    >>> lru['z'] = 3
-    Lost x 1
+    Keep the latest 100 accessed values in memory
+    >>> from zict import Cache, File, LRU, WeakValueMapping
+    >>> d = Cache(File('myfile'), LRU(100, {}))  # doctest: +SKIP
+
+    Read data from disk every time, unless it was previously accessed and it's still in
+    use somewhere else in the application
+    >>> d = Cache(File('myfile'), WeakValueMapping())  # doctest: +SKIP
     """
 
-    d: MutableMapping[KT, VT]
-    heap: heapdict[KT, VT]
-    on_evict: list[Callable[[KT, VT], None]]
-    weight: Callable[[KT, VT], float]
-    n: float
-    i: int
-    total_weight: float
-    weights: dict[KT, float]
+    data: MutableMapping[KT, VT]
+    cache: MutableMapping[KT, VT]
+    update_on_set: bool
+    _gen: int
+    _last_updated: dict[KT, int]
 
     def __init__(
         self,
-        n: float,
-        d: MutableMapping[KT, VT],
-        on_evict: Callable[[KT, VT], None]
-        | list[Callable[[KT, VT], None]]
-        | None = None,
-        weight: Callable[[KT, VT], float] = lambda k, v: 1,
+        data: MutableMapping[KT, VT],
+        cache: MutableMapping[KT, VT],
+        update_on_set: bool = True,
     ):
-        self.d = d
-        self.n = n
-        self.heap = heapdict()
-        self.i = 0
-        if callable(on_evict):
-            on_evict = [on_evict]
-        self.on_evict = on_evict or []
-        # FIXME https://github.com/python/mypy/issues/708
-        self.weight = weight  # type: ignore
-        self.total_weight = 0
-        self.weights = {}
+        super().__init__()
+        self.data = data
+        self.cache = cache
+        self.update_on_set = update_on_set
+        self._gen = 0
+        self._last_updated = {}
 
+    @locked
     def __getitem__(self, key: KT) -> VT:
-        result = self.d[key]
-        self.i += 1
-        self.heap[key] = self.i
-        return result
+        try:
+            return self.cache[key]
+        except KeyError:
+            pass
+        gen = self._last_updated[key]
+
+        with self.unlock():
+            value = self.data[key]
+
+        # Could another thread have called __setitem__ or __delitem__ on the
+        # same key in the meantime? If not, update the cache
+        if gen == self._last_updated.get(key):
+            self.cache[key] = value
+            self._last_updated[key] += 1
+        return value
 
+    @locked
     def __setitem__(self, key: KT, value: VT) -> None:
-        if key in self.d:
-            del self[key]
-
-        weight = self.weight(key, value)  # type: ignore
-
-        def set_():
-            self.d[key] = value
-            self.i += 1
-            self.heap[key] = self.i
-            self.weights[key] = weight
-            self.total_weight += weight
-            # Evicting the last key/value pair is guaranteed to fail, so don't try.
-            # This is because it is always the last one inserted by virtue of this
-            # being an LRU, which in turn means we reached this point because
-            # weight > self.n and a callbacks raised exception (e.g. disk full).
-            while self.total_weight > self.n and len(self.d) > 1:
-                self.evict()
-
-        if weight <= self.n:
-            set_()
+        # If the item was already in cache and data.__setitem__ fails, e.g. because
+        # it's a File and the disk is full, make sure that the cache is invalidated.
+        discard(self.cache, key)
+        gen = self._gen
+        gen += 1
+        self._last_updated[key] = self._gen = gen
+
+        with self.unlock():
+            self.data[key] = value
+
+        if key not in self._last_updated:
+            # Another thread called __delitem__ in the meantime
+            discard(self.data, key)
+        elif gen != self._last_updated[key]:
+            # Another thread called __setitem__ in the meantime. We have no idea which
+            # of the two ended up actually setting self.data.
+            # Case 1: the other thread did not enter this locked code block yet.
+            #         Prevent it from setting the cache.
+            self._last_updated[key] += 1
+            # Case 2: the other thread already exited this locked code block and set the
+            #         cache. Invalidate it.
+            discard(self.cache, key)
         else:
-            try:
-                for cb in self.on_evict:
-                    cb(key, value)
-            except Exception:
-                # e.g. if a callback tried storing to disk and raised a disk full error
-                set_()
-                raise
-
-    def evict(self) -> tuple[KT, VT, float]:
-        """Evict least recently used key
-
-        This is typically called from internal use, but can be externally
-        triggered as well.
-
-        Returns
-        -------
-        k: key
-        v: value
-        w: weight
-        """
-        k, priority = self.heap.popitem()
-        v = self.d.pop(k)
-        try:
-            for cb in self.on_evict:
-                cb(k, v)
-        except Exception:
-            # e.g. if a callback tried storing to disk and raised a disk full error
-            self.heap[k] = priority
-            self.d[k] = v
-            raise
-
-        weight = self.weights.pop(k)
-        self.total_weight -= weight
-        return k, v, weight
+            # No race condition
+            self._last_updated[key] += 1
+            if self.update_on_set:
+                self.cache[key] = value
 
+    @locked
     def __delitem__(self, key: KT) -> None:
-        del self.d[key]
-        del self.heap[key]
-        self.total_weight -= self.weights.pop(key)
-
-    def keys(self) -> KeysView[KT]:
-        return self.d.keys()
-
-    def values(self) -> ValuesView[VT]:
-        return self.d.values()
-
-    def items(self) -> ItemsView[KT, VT]:
-        return self.d.items()
+        del self.data[key]
+        del self._last_updated[key]
+        discard(self.cache, key)
 
     def __len__(self) -> int:
-        return len(self.d)
+        return len(self.data)
 
     def __iter__(self) -> Iterator[KT]:
-        return iter(self.d)
+        return iter(self.data)
 
     def __contains__(self, key: object) -> bool:
-        return key in self.d
-
-    def __str__(self) -> str:
-        sub = str(self.d) if not isinstance(self.d, dict) else "dict"
-        return f"<LRU: {self.total_weight}/{self.n} on {sub}>"
-
-    __repr__ = __str__
+        # Do not let MutableMapping call self.data[key]
+        return key in self.data
 
     def flush(self) -> None:
-        flush(self.d)
+        flush(self.cache, self.data)
 
     def close(self) -> None:
-        close(self.d)
+        close(self.cache, self.data)
+
+
+if TYPE_CHECKING:
+    # TODO remove this branch and just use [] in the implementation below (needs Python >=3.9)
+    class WeakValueMapping(weakref.WeakValueDictionary[KT, VT]):
+        ...
+
+else:
+
+    class WeakValueMapping(weakref.WeakValueDictionary):
+        """Variant of weakref.WeakValueDictionary which silently ignores objects that
+        can't be referenced by a weakref.ref
+        """
+
+        def __setitem__(self, key: KT, value: VT) -> None:
+            try:
+                super().__setitem__(key, value)
+            except TypeError:
+                pass
```

### Comparing `zict-2.2.0/zict/tests/test_file.py` & `zict-3.0.0/zict/tests/test_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,148 @@
 import os
-import shutil
+import pathlib
+import sys
 
 import pytest
 
-from zict.file import File
+from zict import File
 from zict.tests import utils_test
 
 
-@pytest.fixture
-def fn():
-    filename = ".tmp"
-    if os.path.exists(filename):
-        shutil.rmtree(filename)
-
-    yield filename
-
-    if os.path.exists(filename):
-        shutil.rmtree(filename)
-
-
-def test_mapping(fn):
+def test_mapping(tmp_path, check_fd_leaks):
     """
     Test mapping interface for File().
     """
-    z = File(fn)
+    z = File(tmp_path)
     utils_test.check_mapping(z)
 
 
-def test_implementation(fn):
-    z = File(fn)
+@pytest.mark.parametrize("dirtype", [str, pathlib.Path, lambda x: x])
+def test_implementation(tmp_path, check_fd_leaks, dirtype):
+    z = File(dirtype(tmp_path))
     assert not z
 
     z["x"] = b"123"
-    assert os.listdir(fn) == ["x"]
-    with open(os.path.join(fn, "x"), "rb") as f:
+    assert os.listdir(tmp_path) == ["x#0"]
+    with open(tmp_path / "x#0", "rb") as f:
         assert f.read() == b"123"
 
     assert "x" in z
+    out = z["x"]
+    assert isinstance(out, bytearray)
+    assert out == b"123"
 
 
-def test_memmap_implementation(fn):
-    z = File(fn, memmap=True)
+def test_memmap_implementation(tmp_path, check_fd_leaks):
+    z = File(tmp_path, memmap=True)
     assert not z
 
-    z["x"] = b"123"
-    assert os.listdir(fn) == ["x"]
-    assert z["x"] == memoryview(b"123")
-
+    mv = memoryview(b"123")
+    assert "x" not in z
+    z["x"] = mv
+    assert os.listdir(tmp_path) == ["x#0"]
     assert "x" in z
+    mv2 = z["x"]
+    assert mv2 == b"123"
+    # Buffer is writeable
+    mv2[0] = mv2[1]
+    assert mv2 == b"223"
 
 
-def test_str(fn):
-    z = File(fn)
-    assert fn in str(z)
-    assert fn in repr(z)
-    assert z.mode in str(z)
-    assert z.mode in repr(z)
+def test_str(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
+    assert str(z) == repr(z) == f"<File: {tmp_path}, 0 elements>"
 
 
-def test_setitem_typeerror(fn):
-    z = File(fn)
+def test_setitem_typeerror(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
     with pytest.raises(TypeError):
         z["x"] = 123
 
 
-def test_contextmanager(fn):
-    with File(fn) as z:
+def test_contextmanager(tmp_path, check_fd_leaks):
+    with File(tmp_path) as z:
         z["x"] = b"123"
 
-    with open(os.path.join(fn, "x"), "rb") as f:
-        assert f.read() == b"123"
+    with open(tmp_path / "x#0", "rb") as fh:
+        assert fh.read() == b"123"
 
 
-def test_delitem(fn):
-    z = File(fn)
+def test_delitem(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
 
     z["x"] = b"123"
-    assert os.path.exists(os.path.join(z.directory, "x"))
+    assert os.listdir(tmp_path) == ["x#0"]
     del z["x"]
-    assert not os.path.exists(os.path.join(z.directory, "x"))
+    assert os.listdir(tmp_path) == []
+    # File name is never repeated
+    z["x"] = b"123"
+    assert os.listdir(tmp_path) == ["x#1"]
+    # __setitem__ deletes the previous file
+    z["x"] = b"123"
+    assert os.listdir(tmp_path) == ["x#2"]
 
 
-def test_missing_key(fn):
-    z = File(fn)
+def test_missing_key(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
 
     with pytest.raises(KeyError):
         z["x"]
 
 
-def test_arbitrary_chars(fn):
-    z = File(fn)
+def test_arbitrary_chars(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
 
     # Avoid hitting the Windows max filename length
     chunk = 16
     for i in range(1, 128, chunk):
         key = "".join(["foo_"] + [chr(i) for i in range(i, min(128, i + chunk))])
         with pytest.raises(KeyError):
             z[key]
         z[key] = b"foo"
         assert z[key] == b"foo"
         assert list(z) == [key]
         assert list(z.keys()) == [key]
         assert list(z.items()) == [(key, b"foo")]
         assert list(z.values()) == [b"foo"]
 
-        zz = File(fn)
+        zz = File(tmp_path)
         assert zz[key] == b"foo"
         assert list(zz) == [key]
         assert list(zz.keys()) == [key]
         assert list(zz.items()) == [(key, b"foo")]
         assert list(zz.values()) == [b"foo"]
         del zz
 
         del z[key]
         with pytest.raises(KeyError):
             z[key]
 
 
-def test_write_list_of_bytes(fn):
-    z = File(fn)
+def test_write_list_of_bytes(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
 
     z["x"] = [b"123", b"4567"]
     assert z["x"] == b"1234567"
+
+
+def test_bad_types(tmp_path, check_fd_leaks):
+    z = File(tmp_path)
+    utils_test.check_bad_key_types(z)
+    utils_test.check_bad_value_types(z)
+
+
+@pytest.mark.stress
+@pytest.mark.repeat(utils_test.REPEAT_STRESS_TESTS)
+def test_stress_different_keys_threadsafe(tmp_path):
+    z = File(tmp_path)
+    utils_test.check_different_keys_threadsafe(z)
+    utils_test.check_mapping(z)
+
+
+@pytest.mark.stress
+@pytest.mark.repeat(utils_test.REPEAT_STRESS_TESTS)
+@pytest.mark.skipif(sys.platform == "win32", reason="Can't delete file with open fd")
+def test_stress_same_key_threadsafe(tmp_path):
+    z = File(tmp_path)
+    utils_test.check_same_key_threadsafe(z)
+    utils_test.check_mapping(z)
```

### Comparing `zict-2.2.0/zict/tests/test_func.py` & `zict-3.0.0/zict/tests/test_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def rotr(x):
     return x[-1:] + x[:-1]
 
 
 def test_simple():
-    d = dict()
+    d = {}
     f = Func(inc, dec, d)
     f["x"] = 10
     assert f["x"] == 10
     assert d["x"] == 11
 
     assert "x" in f
     assert list(f) == ["x"]
```

### Comparing `zict-2.2.0/zict/zip.py` & `zict-3.0.0/zict/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,129 @@
 from __future__ import annotations
 
-import zipfile
-from collections.abc import Iterator
+import threading
+from collections.abc import Callable, Iterable, Iterator, Mapping
+from contextlib import contextmanager
+from enum import Enum
+from functools import wraps
+from itertools import chain
 from typing import MutableMapping  # TODO move to collections.abc (needs Python >=3.9)
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, TypeVar, cast
+
+T = TypeVar("T")
+KT = TypeVar("KT")
+VT = TypeVar("VT")
 
 if TYPE_CHECKING:
-    # TODO: move to typing on Python 3.8+ and 3.10+ respectively
-    from typing_extensions import Literal, TypeAlias
+    # TODO import ParamSpec from typing (needs Python >=3.10)
+    # TODO import Self from typing (needs Python >=3.11)
+    from typing_extensions import ParamSpec, Self
 
-    FileMode: TypeAlias = Literal["r", "w", "x", "a"]
+    P = ParamSpec("P")
 
 
-class Zip(MutableMapping[str, bytes]):
-    """Mutable Mapping interface to a Zip file
+class NoDefault(Enum):
+    nodefault = None
 
-    Keys must be strings, values must be bytes
 
-    Parameters
-    ----------
-    filename: string
-    mode: string, ('r', 'w', 'a'), defaults to 'a'
+nodefault = NoDefault.nodefault
 
-    Examples
-    --------
-    >>> z = Zip('myfile.zip')  # doctest: +SKIP
-    >>> z['x'] = b'123'  # doctest: +SKIP
-    >>> z['x']  # doctest: +SKIP
-    b'123'
-    >>> z.flush()  # flush and write metadata to disk  # doctest: +SKIP
-    """
 
-    filename: str
-    mode: FileMode | Literal["closed"]
-    _file: zipfile.ZipFile | None
-
-    def __init__(self, filename: str, mode: FileMode = "a"):
-        self.filename = filename
-        self.mode = mode
-        self._file = None
-
-    @property
-    def file(self) -> zipfile.ZipFile:
-        if self.mode == "closed":
-            raise OSError("File closed")
-        if not self._file or not self._file.fp:
-            self._file = zipfile.ZipFile(self.filename, mode=self.mode)
-        return self._file
-
-    def __getitem__(self, key: str) -> bytes:
-        return self.file.read(key)
-
-    def __setitem__(self, key: str, value: bytes) -> None:
-        self.file.writestr(key, value)
-
-    # FIXME dictionary views https://github.com/dask/zict/issues/61
-    def keys(self) -> Iterator[str]:  # type: ignore
-        return (zi.filename for zi in self.file.filelist)
-
-    def values(self) -> Iterator[bytes]:  # type: ignore
-        return (self.file.read(key) for key in self.keys())
-
-    def items(self) -> Iterator[tuple[str, bytes]]:  # type: ignore
-        return ((zi.filename, self.file.read(zi.filename)) for zi in self.file.filelist)
-
-    def __iter__(self) -> Iterator[str]:
-        return self.keys()
-
-    def __delitem__(self, key: str) -> None:
-        raise NotImplementedError("Not supported by stdlib zipfile")
-
-    def __len__(self) -> int:
-        return len(self.file.filelist)
-
-    def flush(self) -> None:
-        if self._file:
-            if self._file.fp:
-                self._file.fp.flush()
-            self._file.close()
-            self._file = None
+class ZictBase(MutableMapping[KT, VT]):
+    """Base class for zict mappings"""
+
+    lock: threading.RLock
+
+    def __init__(self) -> None:
+        self.lock = threading.RLock()
+
+    def __getstate__(self) -> dict[str, Any]:
+        state = self.__dict__.copy()
+        del state["lock"]
+        return state
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        self.__dict__ = state
+        self.lock = threading.RLock()
+
+    def update(  # type: ignore[override]
+        self,
+        other: Mapping[KT, VT] | Iterable[tuple[KT, VT]] = (),
+        /,
+        **kwargs: VT,
+    ) -> None:
+        if hasattr(other, "items"):
+            other = other.items()
+        other = chain(other, kwargs.items())  # type: ignore
+        self._do_update(other)
+
+    def _do_update(self, items: Iterable[tuple[KT, VT]]) -> None:
+        # Default implementation, can be overriden for speed
+        for k, v in items:
+            self[k] = v
+
+    def discard(self, key: KT) -> None:
+        """Flush *key* if possible.
+        Not the same as ``m.pop(key, None)``, as it doesn't trigger ``__getitem__``.
+        """
+        discard(self, key)
 
     def close(self) -> None:
-        self.flush()
-        self.mode = "closed"
+        """Release any system resources held by this object"""
 
-    def __enter__(self) -> Zip:
+    def __enter__(self) -> Self:
         return self
 
-    def __exit__(self, type, value, traceback) -> None:
+    def __exit__(self, *args: Any) -> None:
         self.close()
+
+    def __del__(self) -> None:
+        self.close()
+
+    @contextmanager
+    def unlock(self) -> Iterator[None]:
+        """To be used in a method decorated by ``@locked``.
+        Temporarily releases the mapping's RLock.
+        """
+        self.lock.release()
+        try:
+            yield
+        finally:
+            self.lock.acquire()
+
+
+def close(*z: Any) -> None:
+    """Close *z* if possible."""
+    for zi in z:
+        if hasattr(zi, "close"):
+            zi.close()
+
+
+def flush(*z: Any) -> None:
+    """Flush *z* if possible."""
+    for zi in z:
+        if hasattr(zi, "flush"):
+            zi.flush()
+
+
+def discard(m: MutableMapping[KT, VT], key: KT) -> None:
+    """Flush *key* if possible.
+    Not the same as ``m.pop(key, None)``, as it doesn't trigger ``__getitem__``.
+    """
+    try:
+        del m[key]
+    except KeyError:
+        pass
+
+
+def locked(func: Callable[P, VT]) -> Callable[P, VT]:
+    """Decorator for a method of ZictBase, which wraps the whole method in a
+    instance-specific (but not key-specific) rlock.
+    """
+
+    @wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> VT:
+        self = cast(ZictBase, args[0])
+        with self.lock:
+            return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `zict-2.2.0/zict.egg-info/PKG-INFO` & `zict-3.0.0/zict.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: zict
-Version: 2.2.0
+Version: 3.0.0
 Summary: Mutable mapping tools
 Home-page: http://zict.readthedocs.io/en/latest/
 Maintainer: Matthew Rocklin
 Maintainer-email: mrocklin@coiled.io
 License: BSD
 Keywords: mutable mapping,dict,dask
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 
 Mutable Mapping tools. See `documentation`_.
 
 .. _documentation: http://zict.readthedocs.io/en/latest/
```

