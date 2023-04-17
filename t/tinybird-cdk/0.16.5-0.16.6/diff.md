# Comparing `tmp/tinybird-cdk-0.16.5.tar.gz` & `tmp/tinybird-cdk-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.16.5.tar", last modified: Fri Apr 14 14:16:06 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.16.6.tar", last modified: Mon Apr 17 07:42:19 2023, max compression
```

## Comparing `tinybird-cdk-0.16.5.tar` & `tinybird-cdk-0.16.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.884620 tinybird-cdk-0.16.5/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 14:15:52.000000 tinybird-cdk-0.16.5/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.880620 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 14:16:06.000000 tinybird-cdk-0.16.5/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.301099 tinybird-cdk-0.16.6/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 07:42:10.000000 tinybird-cdk-0.16.6/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:42:19.297099 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 07:42:19.000000 tinybird-cdk-0.16.6/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.16.5/README.md` & `tinybird-cdk-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/setup.py` & `tinybird-cdk-0.16.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.16.5',
+    version='0.16.6',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.16.5/tests/test_gcp.py` & `tinybird-cdk-0.16.6/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.16.6/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.16.6/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.16.6/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.16.6/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/config.py` & `tinybird-cdk-0.16.6/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connector.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,19 +213,28 @@
         for schema in list(self._query(f'show schemas in database {database}')):
             schemas.append(connector.Scope(name=schema['name'], value=f'{schema["database_name"]}.{schema["name"]}'))
         schemas.sort(key=lambda schema: schema.name)
         return schemas
 
     def _list_tables(self, database, schema):
         tables = []
+
+        # Tables
         for table in list(self._query(f'show tables in {database}.{schema}')):
             tables.append(connector.Table(
                 name=table['name'], value=f'{table["database_name"]}.{table["schema_name"]}.{table["name"]}',
                 num_rows=table['rows'], size=table['bytes']
             ))
+
+        # Views
+        for view in list(self._query(f'show views in {database}.{schema}')):
+            tables.append(connector.Table(
+                name=view['name'], value=f'{view["database_name"]}.{view["schema_name"]}.{view["name"]}'
+            ))
+
         tables.sort(key=lambda table: table.name)
         return tables
 
     #
     # --- Schema Suggestion -----------------------------------------------------------------------
     #
 
@@ -234,14 +243,16 @@
             raise errors.MissingConfiguration('database')
         if not (sf_schema := scopes.get('schema')):
             raise errors.MissingConfiguration('schema')
         if not (table := scopes.get('table')):
             raise errors.MissingConfiguration('table')
 
         suggested_schema = schema.Schema(scopes, table)
+        # In Snowflake, `desc[ribe] table` works for both tables and views.
+        #   https://docs.snowflake.com/en/sql-reference/sql/desc-table#usage-notes
         snowflake_schema = self._query(f'describe table {database}.{sf_schema}.{table}')
         for field in snowflake_schema:
             suggested_schema.columns.append(self._column(field))
 
         return suggested_schema
 
     # https://docs.snowflake.com/en/sql-reference/intro-summary-data-types
```

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.16.6/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/errors.py` & `tinybird-cdk-0.16.6/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/export.py` & `tinybird-cdk-0.16.6/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/formats.py` & `tinybird-cdk-0.16.6/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/logger.py` & `tinybird-cdk-0.16.6/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/migration.py` & `tinybird-cdk-0.16.6/tinybird_cdk/migration.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/schema.py` & `tinybird-cdk-0.16.6/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.16.6/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.16.5/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.16.6/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

