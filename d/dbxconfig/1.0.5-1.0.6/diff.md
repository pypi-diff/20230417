# Comparing `tmp/dbxconfig-1.0.5.tar.gz` & `tmp/dbxconfig-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.5.tar", last modified: Mon Apr 17 15:55:59 2023, max compression
+gzip compressed data, was "dbxconfig-1.0.6.tar", last modified: Mon Apr 17 21:42:41 2023, max compression
```

## Comparing `dbxconfig-1.0.5.tar` & `dbxconfig-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 15:55:59.383612 dbxconfig-1.0.5/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 15:55:59.383474 dbxconfig-1.0.5/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.5/README.md
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 15:55:59.382499 dbxconfig-1.0.5/dbxconfig/
--rw-r--r--   0 shaunryan   (501) staff       (20)      428 2023-04-17 12:50:14.000000 dbxconfig-1.0.5/dbxconfig/__init__.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     3482 2023-04-17 12:57:34.000000 dbxconfig-1.0.5/dbxconfig/_config.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     2935 2023-04-17 15:55:15.000000 dbxconfig-1.0.5/dbxconfig/_deltalake.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4892 2023-04-17 15:50:34.000000 dbxconfig-1.0.5/dbxconfig/_source.py
--rw-r--r--   0 shaunryan   (501) staff       (20)      110 2023-04-17 12:57:48.000000 dbxconfig-1.0.5/dbxconfig/_stage_type.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     4187 2023-04-17 12:57:48.000000 dbxconfig-1.0.5/dbxconfig/_table_index.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.5/dbxconfig/_timeslice.py
--rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.5/dbxconfig/_utils.py
-drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 15:55:59.383283 dbxconfig-1.0.5/dbxconfig.egg-info/
--rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 15:55:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 shaunryan   (501) staff       (20)      397 2023-04-17 15:55:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-17 15:55:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-17 15:55:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-17 15:55:59.000000 dbxconfig-1.0.5/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-17 15:55:59.383661 dbxconfig-1.0.5/setup.cfg
--rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-17 15:51:51.000000 dbxconfig-1.0.5/setup.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.122561 dbxconfig-1.0.6/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 21:42:41.122432 dbxconfig-1.0.6/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2936 2023-04-16 22:21:21.000000 dbxconfig-1.0.6/README.md
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.121301 dbxconfig-1.0.6/dbxconfig/
+-rw-r--r--   0 shaunryan   (501) staff       (20)      428 2023-04-17 12:50:14.000000 dbxconfig-1.0.6/dbxconfig/__init__.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3853 2023-04-17 21:24:13.000000 dbxconfig-1.0.6/dbxconfig/_config.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     2935 2023-04-17 15:55:15.000000 dbxconfig-1.0.6/dbxconfig/_deltalake.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4892 2023-04-17 15:50:34.000000 dbxconfig-1.0.6/dbxconfig/_source.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)      110 2023-04-17 12:57:48.000000 dbxconfig-1.0.6/dbxconfig/_stage_type.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     4187 2023-04-17 12:57:48.000000 dbxconfig-1.0.6/dbxconfig/_table_index.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     5706 2023-04-16 20:49:59.000000 dbxconfig-1.0.6/dbxconfig/_timeslice.py
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1836 2023-04-17 14:42:51.000000 dbxconfig-1.0.6/dbxconfig/_utils.py
+drwxr-xr-x   0 shaunryan   (501) staff       (20)        0 2023-04-17 21:42:41.122239 dbxconfig-1.0.6/dbxconfig.egg-info/
+-rw-r--r--   0 shaunryan   (501) staff       (20)     3508 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 shaunryan   (501) staff       (20)      397 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)        1 2023-04-16 20:49:59.000000 dbxconfig-1.0.6/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 shaunryan   (501) staff       (20)       31 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       10 2023-04-17 21:42:41.000000 dbxconfig-1.0.6/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 shaunryan   (501) staff       (20)       38 2023-04-17 21:42:41.122623 dbxconfig-1.0.6/setup.cfg
+-rw-r--r--   0 shaunryan   (501) staff       (20)     1069 2023-04-17 21:42:30.000000 dbxconfig-1.0.6/setup.py
```

### Comparing `dbxconfig-1.0.5/PKG-INFO` & `dbxconfig-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.5
+Version: 1.0.6
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.5/README.md` & `dbxconfig-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig/_config.py` & `dbxconfig-1.0.6/dbxconfig/_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,14 +84,20 @@
 
     def link_checkpoint(
         self,
         source: Union[Source, DeltaLake],
         destination: DeltaLake,
         checkpoint_name: str = None,
     ):
+        if not isinstance(source, Source) and not isinstance(source, DeltaLake):
+            raise ValueError(f"source must be a Source or Deltalake Object, invalid type {type(source)} was found.")
+        
+        if not isinstance(destination, DeltaLake):
+            raise ValueError(f"destination must be a Deltalake Object, invalid type {type(source)} was found.")
+
         if not checkpoint_name:
             checkpoint_name = f"{source.database}.{source.table}-{destination.database}.{destination.table}"
 
         source.checkpoint = checkpoint_name
         source._render()
         destination.checkpoint = checkpoint_name
         destination._render()
```

### Comparing `dbxconfig-1.0.5/dbxconfig/_deltalake.py` & `dbxconfig-1.0.6/dbxconfig/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig/_source.py` & `dbxconfig-1.0.6/dbxconfig/_source.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig/_table_index.py` & `dbxconfig-1.0.6/dbxconfig/_table_index.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig/_timeslice.py` & `dbxconfig-1.0.6/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig/_utils.py` & `dbxconfig-1.0.6/dbxconfig/_utils.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.5/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-1.0.6/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.5
+Version: 1.0.6
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.5/setup.py` & `dbxconfig-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.5",
+    version="1.0.6",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```

