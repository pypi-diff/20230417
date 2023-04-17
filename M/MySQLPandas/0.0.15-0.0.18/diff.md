# Comparing `tmp/MySQLPandas-0.0.15.tar.gz` & `tmp/MySQLPandas-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySQLPandas-0.0.15.tar", last modified: Tue Apr 11 06:50:02 2023, max compression
+gzip compressed data, was "MySQLPandas-0.0.18.tar", last modified: Fri Apr 14 06:51:00 2023, max compression
```

## Comparing `MySQLPandas-0.0.15.tar` & `MySQLPandas-0.0.18.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:50:02.823801 MySQLPandas-0.0.15/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    18092 2023-04-11 06:04:32.000000 MySQLPandas-0.0.15/LICENSE
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-11 04:33:53.000000 MySQLPandas-0.0.15/MANIFEST.in
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:50:02.806801 MySQLPandas-0.0.15/MySQLPandas/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      294 2023-04-11 06:49:55.000000 MySQLPandas-0.0.15/MySQLPandas/__init__.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    13341 2023-04-10 05:49:22.000000 MySQLPandas-0.0.15/MySQLPandas/core.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:50:02.817801 MySQLPandas-0.0.15/MySQLPandas/lib/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-04-07 05:18:00.000000 MySQLPandas-0.0.15/MySQLPandas/lib/DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-03-27 05:45:36.000000 MySQLPandas-0.0.15/MySQLPandas/lib/ErrorClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-03-27 05:12:58.000000 MySQLPandas-0.0.15/MySQLPandas/lib/__init__.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:50:02.813801 MySQLPandas-0.0.15/MySQLPandas.egg-info/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2537 2023-04-11 06:50:02.000000 MySQLPandas-0.0.15/MySQLPandas.egg-info/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-04-11 06:50:02.000000 MySQLPandas-0.0.15/MySQLPandas.egg-info/SOURCES.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-04-11 06:50:02.000000 MySQLPandas-0.0.15/MySQLPandas.egg-info/dependency_links.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       45 2023-04-11 06:50:02.000000 MySQLPandas-0.0.15/MySQLPandas.egg-info/requires.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-04-11 06:50:02.000000 MySQLPandas-0.0.15/MySQLPandas.egg-info/top_level.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2537 2023-04-11 06:50:02.821801 MySQLPandas-0.0.15/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1894 2023-04-11 06:49:51.000000 MySQLPandas-0.0.15/README.md
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-04-11 06:50:02.823801 MySQLPandas-0.0.15/setup.cfg
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1893 2023-04-11 06:10:37.000000 MySQLPandas-0.0.15/setup.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-11 06:50:02.820801 MySQLPandas-0.0.15/tests/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.15/tests/test_DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.15/tests/test_coreClass.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.546800 MySQLPandas-0.0.18/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    18092 2023-04-11 06:04:32.000000 MySQLPandas-0.0.18/LICENSE
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-14 06:31:32.000000 MySQLPandas-0.0.18/MANIFEST.in
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.534800 MySQLPandas-0.0.18/MySQLPandas/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      294 2023-04-14 06:50:35.000000 MySQLPandas-0.0.18/MySQLPandas/__init__.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    14088 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/core.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.542800 MySQLPandas-0.0.18/MySQLPandas/lib/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/ErrorClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/__init__.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.539801 MySQLPandas-0.0.18/MySQLPandas.egg-info/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3464 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       58 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/requires.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/top_level.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3464 2023-04-14 06:51:00.545800 MySQLPandas-0.0.18/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2821 2023-04-14 06:50:30.000000 MySQLPandas-0.0.18/README.md
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-04-14 06:51:00.546800 MySQLPandas-0.0.18/setup.cfg
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1893 2023-04-11 06:10:37.000000 MySQLPandas-0.0.18/setup.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.544800 MySQLPandas-0.0.18/tests/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.18/tests/test_DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.18/tests/test_coreClass.py
```

### Comparing `MySQLPandas-0.0.15/LICENSE` & `MySQLPandas-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.15/MySQLPandas/core.py` & `MySQLPandas-0.0.18/MySQLPandas/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 import getpass
 import os
 import sys
 import time
+from tqdm import tqdm
 from configparser import ConfigParser
 from mysql.connector import MySQLConnection
 from typing import Optional
 
 from MySQLPandas.lib.DataFrameClass import DataframeProcessing,TwoDataframesProcessing
 from MySQLPandas.lib.ErrorClass import PandasMySQLError
 #mysql-python-connector=8.0.29
@@ -99,14 +100,15 @@
             When it disconnects DB.
         """
         con = self
         if con.is_connected():
             print("Connected to the database")
         else:
             raise PandasMySQLError("something went wrong.")
+        self.__catchwaringshow()
 
     def showTableList(self) -> None:
         """
         Display exist table name list.  
 
         Parameters
         ----------
@@ -115,14 +117,16 @@
         Returns
         ----------
         None
         """
         self.__catchTableList()
         for DBname in self.DBList:
             print(DBname)
+        self.__catchwaringshow()
+        
     
     def showTableinfo(self,table_name:str) -> None:
         """
         Display table column definition.
 
         Parameters
         ----------
@@ -135,14 +139,15 @@
         Raises
         ----------
         PandasMySQLError
             Input not existing table name.
         """
         self.__catchTableInfo(table_name=table_name)
         print(self.table_info)
+        self.__catchwaringshow()
     
     def deleteTable(self,table_name:str) -> None:
         """
         Delete Table.
 
         Parameters
         ----------
@@ -156,14 +161,15 @@
         ----------
         PandasMySQLError
             Input not existing table name.
         """        
         con = self
         cursor = con.cursor()
         cursor.execute(f"drop table {table_name};")
+        self.__catchwaringshow()
 
     def makeTable(
             self,
             table_name: str,
             df_path: Optional[str] = None,
             df:Optional[pd.DataFrame] = None,
             converters:Optional[dict] = None,
@@ -206,14 +212,15 @@
             sep=sep,
             converters = converters)
         df_object.makeDBFrame()
         df_object.makeTableSQLcommand()
         con = self
         cursor = con.cursor()
         cursor.execute(df_object.sql_command)
+        self.__catchwaringshow()
     
     def insertRecord(
             self,
             table_name: str,
             df_path: Optional[str] = None,
             df:Optional[pd.DataFrame] = None,
             converters:Optional[dict] = None,
@@ -274,15 +281,15 @@
         #is match insert data and exist data
         dfs_obj = TwoDataframesProcessing(
             df_exist=df_exist.df_for_command,
             df_insert=df_insert.df_for_command)
         status_message = dfs_obj.isEqualDataFrames(Strict_Mode=Strict_Mode)
         match status_message:
             case "continue":
-                __insertRecordBuffer(
+                _insertRecordBuffer(
                     self,
                     table_name = table_name,
                     df = df,
                     df_path = df_path,
                     sep=sep,
                     converters = converters
                     )
@@ -301,15 +308,15 @@
                     try:
                         cursor.execute(sql_command)
                         con.commit()
                     except Exception as e:
                         con.rollback()
                         raise PandasMySQLError(e)
                 
-                __insertRecordBuffer(
+                _insertRecordBuffer(
                     self,
                     table_name = table_name,
                     df = df,
                     df_path = df_path,
                     sep=sep,
                     converters = converters
                     )
@@ -336,14 +343,15 @@
         Returns
         ----------
         None
         """ 
         con = self
         cursor = con.cursor()
         cursor.execute(f"alter table {table_name} add primary key ({primary_key});")
+        self.__catchwaringshow()
     
     def deletePrimaryKey(self,table_name:str) -> None:
         """
         Delete PrimaryKey.
 
         Parameters
         ----------
@@ -352,14 +360,15 @@
         Return
         ----------
         None
         """ 
         con = self
         cursor = con.cursor()
         cursor.execute(f"alter table {table_name} drop primary key;")
+        self.__catchwaringshow()
 
     def __catchTableInfo(self,table_name:str) -> None:
         con = self
         cursor = con.cursor()
         cursor.execute(f"show columns from {table_name}")
         rows = cursor.fetchall()
         self.table_info = pd.DataFrame(
@@ -372,33 +381,42 @@
         con = self
         cursor = con.cursor()
         cursor.execute("show tables;")
         rows = cursor.fetchall()
         for row in rows:
             self.DBList.append(row[0])
     
+    def __catchwaringshow(self) -> Optional[pd.DataFrame]:
+        con = self
+        cursor = con.cursor()
+        cursor.execute('show warnings;')
+        warn_state = pd.DataFrame(cursor.fetchall())
+        if not warn_state.empty:
+            print(warn_state)
+
     def executeSQLcommand(self,command:str) -> pd.DataFrame:
         """
         Execute SQL command and return DataFrame object
 
         Parameters
         ----------
         command:str
 
         Return
         ----------
-        None
+        DataFrame
         """ 
         con = self
         cursor = con.cursor()
         try:
             cursor.execute(command)
         except Exception as e:
             raise PandasMySQLError(e)
         result = cursor.fetchall()
+        self.__catchwaringshow()
         return pd.DataFrame(result)
 
     #debug
     def isNullTableNameinTableList(self,table_name:str) -> bool:
         """
         For debug. If self.DBList is None, it return True.
         """
@@ -409,15 +427,15 @@
             return False
 
     def __exit__(self, exc_type, exc_value, traceback):
         return super().__exit__(exc_type, exc_value, traceback)
 
 
 #tools
-def __insertRecordBuffer(
+def _insertRecordBuffer(
         self:MySQLPandas,
         table_name: str,
         df_path: Optional[str] = None,
         df:Optional[pd.DataFrame] = None,
         converters:Optional[dict] = None,
         sep:str = ","
         ):
@@ -432,22 +450,29 @@
     record_list.makeRecordSQLcommand()
 
     con = self
     con.autocommit = False
     cursor = con.cursor()
     
     rep = 0
+    #make progress bar object
+    pbar = tqdm(total=((len(record_list.list_for_command)//1000)+1)*1000)
+
     while not rep >= len(record_list.list_for_command):   
         split_list_for_command = record_list.list_for_command[rep:rep+1000]
         rep += 1000
+        pbar.update(1000)
         try:
             cursor.executemany(record_list.sql_command,split_list_for_command)
             con.commit()
+
+            #print if MySQL output some error.
+            cursor.execute('show warnings;')
+            warn_state = pd.DataFrame(cursor.fetchall())
+            if not warn_state.empty:
+                print(warn_state)
+            
             time.sleep(1.0)
         except Exception as e:
             con.rollback()
             raise PandasMySQLError(e)
-        percentile = round((rep * 100)/len(record_list.list_for_command))
-        if percentile < 100:
-            print(f"{percentile}% complete.")
-        else:
-            print("100% complete")
+    pbar.close()
```

### Comparing `MySQLPandas-0.0.15/MySQLPandas/lib/DataFrameClass.py` & `MySQLPandas-0.0.18/MySQLPandas/lib/DataFrameClass.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.15/MySQLPandas.egg-info/PKG-INFO` & `MySQLPandas-0.0.18/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,13 @@
-Metadata-Version: 2.1
-Name: MySQLPandas
-Version: 0.0.15
-Summary: MySQLPandas: simple connector between MySQL(MariaDB) and Pandas
-Home-page: https://github.com/Sota-Nakashima/MySQLPandas
-Author: Sota-Nakashima
-Author-email: souta.nakashima2001@gmail.com
-License: GPLv2
-Keywords: Python,Pandas,Database
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![PyPI](https://img.shields.io/badge/PyPI-0.0.15-blue)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![GNU GPLv2](http://img.shields.io/badge/license-GNU_GPLv2-blue.svg?style=flat)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
+[![PyPI](https://img.shields.io/badge/PyPI-0.0.18-blue)](https://pypi.org/project/MySQLPandas/)
+[![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
 The tool supports MySQL or MariaDB as the database engine.
@@ -34,24 +17,42 @@
 from MySQLPandas.core import MySQLPandas
 with MySQLPandas("hoge","hoge_db",initfile_path="hoge.ini") as obj:
     obj.makeTable("sample_table",df_path="sample.csv")
     obj.showTableinfo("sample_table")
     obj.insertRecord("sample_table",df_path="sample.csv")
 ```
 
-About other functions, see [here](https://sota-nakashima.github.io/MySQLPandas/MySQLPandas.html).
+Regarding other functions, see [here](https://sota-nakashima.github.io/MySQLPandas/MySQLPandas.html).
+
+## Note
+In MySQLPandas function of insertRecord, it doesn't allow any difference on table denfinition.(If it has slightly differcence, MySQLPandas raise error.)  
+```
+raise PandasMySQLError("Not match Table frame")
+MySQLPandas.lib.ErrorClass.PandasMySQLError: Not match Table frame
+```
+If you want to change table definition, please see below.  
+* Change string type column  
+  You can change table denfiniton automatically. Please rewrite  "Strict_Mode = False" in "insertRecord" method.
+* Change int or float type column  
+  Sorry, you can't change it in MySQLPandas. Please rewrite it by using "executeSQLcommand" method. 
+
+## Setup password.ini
+In default, you need to input DB password in your console every time.  
+If you felt bothered, you avoid this by creating "password.ini" file.  
+In GitHub page, it's put [sample file](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/password_sample.ini).
 ## Requirement
 * MySQL(MariaDB)  
 The version of Auther's MariaDB is 5.5.68-MariaDB MariaDB Server.  
 Don't try the newest version so please check your MariaDB version.
 * Pandas <= 1.5.3
 * Python 3.*
 * mysql-connector-python <= 8.0.29
+* tqdm <= 4.65.0
 
-## Pages
+## Developer Guide
 See [here](https://sota-nakashima.github.io/MySQLPandas/).
 ## Install
 Install through pip.
 ```
 pip install MySQLPandas
 ```
```

### Comparing `MySQLPandas-0.0.15/setup.py` & `MySQLPandas-0.0.18/setup.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.15/tests/test_DataFrameClass.py` & `MySQLPandas-0.0.18/tests/test_DataFrameClass.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.15/tests/test_coreClass.py` & `MySQLPandas-0.0.18/tests/test_coreClass.py`

 * *Files identical despite different names*

