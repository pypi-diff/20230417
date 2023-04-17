# Comparing `tmp/NikeCA-0.1.56.tar.gz` & `tmp/NikeCA-0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.56.tar", last modified: Mon Apr 17 08:02:46 2023, max compression
+gzip compressed data, was "NikeCA-0.1.57.tar", last modified: Mon Apr 17 08:06:10 2023, max compression
```

## Comparing `NikeCA-0.1.56.tar` & `NikeCA-0.1.57.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.406652 NikeCA-0.1.56/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.56/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:02:46.406247 NikeCA-0.1.56/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.56/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 08:02:46.406784 NikeCA-0.1.56/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 08:02:14.000000 NikeCA-0.1.56/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.403210 NikeCA-0.1.56/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:02:46.405609 NikeCA-0.1.56/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 08:02:46.000000 NikeCA-0.1.56/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    20795 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3816 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.56/src/_IMPSummaryDashboard.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     2244 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:01:58.000000 NikeCA-0.1.56/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:06:10.341708 NikeCA-0.1.57/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.57/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:06:10.341302 NikeCA-0.1.57/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.57/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 08:06:10.341820 NikeCA-0.1.57/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 08:05:54.000000 NikeCA-0.1.57/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:06:10.338489 NikeCA-0.1.57/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:06:10.340719 NikeCA-0.1.57/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 08:06:10.000000 NikeCA-0.1.57/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      472 2023-04-17 08:06:10.000000 NikeCA-0.1.57/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 08:06:10.000000 NikeCA-0.1.57/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 08:06:10.000000 NikeCA-0.1.57/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 08:06:10.000000 NikeCA-0.1.57/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    20795 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3703 2023-04-10 21:17:23.000000 NikeCA-0.1.57/src/_IMPSummaryDashboard.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2244 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 08:05:41.000000 NikeCA-0.1.57/src/__init__.py
```

### Comparing `NikeCA-0.1.56/LICENSE` & `NikeCA-0.1.57/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/PKG-INFO` & `NikeCA-0.1.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.56
+Version: 0.1.57
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.56/README.md` & `NikeCA-0.1.57/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/setup.py` & `NikeCA-0.1.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.56',
+	version='0.1.57',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_Dashboards",
```

### Comparing `NikeCA-0.1.56/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.57/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.56
+Version: 0.1.57
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.56/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.57/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/NikeQA.py` & `NikeCA-0.1.57/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/NikeSF.py` & `NikeCA-0.1.57/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_BuildSearchQuery.py` & `NikeCA-0.1.57/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_Dashboards.py` & `NikeCA-0.1.57/src/_Dashboards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
-from _InclusionExclusion import InclusionExclusion
 
-
-class Dashboards(InclusionExclusion):
+class Dashboards:
 
     def imp_summary_dashboard(self
                               , username: str
                               , warehouse: str
                               , database: str
                               , role: str
                               , date_min: str = '1900-01-01'
```

### Comparing `NikeCA-0.1.56/src/_GitHub.py` & `NikeCA-0.1.57/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_IMPSummaryDashboard.py` & `NikeCA-0.1.57/src/_IMPSummaryDashboard.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_InclusionExclusion.py` & `NikeCA-0.1.57/src/_InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_QA.py` & `NikeCA-0.1.57/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_SearchFiles.py` & `NikeCA-0.1.57/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_SnowflakeData.py` & `NikeCA-0.1.57/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_SnowflakeDependencies.py` & `NikeCA-0.1.57/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.56/src/_SnowflakePull.py` & `NikeCA-0.1.57/src/_SnowflakePull.py`

 * *Files identical despite different names*

