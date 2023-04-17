# Comparing `tmp/crispr_library_prep-0.1.1.tar.gz` & `tmp/crispr_library_prep-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_library_prep-0.1.1.tar", max compression
+gzip compressed data, was "crispr_library_prep-0.1.2.tar", max compression
```

## Comparing `crispr_library_prep-0.1.1.tar` & `crispr_library_prep-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       57 2023-04-17 16:42:04.861650 crispr_library_prep-0.1.1/crispr_library_prep/__init__.py
--rw-r--r--   0        0        0    11614 2023-04-17 16:40:48.000474 crispr_library_prep-0.1.1/crispr_library_prep/CrisprLibraryPrep.py
--rw-r--r--   0        0        0      555 2023-04-17 16:49:07.244326 crispr_library_prep-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.1/README.md
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.1/setup.py
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-04-17 16:42:04.861650 crispr_library_prep-0.1.2/crispr_library_prep/__init__.py
+-rw-r--r--   0        0        0    11614 2023-04-17 16:40:48.000474 crispr_library_prep-0.1.2/crispr_library_prep/CrisprLibraryPrep.py
+-rw-r--r--   0        0        0      529 2023-04-17 17:25:39.097372 crispr_library_prep-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:47:11.053642 crispr_library_prep-0.1.2/README.md
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.2/setup.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 crispr_library_prep-0.1.2/PKG-INFO
```

### Comparing `crispr_library_prep-0.1.1/crispr_library_prep/CrisprLibraryPrep.py` & `crispr_library_prep-0.1.2/crispr_library_prep/CrisprLibraryPrep.py`

 * *Files identical despite different names*

### Comparing `crispr_library_prep-0.1.1/pyproject.toml` & `crispr_library_prep-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "crispr-library-prep"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Basheer Becerra <bbecerr@outlook.com>"]
 readme = "README.md"
 packages = [{include = "crispr_library_prep"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-numpy = "^1.24.2"
+numpy = "^1.23"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 biopython = "^1.81"
-pandarallel = "^1.6.4"
 typeguard = "^3.0.2"
 pandas = "^1.5.3"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `crispr_library_prep-0.1.1/setup.py` & `crispr_library_prep-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['biopython>=1.81,<2.0',
  'matplotlib>=3.7.1,<4.0.0',
- 'numpy>=1.24.2,<2.0.0',
- 'pandarallel>=1.6.4,<2.0.0',
+ 'numpy>=1.23,<2.0',
  'pandas>=1.5.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'typeguard>=3.0.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'crispr-library-prep',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'Basheer Becerra',
     'author_email': 'bbecerr@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

