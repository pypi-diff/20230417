# Comparing `tmp/rframe-0.2.7.tar.gz` & `tmp/rframe-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rframe-0.2.7.tar", max compression
+gzip compressed data, was "rframe-0.2.8.tar", max compression
```

## Comparing `rframe-0.2.7.tar` & `rframe-0.2.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1073 2023-04-13 18:31:23.906425 rframe-0.2.7/LICENSE
--rw-r--r--   0        0        0     1026 2023-04-13 18:31:23.906425 rframe-0.2.7/README.rst
--rw-r--r--   0        0        0     3021 2023-04-13 18:31:23.910425 rframe-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      618 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/__init__.py
--rw-r--r--   0        0        0     2809 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/_hypothesis_plugin.py
--rw-r--r--   0        0        0     6601 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/data_accessor.py
--rw-r--r--   0        0        0     1026 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/dispatchers.py
--rw-r--r--   0        0        0      212 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/__init__.py
--rw-r--r--   0        0        0     2610 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/base.py
--rw-r--r--   0        0        0       63 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/index.py
--rw-r--r--   0        0        0     3205 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/interpolating_index.py
--rw-r--r--   0        0        0     1245 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/interval_index.py
--rw-r--r--   0        0        0     1999 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/multi_index.py
--rw-r--r--   0        0        0      472 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/base.py
--rw-r--r--   0        0        0    10732 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/json.py
--rw-r--r--   0        0        0    27454 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/mongo.py
--rw-r--r--   0        0        0    12136 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/pandas.py
--rw-r--r--   0        0        0     3852 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/rest.py
--rw-r--r--   0        0        0    11551 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/tinydb.py
--rw-r--r--   0        0        0     6290 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rest_client.py
--rw-r--r--   0        0        0    14218 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rest_server.py
--rw-r--r--   0        0        0    13145 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rframe.py
--rw-r--r--   0        0        0    19976 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/schema.py
--rw-r--r--   0        0        0     5516 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/types.py
--rw-r--r--   0        0        0     7529 2023-04-13 18:31:23.914425 rframe-0.2.7/rframe/utils.py
--rw-r--r--   0        0        0       36 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_basics.py
--rw-r--r--   0        0        0     1948 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_json.py
--rw-r--r--   0        0        0     3306 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_mongo.py
--rw-r--r--   0        0        0     2514 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_pandas.py
--rw-r--r--   0        0        0     3510 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_rest.py
--rw-r--r--   0        0        0     9442 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_schemas.py
--rw-r--r--   0        0        0     2297 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_tinydb.py
--rw-r--r--   0        0        0      478 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_utils.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-17 17:02:35.949450 rframe-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1026 2023-04-17 17:02:35.949450 rframe-0.2.8/README.rst
+-rw-r--r--   0        0        0     3021 2023-04-17 17:02:35.949450 rframe-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      618 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/__init__.py
+-rw-r--r--   0        0        0     2809 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     6927 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/data_accessor.py
+-rw-r--r--   0        0        0     1026 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/dispatchers.py
+-rw-r--r--   0        0        0      212 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/__init__.py
+-rw-r--r--   0        0        0     2610 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/base.py
+-rw-r--r--   0        0        0       63 2023-04-17 17:02:35.949450 rframe-0.2.8/rframe/indexes/index.py
+-rw-r--r--   0        0        0     3205 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/interpolating_index.py
+-rw-r--r--   0        0        0     1245 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/interval_index.py
+-rw-r--r--   0        0        0     1999 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/indexes/multi_index.py
+-rw-r--r--   0        0        0      472 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/base.py
+-rw-r--r--   0        0        0    10732 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/json.py
+-rw-r--r--   0        0        0    27454 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/mongo.py
+-rw-r--r--   0        0        0    12136 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/pandas.py
+-rw-r--r--   0        0        0     3852 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/rest.py
+-rw-r--r--   0        0        0    11551 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/interfaces/tinydb.py
+-rw-r--r--   0        0        0     6290 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rest_client.py
+-rw-r--r--   0        0        0    14218 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rest_server.py
+-rw-r--r--   0        0        0    13145 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/rframe.py
+-rw-r--r--   0        0        0    19976 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/schema.py
+-rw-r--r--   0        0        0     5516 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/types.py
+-rw-r--r--   0        0        0     7529 2023-04-17 17:02:35.953450 rframe-0.2.8/rframe/utils.py
+-rw-r--r--   0        0        0       36 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_basics.py
+-rw-r--r--   0        0        0     1948 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_json.py
+-rw-r--r--   0        0        0     3306 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_mongo.py
+-rw-r--r--   0        0        0     2514 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_pandas.py
+-rw-r--r--   0        0        0     3510 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_rest.py
+-rw-r--r--   0        0        0     9442 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_schemas.py
+-rw-r--r--   0        0        0     2297 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_tinydb.py
+-rw-r--r--   0        0        0      478 2023-04-17 17:02:35.953450 rframe-0.2.8/tests/test_utils.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.8/PKG-INFO
```

### Comparing `rframe-0.2.7/LICENSE` & `rframe-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/README.rst` & `rframe-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/pyproject.toml` & `rframe-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rframe"
-version = "0.2.7"
+version = "0.2.8"
 homepage = "https://github.com/jmosbacher/rframe"
 description = "Top-level package for rframe."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `rframe-0.2.7/rframe/__init__.py` & `rframe-0.2.8/rframe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for rframe."""
 
 __author__ = """Yossi Mosbacher"""
 __email__ = "joe.mosbacher@gmail.com"
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 from loguru import logger
 
 from . import schema, indexes, utils, dispatchers
 
 from .indexes import Index, InterpolatingIndex, IntervalIndex
 from .types import Interval, IntegerInterval, TimeInterval
```

### Comparing `rframe-0.2.7/rframe/_hypothesis_plugin.py` & `rframe-0.2.8/rframe/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/data_accessor.py` & `rframe-0.2.8/rframe/data_accessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,57 +55,59 @@
 
     def _find(
         self, skip=None, limit=None, sort=None, **labels
     ) -> Generator[dict, None, None]:
         """Internal find function, performs data validation but
         returns raw dicts, not schema instances.
         """
+        labels = {k: v for k, v in labels.items() if v is not None}
         query = self.schema.compile_query(datasource=self.storage, **labels)
         for doc in query.iter(limit=limit, skip=skip, sort=sort):
             try:
                 doc = self.schema(**doc).dict()
             except ValidationError:
                 continue
             yield doc
 
     def _find_dicts(self, skip=None, limit=None, sort=None, **labels):
-        return list(self.find(skip=skip, limit=limit, sort=sort, **labels))
+        return list(self._find(skip=skip, limit=limit, sort=sort, **labels))
 
     def _find_docs(self, skip=None, limit=None, sort=None, **labels):
-        return list(self.find_iter(skip=skip, limit=limit, sort=sort, **labels))
+        return list(self._find_iter(skip=skip, limit=limit, sort=sort, **labels))
 
     def _find_iter(self, skip=None, limit=None, sort=None, **labels):
         for doc in self._find(skip=skip, limit=limit, sort=sort, **labels):
             yield self.schema(**doc)
 
-    def _find_df(self, skip=None, limit=None, sort=None, **labels) -> pd.DateOffset:
+    def _find_df(self, skip=None, limit=None, sort=None, **labels) -> pd.DataFrame:
         docs = [
             to_pandas(d)
             for d in self._find_dicts(skip=skip, limit=limit, sort=sort, **labels)
         ]
         df = pd.json_normalize(docs)
         if not len(df):
             df = df.reindex(columns=list(self.schema.__fields__))
         index_fields = list(self.schema.get_index_fields())
         if len(index_fields) == 1:
             index_fields = index_fields[0]
         return df.set_index(index_fields)
 
     def _find_one(self, skip=None, sort=None, **labels) -> Optional["BaseSchema"]:
-        docs = self.find_docs(skip=skip, limit=1, sort=sort, **labels)
+        docs = self._find_docs(skip=skip, limit=1, sort=sort, **labels)
         if docs:
             return docs[0]
         return None
 
     def _min(self, fields=None, **labels) -> Any:
         if fields is None:
             fields = list(self.schema.__fields__)
         elif isinstance(fields, str):
             fields = [fields]
         
+        labels = {k: v for k, v in labels.items() if v is not None}
         query = self.schema.compile_query(self.storage, **labels)
 
         result = query.min(fields)
         if isinstance(result, dict):
             result = { k: self.schema.validate_partial(**{k: v})
                         for k,v in result.items() }
         else:
@@ -113,15 +115,16 @@
         return result
 
     def _max(self, fields=None, **labels) -> Any:
         if fields is None:
             fields = list(self.schema.__fields__)
         elif isinstance(fields, str):
             fields = [fields]
-        
+
+        labels = {k: v for k, v in labels.items() if v is not None}
         query = self.schema.compile_query(self.storage, **labels)
 
         result = query.max(fields)
         if isinstance(result, dict):
             result = { k: self.schema.validate_partial(**{k: v})
                         for k,v in result.items() }
         else:
@@ -129,26 +132,28 @@
         return result
 
     def _unique(self, fields=None, **labels) -> Any:
         if fields is None:
             fields = list(self.schema.__fields__)
         elif isinstance(fields, str):
             fields = [fields]
-        
+
+        labels = {k: v for k, v in labels.items() if v is not None}
         query = self.schema.compile_query(self.storage, **labels)
 
         result = query.unique(fields)
         if isinstance(result, dict):
             result = { k: [self.schema.validate_partial(**{k: v}) for v in vs]
                         for k, vs in result.items() }
         else:
             result = [self.schema.validate_partial(**{fields[0]: v}) for v in result]
         return result
 
     def _count(self, **labels):
+        labels = {k: v for k, v in labels.items() if v is not None}
         query = self.schema.compile_query(self.storage, **labels)
         return int(query.count())
 
     def insert(self, docs, raise_on_error=True):
         if not self.initialized:
             self.initdb()
```

### Comparing `rframe-0.2.7/rframe/dispatchers.py` & `rframe-0.2.8/rframe/dispatchers.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/indexes/base.py` & `rframe-0.2.8/rframe/indexes/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/indexes/interpolating_index.py` & `rframe-0.2.8/rframe/indexes/interpolating_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/indexes/interval_index.py` & `rframe-0.2.8/rframe/indexes/interval_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/indexes/multi_index.py` & `rframe-0.2.8/rframe/indexes/multi_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/base.py` & `rframe-0.2.8/rframe/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/json.py` & `rframe-0.2.8/rframe/interfaces/json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/mongo.py` & `rframe-0.2.8/rframe/interfaces/mongo.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/pandas.py` & `rframe-0.2.8/rframe/interfaces/pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/rest.py` & `rframe-0.2.8/rframe/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/interfaces/tinydb.py` & `rframe-0.2.8/rframe/interfaces/tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/rest_client.py` & `rframe-0.2.8/rframe/rest_client.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/rest_server.py` & `rframe-0.2.8/rframe/rest_server.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/rframe.py` & `rframe-0.2.8/rframe/rframe.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/schema.py` & `rframe-0.2.8/rframe/schema.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/types.py` & `rframe-0.2.8/rframe/types.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/rframe/utils.py` & `rframe-0.2.8/rframe/utils.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_basics.py` & `rframe-0.2.8/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_json.py` & `rframe-0.2.8/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_mongo.py` & `rframe-0.2.8/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_pandas.py` & `rframe-0.2.8/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_rest.py` & `rframe-0.2.8/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_schemas.py` & `rframe-0.2.8/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/tests/test_tinydb.py` & `rframe-0.2.8/tests/test_tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.7/PKG-INFO` & `rframe-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rframe
-Version: 0.2.7
+Version: 0.2.8
 Summary: Top-level package for rframe.
 Home-page: https://github.com/jmosbacher/rframe
 License: MIT
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

