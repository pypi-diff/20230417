# Comparing `tmp/deli-0.1.1.tar.gz` & `tmp/deli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deli-0.1.1.tar", last modified: Tue Feb  7 08:52:10 2023, max compression
+gzip compressed data, was "deli-0.2.0.tar", last modified: Mon Apr 17 09:55:14 2023, max compression
```

## Comparing `deli-0.1.1.tar` & `deli-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:52:10.382651 deli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-07 08:52:07.000000 deli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-07 08:52:07.000000 deli-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-07 08:52:10.382651 deli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-07 08:52:07.000000 deli-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:52:10.378651 deli-0.1.1/deli/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-07 08:52:07.000000 deli-0.1.1/deli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-07 08:52:07.000000 deli-0.1.1/deli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-02-07 08:52:07.000000 deli-0.1.1/deli/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:52:10.382651 deli-0.1.1/deli/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/nifty.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/numpy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-02-07 08:52:07.000000 deli-0.1.1/deli/serializers/packaged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:52:10.382651 deli-0.1.1/deli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-07 08:52:10.000000 deli-0.1.1/deli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-07 08:52:10.000000 deli-0.1.1/deli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 08:52:10.000000 deli-0.1.1/deli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 08:52:10.000000 deli-0.1.1/deli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 08:52:10.000000 deli-0.1.1/deli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-07 08:52:07.000000 deli-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 08:52:07.000000 deli-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 08:52:10.382651 deli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-07 08:52:07.000000 deli-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 09:55:12.000000 deli-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 09:55:12.000000 deli-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 09:55:14.641601 deli-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 09:55:12.000000 deli-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.637601 deli-0.2.0/deli/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 09:55:12.000000 deli-0.2.0/deli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 09:55:12.000000 deli-0.2.0/deli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-17 09:55:12.000000 deli-0.2.0/deli/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/deli/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/nifty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/numpy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-17 09:55:12.000000 deli-0.2.0/deli/serializers/packaged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:55:14.641601 deli-0.2.0/deli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 09:55:14.000000 deli-0.2.0/deli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-17 09:55:12.000000 deli-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 09:55:12.000000 deli-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:55:14.641601 deli-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 09:55:12.000000 deli-0.2.0/setup.py
```

### Comparing `deli-0.1.1/LICENSE` & `deli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deli-0.1.1/PKG-INFO` & `deli-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
 License: MIT
-Download-URL: https://github.com/maxme1/deli/archive/v0.1.1.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.0.tar.gz
 Keywords: serialization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deli-0.1.1/deli/interface.py` & `deli-0.2.0/deli/interface.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,58 +22,86 @@
     """
     Load a value from a file-like or buffer `source`.
     `hint` is used to override the format detection.
     `kwargs` are format-specific keyword arguments.
     """
     choice = Choice(*REGISTRY)
 
+    hint = _resolve_hint(hint, source)
+    strict = hint is not None
+    # TODO: what is it's both BinaryIO and PathLike?
     if isinstance(source, (str, PathLike)):
-        if hint is None:
-            hint = os.path.basename(os.fspath(source))
+        loader = choice
+        if strict:
+            loader = choice.match_load_path(source, hint, kwargs)
+            if loader is None:
+                raise WrongSerializer(f"Couldn't load from value using {hint!r} as hint")
 
-        try:
-            return choice.load_path(source, hint, kwargs)
-        except WrongSerializer:
-            pass
-
-        with open(source, 'rb') as buffer:
-            return choice.load_buffer(buffer, hint, False, kwargs)
+        return loader.load_path(source, hint, kwargs)
 
     if not isinstance(source, BinaryIO):
-        raise TypeError('Need a binary buffer')
+        raise TypeError(f'Need a binary buffer, not {type(source).__name__}')
+
+    # TODO: reuse
+    loader = choice
+    if strict:
+        loader = choice.match_load_buffer(hint, True, kwargs)
+        if loader is None:
+            raise WrongSerializer(f"Couldn't load from value using {hint!r} as hint")
 
-    return choice.load_buffer(source, hint, True, kwargs)
+    return loader.load_buffer(source, hint, True, kwargs)
 
 
 def save(value: Any, destination: Union[str, PathLike, BinaryIO], hint: MaybeHint = None, **kwargs) -> Hint:
     """
     Save `value` to a file-like or buffer `destination`.
     `hint` is used to override the format detection.
     `kwargs` are format-specific keyword arguments.
     """
     choice = Choice(*REGISTRY)
 
+    hint = _resolve_hint(hint, destination)
+    strict = hint is not None
+    # TODO: what is it's both BinaryIO and PathLike?
     if isinstance(destination, (str, PathLike)):
-        if hint is None:
-            hint = os.path.basename(os.fspath(destination))
-
-        try:
-            return choice.save_path(value, destination, hint, kwargs)
-        except WrongSerializer:
-            pass
+        loader = choice
+        if strict:
+            loader = choice.match_save_path(value, destination, hint, kwargs)
+            if loader is None:
+                raise WrongSerializer(f"Couldn't save value using {hint!r} as hint")
 
-        with open(destination, 'wb') as buffer:
-            return choice.save_buffer(value, buffer, hint, kwargs)
+        return loader.save_path(value, destination, hint, kwargs)
 
     if not isinstance(destination, BinaryIO):
-        raise TypeError('Need a binary buffer')
+        raise TypeError(f'Need a binary buffer, not {type(destination).__name__}')
 
-    return choice.save_buffer(value, destination, hint, kwargs)
+    # TODO: reuse
+    loader = choice
+    if strict:
+        loader = choice.match_save_buffer(value, hint, kwargs)
+        if loader is None:
+            raise WrongSerializer(f"Couldn't save value using {hint!r} as hint")
+
+    return loader.save_buffer(value, destination, hint, kwargs)
+
+
+def _resolve_hint(hint, path) -> MaybeHint:
+    assert isinstance(hint, (str, bool)) or hint is None, hint
+    if hint is None:
+        hint = True
+    if isinstance(hint, str):
+        return hint
+    if not hint:
+        return None
+    if isinstance(path, (str, PathLike)):
+        return os.path.basename(os.fspath(path))
+    return None
 
 
+# TODO: rewrite as generic calls with hints
 def load_json(path: PathLike):
     """Load the contents of a json file."""
     with open(path, 'r') as f:
         return json.load(f)
 
 
 def save_json(value, path: PathLike, *, indent: int = None):
```

### Comparing `deli-0.1.1/deli/serializers/choice.py` & `deli-0.2.0/deli/serializers/choice.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,114 +1,88 @@
 from os import PathLike
 from typing import Any, BinaryIO, Sequence
 
-from .. import Hint, MatchHint, MaybeHint
-from ..serializer import Serializer, WrongSerializer, RequireLazy
+from .. import Hint, MaybeHint
+from ..serializer import Serializer, WrongSerializer, RequireLazy, MaybeSerializer
 
 
 class Choice(Serializer):
     def __init__(self, *choices: Serializer):
         self.choices = choices
 
     # matching
 
-    def match_save_buffer(self, value: Any, hint: MaybeHint, params: dict) -> MatchHint:
-        return min(
-            (choice.match_save_buffer(value, hint, params) for choice in self.choices),
-            key=lambda m: m.value, default=MatchHint.Reject
-        )
-
-    def match_save_path(self, value: Any, destination: PathLike, hint: Hint, params: dict) -> MatchHint:
-        return min(
-            (choice.match_save_path(value, destination, hint, params) for choice in self.choices),
-            key=lambda m: m.value, default=MatchHint.Reject
-        )
-
-    def match_load_buffer(self, hint: MaybeHint, allow_lazy: bool, params: dict) -> MatchHint:
-        return min(
-            (choice.match_load_buffer(hint, allow_lazy, params) for choice in self.choices),
-            key=lambda m: m.value, default=MatchHint.Reject
-        )
-
-    def match_load_path(self, source: PathLike, hint: Hint, params: dict) -> MatchHint:
-        return min(
-            (choice.match_load_path(source, hint, params) for choice in self.choices),
-            key=lambda m: m.value, default=MatchHint.Reject
-        )
+    def match_save_buffer(self, value: Any, hint: MaybeHint, params: dict) -> MaybeSerializer:
+        return self._match(lambda choice: choice.match_save_buffer(value, hint, params))
+
+    def match_save_path(self, value: Any, destination: PathLike, hint: Hint, params: dict) -> MaybeSerializer:
+        return self._match(lambda choice: choice.match_save_path(value, destination, hint, params))
+
+    def match_load_buffer(self, hint: MaybeHint, allow_lazy: bool, params: dict) -> MaybeSerializer:
+        return self._match(lambda choice: choice.match_load_buffer(hint, allow_lazy, params))
+
+    def match_load_path(self, source: PathLike, hint: Hint, params: dict) -> MaybeSerializer:
+        return self._match(lambda choice: choice.match_load_path(source, hint, params))
 
     # saving
 
     def save_buffer(self, value: Any, destination: BinaryIO, hint: MaybeHint, params: dict) -> Hint:
-        choices = self._filter(
-            (choice.match_save_buffer(value, hint, params), choice)
-            for choice in self.choices
-        )
-
         position = destination.tell()
-        for choice in choices:
+        for choice in self.choices:
             try:
                 return choice.save_buffer(value, destination, hint, params)
             except WrongSerializer:
                 if position != destination.tell():
                     destination.seek(position)
                     destination.truncate()
 
         raise WrongSerializer('No serializer was able to save the value')
 
     def save_path(self, value: Any, destination: PathLike, hint: Hint, params: dict) -> Hint:
-        choices = self._filter(
-            (choice.match_save_path(value, destination, hint, params), choice)
-            for choice in self.choices
-        )
-
-        for choice in choices:
+        for choice in self.choices:
             try:
                 return choice.save_path(value, destination, hint, params)
             except WrongSerializer:
                 pass
 
         raise WrongSerializer('No serializer was able to save the value')
 
     # loading
 
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
-        choices = self._filter(
-            (choice.match_load_buffer(hint, allow_lazy, params), choice)
-            for choice in self.choices
-        )
-
         requires_lazy = None
         position = source.tell()
-        for choice in choices:
+        for choice in self.choices:
             try:
                 return choice.load_buffer(source, hint, allow_lazy, params)
             except (WrongSerializer, RequireLazy) as e:
                 if isinstance(e, RequireLazy):
                     requires_lazy = e
 
                 if position != source.tell():
                     source.seek(position)
-                    source.truncate()
 
         if requires_lazy is not None:
             raise requires_lazy
-        raise WrongSerializer('No serializer was able to save the value')
+        raise WrongSerializer('No serializer was able to load the value')
 
     def load_path(self, source: PathLike, hint: Hint, params: dict) -> Any:
-        choices = self._filter(
-            (choice.match_load_path(source, hint, params), choice)
-            for choice in self.choices
-        )
-
-        for choice in choices:
+        for choice in self.choices:
             try:
                 return choice.load_path(source, hint, params)
             except WrongSerializer:
                 pass
 
-        raise WrongSerializer('No serializer was able to save the value')
+        raise WrongSerializer('No serializer was able to load the value')
 
     # internals
 
-    @staticmethod
-    def _filter(values) -> Sequence[Serializer]:
-        return [v for k, v in sorted(values, key=lambda m: m[0].value) if k is not MatchHint.Reject]
+    def _match(self, match):
+        results = []
+        for choice in self.choices:
+            value = match(choice)
+            if value is not None:
+                results.append(value)
+
+        if not results:
+            return None
+        return Choice(*results)
```

### Comparing `deli-0.1.1/deli/serializers/dicom.py` & `deli-0.2.0/deli/serializers/dicom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from os import PathLike
 from typing import BinaryIO, Any, Union
 
-from ..serializer import MaybeHint, REGISTRY, Hint
+from ..serializer import MaybeHint, REGISTRY, Hint, WrongSerializer
 from .helpers import ExtensionMatch, SourceAgnostic
 from .packaged import Gzip
 
 
 class DICOM(ExtensionMatch, SourceAgnostic):
     extensions = '.dcm',
 
     def _match_value(self, value):
         return isinstance(value, pydicom.Dataset)
 
     def load(self, source: Union[PathLike, BinaryIO], hint: MaybeHint, params) -> Any:
-        return pydicom.dcmread(source)
+        try:
+            return pydicom.dcmread(source)
+        except pydicom.errors.InvalidDicomError as e:
+            if hint is not None:
+                raise
+            raise WrongSerializer from e
 
     def save(self, value: Any, destination: Union[PathLike, BinaryIO], hint: MaybeHint, params) -> Hint:
         pydicom.dcmwrite(destination, value)
         return '.dcm'
 
 
 try:
     import pydicom
+    import pydicom.errors
 
     REGISTRY.append(DICOM())
     REGISTRY.append(Gzip(DICOM()))
 
 except ImportError:
     pass
```

### Comparing `deli-0.1.1/deli/serializers/images.py` & `deli-0.2.0/deli/serializers/images.py`

 * *Files identical despite different names*

### Comparing `deli-0.1.1/deli/serializers/nifty.py` & `deli-0.2.0/deli/serializers/nifty.py`

 * *Files identical despite different names*

### Comparing `deli-0.1.1/deli/serializers/packaged.py` & `deli-0.2.0/deli/serializers/packaged.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 
 try:
     from gzip import BadGzipFile
 except ImportError:
     # for py3.6
     BadGzipFile = OSError
 
-from .helpers import ExtensionMatch, NoPath
-from ..serializer import Serializer, MatchHint, MaybeHint, WrongSerializer, REGISTRY, Hint
+from .helpers import ExtensionMatch, PathAsBuffer
+from ..serializer import Serializer, MaybeSerializer, MaybeHint, WrongSerializer, REGISTRY, Hint
 
 
-class JSON(NoPath, ExtensionMatch):
+class JSON(PathAsBuffer, ExtensionMatch):
     extensions = '.json',
 
     def _match_save_params(self, params: dict):
         return set(params) <= {'indent'}
 
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
         wrapper = TextIOWrapper(source)
         try:
             return json.load(wrapper)
-        except TypeError as e:
+        except (TypeError, json.JSONDecodeError) as e:
+            if hint is not None:
+                raise
             raise WrongSerializer from e
         finally:
             wrapper.detach()
 
     def save_buffer(self, value: Any, destination: BinaryIO, hint: MaybeHint, params: dict) -> Hint:
         wrapper = TextIOWrapper(destination)
         try:
@@ -37,27 +39,27 @@
             raise WrongSerializer from e
         finally:
             wrapper.detach()
 
         return '.json'
 
 
-class Pickle(ExtensionMatch, NoPath):
+class Pickle(ExtensionMatch, PathAsBuffer):
     extensions = '.pkl',
 
     # TODO: check magic bits
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
         return pickle.load(source)
 
     def save_buffer(self, value: Any, destination: BinaryIO, hint: MaybeHint, params: dict) -> Hint:
         pickle.dump(value, destination)
         return '.pkl'
 
 
-class Text(ExtensionMatch, NoPath):
+class Text(ExtensionMatch, PathAsBuffer):
     extensions = '.txt',
 
     def _match_value(self, value):
         return isinstance(value, str)
 
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
         wrapper = TextIOWrapper(source)
@@ -72,55 +74,65 @@
             wrapper.write(value)
         finally:
             wrapper.detach()
 
         return '.txt'
 
 
-class Gzip(NoPath, Serializer):
+class Gzip(PathAsBuffer, Serializer):
     def __init__(self, serializer: Serializer):
         self.serializer = serializer
         self._ext = '.gz'
 
     def _match(self, name):
         return name is not None and name.endswith(self._ext)
 
     def _trim(self, name):
         return None if name is None else name[:-len(self._ext)]
 
-    def match_save_buffer(self, value: Any, hint: MaybeHint, params: dict) -> MatchHint:
+    def match_save_buffer(self, value: Any, hint: MaybeHint, params: dict) -> MaybeSerializer:
         if not self._match(hint):
-            return MatchHint.NotSure
+            return
 
         params = params.copy()
         params.pop('compression', None)
-        return self.serializer.match_save_buffer(value, self._trim(hint), params)
+        child = self.serializer.match_save_buffer(value, self._trim(hint), params)
+        if child is None:
+            return
+        return Gzip(child)
 
-    def match_load_buffer(self, hint: MaybeHint, allow_lazy: bool, params: dict) -> MatchHint:
+    def match_load_buffer(self, hint: MaybeHint, allow_lazy: bool, params: dict) -> MaybeSerializer:
         if not self._match(hint):
-            return MatchHint.NotSure
+            return
 
-        return self.serializer.match_load_buffer(self._trim(hint), allow_lazy, params)
+        child = self.serializer.match_load_buffer(self._trim(hint), allow_lazy, params)
+        if child is None:
+            return
+        return Gzip(child)
 
     def load_buffer(self, source: BinaryIO, hint: MaybeHint, allow_lazy: bool, params: dict) -> Any:
         try:
             with GzipFile(fileobj=source, mode='rb') as local:
                 return self.serializer.load_buffer(local, self._trim(hint), allow_lazy, params)
         except BadGzipFile as e:
+            if self.match_load_buffer(hint, allow_lazy, params):
+                raise
             raise WrongSerializer from e
 
     def save_buffer(self, value: Any, destination: BinaryIO, hint: MaybeHint, params: dict) -> Hint:
         params = params.copy()
         compression = params.pop('compression', 1)
         mtime = 0
 
         try:
             with GzipFile(fileobj=destination, mode='wb', compresslevel=compression, mtime=mtime) as local:
                 result = self.serializer.save_buffer(value, local, self._trim(hint), params)
         except BadGzipFile as e:
+            if self.match_save_buffer(value, hint, params):
+                raise
             raise WrongSerializer from e
 
         return result + self._ext
 
 
 REGISTRY.extend((
     JSON(), Text(), Pickle(),
```

### Comparing `deli-0.1.1/deli.egg-info/PKG-INFO` & `deli-0.2.0/deli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: deli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Smart serialization and deserialization for (almost) any python object
 Home-page: https://github.com/maxme1/deli
 License: MIT
-Download-URL: https://github.com/maxme1/deli/archive/v0.1.1.tar.gz
+Download-URL: https://github.com/maxme1/deli/archive/v0.2.0.tar.gz
 Keywords: serialization
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `deli-0.1.1/deli.egg-info/SOURCES.txt` & `deli-0.2.0/deli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deli-0.1.1/pyproject.toml` & `deli-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 [project]
-name = "deli"
-dynamic = ["version"]
-description = "Smart serialization and deserialization for (almost) any python object"
-readme = "README.md"
-requires-python = ">=3.6"
-license = { file = "LICENSE" }
-keywords = ["serialization"]
+name = 'deli'
+dynamic = ['version', 'dependencies']
+description = 'Smart serialization and deserialization for (almost) any python object'
+readme = 'README.md'
+requires-python = '>=3.6'
+license = { file = 'LICENSE' }
+keywords = ['serialization']
 authors = [
-    { name = "Max", email = "maxs987@gmail.com" }
+    { name = 'Max', email = 'maxs987@gmail.com' }
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "pandas",
-    "pydicom",
-    "nibabel",
-    "numpy",
-    "imageio>=2.0.0",
+    'Development Status :: 3 - Alpha',
+    'License :: OSI Approved :: MIT License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3 :: Only',
+    'Operating System :: OS Independent',
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/maxme1/deli"
-"Issues" = "https://github.com/maxme1/deli/issues"
-"Source" = "https://github.com/maxme1/deli"
+'Homepage' = 'https://github.com/maxme1/deli'
+'Issues' = 'https://github.com/maxme1/deli/issues'
+'Source' = 'https://github.com/maxme1/deli'
 
 [build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ['setuptools>=43.0.0', 'wheel']
+build-backend = 'setuptools.build_meta'
 
 [tool.setuptools.packages.find]
-include = ["deli"]
+include = ['deli']
 
 [tool.setuptools.dynamic]
-version = { attr = "deli.__version__.__version__" }
+version = { attr = 'deli.__version__.__version__' }
+dependencies = { file = 'requirements.txt' }
```

### Comparing `deli-0.1.1/setup.py` & `deli-0.2.0/setup.py`

 * *Files identical despite different names*

