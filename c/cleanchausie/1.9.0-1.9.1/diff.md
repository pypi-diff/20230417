# Comparing `tmp/cleanchausie-1.9.0.tar.gz` & `tmp/cleanchausie-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanchausie-1.9.0.tar", last modified: Tue Mar  7 16:35:23 2023, max compression
+gzip compressed data, was "cleanchausie-1.9.1.tar", last modified: Thu Mar  9 12:55:10 2023, max compression
```

## Comparing `cleanchausie-1.9.0.tar` & `cleanchausie-1.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1094 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     3541 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2304 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie/
--rw-r--r--   0 runner    (1000) runner    (1000)     1370 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/consts.py
--rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/errors.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie/ext/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/ext/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3887 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/ext/attrs.py
--rw-r--r--   0 runner    (1000) runner    (1000)      620 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/ext/pytz.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie/fields/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7411 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/field.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1207 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/type_map.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie/fields/types/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      373 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/bools.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1338 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/datetimes.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1675 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/dicts.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1328 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/enums.py
--rw-r--r--   0 runner    (1000) runner    (1000)      448 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/instances.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1882 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/lists.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1445 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/nested.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1392 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/numbers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6354 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/polymorphic.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4758 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/types/strings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1756 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/utils.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7292 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/fields/validation.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2075 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/interface.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie/mypy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/mypy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8118 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/mypy/plugin.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/py.typed
--rw-r--r--   0 runner    (1000) runner    (1000)     9546 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/schema.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4294 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/schema_definition.py
--rw-r--r--   0 runner    (1000) runner    (1000)      548 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/cleanchausie/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-07 16:35:23.217091 cleanchausie-1.9.0/cleanchausie.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3541 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1164 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)       39 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-03-07 16:35:23.000000 cleanchausie-1.9.0/cleanchausie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      281 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      713 2023-03-07 16:35:23.221092 cleanchausie-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1454 2023-03-07 16:35:14.000000 cleanchausie-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1094 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     3541 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2304 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.916055 cleanchausie-1.9.1/cleanchausie/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1370 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/consts.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/errors.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/cleanchausie/ext/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/ext/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3887 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/ext/attrs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      620 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/ext/pytz.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/cleanchausie/fields/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7411 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/field.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1207 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/type_map.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/cleanchausie/fields/types/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      373 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/bools.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1338 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/datetimes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1675 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/dicts.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1328 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/enums.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      448 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/instances.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1882 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/lists.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1445 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/nested.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1392 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/numbers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6568 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/polymorphic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4758 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/types/strings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1756 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/utils.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7292 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/fields/validation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2075 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/interface.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/cleanchausie/mypy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/mypy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8118 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/mypy/plugin.py
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/py.typed
+-rw-r--r--   0 runner    (1000) runner    (1000)     9546 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/schema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4294 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/schema_definition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      548 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/cleanchausie/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-03-09 12:55:10.916055 cleanchausie-1.9.1/cleanchausie.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3541 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1164 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       39 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-03-09 12:55:10.000000 cleanchausie-1.9.1/cleanchausie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      281 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      713 2023-03-09 12:55:10.920055 cleanchausie-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1454 2023-03-09 12:55:00.000000 cleanchausie-1.9.1/setup.py
```

### Comparing `cleanchausie-1.9.0/LICENSE` & `cleanchausie-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/PKG-INFO` & `cleanchausie-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanchausie
-Version: 1.9.0
+Version: 1.9.1
 Summary: Data validation and transformation library for Python. Successor to CleanCat.
 Home-page: http://github.com/closeio/cleanchausie
 Author: Alec Rosenbaum
 Author-email: engineering@close.io
 Maintainer: Alec Rosenbaum
 Maintainer-email: engineering@close.io
 License: MIT
```

### Comparing `cleanchausie-1.9.0/README.md` & `cleanchausie-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/__init__.py` & `cleanchausie-1.9.1/cleanchausie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     "field",
     "OMITTED",
     "omitted",
     "clean",
     "serialize",
 ]
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
```

### Comparing `cleanchausie-1.9.0/cleanchausie/errors.py` & `cleanchausie-1.9.1/cleanchausie/errors.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/ext/attrs.py` & `cleanchausie-1.9.1/cleanchausie/ext/attrs.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/ext/pytz.py` & `cleanchausie-1.9.1/cleanchausie/ext/pytz.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/field.py` & `cleanchausie-1.9.1/cleanchausie/fields/field.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/type_map.py` & `cleanchausie-1.9.1/cleanchausie/fields/type_map.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/datetimes.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/datetimes.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/dicts.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/dicts.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/enums.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/enums.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/lists.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/lists.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/nested.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/nested.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/numbers.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/numbers.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/polymorphic.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/polymorphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,22 @@
             (m for m in mappings if m.public_type == public_type), empty
         )
 
     def _serialize_func(value):
         if value is None:
             return None
         mapping = next(
-            m for m in mappings if isinstance(value, m.internal_type)
+            (m for m in mappings if isinstance(value, m.internal_type)),
+            None,
         )
+        if mapping is None:
+            raise TypeError(
+                f"Value '{value}' is not an instance of any of the "
+                "provided mappings' internal types."
+            )
         result = mapping.serializer(value)
         if isinstance(result, dict):
             result[type_field] = mapping.public_type
         return result
 
     @field(serialize_func=_serialize_func)
     def _polymorphic_field(
```

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/types/strings.py` & `cleanchausie-1.9.1/cleanchausie/fields/types/strings.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/utils.py` & `cleanchausie-1.9.1/cleanchausie/fields/utils.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/fields/validation.py` & `cleanchausie-1.9.1/cleanchausie/fields/validation.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/interface.py` & `cleanchausie-1.9.1/cleanchausie/interface.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/mypy/plugin.py` & `cleanchausie-1.9.1/cleanchausie/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/schema.py` & `cleanchausie-1.9.1/cleanchausie/schema.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/schema_definition.py` & `cleanchausie-1.9.1/cleanchausie/schema_definition.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie/utils.py` & `cleanchausie-1.9.1/cleanchausie/utils.py`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/cleanchausie.egg-info/PKG-INFO` & `cleanchausie-1.9.1/cleanchausie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanchausie
-Version: 1.9.0
+Version: 1.9.1
 Summary: Data validation and transformation library for Python. Successor to CleanCat.
 Home-page: http://github.com/closeio/cleanchausie
 Author: Alec Rosenbaum
 Author-email: engineering@close.io
 Maintainer: Alec Rosenbaum
 Maintainer-email: engineering@close.io
 License: MIT
```

### Comparing `cleanchausie-1.9.0/cleanchausie.egg-info/SOURCES.txt` & `cleanchausie-1.9.1/cleanchausie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/setup.cfg` & `cleanchausie-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cleanchausie-1.9.0/setup.py` & `cleanchausie-1.9.1/setup.py`

 * *Files identical despite different names*

