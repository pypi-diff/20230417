# Comparing `tmp/govtech_data-0.1.8.tar.gz` & `tmp/govtech_data-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.8.tar", max compression
+gzip compressed data, was "govtech_data-0.1.9.tar", max compression
```

## Comparing `govtech_data-0.1.8.tar` & `govtech_data-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.8/README.md
--rw-r--r--   0        0        0      869 2023-04-15 07:24:52.383933 govtech_data-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.8/src/govtech_data/__init__.py
--rw-r--r--   0        0        0     4829 2023-04-15 07:23:31.757518 govtech_data-0.1.8/src/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.8/src/govtech_data/models/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-15 06:49:21.541855 govtech_data-0.1.8/src/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.8/src/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.8/src/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.8/src/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.8/src/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.8/src/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.8/src/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      454 2023-04-15 07:24:29.232006 govtech_data-0.1.8/src/govtech_data/utils/content.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 govtech_data-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    15089 2023-04-17 19:29:01.305094 govtech_data-0.1.9/README.md
+-rw-r--r--   0        0        0     1183 2023-04-17 21:10:48.227318 govtech_data-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.9/src/govtech_data/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-17 19:29:01.317137 govtech_data-0.1.9/src/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.9/src/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0     1140 2023-04-17 19:29:01.317390 govtech_data-0.1.9/src/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.9/src/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-15 04:10:21.224681 govtech_data-0.1.9/src/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-15 04:10:21.587789 govtech_data-0.1.9/src/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-15 04:10:21.933080 govtech_data-0.1.9/src/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-15 04:10:22.457596 govtech_data-0.1.9/src/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:29:01.317544 govtech_data-0.1.9/src/govtech_data/prompts/__init__.py
+-rw-r--r--   0        0        0     2488 2023-04-17 19:29:01.317772 govtech_data-0.1.9/src/govtech_data/prompts/task.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.9/src/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0     2338 2023-04-17 19:29:01.317863 govtech_data-0.1.9/src/govtech_data/utils/commands.py
+-rw-r--r--   0        0        0      455 2023-04-17 19:29:01.318030 govtech_data-0.1.9/src/govtech_data/utils/content.py
+-rw-r--r--   0        0        0     9667 2023-04-17 19:29:01.318131 govtech_data-0.1.9/src/govtech_data/utils/openai.py
+-rw-r--r--   0        0        0    16268 1970-01-01 00:00:00.000000 govtech_data-0.1.9/PKG-INFO
```

### Comparing `govtech_data-0.1.8/src/govtech_data/client.py` & `govtech_data-0.1.9/src/govtech_data/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from functools import lru_cache
 from typing import Type, Union
 
 import requests
-
 from fuzzywuzzy import process
 from loguru import logger
+from polars import DataFrame
 from pydantic import BaseModel, validate_arguments
 
-from govtech_data.utils.content import fetch_url, convert_response_to_io
 from govtech_data.models.api import (
     DatastoreSearch,
     PackageShow,
     ResourceShow,
     SearchPackage,
     PackageResourceContent,
     PackageContent,
@@ -19,14 +18,15 @@
 from govtech_data.models.resources.datastore_search import DatastoreSearchModel
 from govtech_data.models.resources.package_list import PackageListModel
 from govtech_data.models.resources.package_show import (
     PackageShowModel,
     Result as PackageShowModelResult,
 )
 from govtech_data.models.resources.resource_show import ResourceShowModel
+from govtech_data.utils.content import fetch_url, convert_response_to_io
 
 API_ENDPOINTS = {
     "ckan_datastore_search": "https://data.gov.sg/api/action/datastore_search",
     "ckan_package_show": "https://data.gov.sg/api/action/package_show",
     "ckan_package_list": "https://data.gov.sg/api/action/package_list",
     "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
 }
@@ -102,15 +102,15 @@
     def get_model_from_json_response(
         cls, url: str, params: dict, model: Type[BaseModel]
     ):
         if url is None:
             raise Exception("url cannot be None!")
         if model is None:
             raise Exception("model cannot be None!")
-        logger.debug(f"endpoint name: {url}")
+        logger.debug(f"endpoint: {url}")
         resp = requests.get(
             url,
             params=params,
             headers=COMMON_HEADERS,
             timeout=DEFAULT_TIMEOUT_IN_SECONDS,
         )
         if not resp.ok:
@@ -144,7 +144,15 @@
             return None
         return PackageContent(
             package=package_show_model.result,
             resources=cls.fetch_resources_from_package_result(
                 package_show_model.result, limit
             ),
         )
+
+    @classmethod
+    @validate_arguments
+    def fetch_dataframe_from_package(cls, package_name: str) -> Union[DataFrame, None]:
+        package_content = cls.fetch_content_from_package(package_name, 1)
+        if len(package_content.resources) == 0:
+            return None
+        return package_content.resources[0].get_dataframe()
```

### Comparing `govtech_data-0.1.8/src/govtech_data/models/api.py` & `govtech_data-0.1.9/src/govtech_data/models/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 
-from pydantic import BaseModel
 import polars as pl
+from pydantic import BaseModel
 
 from govtech_data.models.resources import package_show
 
 INFER_SCHEMA_LENGTH = None  # this does a full table scan, which is slow but acceptible since most datasets are small
 
 
 class PackageShow(BaseModel):
@@ -37,13 +37,18 @@
     content: io.StringIO
 
     class Config:
         arbitrary_types_allowed = True
 
     def get_dataframe(self):
         self.content.seek(0)
-        return pl.read_csv(self.content, infer_schema_length=INFER_SCHEMA_LENGTH)
+        return pl.read_csv(
+            self.content,
+            quote_char=None,
+            use_pyarrow=True,
+            infer_schema_length=INFER_SCHEMA_LENGTH,
+        )
 
 
 class PackageContent(BaseModel):
     package: package_show.Result
     resources: list[PackageResourceContent] | None
```

### Comparing `govtech_data-0.1.8/src/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.9/src/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.8/src/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.9/src/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.8/src/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.9/src/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

