# Comparing `tmp/NikeCA-0.1.54.tar.gz` & `tmp/NikeCA-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.54.tar", last modified: Mon Apr 10 21:20:06 2023, max compression
+gzip compressed data, was "NikeCA-0.1.55.tar", last modified: Mon Apr 17 07:42:59 2023, max compression
```

## Comparing `NikeCA-0.1.54.tar` & `NikeCA-0.1.55.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:20:06.199159 NikeCA-0.1.54/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.54/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 21:20:06.198855 NikeCA-0.1.54/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.54/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-10 21:20:06.199291 NikeCA-0.1.54/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2254 2023-04-10 21:19:38.000000 NikeCA-0.1.54/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:20:06.196495 NikeCA-0.1.54/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:20:06.198471 NikeCA-0.1.54/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-10 21:20:06.000000 NikeCA-0.1.54/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      426 2023-04-10 21:20:06.000000 NikeCA-0.1.54/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-10 21:20:06.000000 NikeCA-0.1.54/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-10 21:20:06.000000 NikeCA-0.1.54/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      147 2023-04-10 21:20:06.000000 NikeCA-0.1.54/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19706 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3205 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14125 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6490 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-10 21:17:23.000000 NikeCA-0.1.54/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.017375 NikeCA-0.1.55/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.55/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 07:42:59.016931 NikeCA-0.1.55/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.55/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 07:42:59.017488 NikeCA-0.1.55/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 07:39:52.000000 NikeCA-0.1.55/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.014511 NikeCA-0.1.55/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.016462 NikeCA-0.1.55/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19652 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3743 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.55/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2244 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/__init__.py
```

### Comparing `NikeCA-0.1.54/LICENSE` & `NikeCA-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/PKG-INFO` & `NikeCA-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.54
+Version: 0.1.55
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.54/README.md` & `NikeCA-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/setup.py` & `NikeCA-0.1.55/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.54',
+	version='0.1.55',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
-		"_IMPSummaryDashboard",
+		"_Dashboards",
+		"_InclusionExclusion",
 		"_SearchFiles",
 		"_SnowflakeDependencies",
 		"_SnowflakePull",
 		"NikeQA",
 		"_QA",
 		"_GitHub",
 		"NikeCA"
```

### Comparing `NikeCA-0.1.54/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.55/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.54
+Version: 0.1.55
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.54/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.55/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/NikeQA.py` & `NikeCA-0.1.55/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/NikeSF.py` & `NikeCA-0.1.55/src/NikeSF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
-from _IMPSummaryDashboard import IMPSummaryDashboard
+from _Dashboards import Dashboards
 
 
-class Snowflake(SnowflakeData, IMPSummaryDashboard, SnowflakeDependencies, BuildSearchQuery):
+class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
@@ -523,13 +523,13 @@
         if date_max is None:
             date_max = self.__date_max
         if column_filters is None:
             column_filters = self.__column_filters
         if polars is False:
             polars = self.__polars
 
-        return IMPSummaryDashboard.imp_summary_dashboard(self, username=username, warehouse=warehouse, database=database
-                                                         , role=role, date_min=date_min, date_max=date_max,
-                                                         column_filters=column_filters, polars=polars)
+        return Dashboards.imp_summary_dashboard(self, username=username, warehouse=warehouse, database=database
+                                                , role=role, date_min=date_min, date_max=date_max,
+                                                column_filters=column_filters, polars=polars)
```

### Comparing `NikeCA-0.1.54/src/_BuildSearchQuery.py` & `NikeCA-0.1.55/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/_GitHub.py` & `NikeCA-0.1.55/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/_IMPSummaryDashboard.py` & `NikeCA-0.1.55/src/_IMPSummaryDashboard.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/_QA.py` & `NikeCA-0.1.55/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.54/src/_SearchFiles.py` & `NikeCA-0.1.55/src/_SearchFiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,38 +51,43 @@
 
             # Recursively search through the directory
             for root, dirs, files in os.walk(directory_path):
                 for file in files:
                     # Get the relative path for the file
                     path = os.path.relpath(os.path.join(root, file), directory_path)
                     filepath = path
+                    print(f"Searching:\t{filepath}/{file}")
 
                     with open(os.path.join(root, file), 'rb') as f:
                         byte_sequence = f.read()  # read the first 100 bytes
                         lines = byte_sequence.decode('iso-8859-1')
 
-                        indexes = [index.start() for index in re.finditer(i.upper(), lines.upper())]
+                        if f'{i.upper()} ' in lines.upper():
+                            print('test')
 
-                        df[i][filepath] = {}
-                        df[i][filepath]['Start'] = lines[:1000]
-                        df[i][filepath]['char_index'] = {}
-
-                        instance = 1
-                        for index in indexes:
-                            if index < 250:
-                                index = 250
-                            instance += 1
+                            indexes = [index.start() for index in re.finditer(i.upper(), lines.upper())]
 
-                            df[i][filepath]['char_index'][str(index)] = lines[index - 250: index + 250]
+                            instance = 1
+                            for index in indexes:
+                                if index < 100:
+                                    index = 100
+                                instance += 1
+                                if 'pos'.upper() not in lines[index - 10: index].upper():
+                                    df[i][filepath] = {}
+                                    df[i][filepath]['Start'] = lines[:500]
+                                    df[i][filepath]['char_index'] = {}
+                                    df[i][filepath]['char_index'][str(index)] = lines[index - 100: index + 100]
 
             print(i)
 
         reformed_dict = {}
         for k, v in df.items():
             for x, y in v.items():
                 reformed_dict[(k, x)] = y
 
         df_pd = pd.DataFrame(reformed_dict).T
 
         df_pd.to_csv(save_path)
 
+        print(df_pd)
+
         return df_pd
```

### Comparing `NikeCA-0.1.54/src/_SnowflakeData.py` & `NikeCA-0.1.55/src/_SnowflakeData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import _BuildSearchQuery
 import _SnowflakePull
 import _SnowflakeDependencies
-import _IMPSummaryDashboard
+import _Dashboards
 
 
-class SnowflakeData(_IMPSummaryDashboard.IMPSummaryDashboard
+class SnowflakeData(_Dashboards.Dashboards
                     , _SnowflakePull.SnowflakePull
                     , _SnowflakeDependencies.SnowflakeDependencies
                     , _BuildSearchQuery.BuildSearchQuery):
 
     def snowflake_pull(self, query: str | dict | None, un, wh, db, role, schema=None, table=None,
                        sample_table: bool = False, sample_val: bool = False, table_sample: dict = None,
                        dtypes_conv=None, separate_dataframes: bool = True, polars: bool = True): # -> pandas.DataFrame:
```

### Comparing `NikeCA-0.1.54/src/_SnowflakeDependencies.py` & `NikeCA-0.1.55/src/_SnowflakeDependencies.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 
 
 class SnowflakeDependencies:
-    import pandas
 
     def snowflake_dependencies(self,
                                tables: str | list,
                                username: str,
                                warehouse: str,
                                role: str,
                                database: str | None = None,
                                schema: str | list | None = None,
                                save_path: str | None = None):
 
         """
         Searches the snowflake database and finds instances where the table is referenced and where the reference is not
             in the actual creation of the table itself
 
-        There are some tables in the databases that do not have any results for the get_ddl(). I have set it to skip
-            these tables
-
-        :param save_path:
-        :param tables: This is a list or string to check for in the database
+        :param save_path: (str | None) The path to save the output.
+        :param tables: (str | list): The list of tables or views to fetch DDL for.
         :param username: username for Snowflake
         :param warehouse: warehouse for Snowflake
         :param role: role for Snowflake
         :param database: database to search in must provide
         :param schema: filling this in can really help to speed up the query
         :return: pandas Dataframe
+
+        This function is used to fetch the DDL of tables and views from Snowflake.
+
+        Parameters:
+            tables (str | list): The list of tables or views to fetch DDL for.
+            username (str): The username of the Snowflake user.
+            warehouse (str): The warehouse to use for the connection.
+            role (str): The role of the Snowflake user.
+            database (str | None): The database to use for the connection.
+            schema (str | list | None): The schema to use for the connection.
+            save_path (str | None): The path to save the output.
+
+        Returns:
+            dict: A dictionary containing the DDL of the tables and views.
         """
 
         # snowflake connection packages:
         import pandas as pd
         import polars as pl
         import snowflake.connector
         import time
```

### Comparing `NikeCA-0.1.54/src/_SnowflakePull.py` & `NikeCA-0.1.55/src/_SnowflakePull.py`

 * *Files identical despite different names*

