# Comparing `tmp/datumaro-1.2.0rc1.tar.gz` & `tmp/datumaro-1.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.2.0rc1.tar", last modified: Fri Apr 14 10:11:45 2023, max compression
+gzip compressed data, was "datumaro-1.2.0rc2.tar", last modified: Mon Apr 17 05:09:49 2023, max compression
```

## Comparing `datumaro-1.2.0rc1.tar` & `datumaro-1.2.0rc2.tar`

### file list

```diff
@@ -1,303 +1,307 @@
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)   361854 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/3rd-party.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1090 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/LICENSE
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      103 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/MANIFEST.in
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      229 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/NOTICE
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5901 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/PKG-INFO
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5328 2023-03-29 05:58:32.000000 datumaro-1.2.0rc1/README.md
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1715 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      178 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/__main__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/capi/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3379 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/capi/pybind.cpp
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-04-03 09:17:53.000000 datumaro-1.2.0rc1/datumaro/cli/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5494 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/__main__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      962 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5063 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/convert.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3991 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/detect_format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10146 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/download.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9340 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/explain.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9046 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/filter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3073 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/generate.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9396 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/cli/commands/merge.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5979 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/patch.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1355 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/__init__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      134 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9162 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/diff.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5906 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/export.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4242 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/info.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3120 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/stats.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8369 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/transform.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4843 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/validate.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      116 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5227 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/add.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1957 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/create.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5892 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/import_.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1677 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/remove.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      123 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2946 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2150 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/commit.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2758 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/info.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1132 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/log.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1412 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/status.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4250 2023-04-05 05:07:46.000000 datumaro-1.2.0rc1/datumaro/cli/commands/search.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/contexts/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      121 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9089 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/model.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/contexts/project/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4501 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/project/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2553 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/source.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4097 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/contexts/util.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.272044 datumaro-1.2.0rc1/datumaro/cli/util/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3988 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13328 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/diff.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      391 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/cli/util/errors.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5638 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/cli/util/project.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/__init__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/algorithms/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      135 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/__init__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      111 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7851 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8073 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/algorithms/rise.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    29706 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/annotation.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/annotations/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      118 2023-03-30 07:03:27.000000 datumaro-1.2.0rc1/datumaro/components/annotations/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8964 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/annotations/matcher.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5242 2023-03-30 07:03:27.000000 datumaro-1.2.0rc1/datumaro/components/annotations/merger.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2146 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/cli_plugin.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8101 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/config.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3570 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/config_model.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2240 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/crypter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    52703 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/dataset.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10947 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/dataset_base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9776 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/environment.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17884 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/errors.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13568 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19651 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/extractor_tfds.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10063 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/filter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19613 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/format_detection.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      534 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/generator.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/hl_ops/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8556 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/hl_ops/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8657 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/components/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2901 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/launcher.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    36037 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/media.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2450 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/media_manager.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/components/merge/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      662 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2047 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11438 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/exact_merge.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20825 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/intersect_merge.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3412 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/merge/union_merge.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    23475 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/operations.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5222 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/components/progress_reporting.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    89324 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/components/project.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5206 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/searcher.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9352 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/shift_analyzer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1830 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/transformer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2105 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/components/validator.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17135 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/components/visualizer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      164 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/errors.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      172 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/ops.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/__init__.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1148 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.276044 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4038 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2217 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       77 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6297 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2017.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8482 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2020.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      232 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5909 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2351 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    14655 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1514 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2129 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/importer.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8441 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5585 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3501 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3659 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats_numpy.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17438 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/camvid.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      183 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7512 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10476 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/celeba.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12141 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cifar.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20683 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cityscapes.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.280044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    19013 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    28658 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      477 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6074 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6348 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3128 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_super_resolution.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    13642 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20627 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      214 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/format.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       72 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11047 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    15359 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      317 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1236 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/importer.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      286 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6627 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11117 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      828 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1921 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      631 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11105 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2236 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1563 2023-03-30 05:54:18.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5235 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11780 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6440 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      311 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1828 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_dir.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3950 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_zip.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6824 2023-04-14 10:02:55.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8124 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet_txt.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5752 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kinetics.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5975 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11358 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3970 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3713 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/importer.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11148 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    17769 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      711 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    20175 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/labelme.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    14960 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/lfw.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10904 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12550 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3712 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6396 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/market1501.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5013 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mars.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9041 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7026 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist_csv.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10664 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mot.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6493 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mots.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.284044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      556 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5193 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4937 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3937 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4813 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      563 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1873 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1625 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    38486 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/open_images.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6888 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16130 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      420 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7024 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/synthia.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7629 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8812 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      308 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    15332 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vgg_face2.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6379 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/video.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16609 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    30069 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9071 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2897 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2813 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_csv.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3854 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_json.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10103 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/widerface.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12374 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/base.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    12070 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/exporter.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      457 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/format.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5573 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/importer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    16787 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/ndr.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        0 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9757 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/launcher.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/sampler/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       72 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     7785 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/random_sampler.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8754 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/sampler/relevancy_sampler.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2869 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/searcher.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1213 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/shift_analyzer.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    32124 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/splitter.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      155 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11335 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/background_colors.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11577 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/image_generator.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6194 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/utils.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.288044 datumaro-1.2.0rc1/datumaro/plugins/tiling/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      116 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9398 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/merge_tile.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     9834 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/tile.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1141 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/tiling/util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    41229 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/plugins/transforms.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    47389 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/plugins/validators.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      376 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/project.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/datumaro/util/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4809 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/__init__.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8473 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/annotation_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     1198 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/attrs_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      262 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/definitions.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      882 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/util/file_utils.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11657 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/datumaro/util/image.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      968 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/image_cache.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      795 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/log_utils.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    11440 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/mask_tools.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2062 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/meta_file_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     8479 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/os_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      758 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/util/pickle_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      246 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/samples.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     4702 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/scope.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      616 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/telemetry_stub.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     6254 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/datumaro/util/telemetry_utils.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2579 2023-03-29 05:59:21.000000 datumaro-1.2.0rc1/datumaro/util/tf_util.py
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       25 2023-04-14 10:04:40.000000 datumaro-1.2.0rc1/datumaro/version.py
-drwxrwxr-x   0 vinnamki  (1000) vinnamki  (1000)        0 2023-04-14 10:11:45.268044 datumaro-1.2.0rc1/datumaro.egg-info/
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     5901 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/PKG-INFO
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)    10677 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/SOURCES.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        1 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/dependency_links.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       53 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/entry_points.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      764 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/requires.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)        9 2023-04-14 10:11:45.000000 datumaro-1.2.0rc1/datumaro.egg-info/top_level.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     2488 2023-03-29 05:58:33.000000 datumaro-1.2.0rc1/pyproject.toml
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      692 2023-04-14 10:02:59.000000 datumaro-1.2.0rc1/requirements-core.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)      266 2023-03-29 05:58:32.000000 datumaro-1.2.0rc1/requirements-default.txt
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)       38 2023-04-14 10:11:45.292044 datumaro-1.2.0rc1/setup.cfg
--rw-rw-r--   0 vinnamki  (1000) vinnamki  (1000)     3342 2023-04-14 06:09:49.000000 datumaro-1.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/commands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.534255 datumaro-1.2.0rc2/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.538255 datumaro-1.2.0rc2/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.538255 datumaro-1.2.0rc2/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23475 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89324 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.542255 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.546256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.546256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.550256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/synthia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.554256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.558256 datumaro-1.2.0rc2/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41229 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 05:09:33.000000 datumaro-1.2.0rc2/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:09:49.530254 datumaro-1.2.0rc2/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 05:09:49.000000 datumaro-1.2.0rc2/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:09:49.562257 datumaro-1.2.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 05:09:34.000000 datumaro-1.2.0rc2/setup.py
```

### Comparing `datumaro-1.2.0rc1/3rd-party.txt` & `datumaro-1.2.0rc2/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/LICENSE` & `datumaro-1.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/PKG-INFO` & `datumaro-1.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc1
+Version: 1.2.0rc2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc1/README.md` & `datumaro-1.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/__init__.py` & `datumaro-1.2.0rc2/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/capi/pybind.cpp` & `datumaro-1.2.0rc2/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/__main__.py` & `datumaro-1.2.0rc2/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/__init__.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/convert.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/detect_format.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/download.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/explain.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/filter.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/generate.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/merge.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-# Copyright (C) 2020-2022 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
-from collections import OrderedDict
 
 from datumaro.components.dataset import DEFAULT_FORMAT
 from datumaro.components.environment import Environment
-from datumaro.components.errors import DatasetMergeError, DatasetQualityError, ProjectNotFoundError
+from datumaro.components.errors import ProjectNotFoundError
+from datumaro.components.hl_ops import HLOps
 from datumaro.components.merge.intersect_merge import IntersectMerge
 from datumaro.components.project import ProjectBuildTargets
-from datumaro.util import dump_json_file
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter, join_cli_args
 from ..util.errors import CliException
 from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
-        help="Merge few projects",
+        help="Merge few datasets or projects",
         description="""
         Merges multiple datasets into one and produces a new dataset.
-        The command can be useful if you have few annotations and wish
-        to merge them, taking into consideration potential overlaps and
-        conflicts. This command can try to find common ground by voting or
-        return a list of conflicts.|n
+        The command can be useful if you want to merge several datasets
+        which have homogeneous or heterogeneous label categories.
+        We provide three merge policies: 1) "exact" for homogenous datasets;
+        2) "union", or 3) "intersect" for heterogenous datasets. The default merge
+        policy is "union".
+        |n
         |n
         In simple cases, when dataset images do not intersect and new
-        labels are not added, the recommended way of merging is using the
-        "patch" command. It will offer better performance and provide the same
-        results.|n
+        labels are not added, we can use the "exact" merge policy for this situation.
+        |n
+        |n
+        On the other hand, when two datasets have different label categories or
+        have the same (id, subset) pairs in their dataset items. you have to use
+        the "union" or "intersect" merge.
+        |n
+        The "union" merge is more simple way to merge them.
+        It tries to obtain a union set from their label categories and attempts to merge
+        their dataset items. However, if there exist the same (id, subset) pairs, it appends
+        a suffix to each item's id to prevent the same (id, subset) pair in the merged dataset.
+        |n
+        The "intersect" policy is a more complicated way to merge heterogeneous datasets. If you want to merge
+        the annotations in the same (id, subset) pairs which coming from the different datasets
+        each other you wish to merge. You have to taking into consideration potential overlaps
+        and conflicts between the annotations. "intersect" merge policy can try to find common
+        ground by voting or return a list of conflicts.
+        |n
         |n
         This command has multiple forms:|n
         1) %(prog)s <revpath>|n
         2) %(prog)s <revpath> <revpath> ...|n
         |n
         1 - Merges the current project's main target ('project')
         in the working tree with the specified dataset.|n
@@ -60,75 +76,55 @@
         the current project's working tree is used.|n
         |n
         The output format can be specified with the '-f/--format' option.
         Each dataset format has its own export
         options, which are passed after the '--' separator (see examples),
         pass '-- -h' for more info. If not stated otherwise, by default
         only annotations are exported; to include images pass
-        '--save-images' parameter.|n
+        '--save-media' parameter.|n
         |n
         Examples:|n
         - Merge annotations from 3 (or more) annotators:|n
         |s|s%(prog)s project1/ project2/ project3/|n
         |n
+        - Merge datasets with varying merge policies:|n
+        |s|s%(prog)s project1/ project2/ -m <union|intersect|exact>|n
+        |n
         - Check groups of the merged dataset for consistency:|n
         |s|s|slook for groups consising of 'person', 'hand' 'head', 'foot'|n
         |s|s%(prog)s project1/ project2/ -g 'person,hand?,head,foot?'|n
         |n
         - Merge two datasets, specify formats:|n
         |s|s%(prog)s path/to/dataset1:voc path/to/dataset2:coco|n
         |n
         - Merge the current working tree and a dataset:|n
         |s|s%(prog)s path/to/dataset2:coco|n
         |n
         - Merge a source from a previous revision and a dataset:|n
         |s|s%(prog)s HEAD~2:source-2 path/to/dataset2:yolo
         |n
         - Merge datasets and save in different format:|n
-        |s|s%(prog)s -f voc dataset1/:yolo path2/:coco -- --save-images
+        |s|s%(prog)s -f voc dataset1/:yolo path2/:coco -- --save-media
         """,
         formatter_class=MultilineFormatter,
     )
 
     def _group(s):
         return s.split(",")
 
     parser.add_argument(
         "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
     )  # workaround for -- eaten by positionals
     parser.add_argument("targets", nargs="+", help="Target dataset revpaths (repeatable)")
     parser.add_argument(
-        "-iou",
-        "--iou-thresh",
-        default=0.25,
-        type=float,
-        help="IoU match threshold for segments (default: %(default)s)",
-    )
-    parser.add_argument(
-        "-oconf",
-        "--output-conf-thresh",
-        default=0.0,
-        type=float,
-        help="Confidence threshold for output " "annotations (default: %(default)s)",
-    )
-    parser.add_argument(
-        "--quorum",
-        default=0,
-        type=int,
-        help="Minimum count for a label and attribute voting "
-        "results to be counted (default: %(default)s)",
-    )
-    parser.add_argument(
-        "-g",
-        "--groups",
-        action="append",
-        type=_group,
-        help="A comma-separated list of labels in "
-        "annotation groups to check. '?' postfix can be added to a label to "
-        "make it optional in the group (repeatable)",
+        "-m",
+        "--merge-policy",
+        default="union",
+        type=str,
+        help="Policy for how to merge datasets (default: %(default)s)",
     )
     parser.add_argument(
         "-o",
         "--output-dir",
         dest="dst_dir",
         default=None,
         help="Output directory (default: generate a new one)",
@@ -148,14 +144,50 @@
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
         help="Additional arguments for exporter (pass '-- -h' for help). "
         "Must be specified after the main command arguments and after "
         "the '--' separator",
     )
+
+    intersect_args = parser.add_argument_group(
+        title="intersect policy arguments",
+        description="These parameters are optional for the intersect policy only.",
+    )
+    intersect_args.add_argument(
+        "-iou",
+        "--iou-thresh",
+        default=0.25,
+        type=float,
+        help="IoU match threshold for segments (default: %(default)s)",
+    )
+    intersect_args.add_argument(
+        "-oconf",
+        "--output-conf-thresh",
+        default=0.0,
+        type=float,
+        help="Confidence threshold for output " "annotations (default: %(default)s)",
+    )
+    intersect_args.add_argument(
+        "--quorum",
+        default=0,
+        type=int,
+        help="Minimum count for a label and attribute voting "
+        "results to be counted (default: %(default)s)",
+    )
+    intersect_args.add_argument(
+        "-g",
+        "--groups",
+        action="append",
+        type=_group,
+        help="A comma-separated list of labels in "
+        "annotation groups to check. '?' postfix can be added to a label to "
+        "make it optional in the group (repeatable)",
+    )
+
     parser.set_defaults(command=merge_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
@@ -218,52 +250,30 @@
             target_dataset, target_project = parse_full_revpath(t, project)
             if target_project:
                 scope_add(target_project)
             source_datasets.append(target_dataset)
     except Exception as e:
         raise CliException(str(e))
 
-    merger = IntersectMerge(
-        conf=IntersectMerge.Conf(
-            pairwise_dist=args.iou_thresh,
-            groups=args.groups or [],
-            output_conf_thresh=args.output_conf_thresh,
-            quorum=args.quorum,
-        )
+    report_path = osp.join(dst_dir, "merge_report.json")
+    options = (
+        {
+            "conf": IntersectMerge.Conf(
+                pairwise_dist=args.iou_thresh,
+                groups=args.groups or [],
+                output_conf_thresh=args.output_conf_thresh,
+                quorum=args.quorum,
+            )
+        }
+        if args.merge_policy == "intersect"
+        else {}
+    )
+    merged_dataset = HLOps.merge(
+        *source_datasets, merge_policy=args.merge_policy, report_path=report_path, **options
     )
-    merged_dataset = merger.merge(source_datasets)
 
     merged_dataset.export(save_dir=dst_dir, format=exporter, **export_args)
 
-    report_path = osp.join(dst_dir, "merge_report.json")
-    save_merge_report(merger, report_path)
-
     log.info("Merge results have been saved to '%s'" % dst_dir)
     log.info("Report has been saved to '%s'" % report_path)
 
     return 0
-
-
-def save_merge_report(merger, path):
-    item_errors = OrderedDict()
-    source_errors = OrderedDict()
-    all_errors = []
-
-    for e in merger.errors:
-        if isinstance(e, DatasetQualityError):
-            item_errors[str(e.item_id)] = item_errors.get(str(e.item_id), 0) + 1
-        elif isinstance(e, DatasetMergeError):
-            for s in e.sources:
-                source_errors[str(s)] = source_errors.get(s, 0) + 1
-            item_errors[str(e.item_id)] = item_errors.get(str(e.item_id), 0) + 1
-
-        all_errors.append(str(e))
-
-    errors = OrderedDict(
-        [
-            ("Item errors", item_errors),
-            ("Source errors", source_errors),
-            ("All errors", all_errors),
-        ]
-    )
-
-    dump_json_file(path, errors, indent=True)
```

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/patch.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/diff.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/export.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/info.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/stats.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/transform.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/dataset_operations/validate.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/dataset_operations/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/commands/search.py` & `datumaro-1.2.0rc2/datumaro/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/contexts/model.py` & `datumaro-1.2.0rc2/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.2.0rc2/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/contexts/source.py` & `datumaro-1.2.0rc2/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/contexts/util.py` & `datumaro-1.2.0rc2/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/util/__init__.py` & `datumaro-1.2.0rc2/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/util/diff.py` & `datumaro-1.2.0rc2/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/cli/util/project.py` & `datumaro-1.2.0rc2/datumaro/cli/util/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 def split_local_revpath(revpath: str) -> Tuple[Revision, str]:
     """
     Splits the given string into revpath components.
 
     A local revpath is a path to a revision withing the current project.
     The syntax is:
-      - [ <revision> : ] [ <target> ]
+        - [ <revision> : ] [ <target> ]
     At least one part must be present.
 
     Returns: (revision, build target)
     """
 
     sep_pos = revpath.find(":")
     if -1 < sep_pos:
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.2.0rc2/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/algorithms/rise.py` & `datumaro-1.2.0rc2/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/annotation.py` & `datumaro-1.2.0rc2/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/annotations/matcher.py` & `datumaro-1.2.0rc2/datumaro/components/annotations/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 from typing import Optional
 
 import numpy as np
 from attr import attrib, attrs
 
-from datumaro.components.merge.base import Merger
+from datumaro.components.abstracts import IMerger
 from datumaro.util.annotation_util import (
     OKS,
     approximate_line,
     bbox_iou,
     max_bbox,
     mean_bbox,
     segment_iou,
@@ -93,15 +93,15 @@
     b_unmatched = [b_segms[i] for i, m in enumerate(b_matches) if m < 0]
 
     return matches, mispred, a_unmatched, b_unmatched
 
 
 @attrs(kw_only=True)
 class AnnotationMatcher:
-    _context: Optional[Merger] = attrib(default=None)
+    _context: Optional[IMerger] = attrib(default=None)
 
     def match_annotations(self, sources):
         raise NotImplementedError()
 
 
 @attrs
 class LabelMatcher(AnnotationMatcher):
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/annotations/merger.py` & `datumaro-1.2.0rc2/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/cli_plugin.py` & `datumaro-1.2.0rc2/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/config.py` & `datumaro-1.2.0rc2/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/config_model.py` & `datumaro-1.2.0rc2/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/crypter.py` & `datumaro-1.2.0rc2/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/dataset.py` & `datumaro-1.2.0rc2/datumaro/components/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     DEFAULT_SUBSET_NAME,
     CategoriesInfo,
     DatasetBase,
     DatasetInfo,
     DatasetItem,
     IDataset,
 )
+from datumaro.components.dataset_item_storage import (
+    DatasetItemStorage,
+    DatasetItemStorageDatasetView,
+)
 from datumaro.components.environment import DEFAULT_ENVIRONMENT, Environment
 from datumaro.components.errors import (
     CategoriesRedefinedError,
     ConflictingCategoriesError,
     DatasetInfosRedefinedError,
     MediaTypeError,
     MultipleFormatsMatchError,
@@ -48,193 +52,14 @@
 from datumaro.util.log_utils import logging_disabled
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scoped
 
 DEFAULT_FORMAT = "datumaro"
 
 
-class DatasetItemStorage:
-    def __init__(self):
-        self.data = {}  # { subset_name: { id: DatasetItem } }
-        self._traversal_order = {}  # maintain the order of elements
-
-    def __iter__(self) -> Iterator[DatasetItem]:
-        for item in self._traversal_order.values():
-            yield item
-
-    def __len__(self) -> int:
-        return len(self._traversal_order)
-
-    def is_empty(self) -> bool:
-        # Subsets might contain removed items, so this may differ from __len__
-        return all(len(s) == 0 for s in self.data.values())
-
-    def put(self, item: DatasetItem) -> bool:
-        subset = self.data.setdefault(item.subset, {})
-        is_new = subset.get(item.id) is None
-        self._traversal_order[(item.id, item.subset)] = item
-        subset[item.id] = item
-        return is_new
-
-    def get(
-        self, id: Union[str, DatasetItem], subset: Optional[str] = None, dummy: Any = None
-    ) -> Optional[DatasetItem]:
-        if isinstance(id, DatasetItem):
-            id, subset = id.id, id.subset
-        else:
-            id = str(id)
-            subset = subset or DEFAULT_SUBSET_NAME
-
-        return self.data.get(subset, {}).get(id, dummy)
-
-    def remove(self, id: Union[str, DatasetItem], subset: Optional[str] = None) -> bool:
-        if isinstance(id, DatasetItem):
-            id, subset = id.id, id.subset
-        else:
-            id = str(id)
-            subset = subset or DEFAULT_SUBSET_NAME
-
-        subset_data = self.data.setdefault(subset, {})
-        is_removed = subset_data.get(id) is not None
-        subset_data[id] = None
-        if is_removed:
-            # TODO : investigate why "del subset_data[id]" cannot replace "subset_data[id] = None".
-            self._traversal_order.pop((id, subset))
-        return is_removed
-
-    def __contains__(self, x: Union[DatasetItem, Tuple[str, str]]) -> bool:
-        if not isinstance(x, tuple):
-            x = [x]
-        dummy = 0
-        return self.get(*x, dummy=dummy) is not dummy
-
-    def get_subset(self, name):
-        return self.data.get(name, {})
-
-    def subsets(self):
-        return self.data
-
-    def get_annotated_items(self):
-        return sum(bool(s.annotations) for s in self._traversal_order.values())
-
-    def get_datasetitem_by_path(self, path):
-        for s in self._traversal_order.values():
-            if s.media.path == path:
-                return s
-
-    def get_annotations(self):
-        annotations_by_type = {t.name: {"count": 0} for t in AnnotationType}
-        for item in self._traversal_order.values():
-            for ann in item.annotations:
-                annotations_by_type[ann.type.name]["count"] += 1
-        return sum(t["count"] for t in annotations_by_type.values())
-
-    def __copy__(self):
-        copied = DatasetItemStorage()
-        copied._traversal_order = copy(self._traversal_order)
-        copied.data = copy(self.data)
-        return copied
-
-
-class DatasetItemStorageDatasetView(IDataset):
-    class Subset(IDataset):
-        def __init__(self, parent: DatasetItemStorageDatasetView, name: str):
-            super().__init__()
-            self.parent = parent
-            self.name = name
-            self._length = None
-
-        @property
-        def _data(self):
-            return self.parent._get_subset_data(self.name)
-
-        def __iter__(self):
-            for item in self._data.values():
-                if item:
-                    yield item
-
-        def __len__(self):
-            if self._length is not None:
-                return self._length
-
-            self._length = 0
-            for item in self._data.values():
-                if item is not None:
-                    self._length += 1
-            return self._length
-
-        def put(self, item):
-            self._length = None
-            return self._data.put(item)
-
-        def get(self, id, subset=None):
-            assert (subset or DEFAULT_SUBSET_NAME) == (self.name or DEFAULT_SUBSET_NAME)
-            return self._data.get(id, subset)
-
-        def remove(self, id, subset=None):
-            assert (subset or DEFAULT_SUBSET_NAME) == (self.name or DEFAULT_SUBSET_NAME)
-            self._length = None
-            return self._data.remove(id, subset)
-
-        def get_subset(self, name):
-            assert (name or DEFAULT_SUBSET_NAME) == (self.name or DEFAULT_SUBSET_NAME)
-            return self
-
-        def subsets(self):
-            return {self.name or DEFAULT_SUBSET_NAME: self}
-
-        def infos(self):
-            return self.parent.infos()
-
-        def categories(self):
-            return self.parent.categories()
-
-        def media_type(self):
-            return self.parent.media_type()
-
-    def __init__(
-        self,
-        parent: DatasetItemStorage,
-        infos: DatasetInfo,
-        categories: CategoriesInfo,
-        media_type: Optional[Type[MediaElement]],
-    ):
-        self._parent = parent
-        self._infos = infos
-        self._categories = categories
-        self._media_type = media_type
-
-    def __iter__(self):
-        yield from self._parent
-
-    def __len__(self):
-        return len(self._parent)
-
-    def infos(self):
-        return self._infos
-
-    def categories(self):
-        return self._categories
-
-    def get_subset(self, name):
-        return self.Subset(self, name)
-
-    def _get_subset_data(self, name):
-        return self._parent.get_subset(name)
-
-    def subsets(self):
-        return {k: self.get_subset(k) for k in self._parent.subsets()}
-
-    def get(self, id, subset=None):
-        return self._parent.get(id, subset=subset)
-
-    def media_type(self):
-        return self._media_type
-
-
 class ItemStatus(Enum):
     added = auto()
     modified = auto()
     removed = auto()
 
 
 class DatasetPatch:
@@ -902,25 +727,17 @@
             dataset: A new dataset with contents produced by input extractors
         """
 
         if len(sources) == 1:
             source = sources[0]
             dataset = Dataset(source=source, env=env)
         else:
-            from datumaro.components.merge import get_merger
+            from datumaro.components.hl_ops import HLOps
 
-            merger = get_merger(merge_policy)
-
-            categories = merger.merge_categories(s.categories() for s in sources)
-            infos = merger.merge_infos(s.infos() for s in sources)
-            media_type = merger.merge_media_types(sources)
-            source = merger.merge(*sources)
-            dataset = Dataset(
-                source=source, infos=infos, categories=categories, media_type=media_type, env=env
-            )
+            return HLOps.merge(*sources, merge_policy=merge_policy)
 
         return dataset
 
     def __init__(
         self,
         source: Optional[IDataset] = None,
         *,
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/dataset_base.py` & `datumaro-1.2.0rc2/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/environment.py` & `datumaro-1.2.0rc2/datumaro/components/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 
 import glob
 import importlib
 import logging as log
 import os.path as osp
 from functools import partial
 from inspect import isclass
-from typing import Callable, Dict, Generic, Iterable, Iterator, List, Optional, Set, Type, TypeVar
+from typing import (
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Type,
+    TypeVar,
+)
 
 from datumaro.components.cli_plugin import CliPlugin, plugin_types
 from datumaro.components.format_detection import (
     DetectedFormat,
     FormatDetectionConfidence,
     RejectionReason,
     detect_dataset_format,
@@ -210,20 +222,20 @@
 
     def load_plugins(self, plugins_dir):
         module_names = self._find_plugins(plugins_dir)
         plugins = self._load_plugins(
             module_names, importer=partial(import_foreign_module, path=plugins_dir)
         )
 
-        self._register_plugins(plugins)
+        self.register_plugins(plugins)
 
     def _register_builtin_plugins(self):
-        self._register_plugins(self._load_builtin_plugins())
+        self.register_plugins(self._load_builtin_plugins())
 
-    def _register_plugins(self, plugins):
+    def register_plugins(self, plugins):
         self.extractors.batch_register(plugins)
         self.importers.batch_register(plugins)
         self.launchers.batch_register(plugins)
         self.exporters.batch_register(plugins)
         self.generators.batch_register(plugins)
         self.transforms.batch_register(plugins)
         self.validators.batch_register(plugins)
@@ -283,9 +295,30 @@
         )
 
         return [str(format) for format in all_matched_formats if format.confidence == max_conf]
 
     def __reduce__(self):
         return (self.__class__, ())
 
+    @classmethod
+    def merge(cls, envs: Sequence["Environment"]) -> "Environment":
+        if all([env == DEFAULT_ENVIRONMENT for env in envs]):
+            return DEFAULT_ENVIRONMENT
+
+        merged = Environment()
+
+        def _register(registry: PluginRegistry):
+            merged.register_plugins(plugin for plugin in registry)
+
+        for env in envs:
+            _register(env.extractors)
+            _register(env.importers)
+            _register(env.launchers)
+            _register(env.exporters)
+            _register(env.generators)
+            _register(env.transforms)
+            _register(env.validators)
+
+        return merged
+
 
 DEFAULT_ENVIRONMENT = Environment()
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/errors.py` & `datumaro-1.2.0rc2/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/exporter.py` & `datumaro-1.2.0rc2/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/extractor_tfds.py` & `datumaro-1.2.0rc2/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/filter.py` & `datumaro-1.2.0rc2/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/format_detection.py` & `datumaro-1.2.0rc2/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/generator.py` & `datumaro-1.2.0rc2/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/hl_ops/__init__.py` & `datumaro-1.2.0rc2/datumaro/components/hl_ops/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from datumaro.components.dataset import Dataset, DatasetItemStorageDatasetView, IDataset
 from datumaro.components.environment import Environment
 from datumaro.components.errors import DatasetError
 from datumaro.components.exporter import Exporter
 from datumaro.components.filter import XPathAnnotationsFilter, XPathDatasetFilter
 from datumaro.components.launcher import Launcher, ModelTransform
-from datumaro.components.merge.exact_merge import ExactMerge
+from datumaro.components.merge import DEFAULT_MERGE_POLICY, get_merger
 from datumaro.components.transformer import Transform
 from datumaro.components.validator import TaskType, Validator
 from datumaro.util import parse_str_enum_value
 from datumaro.util.scope import on_error_do, scoped
 
 __all__ = ["HLOps"]
 
@@ -94,37 +94,40 @@
             )
         else:
             if not expr:
                 return dataset
             return HLOps.transform(dataset, XPathDatasetFilter, xpath=expr)
 
     @staticmethod
-    def merge(*datasets: IDataset) -> IDataset:
-        """
-        Merges several datasets using the "simple" (exact matching) algorithm:
-
-            - items are matched by (id, subset) pairs
-            - matching items share the fields available
-
-                - nothing + nothing = nothing,
-                - nothing + something = something
-                - something A + something B = conflict
-            - annotations are matched by value and shared
-            - in case of conflicts, throws an error
-
-        Returns: a wrapper around the input datasets
+    def merge(
+        *datasets: Dataset,
+        merge_policy: str = DEFAULT_MERGE_POLICY,
+        report_path: Optional[str] = None,
+        **kwargs,
+    ) -> Dataset:
         """
-
-        merger = ExactMerge()
-        infos = merger.merge_infos(d.infos() for d in datasets)
-        categories = merger.merge_categories(d.categories() for d in datasets)
-        media_type = merger.merge_media_types(datasets)
-        return DatasetItemStorageDatasetView(
-            merger.merge(*datasets), infos=infos, categories=categories, media_type=media_type
+        Merge `datasets` according to `merge_policy`. You have to choose an appropriate `merge_policy`
+        for your purpose. The available merge policies are "union", "intersect", and "exact".
+        For more details about the merge policies, please refer to :func:`get_merger`.
+        """
+
+        merger = get_merger(merge_policy, **kwargs)
+        merged = merger(*datasets)
+        env = Environment.merge(
+            dataset.env
+            for dataset in datasets
+            if hasattr(
+                dataset, "env"
+            )  # TODO: Sometimes, there is dataset which is not exactly "Dataset",
+            # e.g., VocClassificationBase. this should be fixed and every object from
+            # Dataset.import_from should have "Dataset" type.
         )
+        if report_path:
+            merger.save_merge_report(report_path)
+        return Dataset(source=merged, env=env)
 
     @staticmethod
     def run_model(
         dataset: IDataset,
         model: Union[Launcher, Type[ModelTransform]],
         *,
         batch_size: int = 1,
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/importer.py` & `datumaro-1.2.0rc2/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/launcher.py` & `datumaro-1.2.0rc2/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/media.py` & `datumaro-1.2.0rc2/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/media_manager.py` & `datumaro-1.2.0rc2/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/merge/exact_merge.py` & `datumaro-1.2.0rc2/datumaro/components/merge/exact_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from typing import Any, Dict, Iterable, List, Tuple, Union
-
-from attr import attrs
+from typing import Any, Dict, Iterable, List, Sequence, Tuple, Union
 
 from datumaro.components.annotation import Annotation
-from datumaro.components.dataset import DatasetItemStorage
 from datumaro.components.dataset_base import DatasetItem, IDataset
+from datumaro.components.dataset_item_storage import DatasetItemStorage
 from datumaro.components.errors import (
     DatasetMergeError,
     MismatchingAttributesError,
     MismatchingImageInfoError,
     MismatchingMediaError,
     MismatchingMediaPathError,
     VideoMergeError,
 )
 from datumaro.components.media import Image, MediaElement, MultiframeImage, PointCloud, Video
 from datumaro.components.merge import Merger
 
 __all__ = ["ExactMerge"]
 
 
-@attrs
 class ExactMerge(Merger):
     """
     Merges several datasets using the "simple" algorithm:
+        - All datasets should have the same categories
         - items are matched by (id, subset) pairs
         - matching items share the media info available:
-
             - nothing + nothing = nothing
             - nothing + something = something
             - something A + something B = conflict
         - annotations are matched by value and shared
         - in case of conflicts, throws an error
     """
 
     def __init__(self, **options):
         super().__init__(**options)
 
-    def merge(self, *sources: IDataset) -> DatasetItemStorage:
+    def merge(self, sources: Sequence[IDataset]) -> DatasetItemStorage:
         items = DatasetItemStorage()
         for source_idx, source in enumerate(sources):
             for item in source:
                 existing_item = items.get(item.id, item.subset)
                 if existing_item is not None:
                     try:
                         item = self._merge_items(existing_item, item)
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/merge/intersect_merge.py` & `datumaro-1.2.0rc2/datumaro/components/merge/intersect_merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 from collections import OrderedDict
+from typing import Dict, Sequence
 
 import attr
 from attr import attrib, attrs
 
 from datumaro.components.annotation import (
     AnnotationType,
     LabelCategories,
@@ -24,15 +25,19 @@
     ImageAnnotationMerger,
     LabelMerger,
     LineMerger,
     MaskMerger,
     PointsMerger,
     PolygonMerger,
 )
-from datumaro.components.dataset import Dataset
+from datumaro.components.dataset_base import DatasetItem, IDataset
+from datumaro.components.dataset_item_storage import (
+    DatasetItemStorage,
+    DatasetItemStorageDatasetView,
+)
 from datumaro.components.errors import (
     AnnotationsTooCloseError,
     ConflictingCategoriesError,
     FailedAttrVotingError,
     NoMatchingAnnError,
     NoMatchingItemError,
     WrongGroupError,
@@ -43,19 +48,76 @@
 from datumaro.util.attrs_util import ensure_cls
 
 __all__ = ["IntersectMerge"]
 
 
 @attrs
 class IntersectMerge(Merger):
+    """
+    Merge several datasets with "intersect" policy:
+
+    - If there are two or more dataset items whose (id, subset) pairs match each other,
+    we can consider this as having an intersection in our dataset. This method merges
+    the annotations of the corresponding :class:`DatasetItem` into one :class:`DatasetItem`
+    to handle this intersection. The rule to handle merging annotations is provided by
+    :class:`AnnotationMerger` according to their annotation types. For example,
+    DatasetItem(id="item_1", subset="train", annotations=[Bbox(0, 0, 1, 1)]) from Dataset-A and
+    DatasetItem(id="item_1", subset="train", annotations=[Bbox(.5, .5, 1, 1)]) from Dataset-B can be
+    merged into DatasetItem(id="item_1", subset="train", annotations=[Bbox(0, 0, 1, 1)]).
+
+    - Label categories are merged according to the union of their label names
+    (Same as `UnionMerge`). For example, if Dataset-A has {"car", "cat", "dog"}
+    and Dataset-B has {"car", "bus", "truck"} labels, the merged dataset will have
+    {"bust", "car", "cat", "dog", "truck"} labels.
+
+    - This merge has configuration parameters (`conf`) to control the annotation merge behaviors.
+
+    For example,
+
+    ```python
+    merge = IntersectMerge(
+        conf=IntersectMerge.Conf(
+            pairwise_dist=0.25,
+            groups=[],
+            output_conf_thresh=0.0,
+            quorum=0,
+        )
+    )
+    ```
+
+    For more details for the parameters, please refer to :class:`IntersectMerge.Conf`.
+    """
+
     def __init__(self, **options):
         super().__init__(**options)
 
     @attrs(repr_ns="IntersectMerge", kw_only=True)
     class Conf:
+        """
+        Parameters
+        ----------
+        pairwise_dist
+            IoU match threshold for segments
+        sigma
+            Parameter for Object Keypoint Similarity metric
+            (https://cocodataset.org/#keypoints-eval)
+        output_conf_thresh
+            Confidence threshold for output annotations
+        quorum
+            Minimum count for a label and attribute voting results to be counted
+        ignored_attributes
+            Attributes to be ignored in the merged :class:`DatasetItem`
+        groups
+            A comma-separated list of labels in annotation groups to check.
+            '?' postfix can be added to a label to make it optional in the group (repeatable)
+        close_distance
+            Distance threshold between annotations to decide their closeness. If they are decided
+            to be close, it will be enrolled to the error tracker.
+        """
+
         pairwise_dist = attrib(converter=float, default=0.5)
         sigma = attrib(converter=list, factory=list)
 
         output_conf_thresh = attrib(converter=float, default=0)
         quorum = attrib(converter=int, default=0)
         ignored_attributes = attrib(converter=set, factory=set)
 
@@ -88,44 +150,55 @@
     _item_id = attrib(init=False)
     _item = attrib(init=False)
 
     # Misc.
     _infos = attrib(init=False)  # merged infos
     _categories = attrib(init=False)  # merged categories
 
-    def merge(self, datasets):
-        self._infos = self.merge_infos([d.infos() for d in datasets])
-        self._categories = self.merge_categories([d.categories() for d in datasets])
-        merged = Dataset(
-            infos=self._infos,
-            categories=self._categories,
-            media_type=self.merge_media_types(datasets),
-        )
-
+    def merge(self, sources: Sequence[IDataset]) -> DatasetItemStorage:
+        self._infos = self.merge_infos([d.infos() for d in sources])
+        self._categories = self.merge_categories([d.categories() for d in sources])
+        merged = DatasetItemStorage()
         self._check_groups_definition()
 
-        item_matches, item_map = self.match_items(datasets)
+        item_matches, item_map = self.match_items(sources)
         self._item_map = item_map
-        self._dataset_map = {id(d): (d, i) for i, d in enumerate(datasets)}
+        self._dataset_map = {id(d): (d, i) for i, d in enumerate(sources)}
 
         for item_id, items in item_matches.items():
             self._item_id = item_id
 
-            if len(items) < len(datasets):
-                missing_sources = set(id(s) for s in datasets) - set(items)
+            if len(items) < len(sources):
+                missing_sources = set(id(s) for s in sources) - set(items)
                 missing_sources = [self._dataset_map[s][1] for s in missing_sources]
                 self.add_item_error(NoMatchingItemError, sources=missing_sources)
             merged.put(self.merge_items(items))
 
         return merged
 
     def get_ann_source(self, ann_id):
         return self._item_map[self._ann_map[ann_id][1]][1]
 
-    def merge_categories(self, sources):
+    def __call__(self, *datasets: IDataset) -> DatasetItemStorageDatasetView:
+        # TODO: self.merge() should be the first since this order matters for
+        # IntersectMerge.
+        merged = self.merge(datasets)
+        infos = self.merge_infos(d.infos() for d in datasets)
+        categories = self.merge_categories(d.categories() for d in datasets)
+        media_type = self.merge_media_types(datasets)
+        return DatasetItemStorageDatasetView(
+            parent=merged, infos=infos, categories=categories, media_type=media_type
+        )
+
+    def merge_categories(self, sources: Sequence[IDataset]) -> Dict:
+        # TODO: This is a temporary workaround to minimize code changes.
+        # We have to revisit it to make this class stateless.
+        if hasattr(self, "_categories"):
+            return self._categories
+
         dst_categories = {}
 
         label_cat = self._merge_label_categories(sources)
         if label_cat is None:
             label_cat = LabelCategories()
         dst_categories[AnnotationType.label] = label_cat
 
@@ -135,15 +208,15 @@
 
         mask_cat = self._merge_mask_categories(sources, label_cat)
         if mask_cat is not None:
             dst_categories[AnnotationType.mask] = mask_cat
 
         return dst_categories
 
-    def merge_items(self, items):
+    def merge_items(self, items: Dict[int, DatasetItem]) -> DatasetItem:
         self._item = next(iter(items.values()))
 
         self._ann_map = {}
         sources = []
         for item in items.values():
             self._ann_map.update({id(a): (a, id(item)) for a in item.annotations})
             sources.append(item.annotations)
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/merge/union_merge.py` & `datumaro-1.2.0rc2/datumaro/components/merge/union_merge.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+from collections import defaultdict
+from typing import Dict, List, Sequence, Tuple
+
 from datumaro.components.annotation import AnnotationType, LabelCategories
-from datumaro.components.dataset import DatasetItemStorage
-from datumaro.components.dataset_base import IDataset
+from datumaro.components.dataset_base import DatasetItem, IDataset
+from datumaro.components.dataset_item_storage import DatasetItemStorage
 from datumaro.components.merge import Merger
 
 __all__ = ["UnionMerge"]
 
 
 class UnionMerge(Merger):
     """
-    Merges several datasets using the "simple" algorithm:
-        - items are matched by (id, subset) pairs
-        - matching items share the media info available:
-            - nothing + nothing = nothing
-            - nothing + something = something
-            - something A + something B = something (A + B)
-        - annotations are matched by value and shared
-        - in case of conflicts, throws an error
+    Merge several datasets with "union" policy:
+
+    - Label categories are merged according to the union of their label names.
+    For example, if Dataset-A has {"car", "cat", "dog"} and Dataset-B has
+    {"car", "bus", "truck"} labels, the merged dataset will have
+    {"bust", "car", "cat", "dog", "truck"} labels.
+
+    - If there are two or more dataset items whose (id, subset) pairs match each other,
+    both are included in the merged dataset. At this time, since the same (id, subset)
+    pair cannot be duplicated in the dataset, we add a suffix to the id of each source item.
+    For example, if Dataset-A has DatasetItem(id="magic", subset="train") and Dataset-B has
+    also DatasetItem(id="magic", subset="train"), the merged dataset will have
+    DatasetItem(id="magic-0", subset="train") and DatasetItem(id="magic-1", subset="train").
     """
 
     def __init__(self, **options):
         super().__init__(**options)
         self._matching_table = {}
 
-    def merge(self, *sources: IDataset) -> DatasetItemStorage:
-        items = DatasetItemStorage()
+    def merge(self, sources: Sequence[IDataset]) -> DatasetItemStorage:
+        dict_items: Dict[Tuple[str, str], List[DatasetItem]] = defaultdict(list)
+
         for source_idx, source in enumerate(sources):
             for item in source:
                 if self._matching_table.get(source_idx, None):
                     for ann in item.annotations:
                         ann.label = self._matching_table[source_idx][ann.label]
-                items.put(item)
-        return items
+                dict_items[item.id, item.subset].append(item)
+
+        item_storage = DatasetItemStorage()
+
+        for items in dict_items.values():
+            if len(items) == 1:
+                item_storage.put(items[0])
+            else:
+                for idx, item in enumerate(items):
+                    # Add prefix
+                    item_storage.put(item.wrap(id=f"{item.id}-{idx}"))
+
+        return item_storage
 
-    def merge_categories(self, sources):
+    def merge_categories(self, sources: Sequence[IDataset]) -> Dict:
         dst_categories = {}
 
         label_cat = self._merge_label_categories(sources)
         if label_cat is None:
             label_cat = LabelCategories()
         dst_categories[AnnotationType.label] = label_cat
 
         return dst_categories
 
-    def _merge_label_categories(self, sources):
+    def _merge_label_categories(self, sources: Sequence[IDataset]) -> LabelCategories:
         dst_cat = LabelCategories()
         dst_indices = {}
         dst_labels = []
 
         for src_id, src_categories in enumerate(sources):
             src_cat = src_categories.get(AnnotationType.label)
             if src_cat is None:
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/operations.py` & `datumaro-1.2.0rc2/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/progress_reporting.py` & `datumaro-1.2.0rc2/datumaro/components/progress_reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self._total = total
         self._desc = desc
 
     def report_status(self, progress: int):
         status = str(self._desc) if self._desc else ""
         status += (
             f" {progress:0{len(str(self._total))}d}/{self._total}"
-            f" ({progress/self._total*100: 6.2f}%)"
+            f" ({progress/self._total*100:6.2f}%)"
         )
         print(status)
 
     def finish(self):
         self.report_status(self._total)
 
     def split(self, count: int):
```

### Comparing `datumaro-1.2.0rc1/datumaro/components/project.py` & `datumaro-1.2.0rc2/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/searcher.py` & `datumaro-1.2.0rc2/datumaro/components/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/shift_analyzer.py` & `datumaro-1.2.0rc2/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/transformer.py` & `datumaro-1.2.0rc2/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/validator.py` & `datumaro-1.2.0rc2/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/components/visualizer.py` & `datumaro-1.2.0rc2/datumaro/components/visualizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import math
+import random
 import warnings
 from collections import defaultdict
-from typing import Iterable, List, Optional, Tuple, Union
+from typing import Iterable, List, Optional, Tuple, Union, overload
 
 import cv2
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
@@ -118,14 +119,16 @@
         self.color_cycles = color_cycles if color_cycles is not None else DEFAULT_COLOR_CYCLES
         self.bbox_linewidth = bbox_linewidth
         self.text_y_offset = text_y_offset
 
         assert 0.0 <= alpha <= 1.0, "alpha should be in [0, 1]."
         self.alpha = alpha
 
+        self._items = [item for item in self.dataset]
+
     @property
     def draw_only_image(self):
         """
         If self.alpha = 0, we do not overdraw any annotation over the image.
         """
         return self.alpha == 0.0
 
@@ -188,58 +191,204 @@
     def _sort_by_z_order(self, annotations: List[Annotation]) -> List[Annotation]:
         def _sort_key(ann: Annotation):
             z_order = getattr(ann, "z_order", -1)
             return z_order
 
         return sorted(annotations, key=_sort_key)
 
+    def get_random_items(self, n_samples: int) -> List[DatasetItem]:
+        """Get random samples from the dataset"""
+        if n_samples >= len(self.dataset):
+            raise ValueError(
+                f"n_samples={n_samples} should be less than the dataset size ({len(self.dataset)})."
+            )
+
+        return random.choices(self._items, k=n_samples)
+
+    @overload
+    def vis_gallery(
+        self,
+        ids: List[str],
+        subsets: Union[str, List[str]] = None,
+        grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
+    ):
+        """Visualize several :class:`DatasetItem` as a gallery
+
+        Parameters
+        ----------
+        ids
+            A list of :class:`DatasetItem`'s ID to visualize
+        subsets
+            A list of :class:`DatasetItem`'s subset name to visualize.
+            If a string is given, it is automatically expanded into
+            a list up to the length of `ids`.
+        grid_size
+            Grid size of the gallery plot. If `None`, we automatically infer its size.
+
+        Return
+        ------
+            :class:`Figure` include visualization plots.
+        """
+        ...
+
+    @overload
     def vis_gallery(
         self,
-        ids: List[Union[str, DatasetItem]],
-        subset: Optional[Union[str, List[str]]] = None,
+        items: List[DatasetItem],
+        grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
+    ):
+        """Visualize several :class:`DatasetItem` as a gallery
+
+        Parameters
+        ----------
+        items
+            A list of :class:`DatasetItem` to visualize
+
+        Return
+        ------
+            :class:`Figure` include visualization plots.
+        """
+        ...
+
+    def vis_gallery(
+        self,
+        *inputs,
         grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
     ) -> Figure:
+        """Visualize several :class:`DatasetItem` as a gallery"""
+        if len(inputs) == 1:
+            ids, subsets = None, None
+            (items,) = inputs
+
+        elif len(inputs) == 2:
+            ids, subsets = inputs
+            items = None
+            if isinstance(subsets, str):
+                subsets = [subsets] * len(ids)  # expand it to have len(ids)
+
+        def _parse_inputs(
+            ids: Optional[List[str]],
+            subsets: Optional[List[str]],
+            items: Optional[List[DatasetItem]],
+        ) -> Tuple[List[str], List[str]]:
+            if ids is not None and subsets is not None:
+                return ids, subsets
+            elif items is not None:
+                return [item.id for item in items], [item.subset for item in items]
+            raise ValueError(
+                f"ids={ids}, subsets={subsets}, and items={items} is an invalid input."
+            )
+
+        ids, subsets = _parse_inputs(ids, subsets, items)
+
         nrows, ncols = _infer_grid_size(len(ids), grid_size)
         fig, axs = plt.subplots(nrows, ncols, figsize=self.figsize)
 
-        if isinstance(subset, list):
-            assert len(ids) == len(
-                subset
-            ), "If subset is a list, it should have the same length as ids."
-
-        for i, (dataset_id, ax) in enumerate(zip(ids, axs.flatten())):
-            if isinstance(subset, List):
-                self.vis_one_sample(dataset_id, subset[i], ax)
-            else:
-                self.vis_one_sample(dataset_id, subset, ax)
+        assert len(ids) == len(
+            subsets
+        ), "If subset is a list, it should have the same length as ids."
+
+        for item_id, subset, ax in zip(ids, subsets, axs.flatten()):
+            self.vis_one_sample(item_id, subset, ax=ax)
 
         return fig
 
+    @overload
     def vis_one_sample(
-        self, id: Union[str, DatasetItem], subset: Optional[str] = None, ax: Optional[Axes] = None
+        self,
+        item_id: str = None,
+        subset: str = None,
+        ax: Optional[Axes] = None,
     ) -> Figure:
+        """Visualize one :class:`DatasetItem`
+
+        Parameters
+        ----------
+        item_id
+            ID of :class:`DatasetItem` to visualize
+        subset
+            Subset name of :class:`DatasetItem` to visualize
+        ax
+            If not `None`, draw on `ax` instead of creating a new one
+
+        Return
+        ------
+            :class:`Figure` include visualization plot of the :class:`DatasetItem`.
+        """
+        ...
+
+    @overload
+    def vis_one_sample(
+        self,
+        item: DatasetItem = None,
+        ax: Optional[Axes] = None,
+    ) -> Figure:
+        """Visualize one :class:`DatasetItem`
+
+        Parameters
+        ----------
+        item
+            :class:`DatasetItem` to visualize
+        ax
+            If not `None`, draw on `ax` instead of creating a new one
+
+        Return
+        ------
+            :class:`Figure` include visualization plot of the :class:`DatasetItem`.
+        """
+        ...
+
+    def vis_one_sample(
+        self,
+        *inputs,
+        ax: Optional[Axes] = None,
+    ) -> Figure:
+        """Visualize one dataset item"""
+        if len(inputs) == 1:
+            item_id, subset = None, None
+            (item,) = inputs
+
+        elif len(inputs) == 2:
+            item_id, subset = inputs
+            item = None
+
         if ax is None:
             fig = plt.figure(figsize=self.figsize)
             ax = plt.gca()
         else:
             fig = ax.get_figure()
             plt.sca(ax)
 
-        item: DatasetItem = self.dataset.get(id, subset)
-        assert item is not None, f"Cannot find id={id}, subset={subset}"
+        def _parse_inputs(
+            item_id: Optional[str], subset: Optional[str], item: Optional[DatasetItem]
+        ) -> Tuple[str, str]:
+            if item_id is not None and subset is not None:
+                return item_id, subset
+            elif item is not None:
+                item_id = item.id
+                subset = item.subset
+                return item_id, subset
+            raise ValueError(
+                f"item_id={item_id}, subset={subset}, and item={item} is an invalid input."
+            )
+
+        item_id, subset = _parse_inputs(item_id, subset, item)
+        item: DatasetItem = self.dataset.get(item_id, subset)
+
+        assert item is not None, f"Cannot find id={item_id}, subset={subset}"
         assert (
             item is not Image
         ), f"Media type should be Image, Current media type={type(item.media)}"
 
         img = item.media.data.astype(np.uint8)
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         ax.imshow(img)
 
         width = ax.transAxes.transform_point((1, 0))[0] - ax.transAxes.transform_point((0, 0))[0]
-        text = ax.set_title(f"ID: {id}, Subset: {subset}", loc="center", wrap=True)
+        text = ax.set_title(f"ID: {item_id}, Subset: {subset}", loc="center", wrap=True)
         text.__get_wrapped_text = text._get_wrapped_text
 
         def _get_wrapped_text():
             wrapped_text = text.__get_wrapped_text()
             text._text = wrapped_text
             return wrapped_text
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.2.0rc2/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,17 @@
     @overload
     def __getitem__(self, key: Union[range, slice]) -> List[Dict]:
         ...
 
     def __getitem__(
         self, key: Union[int, range, slice, str]
     ) -> Union[Dict, List[Dict], "ArrowDataset"]:
-        # TODO: add unit test
         if isinstance(key, str):
+            if key not in self.column_names:
+                raise KeyError(key)
             dataset = ArrowDataset(self._files, self._keep_in_memory)
             dataset._update_table(
                 self.table.drop([name for name in self.column_names if name != key])
             )
             return dataset
         elif isinstance(key, slice):
             key = range(*key.indices(len(self)))
@@ -187,15 +188,15 @@
                 for key_ in key
             ]
         if isinstance(key, int):
             if key < 0:
                 key += len(self)
             return self.slice(key, 1)[0]
 
-        raise KeyError()
+        raise KeyError(key)
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}("
             f"num_rows={len(self)}, "
             f"columns={self.column_names}, "
             f"keep_in_memory={self._keep_in_memory}"
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,16 +340,24 @@
 
     @classmethod
     def patch(cls, dataset, patch, save_dir, **kwargs):
         # no patch supported
         with tempfile.TemporaryDirectory() as temp_dir:
             cls.convert(dataset, save_dir=temp_dir, **kwargs)
             if os.path.exists(save_dir):
-                rmtree(save_dir)
-            move(temp_dir, save_dir)
+                for file in os.listdir(save_dir):
+                    file = os.path.join(save_dir, file)
+                    if os.path.isdir(file):
+                        rmtree(file)
+                    else:
+                        os.remove(file)
+            for file in os.listdir(temp_dir):
+                file_from = os.path.join(temp_dir, file)
+                file_to = os.path.join(save_dir, file)
+                move(file_from, file_to)
 
     def __init__(
         self,
         extractor: IDataset,
         save_dir: str,
         *,
         save_images=None,  # Deprecated
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,23 +161,23 @@
         return [{"url": path, "format": "common_semantic_segmentation"}]
 
 
 @with_subset_dirs
 class CommonSemanticSegmentationWithSubsetDirsImporter(CommonSemanticSegmentationImporter):
     """It supports the following subset sub-directory structure for CommonSemanticSegmentation.
 
-    ```
-    Dataset/
-    └─ <split: train,val, ...>
-        ├── dataset_meta.json # a list of labels
-        ├── images/
-        │   ├── <img1>.png
-        │   ├── <img2>.png
-        │   └── ...
-        └── masks/
-            ├── <img1>.png
-            ├── <img2>.png
-            └── ...
+    .. code-block::
+
+        Dataset/
+        └─ <split: train,val, ...>
+            ├── dataset_meta.json # a list of labels
+            ├── images/
+            │   ├── <img1>.png
+            │   ├── <img2>.png
+            │   └── ...
+            └── masks/
+                ├── <img1>.png
+                ├── <img2>.png
+                └── ...
 
     Then, the imported dataset will have train, val, ... CommonSemanticSegmentation subsets.
-    ```
     """
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # ruff: noqa: F405
 
 from .annotation import *
-from .common import *
+from .common import DictMapper, FloatListMapper, IntListMapper, Mapper, StringMapper
 from .dataset_item import *
 from .media import *
 
 __all__ = [
     # anns
     "AnnotationListMapper",
     "LabelMapper",
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,23 @@
         return items
 
 
 class ImagenetImporter(Importer):
     """TorchVision's ImageFolder style importer.
     For example, it imports the following directory structure.
 
-    root
-    ├── label_0
-    │   ├── label_0_1.jpg
-    │   └── label_0_2.jpg
-    └── label_1
-        └── label_1_1.jpg
+    .. code-block:: text
+
+        root
+        ├── label_0
+        │   ├── label_0_1.jpg
+        │   └── label_0_2.jpg
+        └── label_1
+            └── label_1_1.jpg
+
     """
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
         # Images must not be under a directory whose name is blacklisted.
         for dname in os.listdir(context.root_path):
             dpath = osp.join(context.root_path, dname)
@@ -102,33 +105,35 @@
 
 
 @with_subset_dirs
 class ImagenetWithSubsetDirsImporter(ImagenetImporter):
     """TorchVision ImageFolder style importer.
     For example, it imports the following directory structure.
 
-    root
-    ├── train
-    │   ├── label_0
-    │   │   ├── label_0_1.jpg
-    │   │   └── label_0_2.jpg
-    │   └── label_1
-    │       └── label_1_1.jpg
-    ├── val
-    │   ├── label_0
-    │   │   ├── label_0_1.jpg
-    │   │   └── label_0_2.jpg
-    │   └── label_1
-    │       └── label_1_1.jpg
-    └── test
-        ├── label_0
-        │   ├── label_0_1.jpg
-        │   └── label_0_2.jpg
-        └── label_1
-            └── label_1_1.jpg
+    .. code-block::
+
+        root
+        ├── train
+        │   ├── label_0
+        │   │   ├── label_0_1.jpg
+        │   │   └── label_0_2.jpg
+        │   └── label_1
+        │       └── label_1_1.jpg
+        ├── val
+        │   ├── label_0
+        │   │   ├── label_0_1.jpg
+        │   │   └── label_0_2.jpg
+        │   └── label_1
+        │       └── label_1_1.jpg
+        └── test
+            ├── label_0
+            │   ├── label_0_1.jpg
+            │   └── label_0_2.jpg
+            └── label_1
+                └── label_1_1.jpg
 
     Then, it will have three subsets: train, val, and test and they have label_0 and label_1 labels.
     """
 
 
 class ImagenetExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mars.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mot.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mots.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/synthia.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/synthia.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/video.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.2.0rc2/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/ndr.py` & `datumaro-1.2.0rc2/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.2.0rc2/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.2.0rc2/datumaro/plugins/sampler/random_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import DatasetItem, IDataset
 from datumaro.components.transformer import Transform
 from datumaro.util import cast
 
 
 class RandomSampler(Transform, CliPlugin):
-    """
+    r"""
     Sampler that keeps no more than required number of items in the dataset.|n
     |n
     Notes:|n
     |s|s- Items are selected uniformly|n
     |s|s- Requesting a sample larger than the number of all images will|n
     |s|s|s|sreturn all images|n
     |n
```

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.2.0rc2/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/searcher.py` & `datumaro-1.2.0rc2/datumaro/plugins/searcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/shift_analyzer.py` & `datumaro-1.2.0rc2/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/splitter.py` & `datumaro-1.2.0rc2/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.2.0rc2/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.2.0rc2/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/tiling/tile.py` & `datumaro-1.2.0rc2/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/tiling/util.py` & `datumaro-1.2.0rc2/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/transforms.py` & `datumaro-1.2.0rc2/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/plugins/validators.py` & `datumaro-1.2.0rc2/datumaro/plugins/validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -192,18 +192,19 @@
             },
             "attribute_distribution": {"defined_attributes": {}, "undefined_attributes": {}},
         }
         stats["total_ann_count"] = 0
         stats["items_missing_annotation"] = []
 
         label_dist = stats["label_distribution"]
-        attr_dist = stats["attribute_distribution"]
         defined_label_dist = label_dist["defined_labels"]
-        defined_attr_dist = attr_dist["defined_attributes"]
         undefined_label_dist = label_dist["undefined_labels"]
+
+        attr_dist = stats["attribute_distribution"]
+        defined_attr_dist = attr_dist["defined_attributes"]
         undefined_attr_dist = attr_dist["undefined_attributes"]
 
         label_categories = dataset.categories().get(AnnotationType.label, LabelCategories())
         base_valid_attrs = label_categories.attributes
 
         for category in label_categories:
             defined_label_dist[category.name] = 0
@@ -262,55 +263,68 @@
                         attr_dets = defined_attr_stats[attr]
 
                     attr_dets["distribution"].setdefault(str(value), 0)
                     attr_dets["distribution"][str(value)] += 1
 
         return stats, filtered_anns
 
-    @staticmethod
-    def _update_prop_distributions(curr_prop_stats, target_stats):
-        for prop, val in curr_prop_stats.items():
-            prop_stats = target_stats[prop]
-            prop_dist = prop_stats["distribution"]
-            prop_stats["distribution"] = np.append(prop_dist, val)
+    def _generate_common_reports(self, stats):
+        """
+        Validates the dataset for classification tasks based on its statistics.
 
-    @staticmethod
-    def _compute_prop_stats_from_dist(dist_by_label, dist_by_attr):
-        for label_name, stats in dist_by_label.items():
-            prop_stats_list = list(stats.values())
-            attr_label = dist_by_attr.get(label_name, {})
-            for vals in attr_label.values():
-                for val_stats in vals.values():
-                    prop_stats_list += list(val_stats.values())
+        Parameters
+        ----------
+        dataset : IDataset object
+        stats: Dict object
 
-            for prop_stats in prop_stats_list:
-                prop_dist = prop_stats.pop("distribution", [])
-                if len(prop_dist) > 0:
-                    prop_stats["mean"] = np.mean(prop_dist)
-                    prop_stats["stdev"] = np.std(prop_dist)
-                    prop_stats["min"] = np.min(prop_dist)
-                    prop_stats["max"] = np.max(prop_dist)
-                    prop_stats["median"] = np.median(prop_dist)
+        Returns
+        -------
+        reports (list): List of validation reports (DatasetValidationError).
+        """
 
-                    counts, bins = np.histogram(prop_dist)
-                    prop_stats["histogram"]["bins"] = bins.tolist()
-                    prop_stats["histogram"]["counts"] = counts.tolist()
+        reports = []
 
-    def _compute_far_from_mean(self, prop_stats, val, item_key, ann):
-        def _far_from_mean(val, mean, stdev):
-            thr = self.far_from_mean_thr
-            return val > mean + (thr * stdev) or val < mean - (thr * stdev)
+        # report for dataset
+        reports += self._check_missing_label_categories(stats)
 
-        mean = prop_stats["mean"]
-        stdev = prop_stats["stdev"]
+        # report for item
+        reports += self._check_missing_annotation(stats)
 
-        if _far_from_mean(val, mean, stdev):
-            items_far_from_mean = prop_stats["items_far_from_mean"]
-            far_from_mean = items_far_from_mean.setdefault(item_key, {})
-            far_from_mean[ann.id] = val
+        # report for label
+        reports += self._check_undefined_label(stats)
+        reports += self._check_label_defined_but_not_found(stats)
+        reports += self._check_only_one_label(stats)
+        reports += self._check_few_samples_in_label(stats)
+        reports += self._check_imbalanced_labels(stats)
+
+        # report for attributes
+        attr_dist = stats["attribute_distribution"]
+        defined_attr_dist = attr_dist["defined_attributes"]
+        undefined_attr_dist = attr_dist["undefined_attributes"]
+
+        defined_labels = defined_attr_dist.keys()
+        for label_name in defined_labels:
+            attr_stats = defined_attr_dist[label_name]
+
+            reports += self._check_attribute_defined_but_not_found(label_name, attr_stats)
+
+            for attr_name, attr_dets in attr_stats.items():
+                reports += self._check_missing_attribute(label_name, attr_name, attr_dets)
+                reports += self._check_only_one_attribute(label_name, attr_name, attr_dets)
+                reports += self._check_few_samples_in_attribute(label_name, attr_name, attr_dets)
+                reports += self._check_imbalanced_attribute(label_name, attr_name, attr_dets)
+
+        for label_name, attr_stats in undefined_attr_dist.items():
+            for attr_name, attr_dets in attr_stats.items():
+                reports += self._check_undefined_attribute(label_name, attr_name, attr_dets)
+
+        return reports
+
+    def _generate_validation_report(self, error, *args, **kwargs):
+        return [error(*args, **kwargs)]
 
     def _check_missing_label_categories(self, stats):
         validation_reports = []
 
         if len(stats["label_distribution"]["defined_labels"]) == 0:
             validation_reports += self._generate_validation_report(
                 MissingLabelCategories, Severity.error
@@ -337,23 +351,24 @@
             details = (item_subset, label_name, attr_name)
             validation_reports += self._generate_validation_report(
                 MissingAttribute, Severity.warning, item_id, *details
             )
 
         return validation_reports
 
-    def _check_undefined_label(self, label_name, label_stats):
+    def _check_undefined_label(self, stats):
         validation_reports = []
 
-        items_with_undefined_label = label_stats["items_with_undefined_label"]
-        for item_id, item_subset in items_with_undefined_label:
-            details = (item_subset, label_name)
-            validation_reports += self._generate_validation_report(
-                UndefinedLabel, Severity.error, item_id, *details
-            )
+        undefined_label_dist = stats["label_distribution"]["undefined_labels"]
+        for label_name, label_stats in undefined_label_dist.items():
+            for item_id, item_subset in label_stats["items_with_undefined_label"]:
+                details = (item_subset, label_name)
+                validation_reports += self._generate_validation_report(
+                    UndefinedLabel, Severity.error, item_id, *details
+                )
 
         return validation_reports
 
     def _check_undefined_attribute(self, label_name, attr_name, attr_dets):
         validation_reports = []
 
         items_with_undefined_attr = attr_dets["items_with_undefined_attr"]
@@ -405,15 +420,15 @@
         if len(labels_found) == 1:
             validation_reports += self._generate_validation_report(
                 OnlyOneLabel, Severity.warning, labels_found[0]
             )
 
         return validation_reports
 
-    def _check_only_one_attribute_value(self, label_name, attr_name, attr_dets):
+    def _check_only_one_attribute(self, label_name, attr_name, attr_dets):
         validation_reports = []
         values = list(attr_dets["distribution"].keys())
 
         if len(values) == 1:
             details = (label_name, attr_name, values[0])
             validation_reports += self._generate_validation_report(
                 OnlyOneAttributeValue, Severity.warning, *details
@@ -491,168 +506,38 @@
         if balance >= thr:
             validation_reports += self._generate_validation_report(
                 ImbalancedAttribute, Severity.warning, label_name, attr_name
             )
 
         return validation_reports
 
-    def _check_imbalanced_dist_in_label(self, label_name, label_stats):
-        validation_reports = []
-        thr = self.dominance_thr
-        topk_ratio = self.topk_bins_ratio
-
-        for prop, prop_stats in label_stats.items():
-            value_counts = prop_stats["histogram"]["counts"]
-            n_bucket = len(value_counts)
-            if n_bucket < 2:
-                continue
-            topk = max(1, int(np.around(n_bucket * topk_ratio)))
-
-            if topk > 0:
-                topk_values = np.sort(value_counts)[-topk:]
-                ratio = np.sum(topk_values) / np.sum(value_counts)
-                if ratio >= thr:
-                    details = (label_name, f"{self.str_ann_type} {prop}")
-                    validation_reports += self._generate_validation_report(
-                        ImbalancedDistInLabel, Severity.warning, *details
-                    )
-
-        return validation_reports
-
-    def _check_imbalanced_dist_in_attr(self, label_name, attr_name, attr_stats):
-        validation_reports = []
-        thr = self.dominance_thr
-        topk_ratio = self.topk_bins_ratio
-
-        for attr_value, value_stats in attr_stats.items():
-            for prop, prop_stats in value_stats.items():
-                value_counts = prop_stats["histogram"]["counts"]
-                n_bucket = len(value_counts)
-                if n_bucket < 2:
-                    continue
-                topk = max(1, int(np.around(n_bucket * topk_ratio)))
-
-                if topk > 0:
-                    topk_values = np.sort(value_counts)[-topk:]
-                    ratio = np.sum(topk_values) / np.sum(value_counts)
-                    if ratio >= thr:
-                        details = (label_name, attr_name, attr_value, f"{self.str_ann_type} {prop}")
-                        validation_reports += self._generate_validation_report(
-                            ImbalancedDistInAttribute, Severity.warning, *details
-                        )
-
-        return validation_reports
-
-    def _check_invalid_value(self, stats):
-        validation_reports = []
-
-        items_w_invalid_val = stats["items_with_invalid_value"]
-        for item_dets, anns_w_invalid_val in items_w_invalid_val.items():
-            item_id, item_subset = item_dets
-            for ann_id, props in anns_w_invalid_val.items():
-                for prop in props:
-                    details = (item_subset, ann_id, f"{self.str_ann_type} {prop}")
-                    validation_reports += self._generate_validation_report(
-                        InvalidValue, Severity.error, item_id, *details
-                    )
-
-        return validation_reports
-
-    def _check_far_from_label_mean(self, label_name, label_stats):
-        validation_reports = []
-
-        for prop, prop_stats in label_stats.items():
-            items_far_from_mean = prop_stats["items_far_from_mean"]
-            if prop_stats["mean"] is not None:
-                mean = round(prop_stats["mean"], 2)
-
-            for item_dets, anns_far in items_far_from_mean.items():
-                item_id, item_subset = item_dets
-                for ann_id, val in anns_far.items():
-                    val = round(val, 2)
-                    details = (
-                        item_subset,
-                        label_name,
-                        ann_id,
-                        f"{self.str_ann_type} {prop}",
-                        mean,
-                        val,
-                    )
-                    validation_reports += self._generate_validation_report(
-                        FarFromLabelMean, Severity.warning, item_id, *details
-                    )
-
-        return validation_reports
-
-    def _check_far_from_attr_mean(self, label_name, attr_name, attr_stats):
-        validation_reports = []
-
-        for attr_value, value_stats in attr_stats.items():
-            for prop, prop_stats in value_stats.items():
-                items_far_from_mean = prop_stats["items_far_from_mean"]
-                if prop_stats["mean"] is not None:
-                    mean = round(prop_stats["mean"], 2)
-
-                for item_dets, anns_far in items_far_from_mean.items():
-                    item_id, item_subset = item_dets
-                    for ann_id, val in anns_far.items():
-                        val = round(val, 2)
-                        details = (
-                            item_subset,
-                            label_name,
-                            ann_id,
-                            attr_name,
-                            attr_value,
-                            f"{self.str_ann_type} {prop}",
-                            mean,
-                            val,
-                        )
-                        validation_reports += self._generate_validation_report(
-                            FarFromAttrMean, Severity.warning, item_id, *details
-                        )
-
-        return validation_reports
-
-    def _generate_validation_report(self, error, *args, **kwargs):
-        return [error(*args, **kwargs)]
-
 
 class ClassificationValidator(_TaskValidator):
     """
     A specific validator class for classification task.
     """
 
     def __init__(
         self,
+        task_type=TaskType.classification,
         few_samples_thr=None,
         imbalance_ratio_thr=None,
         far_from_mean_thr=None,
         dominance_ratio_thr=None,
         topk_bins=None,
     ):
         super().__init__(
-            task_type=TaskType.classification,
+            task_type=task_type,
             few_samples_thr=few_samples_thr,
             imbalance_ratio_thr=imbalance_ratio_thr,
             far_from_mean_thr=far_from_mean_thr,
             dominance_ratio_thr=dominance_ratio_thr,
             topk_bins=topk_bins,
         )
 
-    def _check_multi_label_annotations(self, stats):
-        validation_reports = []
-
-        items_with_multiple_labels = stats["items_with_multiple_labels"]
-        for item_id, item_subset in items_with_multiple_labels:
-            validation_reports += self._generate_validation_report(
-                MultiLabelAnnotations, Severity.error, item_id, item_subset
-            )
-
-        return validation_reports
-
     def compute_statistics(self, dataset):
         """
         Computes statistics of the dataset for the classification task.
 
         Parameters
         ----------
         dataset : IDataset object
@@ -661,15 +546,14 @@
         -------
         stats (dict): A dict object containing statistics of the dataset.
         """
 
         stats, filtered_anns = self._compute_common_statistics(dataset)
 
         stats["items_with_multiple_labels"] = []
-
         for item_key, anns in filtered_anns:
             ann_count = len(anns)
             if ann_count > 1:
                 stats["items_with_multiple_labels"].append(item_key)
 
         return stats
 
@@ -683,126 +567,85 @@
         stats: Dict object
 
         Returns
         -------
         reports (list): List of validation reports (DatasetValidationError).
         """
 
-        reports = []
-
-        reports += self._check_missing_label_categories(stats)
-        reports += self._check_missing_annotation(stats)
+        reports = self._generate_common_reports(stats)
         reports += self._check_multi_label_annotations(stats)
-        reports += self._check_label_defined_but_not_found(stats)
-        reports += self._check_only_one_label(stats)
-        reports += self._check_few_samples_in_label(stats)
-        reports += self._check_imbalanced_labels(stats)
-
-        label_dist = stats["label_distribution"]
-        attr_dist = stats["attribute_distribution"]
-        defined_attr_dist = attr_dist["defined_attributes"]
-        undefined_label_dist = label_dist["undefined_labels"]
-        undefined_attr_dist = attr_dist["undefined_attributes"]
-
-        defined_labels = defined_attr_dist.keys()
-        for label_name in defined_labels:
-            attr_stats = defined_attr_dist[label_name]
 
-            reports += self._check_attribute_defined_but_not_found(label_name, attr_stats)
-
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_few_samples_in_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_imbalanced_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_only_one_attribute_value(label_name, attr_name, attr_dets)
-                reports += self._check_missing_attribute(label_name, attr_name, attr_dets)
+        return reports
 
-        for label_name, label_stats in undefined_label_dist.items():
-            reports += self._check_undefined_label(label_name, label_stats)
+    def _check_multi_label_annotations(self, stats):
+        validation_reports = []
 
-        for label_name, attr_stats in undefined_attr_dist.items():
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_undefined_attribute(label_name, attr_name, attr_dets)
+        items_with_multiple_labels = stats["items_with_multiple_labels"]
+        for item_id, item_subset in items_with_multiple_labels:
+            validation_reports += self._generate_validation_report(
+                MultiLabelAnnotations, Severity.error, item_id, item_subset
+            )
 
-        return reports
+        return validation_reports
 
 
 class DetectionValidator(_TaskValidator):
     """
     A specific validator class for detection task.
     """
 
     def __init__(
         self,
+        task_type=TaskType.detection,
         few_samples_thr=None,
         imbalance_ratio_thr=None,
         far_from_mean_thr=None,
         dominance_ratio_thr=None,
         topk_bins=None,
     ):
         super().__init__(
-            task_type=TaskType.detection,
+            task_type=task_type,
             few_samples_thr=few_samples_thr,
             imbalance_ratio_thr=imbalance_ratio_thr,
             far_from_mean_thr=far_from_mean_thr,
             dominance_ratio_thr=dominance_ratio_thr,
             topk_bins=topk_bins,
         )
 
-    def _check_negative_length(self, stats):
-        validation_reports = []
-
-        items_w_neg_len = stats["items_with_negative_length"]
-        for item_dets, anns_w_neg_len in items_w_neg_len.items():
-            item_id, item_subset = item_dets
-            for ann_id, props in anns_w_neg_len.items():
-                for prop, val in props.items():
-                    val = round(val, 2)
-                    details = (item_subset, ann_id, f"{self.str_ann_type} {prop}", val)
-                    validation_reports += self._generate_validation_report(
-                        NegativeLength, Severity.error, item_id, *details
-                    )
-
-        return validation_reports
+        self.point_template = {
+            "width": deepcopy(self.numerical_stat_template),
+            "height": deepcopy(self.numerical_stat_template),
+            "area(wxh)": deepcopy(self.numerical_stat_template),
+            "ratio(w/h)": deepcopy(self.numerical_stat_template),
+            "short": deepcopy(self.numerical_stat_template),
+            "long": deepcopy(self.numerical_stat_template),
+        }
 
     def compute_statistics(self, dataset):
         """
         Computes statistics of the dataset for the detection task.
 
         Parameters
         ----------
         dataset : IDataset object
 
         Returns
         -------
         stats (dict): A dict object containing statistics of the dataset.
         """
 
-        stats, filtered_anns = self._compute_common_statistics(dataset)
-
-        # detection-specific
-        bbox_template = {
-            "width": deepcopy(self.numerical_stat_template),
-            "height": deepcopy(self.numerical_stat_template),
-            "area(wxh)": deepcopy(self.numerical_stat_template),
-            "ratio(w/h)": deepcopy(self.numerical_stat_template),
-            "short": deepcopy(self.numerical_stat_template),
-            "long": deepcopy(self.numerical_stat_template),
-        }
+        stats, filtered_items = self._compute_common_statistics(dataset)
 
         stats["items_with_negative_length"] = {}
         stats["items_with_invalid_value"] = {}
-        stats["bbox_distribution_in_label"] = {}
-        stats["bbox_distribution_in_attribute"] = {}
-        stats["bbox_distribution_in_dataset_item"] = {}
-
-        dist_by_label = stats["bbox_distribution_in_label"]
-        dist_by_attr = stats["bbox_distribution_in_attribute"]
-        bbox_dist_in_item = stats["bbox_distribution_in_dataset_item"]
-        items_w_neg_len = stats["items_with_negative_length"]
-        items_w_invalid_val = stats["items_with_invalid_value"]
+        stats["point_distribution_in_label"] = {}
+        stats["point_distribution_in_attribute"] = {}
+        stats["point_distribution_in_dataset_item"] = {}
+
+        self.items = filtered_items
 
         def _generate_ann_bbox_info(_x, _y, _w, _h, area, ratio, _short, _long):
             return {
                 "x": _x,
                 "y": _y,
                 "width": _w,
                 "height": _h,
@@ -824,21 +667,23 @@
                 ratio = float("nan")
 
             _short = _w if _w < _h else _h
             _long = _w if _w > _h else _h
 
             ann_bbox_info = _generate_ann_bbox_info(_x, _y, _w, _h, area, ratio, _short, _long)
 
+            items_w_invalid_val = stats["items_with_invalid_value"]
             for prop, val in ann_bbox_info.items():
                 if val == float("inf") or np.isnan(val):
                     bbox_has_error = True
                     anns_w_invalid_val = items_w_invalid_val.setdefault(item_key, {})
                     invalid_props = anns_w_invalid_val.setdefault(ann.id, [])
                     invalid_props.append(prop)
 
+            items_w_neg_len = stats["items_with_negative_length"]
             for prop in ["width", "height"]:
                 val = ann_bbox_info[prop]
                 if val < 1:
                     bbox_has_error = True
                     anns_w_neg_len = items_w_neg_len.setdefault(item_key, {})
                     neg_props = anns_w_neg_len.setdefault(ann.id, {})
                     neg_props[prop] = val
@@ -846,59 +691,34 @@
             if not bbox_has_error:
                 ann_bbox_info.pop("x")
                 ann_bbox_info.pop("y")
                 self._update_prop_distributions(ann_bbox_info, bbox_label_stats)
 
             return ann_bbox_info, bbox_has_error
 
+        # Collect property distribution
         label_categories = dataset.categories().get(AnnotationType.label, LabelCategories())
-        base_valid_attrs = label_categories.attributes
-
-        for item_key, annotations in filtered_anns:
-            ann_count = len(annotations)
+        self._compute_prop_dist(label_categories, stats, _update_bbox_stats_by_label)
 
-            bbox_dist_in_item[item_key] = ann_count
-
-            for ann in annotations:
-                if not 0 <= ann.label < len(label_categories):
-                    label_name = ann.label
-                    valid_attrs = set()
-                else:
-                    label_name = label_categories[ann.label].name
-                    valid_attrs = base_valid_attrs.union(label_categories[ann.label].attributes)
-
-                    bbox_label_stats = dist_by_label.setdefault(label_name, deepcopy(bbox_template))
-                    ann_bbox_info, bbox_has_error = _update_bbox_stats_by_label(
-                        item_key, ann, bbox_label_stats
-                    )
-
-                for attr, value in ann.attributes.items():
-                    if attr in valid_attrs:
-                        bbox_attr_label = dist_by_attr.setdefault(label_name, {})
-                        bbox_attr_stats = bbox_attr_label.setdefault(attr, {})
-                        bbox_val_stats = bbox_attr_stats.setdefault(
-                            str(value), deepcopy(bbox_template)
-                        )
-
-                        if not bbox_has_error:
-                            self._update_prop_distributions(ann_bbox_info, bbox_val_stats)
-
-        # Compute prop stats from distribution
+        # Compute property statistics from distribution
+        dist_by_label = stats["point_distribution_in_label"]
+        dist_by_attr = stats["point_distribution_in_attribute"]
         self._compute_prop_stats_from_dist(dist_by_label, dist_by_attr)
 
-        def _is_valid_ann(item_key, ann):
+        def _is_valid_bbox(item_key, ann):
             has_defined_label = 0 <= ann.label < len(label_categories)
             if not has_defined_label:
                 return False
 
-            bbox_has_neg_len = ann.id in items_w_neg_len.get(item_key, {})
-            bbox_has_invalid_val = ann.id in items_w_invalid_val.get(item_key, {})
+            bbox_has_neg_len = ann.id in stats["items_with_negative_length"].get(item_key, {})
+            bbox_has_invalid_val = ann.id in stats["items_with_invalid_value"].get(item_key, {})
             return not (bbox_has_neg_len or bbox_has_invalid_val)
 
-        def _update_props_far_from_mean(item_key, ann):
+        def _update_bbox_props_far_from_mean(item_key, ann):
+            base_valid_attrs = label_categories.attributes
             valid_attrs = base_valid_attrs.union(label_categories[ann.label].attributes)
             label_name = label_categories[ann.label].name
             bbox_label_stats = dist_by_label[label_name]
 
             _x, _y, _w, _h = ann.get_bbox()
             area = ann.get_area()
             ratio = _w / _h
@@ -918,18 +738,19 @@
                     bbox_attr_stats = dist_by_attr[label_name][attr]
                     bbox_val_stats = bbox_attr_stats[str(value)]
 
                     for prop, val in ann_bbox_info.items():
                         prop_stats = bbox_val_stats[prop]
                         self._compute_far_from_mean(prop_stats, val, item_key, ann)
 
-        for item_key, annotations in filtered_anns:
+        # Compute far_from_mean from property
+        for item_key, annotations in self.items:
             for ann in annotations:
-                if _is_valid_ann(item_key, ann):
-                    _update_props_far_from_mean(item_key, ann)
+                if _is_valid_bbox(item_key, ann):
+                    _update_bbox_props_far_from_mean(item_key, ann)
 
         return stats
 
     def generate_reports(self, stats):
         """
         Validates the dataset for detection tasks based on its statistics.
 
@@ -939,204 +760,360 @@
         stats : Dict object
 
         Returns
         -------
         reports (list): List of validation reports (DatasetValidationError).
         """
 
-        reports = []
-
-        reports += self._check_missing_label_categories(stats)
-        reports += self._check_missing_annotation(stats)
-        reports += self._check_label_defined_but_not_found(stats)
-        reports += self._check_only_one_label(stats)
-        reports += self._check_few_samples_in_label(stats)
-        reports += self._check_imbalanced_labels(stats)
+        reports = self._generate_common_reports(stats)
         reports += self._check_negative_length(stats)
         reports += self._check_invalid_value(stats)
 
-        label_dist = stats["label_distribution"]
-        attr_dist = stats["attribute_distribution"]
-        defined_attr_dist = attr_dist["defined_attributes"]
-        undefined_label_dist = label_dist["undefined_labels"]
-        undefined_attr_dist = attr_dist["undefined_attributes"]
+        defined_attr_dist = stats["attribute_distribution"]["defined_attributes"]
 
-        dist_by_label = stats["bbox_distribution_in_label"]
-        dist_by_attr = stats["bbox_distribution_in_attribute"]
+        dist_by_label = stats["point_distribution_in_label"]
+        dist_by_attr = stats["point_distribution_in_attribute"]
 
         defined_labels = defined_attr_dist.keys()
         for label_name in defined_labels:
-            attr_stats = defined_attr_dist[label_name]
-
-            reports += self._check_attribute_defined_but_not_found(label_name, attr_stats)
-
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_few_samples_in_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_imbalanced_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_only_one_attribute_value(label_name, attr_name, attr_dets)
-                reports += self._check_missing_attribute(label_name, attr_name, attr_dets)
-
             bbox_label_stats = dist_by_label[label_name]
             bbox_attr_label = dist_by_attr.get(label_name, {})
 
             reports += self._check_far_from_label_mean(label_name, bbox_label_stats)
             reports += self._check_imbalanced_dist_in_label(label_name, bbox_label_stats)
 
             for attr_name, bbox_attr_stats in bbox_attr_label.items():
                 reports += self._check_far_from_attr_mean(label_name, attr_name, bbox_attr_stats)
                 reports += self._check_imbalanced_dist_in_attr(
                     label_name, attr_name, bbox_attr_stats
                 )
 
-        for label_name, label_stats in undefined_label_dist.items():
-            reports += self._check_undefined_label(label_name, label_stats)
+        return reports
 
-        for label_name, attr_stats in undefined_attr_dist.items():
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_undefined_attribute(label_name, attr_name, attr_dets)
+    def _update_prop_distributions(self, curr_stats, target_stats):
+        for prop, val in curr_stats.items():
+            prop_stats = target_stats[prop]
+            prop_dist = prop_stats["distribution"]
+            prop_stats["distribution"] = np.append(prop_dist, val)
 
-        return reports
+    def _compute_prop_dist(self, label_categories, stats, update_stats_by_label):
+        dist_by_label = stats["point_distribution_in_label"]
+        dist_by_attr = stats["point_distribution_in_attribute"]
+        point_dist_in_item = stats["point_distribution_in_dataset_item"]
+
+        base_valid_attrs = label_categories.attributes
+
+        for item_key, annotations in self.items:
+            ann_count = len(annotations)
+            point_dist_in_item[item_key] = ann_count
+
+            for ann in annotations:
+                if not 0 <= ann.label < len(label_categories):
+                    label_name = ann.label
+                    valid_attrs = set()
+                else:
+                    label_name = label_categories[ann.label].name
+                    valid_attrs = base_valid_attrs.union(label_categories[ann.label].attributes)
+
+                    point_label_stats = dist_by_label.setdefault(
+                        label_name, deepcopy(self.point_template)
+                    )
+                    ann_point_info, _has_error = update_stats_by_label(
+                        item_key, ann, point_label_stats
+                    )
+
+                for attr, value in ann.attributes.items():
+                    if attr in valid_attrs:
+                        point_attr_label = dist_by_attr.setdefault(label_name, {})
+                        point_attr_stats = point_attr_label.setdefault(attr, {})
+                        point_val_stats = point_attr_stats.setdefault(
+                            str(value), deepcopy(self.point_template)
+                        )
+
+                        if not _has_error:
+                            self._update_prop_distributions(ann_point_info, point_val_stats)
+
+    def _compute_prop_stats_from_dist(self, dist_by_label, dist_by_attr):
+        for label_name, stats in dist_by_label.items():
+            prop_stats_list = list(stats.values())
+            attr_label = dist_by_attr.get(label_name, {})
+            for vals in attr_label.values():
+                for val_stats in vals.values():
+                    prop_stats_list += list(val_stats.values())
+
+            for prop_stats in prop_stats_list:
+                prop_dist = prop_stats.pop("distribution", [])
+                if len(prop_dist) > 0:
+                    prop_stats["mean"] = np.mean(prop_dist)
+                    prop_stats["stdev"] = np.std(prop_dist)
+                    prop_stats["min"] = np.min(prop_dist)
+                    prop_stats["max"] = np.max(prop_dist)
+                    prop_stats["median"] = np.median(prop_dist)
+
+                    counts, bins = np.histogram(prop_dist)
+                    prop_stats["histogram"]["bins"] = bins.tolist()
+                    prop_stats["histogram"]["counts"] = counts.tolist()
+
+    def _compute_far_from_mean(self, prop_stats, val, item_key, ann):
+        def _far_from_mean(val, mean, stdev):
+            thr = self.far_from_mean_thr
+            return val > mean + (thr * stdev) or val < mean - (thr * stdev)
+
+        mean = prop_stats["mean"]
+        stdev = prop_stats["stdev"]
+
+        if _far_from_mean(val, mean, stdev):
+            items_far_from_mean = prop_stats["items_far_from_mean"]
+            far_from_mean = items_far_from_mean.setdefault(item_key, {})
+            far_from_mean[ann.id] = val
+
+    def _check_negative_length(self, stats):
+        validation_reports = []
+
+        items_w_neg_len = stats["items_with_negative_length"]
+        for item_dets, anns_w_neg_len in items_w_neg_len.items():
+            item_id, item_subset = item_dets
+            for ann_id, props in anns_w_neg_len.items():
+                for prop, val in props.items():
+                    val = round(val, 2)
+                    details = (item_subset, ann_id, f"{self.str_ann_type} {prop}", val)
+                    validation_reports += self._generate_validation_report(
+                        NegativeLength, Severity.error, item_id, *details
+                    )
+
+        return validation_reports
+
+    def _check_invalid_value(self, stats):
+        validation_reports = []
+
+        items_w_invalid_val = stats["items_with_invalid_value"]
+        for item_dets, anns_w_invalid_val in items_w_invalid_val.items():
+            item_id, item_subset = item_dets
+            for ann_id, props in anns_w_invalid_val.items():
+                for prop in props:
+                    details = (item_subset, ann_id, f"{self.str_ann_type} {prop}")
+                    validation_reports += self._generate_validation_report(
+                        InvalidValue, Severity.error, item_id, *details
+                    )
+
+        return validation_reports
+
+    def _check_imbalanced_dist_in_label(self, label_name, label_stats):
+        validation_reports = []
+        thr = self.dominance_thr
+        topk_ratio = self.topk_bins_ratio
+
+        for prop, prop_stats in label_stats.items():
+            value_counts = prop_stats["histogram"]["counts"]
+            n_bucket = len(value_counts)
+            if n_bucket < 2:
+                continue
+            topk = max(1, int(np.around(n_bucket * topk_ratio)))
+
+            if topk > 0:
+                topk_values = np.sort(value_counts)[-topk:]
+                ratio = np.sum(topk_values) / np.sum(value_counts)
+                if ratio >= thr:
+                    details = (label_name, f"{self.str_ann_type} {prop}")
+                    validation_reports += self._generate_validation_report(
+                        ImbalancedDistInLabel, Severity.warning, *details
+                    )
+
+        return validation_reports
 
+    def _check_imbalanced_dist_in_attr(self, label_name, attr_name, attr_stats):
+        validation_reports = []
+        thr = self.dominance_thr
+        topk_ratio = self.topk_bins_ratio
 
-class SegmentationValidator(_TaskValidator):
+        for attr_value, value_stats in attr_stats.items():
+            for prop, prop_stats in value_stats.items():
+                value_counts = prop_stats["histogram"]["counts"]
+                n_bucket = len(value_counts)
+                if n_bucket < 2:
+                    continue
+                topk = max(1, int(np.around(n_bucket * topk_ratio)))
+
+                if topk > 0:
+                    topk_values = np.sort(value_counts)[-topk:]
+                    ratio = np.sum(topk_values) / np.sum(value_counts)
+                    if ratio >= thr:
+                        details = (label_name, attr_name, attr_value, f"{self.str_ann_type} {prop}")
+                        validation_reports += self._generate_validation_report(
+                            ImbalancedDistInAttribute, Severity.warning, *details
+                        )
+
+        return validation_reports
+
+    def _check_far_from_label_mean(self, label_name, label_stats):
+        validation_reports = []
+
+        for prop, prop_stats in label_stats.items():
+            items_far_from_mean = prop_stats["items_far_from_mean"]
+            if prop_stats["mean"] is not None:
+                mean = round(prop_stats["mean"], 2)
+
+            for item_dets, anns_far in items_far_from_mean.items():
+                item_id, item_subset = item_dets
+                for ann_id, val in anns_far.items():
+                    val = round(val, 2)
+                    details = (
+                        item_subset,
+                        label_name,
+                        ann_id,
+                        f"{self.str_ann_type} {prop}",
+                        mean,
+                        val,
+                    )
+                    validation_reports += self._generate_validation_report(
+                        FarFromLabelMean, Severity.warning, item_id, *details
+                    )
+
+        return validation_reports
+
+    def _check_far_from_attr_mean(self, label_name, attr_name, attr_stats):
+        validation_reports = []
+
+        for attr_value, value_stats in attr_stats.items():
+            for prop, prop_stats in value_stats.items():
+                items_far_from_mean = prop_stats["items_far_from_mean"]
+                if prop_stats["mean"] is not None:
+                    mean = round(prop_stats["mean"], 2)
+
+                for item_dets, anns_far in items_far_from_mean.items():
+                    item_id, item_subset = item_dets
+                    for ann_id, val in anns_far.items():
+                        val = round(val, 2)
+                        details = (
+                            item_subset,
+                            label_name,
+                            ann_id,
+                            attr_name,
+                            attr_value,
+                            f"{self.str_ann_type} {prop}",
+                            mean,
+                            val,
+                        )
+                        validation_reports += self._generate_validation_report(
+                            FarFromAttrMean, Severity.warning, item_id, *details
+                        )
+
+        return validation_reports
+
+
+class SegmentationValidator(DetectionValidator):
     """
     A specific validator class for (instance) segmentation task.
     """
 
     def __init__(
         self,
+        task_type=TaskType.segmentation,
         few_samples_thr=None,
         imbalance_ratio_thr=None,
         far_from_mean_thr=None,
         dominance_ratio_thr=None,
         topk_bins=None,
     ):
         super().__init__(
-            task_type=TaskType.segmentation,
+            task_type=task_type,
             few_samples_thr=few_samples_thr,
             imbalance_ratio_thr=imbalance_ratio_thr,
             far_from_mean_thr=far_from_mean_thr,
             dominance_ratio_thr=dominance_ratio_thr,
             topk_bins=topk_bins,
         )
 
+        self.point_template = {
+            "area": deepcopy(self.numerical_stat_template),
+            "width": deepcopy(self.numerical_stat_template),
+            "height": deepcopy(self.numerical_stat_template),
+        }
+
     def compute_statistics(self, dataset):
         """
         Computes statistics of the dataset for the segmentation task.
 
         Parameters
         ----------
         dataset : IDataset object
 
         Returns
         -------
         stats (dict): A dict object containing statistics of the dataset.
         """
 
-        stats, filtered_anns = self._compute_common_statistics(dataset)
-
-        # segmentation-specific
-        mask_template = {
-            "area": deepcopy(self.numerical_stat_template),
-            "width": deepcopy(self.numerical_stat_template),
-            "height": deepcopy(self.numerical_stat_template),
-        }
+        stats, filtered_items = self._compute_common_statistics(dataset)
 
         stats["items_with_invalid_value"] = {}
-        stats["mask_distribution_in_label"] = {}
-        stats["mask_distribution_in_attribute"] = {}
-        stats["mask_distribution_in_dataset_item"] = {}
-
-        dist_by_label = stats["mask_distribution_in_label"]
-        dist_by_attr = stats["mask_distribution_in_attribute"]
-        mask_dist_in_item = stats["mask_distribution_in_dataset_item"]
-        items_w_invalid_val = stats["items_with_invalid_value"]
+        stats["point_distribution_in_label"] = {}
+        stats["point_distribution_in_attribute"] = {}
+        stats["point_distribution_in_dataset_item"] = {}
+
+        self.items = filtered_items
 
         def _generate_ann_mask_info(area, _w, _h):
             return {
                 "area": area,
                 "width": _w,
                 "height": _h,
             }
 
         def _update_mask_stats_by_label(item_key, ann, mask_label_stats):
             mask_has_error = False
 
-            _x, _y, _w, _h = ann.get_bbox()
+            _, _, _w, _h = ann.get_bbox()
 
             # Detete the following block when #226 is resolved
             # https://github.com/openvinotoolkit/datumaro/issues/226
             if ann.type == AnnotationType.mask:
                 _w += 1
                 _h += 1
 
             area = ann.get_area()
 
             ann_mask_info = _generate_ann_mask_info(area, _w, _h)
 
+            items_w_invalid_val = stats["items_with_invalid_value"]
             for prop, val in ann_mask_info.items():
                 if val == float("inf") or np.isnan(val):
                     mask_has_error = True
                     anns_w_invalid_val = items_w_invalid_val.setdefault(item_key, {})
                     invalid_props = anns_w_invalid_val.setdefault(ann.id, [])
                     invalid_props.append(prop)
 
             if not mask_has_error:
                 self._update_prop_distributions(ann_mask_info, mask_label_stats)
 
             return ann_mask_info, mask_has_error
 
+        # Collect property distribution
         label_categories = dataset.categories().get(AnnotationType.label, LabelCategories())
-        base_valid_attrs = label_categories.attributes
-
-        for item_key, annotations in filtered_anns:
-            ann_count = len(annotations)
-            mask_dist_in_item[item_key] = ann_count
-
-            for ann in annotations:
-                if not 0 <= ann.label < len(label_categories):
-                    label_name = ann.label
-                    valid_attrs = set()
-                else:
-                    label_name = label_categories[ann.label].name
-                    valid_attrs = base_valid_attrs.union(label_categories[ann.label].attributes)
+        self._compute_prop_dist(label_categories, stats, _update_mask_stats_by_label)
 
-                    mask_label_stats = dist_by_label.setdefault(label_name, deepcopy(mask_template))
-                    ann_mask_info, mask_has_error = _update_mask_stats_by_label(
-                        item_key, ann, mask_label_stats
-                    )
-
-                for attr, value in ann.attributes.items():
-                    if attr in valid_attrs:
-                        mask_attr_label = dist_by_attr.setdefault(label_name, {})
-                        mask_attr_stats = mask_attr_label.setdefault(attr, {})
-                        mask_val_stats = mask_attr_stats.setdefault(
-                            str(value), deepcopy(mask_template)
-                        )
-
-                        if not mask_has_error:
-                            self._update_prop_distributions(ann_mask_info, mask_val_stats)
-
-        # compute prop stats from dist.
+        # Compute property statistics from distribution
+        dist_by_label = stats["point_distribution_in_label"]
+        dist_by_attr = stats["point_distribution_in_attribute"]
         self._compute_prop_stats_from_dist(dist_by_label, dist_by_attr)
 
-        def _is_valid_ann(item_key, ann):
+        def _is_valid_mask(item_key, ann):
             has_defined_label = 0 <= ann.label < len(label_categories)
             if not has_defined_label:
                 return False
 
-            mask_has_invalid_val = ann.id in items_w_invalid_val.get(item_key, {})
+            mask_has_invalid_val = ann.id in stats["items_with_invalid_value"].get(item_key, {})
             return not mask_has_invalid_val
 
-        def _update_props_far_from_mean(item_key, ann):
+        def _update_mask_props_far_from_mean(item_key, ann):
+            base_valid_attrs = label_categories.attributes
             valid_attrs = base_valid_attrs.union(label_categories[ann.label].attributes)
             label_name = label_categories[ann.label].name
             mask_label_stats = dist_by_label[label_name]
 
-            _x, _y, _w, _h = ann.get_bbox()
+            _, _, _w, _h = ann.get_bbox()
 
             # Detete the following block when #226 is resolved
             # https://github.com/openvinotoolkit/datumaro/issues/226
             if ann.type == AnnotationType.mask:
                 _w += 1
                 _h += 1
             area = ann.get_area()
@@ -1152,18 +1129,18 @@
                     mask_attr_stats = dist_by_attr[label_name][attr]
                     mask_val_stats = mask_attr_stats[str(value)]
 
                     for prop, val in ann_mask_info.items():
                         prop_stats = mask_val_stats[prop]
                         self._compute_far_from_mean(prop_stats, val, item_key, ann)
 
-        for item_key, annotations in filtered_anns:
+        for item_key, annotations in self.items:
             for ann in annotations:
-                if _is_valid_ann(item_key, ann):
-                    _update_props_far_from_mean(item_key, ann)
+                if _is_valid_mask(item_key, ann):
+                    _update_mask_props_far_from_mean(item_key, ann)
 
         return stats
 
     def generate_reports(self, stats):
         """
         Validates the dataset for segmentation tasks based on its statistics.
 
@@ -1173,58 +1150,30 @@
         stats : Dict object
 
         Returns
         -------
         reports (list): List of validation reports (DatasetValidationError).
         """
 
-        reports = []
-
-        reports += self._check_missing_label_categories(stats)
-        reports += self._check_missing_annotation(stats)
-        reports += self._check_label_defined_but_not_found(stats)
-        reports += self._check_only_one_label(stats)
-        reports += self._check_few_samples_in_label(stats)
-        reports += self._check_imbalanced_labels(stats)
+        reports = self._generate_common_reports(stats)
         reports += self._check_invalid_value(stats)
 
-        label_dist = stats["label_distribution"]
-        attr_dist = stats["attribute_distribution"]
-        defined_attr_dist = attr_dist["defined_attributes"]
-        undefined_label_dist = label_dist["undefined_labels"]
-        undefined_attr_dist = attr_dist["undefined_attributes"]
+        defined_attr_dist = stats["attribute_distribution"]["defined_attributes"]
 
-        dist_by_label = stats["mask_distribution_in_label"]
-        dist_by_attr = stats["mask_distribution_in_attribute"]
+        dist_by_label = stats["point_distribution_in_label"]
+        dist_by_attr = stats["point_distribution_in_attribute"]
 
         defined_labels = defined_attr_dist.keys()
         for label_name in defined_labels:
-            attr_stats = defined_attr_dist[label_name]
-
-            reports += self._check_attribute_defined_but_not_found(label_name, attr_stats)
-
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_few_samples_in_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_imbalanced_attribute(label_name, attr_name, attr_dets)
-                reports += self._check_only_one_attribute_value(label_name, attr_name, attr_dets)
-                reports += self._check_missing_attribute(label_name, attr_name, attr_dets)
-
             mask_label_stats = dist_by_label[label_name]
             mask_attr_label = dist_by_attr.get(label_name, {})
 
             reports += self._check_far_from_label_mean(label_name, mask_label_stats)
             reports += self._check_imbalanced_dist_in_label(label_name, mask_label_stats)
 
             for attr_name, mask_attr_stats in mask_attr_label.items():
                 reports += self._check_far_from_attr_mean(label_name, attr_name, mask_attr_stats)
                 reports += self._check_imbalanced_dist_in_attr(
                     label_name, attr_name, mask_attr_stats
                 )
 
-        for label_name, label_stats in undefined_label_dist.items():
-            reports += self._check_undefined_label(label_name, label_stats)
-
-        for label_name, attr_stats in undefined_attr_dist.items():
-            for attr_name, attr_dets in attr_stats.items():
-                reports += self._check_undefined_attribute(label_name, attr_name, attr_dets)
-
         return reports
```

### Comparing `datumaro-1.2.0rc1/datumaro/util/__init__.py` & `datumaro-1.2.0rc2/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/annotation_util.py` & `datumaro-1.2.0rc2/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/attrs_util.py` & `datumaro-1.2.0rc2/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/file_utils.py` & `datumaro-1.2.0rc2/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/image.py` & `datumaro-1.2.0rc2/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/image_cache.py` & `datumaro-1.2.0rc2/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/log_utils.py` & `datumaro-1.2.0rc2/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/mask_tools.py` & `datumaro-1.2.0rc2/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/meta_file_util.py` & `datumaro-1.2.0rc2/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/os_util.py` & `datumaro-1.2.0rc2/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/pickle_util.py` & `datumaro-1.2.0rc2/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/scope.py` & `datumaro-1.2.0rc2/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/telemetry_stub.py` & `datumaro-1.2.0rc2/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/telemetry_utils.py` & `datumaro-1.2.0rc2/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro/util/tf_util.py` & `datumaro-1.2.0rc2/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/datumaro.egg-info/PKG-INFO` & `datumaro-1.2.0rc2/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.0rc1
+Version: 1.2.0rc2
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.2.0rc1/datumaro.egg-info/SOURCES.txt` & `datumaro-1.2.0rc2/datumaro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 datumaro/components/annotation.py
 datumaro/components/cli_plugin.py
 datumaro/components/config.py
 datumaro/components/config_model.py
 datumaro/components/crypter.py
 datumaro/components/dataset.py
 datumaro/components/dataset_base.py
+datumaro/components/dataset_item_storage.py
 datumaro/components/environment.py
 datumaro/components/errors.py
 datumaro/components/exporter.py
 datumaro/components/extractor_tfds.py
 datumaro/components/filter.py
 datumaro/components/format_detection.py
 datumaro/components/generator.py
@@ -83,14 +84,16 @@
 datumaro/components/progress_reporting.py
 datumaro/components/project.py
 datumaro/components/searcher.py
 datumaro/components/shift_analyzer.py
 datumaro/components/transformer.py
 datumaro/components/validator.py
 datumaro/components/visualizer.py
+datumaro/components/abstracts/__init__.py
+datumaro/components/abstracts/merger.py
 datumaro/components/algorithms/__init__.py
 datumaro/components/algorithms/rise.py
 datumaro/components/algorithms/noisy_label_detection/__init__.py
 datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
 datumaro/components/annotations/__init__.py
 datumaro/components/annotations/matcher.py
 datumaro/components/annotations/merger.py
```

### Comparing `datumaro-1.2.0rc1/datumaro.egg-info/requires.txt` & `datumaro-1.2.0rc2/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/pyproject.toml` & `datumaro-1.2.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/requirements-core.txt` & `datumaro-1.2.0rc2/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.0rc1/setup.py` & `datumaro-1.2.0rc2/setup.py`

 * *Files identical despite different names*

