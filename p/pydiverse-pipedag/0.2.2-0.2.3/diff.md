# Comparing `tmp/pydiverse-pipedag-0.2.2.tar.gz` & `tmp/pydiverse-pipedag-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-pipedag-0.2.2.tar", max compression
+gzip compressed data, was "pydiverse-pipedag-0.2.3.tar", max compression
```

## Comparing `pydiverse-pipedag-0.2.2.tar` & `pydiverse-pipedag-0.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.2.2/LICENSE
--rw-r--r--   0        0        0     7028 2023-03-31 15:18:57.054051 pydiverse-pipedag-0.2.2/docs/package/README.md
--rw-r--r--   0        0        0     2822 2023-03-31 15:34:58.725245 pydiverse-pipedag-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       61 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5323 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0    10555 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    19418 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7232 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    62955 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0    40372 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     6241 2023-02-07 12:13:02.783303 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    24913 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5714 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8433 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     4246 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     7739 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    16598 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/util/__init__.py
--rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/util/cache.py
--rw-r--r--   0        0        0     3647 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/util/json.py
--rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0    14721 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/config.py
--rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0      818 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     9052 2023-03-31 15:41:36.459154 pydiverse-pipedag-0.2.2/setup.py
--rw-r--r--   0        0        0     8954 2023-03-31 15:41:36.459662 pydiverse-pipedag-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7028 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/docs/package/README.md
+-rw-r--r--   0        0        0     2822 2023-04-17 10:30:00.401257 pydiverse-pipedag-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       61 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5323 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/lock.py
+-rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    19418 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0     7232 2023-03-31 15:18:57.058051 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0    65364 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/sql.py
+-rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
+-rw-r--r--   0        0        0    40372 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
+-rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     6241 2023-02-07 12:13:02.783303 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    24901 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8463 2023-04-17 10:28:16.433476 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     4246 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     7739 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    16598 2023-03-31 15:18:57.066051 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/__init__.py
+-rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/cache.py
+-rw-r--r--   0        0        0     3647 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/json.py
+-rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0    14721 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/config.py
+-rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0      818 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     9052 2023-04-17 10:30:13.052195 pydiverse-pipedag-0.2.3/setup.py
+-rw-r--r--   0        0        0     8954 2023-04-17 10:30:13.052739 pydiverse-pipedag-0.2.3/PKG-INFO
```

### Comparing `pydiverse-pipedag-0.2.2/LICENSE` & `pydiverse-pipedag-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/docs/package/README.md` & `pydiverse-pipedag-0.2.3/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/pyproject.toml` & `pydiverse-pipedag-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.2.2"
+version = "0.2.3"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/_typing.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/blob.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/lock.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/lock.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import copy
 import itertools
 import json
 import re
 import textwrap
 import threading
+import time
 import traceback
 import warnings
 from collections.abc import Iterable
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
@@ -236,14 +237,22 @@
                 "create_database_if_not_exists is only implemented for postgres, yet"
             )
         engine.dispose()
 
     @staticmethod
     def _connect(engine_url, schema_prefix, schema_suffix):
         engine = sa.create_engine(engine_url)
+        # if engine.dialect.name == "ibm_db_sa":
+        #     engine.dispose()
+        #     # switch to READ STABILITY isolation level to avoid unnecessary deadlock
+        #     # victims in case of background operations when reflecting columns
+        #     engine = sa.create_engine(
+        #         engine_url, execution_options={"isolation_level": "RS"}
+        #     )
+
         if engine.dialect.name == "mssql":
             engine.dispose()
             # this is needed to allow for CREATE DATABASE statements
             # (we don't rely on database transactions anyways)
             engine = sa.create_engine(engine_url, connect_args={"autocommit": True})
 
         if engine.dialect.name == "mssql":
@@ -388,17 +397,27 @@
         schema: Schema,
         key_columns: list[str],
         *,
         name: str | None = None,
         early_not_null_possible: bool = False,
     ):
         if not early_not_null_possible:
-            self.execute(
-                ChangeColumnNullable(table_name, schema, key_columns, nullable=False)
-            )
+            for retry_iteration in range(4):
+                # retry operation since it might have been terminated as a
+                # deadlock victim
+                try:
+                    self.execute(
+                        ChangeColumnNullable(
+                            table_name, schema, key_columns, nullable=False
+                        )
+                    )
+                except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+                    if retry_iteration == 3:
+                        raise
+                    time.sleep(retry_iteration * retry_iteration * 1.1)
         self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
 
     # @add_index.dialect("ibm_db_sa")
     # def _add_index_ibm_db_sa(
     #     self, table_name: str, schema: Schema, index: list[str],
     #     name: str | None = None
     # ):
@@ -438,18 +457,18 @@
             self.add_index(
                 dest_table, dest_schema, index["column_names"], index["name"]
             )
 
     def reflect_sql_types(
         self, col_names: Iterable[str], table_name: str, schema: Schema
     ):
-        meta = sa.MetaData()
-        meta.reflect(bind=self.engine, schema=schema.get())
-        tables = {table.name: table for table in meta.tables.values()}
-        sql_types = [tables[table_name].c[col].type for col in col_names]
+        inspector = sa.inspect(self.engine)
+        columns = inspector.get_columns(table_name, schema=schema.get())
+        types = {d["name"]: d["type"] for d in columns}
+        sql_types = [types[col] for col in col_names]
         return sql_types
 
     @staticmethod
     def format_sql_string(query_str: str) -> str:
         return textwrap.dedent(query_str).strip()
 
     @engine_dispatch
@@ -589,19 +608,24 @@
                 self.drop_all_dialect_specific(schema=transaction_schema)
             else:
                 self.execute(cs_base, conn=conn)
                 self.execute(ds_trans, conn=conn)
                 self.execute(cs_trans, conn=conn)
 
             if not self.disable_caching:
-                conn.execute(
-                    self.tasks_table.delete()
-                    .where(self.tasks_table.c.stage == stage.name)
-                    .where(self.tasks_table.c.in_transaction_schema.in_([True]))
-                )
+                for table in [
+                    self.tasks_table,
+                    self.lazy_cache_table,
+                    self.raw_sql_cache_table,
+                ]:
+                    conn.execute(
+                        table.delete()
+                        .where(table.c.stage == stage.name)
+                        .where(table.c.in_transaction_schema)
+                    )
 
     @_init_stage_schema_swap.dialect("mssql")
     def _init_stage_schema_swap_mssql(self, stage: Stage):
         if "." not in self.schema_suffix:
             return self._init_stage_schema_swap.original(self, stage)
 
         schema = self.get_schema(stage.name)
@@ -656,19 +680,24 @@
                 self.execute(
                     DropAlias(name, transaction_schema, if_exists=True),
                     conn=conn,
                 )
 
             # Clear metadata
             if not self.disable_caching:
-                conn.execute(
-                    self.tasks_table.delete()
-                    .where(self.tasks_table.c.stage == stage.name)
-                    .where(self.tasks_table.c.in_transaction_schema.in_([True]))
-                )
+                for table in [
+                    self.tasks_table,
+                    self.lazy_cache_table,
+                    self.raw_sql_cache_table,
+                ]:
+                    conn.execute(
+                        table.delete()
+                        .where(table.c.stage == stage.name)
+                        .where(table.c.in_transaction_schema)
+                    )
 
     def _init_stage_read_views(self, stage: Stage):
         try:
             with self.engine.connect() as conn:
                 metadata_rows = (
                     conn.execute(
                         self.stage_table.select().where(
@@ -803,15 +832,15 @@
                 self.tasks_table,
                 self.lazy_cache_table,
                 self.raw_sql_cache_table,
             ]:
                 conn.execute(
                     table.delete()
                     .where(table.c.stage == stage.name)
-                    .where(table.c.in_transaction_schema.in_([False]))
+                    .where(~table.c.in_transaction_schema)
                 )
                 conn.execute(
                     table.update()
                     .where(table.c.stage == stage.name)
                     .values(in_transaction_schema=False)
                 )
 
@@ -839,15 +868,15 @@
                 f"Failed to copy table '{table.name}' (schema: '{stage.name}')"
                 " to transaction."
             )
             self.logger.error(
                 msg
                 + " This error is treated as cache-lookup-failure and thus we can"
                 " continue.",
-                exception="\n".join(traceback.format_exception(_e)),
+                exception=traceback.format_exc(),
             )
             raise CacheError(msg) from _e
         self.add_indexes(table, self.get_schema(stage.transaction_name))
 
     def deferred_copy_lazy_table_to_transaction(
         self, src_name: str, src_stage: Stage, table: Table
     ):
@@ -873,14 +902,21 @@
                 )
             )
         except Exception as _e:
             msg = (
                 f"Failed to copy lazy table {src_name} (schema:"
                 f" '{src_schema}' -> '{dest_schema}') to transaction."
             )
+            self.logger.error(
+                "Exception in table copy in background",
+                thread=thread_id,
+                table=src_name,
+                msg=msg,
+                exception=str(_e),
+            )
             raise RuntimeError(msg) from _e
         table = copy.deepcopy(table)
         table.name = "__cpy_" + src_name
         self.add_indexes(
             table, self.get_schema(stage.transaction_name), early_not_null_possible=True
         )
         self.logger.info(
@@ -948,15 +984,15 @@
                 table,
             )
         except Exception as _e:
             msg = (
                 f"Failed to copy lazy table {metadata.name} (schema:"
                 f" '{metadata.stage}') to transaction."
             )
-            self.logger.error(msg, exception="\n".join(traceback.format_exception(_e)))
+            self.logger.error(msg, exception=traceback.format_exc())
             raise CacheError(msg) from _e
 
     @engine_dispatch
     def get_view_names(self, schema: str, *, include_everything=False) -> list[str]:
         """
         List all views that are present in a schema.
 
@@ -1048,15 +1084,15 @@
                     f"Failed to copy raw sql generated table {table_name} (schema:"
                     f" '{src_schema}') to transaction."
                 )
                 self.logger.error(
                     msg
                     + " This error is treated as cache-lookup-failure and thus we can"
                     " continue.",
-                    exception="\n".join(traceback.format_exception(_e)),
+                    exception=traceback.format_exc(),
                 )
                 raise CacheError(msg) from _e
 
         views_to_copy = new_tables & set(views)
         for view_name in views_to_copy:
             self._copy_view_to_transaction(view_name, src_schema, dest_schema)
 
@@ -1391,50 +1427,76 @@
         store.add_indexes(table, schema, early_not_null_possible=True)
 
     @classmethod
     def retrieve(cls, store, table, stage_name, as_type):
         table_name = table.name
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_aliases(table_name, schema)
-        return sa.Table(
-            table_name,
-            sa.MetaData(bind=store.engine),
-            schema=schema,
-            autoload_with=store.engine,
-        )
+        for retry_iteration in range(4):
+            # retry operation since it might have been terminated as a deadlock victim
+            try:
+                tbl = sa.Table(
+                    table_name,
+                    sa.MetaData(),
+                    schema=schema,
+                    autoload_with=store.engine,
+                )
+            except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+                if retry_iteration == 3:
+                    raise
+                time.sleep(retry_iteration * retry_iteration * 1.2)
+        return tbl
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
-        return str(obj.compile(store.engine, compile_kwargs={"literal_binds": True}))
+        if isinstance(obj, sa.sql.selectable.FromClause):
+            query = sa.select([sa.text("*")]).select_from(obj)
+        else:
+            query = obj
+        query_str = str(
+            query.compile(store.engine, compile_kwargs={"literal_binds": True})
+        )
+        # hacky way to canonicalize query (despite __tmp/__even/__odd suffixes
+        # and alias resolution)
+        query_str = re.sub(
+            r"(__tmp|__even|__odd)(?=[ \t\n.;]|$)", "", query_str.lower()
+        )
+        query_str = re.sub(r'["\[\]]', "", query_str)
+        return query_str
 
 
 def _resolve_alias_ibm_db_sa(conn, table_name: str, schema: str, *, _iteration=0):
     # TODO: consider speeding this up by caching information for complete schemas
     #  instead of running at least two queries per source table; Ultimately problem can
     #  also be fixed by upstream contribution to ibm_db_sa
 
     # we need to resolve aliases since pandas.read_sql_table does not work for them
     # and sa.Table does not auto-reflect columns
     table_name = ibm_db_sa_fix_name(table_name)
     schema = ibm_db_sa_fix_name(schema)
-    tbl = sa.Table("TABLES", sa.MetaData(), schema="SYSCAT", autoload_with=conn)
+    tbl = sa.Table("SYSTABLES", sa.MetaData(), schema="SYSIBM", autoload_with=conn)
     query = (
-        sa.select([tbl.c.base_tabname, tbl.c.base_tabschema])
+        sa.select([tbl.c.base_name, tbl.c.base_schema])
         .select_from(tbl)
         .where(
-            (tbl.c.tabschema == schema)
-            & (tbl.c.tabname == table_name)
-            & (tbl.c.TYPE == "A")
+            (tbl.c.creator == schema) & (tbl.c.name == table_name) & (tbl.c.TYPE == "A")
         )
     )
-    row = conn.execute(query).mappings().one_or_none()
+    for retry_iteration in range(4):
+        # retry operation since it might have been terminated as a deadlock victim
+        try:
+            row = conn.execute(query).mappings().one_or_none()
+        except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+            if retry_iteration == 3:
+                raise
+            time.sleep(retry_iteration * retry_iteration)
     if row is not None:
         assert _iteration < 3, f"Unexpected recursion looking up {schema}.{table_name}"
         table_name, schema = _resolve_alias_ibm_db_sa(
-            conn, row["base_tabname"], row["base_tabschema"], _iteration=_iteration + 1
+            conn, row["base_name"], row["base_schema"], _iteration=_iteration + 1
         )
     return table_name, schema
 
 
 def _resolve_alias_mssql(conn, table_name: str, schema: str, *, _iteration=0):
     # TODO: consider speeding this up by caching information for complete schemas
     #  instead of running at least two queries per source table; Ultimately problem can
@@ -1515,16 +1577,15 @@
         store.add_indexes(table, schema)
 
     @classmethod
     def retrieve(cls, store, table, stage_name, as_type):
         schema = store.get_schema(stage_name).get()
         with store.engine.connect() as conn:
             table_name = table.name
-            if store.engine.dialect.name == "ibm_db_sa":
-                table_name, schema = _resolve_alias_ibm_db_sa(conn, table_name, schema)
+            table_name, schema = store.resolve_aliases(table_name, schema)
             df = pd.read_sql_table(table_name, conn, schema=schema)
             return df
 
     @classmethod
     def auto_table(cls, obj: pd.DataFrame):
         if name := obj.attrs.get("name"):
             return Table(obj, name)
```

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/backend/table/util/sql_ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/context/context.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/context.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/context/run_context.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/context/run_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             op = getattr(self, op_name)
             if not callable(op) or op_name[0] == "_":
                 raise TypeError(f"OP '{op_name}' is not allowed on RunContextServer")
 
             result = op(*args)
             return [None, result]
         except Exception as e:
-            exception_str = "\n".join(traceback.format_exception(e))
+            exception_str = traceback.format_exc()
             try:
                 pickled_exception = pickle.dumps(e)
             except Exception as e2:
                 self.logger.error(
                     "failed pickling exception",
                     exception=exception_str,
                     pickle_exception=str(e2),
@@ -333,16 +333,16 @@
             stage_id in self._deferred_table_store_ops
             and len(self._deferred_table_store_ops[stage_id]) > 0
         ):
             if len(self._deferred_table_store_op_threads.get(stage_id, {})) == 0:
                 self._deferred_table_store_op_threads[stage_id] = {}
                 started_ops_end = 0
             else:
-                started_ops_end = max(
-                    self._deferred_table_store_op_threads[stage_id].keys()
+                started_ops_end = (
+                    max(self._deferred_table_store_op_threads[stage_id].keys()) + 1
                 )
             store = self.config_ctx.store
             for i, (op, commit_op, args, kwargs) in enumerate(
                 self._deferred_table_store_ops[stage_id][started_ops_end:]
             ):
                 _id = started_ops_end + i
                 fn = getattr(store.table_store, op)
```

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/flow.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/result.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/stage.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/core/task.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/base.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             store.copy_lazy_table_to_transaction(metadata, table)
             store.logger.info(f"Lazy cache of table '{table.name}' found")
             table.name = metadata.name
             is_cache_valid = True
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
-            store.logger.warning("cache miss", exception=str(e))
+            store.logger.warning("cache miss", table=table.name, exception=str(e))
             is_cache_valid = False
 
         # Store metadata
         store.store_lazy_table_metadata(
             LazyTableMetadata(
                 name=table.name,
                 stage=table.stage.name,
@@ -194,15 +194,15 @@
             )
             store.copy_raw_sql_tables_to_transaction(metadata, raw_sql.stage)
             store.logger.info(f"Lazy cache of stage '{raw_sql.stage}' found")
             is_cache_valid = True
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
-            store.logger.warning("cache miss", exception=str(e))
+            store.logger.warning("cache miss for raw-SQL", exception=str(e))
             is_cache_valid = False
         return TableCacheInfo(raw_sql.stage, task_hash, query_hash, is_cache_valid)
 
     @staticmethod
     def task_cache_key(task: MaterializingTask, input_hash: str, cache_fn_hash: str):
         """Cache key used to judge cache validity of the current task output.
```

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/container.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/container.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/core.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/store.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/util/cache.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/materialize/util/json.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/materialize/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/config.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/config.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/disposable.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/import_.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/ipc.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/src/pydiverse/pipedag/util/naming.py` & `pydiverse-pipedag-0.2.3/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.2.2/setup.py` & `pydiverse-pipedag-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'ibm_db2': ['ibm-db>=3.1.4', 'ibm-db-sa>=0.3.8'],
  'mssql': ['pyodbc>=4.0.35', 'pytsql>=1.1.4'],
  'prefect': ['prefect>=1.3,<2'],
  'zookeeper': ['kazoo>=2.8.0']}
 
 setup_kwargs = {
     'name': 'pydiverse-pipedag',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.',
     'long_description': '# pydiverse.pipedag\n\n[![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)\n\nA pipeline orchestration library executing tasks within one python session. It takes care of SQL table\n(de)materialization, caching and cache invalidation. Blob storage is supported as well for example\nfor storing model files.\n\nThis is an early stage version 0.x which lacks documentation. Please contact\nhttps://github.com/orgs/pydiverse/teams/code-owners if you like to become an early adopter\nor to contribute early stage usage examples.\n\n## Usage\n\npydiverse.pipedag can either be installed via pypi with `pip install pydiverse-pipedag` or via conda-forge\nwith `conda install pydiverse-pipedag -c conda-forge`.\n\n## Example\n\nA flow can look like this (i.e. put this in a file named `run_pipeline.py`):\n\n```python\nfrom pydiverse.pipedag import materialize, Table, Flow, Stage\nimport sqlalchemy as sa\nimport pandas as pd\n\nfrom pydiverse.pipedag.context import StageLockContext, RunContext\nfrom pydiverse.pipedag.util import setup_structlog\n\n\n@materialize(lazy=True)\ndef lazy_task_1():\n    return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_2(input1: sa.Table, input2: sa.Table):\n    query = sa.select([(input1.c.x * 5).label("x5"), input2.c.a]).select_from(\n        input1.outerjoin(input2, input2.c.x == input1.c.x)\n    )\n    return Table(query, name="task_2_out", primary_key=["a"])\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_3(input: sa.Table, my_stage: Stage):\n    return sa.text(f"SELECT * FROM {my_stage.transaction_name}.{input.name}")\n\n\n@materialize(lazy=True, input_type=sa.Table)\ndef lazy_task_4(input: sa.Table, prev_stage: Stage):\n    return sa.text(f"SELECT * FROM {prev_stage.name}.{input.name}")\n\n\n@materialize(nout=2, version="1.0.0")\ndef eager_inputs():\n    dfA = pd.DataFrame(\n        {\n            "a": [0, 1, 2, 4],\n            "b": [9, 8, 7, 6],\n        }\n    )\n    dfB = pd.DataFrame(\n        {\n            "a": [2, 1, 0, 1],\n            "x": [1, 1, 2, 2],\n        }\n    )\n    return Table(dfA, "dfA"), Table(dfB, "dfB_%%")\n\n\n@materialize(version="1.0.0", input_type=pd.DataFrame)\ndef eager_task(tbl1: pd.DataFrame, tbl2: pd.DataFrame):\n    return tbl1.merge(tbl2, on="x")\n\n\ndef main():\n    with Flow() as f:\n        with Stage("stage_1"):\n            lazy_1 = lazy_task_1()\n            a, b = eager_inputs()\n\n        with Stage("stage_2") as stage2:\n            lazy_2 = lazy_task_2(lazy_1, b)\n            lazy_3 = lazy_task_3(lazy_2, stage2)\n            eager = eager_task(lazy_1, b)\n\n        with Stage("stage_3"):\n            lazy_4 = lazy_task_4(lazy_2, stage2)\n        _ = lazy_3, lazy_4, eager  # unused terminal output tables\n\n    # Run flow\n    result = f.run()\n    assert result.successful\n\n    # Run in a different way for testing\n    with StageLockContext():\n        result = f.run()\n        assert result.successful\n        assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1\n\n\nif __name__ == "__main__":\n    # initialize logging\n    setup_structlog()\n    main()\n```\n\nCreate a file called `pipedag.yaml` in the same directory:\n\n```yaml\nname: pipedag_tests\ntable_store_connections:\n  postgres:\n    # Postgres: this can be used after running `docker-compose up`\n    url: "postgresql://{$POSTGRES_USERNAME}:{$POSTGRES_PASSWORD}@127.0.0.1:6543/{instance_id}"\n\ninstances:\n  __any__:\n    # listen-interface for pipedag context server which synchronizes some task state during DAG execution\n    network_interface: "127.0.0.1"\n    # classes to be materialized to table store even without pipedag Table wrapper (we have loose coupling between\n    # pipedag and pydiverse.transform, so consider adding \'pydiverse.transform.Table\' in your config)\n    auto_table: ["pandas.DataFrame", "sqlalchemy.sql.elements.TextClause", "sqlalchemy.sql.selectable.Selectable"]\n    fail_fast: true\n\n    instance_id: pipedag_default\n    table_store:\n      class: "pydiverse.pipedag.backend.table.SQLTableStore"\n\n      # Postgres: this can be used after running `docker-compose up`\n      table_store_connection: postgres\n      create_database_if_not_exists: True\n\n      # print select statements before being encapsualted in materialize expressions and tables before writing to\n      # database\n      print_materialize: true\n      # print final sql statements\n      print_sql: true\n\n    blob_store:\n      class: "pydiverse.pipedag.backend.blob.FileBlobStore"\n      base_path: "/tmp/pipedag/blobs"\n\n    lock_manager:\n      class: "pydiverse.pipedag.backend.lock.ZooKeeperLockManager"\n      hosts: "localhost:2181"\n\n    orchestration:\n      class: "pydiverse.pipedag.engine.SequentialEngine"\n```\n\nIf you don\'t have a postgres, Microsoft SQL Server, or IBM DB2 database at hand, you can\nstart a postgres database with the following `docker-compose.yaml` file:\n\n```yaml\nversion: "3.9"\nservices:\n  postgres:\n    image: postgres\n    environment:\n      POSTGRES_USER: sa\n      POSTGRES_PASSWORD: Pydiverse23\n      POSTGRES_PORT: 6543\n    ports:\n      - 6543:5432\n  zoo:\n    image: zookeeper\n    environment:\n      ZOO_4LW_COMMANDS_WHITELIST: ruok\n      ZOO_MAX_CLIENT_CNXNS: 100\n    ports:\n      - 2181:2181\n```\n\nRun `docker-compose up` in the directory of your `docker-compose.yaml` and then execute\nthe flow script as follows with a shell like `bash` and a python environment that\nincludes `pydiverse-pipedag`, `pandas`, and `sqlalchemy`:\n\n```bash\nexport POSTGRES_USERNAME=sa\nexport POSTGRES_PASSWORD=Pydiverse23\npython run_pipeline.py\n```\n\nFinally, you may connect to your localhost postgres database `pipedag_default` and\nlook at tables in schemas `stage_1`..`stage_3`.\n\nIf you don\'t have a SQL UI at hand, you may use `psql` command line tool inside the docker container.\nCheck out the `NAMES` column in `docker ps` output. If the name of your postgres container is\n`example_postgres_1`, then you can look at output tables like this:\n\n```bash\ndocker exec example_postgres_1 psql --username=sa --dbname=pipedag_default -c \'select * from stage_1.dfa;\'\n```\n\nOr more interactively:\n\n```bash\ndocker exec -t -i example_postgres_1 bash\npsql --username=sa --dbname=pipedag_default\n\\dt stage_*.*\nselect * from stage_2.task_2_out;\n```\n\n## Troubleshooting\n\n### Installing mssql odbc driver for linux\n\nInstalling with\ninstructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)\nworked.\nBut `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings\nits own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the\nproblem. Try `python -c \'import pyodbc;print(pyodbc.drivers())\'` and see whether you get more than an empty list.\nFurthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.\n',
     'author': 'QuantCo, Inc.',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pydiverse-pipedag-0.2.2/PKG-INFO` & `pydiverse-pipedag-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.2.2
+Version: 0.2.3
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

