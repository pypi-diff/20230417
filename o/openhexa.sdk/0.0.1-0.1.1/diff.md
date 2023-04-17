# Comparing `tmp/openhexa.sdk-0.0.1.tar.gz` & `tmp/openhexa.sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.sdk-0.0.1.tar", last modified: Mon Apr 17 09:19:51 2023, max compression
+gzip compressed data, was "openhexa.sdk-0.1.1.tar", last modified: Mon Apr 17 10:55:35 2023, max compression
```

## Comparing `openhexa.sdk-0.0.1.tar` & `openhexa.sdk-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.351129 openhexa.sdk-0.0.1/
--rw-r--r--   0 pierre     (501) staff       (20)     1057 2023-04-13 09:50:26.000000 openhexa.sdk-0.0.1/LICENCE
--rw-r--r--   0 pierre     (501) staff       (20)     1130 2023-04-17 09:19:51.351289 openhexa.sdk-0.0.1/PKG-INFO
--rw-r--r--   0 pierre     (501) staff       (20)      651 2023-04-13 17:27:46.000000 openhexa.sdk-0.0.1/README.md
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.346092 openhexa.sdk-0.0.1/openhexa/
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-04-13 10:05:22.000000 openhexa.sdk-0.0.1/openhexa/__init__.py
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.348745 openhexa.sdk-0.0.1/openhexa/sdk/
--rw-r--r--   0 pierre     (501) staff       (20)       22 2023-04-13 09:50:26.000000 openhexa.sdk-0.0.1/openhexa/sdk/__init__.py
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.349929 openhexa.sdk-0.0.1/openhexa/sdk/pipelines/
--rw-r--r--   0 pierre     (501) staff       (20)      101 2023-04-17 09:06:55.000000 openhexa.sdk-0.0.1/openhexa/sdk/pipelines/__init__.py
--rw-r--r--   0 pierre     (501) staff       (20)     9944 2023-04-17 09:06:55.000000 openhexa.sdk-0.0.1/openhexa/sdk/pipelines/parameter.py
--rw-r--r--   0 pierre     (501) staff       (20)     5824 2023-04-17 09:06:55.000000 openhexa.sdk-0.0.1/openhexa/sdk/pipelines/pipeline.py
--rw-r--r--   0 pierre     (501) staff       (20)     3654 2023-04-13 16:55:24.000000 openhexa.sdk-0.0.1/openhexa/sdk/pipelines/task.py
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.348350 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/
--rw-r--r--   0 pierre     (501) staff       (20)     1130 2023-04-17 09:19:51.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/PKG-INFO
--rw-r--r--   0 pierre     (501) staff       (20)      509 2023-04-17 09:19:51.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pierre     (501) staff       (20)        1 2023-04-17 09:19:51.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pierre     (501) staff       (20)       97 2023-04-17 09:19:51.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/requires.txt
--rw-r--r--   0 pierre     (501) staff       (20)       15 2023-04-17 09:19:51.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/top_level.txt
--rw-r--r--   0 pierre     (501) staff       (20)        1 2023-04-13 10:05:49.000000 openhexa.sdk-0.0.1/openhexa.sdk.egg-info/zip-safe
--rw-r--r--   0 pierre     (501) staff       (20)      312 2023-04-13 11:16:49.000000 openhexa.sdk-0.0.1/pyproject.toml
--rw-r--r--   0 pierre     (501) staff       (20)      745 2023-04-17 09:19:51.351972 openhexa.sdk-0.0.1/setup.cfg
--rw-r--r--   0 pierre     (501) staff       (20)       89 2023-04-13 09:50:26.000000 openhexa.sdk-0.0.1/setup.py
-drwxr-xr-x   0 pierre     (501) staff       (20)        0 2023-04-17 09:19:51.350895 openhexa.sdk-0.0.1/tests/
--rw-r--r--   0 pierre     (501) staff       (20)        0 2023-04-13 09:59:12.000000 openhexa.sdk-0.0.1/tests/__init__.py
--rw-r--r--   0 pierre     (501) staff       (20)     7394 2023-04-17 09:06:55.000000 openhexa.sdk-0.0.1/tests/test_parameter.py
--rw-r--r--   0 pierre     (501) staff       (20)     2098 2023-04-17 09:06:55.000000 openhexa.sdk-0.0.1/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.930080 openhexa.sdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 10:55:35.930080 openhexa.sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.926080 openhexa.sdk-0.1.1/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.926080 openhexa.sdk-0.1.1/openhexa/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.930080 openhexa.sdk-0.1.1/openhexa/sdk/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/sdk/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/sdk/pipelines/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/sdk/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/openhexa/sdk/pipelines/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.926080 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 10:55:35.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-17 10:55:35.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:55:35.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 10:55:35.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 10:55:35.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:55:28.000000 openhexa.sdk-0.1.1/openhexa.sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 10:55:35.930080 openhexa.sdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:35.930080 openhexa.sdk-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-17 10:55:22.000000 openhexa.sdk-0.1.1/tests/test_pipeline.py
```

### Comparing `openhexa.sdk-0.0.1/LICENCE` & `openhexa.sdk-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/PKG-INFO` & `openhexa.sdk-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.0.1
+Version: 0.1.1
 Summary: OpenHexa SDK
-Home-page: https://www.bluesquarehub.com
+Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openhexa.sdk-0.0.1/README.md` & `openhexa.sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/openhexa/sdk/pipelines/parameter.py` & `openhexa.sdk-0.1.1/openhexa/sdk/pipelines/parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/openhexa/sdk/pipelines/pipeline.py` & `openhexa.sdk-0.1.1/openhexa/sdk/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/openhexa/sdk/pipelines/task.py` & `openhexa.sdk-0.1.1/openhexa/sdk/pipelines/task.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/openhexa.sdk.egg-info/PKG-INFO` & `openhexa.sdk-0.1.1/openhexa.sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.0.1
+Version: 0.1.1
 Summary: OpenHexa SDK
-Home-page: https://www.bluesquarehub.com
+Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openhexa.sdk-0.0.1/setup.cfg` & `openhexa.sdk-0.1.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = openhexa.sdk
 version = attr: openhexa.sdk.__version__
 author = Bluesquare
 author_email = dev@bluesquarehub.com
-url = https://www.bluesquarehub.com
+url = https://github.com/BLSQ/openhexa-sdk-python
 description = OpenHexa SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = openhexa, pipelines
 license = MIT License
 classifiers = 
 	Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
 	multiprocess
 
 [options.extras_require]
-dev = pytest;pre-commit
+dev = pytest;pytest-cov;pre-commit;build
 examples = geopandas;pandas;rasterio;requests;rasterstats
 
 [options.package_data]
 * = README.md
 
 [egg_info]
 tag_build =
```

### Comparing `openhexa.sdk-0.0.1/tests/test_parameter.py` & `openhexa.sdk-0.1.1/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.0.1/tests/test_pipeline.py` & `openhexa.sdk-0.1.1/tests/test_pipeline.py`

 * *Files identical despite different names*

