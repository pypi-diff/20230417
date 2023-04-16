# Comparing `tmp/dbxconfig-0.1.0.tar.gz` & `tmp/dbxconfig-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-0.1.0.tar", last modified: Sun Apr 16 21:00:18 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.0.dev1.tar", last modified: Sun Apr 16 22:18:14 2023, max compression
```

## Comparing `dbxconfig-0.1.0.tar` & `dbxconfig-1.0.0.dev1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 21:00:18.638229 dbxconfig-0.1.0/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1692 2023-04-16 21:00:18.638124 dbxconfig-0.1.0/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     1120 2023-04-16 20:57:36.000000 dbxconfig-0.1.0/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 21:00:18.637228 dbxconfig-0.1.0/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3356 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2021 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3428 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1811 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 21:00:18.637948 dbxconfig-0.1.0/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1692 2023-04-16 21:00:18.000000 dbxconfig-0.1.0/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 21:00:18.000000 dbxconfig-0.1.0/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 21:00:18.000000 dbxconfig-0.1.0/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 21:00:18.000000 dbxconfig-0.1.0/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 21:00:18.000000 dbxconfig-0.1.0/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 21:00:18.638274 dbxconfig-0.1.0/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-16 20:49:59.000000 dbxconfig-0.1.0/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.027414 dbxconfig-1.0.0.dev1/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1697 2023-04-16 22:18:14.027281 dbxconfig-1.0.0.dev1/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1120 2023-04-16 20:57:36.000000 dbxconfig-1.0.0.dev1/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.025633 dbxconfig-1.0.0.dev1/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3356 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2416 2023-04-16 22:17:46.000000 dbxconfig-1.0.0.dev1/dbxconfig/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_source.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3428 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_table_index.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.0.dev1/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.027012 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1697 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 22:18:14.027464 dbxconfig-1.0.0.dev1/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1074 2023-04-16 22:16:47.000000 dbxconfig-1.0.0.dev1/setup.py
```

### Comparing `dbxconfig-0.1.0/PKG-INFO` & `dbxconfig-1.0.0.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 0.1.0
+Version: 1.0.0.dev1
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-0.1.0/README.md` & `dbxconfig-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-0.1.0/dbxconfig/_config.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_config.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-0.1.0/dbxconfig/_deltalake.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_deltalake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from pydantic import BaseModel, Field, PrivateAttr
 from ._utils import JinjaVariables, render_jinja
 from typing import Any, Dict, Union
 from ._timeslice import Timeslice
-from databricks.sdk.runtime import spark
+
+# from databricks.sdk.runtime import spark
 import os
 
 
 class DeltaLake(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
@@ -42,15 +43,23 @@
         if self.options:
             for option, value in self.options.items():
                 self.options[option] = render_jinja(value, self._replacements)
 
         self.location = os.path.join(self.root, self.path)
 
     def create_table(self):
-        spark.sql(f"CREATE DATABASE IF NOT EXISTS `{self.database}`")
-        spark.sql(
-            f"""
-                CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
-                USING DELTA
-                LOCATION '{self.location}'
-                """
-        )
+        try:
+            spark.sql(f"CREATE DATABASE IF NOT EXISTS `{self.database}`")  # noqa F821
+            spark.sql(  # noqa F821
+                f"""
+                    CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
+                    USING DELTA
+                    LOCATION '{self.location}'
+                    """
+            )
+        except NameError:
+            version = os.getenv("DATABRICKS_RUNTIME_VERSION", None)
+            if version:
+                raise Exception("Spark undefined on databricks runtime!")
+            logging.warning(
+                "spark is not defined, skipping Spark operation for testing purposes"
+            )
```

### Comparing `dbxconfig-0.1.0/dbxconfig/_source.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_source.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-0.1.0/dbxconfig/_table_index.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_table_index.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-0.1.0/dbxconfig/_timeslice.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-0.1.0/dbxconfig/_utils.py` & `dbxconfig-1.0.0.dev1/dbxconfig/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 def get_html_table(data: dict):
     rows = []
     for k, v in data.items():
         if isinstance(v, dict):
             for ki, vi in v.items():
-                row = f"<tr><td>{k}{ki}</td><td>{vi}</td></tr>"
+                row = f"<tr><td>{k}.{ki}</td><td>{vi}</td></tr>"
                 rows.append(row)
         else:
             row = f"<tr><td>{k}</td><td>{v}</td></tr>"
             rows.append(row)
 
     html = "".join(rows)
```

### Comparing `dbxconfig-0.1.0/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.0.dev1/dbxconfig.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 0.1.0
+Version: 1.0.0.dev1
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-0.1.0/setup.py` & `dbxconfig-1.0.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="0.1.0",
+    version="1.0.0.dev1",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

