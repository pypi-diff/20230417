# Comparing `tmp/to-cloud-run-1.4.tar.gz` & `tmp/to-cloud-run-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.4.tar", last modified: Mon Apr 17 00:08:36 2023, max compression
+gzip compressed data, was "to-cloud-run-1.5.tar", last modified: Mon Apr 17 04:02:19 2023, max compression
```

## Comparing `to-cloud-run-1.4.tar` & `to-cloud-run-1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:08:36.333631 to-cloud-run-1.4/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:08:36.333522 to-cloud-run-1.4/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     1820 2023-04-17 00:08:36.000000 to-cloud-run-1.4/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 00:08:36.333664 to-cloud-run-1.4/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 00:08:36.000000 to-cloud-run-1.4/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 00:08:36.333370 to-cloud-run-1.4/to_cloud_run.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1988 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3151 2023-04-17 00:08:36.000000 to-cloud-run-1.4/to_cloud_run.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:02:19.730145 to-cloud-run-1.5/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:02:19.730010 to-cloud-run-1.5/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3057 2023-04-17 04:02:19.000000 to-cloud-run-1.5/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 04:02:19.730186 to-cloud-run-1.5/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 04:02:19.000000 to-cloud-run-1.5/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:02:19.729813 to-cloud-run-1.5/to_cloud_run.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3346 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.py
```

### Comparing `to-cloud-run-1.4/to_cloud_run.py` & `to-cloud-run-1.5/to_cloud_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,29 @@
            f'--cpu={cpu} '
            f'--memory={memory} '
            f'--max-instances={max_instances} '
            f'--region={region} '
            f'--project={getenv("GCP_PROJECT_ID")}')
 
 
+def usage():
+    print('''Suggest create requirements.txt at folder root:
+uvicorn
+fastapi
+starlette
+pydantic
+jinja2
+
+Please put all your fastapi files into ./app folder.
+    ''')
+
+
 def main():
-    load_dotenv(getcwd()+"/.env")
+    usage()
+    load_dotenv(getcwd() + "/.env")
     if not getenv('GCP_PROJECT_ID'):
         print('Error: GCP_PROJECT_ID is not set in the environment or .env file.')
         return
     if not getenv('GCP_SERVICE_ACCOUNT'):
         print('Error: GCP_SERVICE_ACCOUNT is not set in the environment or .env file.')
         return
```

