# Comparing `tmp/modeci-mdf-0.4.4.tar.gz` & `tmp/modeci-mdf-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeci-mdf-0.4.4.tar", last modified: Thu Feb 16 19:23:28 2023, max compression
+gzip compressed data, was "modeci-mdf-0.4.5.tar", last modified: Mon Apr 17 16:56:20 2023, max compression
```

## Comparing `modeci-mdf-0.4.4.tar` & `modeci-mdf-0.4.5.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.424185 modeci-mdf-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 19:23:16.000000 modeci-mdf-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-02-16 19:23:28.424185 modeci-mdf-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-02-16 19:23:16.000000 modeci-mdf-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-02-16 19:23:28.424185 modeci-mdf-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.412185 modeci-mdf-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.416185 modeci-mdf-0.4.4/src/modeci_mdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/full_translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.416185 modeci-mdf-0.4.4/src/modeci_mdf/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.416185 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.416185 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/functions/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/actr/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/actr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/actr/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/graphviz/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/graphviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16775 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/graphviz/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.420185 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/mdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/src/modeci_mdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.416185 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-02-16 19:23:28.000000 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-02-16 19:23:28.000000 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 19:23:28.000000 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-16 19:23:28.000000 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-16 19:23:28.000000 modeci-mdf-0.4.4/src/modeci_mdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 19:23:28.424185 modeci-mdf-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_mdf_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_onnx_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-02-16 19:23:17.000000 modeci-mdf-0.4.4/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 16:56:08.000000 modeci-mdf-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-17 16:56:08.000000 modeci-mdf-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50241 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/full_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/functions/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23284 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/mdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/src/modeci_mdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.821674 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 16:56:20.000000 modeci-mdf-0.4.5/src/modeci_mdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:56:20.825674 modeci-mdf-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_mdf_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_onnx_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-17 16:56:09.000000 modeci-mdf-0.4.5/tests/test_scheduler.py
```

### Comparing `modeci-mdf-0.4.4/LICENSE` & `modeci-mdf-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/PKG-INFO` & `modeci-mdf-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.4
+Version: 0.4.5
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
@@ -25,14 +25,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: psyneulink
 Provides-Extra: neuroml
+Provides-Extra: tensorflow
 Provides-Extra: test
 Provides-Extra: optional
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
```

### Comparing `modeci-mdf-0.4.4/README.md` & `modeci-mdf-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/pyproject.toml` & `modeci-mdf-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/setup.cfg` & `modeci-mdf-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/__init__.py` & `modeci-mdf-0.4.5/src/modeci_mdf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 widely-used programming environments in a range of disciplines, and for easily extending these to other environments.
 """
 
 # Version of the specification for MDF
 MODECI_MDF_VERSION = "0.4"
 
 # Version of the Python module.
-__version__ = "0.4.4"
+__version__ = "0.4.5"
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/execution_engine.py` & `modeci-mdf-0.4.5/src/modeci_mdf/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import attr
 import numpy as np
 
 import graph_scheduler
 import onnxruntime
 
 from modeci_mdf.functions.standard import mdf_functions, create_python_expression
-from modeci_mdf.utils import is_number
+
 
 from modelspec.utils import evaluate as evaluate_params_modelspec
 from modelspec.utils import _params_info, _val_info
 from modelspec.utils import FORMAT_NUMPY
 
 from collections import OrderedDict
 from typing import Union, List, Dict, Optional, Any, Tuple
@@ -46,14 +46,15 @@
     InputPort,
     Node,
     Parameter,
 )
 
 import modeci_mdf.functions.onnx as onnx_ops
 import modeci_mdf.functions.actr as actr_funcs
+import modeci_mdf.functions.ddm as ddm_funcs
 
 
 FORMAT_DEFAULT = FORMAT_NUMPY
 
 KNOWN_PARAMETERS = ["constant", "math", "numpy"] + dir(builtins)
 
 
@@ -363,14 +364,19 @@
                 self.verbose,
             )
         elif "actr." in expr:
             actr_function = getattr(actr_funcs, expr.split("(")[0].split(".")[-1])
             self.curr_value = actr_function(
                 *[func_params[arg] for arg in self.function.args]
             )
+        elif "ddm." in expr:
+            actr_function = getattr(ddm_funcs, expr.split("(")[0].split(".")[-1])
+            self.curr_value = ddm_function(
+                *[func_params[arg] for arg in self.function.args]
+            )
         else:
             self.curr_value = evaluate_expr(
                 expr, func_params, verbose=self.verbose, array_format=array_format
             )
 
         if self.verbose:
             print(
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/full_translator.py` & `modeci-mdf-0.4.5/src/modeci_mdf/full_translator.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/__init__.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/__init__.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 import random
 from .ccm.pattern import Pattern
 from .ccm.scheduler import Scheduler
 from .ccm.dm import Memory
 from .ccm.buffer import Chunk, Buffer
 from typing import Union, Dict, Any, Tuple, List, Callable
 
+__all__ = [
+    "chunk_to_string",
+    "pattern_to_string",
+    "change_goal",
+    "retrieve_chunk",
+    "match_production",
+    "pattern_matching_function",
+    "update_buffer",
+    "update_goal",
+    "update_retrieval",
+    "conflict_resolution_function",
+    "check_termination",
+]
+
 
 def chunk_to_string(chunk: Dict[str, str]) -> str:
     """Converts a chunk dictionary to a string format.
 
     Args:
         chunk: A dict representing a chunk.
 
@@ -200,73 +214,7 @@
     Args:
         production: A production dict that was selected.
 
     Returns:
         True if the production is empty.
     """
     return production == {}
-
-
-def get_actr_functions() -> List[Dict[str, Any]]:
-    """Creates a list of all the ACT-R functions as MDF specifications.
-
-    Returns:
-        A list of MDF function specifications.
-    """
-    actr_funcs = []
-    actr_funcs.append(
-        dict(
-            name="change_goal",
-            description="ACT-R change goal buffer function",
-            arguments=["pattern", "curr_goal"],
-            expression_string="actr.change_goal(pattern, curr_goal)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="retrieve_chunk",
-            description="ACT-R retrieve chunk function",
-            arguments=["pattern", "dm_chunks", "types"],
-            expression_string="actr.retrieve_chunk(pattern, dm_chunks, types)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="pattern_matching_function",
-            description="ACT-R pattern matching function",
-            arguments=["productions", "goal", "retrieval"],
-            expression_string="actr.pattern_matching_function(productions, goal, retrieval)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="conflict_resolution_function",
-            description="ACT-R conflict resolution function",
-            arguments=["productions"],
-            expression_string="actr.conflict_resolution_function(productions)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="update_goal",
-            description="ACT-R update goal buffer function",
-            arguments=["production"],
-            expression_string="actr.update_goal(production)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="update_retrieval",
-            description="ACT-R update retrieval buffer function",
-            arguments=["production"],
-            expression_string="actr.update_retrieval(production)",
-        )
-    )
-    actr_funcs.append(
-        dict(
-            name="check_termination",
-            description="check_termination",
-            arguments=["production"],
-            expression_string="actr.check_termination(production)",
-        )
-    )
-    return actr_funcs
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/buffer.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/buffer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/dm.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/dm.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/logger.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/logger.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/model.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/pattern.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/pattern.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/actr/ccm/scheduler.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/actr/ccm/scheduler.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/onnx.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,20 +216,25 @@
         opset_version: The opset version to use.
 
     Returns:
         A list of MDF function specifications. Each entry is a Dict that is feed directly to
             add_mdf_function.
     """
 
+    ops_blacklist = ["Loop", "Scan", "If"]
+
     mdf_funcspecs = []
     for schema in get_all_schemas_version(opset_version):
         args_list = [input.name for input in schema.inputs]
         params_list = [p for p in schema.attributes]
         args_params_str = ", ".join(args_list + params_list)
 
+        if schema.name in ops_blacklist:
+            continue
+
         mdf_funcspecs.append(
             dict(
                 name=f"onnx::{schema.name}",
                 description=schema.doc,
                 arguments=args_list,
                 expression_string=f"onnx_ops.{schema.name.lower()}({args_params_str})",
             )
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/functions/standard.py` & `modeci-mdf-0.4.5/src/modeci_mdf/functions/standard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 Implementation of core MDF function ontology.
 
 This module implements and registers all builtin MDF functions.
 
 """
-from typing import List, Dict
+import warnings
+
+from typing import List, Dict, Callable
+
+from docstring_parser import parse
+
 
 # Make sure we import math and numpy for Python expression strings. These imports
 # are important, do not remove even though they appear unused.
 import math
 import numpy
 
 
@@ -120,14 +125,84 @@
     func_str = f"def {name}({','.join(arguments)}):\n\treturn {expr}"
 
     res = {}
     exec(func_str, globals(), res)
     return res[name]
 
 
+def parse_description_and_args(f: Callable):
+    """Parse the description and arguments from a callable."""
+
+    # Parse the docstring into markdown format
+    p = parse(f.__doc__)
+
+    # Extract the description, use the long description if available.
+    # "short_description" only parse the first non-empty line and
+    # "long_description" parse the rest of the docstring i.e.
+    # it skips the first non-empty line and parse the rest of the docstring
+    if p.long_description:
+        description = f"{p.short_description} {p.long_description}"
+    else:
+        description = p.short_description
+
+    args = [p.arg_name for p in p.params]
+
+    return description, args
+
+
+def add_function_from_callable(f: Callable, module_alias: str = None):
+    """Adds a standard function from a callable.
+
+    Args:
+        f: A callable object.
+        module_alias: A string to prepend to the function name.
+
+    Returns:
+        None
+    """
+    description, args = parse_description_and_args(f)
+
+    expression_string = f.__name__ + "(" + ",".join(args) + ")"
+
+    if module_alias:
+        expression_string = module_alias + "." + expression_string
+
+    add_mdf_function(
+        name=f.__name__,
+        description=description,
+        arguments=args,
+        expression_string=expression_string,
+    )
+
+
+def add_public_functions_from_module(module, module_alias: str = None):
+    """Adds all public functions from a module to MDF standard functions.
+
+    Args:
+        module: A module object.
+        module_alias: A string to prepend to the function names.
+
+    Returns:
+        None
+    """
+
+    try:
+        for name in module.__all__:
+            if callable(module.__dict__[name]):
+                add_function_from_callable(
+                    module.__dict__[name], module_alias=module_alias
+                )
+
+    except AttributeError:
+        warnings.warn(
+            f"Module {module.__name__} does not have an __all__ attribute. "
+            f"No MDF standard functions were found."
+        )
+
+
 # Populate the list of known functions
 
 if len(mdf_functions) == 0:
 
     STANDARD_ARG_0 = "variable0"
     STANDARD_ARG_1 = "variable1"
 
@@ -212,19 +287,22 @@
     # Enumerate all available ONNX operators and add them as MDF functions.
     from modeci_mdf.functions.onnx import get_onnx_ops
 
     for mdf_func_spec in get_onnx_ops():
         add_mdf_function(**mdf_func_spec)
 
     # Add the ACT-R functions.
-    from modeci_mdf.functions.actr import get_actr_functions
+    import modeci_mdf.functions.actr as actr
 
-    for mdf_func_spec in get_actr_functions():
-        add_mdf_function(**mdf_func_spec)
+    add_public_functions_from_module(actr, module_alias="actr")
+
+    # Add the DDM functions.
+    import modeci_mdf.functions.ddm as ddm
 
+    add_public_functions_from_module(ddm, module_alias="ddm")
 
 if __name__ == "__main__":
 
     import pprint
 
     pp = pprint.PrettyPrinter(indent=4)
     pp.pprint(mdf_functions)
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/actr/importer.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/actr/importer.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/graphviz/exporter.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/graphviz/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 NO_VIEW = "-noview"
 
 LEVEL_1 = 1
 LEVEL_2 = 2
 LEVEL_3 = 3
 
 COLOR_MAIN = "#444444"
-# COLOR_BG_MAIN = "#999911"
+COLOR_BG_MAIN = "#ffffff"
 COLOR_LABEL = "#666666"
 COLOR_NUM = "#444444"
 COLOR_PARAM = "#1666ff"
 COLOR_INPUT = "#188855"
 COLOR_FUNC = "#441199"
 COLOR_OUTPUT = "#cc3355"
 COLOR_COND = "#ffa1d"
@@ -139,14 +139,15 @@
     mdf_graph,
     engine="dot",
     output_format="png",
     view_on_render=False,
     level=LEVEL_2,
     filename_root=None,
     is_horizontal=False,
+    solid_color=False,
 ):
 
     DEFAULT_POP_SHAPE = "ellipse"
     DEFAULT_ARROW_SHAPE = "empty"
 
     print(
         f"Converting MDF graph: {mdf_graph.id} to graphviz (level: {level}, format: {output_format})"
@@ -195,36 +196,84 @@
             info += "</td></tr>"
         if nt.type == "And":
             info += "<tr><td>{}{} = All conditions in the Graph are satisfied".format(
                 format_label(" "),
                 format_term_condition("Termination cond"),
             )
             info += "</td></tr>"
+        if nt.type == "All":
+            info += "<tr><td>{}{} = Satisfied when".format(
+                format_label(" "),
+                format_term_condition("Termination cond"),
+            )
+            i = 0
+            for item in args.get("dependencies"):
+                while i < (len(args.get("dependencies")) - 1):
+                    info += " <b>{}</b> condition on node <b>{}</b> has ran after <b>{}</b> times and ".format(
+                        item.type, item.kwargs["dependencies"], item.kwargs["n"]
+                    )
+                    i = i + 1
+
+            info += " <b>{}</b> condition on node <b>{}</b> has ran after <b>{}</b> times. ".format(
+                item.type, item.kwargs["dependencies"], item.kwargs["n"]
+            )
+
+            info += "</td></tr>"
         info += "</table>"
         graph.node("termination condition", label="<%s>" % info)
 
     for node in mdf_graph.nodes:
         print("    Node: %s" % node.id)
         color = COLOR_MAIN
+        fillcolor = COLOR_BG_MAIN
         penwidth = "1"
-        # bg_color = COLOR_BG_MAIN
 
         if node.metadata is not None:
             if "color" in node.metadata:
                 color = color_rgb_to_hex(node.metadata["color"])
                 penwidth = "2"
 
-        graph.attr(
-            "node",
-            color=color,
-            style="rounded",
-            shape="box",
-            fontcolor=COLOR_MAIN,
-            penwidth=penwidth,
-        )
+        if solid_color:
+            rgb_ = None
+            if node.metadata is not None and "color" in node.metadata:
+                fillcolor = color
+                rgb_ = node.metadata["color"].split(" ")
+
+                if (
+                    float(rgb_[0]) * 0.299
+                    + float(rgb_[1]) * 0.587
+                    + float(rgb_[2]) * 0.2
+                ) > 0.45:
+                    fcolor = "black"
+                else:
+                    fcolor = "white"
+            else:
+                fcolor = "black"
+
+            # print(f"Bkgd color: {rgb_} ({color}), font: {fcolor}")
+
+            graph.attr(
+                "node",
+                color=color,
+                fillcolor=fillcolor,
+                style="rounded,filled",
+                shape="box",
+                fontcolor=fcolor,
+                penwidth=penwidth,
+            )
+        else:
+            graph.attr(
+                "node",
+                color=color,
+                style="rounded",
+                shape="box",
+                fontcolor=COLOR_MAIN,
+                penwidth=penwidth,
+            )
+
         info = '<table border="0" cellborder="0">'
         info += '<tr><td colspan="2"><b>%s</b></td></tr>' % (node.id)
 
         if node.metadata is not None and level >= LEVEL_3:
 
             info += "<tr><td>%s" % format_label("METADATA")
 
@@ -360,14 +409,23 @@
                         format_condition("condition"),
                         node.id,
                         args.get("n"),
                         args.get("dependencies"),
                     )
                     info += "</td></tr>"
                 elif ns.type == "AfterNCalls":
+                    info += "<tr><td>{}{} = <b>{}</b> will run when or after <b>{}</b> calls of <b>{}</b>".format(
+                        format_label(" "),
+                        format_condition("condition"),
+                        node.id,
+                        args.get("n"),
+                        args.get("dependencies"),
+                    )
+                    info += "</td></tr>"
+                elif ns.type == "AfterCall":
                     info += "<tr><td>{}{} = <b>{}</b> will run after <b>{}</b> calls of <b>{}</b>".format(
                         format_label(" "),
                         format_condition("condition"),
                         node.id,
                         args.get("n"),
                         args.get("dependencies"),
                     )
@@ -411,15 +469,15 @@
 
             if node.output_ports and len(node.output_ports) > 0:
                 for op in node.output_ports:
                     info += "<tr><td>{}{} = {} {}</td></tr>".format(
                         format_label("OUT"),
                         format_output(op.id),
                         match_in_expr(op.value, node),
-                        "(shape: %s)" % op.shape
+                        "(shape: %s)" % str(op.shape)
                         if op.shape is not None
                         else ""
                         if level >= LEVEL_2 and op.shape is not None
                         else "",
                     )
 
         info += "</table>"
@@ -489,8 +547,9 @@
     # nmllite_file = example.replace('.json','.nmllite.json')
     mdf_to_graphviz(
         mod_graph,
         engine=engines["d"],
         view_on_render=view,
         level=int(sys.argv[2]),
         is_horizontal=is_horizontal,
+        solid_color=False,
     )
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/exporter.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/neuroml/syn_definitions.xml`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/exporter.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/onnx/importer.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/onnx/importer.py`

 * *Files 17% similar despite different names*

```diff
@@ -344,14 +344,96 @@
     onnx_model = onnx.load(input_file)
     onnx.checker.check_model(onnx_model)
     mdf_model = onnx_to_mdf(onnx_model)
     mdf_model.to_json_file(f"{out_filename}.json")
     mdf_model.to_yaml_file(f"{out_filename}.yaml")
 
 
+# The data used for getting the name and categories of graphs are gotten here https://raw.githubusercontent.com/lutzroeder/netron/main/source/onnx-metadata.json'
+
+# the data used for getting the color of categories of graphs are gotten here 'https://github.com/lutzroeder/netron/blob/b7a0be975f852c2c2fbce4a6fce69a37819b3601/source/grapher.css#L27'
+
+
+new_dict = {
+    "AveragePool": "Pool",
+    "BatchNormalization": "Normalization",
+    "Clip": "Activation",
+    "Concat": "Tensor",
+    "Constant": "Constant",
+    "Conv": "Layer",
+    "ConvInteger": "Layer",
+    "ConvTranspose": "Layer",
+    "Dropout": "Dropout",
+    "Elu": "Activation",
+    "Flatten": "Shape",
+    "GRU": "Layer",
+    "Gather": "Transform",
+    "Gemm": "Layer",
+    "GlobalAveragePool": "Pool",
+    "GlobalLpPool": "Pool",
+    "GlobalMaxPool": "Pool",
+    "HardSigmoid": "Activation",
+    "InstanceNormalization": "Normalization",
+    "LRN": "Normalization",
+    "LSTM": "Layer",
+    "LeakyRelu": "Activation",
+    "LogSoftmax": "Activation",
+    "LpNormalization": "Normalization",
+    "LpPool": "Pool",
+    "MaxPool": "Pool",
+    "MaxRoiPool": "Pool",
+    "PRelu": "Activation",
+    "Pad": "Tensor",
+    "RNN": "Layer",
+    "Relu": "Activation",
+    "Reshape": "Shape",
+    "Selu": "Activation",
+    "Sigmoid": "Activation",
+    "Slice": "Tensor",
+    "Softmax": "Activation",
+    "Softplus": "Activation",
+    "Softsign": "Activation",
+    "Split": "Tensor",
+    "Squeeze": "Transform",
+    "Tanh": "Activation",
+    "ThresholdedRelu": "Activation",
+    "Tile": "Shape",
+    "Transpose": "Transform",
+    "Unsqueeze": "Transform",
+    "Upsample": "Data",
+    "FusedConv": "Layer",
+}
+
+color_dict = {
+    "Activation": ".4 .2 .1",
+    "Layer": ".2 .3 .5",
+    "Pool": ".2 .3 .2",
+    "Normalization": ".2 .3 .3",
+    "Tensor": ".3 .3 .2",
+    "Transform": ".2 .3 .3",
+    "Shape": ".4 .3 .3",
+    "Dropout": ".3 .3 .4",
+    "Data": ".3 .3 .3",
+}
+
+
+def get_category_of_onnx_node(entry):
+    for key, value in new_dict.items():
+        if key in entry:
+            return value
+
+
+def get_color_for_onnx_category(shape):
+    a = {}
+    for key, val in color_dict.items():
+        if shape == key:
+            a["color"] = val
+            return a
+
+
 def main():
 
     import argparse
 
     parser = argparse.ArgumentParser(
         description="Simple converter from ONNX to MDF. "
         "Takes in ONNX files and generates MDF JSON/YAML"
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/builtins.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/exporter.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/exporter.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/importer.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 """
 import inspect
 import logging
 
 from typing import Union, Dict, Any, Tuple, List, Callable
 import onnx.defs
 
-
 import torch
 
 from modeci_mdf.mdf import Model, Graph, Node, Edge, InputPort, OutputPort, Parameter
 from modeci_mdf.functions.onnx import onnx_opset_version as modeci_onnx_opset_version
 
 
 logger = logging.getLogger(__name__)
@@ -321,14 +320,24 @@
     # Get the argument names and parameter names and values for this Node's operation
     if "onnx::" in op:
         arguments, parameters = process_onnx_schema(node, consts, port_mapper)
     else:
         arguments, parameters = process_torch_schema(node, consts, port_mapper)
 
     mdf_node = Node(id=make_node_id(node))
+
+    from modeci_mdf.interfaces.onnx.importer import (
+        get_category_of_onnx_node,
+        get_color_for_onnx_category,
+    )
+
+    category = get_category_of_onnx_node(mdf_node.id)
+    color = get_color_for_onnx_category(category)
+    mdf_node.metadata = color
+
     for p in parameters:
         mdf_node.parameters.append(Parameter(id=p, value=parameters[p]))
 
     # Add any output ports
     subscript = lambda x: "" if len(schema.outputs) <= 1 else f"[{x}]"
     for out_num, o in enumerate(outputs):
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py` & `modeci-mdf-0.4.5/src/modeci_mdf/interfaces/pytorch/mod_torch_builtins.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/mdf.py` & `modeci-mdf-0.4.5/src/modeci_mdf/mdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,36 +532,39 @@
         engine: str = "dot",
         output_format: str = "png",
         view_on_render: bool = False,
         level: int = 2,
         filename_root: Optional[str] = None,
         only_warn_on_fail: bool = False,
         is_horizontal: bool = False,
+        solid_color=False,
     ):
         """Convert MDF graph to an image (png or svg) using the Graphviz export
 
         Args:
             engine: dot or other Graphviz formats
             output_format: e.g. png (default) or svg
             view_on_render: if True, will open generated image in system viewer
             level: 1,2,3, depending on how much detail to include
             filename_root: will change name of file generated to filename_root.png, etc.
             only_warn_on_fail: just give a warning if this fails, e.g. no dot executable. Useful for preventing errors in automated tests
+            solid_color: if True, will return a solid color for the graphviz node.  default is False
         """
         from modeci_mdf.interfaces.graphviz.exporter import mdf_to_graphviz
 
         try:
             mdf_to_graphviz(
                 self.graphs[0],
                 engine=engine,
                 output_format=output_format,
                 view_on_render=view_on_render,
                 level=level,
                 filename_root=filename_root,
                 is_horizontal=is_horizontal,
+                solid_color=solid_color,
             )
 
         except Exception as e:
             if only_warn_on_fail:
                 import traceback
 
                 print(traceback.format_exc())
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf/utils.py` & `modeci-mdf-0.4.5/src/modeci_mdf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     """
     return Model.from_yaml_file(filename)
 
 
 def color_rgb_to_hex(rgb):
     """Convert a rgb color to hexadecimal format."""
     color = "#"
-    print("Converting %s to hex color" % rgb)
+    # print("Converting %s to hex color" % rgb)
     for a in rgb.split():
         color = color + "%02x" % int(float(a) * 255)
     return color
 
 
 def is_number(s):
     """Return :code:`True` if cast to :code:`float` does not throw ValueError, :code:`False` otherwise."""
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf.egg-info/PKG-INFO` & `modeci-mdf-0.4.5/src/modeci_mdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeci-mdf
-Version: 0.4.4
+Version: 0.4.5
 Summary: ModECI (Model Exchange and Convergence Initiative) Model Description Format
 Home-page: https://www.modeci.org
 Author: ModECI contributors
 Author-email: p.gleeson@gmail.com
 Maintainer: ModECI contributors
 Maintainer-email: p.gleeson@gmail.com
 License: LGPLv3
@@ -25,14 +25,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: psyneulink
 Provides-Extra: neuroml
+Provides-Extra: tensorflow
 Provides-Extra: test
 Provides-Extra: optional
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf.egg-info/SOURCES.txt` & `modeci-mdf-0.4.5/src/modeci_mdf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/modeci_mdf/utils.py
 src/modeci_mdf.egg-info/PKG-INFO
 src/modeci_mdf.egg-info/SOURCES.txt
 src/modeci_mdf.egg-info/dependency_links.txt
 src/modeci_mdf.egg-info/requires.txt
 src/modeci_mdf.egg-info/top_level.txt
 src/modeci_mdf/functions/__init__.py
+src/modeci_mdf/functions/ddm.py
 src/modeci_mdf/functions/onnx.py
 src/modeci_mdf/functions/standard.py
 src/modeci_mdf/functions/actr/__init__.py
 src/modeci_mdf/functions/actr/ccm/__init__.py
 src/modeci_mdf/functions/actr/ccm/buffer.py
 src/modeci_mdf/functions/actr/ccm/dm.py
 src/modeci_mdf/functions/actr/ccm/logger.py
```

### Comparing `modeci-mdf-0.4.4/src/modeci_mdf.egg-info/requires.txt` & `modeci-mdf-0.4.5/src/modeci_mdf.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 [:python_version < "3.7"]
 dataclasses
 
 [:python_version < "3.8"]
 typing_compat
 
 [all]
+grpcio-tools==1.42.0
 psyneulink
 pyNeuroML>=0.5.20
 neuromllite>=0.5.2
+tensorflow
+keras_visualizer
+pydot
 pytest
 pytest-benchmark
 pytest-mock
 Sphinx~=3.0
 recommonmark>=0.5.0
 nbsphinx
 sphinx_copybutton
@@ -70,16 +74,22 @@
 torchviz
 netron
 torch>=1.11.0
 torchvision<=0.12.0
 h5py
 
 [psyneulink]
+grpcio-tools==1.42.0
 psyneulink
 
+[tensorflow]
+tensorflow
+keras_visualizer
+pydot
+
 [test]
 pytest
 pytest-benchmark
 pytest-mock
 
 [test:python_version < "3.8"]
 typing_extensions
```

### Comparing `modeci-mdf-0.4.4/tests/test_examples.py` & `modeci-mdf-0.4.5/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 example_scripts = glob.glob("examples/**/*.py", recursive=True)
 example_mdf_scripts = {
     Path(f) for f in glob.glob("examples/MDF/**/*.py", recursive=True)
 }
 example_pnl_scripts = {
     Path(f) for f in glob.glob("examples/PsyNeuLink/**/*.py", recursive=True)
 }
-example_exclusion_strings = [".reconstructed.py", "generate_json_and_scripts.py"]
+example_exclusion_strings = [
+    ".reconstructed.py",
+    "generate_json_and_scripts.py",
+    "pytorch_ddm.py",
+]
 
 # Filter any excluded example scripts
 example_scripts = [
     script
     for script in example_scripts
     if all(e not in script for e in example_exclusion_strings)
 ]
```

### Comparing `modeci-mdf-0.4.4/tests/test_execution.py` & `modeci-mdf-0.4.5/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_helpers.py` & `modeci-mdf-0.4.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_mdf_functions.py` & `modeci-mdf-0.4.5/tests/test_mdf_functions.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_model.py` & `modeci-mdf-0.4.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_onnx_functions.py` & `modeci-mdf-0.4.5/tests/test_onnx_functions.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_parameters.py` & `modeci-mdf-0.4.5/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `modeci-mdf-0.4.4/tests/test_scheduler.py` & `modeci-mdf-0.4.5/tests/test_scheduler.py`

 * *Files identical despite different names*

