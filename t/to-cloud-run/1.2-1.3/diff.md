# Comparing `tmp/to-cloud-run-1.2.tar.gz` & `tmp/to-cloud-run-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.2.tar", last modified: Sun Apr 16 23:25:27 2023, max compression
+gzip compressed data, was "to-cloud-run-1.3.tar", last modified: Mon Apr 17 00:05:24 2023, max compression
```

## Comparing `to-cloud-run-1.2.tar` & `to-cloud-run-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-16 23:25:27.887461 to-cloud-run-1.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-16 23:25:27.887314 to-cloud-run-1.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-16 23:25:27.000000 to-cloud-run-1.2/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-16 23:25:27.887506 to-cloud-run-1.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-16 23:25:27.000000 to-cloud-run-1.2/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-16 23:25:27.887114 to-cloud-run-1.2/to_cloud_run.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3127 2023-04-16 23:25:27.000000 to-cloud-run-1.2/to_cloud_run.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:05:24.011069 to-cloud-run-1.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:05:24.010954 to-cloud-run-1.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-17 00:05:23.000000 to-cloud-run-1.3/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 00:05:24.011105 to-cloud-run-1.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 00:05:23.000000 to-cloud-run-1.3/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:05:24.010786 to-cloud-run-1.3/to_cloud_run.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3167 2023-04-17 00:05:23.000000 to-cloud-run-1.3/to_cloud_run.py
```

### Comparing `to-cloud-run-1.2/PKG-INFO` & `to-cloud-run-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.2
+Version: 1.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 自動化 from github to google cloud run 部署作業
```

### Comparing `to-cloud-run-1.2/README.md` & `to-cloud-run-1.3/README.md`

 * *Files identical despite different names*

### Comparing `to-cloud-run-1.2/to_cloud_run.egg-info/PKG-INFO` & `to-cloud-run-1.3/to_cloud_run.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.2
+Version: 1.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 自動化 from github to google cloud run 部署作業
```

### Comparing `to-cloud-run-1.2/to_cloud_run.py` & `to-cloud-run-1.3/to_cloud_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 from argparse import ArgumentParser
-from os import getenv, system, path
+from os import getenv, system, path, getcwd
 
 from dotenv import load_dotenv
 
 
 def create_dockerfile():
     if not path.exists('./Dockerfile'):
         dockerfile = """
@@ -42,14 +42,15 @@
            f'--memory={memory} '
            f'--max-instances={max_instances} '
            f'--region={region} '
            f'--project={getenv("GCP_PROJECT_ID")}')
 
 
 def main():
+    print("getcwd()", getcwd())
     load_dotenv()
     if not getenv('GCP_PROJECT_ID'):
         print('Error: GCP_PROJECT_ID is not set in the environment or .env file.')
         return
     if not getenv('GCP_SERVICE_ACCOUNT'):
         print('Error: GCP_SERVICE_ACCOUNT is not set in the environment or .env file.')
         return
```

