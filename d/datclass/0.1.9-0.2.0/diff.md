# Comparing `tmp/datclass-0.1.9.tar.gz` & `tmp/datclass-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datclass-0.1.9.tar", last modified: Wed Apr  5 06:03:35 2023, max compression
+gzip compressed data, was "datclass-0.2.0.tar", last modified: Mon Apr 17 10:27:02 2023, max compression
```

## Comparing `datclass-0.1.9.tar` & `datclass-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:03:35.830290 datclass-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-05 06:03:30.000000 datclass-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 06:03:30.000000 datclass-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-05 06:03:35.826290 datclass-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-05 06:03:30.000000 datclass-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-05 06:03:30.000000 datclass-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 06:03:30.000000 datclass-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 06:03:35.830290 datclass-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:03:35.826290 datclass-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:03:35.826290 datclass-0.1.9/src/datclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-05 06:03:30.000000 datclass-0.1.9/src/datclass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-04-05 06:03:30.000000 datclass-0.1.9/src/datclass/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-05 06:03:30.000000 datclass-0.1.9/src/datclass/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:03:35.826290 datclass-0.1.9/src/datclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 06:03:35.000000 datclass-0.1.9/src/datclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:27:02.209678 datclass-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 10:26:51.000000 datclass-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 10:26:51.000000 datclass-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-17 10:27:02.209678 datclass-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-17 10:26:51.000000 datclass-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 10:26:51.000000 datclass-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:26:51.000000 datclass-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:27:02.209678 datclass-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:27:02.205678 datclass-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:27:02.205678 datclass-0.2.0/src/datclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-17 10:27:01.000000 datclass-0.2.0/src/datclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 10:26:51.000000 datclass-0.2.0/src/datclass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-17 10:26:51.000000 datclass-0.2.0/src/datclass/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-17 10:26:51.000000 datclass-0.2.0/src/datclass/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:27:02.209678 datclass-0.2.0/src/datclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 10:27:02.000000 datclass-0.2.0/src/datclass.egg-info/top_level.txt
```

### Comparing `datclass-0.1.9/LICENSE` & `datclass-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datclass-0.1.9/PKG-INFO` & `datclass-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.1.9
+Version: 0.2.0
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

### Comparing `datclass-0.1.9/README.md` & `datclass-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datclass-0.1.9/pyproject.toml` & `datclass-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datclass-0.1.9/src/datclass/__init__.py` & `datclass-0.2.0/src/datclass/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __title__ = 'datclass'
 __author__ = 'foyoux'
-__version__ = '0.1.9'
+__version__ = '0.2.0'
 
 __all__ = [
     'main',
     'DatGen',
     'DatClass',
+    'get_datclass',
 ]
 
 import argparse
 import json
 import logging
 import os
 from dataclasses import dataclass, is_dataclass
@@ -28,68 +29,81 @@
         fmt=f'%(asctime)s datclass.%(levelname)s %(message)s',
         datefmt='%Y-%m-%d %H:%M:%S'
     )
 )
 _log.addHandler(_handler)
 
 
-def _datclass_init(self, *args, **kwargs):
-    if kwargs:
-        kwargs = {get_ok_identifier(k): v for k, v in kwargs.items()}
-    getattr(self, _ORIGINAL_INIT)(
-        *args, **{k: kwargs.pop(k) for k in self.__dataclass_fields__ if k in kwargs}
-    )
-    cls = self.__class__
-    for attr, value in kwargs.items():
-        _log.warning(f'{cls.__module__}.{cls.__name__}({attr} : {type(value).__name__} = {value!r})')
-        # 扩展字段
-        setattr(self, attr, value)
-
-
-@dataclass
-class DatClass:
-
-    def __new__(cls, *args, **kwargs):
-        if not hasattr(cls, _ORIGINAL_INIT):
-            setattr(cls, _ORIGINAL_INIT, cls.__init__)
-            setattr(cls, '__init__', _datclass_init)
-        return super().__new__(cls)
-
-    def __post_init__(self, *args, **kwargs):
-        for attr_name, FIELD in self.__dataclass_fields__.items():  # type: ignore
-            attr_type = FIELD.type
-            origin = get_origin(attr_type)
-            if origin is None and is_dataclass(attr_type):
-                attr = getattr(self, attr_name)
-                setattr(self, attr_name, attr_type(**attr) if attr else None)
-                continue
-            for item_type in get_args(attr_type):
-                if is_dataclass(item_type):
-                    setattr(self, attr_name, [item_type(**i) for i in getattr(self, attr_name)])
+def get_datclass(nested: bool = True, extra: bool = True, log: bool = True):
+    def __datclass_init__(obj, *args, **kwargs):
+        # 字段映射为合法字段
+        if kwargs:
+            kwargs = {get_ok_identifier(k): v for k, v in kwargs.items()}
+        # 调用原构造函数
+        getattr(obj, _ORIGINAL_INIT)(*args, **{k: kwargs.pop(k) for k in obj.__dataclass_fields__ if k in kwargs})
+        # 扩展字段或者打印缺失字段日志，并且有未定义的字段
+        if (extra or log) and kwargs:
+            cls = obj.__class__
+            for attr, value in kwargs.items():
+                if log:
+                    _log.warning(f'{cls.__module__}.{cls.__name__}({attr} : {type(value).__name__} = {value!r})')
+                if extra:
+                    setattr(obj, attr, value)
+
+    # noinspection PyPep8Naming
+    @dataclass
+    class __datclass__:
+        def __new__(cls, *args, **kwargs):
+            if not hasattr(cls, _ORIGINAL_INIT):
+                setattr(cls, _ORIGINAL_INIT, cls.__init__)
+                setattr(cls, '__init__', __datclass_init__)
+            return super().__new__(cls)
+
+        # noinspection PyUnusedLocal
+        def __post_init__(self, *args, **kwargs):
+            if not nested:
+                return
+            for attr_name, FIELD in self.__dataclass_fields__.items():  # type: ignore
+                attr_type = FIELD.type
+                origin = get_origin(attr_type)
+                if origin is None and is_dataclass(attr_type):
+                    attr = getattr(self, attr_name)
+                    setattr(self, attr_name, attr_type(**attr) if attr else None)
+                    continue
+                for item_type in get_args(attr_type):
+                    if is_dataclass(item_type):
+                        setattr(self, attr_name, [item_type(**i) for i in getattr(self, attr_name)])
+
+    return __datclass__
+
+
+DatClass = get_datclass()
 
 
 def main():
     epilog = f'%(prog)s({__version__}) by foyoux(https://github.com/foyoux/datclass)'
     parser = argparse.ArgumentParser(prog='datclass', description='generate datclass & support nested and extra',
                                      epilog=epilog)
     parser.add_argument('-v', '--version', action='version', version=epilog)
 
     parser.add_argument('-n', '--name', help='main dat class name', default='Object')
     parser.add_argument('-o', '--output', help='output file - *.py')
-    parser.add_argument('-d', '--dict', help='generate TypedDict class', action='store_true')
+    parser.add_argument('-d', '--dict', help='generate TypedDict class', action='store_false')
+    parser.add_argument('-S', '--no-sort', help='sort attrs', action='store_true')
     parser.add_argument('-R', '--no-recursive', dest='recursive', help='not recursive generate dat class',
                         action='store_false')
     parser.add_argument('file', nargs='?', help='input file - likes-json')
 
     args = parser.parse_args()
 
     name = args.name
     recursive = args.recursive
     input_file = args.file
     output_file = args.output
+    sort = args.sort
 
     if input_file:
         f = Path(input_file)
         if not f.exists():
             print(f'{f.absolute()} not exists')
             return
         text = f.read_text(encoding='utf8')
@@ -104,26 +118,27 @@
         except KeyboardInterrupt:
             print('\n🎉 Bye-Bye')
             return
 
     try:
         body = json.loads(text)
     except json.JSONDecodeError:
+        # noinspection PyBroadException
         try:
             body = eval(text)
-        except:
-            print('\nInvalid JSON/DICT data')
+        except Exception as e:
+            print('\nInvalid JSON/DICT data', e)
             return
 
     gen = DatGen()
 
     if args.dict:
-        codes = gen.gen_typed_dict(body, name, recursive).codes
+        codes = gen.gen_typed_dict(body, name, recursive, sort=sort).codes
     else:
-        codes = gen.gen_datclass(body, name, recursive).codes
+        codes = gen.gen_datclass(body, name, recursive, sort=sort).codes
 
     dat = '\n'.join(gen.imports.codes + codes + [''])
 
     if output_file:
         f = Path(output_file)
         f.parent.mkdir(exist_ok=True, parents=True)
         f.write_text(dat, encoding='utf8')
```

### Comparing `datclass-0.1.9/src/datclass/gens.py` & `datclass-0.2.0/src/datclass/gens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import keyword
 from dataclasses import dataclass, field
 from typing import Union, List
 
-from datclass.utils import get_ok_identifier, get_value_type, get_type_default, merge_list_dict, get_type_string
+from datclass.utils import (
+    get_ok_identifier,
+    get_value_type,
+    get_type_default,
+    merge_list_dict,
+    get_type_string,
+    not_null,
+)
 
 
 @dataclass
 class Imports:
     dataclass: bool = False
     field: bool = False
     List: bool = False
@@ -58,15 +65,15 @@
             if tl:
                 tl += [''] + datclass_imports
             else:
                 tl += datclass_imports
         return tl + ['', '']
 
 
-@dataclass
+@dataclass(order=True)
 class Attr:
     name: str  # attr name
     value: object  # attr value
     # 值类型
     value_type: type = None
     # 缓存
     ok_name: str = None
@@ -85,28 +92,29 @@
     def code(self):
         return f'    {self.ok_name}: {self.type_string} = {self.default_string}{self.comment}'
 
 
 @dataclass
 class Class:
     name: str = None
+    sort: bool = None
     attr_list: List[Attr] = field(default_factory=list)
     classes: List['Class'] = field(default_factory=list)
 
     @property
-    def codes(self, ):
+    def codes(self):
         codes = [f'@dataclass', f'class {self.name}(DatClass):']
-        for attr in self.attr_list:
+        for attr in sorted(self.attr_list) if self.sort else self.attr_list:  # type: ignore
             codes.append(attr.code)
         for cls in self.classes:
             codes = cls.codes + ['', ''] + codes
         return codes
 
 
-@dataclass
+@dataclass(order=True)
 class DictAttr:
     name: str
     value: object
     # 值类型
     value_type: type = None
     type_string: str = None
 
@@ -118,20 +126,22 @@
     def code(self):
         return f'\'{self.name}\': {self.type_string}'
 
 
 @dataclass
 class DictClass:
     name: str = None
+    sort: bool = None
     attr_list: List[DictAttr] = field(default_factory=list)
     classes: List['DictClass'] = field(default_factory=list)
 
     @property
-    def codes(self, ):
-        attr_string = ', '.join([attr.code for attr in self.attr_list])
+    def codes(self):
+        attr_string = ', '.join(
+            [attr.code for attr in (sorted(self.attr_list) if self.sort else self.attr_list)])  # type: ignore
         codes = [f'{self.name} = TypedDict(\'{self.name}\', {{{attr_string}}})']
         for cls in self.classes:
             codes = cls.codes + codes
         return codes
 
 
 class DatGen:
@@ -153,71 +163,75 @@
             cls_name = f'{cls_name}_'
         if keyword.iskeyword(cls_name):
             # 是关键字（eg: None），则加下划线
             cls_name = f'{cls_name}_'
         # 返回之前先记录
         return cls_name
 
-    def gen_datclass(self, dat: Union[list, dict], name='Object', recursive=True, level=0) -> Class:
+    def gen_datclass(self, dat: Union[list, dict], name='Object', recursive=True, sort=True, level=0) -> Class:
         """
         :param dat: 列表 或者 字典
         :param name: 主类名称
         :param recursive: 是否递归生成
+        :param sort: 是否对属性列表进行排序
         :param level: 层级，用以解决 类名 冲突问题
         """
+        assert dat
         self.class_map.append(name)
         try:
             dat = merge_list_dict(dat)
-        except TypeError:
+        except TypeError as e:
             pass
         # 这些针对模块
         self.imports.dataclass = True
         self.imports.DatClass = True
         # 存储类信息
-        obj = Class(name=name)
+        obj = Class(name=name, sort=sort)
         for name, value in dat.items():
             # 存储属性信息
             attr = Attr(name, value)
             # 如果是 列表 或者 字典，且递归为真，则递归处理
-            if recursive and value and (isinstance(value, dict) or attr.type_string == 'List[dict]'):
+            if recursive and not_null(value) and (isinstance(value, dict) or attr.type_string == 'List[dict]'):
                 nice_cls_name = self.get_nice_cls_name(attr.ok_name, level)
                 if isinstance(value, dict):
                     attr.type_string = nice_cls_name
                 elif attr.type_string == 'List[dict]':
                     self.imports.List = True
                     attr.type_string = f'List[{nice_cls_name}]'
                 # 递归处理
-                obj.classes.append(self.gen_datclass(value, nice_cls_name, recursive=True, level=level + 1))
+                obj.classes.append(self.gen_datclass(value, nice_cls_name, recursive=True, sort=sort, level=level + 1))
             # 如果类型是 Dict，则导入 Dict
             if attr.type_string == 'Dict':
                 self.imports.Dict = True
             if attr.type_string.startswith('List'):
                 self.imports.List = True
             # 如果默认值有 field，则导入 field
             if attr.default_string.startswith('field'):
                 self.imports.field = True
             obj.attr_list.append(attr)
         return obj
 
-    def gen_typed_dict(self, dat: Union[list, dict], name='Object', recursive=False, level=0) -> DictClass:
+    def gen_typed_dict(self, dat: Union[list, dict], name='Object', recursive=True, sort=True, level=0) -> DictClass:
         """生成 "Response = TypedDict('Response', {'update_id': int, 'message': Message})" 形式的字典约束（代码提示）类"""
+        assert dat
         try:
             dat = merge_list_dict(dat)
-        except TypeError:
+        except TypeError as e:
             pass
         self.imports.TypedDict = True
-        obj = DictClass(name=name)
+        obj = DictClass(name=name, sort=sort)
         for name, value in dat.items():
             attr = DictAttr(name, value)
-            if recursive and value and (isinstance(value, dict) or attr.type_string == 'List[dict]'):
+            if recursive and not_null(value) and (isinstance(value, dict) or attr.type_string == 'List[dict]'):
                 nice_cls_name = self.get_nice_cls_name(get_ok_identifier(name), level)
                 if isinstance(value, dict):
                     attr.type_string = nice_cls_name
                 elif attr.type_string == 'List[dict]':
                     attr.type_string = f'List[{nice_cls_name}]'
-                obj.classes.append(self.gen_typed_dict(value, nice_cls_name, recursive=True, level=level + 1))
+                obj.classes.append(
+                    self.gen_typed_dict(value, nice_cls_name, recursive=True, sort=sort, level=level + 1))
             if attr.type_string == 'Dict':
                 self.imports.Dict = True
             if attr.type_string.startswith('List'):
                 self.imports.List = True
             obj.attr_list.append(attr)
         return obj
```

### Comparing `datclass-0.1.9/src/datclass/utils.py` & `datclass-0.2.0/src/datclass/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 
 def get_ok_identifier(name: str):
     # 查询缓存
     if name in _NAME_MAP:
         return _NAME_MAP[name]
 
+    # 处理双(多)下划线开头字段，替换为一个
+    if name.startswith('__'):
+        name = '_' + name.lstrip('_')
+
     # 如果是关键字，则加 '_' 后缀
     if keyword.iskeyword(name):
         s = f'{name}_'
     elif name.isidentifier():
         # 关键字是合法标识符，所以先判断关键字，再判断标识符
         s = name
     else:
@@ -82,22 +86,40 @@
         return 'Dict'
     if get_origin(t) is list:
         st = get_args(t)
         return f'List[{get_type_string(st[0])}]' if st and not isinstance(None, st) else 'List'
     return t.__name__
 
 
+def not_null(value):
+    """[{}] [] {}"""
+    if value:
+        if isinstance(value, list) and not any(value):
+            return False
+        return True
+    return False
+
+
 def merge_list_dict(list_dict: List[dict]) -> Dict:
     if not isinstance(list_dict, list):
         raise TypeError(f'({list_dict}) is not list_dict')
     d = {}
     for i in list_dict:
         if not isinstance(i, dict):
             raise TypeError(f'element({i}) of list_dict is not dict')
         for k, v in i.items():
             if k not in d:
                 d[k] = v
-            elif d[k] and isinstance(v, dict):
-                d[k] = merge_list_dict([d[k], v])
-            elif not d[k] and v:
+                continue
+            if d[k] is None:
                 d[k] = v
+                continue
+            if isinstance(v, dict):
+                d[k] = merge_list_dict([d[k], v])
+                continue
+            if isinstance(d[k], list) and isinstance(v, list):
+                try:
+                    ld = d[k] + v
+                    d[k] = [merge_list_dict(ld)]
+                except TypeError as e:
+                    pass
     return d
```

### Comparing `datclass-0.1.9/src/datclass.egg-info/PKG-INFO` & `datclass-0.2.0/src/datclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.1.9
+Version: 0.2.0
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

