# Comparing `tmp/to-cloud-run-1.3.tar.gz` & `tmp/to-cloud-run-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.3.tar", last modified: Mon Apr 17 00:05:24 2023, max compression
+gzip compressed data, was "to-cloud-run-1.4.tar", last modified: Mon Apr 17 00:08:36 2023, max compression
```

## Comparing `to-cloud-run-1.3.tar` & `to-cloud-run-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:05:24.011069 to-cloud-run-1.3/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:05:24.010954 to-cloud-run-1.3/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-17 00:05:23.000000 to-cloud-run-1.3/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 00:05:24.011105 to-cloud-run-1.3/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 00:05:23.000000 to-cloud-run-1.3/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:05:24.010786 to-cloud-run-1.3/to_cloud_run.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3167 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:08:36.333631 to-cloud-run-1.4/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:08:36.333522 to-cloud-run-1.4/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-17 00:08:36.000000 to-cloud-run-1.4/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 00:08:36.333664 to-cloud-run-1.4/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 00:08:36.000000 to-cloud-run-1.4/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:08:36.333370 to-cloud-run-1.4/to_cloud_run.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3151 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.py
```

### Comparing `to-cloud-run-1.3/PKG-INFO` & `to-cloud-run-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.3
+Version: 1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 自動化 from github to google cloud run 部署作業
```

### Comparing `to-cloud-run-1.3/README.md` & `to-cloud-run-1.4/README.md`

 * *Files identical despite different names*

### Comparing `to-cloud-run-1.3/to_cloud_run.egg-info/PKG-INFO` & `to-cloud-run-1.4/to_cloud_run.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.3
+Version: 1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 自動化 from github to google cloud run 部署作業
```

### Comparing `to-cloud-run-1.3/to_cloud_run.py` & `to-cloud-run-1.4/to_cloud_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,15 @@
            f'--memory={memory} '
            f'--max-instances={max_instances} '
            f'--region={region} '
            f'--project={getenv("GCP_PROJECT_ID")}')
 
 
 def main():
-    print("getcwd()", getcwd())
-    load_dotenv()
+    load_dotenv(getcwd()+"/.env")
     if not getenv('GCP_PROJECT_ID'):
         print('Error: GCP_PROJECT_ID is not set in the environment or .env file.')
         return
     if not getenv('GCP_SERVICE_ACCOUNT'):
         print('Error: GCP_SERVICE_ACCOUNT is not set in the environment or .env file.')
         return
```

