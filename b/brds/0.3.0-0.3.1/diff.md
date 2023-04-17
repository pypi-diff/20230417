# Comparing `tmp/brds-0.3.0.tar.gz` & `tmp/brds-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.3.0.tar", last modified: Tue Apr 11 18:45:26 2023, max compression
+gzip compressed data, was "brds-0.3.1.tar", last modified: Mon Apr 17 11:45:11 2023, max compression
```

## Comparing `brds-0.3.0.tar` & `brds-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 18:45:13.000000 brds-0.3.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-11 18:45:13.000000 brds-0.3.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 18:45:13.000000 brds-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 18:45:13.000000 brds-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 18:45:26.874451 brds-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-11 18:45:13.000000 brds-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.870451 brds-0.3.0/brds/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 18:45:13.000000 brds-0.3.0/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 18:45:13.000000 brds-0.3.0/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 18:45:13.000000 brds-0.3.0/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-11 18:45:13.000000 brds-0.3.0/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-11 18:45:13.000000 brds-0.3.0/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 18:45:13.000000 brds-0.3.0/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-11 18:45:13.000000 brds-0.3.0/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 18:45:13.000000 brds-0.3.0/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-11 18:45:13.000000 brds-0.3.0/brds/humanize/sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:13.000000 brds-0.3.0/brds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 18:45:13.000000 brds-0.3.0/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 18:45:13.000000 brds-0.3.0/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.870451 brds-0.3.0/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 18:45:26.000000 brds-0.3.0/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:45:26.874451 brds-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 18:45:13.000000 brds-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:26.874451 brds-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 18:45:13.000000 brds-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-11 18:45:13.000000 brds-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 18:45:13.000000 brds-0.3.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.073657 brds-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 11:44:55.000000 brds-0.3.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-17 11:44:55.000000 brds-0.3.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 11:44:55.000000 brds-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 11:44:55.000000 brds-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-17 11:45:11.073657 brds-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 11:44:55.000000 brds-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 11:44:55.000000 brds-0.3.1/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 11:44:55.000000 brds-0.3.1/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-17 11:44:55.000000 brds-0.3.1/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-17 11:44:55.000000 brds-0.3.1/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-17 11:44:55.000000 brds-0.3.1/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-17 11:44:55.000000 brds-0.3.1/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-17 11:44:55.000000 brds-0.3.1/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 11:44:55.000000 brds-0.3.1/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-17 11:44:55.000000 brds-0.3.1/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:44:55.000000 brds-0.3.1/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 11:44:55.000000 brds-0.3.1/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-17 11:44:55.000000 brds-0.3.1/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 11:45:11.000000 brds-0.3.1/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:45:11.073657 brds-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 11:44:55.000000 brds-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:45:11.069657 brds-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:44:55.000000 brds-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 11:44:55.000000 brds-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 11:44:55.000000 brds-0.3.1/tests/test_base.py
```

### Comparing `brds-0.3.0/HISTORY.md` & `brds-0.3.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Removing unsupported flag. [brahle]
+- Fixing the files. [brahle]
+- Removing codecov which is deleted. [brahle]
+- CORS. [brahle]
+
+
+0.3.0 (2023-04-11)
+------------------
+- Release: version 0.3.0 🚀 [brahle]
 - Release: version 0..0 🚀 [brahle]
 - Preventing exploits. [brahle]
 
 
 0.2.8 (2023-04-10)
 ------------------
 - Release: version 0.2.8 🚀 [brahle]
```

### Comparing `brds-0.3.0/LICENSE` & `brds-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/PKG-INFO` & `brds-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # brds
 
-[![codecov](https://codecov.io/gh/brahle/brds/branch/main/graph/badge.svg?token=brds_token_here)](https://codecov.io/gh/brahle/brds)
 [![CI](https://github.com/brahle/brds/actions/workflows/main.yml/badge.svg)](https://github.com/brahle/brds/actions/workflows/main.yml)
 
 Bruno Rahle's Data Science library.
 
 ## Install it from PyPI
 
 ```bash
```

### Comparing `brds-0.3.0/brds/__init__.py` & `brds-0.3.1/brds/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/app.py` & `brds-0.3.1/brds/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,55 @@
 from os.path import isfile
 from typing import Any, Dict
 
 import pandas as pd
 from fastapi import FastAPI, HTTPException, Path, Request, Response
+from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import FileResponse, HTMLResponse
 from fastapi.templating import Jinja2Templates
 
-from brds import fload, get_dataset_files, list_datasets, get_safe_path
+from brds import fload, get_dataset_files, get_safe_path, list_datasets
 
 app = FastAPI()
 
+origins = [
+    "http://localhost:3000",
+    "https://localhost:3000",
+    "http://localhost:8080",
+    "https://localhost:8080",
+]
+
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=origins,
+    allow_credentials=True,
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
+
+
 templates = Jinja2Templates(directory="./brds/templates")
 
 
 @app.get("/dictionary/{filename:path}")
 async def read_as_dict(filename: str = Path(..., regex=r"[\w\-/]+")) -> Dict[str, Any]:
     try:
         df = fload(str(get_safe_path(filename)))
         return df.to_dict(orient="records")
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/raw/{filename:path}")
-async def read_raw(filename: str = Path(..., regex=r"[\w\-/]+")) -> Dict[str, Any]:
+async def read_raw(filename: str = Path(..., regex=r"[\w\-/]+")) -> Any:
     try:
         df = fload(str(get_safe_path(filename)))
-        return df.to_dict(orient="records")
+        if isinstance(df, pd.DataFrame):
+            return df.to_dict(orient="records")
+        return df
     except FileNotFoundError as exc:
         raise HTTPException(status_code=404, detail=f"Parquet file '{filename}' not found") from exc
 
 
 @app.get("/html/{filename:path}", response_class=HTMLResponse)
 async def read_html(filename: str = Path(..., regex=r"[\w\-/]+")) -> str:
     try:
```

### Comparing `brds-0.3.0/brds/cli.py` & `brds-0.3.1/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/__init__.py` & `brds-0.3.1/brds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/datasets/dataset_files.py` & `brds-0.3.1/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/datasets/dataset_info.py` & `brds-0.3.1/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/datasets/list_datasets.py` & `brds-0.3.1/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/edit.py` & `brds-0.3.1/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/environment.py` & `brds-0.3.1/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/fetch/fetcher.py` & `brds-0.3.1/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/fs/reader.py` & `brds-0.3.1/brds/core/fs/reader.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/fs/writer.py` & `brds-0.3.1/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/importer/gunizp_importer.py` & `brds-0.3.1/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/core/logger.py` & `brds-0.3.1/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/humanize/sizes.py` & `brds-0.3.1/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/templates/dataset_files.html` & `brds-0.3.1/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds/templates/datasets.html` & `brds-0.3.1/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/brds.egg-info/PKG-INFO` & `brds-0.3.1/brds.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: brds
-Version: 0.3.0
+Version: 0.3.1
 Summary: Awesome brds created by brahle
 Home-page: https://github.com/brahle/brds/
 Author: brahle
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # brds
 
-[![codecov](https://codecov.io/gh/brahle/brds/branch/main/graph/badge.svg?token=brds_token_here)](https://codecov.io/gh/brahle/brds)
 [![CI](https://github.com/brahle/brds/actions/workflows/main.yml/badge.svg)](https://github.com/brahle/brds/actions/workflows/main.yml)
 
 Bruno Rahle's Data Science library.
 
 ## Install it from PyPI
 
 ```bash
```

### Comparing `brds-0.3.0/brds.egg-info/SOURCES.txt` & `brds-0.3.1/brds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brds-0.3.0/setup.py` & `brds-0.3.1/setup.py`

 * *Files identical despite different names*

