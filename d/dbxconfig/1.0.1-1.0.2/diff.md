# Comparing `tmp/dbxconfig-1.0.1.tar.gz` & `tmp/dbxconfig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.1.tar", last modified: Sun Apr 16 23:37:20 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.2.tar", last modified: Sun Apr 16 23:43:47 2023, max compression
```

## Comparing `dbxconfig-1.0.1.tar` & `dbxconfig-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.518117 dbxconfig-1.0.1/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:37:20.517979 dbxconfig-1.0.1/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.1/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.516695 dbxconfig-1.0.1/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3422 2023-04-16 23:34:52.000000 dbxconfig-1.0.1/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2815 2023-04-16 23:36:39.000000 dbxconfig-1.0.1/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4012 2023-04-16 23:36:39.000000 dbxconfig-1.0.1/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.1/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.517785 dbxconfig-1.0.1/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 23:37:20.518164 dbxconfig-1.0.1/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-16 23:37:06.000000 dbxconfig-1.0.1/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:43:47.615721 dbxconfig-1.0.2/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:43:47.615586 dbxconfig-1.0.2/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.2/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:43:47.614521 dbxconfig-1.0.2/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-1.0.2/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3410 2023-04-16 23:42:22.000000 dbxconfig-1.0.2/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2771 2023-04-16 23:37:54.000000 dbxconfig-1.0.2/dbxconfig/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-1.0.2/dbxconfig/_source.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4012 2023-04-16 23:36:39.000000 dbxconfig-1.0.2/dbxconfig/_table_index.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.2/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.2/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:43:47.615392 dbxconfig-1.0.2/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:43:47.000000 dbxconfig-1.0.2/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 23:43:47.000000 dbxconfig-1.0.2/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 23:43:47.000000 dbxconfig-1.0.2/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.2/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 23:43:47.000000 dbxconfig-1.0.2/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 23:43:47.000000 dbxconfig-1.0.2/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 23:43:47.615781 dbxconfig-1.0.2/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-16 23:43:36.000000 dbxconfig-1.0.2/setup.py
```

### Comparing `dbxconfig-1.0.1/PKG-INFO` & `dbxconfig-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.1/README.md` & `dbxconfig-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.1/dbxconfig/_config.py` & `dbxconfig-1.0.2/dbxconfig/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,17 @@
                     table_mapping.source[name] = Source(**stage_config)
                 if table_obj.stage != StageType.landing:
                     table_mapping.source[name] = DeltaLake(**stage_config)
 
         elif isinstance(table_mapping.source, Table):
             stage_config = self._get_stage_config(table_mapping.source, timeslice)
             if table_mapping.source.stage == StageType.landing:
-                table_mapping.source[name] = Source(**stage_config)
+                table_mapping.source = Source(**stage_config)
             if table_mapping.source.stage != StageType.landing:
-                table_mapping.source[name] = DeltaLake(**stage_config)
+                table_mapping.source = DeltaLake(**stage_config)
 
         stage_config = self._get_stage_config(table_mapping.destination, timeslice)
         if table_mapping.destination.stage in (StageType.base, StageType.raw):
             table_mapping.destination = DeltaLake(**stage_config)
         else:
             raise Exception(
                 f"Table mapping destinations must be {StageType.raw} ro {StageType.base}"
```

### Comparing `dbxconfig-1.0.1/dbxconfig/_deltalake.py` & `dbxconfig-1.0.2/dbxconfig/_deltalake.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import logging
 from pydantic import BaseModel, Field, PrivateAttr
 from ._utils import JinjaVariables, render_jinja
 from typing import Any, Dict, Union
 from ._timeslice import Timeslice
-
-# from databricks.sdk.runtime import spark
 import os
 
 
 class DeltaLake(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
```

### Comparing `dbxconfig-1.0.1/dbxconfig/_source.py` & `dbxconfig-1.0.2/dbxconfig/_source.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.1/dbxconfig/_table_index.py` & `dbxconfig-1.0.2/dbxconfig/_table_index.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.1/dbxconfig/_timeslice.py` & `dbxconfig-1.0.2/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.1/dbxconfig/_utils.py` & `dbxconfig-1.0.2/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.1/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.2/dbxconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.1/setup.py` & `dbxconfig-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.1",
+    version="1.0.2",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

