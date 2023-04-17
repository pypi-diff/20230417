# Comparing `tmp/atlas-consortia-commons-1.0.2.tar.gz` & `tmp/atlas-consortia-commons-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-consortia-commons-1.0.2.tar", last modified: Fri Mar 24 14:39:58 2023, max compression
+gzip compressed data, was "atlas-consortia-commons-1.0.3.tar", last modified: Mon Apr 17 14:53:23 2023, max compression
```

## Comparing `atlas-consortia-commons-1.0.2.tar` & `atlas-consortia-commons-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.433031 atlas-consortia-commons-1.0.2/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1374 2023-03-24 14:39:58.432545 atlas-consortia-commons-1.0.2/PKG-INFO
--rw-r--r--   0 maxsibilla   (503) staff       (20)      910 2023-03-21 17:48:33.000000 atlas-consortia-commons-1.0.2/README.md
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.400009 atlas-consortia-commons-1.0.2/atlas_consortia_commons/
--rw-r--r--   0 maxsibilla   (503) staff       (20)        0 2023-03-15 17:35:40.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.418066 atlas-consortia-commons-1.0.2/atlas_consortia_commons/file/
--rw-r--r--   0 maxsibilla   (503) staff       (20)      535 2023-03-17 17:41:40.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/file/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.421764 atlas-consortia-commons-1.0.2/atlas_consortia_commons/object/
--rw-r--r--   0 maxsibilla   (503) staff       (20)      944 2023-03-21 17:48:46.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/object/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.425925 atlas-consortia-commons-1.0.2/atlas_consortia_commons/rest/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     3539 2023-03-21 14:58:41.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/rest/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.427051 atlas-consortia-commons-1.0.2/atlas_consortia_commons/string/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1385 2023-03-24 14:39:19.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/string/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.431674 atlas-consortia-commons-1.0.2/atlas_consortia_commons/ubkg/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     3052 2023-03-21 17:48:46.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons/ubkg/__init__.py
-drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-03-24 14:39:58.414174 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1374 2023-03-24 14:39:58.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/PKG-INFO
--rw-r--r--   0 maxsibilla   (503) staff       (20)      497 2023-03-24 14:39:58.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/SOURCES.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)        1 2023-03-24 14:39:58.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/dependency_links.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)      147 2023-03-24 14:39:58.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/requires.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)       24 2023-03-24 14:39:58.000000 atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/top_level.txt
--rw-r--r--   0 maxsibilla   (503) staff       (20)       38 2023-03-24 14:39:58.433156 atlas-consortia-commons-1.0.2/setup.cfg
--rw-r--r--   0 maxsibilla   (503) staff       (20)     1669 2023-03-24 14:39:54.000000 atlas-consortia-commons-1.0.2/setup.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.370784 atlas-consortia-commons-1.0.3/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1374 2023-04-17 14:53:23.370270 atlas-consortia-commons-1.0.3/PKG-INFO
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      910 2023-03-21 17:48:33.000000 atlas-consortia-commons-1.0.3/README.md
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.345009 atlas-consortia-commons-1.0.3/atlas_consortia_commons/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)        0 2023-03-15 17:35:40.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.359103 atlas-consortia-commons-1.0.3/atlas_consortia_commons/file/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      535 2023-03-17 17:41:40.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/file/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.360006 atlas-consortia-commons-1.0.3/atlas_consortia_commons/object/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1725 2023-04-17 14:52:57.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/object/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.364258 atlas-consortia-commons-1.0.3/atlas_consortia_commons/rest/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     3539 2023-03-21 14:58:41.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/rest/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.365151 atlas-consortia-commons-1.0.3/atlas_consortia_commons/string/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1466 2023-04-17 14:52:57.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/string/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.369418 atlas-consortia-commons-1.0.3/atlas_consortia_commons/ubkg/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     3052 2023-03-21 17:48:46.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons/ubkg/__init__.py
+drwxr-xr-x   0 maxsibilla   (503) staff       (20)        0 2023-04-17 14:53:23.355643 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1374 2023-04-17 14:53:22.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/PKG-INFO
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      497 2023-04-17 14:53:23.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)        1 2023-04-17 14:53:22.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)      147 2023-04-17 14:53:22.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/requires.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)       24 2023-04-17 14:53:22.000000 atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/top_level.txt
+-rw-r--r--   0 maxsibilla   (503) staff       (20)       38 2023-04-17 14:53:23.370941 atlas-consortia-commons-1.0.3/setup.cfg
+-rw-r--r--   0 maxsibilla   (503) staff       (20)     1715 2023-04-17 14:52:57.000000 atlas-consortia-commons-1.0.3/setup.py
```

### Comparing `atlas-consortia-commons-1.0.2/PKG-INFO` & `atlas-consortia-commons-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-commons
-Version: 1.0.2
+Version: 1.0.3
 Summary: The common code supporting the web services in the consortia.
 Home-page: https://github.com/x-atlas-consortia/commons
 Author: Atlas Consortia
 Author-email: api-developers@hubmapconsortium.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atlas-consortia-commons-1.0.2/README.md` & `atlas-consortia-commons-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons/file/__init__.py` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons/file/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons/object/__init__.py` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons/object/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,54 @@
 import enum
 from typing import Union
-from atlas_consortia_commons.string import to_snake_case
+from atlas_consortia_commons.string import to_snake_case_upper, equals
 
 
-def build_enum_class(class_name: str, data: Union[list, dict], key: str = None, val_callback=None,
-                     obj_type: str = 'class'):
+def build_enum_class(class_name: str, data: Union[list, dict], prop_key: str = None, val_key: str = None,
+                     prop_callback=to_snake_case_upper, val_callback=None,
+                     obj_type: str = 'class', data_as_val: bool = False):
     _props = {}
+
+    if val_key is None:
+        val_key = prop_key
+
+    def _populate_props(_item):
+        prop = _item.get(prop_key)
+        val = _item if data_as_val is True else _item.get(val_key)
+        prop = prop if prop_callback is None else prop_callback(prop)
+        _props[prop] = val if val_callback is None else val_callback(val)
+
     try:
         if type(data) is list:
             for item in data:
-                val = item.get(key)
-                prop = to_snake_case(val).upper()
-                _props[prop] = val if val_callback is None else val_callback(val)
+                _populate_props(item)
         else:
-            if key is not None:
-                val = data.get(key)
-                prop = to_snake_case(val).upper()
-                _props[prop] = val if val_callback is None else val_callback(val)
+            if prop_key is not None:
+                _populate_props(data)
             else:
                 _props = data
-        if obj_type == 'enum':
+
+        if equals(obj_type, 'enum'):
             return enum.Enum(class_name, _props)
+        elif equals(obj_type, 'dict'):
+            return _props
+        elif equals(obj_type, 'list'):
+            return list(_props.keys())
         else:
             return type(class_name, (), _props)
     except Exception as e:
         print(e)
+
+
+def includes(data, keyword, as_list=True, insensitive=True, single_index=False):
+    results = []
+    for i, val in enumerate(data):
+        if equals(val, keyword, insensitive):
+            if as_list is True:
+                results.append(i)
+            else:
+                return True
+
+    if as_list and single_index:
+        return results[0] if len(results) > 0 else -1
+
+    return results if as_list is True else False
```

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons/rest/__init__.py` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons/string/__init__.py` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons/string/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         return _val.replace(' ', '_')
 
 
 def to_snake_case(val) -> str:
     return _to_case(val, 'snake')
 
 
+def to_snake_case_upper(val) -> str:
+    return _to_case(val, 'snake').upper()
+
+
 def to_pascal_case(val) -> str:
     return _to_case(val, 'pascal')
 
 
 def to_camel_case(val) -> str:
     return _to_case(val, 'camel')
```

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons/ubkg/__init__.py` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons/ubkg/__init__.py`

 * *Files identical despite different names*

### Comparing `atlas-consortia-commons-1.0.2/atlas_consortia_commons.egg-info/PKG-INFO` & `atlas-consortia-commons-1.0.3/atlas_consortia_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-consortia-commons
-Version: 1.0.2
+Version: 1.0.3
 Summary: The common code supporting the web services in the consortia.
 Home-page: https://github.com/x-atlas-consortia/commons
 Author: Atlas Consortia
 Author-email: api-developers@hubmapconsortium.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atlas-consortia-commons-1.0.2/setup.py` & `atlas-consortia-commons-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="atlas-consortia-commons",
-    version="1.0.2",
+    # Test PyPi version
+    # version="1.0.4"
+    version="1.0.3",
     author="Atlas Consortia",
     author_email="api-developers@hubmapconsortium.org",
     description="The common code supporting the web services in the consortia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/x-atlas-consortia/commons",
     packages=['atlas_consortia_commons',
```

