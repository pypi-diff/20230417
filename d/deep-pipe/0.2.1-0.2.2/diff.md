# Comparing `tmp/deep_pipe-0.2.1.tar.gz` & `tmp/deep_pipe-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_pipe-0.2.1.tar", last modified: Fri Jan 20 13:40:35 2023, max compression
+gzip compressed data, was "deep_pipe-0.2.2.tar", last modified: Mon Apr 17 08:15:39 2023, max compression
```

## Comparing `deep_pipe-0.2.1.tar` & `deep_pipe-0.2.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.825066 deep_pipe-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-20 13:40:35.825066 deep_pipe-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/deep_pipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-20 13:40:35.000000 deep_pipe-0.2.1/deep_pipe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/dpipe/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/dpipe/batch_iter/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/_pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/expiration_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/batch_iter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/dpipe/config/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/config/commands_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/config/test_locker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/dpipe/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/dicom.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/dataset/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.817066 deep_pipe-0.2.1/dpipe/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/experiment/flat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/im/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/hsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/shape_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/im/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/resblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layers/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/layout/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layout/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/layout/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/predict/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/predict/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/predict/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/prototypes/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/prototypes/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/optimization_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/test_single_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/prototypes/strategy/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/split/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/split/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/split/cv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.821066 deep_pipe-0.2.1/dpipe/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/torch/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/torch/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:40:35.825066 deep_pipe-0.2.1/dpipe/train/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/test_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/dpipe/train/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 13:40:35.825066 deep_pipe-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-20 13:40:29.000000 deep_pipe-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.469723 deep_pipe-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 08:15:39.469723 deep_pipe-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/deep_pipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 08:15:39.000000 deep_pipe-0.2.2/deep_pipe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/dpipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/dpipe/batch_iter/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/expiration_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/batch_iter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/dpipe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/config/commands_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/config/test_locker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/dpipe/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/dataset/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.457723 deep_pipe-0.2.2/dpipe/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/experiment/flat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.461723 deep_pipe-0.2.2/dpipe/im/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/hsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/shape_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/im/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.461723 deep_pipe-0.2.2/dpipe/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/resblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layers/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.461723 deep_pipe-0.2.2/dpipe/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layout/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/layout/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.461723 deep_pipe-0.2.2/dpipe/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/predict/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/predict/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.465723 deep_pipe-0.2.2/dpipe/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.465723 deep_pipe-0.2.2/dpipe/prototypes/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.465723 deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/optimization_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/test_single_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/prototypes/strategy/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.465723 deep_pipe-0.2.2/dpipe/split/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/split/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/split/cv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.465723 deep_pipe-0.2.2/dpipe/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/torch/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/torch/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:15:39.469723 deep_pipe-0.2.2/dpipe/train/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/test_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/dpipe/train/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:15:39.469723 deep_pipe-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-17 08:15:36.000000 deep_pipe-0.2.2/setup.py
```

### Comparing `deep_pipe-0.2.1/LICENSE` & `deep_pipe-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/PKG-INFO` & `deep_pipe-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deep_pipe
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of tools for deep learning experiments
 Home-page: https://github.com/neuro-ml/deep_pipe
 Author: NeuroML Group
 License: MIT
-Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.1.tar.gz
+Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.2.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deep_pipe-0.2.1/deep_pipe.egg-info/PKG-INFO` & `deep_pipe-0.2.2/deep_pipe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: deep-pipe
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of tools for deep learning experiments
 Home-page: https://github.com/neuro-ml/deep_pipe
 Author: NeuroML Group
 License: MIT
-Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.1.tar.gz
+Download-URL: https://github.com/neuro-ml/deep_pipe/v0.2.2.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `deep_pipe-0.2.1/deep_pipe.egg-info/SOURCES.txt` & `deep_pipe-0.2.2/deep_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/batch_iter/_pdp.py` & `deep_pipe-0.2.2/dpipe/batch_iter/_pdp.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/batch_iter/expiration_pool.py` & `deep_pipe-0.2.2/dpipe/batch_iter/expiration_pool.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/batch_iter/pipeline.py` & `deep_pipe-0.2.2/dpipe/batch_iter/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/batch_iter/sources.py` & `deep_pipe-0.2.2/dpipe/batch_iter/sources.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/batch_iter/utils.py` & `deep_pipe-0.2.2/dpipe/batch_iter/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/checks.py` & `deep_pipe-0.2.2/dpipe/checks.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/commands.py` & `deep_pipe-0.2.2/dpipe/commands.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/config/commands_runner.py` & `deep_pipe-0.2.2/dpipe/config/commands_runner.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/config/test_locker.py` & `deep_pipe-0.2.2/dpipe/config/test_locker.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/dataset/base.py` & `deep_pipe-0.2.2/dpipe/dataset/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/dataset/csv.py` & `deep_pipe-0.2.2/dpipe/dataset/csv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/dataset/dicom.py` & `deep_pipe-0.2.2/dpipe/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/dataset/segmentation.py` & `deep_pipe-0.2.2/dpipe/dataset/segmentation.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/dataset/wrappers.py` & `deep_pipe-0.2.2/dpipe/dataset/wrappers.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/experiment/flat.py` & `deep_pipe-0.2.2/dpipe/experiment/flat.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/augmentation.py` & `deep_pipe-0.2.2/dpipe/im/augmentation.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/axes.py` & `deep_pipe-0.2.2/dpipe/im/axes.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/box.py` & `deep_pipe-0.2.2/dpipe/im/box.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/dist.py` & `deep_pipe-0.2.2/dpipe/im/dist.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/grid.py` & `deep_pipe-0.2.2/dpipe/im/grid.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/hsv.py` & `deep_pipe-0.2.2/dpipe/im/hsv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/metrics.py` & `deep_pipe-0.2.2/dpipe/im/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/patch.py` & `deep_pipe-0.2.2/dpipe/im/patch.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/preprocessing.py` & `deep_pipe-0.2.2/dpipe/im/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/shape_ops.py` & `deep_pipe-0.2.2/dpipe/im/shape_ops.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/shape_utils.py` & `deep_pipe-0.2.2/dpipe/im/shape_utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/utils.py` & `deep_pipe-0.2.2/dpipe/im/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/im/visualize.py` & `deep_pipe-0.2.2/dpipe/im/visualize.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/io.py` & `deep_pipe-0.2.2/dpipe/io.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/itertools.py` & `deep_pipe-0.2.2/dpipe/itertools.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layers/conv.py` & `deep_pipe-0.2.2/dpipe/layers/conv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layers/fpn.py` & `deep_pipe-0.2.2/dpipe/layers/fpn.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layers/resblock.py` & `deep_pipe-0.2.2/dpipe/layers/resblock.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layers/shape.py` & `deep_pipe-0.2.2/dpipe/layers/shape.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layers/structure.py` & `deep_pipe-0.2.2/dpipe/layers/structure.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layout/base.py` & `deep_pipe-0.2.2/dpipe/layout/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/layout/scripts.py` & `deep_pipe-0.2.2/dpipe/layout/scripts.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/predict/functional.py` & `deep_pipe-0.2.2/dpipe/predict/functional.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/predict/shape.py` & `deep_pipe-0.2.2/dpipe/predict/shape.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/optimization.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/optimization.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/policy.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/optimization_fixtures.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/optimization_fixtures.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/test_composition.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/tests/test_single_strategy.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/tests/test_single_strategy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/prototypes/strategy/train.py` & `deep_pipe-0.2.2/dpipe/prototypes/strategy/train.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/split/base.py` & `deep_pipe-0.2.2/dpipe/split/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/split/cv.py` & `deep_pipe-0.2.2/dpipe/split/cv.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/torch/functional.py` & `deep_pipe-0.2.2/dpipe/torch/functional.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/torch/model.py` & `deep_pipe-0.2.2/dpipe/torch/model.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/torch/utils.py` & `deep_pipe-0.2.2/dpipe/torch/utils.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/base.py` & `deep_pipe-0.2.2/dpipe/train/base.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/checkpoint.py` & `deep_pipe-0.2.2/dpipe/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/logging.py` & `deep_pipe-0.2.2/dpipe/train/logging.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/policy.py` & `deep_pipe-0.2.2/dpipe/train/policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/test_checkpoints.py` & `deep_pipe-0.2.2/dpipe/train/test_checkpoints.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/test_policy.py` & `deep_pipe-0.2.2/dpipe/train/test_policy.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/dpipe/train/validator.py` & `deep_pipe-0.2.2/dpipe/train/validator.py`

 * *Files identical despite different names*

### Comparing `deep_pipe-0.2.1/setup.py` & `deep_pipe-0.2.2/setup.py`

 * *Files identical despite different names*

