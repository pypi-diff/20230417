# Comparing `tmp/dandischema-0.8.2.tar.gz` & `tmp/dandischema-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dandi-schema/dandi-schema/dandischema/dist/.tmp-1ombmbx2/dandischema-0.8.2.tar", last modified: Thu Mar 16 02:07:06 2023, max compression
+gzip compressed data, was "/home/runner/work/dandi-schema/dandi-schema/dandischema/dist/.tmp-5ukzi4l3/dandischema-0.8.3.tar", last modified: Mon Apr 17 17:43:00 2023, max compression
```

## Comparing `dandischema-0.8.2.tar` & `dandischema-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-03-16 02:06:57.000000 dandischema-0.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 02:06:36.000000 dandischema-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-16 02:06:36.000000 dandischema-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-16 02:07:06.000000 dandischema-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-16 02:06:36.000000 dandischema-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/datacite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/digests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/dandietag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/digests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/tests/test_dandietag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/tests/test_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/digests/zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema/tests/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/asset3_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/asset3_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/asset4_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/asset4_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/asset_001.json
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/meta_000004.json
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/meta_000004old.json
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/data/metadata/meta_000008.json
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/test_datacite.py
--rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-16 02:06:36.000000 dandischema-0.8.2/dandischema/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:06:42.000000 dandischema-0.8.2/dandischema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:07:06.000000 dandischema-0.8.2/dandischema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-16 02:06:36.000000 dandischema-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-16 02:07:06.000000 dandischema-0.8.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-03-16 02:06:36.000000 dandischema-0.8.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-16 02:06:36.000000 dandischema-0.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-04-17 17:42:50.000000 dandischema-0.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 17:42:25.000000 dandischema-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 17:42:25.000000 dandischema-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 17:43:00.000000 dandischema-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 17:42:25.000000 dandischema-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/datacite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/digests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/dandietag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/digests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/test_dandietag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/tests/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/digests/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50471 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema/tests/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset3_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset3_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset4_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset4_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/asset_001.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004old.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/data/metadata/meta_000008.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_datacite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-17 17:42:25.000000 dandischema-0.8.3/dandischema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:42:33.000000 dandischema-0.8.3/dandischema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:43:00.000000 dandischema-0.8.3/dandischema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 17:42:25.000000 dandischema-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 17:43:00.000000 dandischema-0.8.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      696 2023-04-17 17:42:25.000000 dandischema-0.8.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 17:42:25.000000 dandischema-0.8.3/tox.ini
```

### Comparing `dandischema-0.8.2/CHANGELOG.md` & `dandischema-0.8.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# 0.8.3 (Mon Apr 17 2023)
+
+#### 🏠 Internal
+
+- [pre-commit.ci] pre-commit autoupdate [#170](https://github.com/dandi/dandi-schema/pull/170) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+
+#### 🔩 Dependency Updates
+
+- Restrict pydantic requirement to < 2.0 [#177](https://github.com/dandi/dandi-schema/pull/177) ([@jwodder](https://github.com/jwodder))
+
+#### Authors: 2
+
+- [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot])
+- John T. Wodder II ([@jwodder](https://github.com/jwodder))
+
+---
+
 # 0.8.2 (Thu Mar 16 2023)
 
 #### 🐛 Bug Fix
 
 - fix: add 0.6.3 to validation [#165](https://github.com/dandi/dandi-schema/pull/165) ([@satra](https://github.com/satra))
 
 #### Authors: 1
```

### Comparing `dandischema-0.8.2/LICENSE` & `dandischema-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/PKG-INFO` & `dandischema-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandischema
-Version: 0.8.2
+Version: 0.8.3
 Summary: Schemata for DANDI archive project
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
```

### Comparing `dandischema-0.8.2/README.md` & `dandischema-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/consts.py` & `dandischema-0.8.3/dandischema/consts.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/datacite.py` & `dandischema-0.8.3/dandischema/datacite.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/digests/dandietag.py` & `dandischema-0.8.3/dandischema/digests/dandietag.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/digests/tests/test_dandietag.py` & `dandischema-0.8.3/dandischema/digests/tests/test_dandietag.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/digests/tests/test_zarr.py` & `dandischema-0.8.3/dandischema/digests/tests/test_zarr.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/digests/zarr.py` & `dandischema-0.8.3/dandischema/digests/zarr.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/exceptions.py` & `dandischema-0.8.3/dandischema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/metadata.py` & `dandischema-0.8.3/dandischema/metadata.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/models.py` & `dandischema-0.8.3/dandischema/models.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/asset3_01.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/asset3_01.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/asset3_02.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/asset3_02.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/asset4_01.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/asset4_01.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/asset4_02.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/asset4_02.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/asset_001.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/asset_001.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/meta_000004.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/meta_000004old.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000004old.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/data/metadata/meta_000008.json` & `dandischema-0.8.3/dandischema/tests/data/metadata/meta_000008.json`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/test_datacite.py` & `dandischema-0.8.3/dandischema/tests/test_datacite.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/test_metadata.py` & `dandischema-0.8.3/dandischema/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/test_models.py` & `dandischema-0.8.3/dandischema/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/tests/test_utils.py` & `dandischema-0.8.3/dandischema/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema/utils.py` & `dandischema-0.8.3/dandischema/utils.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/dandischema.egg-info/PKG-INFO` & `dandischema-0.8.3/dandischema.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dandischema
-Version: 0.8.2
+Version: 0.8.3
 Summary: Schemata for DANDI archive project
 Home-page: http://dandiarchive.org
 Author: DANDI developers
 Author-email: team@dandiarchive.org
 Maintainer: Yaroslav O. Halchenko
 Maintainer-email: debian@onerussian.com
 License: Apache 2.0
```

### Comparing `dandischema-0.8.2/dandischema.egg-info/SOURCES.txt` & `dandischema-0.8.3/dandischema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/pyproject.toml` & `dandischema-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/setup.cfg` & `dandischema-0.8.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 project_urls = 
 	Source Code = https://github.com/dandi/dandischema
 
 [options]
 python_requires = >=3.7
 install_requires = 
 	jsonschema[format]
-	pydantic[email] >= 1.8.1
+	pydantic[email] >= 1.8.1, < 2.0
 	typing_extensions;  python_version < "3.8"
 	requests
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 
 [options.packages.find]
```

### Comparing `dandischema-0.8.2/setup.py` & `dandischema-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `dandischema-0.8.2/tox.ini` & `dandischema-0.8.3/tox.ini`

 * *Files identical despite different names*

