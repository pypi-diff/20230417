# Comparing `tmp/spacy-transformers-1.2.2.tar.gz` & `tmp/spacy-transformers-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-transformers-1.2.2.tar", last modified: Fri Feb 17 20:06:49 2023, max compression
+gzip compressed data, was "spacy-transformers-1.2.3.tar", last modified: Mon Apr 17 12:38:13 2023, max compression
```

## Comparing `spacy-transformers-1.2.2.tar` & `spacy-transformers-1.2.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.654739 spacy-transformers-1.2.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5246 2023-02-17 20:06:49.654739 spacy-transformers-1.2.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3828 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-02-17 20:06:49.654739 spacy-transformers-1.2.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.642739 spacy-transformers-1.2.2/spacy_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/align.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/align.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/annotation_setters.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/data_classes.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.646739 spacy-transformers-1.2.2/spacy_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/hf_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/hf_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/listener.py
--rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/split_trf.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4772 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/layers/trfs2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/span_getters.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.654739 spacy-transformers-1.2.2/spacy_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.654739 spacy-transformers-1.2.2/spacy_transformers/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/regression/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/regression/test_spacy_issue6401.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/regression/test_spacy_issue7029.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_alignment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_configs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_data_classes.py
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_deprecations.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_model_sequence_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_model_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9765 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_spanners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3121 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_tok2vectransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/test_truncation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/truncate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-02-17 20:04:59.000000 spacy-transformers-1.2.2/spacy_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-17 20:06:49.642739 spacy-transformers-1.2.2/spacy_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5246 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1832 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-02-17 20:06:49.000000 spacy-transformers-1.2.2/spacy_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     5491 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4073 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.270227 spacy-transformers-1.2.3/spacy_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/align.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/align.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/annotation_setters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/data_classes.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.274227 spacy-transformers-1.2.3/spacy_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/hf_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/hf_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/listener.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/split_trf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/trfs2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/span_getters.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/spacy_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/spacy_transformers/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue6401.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue7029.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_alignment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_configs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_data_classes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_deprecations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_model_sequence_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_model_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_spanners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_textcatcnn.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_tok2vectransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_truncation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/truncate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.270227 spacy-transformers-1.2.3/spacy_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5491 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/top_level.txt
```

### Comparing `spacy-transformers-1.2.2/LICENSE` & `spacy-transformers-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/PKG-INFO` & `spacy-transformers-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.2
+Version: 1.2.3
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -110,7 +110,13 @@
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
 - 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
   component API reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
+
+## Bug reports and other issues
+
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions)
+for any other issue.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.2 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.3 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -61,8 +61,11 @@
 spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
 ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
 and update components on your own data and integrate custom models - ð
 [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
 Power spaCy components with custom neural networks - ð [`Transformer`]
 (https://spacy.io/api/transformer): Pipeline component API reference - ð
 [Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions
+Architectures and registered functions ## Bug reports and other issues Please
+use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the [discussion board](https://
+github.com/explosion/spaCy/discussions) for any other issue.
```

### Comparing `spacy-transformers-1.2.2/README.md` & `spacy-transformers-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,7 +70,13 @@
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
 - 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
   component API reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
+
+## Bug reports and other issues
+
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions)
+for any other issue.
```

#### html2text {}

```diff
@@ -43,8 +43,11 @@
 spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
 ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
 and update components on your own data and integrate custom models - ð
 [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
 Power spaCy components with custom neural networks - ð [`Transformer`]
 (https://spacy.io/api/transformer): Pipeline component API reference - ð
 [Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions
+Architectures and registered functions ## Bug reports and other issues Please
+use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the [discussion board](https://
+github.com/explosion/spaCy/discussions) for any other issue.
```

### Comparing `spacy-transformers-1.2.2/setup.cfg` & `spacy-transformers-1.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.2
+version = 1.2.3
 description = spaCy pipelines for pre-trained BERT and other transformers
 url = https://spacy.io
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -29,15 +29,15 @@
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.5.0,<4.0.0
 	numpy>=1.15.0
-	transformers>=3.4.0,<4.27.0
+	transformers>=3.4.0,<4.29.0
 	torch>=1.8.0
 	srsly>=2.4.0,<3.0.0
 	dataclasses>=0.6,<1.0; python_version < "3.7"
 	spacy-alignments>=0.7.2,<1.0.0
 
 [options.extras_require]
 cuda =
```

### Comparing `spacy-transformers-1.2.2/setup.py` & `spacy-transformers-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/align.pyi` & `spacy-transformers-1.2.3/spacy_transformers/align.pyi`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/align.pyx` & `spacy-transformers-1.2.3/spacy_transformers/align.pyx`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/annotation_setters.py` & `spacy-transformers-1.2.3/spacy_transformers/annotation_setters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/architectures.py` & `spacy-transformers-1.2.3/spacy_transformers/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/data_classes.py` & `spacy-transformers-1.2.3/spacy_transformers/data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/layers/_util.py` & `spacy-transformers-1.2.3/spacy_transformers/layers/_util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/layers/hf_shim.py` & `spacy-transformers-1.2.3/spacy_transformers/layers/hf_shim.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/layers/hf_wrapper.py` & `spacy-transformers-1.2.3/spacy_transformers/layers/hf_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/layers/listener.py` & `spacy-transformers-1.2.3/spacy_transformers/layers/listener.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/layers/transformer_model.py` & `spacy-transformers-1.2.3/spacy_transformers/layers/transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/pipeline_component.py` & `spacy-transformers-1.2.3/spacy_transformers/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/span_getters.py` & `spacy-transformers-1.2.3/spacy_transformers/span_getters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/regression/test_spacy_issue6401.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue6401.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/regression/test_spacy_issue7029.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue7029.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_alignment.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_configs.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_data_classes.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_model_sequence_classification.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_model_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_model_wrapper.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_pipeline_component.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_serialize.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .. import TransformerData
 
 
 DEFAULT_CONFIG = {
     "model": {
         "@architectures": "spacy-transformers.TransformerModel.v3",
-        "name": "distilbert-base-uncased",
+        "name": "hf-internal-testing/tiny-random-DistilBertModel",
         "tokenizer_config": {"use_fast": False},
     }
 }
 
 
 def test_serialize_transformer_data():
     data = {"x": TransformerData.empty()}
@@ -30,15 +30,15 @@
     assert isinstance(new_data["x"], TransformerData)
 
     nlp = Language()
     nlp.add_pipe(
         "transformer",
         config={
             "model": {
-                "name": "distilbert-base-uncased",
+                "name": "hf-internal-testing/tiny-random-DistilBertModel",
                 "transformer_config": {"output_attentions": True},
             }
         },
     )
     nlp.initialize()
     doc = nlp("This is a test.")
     b = doc.to_bytes()
@@ -182,15 +182,15 @@
 
     [components.tagger.model]
     @architectures = "spacy.Tagger.v1"
     nO = null
 
     [components.tagger.model.tok2vec]
     @architectures = "spacy-transformers.Tok2VecTransformer.v3"
-    name = "distilbert-base-uncased"
+    name = "hf-internal-testing/tiny-random-DistilBertModel"
     tokenizer_config = {"use_fast": true}
     transformer_config = {"output_attentions": false}
     grad_factor = 1.0
 
     [components.tagger.model.tok2vec.get_spans]
     @span_getters = "spacy-transformers.strided_spans.v1"
     window = 256
```

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_spanners.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_tok2vectransformer.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_tok2vectransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     [components.tagger.model]
     @architectures = "spacy.Tagger.v1"
     nO = null
 
     [components.tagger.model.tok2vec]
     @architectures = "spacy-transformers.Tok2VecTransformer.v1"
-    name = "roberta-base"
+    name = "distilbert-base-uncased"
     tokenizer_config = {"use_fast": false}
     grad_factor = 1.0
 
     [components.tagger.model.tok2vec.get_spans]
     @span_getters = "spacy-transformers.strided_spans.v1"
     window = 256
     stride = 256
```

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/test_truncation.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/tests/util.py` & `spacy-transformers-1.2.3/spacy_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/truncate.py` & `spacy-transformers-1.2.3/spacy_transformers/truncate.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers/util.py` & `spacy-transformers-1.2.3/spacy_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers.egg-info/PKG-INFO` & `spacy-transformers-1.2.3/spacy_transformers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.2
+Version: 1.2.3
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -110,7 +110,13 @@
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
 - 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
   component API reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
+
+## Bug reports and other issues
+
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions)
+for any other issue.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.2 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.3 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -61,8 +61,11 @@
 spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
 ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
 and update components on your own data and integrate custom models - ð
 [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
 Power spaCy components with custom neural networks - ð [`Transformer`]
 (https://spacy.io/api/transformer): Pipeline component API reference - ð
 [Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions
+Architectures and registered functions ## Bug reports and other issues Please
+use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the [discussion board](https://
+github.com/explosion/spaCy/discussions) for any other issue.
```

### Comparing `spacy-transformers-1.2.2/spacy_transformers.egg-info/SOURCES.txt` & `spacy-transformers-1.2.3/spacy_transformers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,13 +37,14 @@
 spacy_transformers/tests/test_data_classes.py
 spacy_transformers/tests/test_deprecations.py
 spacy_transformers/tests/test_model_sequence_classification.py
 spacy_transformers/tests/test_model_wrapper.py
 spacy_transformers/tests/test_pipeline_component.py
 spacy_transformers/tests/test_serialize.py
 spacy_transformers/tests/test_spanners.py
+spacy_transformers/tests/test_textcatcnn.py
 spacy_transformers/tests/test_tok2vectransformer.py
 spacy_transformers/tests/test_truncation.py
 spacy_transformers/tests/util.py
 spacy_transformers/tests/regression/__init__.py
 spacy_transformers/tests/regression/test_spacy_issue6401.py
 spacy_transformers/tests/regression/test_spacy_issue7029.py
```

### Comparing `spacy-transformers-1.2.2/spacy_transformers.egg-info/entry_points.txt` & `spacy-transformers-1.2.3/spacy_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.2/spacy_transformers.egg-info/requires.txt` & `spacy-transformers-1.2.3/spacy_transformers.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spacy<4.0.0,>=3.5.0
 numpy>=1.15.0
-transformers<4.27.0,>=3.4.0
+transformers<4.29.0,>=3.4.0
 torch>=1.8.0
 srsly<3.0.0,>=2.4.0
 spacy-alignments<1.0.0,>=0.7.2
 
 [:python_version < "3.7"]
 dataclasses<1.0,>=0.6
```

