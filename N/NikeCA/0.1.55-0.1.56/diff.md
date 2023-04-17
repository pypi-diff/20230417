# Comparing `tmp/NikeCA-0.1.55.tar.gz` & `tmp/NikeCA-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.55.tar", last modified: Mon Apr 17 07:42:59 2023, max compression
+gzip compressed data, was "NikeCA-0.1.56.tar", last modified: Mon Apr 17 08:02:46 2023, max compression
```

## Comparing `NikeCA-0.1.55.tar` & `NikeCA-0.1.56.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.017375 NikeCA-0.1.55/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.55/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 07:42:59.016931 NikeCA-0.1.55/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.55/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 07:42:59.017488 NikeCA-0.1.55/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 07:39:52.000000 NikeCA-0.1.55/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.014511 NikeCA-0.1.55/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:42:59.016462 NikeCA-0.1.55/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 07:42:58.000000 NikeCA-0.1.55/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19652 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3743 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.55/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     2244 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 07:35:54.000000 NikeCA-0.1.55/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.406652 NikeCA-0.1.56/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.56/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:02:46.406247 NikeCA-0.1.56/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.56/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 08:02:46.406784 NikeCA-0.1.56/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 08:02:14.000000 NikeCA-0.1.56/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.403210 NikeCA-0.1.56/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.405609 NikeCA-0.1.56/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    20795 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3816 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.56/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2244 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/__init__.py
```

### Comparing `NikeCA-0.1.55/LICENSE` & `NikeCA-0.1.56/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/PKG-INFO` & `NikeCA-0.1.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.55
+Version: 0.1.56
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.55/README.md` & `NikeCA-0.1.56/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/setup.py` & `NikeCA-0.1.56/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.55',
+	version='0.1.56',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_Dashboards",
```

### Comparing `NikeCA-0.1.55/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.56/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.55
+Version: 0.1.56
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.55/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.56/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/NikeQA.py` & `NikeCA-0.1.56/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/NikeSF.py` & `NikeCA-0.1.56/src/NikeSF.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 
 from _SnowflakeData import SnowflakeData
 from _BuildSearchQuery import BuildSearchQuery
 from _SnowflakeDependencies import SnowflakeDependencies
 from _Dashboards import Dashboards
+from _InclusionExclusion import InclusionExclusion
 
 
-class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):
+class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery, InclusionExclusion):
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
     def __init__(self, username: str, warehouse: str, role: str, database: str = None, schema: str = None,
@@ -527,9 +528,34 @@
         if polars is False:
             polars = self.__polars
 
         return Dashboards.imp_summary_dashboard(self, username=username, warehouse=warehouse, database=database
                                                 , role=role, date_min=date_min, date_max=date_max,
                                                 column_filters=column_filters, polars=polars)
 
+    def pos_data_quality_review(self
+                                , username: str
+                                , warehouse: str
+                                , database: str
+                                , role: str
+                                , columns=None
+                                , filters=None
+                                , order_by=None
+                                , polars: bool = False):
+
+        if username is None:
+            username = self.__username
+        if warehouse is None:
+            warehouse = self.__warehouse
+        if database is None:
+            database = self.__database
+        if role is None:
+            role = self.__role
+        if polars is False:
+            polars = self.__polars
+
+        return InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
+                                                          database=database, role=role, columns=columns,
+                                                          filters=filters, order_by=order_by, polars=polars)
+
```

### Comparing `NikeCA-0.1.55/src/_BuildSearchQuery.py` & `NikeCA-0.1.56/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_Dashboards.py` & `NikeCA-0.1.56/src/_Dashboards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 
-class Dashboards:
+from _InclusionExclusion import InclusionExclusion
+
+
+class Dashboards(InclusionExclusion):
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.1.55/src/_GitHub.py` & `NikeCA-0.1.56/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_IMPSummaryDashboard.py` & `NikeCA-0.1.56/src/_IMPSummaryDashboard.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_InclusionExclusion.py` & `NikeCA-0.1.56/src/_InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_QA.py` & `NikeCA-0.1.56/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_SearchFiles.py` & `NikeCA-0.1.56/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_SnowflakeData.py` & `NikeCA-0.1.56/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_SnowflakeDependencies.py` & `NikeCA-0.1.56/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.55/src/_SnowflakePull.py` & `NikeCA-0.1.56/src/_SnowflakePull.py`

 * *Files identical despite different names*

