# Comparing `tmp/lib_repo_tool-2.0.3.tar.gz` & `tmp/lib_repo_tool-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_repo_tool-2.0.3.tar", last modified: Mon Apr 17 02:14:39 2023, max compression
+gzip compressed data, was "lib_repo_tool-2.0.4.tar", last modified: Mon Apr 17 09:00:17 2023, max compression
```

## Comparing `lib_repo_tool-2.0.3.tar` & `lib_repo_tool-2.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.751685 lib_repo_tool-2.0.3/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 02:14:39.751384 lib_repo_tool-2.0.3/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.3/README.md
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.749371 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      327 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/SOURCES.txt
--rw-r--r--   0 Andy       (501) staff       (20)        1 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/dependency_links.txt
--rw-r--r--   0 Andy       (501) staff       (20)       76 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/entry_points.txt
--rw-r--r--   0 Andy       (501) staff       (20)       36 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/requires.txt
--rw-r--r--   0 Andy       (501) staff       (20)       10 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/top_level.txt
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.750891 lib_repo_tool-2.0.3/repo_tool/
--rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.3/repo_tool/__init__.py
--rw-r--r--   0 Andy       (501) staff       (20)     5287 2023-04-17 02:09:40.000000 lib_repo_tool-2.0.3/repo_tool/common.py
--rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.3/repo_tool/lib_get.py
--rw-r--r--   0 Andy       (501) staff       (20)    17096 2023-03-31 04:59:55.000000 lib_repo_tool-2.0.3/repo_tool/lib_repo.py
--rw-r--r--   0 Andy       (501) staff       (20)       38 2023-04-17 02:14:39.751793 lib_repo_tool-2.0.3/setup.cfg
--rw-r--r--   0 Andy       (501) staff       (20)      473 2023-04-17 02:10:20.000000 lib_repo_tool-2.0.3/setup.py
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 09:00:17.151764 lib_repo_tool-2.0.4/
+-rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 09:00:17.151486 lib_repo_tool-2.0.4/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.4/README.md
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 09:00:17.149248 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/
+-rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      327 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 Andy       (501) staff       (20)        1 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       76 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/entry_points.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       36 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/requires.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       10 2023-04-17 09:00:17.000000 lib_repo_tool-2.0.4/lib_repo_tool.egg-info/top_level.txt
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 09:00:17.151038 lib_repo_tool-2.0.4/repo_tool/
+-rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.4/repo_tool/__init__.py
+-rw-r--r--   0 Andy       (501) staff       (20)     5425 2023-04-17 08:58:23.000000 lib_repo_tool-2.0.4/repo_tool/common.py
+-rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.4/repo_tool/lib_get.py
+-rw-r--r--   0 Andy       (501) staff       (20)    17096 2023-03-31 04:59:55.000000 lib_repo_tool-2.0.4/repo_tool/lib_repo.py
+-rw-r--r--   0 Andy       (501) staff       (20)       38 2023-04-17 09:00:17.151855 lib_repo_tool-2.0.4/setup.cfg
+-rw-r--r--   0 Andy       (501) staff       (20)      473 2023-04-17 08:59:40.000000 lib_repo_tool-2.0.4/setup.py
```

### Comparing `lib_repo_tool-2.0.3/README.md` & `lib_repo_tool-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.3/repo_tool/common.py` & `lib_repo_tool-2.0.4/repo_tool/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 import zipfile
 import sys
 import requests
 import re
 import time
 import hashlib
 import datetime
+import logging
 
 from urllib import parse
 from dataclasses import dataclass
 
+logger = logging.getLogger(__name__)
+logger.addHandler(logging.StreamHandler())
+logger.setLevel(logging.INFO)
+
 # OSS_BASE_PATH = 'arcsite-x-libs-repo'
 OSS_BASE_PATH = 'arcsite-x-libs-repo-2.0'
 
 def md5sum(src):
     m = hashlib.md5()
     m.update(src)
     return m.hexdigest()
@@ -113,17 +118,17 @@
     if cdn_key:
         raw_url = parse.urljoin('http://oss.lib-repo.dev.arcsiteapp.cn', file_key)
         exp = int(time.time()) + 1 * 3600
         download_url = a_auth(raw_url, cdn_key, exp)
     else:
         download_url: str = get_bucket().sign_url('GET', file_key, 60 * 30)
     
-    print(f"Download URL: {download_url}")
+    logger.info(f"Download URL: {download_url}")
     res = requests.get(download_url, stream=True, timeout=10)
-    print(f"download file result: {res.reason} ")
+    logger.info(f"download file result: {res.reason} ")
     with open(to_path, 'wb') as f:
         for chunk in res.iter_content(chunk_size=1024*1024*10):
             if (chunk):
                 f.write(chunk)
 
 def get_file_obj_2_str(file_key, not_exist_exception=False):
     try:
```

### Comparing `lib_repo_tool-2.0.3/repo_tool/lib_get.py` & `lib_repo_tool-2.0.4/repo_tool/lib_get.py`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.3/repo_tool/lib_repo.py` & `lib_repo_tool-2.0.4/repo_tool/lib_repo.py`

 * *Files identical despite different names*

