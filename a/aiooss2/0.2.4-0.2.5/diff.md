# Comparing `tmp/aiooss2-0.2.4.tar.gz` & `tmp/aiooss2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooss2-0.2.4.tar", last modified: Sun Apr 16 09:51:58 2023, max compression
+gzip compressed data, was "aiooss2-0.2.5.tar", last modified: Mon Apr 17 11:55:08 2023, max compression
```

## Comparing `aiooss2-0.2.4.tar` & `aiooss2-0.2.5.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.547588 aiooss2-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.539588 aiooss2-0.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-16 09:51:35.000000 aiooss2-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-16 09:51:35.000000 aiooss2-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-16 09:51:35.000000 aiooss2-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 09:51:35.000000 aiooss2-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-16 09:51:58.547588 aiooss2-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-16 09:51:35.000000 aiooss2-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-16 09:51:35.000000 aiooss2-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 09:51:35.000000 aiooss2-0.2.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-16 09:51:35.000000 aiooss2-0.2.4/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-16 09:51:35.000000 aiooss2-0.2.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-16 09:51:35.000000 aiooss2-0.2.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 09:51:35.000000 aiooss2-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-16 09:51:58.547588 aiooss2-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.539588 aiooss2-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/src/aiooss2/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-16 09:51:35.000000 aiooss2-0.2.4/src/aiooss2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/src/aiooss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 09:51:58.000000 aiooss2-0.2.4/src/aiooss2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.543588 aiooss2-0.2.4/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/func/test_resumable.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/test_aiooss2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:58.547588 aiooss2-0.2.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-16 09:51:35.000000 aiooss2-0.2.4/tests/unit/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-17 11:54:45.000000 aiooss2-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-17 11:54:45.000000 aiooss2-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-17 11:54:45.000000 aiooss2-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 11:54:45.000000 aiooss2-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 11:55:08.979832 aiooss2-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-17 11:54:45.000000 aiooss2-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 11:54:45.000000 aiooss2-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 11:54:45.000000 aiooss2-0.2.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-17 11:54:45.000000 aiooss2-0.2.5/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 11:54:45.000000 aiooss2-0.2.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-17 11:54:45.000000 aiooss2-0.2.5/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 11:54:45.000000 aiooss2-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-17 11:55:08.983832 aiooss2-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.975832 aiooss2-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/src/aiooss2/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29416 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-17 11:54:45.000000 aiooss2-0.2.5/src/aiooss2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/src/aiooss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 11:55:08.000000 aiooss2-0.2.5/src/aiooss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/func/test_resumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/test_aiooss2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:55:08.979832 aiooss2-0.2.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-17 11:54:45.000000 aiooss2-0.2.5/tests/unit/test_adapter.py
```

### Comparing `aiooss2-0.2.4/.cruft.json` & `aiooss2-0.2.5/.cruft.json`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.github/dependabot.yml` & `aiooss2-0.2.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.github/workflows/docs.yml` & `aiooss2-0.2.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.github/workflows/release.yml` & `aiooss2-0.2.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.github/workflows/tests.yml` & `aiooss2-0.2.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.gitignore` & `aiooss2-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/.pre-commit-config.yaml` & `aiooss2-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/CODE_OF_CONDUCT.rst` & `aiooss2-0.2.5/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/CONTRIBUTING.rst` & `aiooss2-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/LICENSE` & `aiooss2-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/PKG-INFO` & `aiooss2-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiooss2-0.2.4/README.md` & `aiooss2-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/README.rst` & `aiooss2-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/docs/assets/logo.svg` & `aiooss2-0.2.5/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/docs/gen_ref_pages.py` & `aiooss2-0.2.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/examples/simple.py` & `aiooss2-0.2.5/examples/simple.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/mkdocs.yml` & `aiooss2-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/noxfile.py` & `aiooss2-0.2.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/pyproject.toml` & `aiooss2-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/setup.cfg` & `aiooss2-0.2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 where = src
 
+[options.package_data]
+aiooss2 = py.typed
+
 [flake8]
 ignore = 
 	E203
 	E266
 	W503
 	P1
 max_line_length = 88
```

### Comparing `aiooss2-0.2.4/src/aiooss2/adapter.py` & `aiooss2-0.2.5/src/aiooss2/adapter.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/api.py` & `aiooss2-0.2.5/src/aiooss2/api.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/exceptions.py` & `aiooss2-0.2.5/src/aiooss2/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/http.py` & `aiooss2-0.2.5/src/aiooss2/http.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/iterators.py` & `aiooss2-0.2.5/src/aiooss2/iterators.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/models.py` & `aiooss2-0.2.5/src/aiooss2/models.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/multipart.py` & `aiooss2-0.2.5/src/aiooss2/multipart.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/resumable.py` & `aiooss2-0.2.5/src/aiooss2/resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2/utils.py` & `aiooss2-0.2.5/src/aiooss2/utils.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/src/aiooss2.egg-info/PKG-INFO` & `aiooss2-0.2.5/src/aiooss2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aiooss2-0.2.4/src/aiooss2.egg-info/SOURCES.txt` & `aiooss2-0.2.5/src/aiooss2.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/aiooss2/adapter.py
 src/aiooss2/api.py
 src/aiooss2/exceptions.py
 src/aiooss2/http.py
 src/aiooss2/iterators.py
 src/aiooss2/models.py
 src/aiooss2/multipart.py
+src/aiooss2/py.typed
 src/aiooss2/resumable.py
 src/aiooss2/utils.py
 src/aiooss2.egg-info/PKG-INFO
 src/aiooss2.egg-info/SOURCES.txt
 src/aiooss2.egg-info/dependency_links.txt
 src/aiooss2.egg-info/not-zip-safe
 src/aiooss2.egg-info/requires.txt
```

### Comparing `aiooss2-0.2.4/src/aiooss2.egg-info/requires.txt` & `aiooss2-0.2.5/src/aiooss2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/tests/conftest.py` & `aiooss2-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/tests/func/test_bucket.py` & `aiooss2-0.2.5/tests/func/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/tests/func/test_object.py` & `aiooss2-0.2.5/tests/func/test_object.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/tests/func/test_resumable.py` & `aiooss2-0.2.5/tests/func/test_resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.4/tests/unit/test_adapter.py` & `aiooss2-0.2.5/tests/unit/test_adapter.py`

 * *Files identical despite different names*

