# Comparing `tmp/grai_source_flat_file-0.0.6.tar.gz` & `tmp/grai_source_flat_file-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_flat_file-0.0.6.tar", max compression
+gzip compressed data, was "grai_source_flat_file-0.0.7.tar", max compression
```

## Comparing `grai_source_flat_file-0.0.6.tar` & `grai_source_flat_file-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      680 2023-01-26 15:48:22.525277 grai_source_flat_file-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      147 2023-01-18 14:35:11.044204 grai_source_flat_file-0.0.6/src/grai_source_flat_file/__init__.py
--rw-r--r--   0        0        0     4277 2023-01-25 21:51:43.347879 grai_source_flat_file-0.0.6/src/grai_source_flat_file/adapters.py
--rw-r--r--   0        0        0      834 2023-01-25 21:51:43.311940 grai_source_flat_file-0.0.6/src/grai_source_flat_file/base.py
--rw-r--r--   0        0        0     1828 2023-01-18 14:35:11.044543 grai_source_flat_file-0.0.6/src/grai_source_flat_file/loader.py
--rw-r--r--   0        0        0      978 2023-01-18 14:35:11.044629 grai_source_flat_file-0.0.6/src/grai_source_flat_file/models.py
--rw-r--r--   0        0        0      150 2023-01-18 14:35:11.044676 grai_source_flat_file-0.0.6/src/grai_source_flat_file/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.6/setup.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      713 2023-04-17 19:09:03.818104 grai_source_flat_file-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-02-13 20:16:22.718033 grai_source_flat_file-0.0.7/src/grai_source_flat_file/__init__.py
+-rw-r--r--   0        0        0     4323 2023-04-17 19:09:03.818263 grai_source_flat_file-0.0.7/src/grai_source_flat_file/adapters.py
+-rw-r--r--   0        0        0      834 2023-02-13 20:16:22.718432 grai_source_flat_file-0.0.7/src/grai_source_flat_file/base.py
+-rw-r--r--   0        0        0     2029 2023-04-17 19:09:03.818417 grai_source_flat_file-0.0.7/src/grai_source_flat_file/loader.py
+-rw-r--r--   0        0        0      978 2023-02-13 20:16:22.718610 grai_source_flat_file-0.0.7/src/grai_source_flat_file/models.py
+-rw-r--r--   0        0        0      188 2023-02-13 20:16:22.718657 grai_source_flat_file-0.0.7/src/grai_source_flat_file/package_definitions.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.7/setup.py
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 grai_source_flat_file-0.0.7/PKG-INFO
```

### Comparing `grai_source_flat_file-0.0.6/pyproject.toml` & `grai_source_flat_file-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [tool.poetry]
 name = "grai_source_flat_file"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_flat_file", from = "src" },
 ]
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 PyYAML = "^6.0"
 multimethod = "^1.8"
 pandas = "^1.4.4"
-grai-schemas = "^0.1.5"
+grai-schemas = "^0.1.10"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 pytest = "^7.2.0"
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_source_flat_file"
 
+[tool.black]
+line-length = 120
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grai_source_flat_file-0.0.6/src/grai_source_flat_file/adapters.py` & `grai_source_flat_file-0.0.7/src/grai_source_flat_file/adapters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,109 +1,101 @@
 from typing import Any, Dict, List, Literal, Sequence, Type, Union
 
 from grai_client.schemas.schema import Schema
 from grai_schemas import config as base_config
 from grai_schemas.generics import DefaultValue
-from grai_schemas.v1.metadata.edges import EdgeTypeLabels, GenericEdgeMetadataV1
+from grai_schemas.v1.metadata.edges import EdgeTypeLabels, TableToColumnMetadata
 from grai_schemas.v1.metadata.nodes import ColumnMetadata, NodeTypeLabels, TableMetadata
 from multimethod import multimethod
 
 from grai_source_flat_file.models import ID, Column, Edge, Table
 from grai_source_flat_file.package_definitions import config
 
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_column(
-    current: Column, version: Literal["v1"] = "v1"
-) -> ColumnMetadata:
+def build_grai_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> ColumnMetadata:
     data = {
         "version": version,
         "node_type": NodeTypeLabels.column.value,
         "node_attributes": {
             "data_type": current.data_type,
             "is_nullable": current.is_nullable,
         },
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_node(
-    current: Table, version: Literal["v1"] = "v1"
-) -> TableMetadata:
+def build_grai_metadata_from_node(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     data = {
         "version": version,
         "node_type": NodeTypeLabels.table.value,
         "node_attributes": {},
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(
-    current: Edge, version: Literal["v1"] = "v1"
-) -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> TableToColumnMetadata:
     data = {
         "version": version,
     }
-    return GenericEdgeMetadataV1(edge_type=EdgeTypeLabels.generic.value, **data)
+    return TableToColumnMetadata(edge_type=EdgeTypeLabels.table_to_column.value, **data)
 
 
 @multimethod
-def build_flat_file_metadata(current: Any, desired: Any) -> None:
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+def build_app_metadata(current: Any, desired: Any) -> None:
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
-@build_flat_file_metadata.register
+@build_app_metadata.register
 def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "table_name": current.table,
     }
     return data
 
 
-@build_flat_file_metadata.register
+@build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
     data = {}
     return data
 
 
-@build_flat_file_metadata.register
+@build_app_metadata.register
 def build_metadata_from_node(current: Table, version: Literal["v1"] = "v1") -> Dict:
     data = {"file_name": current.file_name}
     return data
 
 
 def build_metadata(obj, version):
+    integration_meta = build_app_metadata(obj, version)
+    base_metadata = build_grai_metadata(obj, version)
+    integration_meta["grai"] = base_metadata
+
     return {
-        base_config.metadata_id: build_grai_metadata(obj, version),
-        config.metadata_id: build_flat_file_metadata(obj, version),
+        base_config.metadata_id: base_metadata,
+        config.metadata_id: integration_meta,
     }
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any):
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_column_to_client(
-    current: Union[Table, Column], version: Literal["v1"] = "v1"
-):
+def adapt_column_to_client(current: Union[Table, Column], version: Literal["v1"] = "v1"):
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
```

### Comparing `grai_source_flat_file-0.0.6/src/grai_source_flat_file/base.py` & `grai_source_flat_file-0.0.7/src/grai_source_flat_file/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.6/src/grai_source_flat_file/models.py` & `grai_source_flat_file-0.0.7/src/grai_source_flat_file/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_flat_file-0.0.6/setup.py` & `grai_source_flat_file-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'grai-client>=0.2.0,<0.3.0',
- 'grai-schemas>=0.1.5,<0.2.0',
+ 'grai-schemas>=0.1.10,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pandas>=1.4.4,<2.0.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-flat-file',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_flat_file-0.0.6/PKG-INFO` & `grai_source_flat_file-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: grai-source-flat-file
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: grai-client (>=0.2.0,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.5,<0.2.0)
+Requires-Dist: grai-schemas (>=0.1.10,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
```

