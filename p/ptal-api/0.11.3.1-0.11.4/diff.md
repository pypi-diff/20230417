# Comparing `tmp/ptal_api-0.11.3.1.tar.gz` & `tmp/ptal_api-0.11.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.3.1.tar", max compression
+gzip compressed data, was "ptal_api-0.11.4.tar", max compression
```

## Comparing `ptal_api-0.11.3.1.tar` & `ptal_api-0.11.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-04 15:29:18.455794 ptal_api-0.11.3.1/ptal_api/__init__.py
--rw-r--r--   0        0        0    96789 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/adapter.py
--rw-r--r--   0        0        0      127 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      752 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12105 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      905 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3240 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-04 15:29:18.403793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2107 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1399 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4565 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    22266 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1830 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3364 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-04-04 15:29:18.459794 ptal_api-0.11.3.1/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4803 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1211 2023-04-04 15:29:18.407793 ptal_api-0.11.3.1/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-04-04 15:29:18.459794 ptal_api-0.11.3.1/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   288340 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    91715 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    73079 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   135644 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3641 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-04-04 15:29:18.459794 ptal_api-0.11.3.1/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1047 2023-04-04 15:29:18.411793 ptal_api-0.11.3.1/pyproject.toml
--rw-r--r--   0        0        0     1690 1970-01-01 00:00:00.000000 ptal_api-0.11.3.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-17 12:02:16.437018 ptal_api-0.11.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 12:02:16.497018 ptal_api-0.11.4/ptal_api/__init__.py
+-rw-r--r--   0        0        0    96789 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/adapter.py
+-rw-r--r--   0        0        0      127 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      752 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    12105 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      905 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3240 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2107 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1399 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4565 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    22266 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1830 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-04-17 12:02:16.441018 ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3364 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4803 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1211 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   288635 2023-04-17 12:02:16.445018 ptal_api-0.11.4/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    92810 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   135944 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3641 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:02:16.501018 ptal_api-0.11.4/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-17 12:02:16.449018 ptal_api-0.11.4/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1045 2023-04-17 12:02:16.449018 ptal_api-0.11.4/pyproject.toml
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.4/PKG-INFO
```

### Comparing `ptal_api-0.11.3.1/README.md` & `ptal_api-0.11.4/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/adapter.py` & `ptal_api-0.11.4/ptal_api/adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.4/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.4/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.4/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.4/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/schema/README.md` & `ptal_api-0.11.4/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/schema/api_schema.py` & `ptal_api-0.11.4/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 
 
 class ChartType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('line',)
 
 
+class ChildVisibility(sgqlc.types.Enum):
+    __schema__ = api_schema
+    __choices__ = ('all', 'childrenOnly')
+
+
 class ComponentView(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('keyValue', 'value')
 
 
 class CompositeConceptTypeSorting(sgqlc.types.Enum):
     __schema__ = api_schema
@@ -244,15 +249,15 @@
 class MapNodeType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('concept', 'conceptCandidateFact', 'conceptType', 'document')
 
 
 class Name(sgqlc.types.Enum):
     __schema__ = api_schema
-    __choices__ = ('approvedPropsRelevance', 'conceptApprovedPropsRelevance', 'conceptFactRelevance', 'conceptMeaningPropsRelevance', 'conceptNercRelevance', 'conceptNercSearchRelevance', 'conceptPropsRelevance', 'conceptSubstituteRelevance', 'factRelevance', 'mapApprovedPropsRelevance', 'mapFactRelevance', 'mapMeaningPropsRelevance', 'mapNercRelevance', 'mapNercSearchRelevance', 'mapPropsRelevance', 'meaningPropsRelevance', 'nercRelevance', 'nercSearchRelevance', 'propsRelevance', 'queryScore', 'totalRelevance')
+    __choices__ = ('approvedPropsRelevance', 'conceptApprovedPropsRelevance', 'conceptFactRelevance', 'conceptMeaningPropsRelevance', 'conceptNercRelevance', 'conceptNercSearchRelevance', 'conceptPropsRelevance', 'conceptSubstituteRelevance', 'factRelevance', 'mapApprovedPropsRelevance', 'mapFactRelevance', 'mapMeaningPropsRelevance', 'mapNercRelevance', 'mapNercSearchRelevance', 'mapPropsRelevance', 'meaningPropsRelevance', 'nercRelevance', 'nercSearchRelevance', 'propsRelevance', 'queryScore', 'significantTextRelevance', 'totalRelevance')
 
 
 class NodeType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('header', 'image', 'json', 'key', 'list', 'other', 'row', 'table', 'text')
 
 
@@ -1101,15 +1106,15 @@
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     query = sgqlc.types.Field(String, graphql_name='query')
     filter_settings = sgqlc.types.Field('DocumentFilterSettings', graphql_name='filterSettings')
 
 
 class DocumentFilterSettings(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('search_string', 'substring', 'named_entities', 'concepts', 'meaning_concept_candidates', 'platforms', 'accounts', 'nerc_num', 'concepts_num', 'child_docs_num', 'publication_date', 'registration_date', 'last_update', 'creator', 'publication_author', 'last_updater', 'access_level_id', 'links', 'external_url', 'markers', 'document_type', 'source_type', 'trust_level', 'has_linked_issues', 'nested_ids', 'fact_types', 'story', 'show_read', 'job_ids', 'periodic_job_ids', 'task_ids', 'periodic_task_ids', 'document_is_media', 'document_is_processed')
+    __field_names__ = ('search_string', 'substring', 'named_entities', 'concepts', 'meaning_concept_candidates', 'platforms', 'accounts', 'nerc_num', 'concepts_num', 'child_docs_num', 'publication_date', 'registration_date', 'last_update', 'creator', 'publication_author', 'last_updater', 'access_level_id', 'links', 'external_url', 'markers', 'document_type', 'source_type', 'trust_level', 'has_linked_issues', 'nested_ids', 'fact_types', 'story', 'show_read', 'job_ids', 'periodic_job_ids', 'task_ids', 'periodic_task_ids', 'document_is_media', 'document_is_processed', 'child_visibility')
     search_string = sgqlc.types.Field(String, graphql_name='searchString')
     substring = sgqlc.types.Field(String, graphql_name='substring')
     named_entities = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='namedEntities')
     concepts = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='concepts')
     meaning_concept_candidates = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='meaningConceptCandidates')
     platforms = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='platforms')
     accounts = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='accounts')
@@ -1136,14 +1141,15 @@
     show_read = sgqlc.types.Field(Boolean, graphql_name='showRead')
     job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='jobIds')
     periodic_job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='periodicJobIds')
     task_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='taskIds')
     periodic_task_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='periodicTaskIds')
     document_is_media = sgqlc.types.Field(Boolean, graphql_name='documentIsMedia')
     document_is_processed = sgqlc.types.Field(Boolean, graphql_name='documentIsProcessed')
+    child_visibility = sgqlc.types.Field(ChildVisibility, graphql_name='childVisibility')
 
 
 class DocumentLinkFilterSetting(sgqlc.types.Input):
     __schema__ = api_schema
     __field_names__ = ('document_type',)
     document_type = sgqlc.types.Field(DocumentType, graphql_name='documentType')
 
@@ -1171,22 +1177,23 @@
     __field_names__ = ('sorting_type', 'sort_direction')
     sorting_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentSorting), graphql_name='sortingType')
     sort_direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='sortDirection')
 
 
 class DocumentRelevanceMetricsInput(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
+    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'significant_text_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
     nerc_relevance = sgqlc.types.Field(Int, graphql_name='nercRelevance')
     fact_relevance = sgqlc.types.Field(Int, graphql_name='factRelevance')
     props_relevance = sgqlc.types.Field(Int, graphql_name='propsRelevance')
     approved_props_relevance = sgqlc.types.Field(Int, graphql_name='approvedPropsRelevance')
     meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='meaningPropsRelevance')
     concept_substitute_relevance = sgqlc.types.Field(Int, graphql_name='conceptSubstituteRelevance')
     nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='nercSearchRelevance')
+    significant_text_relevance = sgqlc.types.Field(Int, graphql_name='significantTextRelevance')
     concept_nerc_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercRelevance')
     concept_fact_relevance = sgqlc.types.Field(Int, graphql_name='conceptFactRelevance')
     concept_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptPropsRelevance')
     concept_approved_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptApprovedPropsRelevance')
     concept_meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptMeaningPropsRelevance')
     concept_nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercSearchRelevance')
     map_nerc_relevance = sgqlc.types.Field(Int, graphql_name='mapNercRelevance')
@@ -1218,16 +1225,15 @@
     __schema__ = api_schema
     __field_names__ = ('value',)
     value = sgqlc.types.Field(sgqlc.types.non_null(Float), graphql_name='value')
 
 
 class ExtraSettings(sgqlc.types.Input):
     __schema__ = api_schema
-    __field_names__ = ('hide_child', 'search_on_map', 'ranking_script', 'selected_content')
-    hide_child = sgqlc.types.Field(Boolean, graphql_name='hideChild')
+    __field_names__ = ('search_on_map', 'ranking_script', 'selected_content')
     search_on_map = sgqlc.types.Field(Boolean, graphql_name='searchOnMap')
     ranking_script = sgqlc.types.Field(String, graphql_name='rankingScript')
     selected_content = sgqlc.types.Field('ResearchMapContentSelectInput', graphql_name='selectedContent')
 
 
 class FactInput(sgqlc.types.Input):
     __schema__ = api_schema
@@ -2323,22 +2329,23 @@
     __field_names__ = ('sorting_type', 'sort_direction')
     sorting_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentSorting), graphql_name='sortingType')
     sort_direction = sgqlc.types.Field(sgqlc.types.non_null(SortDirection), graphql_name='sortDirection')
 
 
 class DocumentRelevanceMetrics(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
+    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'significant_text_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
     nerc_relevance = sgqlc.types.Field(Int, graphql_name='nercRelevance')
     fact_relevance = sgqlc.types.Field(Int, graphql_name='factRelevance')
     props_relevance = sgqlc.types.Field(Int, graphql_name='propsRelevance')
     approved_props_relevance = sgqlc.types.Field(Int, graphql_name='approvedPropsRelevance')
     meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='meaningPropsRelevance')
     concept_substitute_relevance = sgqlc.types.Field(Int, graphql_name='conceptSubstituteRelevance')
     nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='nercSearchRelevance')
+    significant_text_relevance = sgqlc.types.Field(Int, graphql_name='significantTextRelevance')
     concept_nerc_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercRelevance')
     concept_fact_relevance = sgqlc.types.Field(Int, graphql_name='conceptFactRelevance')
     concept_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptPropsRelevance')
     concept_approved_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptApprovedPropsRelevance')
     concept_meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptMeaningPropsRelevance')
     concept_nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercSearchRelevance')
     map_nerc_relevance = sgqlc.types.Field(Int, graphql_name='mapNercRelevance')
@@ -3521,15 +3528,14 @@
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('direction', sgqlc.types.Arg(SortDirection, graphql_name='direction', default='descending')),
         ('sort_field', sgqlc.types.Arg(AccessLevelSorting, graphql_name='sortField', default='id')),
 ))
     )
     story_fs2_query = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='storyFs2Query', args=sgqlc.types.ArgDict((
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(DocumentFilterSettings), graphql_name='filterSettings', default=None)),
-        ('extra_settings', sgqlc.types.Arg(sgqlc.types.non_null(ExtraSettings), graphql_name='extraSettings', default=None)),
 ))
     )
     concept_fs2_query = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='conceptFs2Query', args=sgqlc.types.ArgDict((
         ('filter_settings', sgqlc.types.Arg(sgqlc.types.non_null(ConceptFilterSettings), graphql_name='filterSettings', default=None)),
 ))
     )
     markers_bulk = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(Markers)), graphql_name='markersBulk', args=sgqlc.types.ArgDict((
```

### Comparing `ptal_api-0.11.3.1/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.4/ptal_api/schema/crawlers_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,20 @@
 class ProjectSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('creator', 'description', 'id', 'lastUpdater', 'name', 'systemRegistrationDate', 'systemUpdateDate', 'title')
 
 
 class RecoveryJobSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
-    __choices__ = ('createdAt', 'endTime', 'id', 'progress', 'startTime', 'status')
+    __choices__ = ('createdAt', 'endTime', 'id', 'progress', 'startTime', 'status', 'updatedAt')
 
 
 class RecoveryJobStatus(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
-    __choices__ = ('Error', 'InProgress', 'Pending', 'Success')
+    __choices__ = ('Canceled', 'Error', 'InProgress', 'Pending', 'Success')
 
 
 class RequestSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('timestamp',)
 
 
@@ -313,20 +313,21 @@
     is_retrospective = sgqlc.types.Field(Boolean, graphql_name='isRetrospective')
     retrospective_interval = sgqlc.types.Field('TimestampInterval', graphql_name='retrospectiveInterval')
     actual_status = sgqlc.types.Field(InformationSourceLoaderActualStatus, graphql_name='actualStatus')
 
 
 class JobInput(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('crawler_id', 'version_id', 'priority', 'message_priority', 'is_noise', 'settings', 'args')
+    __field_names__ = ('crawler_id', 'version_id', 'priority', 'message_priority', 'is_noise', 'research_map_id', 'settings', 'args')
     crawler_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='crawlerId')
     version_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='versionId')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(MessagePriority, graphql_name='messagePriority')
     is_noise = sgqlc.types.Field(Boolean, graphql_name='isNoise')
+    research_map_id = sgqlc.types.Field(ID, graphql_name='researchMapId')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('KeyValueInputType'))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('KeyValueInputType'))), graphql_name='args')
 
 
 class JobSorting(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
     __field_names__ = ('job_pending_sorting', 'job_running_sorting', 'job_finished_sorting')
@@ -454,22 +455,24 @@
     eggfile = sgqlc.types.Field(String, graphql_name='eggfile')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='args')
 
 
 class RecoveryJobFilterSettings(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('input_value', 'crawlers', 'statuses', 'start_time', 'end_time', 'creators', 'created_at')
+    __field_names__ = ('input_value', 'crawlers', 'statuses', 'start_time', 'end_time', 'creators', 'created_at', 'updaters', 'updated_at')
     input_value = sgqlc.types.Field(String, graphql_name='inputValue')
     crawlers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='crawlers')
     statuses = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(RecoveryJobStatus)), graphql_name='statuses')
     start_time = sgqlc.types.Field('TimestampInterval', graphql_name='startTime')
     end_time = sgqlc.types.Field('TimestampInterval', graphql_name='endTime')
     creators = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='creators')
     created_at = sgqlc.types.Field('TimestampInterval', graphql_name='createdAt')
+    updaters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='updaters')
+    updated_at = sgqlc.types.Field('TimestampInterval', graphql_name='updatedAt')
 
 
 class RequestFilterSettings(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
     __field_names__ = ('input_text', 'interval')
     input_text = sgqlc.types.Field(String, graphql_name='inputText')
     interval = sgqlc.types.Field('TimestampInterval', graphql_name='interval')
@@ -724,15 +727,15 @@
     __field_names__ = ('total', 'list_metric')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_metric = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Metric))), graphql_name='listMetric')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job')
+    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
     update_crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawler', args=sgqlc.types.ArgDict((
         ('crawler_update_input', sgqlc.types.Arg(sgqlc.types.non_null(CrawlerUpdateInput), graphql_name='crawlerUpdateInput', default=None)),
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
 ))
     )
     update_crawler_settings_arguments = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawlerSettingsArguments', args=sgqlc.types.ArgDict((
@@ -867,14 +870,18 @@
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
     add_recovery_job = sgqlc.types.Field(sgqlc.types.non_null('RecoveryJob'), graphql_name='addRecoveryJob', args=sgqlc.types.ArgDict((
         ('add_recovery_job_input', sgqlc.types.Arg(sgqlc.types.non_null(AddRecoveryJobInput), graphql_name='addRecoveryJobInput', default=None)),
 ))
     )
+    cancel_recovery_job = sgqlc.types.Field(sgqlc.types.non_null('RecoveryJob'), graphql_name='cancelRecoveryJob', args=sgqlc.types.ArgDict((
+        ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
+))
+    )
 
 
 class PeriodicJobData(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'name')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
@@ -925,15 +932,15 @@
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     job_ids_with_error_logs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Long))), graphql_name='jobIdsWithErrorLogs')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
+    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
     analytics = sgqlc.types.Field(sgqlc.types.non_null('Stats'), graphql_name='analytics')
     crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='crawler', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     list_crawler = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('Crawler')), graphql_name='listCrawler', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
@@ -948,14 +955,19 @@
 ))
     )
     crawler_args_and_settings_description = sgqlc.types.Field(sgqlc.types.non_null(ArgsAndSettingsDescription), graphql_name='crawlerArgsAndSettingsDescription', args=sgqlc.types.ArgDict((
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('version_id', sgqlc.types.Arg(ID, graphql_name='versionId', default=None)),
 ))
     )
+    crawler_site_map = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='crawlerSiteMap', args=sgqlc.types.ArgDict((
+        ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
+        ('version_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='versionId', default=None)),
+))
+    )
     crawl_state = sgqlc.types.Field(sgqlc.types.non_null(CrawlState), graphql_name='crawlState', args=sgqlc.types.ArgDict((
         ('crawl_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlId', default=None)),
 ))
     )
     crawl_state_by_parameters = sgqlc.types.Field(sgqlc.types.non_null(CrawlState), graphql_name='crawlStateByParameters', args=sgqlc.types.ArgDict((
         ('crawl_state_parameters', sgqlc.types.Arg(sgqlc.types.non_null(CrawlStateParameters), graphql_name='crawlStateParameters', default=None)),
 ))
@@ -1159,26 +1171,28 @@
     system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
     creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
     last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
 
 
 class RecoveryJob(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'crawler_data', 'source_version_data', 'result_version_data', 'status', 'start_time', 'end_time', 'progress', 'progress_message', 'creator', 'system_registration_date')
+    __field_names__ = ('id', 'crawler_data', 'source_version_data', 'result_version_data', 'status', 'start_time', 'end_time', 'progress', 'progress_message', 'creator', 'system_registration_date', 'last_updater', 'system_update_date')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     crawler_data = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawlerData')
     source_version_data = sgqlc.types.Field(sgqlc.types.non_null('VersionData'), graphql_name='sourceVersionData')
     result_version_data = sgqlc.types.Field('VersionData', graphql_name='resultVersionData')
     status = sgqlc.types.Field(sgqlc.types.non_null(RecoveryJobStatus), graphql_name='status')
     start_time = sgqlc.types.Field(UnixTime, graphql_name='startTime')
     end_time = sgqlc.types.Field(UnixTime, graphql_name='endTime')
     progress = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='progress')
     progress_message = sgqlc.types.Field(String, graphql_name='progressMessage')
     creator = sgqlc.types.Field(sgqlc.types.non_null('User'), graphql_name='creator')
     system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
+    last_updater = sgqlc.types.Field('User', graphql_name='lastUpdater')
+    system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
 
 
 class RecoveryJobPagination(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('total', 'list_recovery_job')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_recovery_job = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(RecoveryJob))), graphql_name='listRecoveryJob')
@@ -1276,15 +1290,15 @@
     __field_names__ = ('total', 'list_version')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_version = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Version'))), graphql_name='listVersion')
 
 
 class Crawler(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'name', 'title', 'description', 'project', 'periodic_jobs_num', 'onetime_jobs_num', 'last_collection_date', 'avg_performance_time', 'pinned', 'settings', 'args', 'analytics', 'histogram_items', 'histogram_requests', 'job_stats', 'current_version', 'start_urls', 'sitemap')
+    __field_names__ = ('id', 'name', 'title', 'description', 'project', 'periodic_jobs_num', 'onetime_jobs_num', 'last_collection_date', 'avg_performance_time', 'pinned', 'settings', 'args', 'analytics', 'histogram_items', 'histogram_requests', 'job_stats', 'current_version', 'start_urls')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='title')
     description = sgqlc.types.Field(String, graphql_name='description')
     project = sgqlc.types.Field(sgqlc.types.non_null(ProjectData), graphql_name='project')
     periodic_jobs_num = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='periodicJobsNum')
     onetime_jobs_num = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='onetimeJobsNum')
@@ -1307,15 +1321,14 @@
     )
     job_stats = sgqlc.types.Field(sgqlc.types.non_null(JobStats), graphql_name='jobStats', args=sgqlc.types.ArgDict((
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
     )
     current_version = sgqlc.types.Field('Version', graphql_name='currentVersion')
     start_urls = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='startUrls')
-    sitemap = sgqlc.types.Field(JSON, graphql_name='sitemap')
 
 
 class Credential(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'data_type', 'description', 'login', 'password', 'token', 'domain', 'projects', 'status')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     data_type = sgqlc.types.Field(sgqlc.types.non_null(CredentialType), graphql_name='dataType')
```

### Comparing `ptal_api-0.11.3.1/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.4/ptal_api/schema/tcontroller_api_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class ExportTaskState(sgqlc.types.Enum):
     __schema__ = tcontroller_api_schema
     __choices__ = ('failed', 'ok', 'pending')
 
 
 class ExporterSort(sgqlc.types.Enum):
     __schema__ = tcontroller_api_schema
-    __choices__ = ('id',)
+    __choices__ = ('id', 'lastTaskTime', 'menuTitle', 'title')
 
 
 Float = sgqlc.types.Float
 
 ID = sgqlc.types.ID
 
 Int = sgqlc.types.Int
@@ -183,20 +183,24 @@
     __field_names__ = ('entities', 'params')
     entities = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ExportEntityInput))), graphql_name='entities')
     params = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='params')
 
 
 class ExporterFilter(sgqlc.types.Input):
     __schema__ = tcontroller_api_schema
-    __field_names__ = ('can_export_document', 'can_export_concept', 'can_export_one_entity', 'can_export_multiple_entities', 'can_export_concept_type_ids')
+    __field_names__ = ('can_export_document', 'can_export_concept', 'can_export_one_entity', 'can_export_multiple_entities', 'can_export_concept_type_ids', 'title', 'menu_title', 'creator_id', 'last_updater_id')
     can_export_document = sgqlc.types.Field(Boolean, graphql_name='canExportDocument')
     can_export_concept = sgqlc.types.Field(Boolean, graphql_name='canExportConcept')
     can_export_one_entity = sgqlc.types.Field(Boolean, graphql_name='canExportOneEntity')
     can_export_multiple_entities = sgqlc.types.Field(Boolean, graphql_name='canExportMultipleEntities')
     can_export_concept_type_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='canExportConceptTypeIds')
+    title = sgqlc.types.Field(String, graphql_name='title')
+    menu_title = sgqlc.types.Field(String, graphql_name='menuTitle')
+    creator_id = sgqlc.types.Field(ID, graphql_name='creatorId')
+    last_updater_id = sgqlc.types.Field(ID, graphql_name='lastUpdaterId')
 
 
 class ExporterInput(sgqlc.types.Input):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('menu_title', 'description', 'default_params', 'can_export_one_entity', 'can_export_multiple_entities', 'concept_type_ids')
     menu_title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='menuTitle')
     description = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='description')
@@ -582,15 +586,15 @@
     __schema__ = tcontroller_api_schema
     __field_names__ = ('unknown',)
     unknown = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='unknown')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = tcontroller_api_schema
-    __field_names__ = ('add_pipeline_config', 'copy_pipeline_config', 'import_pipeline_config', 'update_pipeline_config', 'delete_pipeline_config', 'put_kafka_topic', 'update_kafka_topics', 'delete_kafka_topic', 'retry_failed_in_topic', 'retry_failed_message', 'copy_pending_to_kafka', 'reprocess_message', 'reprocess_messages', 'update_exporter', 'add_exporter_task', 'cancel_export_task', 'add_concept_transform_config', 'copy_concept_transform_config', 'update_concept_transform_config', 'update_concept_transform_config_transforms', 'delete_concept_transform_config', 'add_concept_transform_task', 'cancel_concept_transform_task', 'add_user_pipeline_transform', 'update_user_pipeline_transform', 'delete_user_pipeline_transform', 'service_stats')
+    __field_names__ = ('add_pipeline_config', 'copy_pipeline_config', 'import_pipeline_config', 'update_pipeline_config', 'delete_pipeline_config', 'put_kafka_topic', 'update_kafka_topics', 'delete_kafka_topic', 'retry_failed_in_topic', 'retry_failed_message', 'copy_pending_to_kafka', 'reprocess_message', 'reprocess_messages', 'update_exporter', 'add_exporter_task', 'cancel_export_task', 'add_concept_transform_config', 'copy_concept_transform_config', 'update_concept_transform_config', 'update_concept_transform_config_transforms', 'delete_concept_transform_config', 'add_concept_transform_task', 'cancel_concept_transform_task', 'add_user_pipeline_transform', 'update_user_pipeline_transform', 'delete_user_pipeline_transform', 'service_stats', 'add_message')
     add_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='addPipelineConfig', args=sgqlc.types.ArgDict((
         ('description', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='description', default=None)),
         ('transforms', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(PipelineTransformSetupInput))), graphql_name='transforms', default=None)),
 ))
     )
     copy_pipeline_config = sgqlc.types.Field(sgqlc.types.non_null('PipelineConfig'), graphql_name='copyPipelineConfig', args=sgqlc.types.ArgDict((
         ('source_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='sourceId', default=None)),
@@ -716,14 +720,20 @@
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     service_stats = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('ServiceStats'))), graphql_name='serviceStats', args=sgqlc.types.ArgDict((
         ('reset', sgqlc.types.Arg(Boolean, graphql_name='reset', default=False)),
 ))
     )
+    add_message = sgqlc.types.Field(sgqlc.types.non_null(MessageStatus), graphql_name='addMessage', args=sgqlc.types.ArgDict((
+        ('topic', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='topic', default=None)),
+        ('message', sgqlc.types.Arg(sgqlc.types.non_null(JSON), graphql_name='message', default=None)),
+        ('priority', sgqlc.types.Arg(MessagePriority, graphql_name='priority', default='Normal')),
+))
+    )
 
 
 class ParamsSchema(sgqlc.types.Type):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('schema', 'ui_schema')
     schema = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='schema')
     ui_schema = sgqlc.types.Field(JSON, graphql_name='uiSchema')
@@ -794,15 +804,15 @@
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     params = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='params')
     transform = sgqlc.types.Field(sgqlc.types.non_null(PipelineTransform), graphql_name='transform')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = tcontroller_api_schema
-    __field_names__ = ('pipeline_transforms', 'pipeline_transform', 'pipeline_configs', 'pipeline_config', 'export_pipeline_config', 'kafka_pipeline_start_type', 'kafka_topics', 'kafka_topic', 'message_status', 'message_topic', 'message_statuses', 'message_source_available', 'failed_messages', 'pending_messages', 'active_messages', 'completed_ok_messages', 'duplicate_messages', 'messages_by_parent_id', 'exporter', 'exporters', 'export_task', 'export_tasks', 'job_items2', 'periodic_job_items2', 'task_items2', 'periodic_task_items2', 'job_ids_by_message_uuid2', 'job_metrics2', 'periodic_job_metrics2', 'task_metrics2', 'periodic_task_metrics2', 'concept_transform_configs', 'concept_transform_config', 'concept_transform_message_type', 'concept_transform_task', 'concept_transform_tasks', 'user_pipeline_transforms', 'user_pipeline_transform')
+    __field_names__ = ('pipeline_transforms', 'pipeline_transform', 'pipeline_configs', 'pipeline_config', 'export_pipeline_config', 'kafka_pipeline_start_type', 'kafka_topics', 'kafka_topic', 'message_status', 'message_topic', 'message_statuses', 'message_source_available', 'failed_messages', 'pending_messages', 'active_messages', 'completed_ok_messages', 'duplicate_messages', 'messages_by_parent_id', 'exporter', 'exporters', 'export_task', 'export_tasks', 'job_items2', 'periodic_job_items2', 'task_items2', 'periodic_task_items2', 'job_ids_by_message_uuid2', 'job_metrics2', 'periodic_job_metrics2', 'task_metrics2', 'periodic_task_metrics2', 'concept_transform_configs', 'concept_transform_config', 'concept_transform_message_type', 'concept_transform_task', 'concept_transform_tasks', 'user_pipeline_transforms', 'user_pipeline_transform', 'debug_dump_extensions')
     pipeline_transforms = sgqlc.types.Field(sgqlc.types.non_null(PipelineTransformList), graphql_name='pipelineTransforms', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=None)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=None)),
         ('filter', sgqlc.types.Arg(PipelineTransformFilter, graphql_name='filter', default=None)),
 ))
     )
     pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null(PipelineTransform), graphql_name='pipelineTransform', args=sgqlc.types.ArgDict((
@@ -1021,14 +1031,15 @@
         ('filter', sgqlc.types.Arg(UserPipelineTransformFilter, graphql_name='filter', default=None)),
 ))
     )
     user_pipeline_transform = sgqlc.types.Field(sgqlc.types.non_null('UserPipelineTransform'), graphql_name='userPipelineTransform', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
+    debug_dump_extensions = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='debugDumpExtensions')
 
 
 class RecordInterface(sgqlc.types.Interface):
     __schema__ = tcontroller_api_schema
     __field_names__ = ('system_registration_date', 'system_update_date', 'creator', 'last_updater')
     system_registration_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='systemRegistrationDate')
     system_update_date = sgqlc.types.Field(UnixTime, graphql_name='systemUpdateDate')
```

### Comparing `ptal_api-0.11.3.1/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.4/ptal_api/schema/utils_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 class AccountSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('creator', 'id', 'lastUpdater', 'name', 'platformId', 'systemRegistrationDate', 'systemUpdateDate', 'url')
 
 
 Boolean = sgqlc.types.Boolean
 
+class ChildVisibility(sgqlc.types.Enum):
+    __schema__ = utils_api_schema
+    __choices__ = ('all', 'childrenOnly')
+
+
 class ComponentView(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('keyValue', 'value')
 
 
 class CompositeConceptTypeWidgetTypeSorting(sgqlc.types.Enum):
     __schema__ = utils_api_schema
@@ -153,15 +158,15 @@
 class MapNodeType(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('concept', 'conceptCandidateFact', 'conceptType', 'document')
 
 
 class Name(sgqlc.types.Enum):
     __schema__ = utils_api_schema
-    __choices__ = ('approvedPropsRelevance', 'conceptApprovedPropsRelevance', 'conceptFactRelevance', 'conceptMeaningPropsRelevance', 'conceptNercRelevance', 'conceptNercSearchRelevance', 'conceptPropsRelevance', 'conceptSubstituteRelevance', 'factRelevance', 'mapApprovedPropsRelevance', 'mapFactRelevance', 'mapMeaningPropsRelevance', 'mapNercRelevance', 'mapNercSearchRelevance', 'mapPropsRelevance', 'meaningPropsRelevance', 'nercRelevance', 'nercSearchRelevance', 'propsRelevance', 'queryScore', 'totalRelevance')
+    __choices__ = ('approvedPropsRelevance', 'conceptApprovedPropsRelevance', 'conceptFactRelevance', 'conceptMeaningPropsRelevance', 'conceptNercRelevance', 'conceptNercSearchRelevance', 'conceptPropsRelevance', 'conceptSubstituteRelevance', 'factRelevance', 'mapApprovedPropsRelevance', 'mapFactRelevance', 'mapMeaningPropsRelevance', 'mapNercRelevance', 'mapNercSearchRelevance', 'mapPropsRelevance', 'meaningPropsRelevance', 'nercRelevance', 'nercSearchRelevance', 'propsRelevance', 'queryScore', 'significantTextRelevance', 'totalRelevance')
 
 
 class NodeType(sgqlc.types.Enum):
     __schema__ = utils_api_schema
     __choices__ = ('header', 'image', 'json', 'key', 'list', 'other', 'row', 'table', 'text')
 
 
@@ -369,15 +374,15 @@
     __field_names__ = ('date', 'time')
     date = sgqlc.types.Field(sgqlc.types.non_null(DateInput), graphql_name='date')
     time = sgqlc.types.Field('TimeInput', graphql_name='time')
 
 
 class DocumentFilterSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('search_string', 'substring', 'named_entities', 'concepts', 'meaning_concept_candidates', 'platforms', 'accounts', 'nerc_num', 'concepts_num', 'child_docs_num', 'publication_date', 'registration_date', 'last_update', 'creator', 'publication_author', 'last_updater', 'access_level_id', 'links', 'external_url', 'markers', 'document_type', 'source_type', 'trust_level', 'has_linked_issues', 'nested_ids', 'fact_types', 'story', 'show_read', 'job_ids', 'periodic_job_ids', 'task_ids', 'periodic_task_ids', 'document_is_media', 'document_is_processed')
+    __field_names__ = ('search_string', 'substring', 'named_entities', 'concepts', 'meaning_concept_candidates', 'platforms', 'accounts', 'nerc_num', 'concepts_num', 'child_docs_num', 'publication_date', 'registration_date', 'last_update', 'creator', 'publication_author', 'last_updater', 'access_level_id', 'links', 'external_url', 'markers', 'document_type', 'source_type', 'trust_level', 'has_linked_issues', 'nested_ids', 'fact_types', 'story', 'show_read', 'job_ids', 'periodic_job_ids', 'task_ids', 'periodic_task_ids', 'document_is_media', 'document_is_processed', 'child_visibility')
     search_string = sgqlc.types.Field(String, graphql_name='searchString')
     substring = sgqlc.types.Field(String, graphql_name='substring')
     named_entities = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='namedEntities')
     concepts = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='concepts')
     meaning_concept_candidates = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='meaningConceptCandidates')
     platforms = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='platforms')
     accounts = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='accounts')
@@ -404,32 +409,34 @@
     show_read = sgqlc.types.Field(Boolean, graphql_name='showRead')
     job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='jobIds')
     periodic_job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='periodicJobIds')
     task_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='taskIds')
     periodic_task_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='periodicTaskIds')
     document_is_media = sgqlc.types.Field(Boolean, graphql_name='documentIsMedia')
     document_is_processed = sgqlc.types.Field(Boolean, graphql_name='documentIsProcessed')
+    child_visibility = sgqlc.types.Field(ChildVisibility, graphql_name='childVisibility')
 
 
 class DocumentLinkFilterSetting(sgqlc.types.Input):
     __schema__ = utils_api_schema
     __field_names__ = ('document_type',)
     document_type = sgqlc.types.Field(DocumentType, graphql_name='documentType')
 
 
 class DocumentRelevanceMetricsInput(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
+    __field_names__ = ('nerc_relevance', 'fact_relevance', 'props_relevance', 'approved_props_relevance', 'meaning_props_relevance', 'concept_substitute_relevance', 'nerc_search_relevance', 'significant_text_relevance', 'concept_nerc_relevance', 'concept_fact_relevance', 'concept_props_relevance', 'concept_approved_props_relevance', 'concept_meaning_props_relevance', 'concept_nerc_search_relevance', 'map_nerc_relevance', 'map_fact_relevance', 'map_props_relevance', 'map_approved_props_relevance', 'map_meaning_props_relevance', 'map_nerc_search_relevance')
     nerc_relevance = sgqlc.types.Field(Int, graphql_name='nercRelevance')
     fact_relevance = sgqlc.types.Field(Int, graphql_name='factRelevance')
     props_relevance = sgqlc.types.Field(Int, graphql_name='propsRelevance')
     approved_props_relevance = sgqlc.types.Field(Int, graphql_name='approvedPropsRelevance')
     meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='meaningPropsRelevance')
     concept_substitute_relevance = sgqlc.types.Field(Int, graphql_name='conceptSubstituteRelevance')
     nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='nercSearchRelevance')
+    significant_text_relevance = sgqlc.types.Field(Int, graphql_name='significantTextRelevance')
     concept_nerc_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercRelevance')
     concept_fact_relevance = sgqlc.types.Field(Int, graphql_name='conceptFactRelevance')
     concept_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptPropsRelevance')
     concept_approved_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptApprovedPropsRelevance')
     concept_meaning_props_relevance = sgqlc.types.Field(Int, graphql_name='conceptMeaningPropsRelevance')
     concept_nerc_search_relevance = sgqlc.types.Field(Int, graphql_name='conceptNercSearchRelevance')
     map_nerc_relevance = sgqlc.types.Field(Int, graphql_name='mapNercRelevance')
@@ -454,16 +461,15 @@
     concept_type_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptTypeId')
     start_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='startDate')
     end_date = sgqlc.types.Field(sgqlc.types.non_null(UnixTime), graphql_name='endDate')
 
 
 class ExtraSettings(sgqlc.types.Input):
     __schema__ = utils_api_schema
-    __field_names__ = ('hide_child', 'search_on_map', 'ranking_script', 'selected_content')
-    hide_child = sgqlc.types.Field(Boolean, graphql_name='hideChild')
+    __field_names__ = ('search_on_map', 'ranking_script', 'selected_content')
     search_on_map = sgqlc.types.Field(Boolean, graphql_name='searchOnMap')
     ranking_script = sgqlc.types.Field(String, graphql_name='rankingScript')
     selected_content = sgqlc.types.Field('ResearchMapContentSelectInput', graphql_name='selectedContent')
 
 
 class FactInput(sgqlc.types.Input):
     __schema__ = utils_api_schema
```

### Comparing `ptal_api-0.11.3.1/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.4/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.4/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.3.1/pyproject.toml` & `ptal_api-0.11.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.3.1"
+version = "0.11.4"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.3.1/PKG-INFO` & `ptal_api-0.11.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.3.1
+Version: 0.11.4
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

