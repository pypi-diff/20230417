# Comparing `tmp/dbxconfig-1.0.3.tar.gz` & `tmp/dbxconfig-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.3.tar", last modified: Mon Apr 17 12:58:47 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.4.tar", last modified: Mon Apr 17 14:47:02 2023, max compression
```

## Comparing `dbxconfig-1.0.3.tar` & `dbxconfig-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 12:58:47.720231 dbxconfig-1.0.3/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 12:58:47.720112 dbxconfig-1.0.3/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.3/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 12:58:47.719095 dbxconfig-1.0.3/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      428 2023-04-17 12:50:14.000000 dbxconfig-1.0.3/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3482 2023-04-17 12:57:34.000000 dbxconfig-1.0.3/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2840 2023-04-17 12:57:48.000000 dbxconfig-1.0.3/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4821 2023-04-17 12:57:48.000000 dbxconfig-1.0.3/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      110 2023-04-17 12:57:48.000000 dbxconfig-1.0.3/dbxconfig/_stage_type.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4187 2023-04-17 12:57:48.000000 dbxconfig-1.0.3/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.3/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.3/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 12:58:47.719942 dbxconfig-1.0.3/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 12:58:47.000000 dbxconfig-1.0.3/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      397 2023-04-17 12:58:47.000000 dbxconfig-1.0.3/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-17 12:58:47.000000 dbxconfig-1.0.3/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.3/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-17 12:58:47.000000 dbxconfig-1.0.3/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-17 12:58:47.000000 dbxconfig-1.0.3/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-17 12:58:47.720287 dbxconfig-1.0.3/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-17 12:58:22.000000 dbxconfig-1.0.3/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 14:47:02.424171 dbxconfig-1.0.4/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 14:47:02.424053 dbxconfig-1.0.4/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.4/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 14:47:02.423100 dbxconfig-1.0.4/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      428 2023-04-17 12:50:14.000000 dbxconfig-1.0.4/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3482 2023-04-17 12:57:34.000000 dbxconfig-1.0.4/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2840 2023-04-17 12:57:48.000000 dbxconfig-1.0.4/dbxconfig/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4821 2023-04-17 12:57:48.000000 dbxconfig-1.0.4/dbxconfig/_source.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      110 2023-04-17 12:57:48.000000 dbxconfig-1.0.4/dbxconfig/_stage_type.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4187 2023-04-17 12:57:48.000000 dbxconfig-1.0.4/dbxconfig/_table_index.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.4/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.4/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 14:47:02.423887 dbxconfig-1.0.4/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 14:47:02.000000 dbxconfig-1.0.4/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      397 2023-04-17 14:47:02.000000 dbxconfig-1.0.4/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-17 14:47:02.000000 dbxconfig-1.0.4/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.4/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-17 14:47:02.000000 dbxconfig-1.0.4/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-17 14:47:02.000000 dbxconfig-1.0.4/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-17 14:47:02.424219 dbxconfig-1.0.4/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-17 14:46:30.000000 dbxconfig-1.0.4/setup.py
```

### Comparing `dbxconfig-1.0.3/PKG-INFO` & `dbxconfig-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.3
+Version: 1.0.4
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.3/README.md` & `dbxconfig-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_config.py` & `dbxconfig-1.0.4/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_deltalake.py` & `dbxconfig-1.0.4/dbxconfig/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_source.py` & `dbxconfig-1.0.4/dbxconfig/_source.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_table_index.py` & `dbxconfig-1.0.4/dbxconfig/_table_index.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_timeslice.py` & `dbxconfig-1.0.4/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.3/dbxconfig/_utils.py` & `dbxconfig-1.0.4/dbxconfig/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import jinja2
 from enum import Enum
 import yaml
 from pyspark.sql.types import StructType
+from typing import Dict
 
 
 class JinjaVariables(Enum):
     DATABASE = "database"
     TABLE = "table"
     CHECKPOINT = "checkpoint"
     FILENAME_DATE_FORMAT = "filename_date_format"
     PATH_DATE_FORMAT = "path_date_format"
     CONTAINER = "container"
 
 
-def render_jinja(data: str, replacements: dict[JinjaVariables, str]):
+def render_jinja(data: str, replacements: Dict[JinjaVariables, str]):
     if data and isinstance(data, str):
         replace = {k.value: v for (k, v) in replacements.items()}
         skip = False
         for k, v in replace.items():
             if v is None and "{{" + k + "}}" in data.replace(" ", ""):
                 skip = True
                 break
```

### Comparing `dbxconfig-1.0.3/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.4/dbxconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.3
+Version: 1.0.4
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.3/setup.py` & `dbxconfig-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.3",
+    version="1.0.4",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

