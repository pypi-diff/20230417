# Comparing `tmp/grai_source_dbt-0.2.6a0.tar.gz` & `tmp/grai_source_dbt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.2.6a0.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.2.7.tar", max compression
```

## Comparing `grai_source_dbt-0.2.6a0.tar` & `grai_source_dbt-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      741 2023-04-12 16:58:27.208366 grai_source_dbt-0.2.6a0/pyproject.toml
--rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.6a0/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     5964 2023-04-10 15:35:17.408407 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      531 2023-04-10 15:35:17.409417 grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     5499 2023-04-12 16:56:50.880225 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.6a0/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.6a0/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/setup.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.6a0/PKG-INFO
+-rw-r--r--   0        0        0      735 2023-04-17 19:17:40.650637 grai_source_dbt-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-02-23 22:53:26.660798 grai_source_dbt-0.2.7/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.2.7/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     5895 2023-04-17 19:09:03.811520 grai_source_dbt-0.2.7/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      531 2023-04-17 19:09:03.811652 grai_source_dbt-0.2.7/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0      802 2023-03-22 16:41:59.040971 grai_source_dbt-0.2.7/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.2.7/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.2.7/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      764 2023-02-23 22:53:26.661735 grai_source_dbt-0.2.7/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     1881 2023-02-23 22:53:26.661938 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      940 2023-02-23 22:53:26.662122 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      199 2023-02-23 22:53:26.662264 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     5368 2023-04-17 19:09:03.812538 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0     1032 2023-02-23 22:53:26.662601 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-02-23 22:53:26.662723 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-02-23 22:53:26.662932 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663082 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-02-23 22:53:26.663291 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2172 2023-02-28 23:36:16.178370 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      549 2023-02-23 22:53:26.663499 grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.2.7/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-28 23:36:16.178561 grai_source_dbt-0.2.7/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2350 2023-02-13 20:16:22.716054 grai_source_dbt-0.2.7/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      176 2023-02-13 20:16:22.716226 grai_source_dbt-0.2.7/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     1893 2023-02-28 23:36:16.178761 grai_source_dbt-0.2.7/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.2.7/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0      981 2023-02-28 23:34:46.003147 grai_source_dbt-0.2.7/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.7/setup.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 grai_source_dbt-0.2.7/PKG-INFO
```

### Comparing `grai_source_dbt-0.2.6a0/pyproject.toml` & `grai_source_dbt-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_dbt"
-version = "0.2.6-alpha"
+version = "0.2.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_dbt", from = "src" },
 ]
```

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/adapters/adapters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Literal, Sequence, Union
 
+from grai_schemas import config as base_config
 from grai_schemas import config as grai_base_config
-from grai_schemas.schema import Schema
 from grai_schemas.v1 import EdgeV1, NodeV1
 from grai_schemas.v1.metadata.edges import (
     ColumnToColumnMetadata,
     EdgeTypeLabels,
     GenericEdgeMetadataV1,
     TableToColumnMetadata,
     TableToTableMetadata,
@@ -67,80 +67,88 @@
     elif current.edge_type == EdgeTypeLabels.table_to_column:
         return TableToColumnMetadata(**data)
     else:
         raise NotImplementedError(f"No supported metadata implementation for edge_type {current.edge_type.value}")
 
 
 @multimethod
-def build_dbt_metadata(current: Any, version: Any) -> None:
+def build_app_metadata(current: Any, version: Any) -> None:
     raise NotImplementedError(
         f"No objects of type `{type(current)}` have an implementation of `build_dbt_metadata` for version `{version}`."
     )
 
 
-@build_dbt_metadata.register
+@build_app_metadata.register
 def build_metadata_from_column(current: Column, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "description": current.description,
         "data_type": current.data_type,
         "dbt_tags": current.tags,
         "table_name": current.table_name,
         "dbt_quote": current.quote,
         "tests": [test.dict() for test in current.tests],
     }
 
     return data
 
 
-@build_dbt_metadata.register
+@build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "definition": current.definition,
         "constraint_type": current.constraint_type.name,
     }
 
     return data
 
 
-@build_dbt_metadata.register
+@build_app_metadata.register
 def build_metadata_from_node(current: AllDbtNodeTypes, version: Literal["v1"] = "v1") -> Dict:
     return current.dict()
 
 
+# ---
+
+
+def build_metadata(obj, version):
+    integration_meta = build_app_metadata(obj, version)
+    base_metadata = build_grai_metadata(obj, version)
+    integration_meta["grai"] = base_metadata
+
+    return {
+        base_config.metadata_id: base_metadata,
+        config.metadata_id: integration_meta,
+    }
+
+
 @multimethod
 def adapt_to_client(current: Any, version: Any) -> None:
     raise NotImplementedError(f"No objects of type `{type(current)}` have a `{version}` client adapter.")
 
 
 @adapt_to_client.register
 def adapt_table_to_client(current: AllDbtNodeTypes, version: Literal["v1"] = "v1") -> NodeV1:
     spec_dict = {
         "name": current.grai_.full_name,
         "namespace": current.grai_.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
-        "metadata": {
-            grai_base_config.metadata_id: build_grai_metadata(current, version),
-            config.metadata_id: build_dbt_metadata(current, version),
-        },
+        "metadata": build_metadata(current, version),
     }
     return NodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
 def adapt_column_to_client(current: Column, version: Literal["v1"] = "v1") -> NodeV1:
     spec_dict = {
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
-        "metadata": {
-            grai_base_config.metadata_id: build_grai_metadata(current, version),
-            config.metadata_id: build_dbt_metadata(current, version),
-        },
+        "metadata": build_metadata(current, version),
     }
 
     return NodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
 def adapt_edge_to_client(current: Edge, version: Literal["v1"] = "v1") -> EdgeV1:
@@ -152,18 +160,15 @@
             "name": current.source.name,
             "namespace": current.source.namespace,
         },
         "destination": {
             "name": current.destination.name,
             "namespace": current.destination.namespace,
         },
-        "metadata": {
-            grai_base_config.metadata_id: build_grai_metadata(current, version),
-            config.metadata_id: build_dbt_metadata(current, version),
-        },
+        "metadata": build_metadata(current, version),
     }
 
     return EdgeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
 def adapt_list_to_client(objs: Sequence, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
```

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/adapters/v5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Literal
 
 from dbt_artifacts_parser.parsers.manifest.manifest_v5 import ParsedSourceDefinition
 
-from grai_source_dbt.adapters.adapters import build_dbt_metadata
+from grai_source_dbt.adapters.adapters import build_app_metadata
 
 
-@build_dbt_metadata.register
+@build_app_metadata.register
 def build_metadata_from_node(current: ParsedSourceDefinition, version: Literal["v1"] = "v1") -> Dict:
     data = {
         "description": current.description,
         "dbt_resource_type": current.resource_type,
         "table_name": current.name,
         "dbt_model_name": current.unique_id,
     }
```

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/base.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.2.7/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.2.7/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,17 @@
                 column = self.columns[(table.unique_id, column.name)]
                 edge = self.make_edge(table, column, Constraint("bt"), EdgeTypeLabels.table_to_column)
                 result.append(edge)
 
             # Seeds don't have depends_on and will error without this check.
             if hasattr(table.depends_on, "nodes"):
                 for parent_str in table.depends_on.nodes:
-                    if parent_str in self.node_map:
-                        source_node = self.node_map[parent_str]
-                    elif parent_str in self.manifest.sources:
-                        source_node = self.manifest.sources[parent_str]
-                    else:
-                        continue
+                    source_node = (
+                        self.node_map[parent_str] if parent_str in self.node_map else self.manifest.sources[parent_str]
+                    )
                     edge = self.make_edge(source_node, table, Constraint("dbtm"), EdgeTypeLabels.table_to_table, True)
                     result.append(edge)
 
         for table in self.manifest.sources.values():
             for column in table.columns.values():
                 column = self.columns[(table.unique_id, column.name)]
                 edge = self.make_edge(table, column, Constraint("bt"), EdgeTypeLabels.table_to_column)
```

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/loaders/v8.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/loaders/v8.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/processor.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/processor.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.2.7/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.2.6a0/setup.py` & `grai_source_dbt-0.2.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['dbt-artifacts-parser>=0.2.4,<0.3.0',
  'grai-client>=0.2.0,<0.3.0',
  'grai-schemas>=0.1.10,<0.2.0',
  'pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-dbt',
-    'version': '0.2.6a0',
+    'version': '0.2.7',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_dbt-0.2.6a0/PKG-INFO` & `grai_source_dbt-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.2.6a0
+Version: 0.2.7
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

