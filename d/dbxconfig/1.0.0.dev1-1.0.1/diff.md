# Comparing `tmp/dbxconfig-1.0.0.dev1.tar.gz` & `tmp/dbxconfig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.0.dev1.tar", last modified: Sun Apr 16 22:18:14 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.1.tar", last modified: Sun Apr 16 23:37:20 2023, max compression
```

## Comparing `dbxconfig-1.0.0.dev1.tar` & `dbxconfig-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.027414 dbxconfig-1.0.0.dev1/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1697 2023-04-16 22:18:14.027281 dbxconfig-1.0.0.dev1/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     1120 2023-04-16 20:57:36.000000 dbxconfig-1.0.0.dev1/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.025633 dbxconfig-1.0.0.dev1/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3356 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2416 2023-04-16 22:17:46.000000 dbxconfig-1.0.0.dev1/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3428 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.0.dev1/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 22:18:14.027012 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     1697 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 22:18:14.000000 dbxconfig-1.0.0.dev1/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 22:18:14.027464 dbxconfig-1.0.0.dev1/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1074 2023-04-16 22:16:47.000000 dbxconfig-1.0.0.dev1/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.518117 dbxconfig-1.0.1/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:37:20.517979 dbxconfig-1.0.1/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.1/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.516695 dbxconfig-1.0.1/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      404 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3422 2023-04-16 23:34:52.000000 dbxconfig-1.0.1/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2815 2023-04-16 23:36:39.000000 dbxconfig-1.0.1/dbxconfig/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4752 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/_source.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4012 2023-04-16 23:36:39.000000 dbxconfig-1.0.1/dbxconfig/_table_index.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1812 2023-04-16 22:11:37.000000 dbxconfig-1.0.1/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-16 23:37:20.517785 dbxconfig-1.0.1/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      372 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.1/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-16 23:37:20.000000 dbxconfig-1.0.1/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-16 23:37:20.518164 dbxconfig-1.0.1/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-16 23:37:06.000000 dbxconfig-1.0.1/setup.py
```

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_config.py` & `dbxconfig-1.0.1/dbxconfig/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 
         return table_mapping
 
     def _get_stage_config(self, table: Table, timeslice: Timeslice):
         stage_config = self.config[table.stage.name]
         stage_config[self._TIMESLICE] = timeslice
         stage_config[self._TABLE] = table.name
+        stage_config["table_properties"] = table.table_properties
 
         return stage_config
 
     def link_checkpoint(
         self,
         source: Union[Source, DeltaLake],
         destination: DeltaLake,
```

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_deltalake.py` & `dbxconfig-1.0.1/dbxconfig/_deltalake.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     container: str = Field(...)
     root: str = Field(...)
     path: str = Field(...)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint: str = Field(default=None)
+    table_properties: Dict[str, str] = Field(default=None)
 
     def _render(self):
         self._replacements = {
             JinjaVariables.TABLE: self.destination_table,
             JinjaVariables.DATABASE: self.database,
             JinjaVariables.CONTAINER: self.container,
             JinjaVariables.CHECKPOINT: self.checkpoint,
@@ -43,23 +44,31 @@
         if self.options:
             for option, value in self.options.items():
                 self.options[option] = render_jinja(value, self._replacements)
 
         self.location = os.path.join(self.root, self.path)
 
     def create_table(self):
+        table_ddl = f"""
+            CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
+            USING DELTA
+            LOCATION '{self.location}'
+        """
+        # add in the delta properties if there are any
+        if self.table_properties:
+            tbl_properties = [
+                f"{k.lower()} = {v.lower()}" for k, v in self.table_properties.items()
+            ]
+            tbl_properties = ", ".join(tbl_properties)
+            table_ddl = f"""{table_ddl}
+            TBLPROPERTIES({tbl_properties})
+            """
         try:
             spark.sql(f"CREATE DATABASE IF NOT EXISTS `{self.database}`")  # noqa F821
-            spark.sql(  # noqa F821
-                f"""
-                    CREATE TABLE IF NOT EXISTS `{self.database}`.`{self.table}`
-                    USING DELTA
-                    LOCATION '{self.location}'
-                    """
-            )
+            spark.sql(table_ddl)  # noqa F821
         except NameError:
             version = os.getenv("DATABRICKS_RUNTIME_VERSION", None)
             if version:
                 raise Exception("Spark undefined on databricks runtime!")
             logging.warning(
                 "spark is not defined, skipping Spark operation for testing purposes"
             )
```

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_source.py` & `dbxconfig-1.0.1/dbxconfig/_source.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_table_index.py` & `dbxconfig-1.0.1/dbxconfig/_table_index.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 class Table(BaseTable):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     depends_on: List[str] = Field(default=[])
+    table_properties: Dict[str, str] = Field(default=None)
 
 
 class TableMapping(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     destination: Table = Field(...)
@@ -41,36 +42,46 @@
 class Tables(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._load_index()
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
+    table_properties: Dict[str, str] = Field(default=None)
 
     @classmethod
     def get_index(
         cls,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
     ):
         return f"{stage.name}.{database}.{table}"
 
     def _load_index(self):
         for stage in StageType:
             stage_data = self.table_data.get(stage.value)
             if stage_data:
+                stage_table_properties = stage_data.get("table_properties", {})
+
                 for database, tables in stage_data.items():
+                    if database == "table_properties":
+                        continue
+
                     for table, table_details in tables.items():
                         # flatten the config structure for a table
                         if not table_details:
                             table_details = {}
+                        table_properties = table_details.get("table_properties", {})
+                        table_properties = stage_table_properties | table_properties
                         table_details["name"] = table
                         table_details["database"] = database
                         table_details["stage"] = stage
+                        if table_properties:
+                            table_details["table_properties"] = table_properties
 
                         # create a table object
                         table = Table(**table_details)
 
                         # index the table object
                         index = f"{stage.value}.{database}.{table.name}"
                         self.tables_index[index] = table
```

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_timeslice.py` & `dbxconfig-1.0.1/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.0.dev1/dbxconfig/_utils.py` & `dbxconfig-1.0.1/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.0.dev1/setup.py` & `dbxconfig-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.0.dev1",
+    version="1.0.1",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

