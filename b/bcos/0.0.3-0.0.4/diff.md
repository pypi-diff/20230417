# Comparing `tmp/bcos-0.0.3.tar.gz` & `tmp/bcos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcos-0.0.3.tar", last modified: Fri Apr 14 13:56:36 2023, max compression
+gzip compressed data, was "bcos-0.0.4.tar", last modified: Mon Apr 17 11:13:56 2023, max compression
```

## Comparing `bcos-0.0.3.tar` & `bcos-0.0.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.995480 bcos-0.0.3/
--rw-r--r--   0 singh     (1000) singh     (1000)    11368 2023-03-27 17:57:32.000000 bcos-0.0.3/LICENSE
--rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-14 13:56:36.995480 bcos-0.0.3/PKG-INFO
--rw-r--r--   0 singh     (1000) singh     (1000)    10403 2023-04-02 15:27:36.000000 bcos-0.0.3/README.md
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.982146 bcos-0.0.3/bcos/
--rw-r--r--   0 singh     (1000) singh     (1000)     1308 2023-04-01 21:28:12.000000 bcos-0.0.3/bcos/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    18686 2023-04-01 21:28:12.000000 bcos-0.0.3/bcos/common.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.982146 bcos-0.0.3/bcos/data/
--rw-r--r--   0 singh     (1000) singh     (1000)        0 2023-01-30 11:46:04.000000 bcos-0.0.3/bcos/data/__init__.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/data/caching/
--rw-r--r--   0 singh     (1000) singh     (1000)      154 2023-03-06 17:39:07.000000 bcos-0.0.3/bcos/data/caching/__init__.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/data/caching/cached_imagefolder/
--rw-r--r--   0 singh     (1000) singh     (1000)       50 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1395 2023-03-27 18:57:21.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/cached_imagefolder.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4771 2023-03-27 18:57:30.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/cached_loader.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2156 2023-03-27 18:57:36.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/env.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7776 2023-03-27 18:57:41.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/redis_store.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4179 2023-03-27 18:57:46.000000 bcos-0.0.3/bcos/data/caching/cached_imagefolder/store.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1269 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/data/caching/shm_caching.py
--rw-r--r--   0 singh     (1000) singh     (1000)    18020 2023-01-30 11:46:04.000000 bcos-0.0.3/bcos/data/categories.py
--rw-r--r--   0 singh     (1000) singh     (1000)     9296 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/data/datamodules.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6767 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/data/presets.py
--rw-r--r--   0 singh     (1000) singh     (1000)     3048 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/data/sampler.py
--rw-r--r--   0 singh     (1000) singh     (1000)     8868 2023-03-23 14:26:09.000000 bcos-0.0.3/bcos/data/transforms.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.978813 bcos-0.0.3/bcos/experiments/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.978813 bcos-0.0.3/bcos/experiments/CIFAR10/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/experiments/CIFAR10/norm_ablations_final/
--rw-r--r--   0 singh     (1000) singh     (1000)     3830 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)      755 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/CIFAR10/norm_ablations_final/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.978813 bcos-0.0.3/bcos/experiments/ImageNet/
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/experiments/ImageNet/baseline/
--rw-r--r--   0 singh     (1000) singh     (1000)     2666 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/ImageNet/baseline/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)      331 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/experiments/ImageNet/baseline/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final/
--rw-r--r--   0 singh     (1000) singh     (1000)     3547 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.985480 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final_long/
--rw-r--r--   0 singh     (1000) singh     (1000)     4249 2023-03-27 15:19:32.000000 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/experiments/ImageNet/bcos_final_long/model.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.988813 bcos-0.0.3/bcos/experiments/utils/
--rw-r--r--   0 singh     (1000) singh     (1000)      121 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/experiments/utils/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7487 2023-04-02 14:57:16.000000 bcos-0.0.3/bcos/experiments/utils/config_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)      338 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/experiments/utils/exceptions.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.988813 bcos-0.0.3/bcos/experiments/utils/experiment_utils/
--rw-r--r--   0 singh     (1000) singh     (1000)       89 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/experiments/utils/experiment_utils/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    12167 2023-03-27 18:16:53.000000 bcos-0.0.3/bcos/experiments/utils/experiment_utils/experiment_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)    13331 2023-04-14 13:49:34.000000 bcos-0.0.3/bcos/experiments/utils/experiment_utils/loading_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4213 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/experiments/utils/experiment_utils/metric_utils.py
--rw-r--r--   0 singh     (1000) singh     (1000)      419 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/experiments/utils/structure_constants.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.988813 bcos-0.0.3/bcos/models/
--rw-r--r--   0 singh     (1000) singh     (1000)      128 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/models/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)    10339 2023-04-01 15:05:25.000000 bcos-0.0.3/bcos/models/convnext.py
--rw-r--r--   0 singh     (1000) singh     (1000)    15823 2023-04-01 21:28:12.000000 bcos-0.0.3/bcos/models/densenet.py
--rw-r--r--   0 singh     (1000) singh     (1000)    26244 2023-03-27 16:33:18.000000 bcos-0.0.3/bcos/models/pretrained.py
--rw-r--r--   0 singh     (1000) singh     (1000)    24106 2023-04-01 21:28:12.000000 bcos-0.0.3/bcos/models/resnet.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7068 2023-03-27 16:23:30.000000 bcos-0.0.3/bcos/models/vgg.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.992147 bcos-0.0.3/bcos/modules/
--rw-r--r--   0 singh     (1000) singh     (1000)      242 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/modules/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     9520 2023-03-27 16:28:20.000000 bcos-0.0.3/bcos/modules/bcosconv2d.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4089 2023-03-27 16:30:21.000000 bcos-0.0.3/bcos/modules/bcoslinear.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1060 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/modules/common.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1013 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/modules/logitlayer.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4189 2023-03-27 16:23:13.000000 bcos-0.0.3/bcos/modules/losses.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.992147 bcos-0.0.3/bcos/modules/norms/
--rw-r--r--   0 singh     (1000) singh     (1000)      130 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/modules/norms/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6654 2023-03-27 16:23:30.000000 bcos-0.0.3/bcos/modules/norms/centered_norms.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.992147 bcos-0.0.3/bcos/modules/norms/uncentered_norms/
--rw-r--r--   0 singh     (1000) singh     (1000)      140 2023-03-17 12:11:07.000000 bcos-0.0.3/bcos/modules/norms/uncentered_norms/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     4018 2023-03-24 13:32:00.000000 bcos-0.0.3/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     3895 2023-03-24 13:32:00.000000 bcos-0.0.3/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2518 2023-03-27 16:23:30.000000 bcos-0.0.3/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1492 2023-03-27 16:23:30.000000 bcos-0.0.3/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py
--rw-r--r--   0 singh     (1000) singh     (1000)     2005 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/modules/norms/utils.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.992147 bcos-0.0.3/bcos/optim/
--rw-r--r--   0 singh     (1000) singh     (1000)       69 2023-03-23 14:26:09.000000 bcos-0.0.3/bcos/optim/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     7725 2023-03-27 16:25:26.000000 bcos-0.0.3/bcos/optim/lr_scheduler_factory.py
--rw-r--r--   0 singh     (1000) singh     (1000)     6451 2023-03-27 16:26:11.000000 bcos-0.0.3/bcos/optim/optimizer_factory.py
--rw-r--r--   0 singh     (1000) singh     (1000)      686 2023-04-01 21:28:12.000000 bcos-0.0.3/bcos/settings.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.995480 bcos-0.0.3/bcos/training/
--rw-r--r--   0 singh     (1000) singh     (1000)       33 2023-02-14 11:37:10.000000 bcos-0.0.3/bcos/training/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1465 2023-03-08 10:36:14.000000 bcos-0.0.3/bcos/training/agc.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.995480 bcos-0.0.3/bcos/training/callbacks/
--rw-r--r--   0 singh     (1000) singh     (1000)       94 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/training/callbacks/__init__.py
--rw-r--r--   0 singh     (1000) singh     (1000)     8850 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/training/callbacks/explanation_logger.py
--rw-r--r--   0 singh     (1000) singh     (1000)     1858 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/training/callbacks/metricstracker.py
--rw-r--r--   0 singh     (1000) singh     (1000)      766 2023-01-30 11:46:04.000000 bcos-0.0.3/bcos/training/ema.py
--rw-r--r--   0 singh     (1000) singh     (1000)    13515 2023-03-27 13:43:57.000000 bcos-0.0.3/bcos/training/trainer.py
--rw-r--r--   0 singh     (1000) singh     (1000)      146 2023-04-14 13:55:01.000000 bcos-0.0.3/bcos/version.py
-drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-14 13:56:36.982146 bcos-0.0.3/bcos.egg-info/
--rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-14 13:56:36.000000 bcos-0.0.3/bcos.egg-info/PKG-INFO
--rw-r--r--   0 singh     (1000) singh     (1000)     2538 2023-04-14 13:56:36.000000 bcos-0.0.3/bcos.egg-info/SOURCES.txt
--rw-r--r--   0 singh     (1000) singh     (1000)        1 2023-04-14 13:56:36.000000 bcos-0.0.3/bcos.egg-info/dependency_links.txt
--rw-r--r--   0 singh     (1000) singh     (1000)        5 2023-04-14 13:56:36.000000 bcos-0.0.3/bcos.egg-info/top_level.txt
--rw-r--r--   0 singh     (1000) singh     (1000)      842 2023-04-14 13:55:01.000000 bcos-0.0.3/pyproject.toml
--rw-r--r--   0 singh     (1000) singh     (1000)       38 2023-04-14 13:56:36.995480 bcos-0.0.3/setup.cfg
--rw-r--r--   0 singh     (1000) singh     (1000)       85 2023-03-27 13:43:57.000000 bcos-0.0.3/setup.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/
+-rw-r--r--   0 singh     (1000) singh     (1000)    11368 2023-03-27 17:57:32.000000 bcos-0.0.4/LICENSE
+-rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-17 11:13:56.610777 bcos-0.0.4/PKG-INFO
+-rw-r--r--   0 singh     (1000) singh     (1000)    10403 2023-04-02 15:27:36.000000 bcos-0.0.4/README.md
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/
+-rw-r--r--   0 singh     (1000) singh     (1000)     1308 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    18686 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/common.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/
+-rw-r--r--   0 singh     (1000) singh     (1000)        0 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/data/__init__.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/caching/
+-rw-r--r--   0 singh     (1000) singh     (1000)      154 2023-03-06 17:39:07.000000 bcos-0.0.4/bcos/data/caching/__init__.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/data/caching/cached_imagefolder/
+-rw-r--r--   0 singh     (1000) singh     (1000)       50 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1395 2023-03-27 18:57:21.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_imagefolder.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4771 2023-03-27 18:57:30.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_loader.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2156 2023-03-27 18:57:36.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/env.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7776 2023-03-27 18:57:41.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/redis_store.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4179 2023-03-27 18:57:46.000000 bcos-0.0.4/bcos/data/caching/cached_imagefolder/store.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1269 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/caching/shm_caching.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    18020 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/data/categories.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     9296 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/datamodules.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6767 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/data/presets.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     3048 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/data/sampler.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     8868 2023-03-23 14:26:09.000000 bcos-0.0.4/bcos/data/transforms.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/CIFAR10/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/
+-rw-r--r--   0 singh     (1000) singh     (1000)     3830 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      755 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos/experiments/ImageNet/
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/baseline/
+-rw-r--r--   0 singh     (1000) singh     (1000)     2666 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/baseline/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      331 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/experiments/ImageNet/baseline/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/
+-rw-r--r--   0 singh     (1000) singh     (1000)     3547 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/
+-rw-r--r--   0 singh     (1000) singh     (1000)     4249 2023-03-27 15:19:32.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1275 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/model.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/utils/
+-rw-r--r--   0 singh     (1000) singh     (1000)      121 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7487 2023-04-02 14:57:16.000000 bcos-0.0.4/bcos/experiments/utils/config_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      338 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/exceptions.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.607444 bcos-0.0.4/bcos/experiments/utils/experiment_utils/
+-rw-r--r--   0 singh     (1000) singh     (1000)       89 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    12167 2023-03-27 18:16:53.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/experiment_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    13331 2023-04-17 11:11:28.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/loading_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4213 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/experiment_utils/metric_utils.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      419 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/experiments/utils/structure_constants.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/models/
+-rw-r--r--   0 singh     (1000) singh     (1000)      128 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/models/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    10339 2023-04-01 15:05:25.000000 bcos-0.0.4/bcos/models/convnext.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    15823 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/models/densenet.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    26244 2023-03-27 16:33:18.000000 bcos-0.0.4/bcos/models/pretrained.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    24106 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/models/resnet.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7068 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/models/vgg.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/
+-rw-r--r--   0 singh     (1000) singh     (1000)      242 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     9520 2023-03-27 16:28:20.000000 bcos-0.0.4/bcos/modules/bcosconv2d.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4089 2023-03-27 16:30:21.000000 bcos-0.0.4/bcos/modules/bcoslinear.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1060 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/common.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1013 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/modules/logitlayer.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4189 2023-03-27 16:23:13.000000 bcos-0.0.4/bcos/modules/losses.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/norms/
+-rw-r--r--   0 singh     (1000) singh     (1000)      130 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/modules/norms/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6654 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/centered_norms.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/modules/norms/uncentered_norms/
+-rw-r--r--   0 singh     (1000) singh     (1000)      140 2023-03-17 12:11:07.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     4018 2023-03-24 13:32:00.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     3895 2023-03-24 13:32:00.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2518 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1492 2023-03-27 16:23:30.000000 bcos-0.0.4/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     2005 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/modules/norms/utils.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/optim/
+-rw-r--r--   0 singh     (1000) singh     (1000)       69 2023-03-23 14:26:09.000000 bcos-0.0.4/bcos/optim/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     7725 2023-03-27 16:25:26.000000 bcos-0.0.4/bcos/optim/lr_scheduler_factory.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     6451 2023-03-27 16:26:11.000000 bcos-0.0.4/bcos/optim/optimizer_factory.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      686 2023-04-01 21:28:12.000000 bcos-0.0.4/bcos/settings.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/training/
+-rw-r--r--   0 singh     (1000) singh     (1000)       33 2023-02-14 11:37:10.000000 bcos-0.0.4/bcos/training/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1465 2023-03-08 10:36:14.000000 bcos-0.0.4/bcos/training/agc.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.610777 bcos-0.0.4/bcos/training/callbacks/
+-rw-r--r--   0 singh     (1000) singh     (1000)       94 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/__init__.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     8850 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/explanation_logger.py
+-rw-r--r--   0 singh     (1000) singh     (1000)     1858 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/callbacks/metricstracker.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      766 2023-01-30 11:46:04.000000 bcos-0.0.4/bcos/training/ema.py
+-rw-r--r--   0 singh     (1000) singh     (1000)    13515 2023-03-27 13:43:57.000000 bcos-0.0.4/bcos/training/trainer.py
+-rw-r--r--   0 singh     (1000) singh     (1000)      146 2023-04-17 11:12:34.000000 bcos-0.0.4/bcos/version.py
+drwxr-xr-x   0 singh     (1000) singh     (1000)        0 2023-04-17 11:13:56.604110 bcos-0.0.4/bcos.egg-info/
+-rw-r--r--   0 singh     (1000) singh     (1000)    10720 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/PKG-INFO
+-rw-r--r--   0 singh     (1000) singh     (1000)     2538 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/SOURCES.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)        1 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/dependency_links.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)        5 2023-04-17 11:13:56.000000 bcos-0.0.4/bcos.egg-info/top_level.txt
+-rw-r--r--   0 singh     (1000) singh     (1000)      842 2023-04-17 11:12:34.000000 bcos-0.0.4/pyproject.toml
+-rw-r--r--   0 singh     (1000) singh     (1000)       38 2023-04-17 11:13:56.610777 bcos-0.0.4/setup.cfg
+-rw-r--r--   0 singh     (1000) singh     (1000)       85 2023-03-27 13:43:57.000000 bcos-0.0.4/setup.py
```

### Comparing `bcos-0.0.3/LICENSE` & `bcos-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/PKG-INFO` & `bcos-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcos
-Version: 0.0.3
+Version: 0.0.4
 Summary: B-cos models.
 Author-email: Moritz Böhle <mboehle@mpi-inf.mpg.de>, Navdeeppal Singh <npsingh0181@gmail.com>
 License: Apache License 2.0
 Project-URL: repository, https://github.com/B-cos/B-cos-v2/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bcos-0.0.3/README.md` & `bcos-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/__init__.py` & `bcos-0.0.4/bcos/__init__.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/common.py` & `bcos-0.0.4/bcos/common.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/cached_imagefolder/cached_imagefolder.py` & `bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_imagefolder.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/cached_imagefolder/cached_loader.py` & `bcos-0.0.4/bcos/data/caching/cached_imagefolder/cached_loader.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/cached_imagefolder/env.py` & `bcos-0.0.4/bcos/data/caching/cached_imagefolder/env.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/cached_imagefolder/redis_store.py` & `bcos-0.0.4/bcos/data/caching/cached_imagefolder/redis_store.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/cached_imagefolder/store.py` & `bcos-0.0.4/bcos/data/caching/cached_imagefolder/store.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/caching/shm_caching.py` & `bcos-0.0.4/bcos/data/caching/shm_caching.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/categories.py` & `bcos-0.0.4/bcos/data/categories.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/datamodules.py` & `bcos-0.0.4/bcos/data/datamodules.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/presets.py` & `bcos-0.0.4/bcos/data/presets.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/sampler.py` & `bcos-0.0.4/bcos/data/sampler.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/data/transforms.py` & `bcos-0.0.4/bcos/data/transforms.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py` & `bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/CIFAR10/norm_ablations_final/model.py` & `bcos-0.0.4/bcos/experiments/CIFAR10/norm_ablations_final/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/ImageNet/baseline/experiment_parameters.py` & `bcos-0.0.4/bcos/experiments/ImageNet/baseline/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py` & `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/ImageNet/bcos_final/model.py` & `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py` & `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/experiment_parameters.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/ImageNet/bcos_final_long/model.py` & `bcos-0.0.4/bcos/experiments/ImageNet/bcos_final_long/model.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/utils/config_utils.py` & `bcos-0.0.4/bcos/experiments/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/utils/experiment_utils/experiment_utils.py` & `bcos-0.0.4/bcos/experiments/utils/experiment_utils/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/experiments/utils/experiment_utils/loading_utils.py` & `bcos-0.0.4/bcos/experiments/utils/experiment_utils/loading_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         cls,
         training_ckpt: StateDictType,
         ema: bool = False,
     ) -> StateDictType:
         model_state_dict = training_ckpt["state_dict"]
         prefix = cls.MODEL_STATE_DICT_EMA_PREFIX if ema else cls.MODEL_STATE_DICT_PREFIX
 
-        if ema and not all(k.startswith(prefix) for k in model_state_dict.keys()):
+        if ema and not any(k.startswith(prefix) for k in model_state_dict.keys()):
             raise EMANotFound("EMA state dict not found in training checkpoint!")
 
         model_state_dict = change_state_dict_keys(
             model_state_dict, prefix_filter=prefix
         )
         return model_state_dict
```

### Comparing `bcos-0.0.3/bcos/experiments/utils/experiment_utils/metric_utils.py` & `bcos-0.0.4/bcos/experiments/utils/experiment_utils/metric_utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/models/convnext.py` & `bcos-0.0.4/bcos/models/convnext.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/models/densenet.py` & `bcos-0.0.4/bcos/models/densenet.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/models/pretrained.py` & `bcos-0.0.4/bcos/models/pretrained.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/models/resnet.py` & `bcos-0.0.4/bcos/models/resnet.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/models/vgg.py` & `bcos-0.0.4/bcos/models/vgg.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/bcosconv2d.py` & `bcos-0.0.4/bcos/modules/bcosconv2d.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/bcoslinear.py` & `bcos-0.0.4/bcos/modules/bcoslinear.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/common.py` & `bcos-0.0.4/bcos/modules/common.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/logitlayer.py` & `bcos-0.0.4/bcos/modules/logitlayer.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/losses.py` & `bcos-0.0.4/bcos/modules/losses.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/centered_norms.py` & `bcos-0.0.4/bcos/modules/norms/centered_norms.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py` & `bcos-0.0.4/bcos/modules/norms/uncentered_norms/allnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py` & `bcos-0.0.4/bcos/modules/norms/uncentered_norms/batchnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py` & `bcos-0.0.4/bcos/modules/norms/uncentered_norms/groupnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py` & `bcos-0.0.4/bcos/modules/norms/uncentered_norms/posnorm_uncentered.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/modules/norms/utils.py` & `bcos-0.0.4/bcos/modules/norms/utils.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/optim/lr_scheduler_factory.py` & `bcos-0.0.4/bcos/optim/lr_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/optim/optimizer_factory.py` & `bcos-0.0.4/bcos/optim/optimizer_factory.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/settings.py` & `bcos-0.0.4/bcos/settings.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/training/agc.py` & `bcos-0.0.4/bcos/training/agc.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/training/callbacks/explanation_logger.py` & `bcos-0.0.4/bcos/training/callbacks/explanation_logger.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/training/callbacks/metricstracker.py` & `bcos-0.0.4/bcos/training/callbacks/metricstracker.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/training/ema.py` & `bcos-0.0.4/bcos/training/ema.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos/training/trainer.py` & `bcos-0.0.4/bcos/training/trainer.py`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/bcos.egg-info/PKG-INFO` & `bcos-0.0.4/bcos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcos
-Version: 0.0.3
+Version: 0.0.4
 Summary: B-cos models.
 Author-email: Moritz Böhle <mboehle@mpi-inf.mpg.de>, Navdeeppal Singh <npsingh0181@gmail.com>
 License: Apache License 2.0
 Project-URL: repository, https://github.com/B-cos/B-cos-v2/
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bcos-0.0.3/bcos.egg-info/SOURCES.txt` & `bcos-0.0.4/bcos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bcos-0.0.3/pyproject.toml` & `bcos-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "bcos"
 authors = [
     {name = "Moritz Böhle", email = "mboehle@mpi-inf.mpg.de"},
     {name = "Navdeeppal Singh", email = "npsingh0181@gmail.com"},
 ]
-version = "0.0.3"
+version = "0.0.4"
 description = "B-cos models."
 readme = "README.md"
 license = {text = "Apache License 2.0"}
 
 [project.urls]
 repository = "https://github.com/B-cos/B-cos-v2/"
```

