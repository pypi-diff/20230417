# Comparing `tmp/oarepo-model-builder-vocabularies-1.0.8.tar.gz` & `tmp/oarepo-model-builder-vocabularies-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-1.0.8.tar", last modified: Wed Mar 29 08:34:55 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-1.0.9.tar", last modified: Mon Apr 17 19:22:11 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-1.0.8.tar` & `oarepo-model-builder-vocabularies-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:33:25.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-29 08:34:55.000000 oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-29 08:34:55.725909 oarepo-model-builder-vocabularies-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-29 08:32:38.000000 oarepo-model-builder-vocabularies-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:19:42.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 19:22:11.000000 oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-17 19:22:11.466076 oarepo-model-builder-vocabularies-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 19:18:59.000000 oarepo-model-builder-vocabularies-1.0.9/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-1.0.8/PKG-INFO` & `oarepo-model-builder-vocabularies-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from oarepo_model_builder.validation import InvalidModelException
-
-from marshmallow import fields
-from oarepo_model_builder_relations.datatypes import RelationDataType
 import munch
+from marshmallow import fields
+from oarepo_model_builder.datatypes.datatypes import DataType
 from oarepo_model_builder.utils.hyphen_munch import HyphenMunch
+from oarepo_model_builder.validation import InvalidModelException
+from oarepo_model_builder_relations.datatypes import RelationDataType
 
 
 class VocabularyDataType(RelationDataType):
     model_type = "vocabulary"
+    default_facet_class = "VocabularyFacet"
+    default_facet_imports = [
+        {"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}
+    ]
 
     def prepare(self, context):
-        vocabulary_type = self.definition.pop("vocabulary-type", None)
+        vocabulary_type = self.definition.get("vocabulary-type", None)
         vocabulary_class = self.definition.pop("class", None)
 
         vocabulary_imports = self.definition.setdefault("imports", [])
         self.definition.setdefault("model", "vocabularies")
         self.definition.setdefault(
             "keys", ["id", "title", {"key": "type.id", "target": "type"}]
         )
@@ -37,27 +41,60 @@
             else:
                 if vocabulary_type:
                     raise InvalidModelException(
                         "{self.stack.path}: Can not have both vocabulary class and type specified"
                     )
                 pid_field = f"{vocabulary_class}.pid"
 
-        self.definition["type"] = "relation"
+        # self.definition["type"] = "relation"
         self.definition["pid-field"] = pid_field
         super().prepare(context)
 
+    def get_facet(self, stack, parent_path):
+        if not stack:
+            # we are the facet, unlike normal container, for which a facet is not generated,
+            # we need to generate it -> calling direct data type
+            return DataType.get_facet(self, stack, parent_path)
+
+        # do not return any facets for children
+        return []
+
+    def _get_facet_definition(
+        self, stack, facet_class, facet_name, path, path_suffix, label, serialized_args
+    ):
+        # the container's implementation counts on generating facets for children and not self,
+        # so bypassing it and calling direct data type
+        vocabulary_type = self.definition.get("vocabulary-type", None)
+        if vocabulary_type:
+            serialized_args += ", "
+            serialized_args += f'vocabulary="{vocabulary_type}"'
+        return DataType._get_facet_definition(
+            self,
+            stack,
+            facet_class,
+            facet_name,
+            path,
+            path_suffix,
+            label,
+            serialized_args,
+        )
+
     class ModelSchema(RelationDataType.ModelSchema):
         vocabulary_type = fields.String(
             attribute="vocabulary-type", data_key="vocabulary-type", required=False
         )
         model = fields.String(required=False)
 
 
 class TaxonomyDataType(VocabularyDataType):
     model_type = "taxonomy"
+    default_facet_class = "HierarchyVocabularyFacet"
+    default_facet_imports = [
+        {"import": "oarepo_vocabularies.services.facets.HierarchyVocabularyFacet"}
+    ]
 
     def prepare(self, context):
         keys = list(self.definition.get("keys", []))
         self.definition.setdefault("ui", {}).setdefault("detail", "taxonomy_item")
         self.definition["ui"].setdefault("edit", "taxonomy_item")
 
         def has_key(fields, field_name):
@@ -118,17 +155,20 @@
                                     },
                                 },
                             },
                             "ancestors": {
                                 "type": "array",
                                 "items": {"type": "keyword"},
                             },
+                            "ancestors_or_self": {
+                                "type": "array",
+                                "items": {"type": "keyword"},
+                            },
                         },
                     },
                 }
             )
-        self.definition["type"] = type
         self.definition["keys"] = munch.munchify(list(keys), HyphenMunch)
         super().prepare(context)
 
 
 DATATYPES = [VocabularyDataType, TaxonomyDataType]
```

### Comparing `oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/vocabulary.json` & `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 1.0.8
+Version: 1.0.9
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-1.0.8/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-1.0.9/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-1.0.8/setup.cfg` & `oarepo-model-builder-vocabularies-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 1.0.8
+version = 1.0.9
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

