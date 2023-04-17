# Comparing `tmp/nepattern-0.5.2.tar.gz` & `tmp/nepattern-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.2.tar", last modified: Fri Mar 31 19:15:49 2023, max compression
+gzip compressed data, was "nepattern-0.5.3.tar", last modified: Mon Apr 17 06:24:33 2023, max compression
```

## Comparing `nepattern-0.5.2.tar` & `nepattern-0.5.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.2/LICENSE
--rw-r--r--   0        0        0      702 2023-03-31 19:06:53.768450 nepattern-0.5.2/nepattern/__init__.py
--rw-r--r--   0        0        0     8590 2023-03-31 19:06:53.707148 nepattern-0.5.2/nepattern/base.py
--rw-r--r--   0        0        0      349 2022-09-13 15:51:40.755254 nepattern-0.5.2/nepattern/config.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.2/nepattern/context.py
--rw-r--r--   0        0        0     1416 2023-02-25 09:58:14.679430 nepattern-0.5.2/nepattern/context.pyi
--rw-r--r--   0        0        0    14605 2023-03-31 19:06:53.794063 nepattern-0.5.2/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.2/nepattern/exception.py
--rw-r--r--   0        0        0    10123 2023-03-31 19:04:49.666982 nepattern-0.5.2/nepattern/main.py
--rw-r--r--   0        0        0      475 2023-03-31 19:04:53.036048 nepattern-0.5.2/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-03-31 19:03:12.291942 nepattern-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.2/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.3/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.3/nepattern/__init__.py
+-rw-r--r--   0        0        0     8644 2023-04-17 06:05:25.544604 nepattern-0.5.3/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.3/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.3/nepattern/context.pyi
+-rw-r--r--   0        0        0    14689 2023-04-17 06:05:25.471903 nepattern-0.5.3/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.3/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.3/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.3/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.3/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.3/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.3/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-04-17 05:50:23.807298 nepattern-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.3/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.3/PKG-INFO
```

### Comparing `nepattern-0.5.2/LICENSE` & `nepattern-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.2/nepattern/__init__.py` & `nepattern-0.5.3/nepattern/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from tarina import Empty as _Empty  # noqa
+from tarina import Empty as Empty  # noqa
 from .base import (
     MappingPattern,
     RegexPattern,
     SequencePattern,
     SwitchPattern,
     UnionPattern,
 )
-from .config import lang
 from .context import (
     Patterns,
     all_patterns,
     create_local_patterns,
     local_patterns,
     switch_local_patterns,
     reset_local_patterns
@@ -29,7 +28,9 @@
     URL,
     AnyOne,
     AnyString,
     Bind,
     type_parser,
 )
 from .util import AllParam, TPattern, RawStr
+
+PatternModel = MatchMode
```

### Comparing `nepattern-0.5.2/nepattern/base.py` & `nepattern-0.5.3/nepattern/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 import re
 from typing import Iterable, Any, Literal, TypeVar, Dict, Union
 from tarina import Empty
+from tarina.lang import lang
 
-from .config import lang
 from .core import BasePattern, MatchMode
 from .exception import MatchFailed
 
 
 class RegexPattern(BasePattern[Union[dict, tuple]]):
     """针对正则的特化匹配，支持正则组"""
 
     def __init__(self, pattern: str, alias: str | None = None):
         super().__init__(pattern, origin=Union[dict, tuple], alias=alias or 'regex[:group]')  # type: ignore
 
     def match(self, input_: str | Any):
         if not isinstance(input_, str):
-            raise MatchFailed(lang.type_error.format(target=input_))
+            raise MatchFailed(lang.nepattern.type_error.format(target=input_))
         if mat := self.regex_pattern.match(input_):
             return mat.groupdict() or mat.groups()
-        raise MatchFailed(lang.content_error.format(target=input_))
+        raise MatchFailed(lang.nepattern.content_error.format(target=input_))
 
 
 class UnionPattern(BasePattern):
     """多类型参数的匹配"""
 
     optional: bool
     base: list[BasePattern | object | str]
@@ -55,15 +55,15 @@
     def match(self, text: str | Any):
         if not text:
             text = None
         if text not in self.for_equal:
             for pat in self.for_validate:
                 if (res := pat.validate(text)).success:
                     return res.value
-            raise MatchFailed(lang.content_error.format(target=text))
+            raise MatchFailed(lang.nepattern.content_error.format(target=text))
         return text
 
     def __repr__(self):
         return ("!" if self.anti else "") + (
             "|".join(repr(a) for a in (*self.for_validate, *self.for_equal))
         )
 
@@ -113,15 +113,15 @@
                 r"\((.+?)\)", MatchMode.REGEX_MATCH, form, alias=f"tuple[{base}]"
             )
         elif form is set:
             super().__init__(
                 r"\{(.+?)\}", MatchMode.REGEX_MATCH, form, alias=f"set[{base}]"
             )
         else:
-            raise ValueError(lang.sequence_form_error.format(target=str(form)))
+            raise ValueError(lang.nepattern.sequence_form_error.format(target=str(form)))
 
     def match(self, text: str | Any):
         _res = super().match(text)
         _max = 0
         success: list[tuple[int, Any]] = []
         fail: list[tuple[int, MatchFailed]] = []
         for _max, s in enumerate(
@@ -243,11 +243,11 @@
 
     def match(self, input_: Any) -> _TCase:
         try:
             return self.switch[input_]
         except KeyError as e:
             if Ellipsis in self.switch:
                 return self.switch[...]
-            raise MatchFailed(lang.content_error.format(target=input_)) from e
+            raise MatchFailed(lang.nepattern.content_error.format(target=input_)) from e
 
 
 __all__ = ["RegexPattern", "UnionPattern", "SequencePattern", "MappingPattern", "SwitchPattern"]
```

### Comparing `nepattern-0.5.2/nepattern/context.py` & `nepattern-0.5.3/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.2/nepattern/context.pyi` & `nepattern-0.5.3/nepattern/context.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import UserDict
 from typing import Any, Iterable, final
+from tarina import Empty
 
 from .core import BasePattern
-from .util import Empty
+
 
 @final
 class Patterns(UserDict[Any, BasePattern]):
     name: str
     def __init__(self, name: str): ...
     def set(
         self,
```

### Comparing `nepattern-0.5.2/nepattern/core.py` & `nepattern-0.5.3/nepattern/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     Callable,
     Any,
     Generic,
     overload,
 )
 from dataclasses import dataclass, field
 from tarina import Empty, generic_isinstance
+from tarina.lang import lang
 
 try:
     from typing import Annotated, Self, get_origin  # type: ignore
 except ImportError:
     from typing_extensions import Annotated, Self, get_origin
 
 from .exception import MatchFailed
-from .config import lang
 from .util import TPattern
 
 
 def _accept(
     input_: Any,
     patterns: list[BasePattern] | None = None,
     types: list[type] | None = None,
@@ -180,15 +180,15 @@
         validators: list[Callable[[TOrigin], bool]] | None = None,
         anti: bool = False,
     ):
         """
         初始化参数匹配表达式
         """
         if pattern.startswith("^") or pattern.endswith("$"):
-            raise ValueError(lang.pattern_head_or_tail_error.format(target=pattern))
+            raise ValueError(lang.nepattern.pattern_head_or_tail_error.format(target=pattern))
         self.pattern = pattern
         self.regex_pattern = re.compile(f"^{pattern}$")
         self.mode = MatchMode(model)
         self.origin = origin
         self.alias = alias
         self.previous = previous
         accepts = accepts or []
@@ -306,40 +306,40 @@
             input_, self.pattern_accepts, self.type_accepts
         ):
             if not self.previous or not _accept(
                 input_ := self.previous.match(input_),
                 self.pattern_accepts,
                 self.type_accepts,
             ):  # pragma: no cover
-                raise MatchFailed(lang.type_error.format(target=input_.__class__))
+                raise MatchFailed(lang.nepattern.type_error.format(target=input_.__class__))
         if self.mode == MatchMode.KEEP:
             return input_  # type: ignore
         if self.mode == MatchMode.TYPE_CONVERT:
             res = self.converter(self, input_)
             if res is None and self.origin == Any:  # pragma: no cover
-                raise MatchFailed(lang.content_error.format(target=input_))
+                raise MatchFailed(lang.nepattern.content_error.format(target=input_))
             if not generic_isinstance(res, self.origin):
                 if not self.previous or not generic_isinstance(
                     res := self.converter(self, self.previous.match(input_)), self.origin
                 ):
-                    raise MatchFailed(lang.content_error.format(target=input_))
+                    raise MatchFailed(lang.nepattern.content_error.format(target=input_))
             return res
         if not isinstance(input_, str):
             if not self.previous or not isinstance(
                 input_ := self.previous.match(input_), str
             ):
-                raise MatchFailed(lang.type_error.format(target=type(input_)))
+                raise MatchFailed(lang.nepattern.type_error.format(target=type(input_)))
         if mat := self.regex_pattern.match(input_):
             glen = len(mat.groups())
             return (
                 self.converter(self, mat[1] if glen > 0 else mat[0])
                 if self.mode == MatchMode.REGEX_CONVERT
                 else mat[1] if glen > 0 else mat[0]
             )
-        raise MatchFailed(lang.content_error.format(target=input_))
+        raise MatchFailed(lang.nepattern.content_error.format(target=input_))
 
     @overload
     def validate(self, input_: Any) -> ValidateResult[TOrigin]:
         ...
 
     @overload
     def validate(self, input_: Any, default: TDefault) -> ValidateResult[TOrigin | TDefault]:
@@ -353,15 +353,15 @@
 
         若传入默认值，验证失败会返回默认值
         """
         try:
             res = self.match(input_)
             for i in self.validators:
                 if not i(res):
-                    raise MatchFailed(lang.content_error.format(target=input_))
+                    raise MatchFailed(lang.nepattern.content_error.format(target=input_))
             return ValidateResult(_value=res, flag=ResultFlag.VALID)
         except Exception as e:
             if default is None:
                 return ValidateResult(_error=e, flag=ResultFlag.ERROR)
             return ValidateResult(
                 _value=None if default is Empty else default, flag=ResultFlag.DEFAULT  # type: ignore
             )
@@ -388,15 +388,15 @@
             return ValidateResult(_value=input_, flag=ResultFlag.VALID)
         else:
             for i in self.validators:
                 if not i(res):
                     return ValidateResult(_value=input_, flag=ResultFlag.VALID)
             if default is None:
                 return ValidateResult(
-                    _error=MatchFailed(lang.content_error.format(target=input_)),
+                    _error=MatchFailed(lang.nepattern.content_error.format(target=input_)),
                     flag=ResultFlag.ERROR,
                 )
             return ValidateResult(
                 _value=None if default is Empty else default, flag=ResultFlag.DEFAULT
             )
```

### Comparing `nepattern-0.5.2/nepattern/main.py` & `nepattern-0.5.3/nepattern/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 )
 from contextlib import suppress
 from functools import lru_cache
 from pathlib import Path
 from types import FunctionType, LambdaType, MethodType
 from typing import Any, Union, Literal, TypeVar, runtime_checkable
 from tarina import Empty
+from tarina.lang import lang
 
 try:
     from typing import Annotated, get_args, get_origin  # type: ignore
 except ImportError:
     from typing_extensions import Annotated, get_args, get_origin
 
 
-from .config import lang
 from .context import global_patterns, all_patterns
 from .core import BasePattern, MatchMode
 from .base import UnionPattern, MappingPattern, SequencePattern, RegexPattern, SwitchPattern
-from .util import AllParam, GenericAlias, RawStr
+from .util import AllParam, GenericAlias, RawStr, CGenericAlias
 
 _Contents = (Union, types.UnionType, Literal) if sys.version_info >= (3, 10) else (Union, Literal)  # pragma: no cover
 
 
 AnyOne = BasePattern(r".+", MatchMode.KEEP, Any, alias="any")
 """匹配任意内容的表达式"""
 
@@ -193,15 +193,15 @@
     """对数类型的检查， 将一般数据类型转为 BasePattern 或者特殊类型"""
     if isinstance(item, BasePattern) or item is AllParam:
         return item
     with suppress(TypeError):
         if item and (pat := all_patterns().get(item, None)):
             return pat
     with suppress(TypeError):
-        if not inspect.isclass(item) and isinstance(item, GenericAlias):
+        if not inspect.isclass(item) and isinstance(item, (GenericAlias, CGenericAlias)):
             return _generic_parser(item, extra)
     if isinstance(item, TypeVar):
         return _typevar_parser(item)
     if inspect.isclass(item) and getattr(item, "_is_protocol", False):
         return _protocol_parser(item)
     if isinstance(item, (FunctionType, MethodType, LambdaType)):
         if len((sig := inspect.signature(item)).parameters) not in (1, 2):  # pragma: no cover
@@ -235,15 +235,15 @@
     if isinstance(item, (dict, ABCMap, ABCMuMap)):
         return SwitchPattern(dict(item))
     if item is None or type(None) == item:
         return Empty  # type: ignore
     if extra == "ignore":
         return AnyOne
     elif extra == "reject":
-        raise TypeError(lang.validate_reject.format(target=item))
+        raise TypeError(lang.require("nepattern", "validate_reject").format(target=item))
     return BasePattern.of(item) if inspect.isclass(item) else BasePattern.on(item)
 
 
 class Bind:
     __slots__ = ()
 
     def __new__(cls, *args, **kwargs):  # pragma: no cover
```

### Comparing `nepattern-0.5.2/pyproject.toml` & `nepattern-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nepattern"
-version = "0.5.2"
+version = "0.5.3"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "tarina>=0.1.0",
+    "tarina>=0.3.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "typing",
     "pattern",
     "converter",
```

### Comparing `nepattern-0.5.2/README.md` & `nepattern-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.2/PKG-INFO` & `nepattern-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.2
+Version: 0.5.3
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

