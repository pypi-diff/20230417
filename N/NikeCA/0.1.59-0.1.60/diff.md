# Comparing `tmp/NikeCA-0.1.59.tar.gz` & `tmp/NikeCA-0.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.59.tar", last modified: Mon Apr 17 20:01:33 2023, max compression
+gzip compressed data, was "NikeCA-0.1.60.tar", last modified: Mon Apr 17 21:05:43 2023, max compression
```

## Comparing `NikeCA-0.1.59.tar` & `NikeCA-0.1.60.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 20:01:33.354782 NikeCA-0.1.59/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.59/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 20:01:33.354504 NikeCA-0.1.59/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.59/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 20:01:33.354860 NikeCA-0.1.59/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 20:01:08.000000 NikeCA-0.1.59/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 20:01:33.351866 NikeCA-0.1.59/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 20:01:33.354026 NikeCA-0.1.59/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 20:01:33.000000 NikeCA-0.1.59/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 20:01:33.000000 NikeCA-0.1.59/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 20:01:33.000000 NikeCA-0.1.59/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 20:01:33.000000 NikeCA-0.1.59/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 20:01:33.000000 NikeCA-0.1.59/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    21686 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.59/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4049 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 20:00:38.000000 NikeCA-0.1.59/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.621739 NikeCA-0.1.60/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.60/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 21:05:43.621428 NikeCA-0.1.60/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.60/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 21:05:43.621819 NikeCA-0.1.60/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 21:05:16.000000 NikeCA-0.1.60/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.619090 NikeCA-0.1.60/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.620819 NikeCA-0.1.60/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      444 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    21686 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4071 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/__init__.py
```

### Comparing `NikeCA-0.1.59/LICENSE` & `NikeCA-0.1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/PKG-INFO` & `NikeCA-0.1.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.59
+Version: 0.1.60
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.59/README.md` & `NikeCA-0.1.60/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/setup.py` & `NikeCA-0.1.60/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.59',
+	version='0.1.60',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_Dashboards",
```

### Comparing `NikeCA-0.1.59/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.60/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.59
+Version: 0.1.60
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.59/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.60/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/NikeQA.py` & `NikeCA-0.1.60/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/NikeSF.py` & `NikeCA-0.1.60/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_BuildSearchQuery.py` & `NikeCA-0.1.60/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_Dashboards.py` & `NikeCA-0.1.60/src/_Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_GitHub.py` & `NikeCA-0.1.60/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_InclusionExclusion.py` & `NikeCA-0.1.60/src/_InclusionExclusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                 
             ORDER BY
                 {order_by}
                 
             ;
         """
 
+        print(query)
+
         return Snowflake(username=username, warehouse=warehouse, database=database,
                          role=role).snowflake_pull(query=query, polars=polars)
 
     def summary(self
                 , username: str
                 , warehouse: str
                 , database: str
```

### Comparing `NikeCA-0.1.59/src/_QA.py` & `NikeCA-0.1.60/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_SearchFiles.py` & `NikeCA-0.1.60/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_SnowflakeData.py` & `NikeCA-0.1.60/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_SnowflakeDependencies.py` & `NikeCA-0.1.60/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.59/src/_SnowflakePull.py` & `NikeCA-0.1.60/src/_SnowflakePull.py`

 * *Files identical despite different names*

