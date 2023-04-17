# Comparing `tmp/to-cloud-run-1.5.tar.gz` & `tmp/to-cloud-run-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.5.tar", last modified: Mon Apr 17 04:02:19 2023, max compression
+gzip compressed data, was "to-cloud-run-1.6.tar", last modified: Mon Apr 17 04:11:07 2023, max compression
```

## Comparing `to-cloud-run-1.5.tar` & `to-cloud-run-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:02:19.730145 to-cloud-run-1.5/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:02:19.730010 to-cloud-run-1.5/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     3057 2023-04-17 04:02:19.000000 to-cloud-run-1.5/README.md
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 04:02:19.730186 to-cloud-run-1.5/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 04:02:19.000000 to-cloud-run-1.5/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:02:19.729813 to-cloud-run-1.5/to_cloud_run.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3346 2023-04-17 04:02:19.000000 to-cloud-run-1.5/to_cloud_run.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:11:07.965674 to-cloud-run-1.6/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:11:07.965523 to-cloud-run-1.6/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3057 2023-04-17 04:11:07.000000 to-cloud-run-1.6/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-04-17 04:11:07.965711 to-cloud-run-1.6/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      510 2023-04-17 04:11:07.000000 to-cloud-run-1.6/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-04-17 04:11:07.965356 to-cloud-run-1.6/to_cloud_run.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3225 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      252 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       52 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       14 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       13 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3354 2023-04-17 04:11:07.000000 to-cloud-run-1.6/to_cloud_run.py
```

### Comparing `to-cloud-run-1.5/PKG-INFO` & `to-cloud-run-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.5
+Version: 1.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 將服務部署到 GCP Cloud Run
```

### Comparing `to-cloud-run-1.5/README.md` & `to-cloud-run-1.6/README.md`

 * *Files identical despite different names*

### Comparing `to-cloud-run-1.5/to_cloud_run.egg-info/PKG-INFO` & `to-cloud-run-1.6/to_cloud_run.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.5
+Version: 1.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 將服務部署到 GCP Cloud Run
```

### Comparing `to-cloud-run-1.5/to_cloud_run.py` & `to-cloud-run-1.6/to_cloud_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     print('''Suggest create requirements.txt at folder root:
 uvicorn
 fastapi
 starlette
 pydantic
 jinja2
 
-Please put all your fastapi files into ./app folder.
+Please put your main fastapi files into folder root ./app.py
     ''')
 
 
 def main():
     usage()
     load_dotenv(getcwd() + "/.env")
     if not getenv('GCP_PROJECT_ID'):
```

