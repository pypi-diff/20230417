# Comparing `tmp/grai_source_bigquery-0.0.2.tar.gz` & `tmp/grai_source_bigquery-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.0.2.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.0.3.tar", max compression
```

## Comparing `grai_source_bigquery-0.0.2.tar` & `grai_source_bigquery-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      738 2023-03-24 13:30:45.027370 grai_source_bigquery-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.2/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     6422 2023-03-23 17:27:33.945151 grai_source_bigquery-0.0.2/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.2/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.2/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     4778 2023-03-23 17:24:29.958913 grai_source_bigquery-0.0.2/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.2/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.2/setup.py
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      738 2023-04-17 19:09:03.810095 grai_source_bigquery-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-13 20:16:22.712224 grai_source_bigquery-0.0.3/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     6553 2023-04-17 19:09:03.810266 grai_source_bigquery-0.0.3/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     1192 2023-02-13 20:16:22.712633 grai_source_bigquery-0.0.3/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0     5547 2023-02-13 20:16:22.712831 grai_source_bigquery-0.0.3/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     4778 2023-04-13 22:32:27.123660 grai_source_bigquery-0.0.3/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      186 2023-02-13 20:16:22.713174 grai_source_bigquery-0.0.3/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.3/setup.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 grai_source_bigquery-0.0.3/PKG-INFO
```

### Comparing `grai_source_bigquery-0.0.2/pyproject.toml` & `grai_source_bigquery-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_bigquery-0.0.2/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.0.3/src/grai_source_bigquery/adapters.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,29 +9,30 @@
     EdgeTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
     TableToTableMetadata,
 )
 from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeTypeLabels, TableMetadata
 from multimethod import multimethod
+from pydantic import BaseModel
 
 from grai_source_bigquery.models import (
     ID,
     Column,
     ColumnID,
     Constraint,
     Edge,
     Table,
     TableID,
 )
 from grai_source_bigquery.package_definitions import config
 
 
 @multimethod
-def build_grai_metadata(current: Any, desired: Any) -> None:
+def build_grai_metadata(current: Any, desired: Any) -> BaseModel:
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
 def build_grai_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> ColumnMetadata:
     default_value = current.default_value
     if current.default_value is not None:
@@ -86,55 +87,59 @@
     return GenericEdgeMetadataV1(**data)
 
 
 # ---
 
 
 @multimethod
-def build_bigquery_metadata(current: Any, desired: Any) -> None:
+def build_app_metadata(current: Any, desired: Any) -> None:
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
-@build_bigquery_metadata.register
+@build_app_metadata.register
 def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "table_name": current.table,
         "schema": current.column_schema,
     }
 
     return data
 
 
-@build_bigquery_metadata.register
+@build_app_metadata.register
 def build_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "schema": current.table_schema,
         "table_type": current.table_type.value,
     }
     return data
 
 
-@build_bigquery_metadata.register
+@build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "definition": current.definition,
         "constraint_type": current.constraint_type.value,
     }
     data |= current.metadata if current.metadata is not None else {}
 
     return data
 
 
 # ---
 
 
 def build_metadata(obj, version):
+    integration_meta = build_app_metadata(obj, version)
+    base_metadata = build_grai_metadata(obj, version)
+    integration_meta["grai"] = base_metadata
+
     return {
-        base_config.metadata_id: build_grai_metadata(obj, version),
-        config.metadata_id: build_bigquery_metadata(obj, version),
+        base_config.metadata_id: base_metadata,
+        config.metadata_id: integration_meta,
     }
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any) -> Union[NodeV1, EdgeV1]:
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
```

### Comparing `grai_source_bigquery-0.0.2/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.0.3/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.2/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.0.3/src/grai_source_bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.2/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.0.3/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.0.2/setup.py` & `grai_source_bigquery-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'grai-schemas>=0.1.9,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'setuptools>=67.1.0,<68.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-bigquery',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': 'None',
     'author': 'Edward Louth',
     'author_email': 'edward@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_bigquery-0.0.2/PKG-INFO` & `grai_source_bigquery-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

