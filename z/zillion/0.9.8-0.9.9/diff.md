# Comparing `tmp/zillion-0.9.8.tar.gz` & `tmp/zillion-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillion-0.9.8.tar", last modified: Wed Apr 12 17:36:28 2023, max compression
+gzip compressed data, was "zillion-0.9.9.tar", last modified: Thu Apr 13 19:39:59 2023, max compression
```

## Comparing `zillion-0.9.8.tar` & `zillion-0.9.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.354758 zillion-0.9.8/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.8/AUTHORS.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.8/LICENSE
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 17:36:28.354758 zillion-0.9.8/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31036 2023-04-12 13:15:10.000000 zillion-0.9.8/README.md
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-12 17:36:28.354758 zillion-0.9.8/setup.cfg
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2885 2023-04-12 01:54:36.000000 zillion-0.9.8/setup.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.8/zillion/configs.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.8/zillion/core.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.8/zillion/datasource.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion/dialects/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.8/zillion/dialects/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/conversions.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.8/zillion/dialects/duckdb.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/mysql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/postgresql.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/dialects/sqlite.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-04-12 12:47:48.000000 zillion-0.9.8/zillion/field.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.8/zillion/model.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    38893 2023-04-12 17:33:37.000000 zillion-0.9.8/zillion/nlp.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    84745 2023-04-12 17:17:38.000000 zillion-0.9.8/zillion/report.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.354758 zillion-0.9.8/zillion/scripts/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/__init__.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.8/zillion/scripts/bootstrap_datasource_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/json_to_yaml.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.8/zillion/scripts/load_config.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     2674 2023-04-12 12:40:39.000000 zillion-0.9.8/zillion/scripts/run_report.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.8/zillion/scripts/yaml_to_json.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.8/zillion/sql_utils.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-12 17:31:42.000000 zillion-0.9.8/zillion/version.py
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-12 17:03:08.000000 zillion-0.9.8/zillion/warehouse.py
-drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-12 17:36:28.350760 zillion-0.9.8/zillion.egg-info/
--rw-rw-r--   0 kurt      (1000) kurt      (1000)    31693 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)     1080 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-12 17:36:28.000000 zillion-0.9.8/zillion.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-13 19:39:59.985687 zillion-0.9.9/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      297 2022-07-15 16:01:20.000000 zillion-0.9.9/AUTHORS.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     7783 2022-07-15 16:01:20.000000 zillion-0.9.9/LICENSE
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    32748 2023-04-13 19:39:59.985687 zillion-0.9.9/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    32040 2023-04-13 19:38:07.000000 zillion-0.9.9/README.md
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       38 2023-04-13 19:39:59.985687 zillion-0.9.9/setup.cfg
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2936 2023-04-12 17:42:19.000000 zillion-0.9.9/setup.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-13 19:39:59.985687 zillion-0.9.9/zillion/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      507 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    51932 2023-03-28 16:19:04.000000 zillion-0.9.9/zillion/configs.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    13415 2023-04-01 17:19:44.000000 zillion-0.9.9/zillion/core.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    69368 2023-04-10 14:08:30.000000 zillion-0.9.9/zillion/datasource.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-13 19:39:59.985687 zillion-0.9.9/zillion/dialects/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       91 2023-03-23 18:24:15.000000 zillion-0.9.9/zillion/dialects/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     6313 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/dialects/conversions.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4677 2023-03-24 13:49:53.000000 zillion-0.9.9/zillion/dialects/duckdb.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     3700 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/dialects/mysql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4556 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/dialects/postgresql.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     4609 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/dialects/sqlite.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    53505 2023-04-12 12:47:48.000000 zillion-0.9.9/zillion/field.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1718 2023-04-10 13:26:28.000000 zillion-0.9.9/zillion/model.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39157 2023-04-13 17:03:15.000000 zillion-0.9.9/zillion/nlp.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    84745 2023-04-12 17:17:38.000000 zillion-0.9.9/zillion/report.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-13 19:39:59.985687 zillion-0.9.9/zillion/scripts/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        0 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/scripts/__init__.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    15096 2023-04-04 14:54:06.000000 zillion-0.9.9/zillion/scripts/bootstrap_datasource_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      121 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/scripts/json_to_yaml.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1241 2023-04-10 13:55:59.000000 zillion-0.9.9/zillion/scripts/load_config.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     2674 2023-04-12 12:40:39.000000 zillion-0.9.9/zillion/scripts/run_report.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      109 2022-07-15 16:01:20.000000 zillion-0.9.9/zillion/scripts/yaml_to_json.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    16500 2023-04-03 19:12:41.000000 zillion-0.9.9/zillion/sql_utils.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)       44 2023-04-13 17:38:09.000000 zillion-0.9.9/zillion/version.py
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    39878 2023-04-12 17:03:08.000000 zillion-0.9.9/zillion/warehouse.py
+drwxrwxr-x   0 kurt      (1000) kurt      (1000)        0 2023-04-13 19:39:59.985687 zillion-0.9.9/zillion.egg-info/
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)    32748 2023-04-13 19:39:59.000000 zillion-0.9.9/zillion.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)      768 2023-04-13 19:39:59.000000 zillion-0.9.9/zillion.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        1 2023-04-13 19:39:59.000000 zillion-0.9.9/zillion.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)     1080 2023-04-13 19:39:59.000000 zillion-0.9.9/zillion.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1000) kurt      (1000)        8 2023-04-13 19:39:59.000000 zillion-0.9.9/zillion.egg-info/top_level.txt
```

### Comparing `zillion-0.9.8/LICENSE` & `zillion-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/PKG-INFO` & `zillion-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: zillion
-Version: 0.9.8
-Summary: Make sense of it all.
-Home-page: https://github.com/totalhack/zillion
-Author: totalhack
-Author-email: none@none.com
-Maintainer: totalhack
-License: LGPLv3
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: mysql
-Provides-Extra: postgres
-Provides-Extra: duckdb
-Provides-Extra: nlp
-Provides-Extra: dev
-Provides-Extra: complete
-License-File: LICENSE
-License-File: AUTHORS.md
-
 Zillion: Make sense of it all
 =============================
 
 [![Generic badge](https://img.shields.io/badge/Status-Alpha-yellow.svg)](https://shields.io/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: LGPLv3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://opensource.org/licenses/LGPL-3.0)
 ![Python 3](https://img.shields.io/badge/python-3-blue.svg)
@@ -275,14 +251,44 @@
 * QDRANT_HOST
 * OPENAI_API_KEY
 
 Embeddings will be produced and stored in both Qdrant and a local cache. The
 vector database will be initialized the first time you try to use this by
 analyzing all fields in your warehouse. An example docker file to run Qdrant is provided in the root of this repo.
 
+You have some control over how fields get embedded. Namely in the configuration for any field you can choose whether to exclude a field from embeddings or override which embeddings map to that field. All fields are
+included by default. The following example would exclude the `net_revenue` field from being embedded and map `revenue` metric requests to the `gross_revenue` field. This type of control becomes useful as your data
+model gets more complex and you want to guide the NLP logic in cases where it could confuse similarly named fields.
+
+```javascript
+{
+    "name": "gross_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            // enabled defaults to true
+            "embedding_text": "revenue" // str or list of str
+        }
+    }
+},
+{
+    "name": "net_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            "enabled": false
+        }
+    }
+},
+```
+
 > *Note:* This feature is in its infancy. It's usefulness will depend on the
 quality of both the input query and your data model (i.e. good field names).
 
 <a name="zillion-configuration"></a>
 
 ### **Zillion Configuration**
 
@@ -838,9 +844,7 @@
 
 Please See the
 [contributing](https://github.com/totalhack/zillion/blob/master/CONTRIBUTING.md)
 guide for more information. If you are looking for inspiration, adding support and tests for additional database technologies would be a great help.
 
 
 
-
-
```

### Comparing `zillion-0.9.8/README.md` & `zillion-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: zillion
+Version: 0.9.9
+Summary: Make sense of it all. Data modeling and analytics with a sprinkle of AI.
+Home-page: https://github.com/totalhack/zillion
+Author: totalhack
+Author-email: none@none.com
+Maintainer: totalhack
+License: LGPLv3
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: mysql
+Provides-Extra: postgres
+Provides-Extra: duckdb
+Provides-Extra: nlp
+Provides-Extra: dev
+Provides-Extra: complete
+License-File: LICENSE
+License-File: AUTHORS.md
+
 Zillion: Make sense of it all
 =============================
 
 [![Generic badge](https://img.shields.io/badge/Status-Alpha-yellow.svg)](https://shields.io/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: LGPLv3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://opensource.org/licenses/LGPL-3.0)
 ![Python 3](https://img.shields.io/badge/python-3-blue.svg)
@@ -251,14 +275,44 @@
 * QDRANT_HOST
 * OPENAI_API_KEY
 
 Embeddings will be produced and stored in both Qdrant and a local cache. The
 vector database will be initialized the first time you try to use this by
 analyzing all fields in your warehouse. An example docker file to run Qdrant is provided in the root of this repo.
 
+You have some control over how fields get embedded. Namely in the configuration for any field you can choose whether to exclude a field from embeddings or override which embeddings map to that field. All fields are
+included by default. The following example would exclude the `net_revenue` field from being embedded and map `revenue` metric requests to the `gross_revenue` field. This type of control becomes useful as your data
+model gets more complex and you want to guide the NLP logic in cases where it could confuse similarly named fields.
+
+```javascript
+{
+    "name": "gross_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            // enabled defaults to true
+            "embedding_text": "revenue" // str or list of str
+        }
+    }
+},
+{
+    "name": "net_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            "enabled": false
+        }
+    }
+},
+```
+
 > *Note:* This feature is in its infancy. It's usefulness will depend on the
 quality of both the input query and your data model (i.e. good field names).
 
 <a name="zillion-configuration"></a>
 
 ### **Zillion Configuration**
 
@@ -814,7 +868,9 @@
 
 Please See the
 [contributing](https://github.com/totalhack/zillion/blob/master/CONTRIBUTING.md)
 guide for more information. If you are looking for inspiration, adding support and tests for additional database technologies would be a great help.
 
 
 
+
+
```

### Comparing `zillion-0.9.8/setup.py` & `zillion-0.9.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 }
 extras_require["complete"] = sorted(set(sum(extras_require.values(), [])))
 
 exec(open("zillion/version.py").read())
 
 setup(
     name="zillion",
-    description="Make sense of it all.",
+    description="Make sense of it all. Data modeling and analytics with a sprinkle of AI.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/totalhack/zillion",
     author="totalhack",
     author_email="none@none.com",
     maintainer="totalhack",
     version=__version__,
```

### Comparing `zillion-0.9.8/zillion/configs.py` & `zillion-0.9.9/zillion/configs.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/core.py` & `zillion-0.9.9/zillion/core.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/datasource.py` & `zillion-0.9.9/zillion/datasource.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/dialects/conversions.py` & `zillion-0.9.9/zillion/dialects/conversions.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/dialects/duckdb.py` & `zillion-0.9.9/zillion/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/dialects/mysql.py` & `zillion-0.9.9/zillion/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/dialects/postgresql.py` & `zillion-0.9.9/zillion/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/dialects/sqlite.py` & `zillion-0.9.9/zillion/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/field.py` & `zillion-0.9.9/zillion/field.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/model.py` & `zillion-0.9.9/zillion/model.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/nlp.py` & `zillion-0.9.9/zillion/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,20 +548,29 @@
     """
     collection_name = get_warehouse_collection_name(warehouse)
     fields = warehouse.get_fields()
 
     texts = []
     metadatas = []
     for name, fdef in fields.items():
-        emb_text = field_name_to_embedding_text(name)
-        if fdef.meta and fdef.meta.get("embedding_text", None):
+        settings = (fdef.meta or {}).get("nlp", {}) or {}
+        if settings.get("enabled", True) is False:
+            continue
+
+        if settings.get("embedding_text", None):
             # Allow overriding the default embedding text
-            emb_text = fdef.meta["embedding_text"]
-        texts.append(emb_text)
-        metadatas.append({"name": name, "field_type": fdef.field_type})
+            emb_texts = settings["embedding_text"]
+            if isinstance(emb_texts, str):
+                emb_texts = [emb_texts]
+        else:
+            emb_texts = [field_name_to_embedding_text(name)]
+
+        for emb_text in emb_texts:
+            texts.append(emb_text)
+            metadatas.append({"name": name, "field_type": fdef.field_type})
 
     start = time.time()
     info(
         f"Initializing {len(fields)} Warehouse embeddings in collection {collection_name}..."
     )
     embeddings_api.add_texts(
         collection_name=collection_name, texts=texts, metadatas=metadatas
```

### Comparing `zillion-0.9.8/zillion/report.py` & `zillion-0.9.9/zillion/report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/scripts/bootstrap_datasource_config.py` & `zillion-0.9.9/zillion/scripts/bootstrap_datasource_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/scripts/load_config.py` & `zillion-0.9.9/zillion/scripts/load_config.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/scripts/run_report.py` & `zillion-0.9.9/zillion/scripts/run_report.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/sql_utils.py` & `zillion-0.9.9/zillion/sql_utils.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion/warehouse.py` & `zillion-0.9.9/zillion/warehouse.py`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion.egg-info/PKG-INFO` & `zillion-0.9.9/zillion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zillion
-Version: 0.9.8
-Summary: Make sense of it all.
+Version: 0.9.9
+Summary: Make sense of it all. Data modeling and analytics with a sprinkle of AI.
 Home-page: https://github.com/totalhack/zillion
 Author: totalhack
 Author-email: none@none.com
 Maintainer: totalhack
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -275,14 +275,44 @@
 * QDRANT_HOST
 * OPENAI_API_KEY
 
 Embeddings will be produced and stored in both Qdrant and a local cache. The
 vector database will be initialized the first time you try to use this by
 analyzing all fields in your warehouse. An example docker file to run Qdrant is provided in the root of this repo.
 
+You have some control over how fields get embedded. Namely in the configuration for any field you can choose whether to exclude a field from embeddings or override which embeddings map to that field. All fields are
+included by default. The following example would exclude the `net_revenue` field from being embedded and map `revenue` metric requests to the `gross_revenue` field. This type of control becomes useful as your data
+model gets more complex and you want to guide the NLP logic in cases where it could confuse similarly named fields.
+
+```javascript
+{
+    "name": "gross_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            // enabled defaults to true
+            "embedding_text": "revenue" // str or list of str
+        }
+    }
+},
+{
+    "name": "net_revenue",
+    "type": "numeric(10,2)",
+    "aggregation": "sum",
+    "rounding": 2,
+    "meta": {
+        "nlp": {
+            "enabled": false
+        }
+    }
+},
+```
+
 > *Note:* This feature is in its infancy. It's usefulness will depend on the
 quality of both the input query and your data model (i.e. good field names).
 
 <a name="zillion-configuration"></a>
 
 ### **Zillion Configuration**
```

### Comparing `zillion-0.9.8/zillion.egg-info/SOURCES.txt` & `zillion-0.9.9/zillion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zillion-0.9.8/zillion.egg-info/requires.txt` & `zillion-0.9.9/zillion.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pymysql~=1.0.2
 pyyaml~=5.4.1
 simplejson~=3.17.0
 stopit~=1.1.2
 sqlalchemy<2,>=1.3
 sqlparse~=0.3.1
 tabulate~=0.8.7
-tlbx~=0.1.19
+tlbx~=0.1.20
 xlrd~=1.2.0
 
 [complete]
 black
 duckdb-engine~=0.7.0
 duckdb~=0.7.1
 jinja2<3.1.0
```

