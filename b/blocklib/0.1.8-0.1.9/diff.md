# Comparing `tmp/blocklib-0.1.8.tar.gz` & `tmp/blocklib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blocklib-0.1.8.tar", max compression
+gzip compressed data, was "blocklib-0.1.9.tar", max compression
```

## Comparing `blocklib-0.1.8.tar` & `blocklib-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1537 2022-04-04 11:10:25.908087 blocklib-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0    10174 2022-04-04 11:10:25.908087 blocklib-0.1.8/LICENSE
--rw-r--r--   0        0        0     2391 2022-04-04 11:10:25.908087 blocklib-0.1.8/README.md
--rw-r--r--   0        0        0      558 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/__init__.py
--rw-r--r--   0        0        0     6050 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/blocks_generator.py
--rw-r--r--   0        0        0     4522 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/candidate_blocks_generator.py
--rw-r--r--   0        0        0      390 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/configuration.py
--rw-r--r--   0        0        0     1982 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/encoding.py
--rw-r--r--   0        0        0     1807 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/evaluation.py
--rw-r--r--   0        0        0     3392 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/pprlindex.py
--rw-r--r--   0        0        0     3639 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/pprllambdafold.py
--rw-r--r--   0        0        0     5526 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/pprlpsig.py
--rw-r--r--   0        0        0      869 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/schemas/signature-config-schema.json
--rw-r--r--   0        0        0     4859 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/signature_generator.py
--rw-r--r--   0        0        0     5351 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/simmeasure.py
--rw-r--r--   0        0        0     1431 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/stats.py
--rw-r--r--   0        0        0      716 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/utils.py
--rw-r--r--   0        0        0     2254 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/validation/__init__.py
--rw-r--r--   0        0        0      368 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/validation/constrained_types.py
--rw-r--r--   0        0        0      630 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/validation/lambda_fold_validation.py
--rw-r--r--   0        0        0     2024 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/validation/psig_validation.py
--rw-r--r--   0        0        0      370 2022-04-04 11:10:25.908087 blocklib-0.1.8/blocklib/validation/shared_blocking_config.py
--rw-r--r--   0        0        0     1414 2022-04-04 11:10:25.916087 blocklib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3553 2022-04-04 11:10:56.175935 blocklib-0.1.8/setup.py
--rw-r--r--   0        0        0     3768 2022-04-04 11:10:56.176412 blocklib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1587 2023-03-01 12:05:40.825295 blocklib-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0    10174 2023-03-01 12:05:40.825295 blocklib-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2391 2023-03-01 12:05:40.825295 blocklib-0.1.9/README.md
+-rw-r--r--   0        0        0      601 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/__init__.py
+-rw-r--r--   0        0        0     6050 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/blocks_generator.py
+-rw-r--r--   0        0        0     4522 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/candidate_blocks_generator.py
+-rw-r--r--   0        0        0      390 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/configuration.py
+-rw-r--r--   0        0        0     1982 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/encoding.py
+-rw-r--r--   0        0        0     1807 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/evaluation.py
+-rw-r--r--   0        0        0     3392 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/pprlindex.py
+-rw-r--r--   0        0        0     3639 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/pprllambdafold.py
+-rw-r--r--   0        0        0     5526 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/pprlpsig.py
+-rw-r--r--   0        0        0      869 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/schemas/signature-config-schema.json
+-rw-r--r--   0        0        0     4859 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/signature_generator.py
+-rw-r--r--   0        0        0     5351 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/simmeasure.py
+-rw-r--r--   0        0        0     1431 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/stats.py
+-rw-r--r--   0        0        0      716 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/utils.py
+-rw-r--r--   0        0        0     2254 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/validation/__init__.py
+-rw-r--r--   0        0        0      368 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/validation/constrained_types.py
+-rw-r--r--   0        0        0      630 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/validation/lambda_fold_validation.py
+-rw-r--r--   0        0        0     2024 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/validation/psig_validation.py
+-rw-r--r--   0        0        0      370 2023-03-01 12:05:40.825295 blocklib-0.1.9/blocklib/validation/shared_blocking_config.py
+-rw-r--r--   0        0        0     1468 2023-03-01 12:05:40.833295 blocklib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 blocklib-0.1.9/PKG-INFO
```

### Comparing `blocklib-0.1.8/CHANGELOG.md` & `blocklib-0.1.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Change Log
 
 ## new version
 
+## 0.1.9
+
+* Bump supported Python versions #245
+
 ## 0.1.8
 
 * use logging instead of the `print` function  #138
 * use poetry for dependecy management  #139
 * validate blocking schemas with pydantic #140
 * move CI from Azure pipelines to GitHub actions #179
 * rewrite of `asses_blocks_2party` for better scaling #189
@@ -50,8 +54,8 @@
 Correct markdown rendering in Pypi
 
 ## 0.1.0
 
 Support two blocking methods that works for multiparty record linkage
 
 * Probabilistic signature
-* LSH based λ-fold
+* LSH based λ-fold
```

### Comparing `blocklib-0.1.8/LICENSE` & `blocklib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/README.md` & `blocklib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/__init__.py` & `blocklib-0.1.9/blocklib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import pkg_resources
+from importlib.metadata import version
 from .pprlindex import PPRLIndex
 from .pprlpsig import PPRLIndexPSignature
 from .pprllambdafold import PPRLIndexLambdaFold
 from .signature_generator import generate_signatures
 from .blocks_generator import generate_blocks, generate_reverse_blocks
 from .validation import validate_blocking_schema
 from .candidate_blocks_generator import generate_candidate_blocks
 from .encoding import generate_bloom_filter, flip_bloom_filter
 from .evaluation import assess_blocks_2party
 
-
-__version__ = pkg_resources.get_distribution('blocklib').version
+try:
+    __version__ = version('blocklib')
+except ImportError:
+    __version__ = 'unknown'
```

### Comparing `blocklib-0.1.8/blocklib/blocks_generator.py` & `blocklib-0.1.9/blocklib/blocks_generator.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/candidate_blocks_generator.py` & `blocklib-0.1.9/blocklib/candidate_blocks_generator.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/encoding.py` & `blocklib-0.1.9/blocklib/encoding.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/evaluation.py` & `blocklib-0.1.9/blocklib/evaluation.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/pprlindex.py` & `blocklib-0.1.9/blocklib/pprlindex.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/pprllambdafold.py` & `blocklib-0.1.9/blocklib/pprllambdafold.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/pprlpsig.py` & `blocklib-0.1.9/blocklib/pprlpsig.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/schemas/signature-config-schema.json` & `blocklib-0.1.9/blocklib/schemas/signature-config-schema.json`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/signature_generator.py` & `blocklib-0.1.9/blocklib/signature_generator.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/simmeasure.py` & `blocklib-0.1.9/blocklib/simmeasure.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/stats.py` & `blocklib-0.1.9/blocklib/stats.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/utils.py` & `blocklib-0.1.9/blocklib/utils.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/validation/__init__.py` & `blocklib-0.1.9/blocklib/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/validation/lambda_fold_validation.py` & `blocklib-0.1.9/blocklib/validation/lambda_fold_validation.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/blocklib/validation/psig_validation.py` & `blocklib-0.1.9/blocklib/validation/psig_validation.py`

 * *Files identical despite different names*

### Comparing `blocklib-0.1.8/pyproject.toml` & `blocklib-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blocklib"
-version = "0.1.8"
+version = "0.1.9"
 description = "A library for blocking in record linkage"
 license = "Apache-2.0"
 readme = "README.md"
 authors = [
     "Wilko Henecka <wilkohenecka@gmx.net>",
     "Joyce Wang <joyce.wang@csiro.au>",
     "Brian Thorne <brian@hardbyte.nz>"
@@ -21,15 +21,15 @@
     "schemas/*.json*"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/data61/blocklib/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = ">=3.8,<3.12"
 jsonschema = ">=3.1,<5.0"
 numpy = "^1.20.1"
 metaphone = "^0.6"
 tqdm = "^4.36.1"
 pydantic = "^1.8"
 typing_extensions = ">=3.7.4,<5.0.0"
 
@@ -38,23 +38,26 @@
 Sphinx = {version = "^4.1.0", optional = true}
 nbsphinx = {version = "^0.8.2", optional = true}
 pandas = {version = "^1.3.5", optional = true}
 notebook = {version = "^6.2.0", optional = true}
 bitarray = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
+pytest = "^7.1"
 pytest-cov = "^3.0"
-mypy = "^0.942"
+mypy = "^0.960"
 
 [tool.poetry.extras]
 docs = [
     "sphinx",
     "nbsphinx",
     "pandas",
     "notebook",
     "nbval"
 ]
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `blocklib-0.1.8/PKG-INFO` & `blocklib-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: blocklib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for blocking in record linkage
 Home-page: https://github.com/data61/blocklib
 License: Apache-2.0
 Author: Wilko Henecka
 Author-email: wilkohenecka@gmx.net
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=4.1.0,<5.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=4.1.0,<5.0.0) ; extra == "docs"
 Requires-Dist: bitarray (>=2.4.0,<3.0.0)
 Requires-Dist: jsonschema (>=3.1,<5.0)
 Requires-Dist: metaphone (>=0.6,<0.7)
-Requires-Dist: nbsphinx (>=0.8.2,<0.9.0); extra == "docs"
-Requires-Dist: nbval (>=0.9.6,<0.10.0); extra == "docs"
-Requires-Dist: notebook (>=6.2.0,<7.0.0); extra == "docs"
+Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs"
+Requires-Dist: nbval (>=0.9.6,<0.10.0) ; extra == "docs"
+Requires-Dist: notebook (>=6.2.0,<7.0.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.20.1,<2.0.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0); extra == "docs"
+Requires-Dist: pandas (>=1.3.5,<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: tqdm (>=4.36.1,<5.0.0)
 Requires-Dist: typing_extensions (>=3.7.4,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/data61/blocklib/issues
 Project-URL: Documentation, https://blocklib.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
```

