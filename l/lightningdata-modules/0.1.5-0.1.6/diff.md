# Comparing `tmp/lightningdata-modules-0.1.5.tar.gz` & `tmp/lightningdata-modules-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightningdata-modules-0.1.5.tar", last modified: Mon Mar 13 13:44:49 2023, max compression
+gzip compressed data, was "lightningdata-modules-0.1.6.tar", last modified: Mon Apr 17 14:07:53 2023, max compression
```

## Comparing `lightningdata-modules-0.1.5.tar` & `lightningdata-modules-0.1.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.125824 lightningdata-modules-0.1.5/
--rw-rw-rw-   0        0        0     2430 2023-03-13 13:44:49.125824 lightningdata-modules-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1761 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.764874 lightningdata-modules-0.1.5/lightningdata/
--rw-rw-rw-   0        0        0     1352 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.780503 lightningdata-modules-0.1.5/lightningdata/common/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/common/__init__.py
--rw-rw-rw-   0        0        0      508 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/common/config.py
--rw-rw-rw-   0        0        0     4823 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/common/folder2lmdb.py
--rw-rw-rw-   0        0        0     8727 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/common/pre_process.py
--rw-rw-rw-   0        0        0     2395 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.780503 lightningdata-modules-0.1.5/lightningdata/modules/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/__init__.py
--rw-rw-rw-   0        0        0     2241 2023-03-13 13:17:32.000000 lightningdata-modules-0.1.5/lightningdata/modules/datamodule_base.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.805136 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/digit5_datamodule.py
--rw-rw-rw-   0        0        0     8573 2023-03-13 13:17:03.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
--rw-rw-rw-   0        0        0     1394 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
--rw-rw-rw-   0        0        0     1363 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/office31_datamodule.py
--rw-rw-rw-   0        0        0     1405 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.812144 lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/emnist_datamodule.py
--rw-rw-rw-   0        0        0     3966 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/federatedLearning_base.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.827772 lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/__init__.py
--rw-rw-rw-   0        0        0     3378 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/metaLearning_base.py
--rw-rw-rw-   0        0        0     2181 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
--rw-rw-rw-   0        0        0     2156 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/omiglot_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.827772 lightningdata-modules-0.1.5/lightningdata/thirdparty/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.827772 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/
--rw-rw-rw-   0        0        0      359 2023-03-13 09:58:57.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.937548 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/
--rw-rw-rw-   0        0        0     1581 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/__init__.py
--rw-rw-rw-   0        0        0    18803 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/bach.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:48.953171 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/
--rw-rw-rw-   0        0        0      191 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
--rw-rw-rw-   0        0        0     6686 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
--rw-rw-rw-   0        0        0     5214 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
--rw-rw-rw-   0        0        0     5583 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
--rw-rw-rw-   0        0        0     9804 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cub.py
--rw-rw-rw-   0        0        0    10081 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
--rw-rw-rw-   0        0        0    14034 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/helpers.py
--rw-rw-rw-   0        0        0     6347 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
--rw-rw-rw-   0        0        0    11381 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/letter.py
--rw-rw-rw-   0        0        0     9014 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
--rw-rw-rw-   0        0        0    11020 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
--rw-rw-rw-   0        0        0    14444 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
--rw-rw-rw-   0        0        0    14366 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
--rw-rw-rw-   0        0        0    14467 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
--rw-rw-rw-   0        0        0     9741 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
--rw-rw-rw-   0        0        0    21344 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/tcga.py
--rw-rw-rw-   0        0        0    10445 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
--rw-rw-rw-   0        0        0    10092 2023-03-13 10:01:31.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
--rw-rw-rw-   0        0        0     1927 2023-03-13 10:37:57.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.005550 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/
--rw-rw-rw-   0        0        0     1120 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/activation.py
--rw-rw-rw-   0        0        0     2361 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
--rw-rw-rw-   0        0        0      755 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/container.py
--rw-rw-rw-   0        0        0     1184 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/conv.py
--rw-rw-rw-   0        0        0      809 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/linear.py
--rw-rw-rw-   0        0        0     2500 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/module.py
--rw-rw-rw-   0        0        0      571 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/normalization.py
--rw-rw-rw-   0        0        0     2138 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/parallel.py
--rw-rw-rw-   0        0        0     1110 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/sparse.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.016059 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/
--rw-rw-rw-   0        0        0      352 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/__init__.py
--rw-rw-rw-   0        0        0     5747 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/harmonic.py
--rw-rw-rw-   0        0        0     4225 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/helpers.py
--rw-rw-rw-   0        0        0     4873 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
--rw-rw-rw-   0        0        0     6480 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.047311 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/
--rw-rw-rw-   0        0        0      561 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/__init__.py
--rw-rw-rw-   0        0        0     2664 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
--rw-rw-rw-   0        0        0     2826 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/categorical.py
--rw-rw-rw-   0        0        0    16696 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/splitters.py
--rw-rw-rw-   0        0        0      578 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
--rw-rw-rw-   0        0        0     1361 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
--rw-rw-rw-   0        0        0     1168 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.078557 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/
--rw-rw-rw-   0        0        0      863 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.110196 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/
--rw-rw-rw-   0        0        0      838 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
--rw-rw-rw-   0        0        0     2714 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
--rw-rw-rw-   0        0        0    14127 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
--rw-rw-rw-   0        0        0     2157 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
--rw-rw-rw-   0        0        0     2256 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/task.py
--rw-rw-rw-   0        0        0     3211 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
--rw-rw-rw-   0        0        0     2393 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
--rw-rw-rw-   0        0        0     7826 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/matching.py
--rw-rw-rw-   0        0        0     4377 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/metrics.py
--rw-rw-rw-   0        0        0     2909 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/prototype.py
--rw-rw-rw-   0        0        0     5089 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/r2d2.py
--rw-rw-rw-   0        0        0       17 2023-03-13 09:42:33.000000 lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/version.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:44:49.125824 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/
--rw-rw-rw-   0        0        0     2430 2023-03-13 13:44:48.000000 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4581 2023-03-13 13:44:48.000000 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 13:44:48.000000 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-13 13:44:48.000000 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-13 13:44:48.000000 lightningdata-modules-0.1.5/lightningdata_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 13:44:49.125824 lightningdata-modules-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-03-13 13:42:46.000000 lightningdata-modules-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.321437 lightningdata-modules-0.1.6/
+-rw-rw-rw-   0        0        0     2430 2023-04-17 14:07:53.320446 lightningdata-modules-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1761 2022-11-09 12:29:04.000000 lightningdata-modules-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.511141 lightningdata-modules-0.1.6/lightningdata/
+-rw-rw-rw-   0        0        0     1461 2023-04-17 07:40:15.000000 lightningdata-modules-0.1.6/lightningdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.540141 lightningdata-modules-0.1.6/lightningdata/common/
+-rw-rw-rw-   0        0        0        0 2022-02-02 14:20:15.000000 lightningdata-modules-0.1.6/lightningdata/common/__init__.py
+-rw-rw-rw-   0        0        0      550 2023-04-17 07:36:40.000000 lightningdata-modules-0.1.6/lightningdata/common/config.py
+-rw-rw-rw-   0        0        0     4883 2023-04-17 14:03:41.000000 lightningdata-modules-0.1.6/lightningdata/common/folder2lmdb.py
+-rw-rw-rw-   0        0        0     8727 2022-02-14 12:32:07.000000 lightningdata-modules-0.1.6/lightningdata/common/pre_process.py
+-rw-rw-rw-   0        0        0     2395 2022-02-15 15:32:32.000000 lightningdata-modules-0.1.6/lightningdata/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.542141 lightningdata-modules-0.1.6/lightningdata/modules/
+-rw-rw-rw-   0        0        0        0 2022-02-11 08:08:08.000000 lightningdata-modules-0.1.6/lightningdata/modules/__init__.py
+-rw-rw-rw-   0        0        0     2241 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/modules/datamodule_base.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.577140 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/
+-rw-rw-rw-   0        0        0        0 2022-02-09 11:07:33.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/__init__.py
+-rw-rw-rw-   0        0        0     1346 2022-02-21 13:22:43.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/digit5_datamodule.py
+-rw-rw-rw-   0        0        0     8573 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
+-rw-rw-rw-   0        0        0     1394 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
+-rw-rw-rw-   0        0        0     1363 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/office31_datamodule.py
+-rw-rw-rw-   0        0        0     1405 2022-02-21 13:22:15.000000 lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.596144 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/
+-rw-rw-rw-   0        0        0        0 2022-02-10 14:34:26.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-02-11 09:46:51.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/emnist_datamodule.py
+-rw-rw-rw-   0        0        0     3966 2022-11-09 12:58:43.000000 lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/federatedLearning_base.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.621142 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/
+-rw-rw-rw-   0        0        0        0 2022-04-12 08:56:02.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/__init__.py
+-rw-rw-rw-   0        0        0     3378 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/metaLearning_base.py
+-rw-rw-rw-   0        0        0     2181 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
+-rw-rw-rw-   0        0        0     2156 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/omiglot_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.623145 lightningdata-modules-0.1.6/lightningdata/thirdparty/
+-rw-rw-rw-   0        0        0        0 2022-11-09 14:16:25.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.643143 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/
+-rw-rw-rw-   0        0        0      352 2022-11-09 14:09:26.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.812422 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/
+-rw-rw-rw-   0        0        0     1620 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/__init__.py
+-rw-rw-rw-   0        0        0    19222 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/bach.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.847442 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/
+-rw-rw-rw-   0        0        0      195 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
+-rw-rw-rw-   0        0        0     6861 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
+-rw-rw-rw-   0        0        0     5332 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
+-rw-rw-rw-   0        0        0     5708 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
+-rw-rw-rw-   0        0        0    10048 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cub.py
+-rw-rw-rw-   0        0        0    10334 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
+-rw-rw-rw-   0        0        0    14448 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers.py
+-rw-rw-rw-   0        0        0     6522 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
+-rw-rw-rw-   0        0        0    11646 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/letter.py
+-rw-rw-rw-   0        0        0     9242 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
+-rw-rw-rw-   0        0        0    11285 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
+-rw-rw-rw-   0        0        0    14763 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
+-rw-rw-rw-   0        0        0    14686 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
+-rw-rw-rw-   0        0        0    14786 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
+-rw-rw-rw-   0        0        0    10004 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
+-rw-rw-rw-   0        0        0    21872 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tcga.py
+-rw-rw-rw-   0        0        0    10696 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
+-rw-rw-rw-   0        0        0    10345 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
+-rw-rw-rw-   0        0        0     1975 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:52.976430 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/
+-rw-rw-rw-   0        0        0     1100 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/__init__.py
+-rw-rw-rw-   0        0        0     2576 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/activation.py
+-rw-rw-rw-   0        0        0     2301 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
+-rw-rw-rw-   0        0        0      736 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/container.py
+-rw-rw-rw-   0        0        0     1149 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/conv.py
+-rw-rw-rw-   0        0        0      786 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/linear.py
+-rw-rw-rw-   0        0        0     2437 2022-11-09 13:14:11.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/module.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/normalization.py
+-rw-rw-rw-   0        0        0     2091 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/parallel.py
+-rw-rw-rw-   0        0        0     1084 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/sparse.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.041447 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/
+-rw-rw-rw-   0        0        0      345 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/__init__.py
+-rw-rw-rw-   0        0        0     5592 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/harmonic.py
+-rw-rw-rw-   0        0        0     4121 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/helpers.py
+-rw-rw-rw-   0        0        0     4744 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
+-rw-rw-rw-   0        0        0     6312 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.127425 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/
+-rw-rw-rw-   0        0        0      556 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2589 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
+-rw-rw-rw-   0        0        0     2748 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/categorical.py
+-rw-rw-rw-   0        0        0    16328 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/splitters.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
+-rw-rw-rw-   0        0        0     1325 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
+-rw-rw-rw-   0        0        0     1139 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.214445 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/
+-rw-rw-rw-   0        0        0      843 2022-11-09 14:09:46.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.294468 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/
+-rw-rw-rw-   0        0        0      818 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
+-rw-rw-rw-   0        0        0     2651 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
+-rw-rw-rw-   0        0        0    13806 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
+-rw-rw-rw-   0        0        0     2113 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
+-rw-rw-rw-   0        0        0     2190 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/task.py
+-rw-rw-rw-   0        0        0     3129 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
+-rw-rw-rw-   0        0        0     2330 2022-11-09 14:09:55.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
+-rw-rw-rw-   0        0        0     7624 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/matching.py
+-rw-rw-rw-   0        0        0     4277 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/metrics.py
+-rw-rw-rw-   0        0        0     2832 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/prototype.py
+-rw-rw-rw-   0        0        0     4966 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/r2d2.py
+-rw-rw-rw-   0        0        0       17 2022-11-09 13:14:09.000000 lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/version.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:07:53.318441 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/
+-rw-rw-rw-   0        0        0     2430 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4581 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 14:07:52.000000 lightningdata-modules-0.1.6/lightningdata_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:07:53.321437 lightningdata-modules-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-04-17 14:07:24.000000 lightningdata-modules-0.1.6/setup.py
```

### Comparing `lightningdata-modules-0.1.5/PKG-INFO` & `lightningdata-modules-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.5/README.md` & `lightningdata-modules-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # base data module
 from .modules.datamodule_base import LightningDataBase
 # domain adaptation data modules
 from .modules.domain_adaptation.domainAdaptation_base import DomainAdaptationDataModule
 from .modules.domain_adaptation.officeHome_datamodule import OfficeHomeDataModule
 from .modules.domain_adaptation.office31_datamodule import Office31DataModule
 from .modules.domain_adaptation.digit5_datamodule import Digit5DataModule
+from .modules.domain_adaptation.domainNet_datamodule import DomainNetDataModule
 # federated learning data modules
 from .modules.federated_learning.federatedLearning_base import FederatedLearningDataModule
 from .modules.federated_learning.emnist_datamodule import EmnistDataModule
 # meta learning data modules
 from .modules.meta_learning.metaLearning_base import MetaLearningDataModule
 from .modules.meta_learning.omiglot_datamodule import OmiglotDataModule
 from .modules.meta_learning.mini_imagenet_datamodule import MiniImageNetDataModule
 # ImageFolderLMDB, folder2lmdb
 from.common.folder2lmdb import ImageFolderLMDB, folder2lmdb
 
 __all__ = [
     "LightningDataBase",
     "DomainAdaptationDataModule",
-    "FederatedLearningDataModule",
-    "Digit5DataModule",
-    "Office31DataModule",
     "OfficeHomeDataModule",
+    "Office31DataModule",
+    "Digit5DataModule",
+    "DomainNetDataModule",
+    "FederatedLearningDataModule",
     "EmnistDataModule",
     "MetaLearningDataModule",
     "OmiglotDataModule",
     "MiniImageNetDataModule",
     "ImageFolderLMDB",
     "folder2lmdb"
     ]
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/common/folder2lmdb.py` & `lightningdata-modules-0.1.6/lightningdata/common/folder2lmdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from PIL import Image
 import torch.utils.data as data
 from torch.utils.data import DataLoader
 from torchvision.datasets import ImageFolder
 from torchvision import transforms
 import pickle
 
+""" Source: https://github.com/rmccorm4/PyTorch-LMDB """
+
 
 class ImageFolderLMDB(data.Dataset):
     def __init__(self, db_path, transform=transforms.ToTensor(), target_transform=None):
         self.db_path = db_path
         self.transform = transform
         self.target_transform = target_transform
         # attributes that are lazy-loaded
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/common/pre_process.py` & `lightningdata-modules-0.1.6/lightningdata/common/pre_process.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/common/utils.py` & `lightningdata-modules-0.1.6/lightningdata/common/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/datamodule_base.py` & `lightningdata-modules-0.1.6/lightningdata/modules/datamodule_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/digit5_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/digit5_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/domainAdaptation_base.py` & `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainAdaptation_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/domainNet_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/domainNet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/office31_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/office31_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/domain_adaptation/officeHome_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/domain_adaptation/officeHome_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/emnist_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/emnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/federated_learning/federatedLearning_base.py` & `lightningdata-modules-0.1.6/lightningdata/modules/federated_learning/federatedLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/metaLearning_base.py` & `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/metaLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/modules/meta_learning/omiglot_datamodule.py` & `lightningdata-modules-0.1.6/lightningdata/modules/meta_learning/omiglot_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from lightningdata.thirdparty.torchmeta.datasets.triplemnist import TripleMNIST
-from lightningdata.thirdparty.torchmeta.datasets.doublemnist import DoubleMNIST
-from lightningdata.thirdparty.torchmeta.datasets.cub import CUB
-from lightningdata.thirdparty.torchmeta.datasets.cifar100 import CIFARFS, FC100
-from lightningdata.thirdparty.torchmeta.datasets.miniimagenet import MiniImagenet
-from lightningdata.thirdparty.torchmeta.datasets.omniglot import Omniglot
-from lightningdata.thirdparty.torchmeta.datasets.tieredimagenet import TieredImagenet
-from lightningdata.thirdparty.torchmeta.datasets.tcga import TCGA
-from lightningdata.thirdparty.torchmeta.datasets.pascal5i import Pascal5i
-from lightningdata.thirdparty.torchmeta.datasets.letter import Letter
-from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_texture import PlantsTexture
-from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_shape import PlantsShape
-from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_margin import PlantsMargin
-from lightningdata.thirdparty.torchmeta.datasets.bach import Bach
-
-from lightningdata.thirdparty.torchmeta.datasets import helpers
-from lightningdata.thirdparty.torchmeta.datasets import helpers_tabular
-
-__all__ = [
-    # image data
-    'TCGA',
-    'Omniglot',
-    'MiniImagenet',
-    'TieredImagenet',
-    'CIFARFS',
-    'FC100',
-    'CUB',
-    'DoubleMNIST',
-    'TripleMNIST',
-    'Pascal5i',
-    'helpers',
-    # tabular data
-    'Letter',
-    'PlantsTexture',
-    'PlantsShape',
-    'PlantsMargin',
-    'Bach',
-    'helpers_tabular'
-]
+from lightningdata.thirdparty.torchmeta.datasets.triplemnist import TripleMNIST
+from lightningdata.thirdparty.torchmeta.datasets.doublemnist import DoubleMNIST
+from lightningdata.thirdparty.torchmeta.datasets.cub import CUB
+from lightningdata.thirdparty.torchmeta.datasets.cifar100 import CIFARFS, FC100
+from lightningdata.thirdparty.torchmeta.datasets.miniimagenet import MiniImagenet
+from lightningdata.thirdparty.torchmeta.datasets.omniglot import Omniglot
+from lightningdata.thirdparty.torchmeta.datasets.tieredimagenet import TieredImagenet
+from lightningdata.thirdparty.torchmeta.datasets.tcga import TCGA
+from lightningdata.thirdparty.torchmeta.datasets.pascal5i import Pascal5i
+from lightningdata.thirdparty.torchmeta.datasets.letter import Letter
+from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_texture import PlantsTexture
+from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_shape import PlantsShape
+from lightningdata.thirdparty.torchmeta.datasets.one_hundred_plants_margin import PlantsMargin
+from lightningdata.thirdparty.torchmeta.datasets.bach import Bach
+
+from lightningdata.thirdparty.torchmeta.datasets import helpers
+from lightningdata.thirdparty.torchmeta.datasets import helpers_tabular
+
+__all__ = [
+    # image data
+    'TCGA',
+    'Omniglot',
+    'MiniImagenet',
+    'TieredImagenet',
+    'CIFARFS',
+    'FC100',
+    'CUB',
+    'DoubleMNIST',
+    'TripleMNIST',
+    'Pascal5i',
+    'helpers',
+    # tabular data
+    'Letter',
+    'PlantsTexture',
+    'PlantsShape',
+    'PlantsMargin',
+    'Bach',
+    'helpers_tabular'
+]
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/bach.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/bach.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,419 +1,419 @@
-import numpy as np
-import os
-import json
-import h5py
-from tqdm import tqdm
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class Bach(CombinationMetaDataset):
-    """The Bach dataset """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False, process_features=True, min_num_samples_per_class=1):
-        """
-        Bach Choral Harmony dataset [1], [2]
-        open-ml-id: 4552
-        https://archive.ics.uci.edu/ml/datasets/Bach+Choral+Harmony
-
-        Abstract: The data set is composed of 60 chorales (5665 events) by
-        J.S. Bach (1675-1750). Each event of each chorale is labelled using 1
-        among 101 chord labels and described through 14 features.
-
-        Data Set Information:
-
-        Pitch classes information has been extracted from MIDI sources downloaded
-        from (JSB Chorales)[http://www.jsbchorales.net/]. Meter information has
-        been computed through the Meter program which is part of the Melisma
-        music analyser (Melisma)[http://www.link.cs.cmu.edu/music-analysis/].
-        Chord labels have been manually annotated by a human expert.
-
-        Attribute Information:
-
-        1. Choral ID: corresponding to the file names from (Bach Central)[http://www.bachcentral.com/].
-        2. Event number: index (starting from 1) of the event inside the chorale.
-        3-14. Pitch classes: YES/NO depending on whether a given pitch is present.
-        Pitch classes/attribute correspondence is as follows:
-        C -> 3
-        C#/Db -> 4
-        D -> 5
-        ...
-        B -> 14
-        15. Bass: Pitch class of the bass note
-        16. Meter: integers from 1 to 5. Lower numbers denote less accented events,
-        higher numbers denote more accented events.
-        17. Chord label: Chord resonating during the given event.
-
-        Notes
-        ----------
-
-        The features V1 and V2 are dropped during the processing. V1 is the Choral ID. V2 is
-        the event number of the event inside the chorale.
-
-        Parameters
-        ----------
-        root : string
-            Root directory where the dataset folder `bach` exists.
-
-        num_classes_per_task : int
-            Number of classes per tasks. This corresponds to "N" in "N-way"
-            classification.
-
-        meta_train : bool (default: `False`)
-            Use the meta-train split of the dataset. If set to `True`, then the
-            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
-            of these three arguments must be set to `True`.
-
-        meta_val : bool (default: `False`)
-            Use the meta-validation split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_test : bool (default: `False`)
-            Use the meta-test split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_split : string in {'train', 'val', 'test'}, optional
-            Name of the split to use. This overrides the arguments `meta_train`,
-            `meta_val` and `meta_test` if all three are set to `False`.
-
-        transform : callable, optional
-            A function/transform that takes a numpy array or a pytorch array
-            (depending when the transforms is applied), and returns a transformed
-            version.
-
-        target_transform : callable, optional
-            A function/transform that takes a target, and returns a transformed
-            version.
-
-        dataset_transform : callable, optional
-            A function/transform that takes a dataset (ie. a task), and returns a
-            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-        class_augmentations : list of callable, optional
-            A list of functions that augment the dataset with new classes. These
-            classes are transformations of existing classes.
-
-        download : bool (default: `False`)
-            If `True`, downloads the original files and processes the dataset in the
-            root directory (under the `bach' folder). If the dataset
-            is already available, this does not download/process the dataset again.
-
-        process_features : bool (default: `True`)
-            If `True`, normalizes the numeric feature f according to (f-lower) / (upper - lower) where upper
-            and lower are the min and max values of feature f of the meta-train dataset.
-            And also one-hot encodes the categorical features.
-
-        min_num_samples_per_class : int (default: 1)
-            Minimal number of samples per class that need to be present for the class to be used.
-
-        References
-        -----
-
-        [1] D. P. Radicioni and R. Esposito. Advances in Music Information Retrieval,
-        chapter BREVE: an HMPerceptron-Based Chord Recognition System.
-        Studies in Computational Intelligence,
-        Zbigniew W. Ras and Alicja Wieczorkowska (Editors), Springer, 2010.
-
-        [2] Esposito, R. and Radicioni, D. P., CarpeDiem: Optimizing the Viterbi
-        Algorithm and Applications to Supervised Sequential Learning, Journal
-        of Machine Learning Research, 10(Aug):1851-1880, 2009.
-        """
-        dataset = BachClassDataset(root,
-                                   meta_train=meta_train,
-                                   meta_val=meta_val,
-                                   meta_test=meta_test,
-                                   meta_split=meta_split,
-                                   transform=transform,
-                                   class_augmentations=class_augmentations,
-                                   download=download,
-                                   process_features=process_features,
-                                   min_num_samples_per_class=min_num_samples_per_class)
-        super(Bach, self).__init__(dataset,
-                                   num_classes_per_task,
-                                   target_transform=target_transform,
-                                   dataset_transform=dataset_transform)
-
-
-class BachClassDataset(ClassDataset):
-
-    open_ml_id = 4552
-    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
-    dataset_name = "bach"
-
-    folder = "bach"
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-    filename_meta_data = 'meta_data.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
-                 class_augmentations=None, download=False, process_features=True, min_num_samples_per_class=None):
-        super(BachClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
-                                               meta_split=meta_split, class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
-        self.split_filename_meta_data = os.path.join(self.root, self.filename_meta_data)
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        self._meta_data = None
-        self._lower_upper = None
-        self._categories = None
-
-        if download:
-            self.download(process_features, min_num_samples_per_class)
-
-        if min_num_samples_per_class != self.meta_data["min_num_data_per_class"]:
-            raise ValueError("min_num_samples_per_class given ({0}) does not match existing value"
-                             "({1}).".format(min_num_samples_per_class, self.meta_data["min_num_data_per_class"]))
-
-        if not self._check_integrity():
-            raise RuntimeError('Bach integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-        return BachDataset(index, data, label, transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    @property
-    def meta_data(self):
-        if self._meta_data is None:
-            with open(self.split_filename_meta_data, 'r') as f:
-                self._meta_data = json.load(f)
-        return self._meta_data
-
-    @property
-    def lower_upper(self):
-        if self._lower_upper is None:
-            self._lower_upper = {"lower": self.meta_data["lower"],
-                                 "upper": self.meta_data["upper"],
-                                 "feature_names_numerical":  self.meta_data["feature_names_numerical"]}
-        return self._lower_upper
-
-    @property
-    def categories(self):
-        if self._categories is None:
-            self._categories = {"categories": self.meta_data["categories"],
-                                "feature_names_categorical": self.meta_data["feature_names_categorical"]}
-        return self._categories
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data is not None:
-            self._data.close()
-            self._data = None
-
-    def download(self, process_features, min_num_samples_per_class):
-
-        if self._check_integrity():
-            return
-
-        from sklearn.datasets import fetch_openml
-
-        data = fetch_openml(data_id=self.open_ml_id)
-        features = data.data
-        targets = data.target
-        feature_names = np.array(data.feature_names)
-
-        # drop V1 and V2. V1 is the index of the choral, and V2 is the event number: index
-        # (starting from 1) of the event inside the chorale.
-        features_to_drop = np.array(['V1', 'V2'])
-        idx_drop = [np.where(feature_names == v)[0][0] for v in features_to_drop]
-        idx_keep = np.array([True] * feature_names.shape[0])
-        for i in idx_drop:
-            idx_keep[i] = False
-
-        features = features[:, idx_keep]
-        feature_names = feature_names[idx_keep]
-
-        # get categorical feature names
-        feature_names_cat = []
-        for v in feature_names:
-            if v in data.categories.keys():
-                feature_names_cat.append(v)
-        feature_names_cat = np.array(feature_names_cat)
-
-        # get numerical feature names
-        feature_names_num = []
-        for fname in feature_names:
-            if fname not in feature_names_cat:
-                feature_names_num.append(fname)
-        feature_names_num = np.array(feature_names_num)
-
-        assert feature_names_num.shape[0] + feature_names_cat.shape[0] == len(feature_names)
-
-        is_categorical = np.array([feature_name in feature_names_cat for feature_name in feature_names])
-        is_numerical = np.array([feature_name in feature_names_num for feature_name in feature_names])
-
-        # get categories
-        categories = []
-        for i in range(feature_names_cat.shape[0]):
-            categories_i = np.unique(features[:, is_categorical][:, i])
-            categories.append(categories_i.tolist())
-
-        if process_features:
-            from sklearn.preprocessing import OneHotEncoder
-            ohe = OneHotEncoder(categories=categories, sparse=False, dtype=np.float)
-
-        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
-        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
-        for s, split in enumerate(['train', 'val', 'test']):
-            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
-
-            is_in_split = [t in targets_assets_split for t in targets]
-            features_split = features[is_in_split, :]
-            targets_split = targets[is_in_split]
-            assert targets_split.shape[0] == features_split.shape[0]
-
-            unique_targets_split = np.unique(targets_split)
-
-            # first we check how many data-points are associated with each class. If it is less than the threshold,
-            # min_num_samples_per_class, then we discard the whole class.
-            num_dat_per_class = []
-            for label in unique_targets_split:
-                num_dat_per_class.append(features_split[targets_split == label, :].shape[0])
-            num_dat_per_class = np.array(num_dat_per_class)
-
-            # remove labels which have less data-points associate with them than the threshold min_num_data_per_class.
-            classes_to_keep = num_dat_per_class >= min_num_samples_per_class
-            unique_targets_with_enough_data_split = unique_targets_split[classes_to_keep]
-
-            if unique_targets_with_enough_data_split.shape[0] < unique_targets_split.shape[0]:
-                print("split: ({2}): number of unique targets with enough data ({0}) is smaller than "
-                      "number of unique targets in assets ({1})".format(
-                    unique_targets_with_enough_data_split.shape[0], unique_targets_split.shape[0], split))
-
-            # write unique targets to json file.
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(unique_targets_with_enough_data_split.tolist(), f)
-
-            # get pre-processing stats from the meta-train split
-            if split == 'train':
-                # numerical features
-                lower, upper = np.zeros(features.shape[1]), np.ones(features.shape[1])
-                if process_features:
-                    # lower upper
-                    lower = np.min(features[:, is_numerical], axis=0)
-                    upper = np.max(features[:, is_numerical], axis=0)
-                self._lower_upper = {'lower': lower.tolist(), 'upper': upper.tolist(),
-                                     'features_names': feature_names_num.tolist()}
-
-            # apply pre-processing of features
-            if process_features:
-                features_split_num = np.true_divide((features_split[:, is_numerical] - lower), (upper - lower))
-                features_split_cat = ohe.fit_transform(features_split[:, is_categorical])
-                features_split = np.hstack([features_split_num, features_split_cat])
-
-            # write data (features and class labels)
-            filename = os.path.join(self.root, self.filename.format(split))
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-
-                for i, label in enumerate(tqdm(unique_targets_with_enough_data_split, desc=filename)):
-                    data_class = features_split[targets_split == label, :]
-                    group.create_dataset(label, data=data_class)
-
-        # store meta-data of the dataset (not the meta-dataset).
-        # Extend this dictionary if you want to store more meta-data of the meta-dataset.
-        meta_data = {"min_num_data_per_class": min_num_samples_per_class,
-                     "lower": lower.tolist(),
-                     "upper": upper.tolist(),
-                     "feature_names_numerical": feature_names_num.tolist(),
-                     "feature_names_categorical": feature_names_cat.tolist(),
-                     "categories": categories,
-                     "dropped_features": features_to_drop.tolist()}
-
-        with open(self.split_filename_meta_data, 'w') as f:
-            json.dump(meta_data, f)
-
-
-class BachDataset(Dataset):
-    def __init__(self, index, data, label, transform=None, target_transform=None):
-        super(BachDataset, self).__init__(index, transform=transform, target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        features = self.data[index, :]
-        target = self.label
-
-        if self.transform is not None:
-            features = self.transform(features)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return features, target
-
-
-def create_asset(root='data', fractions=None, seed=42):
-    """This methods creates the assets of the Bach dataset. These are the meta-dataset splits from the
-    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
-    this directory: torchmeta.datasets.assets.bach. You can also manually change the assets."""
-
-    # split fractions: train, valid, test
-    if fractions is None:
-        fractions = [0.6, 0.2, 0.2]
-    assert sum(fractions) == 1
-
-    from sklearn.datasets import fetch_openml
-
-    data = fetch_openml(data_id=BachClassDataset.open_ml_id)
-    unique_targets = np.unique(data.target)
-    num_unique_targets = len(unique_targets)
-
-    num_split = [int(f * num_unique_targets) for f in fractions]
-    num_split[2] = num_unique_targets - num_split[0] - num_split[1]
-    assert sum(num_split) == num_unique_targets
-
-    # split unique labels randomly
-    np.random.seed(seed)
-    perm = np.random.permutation(num_unique_targets)
-    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
-                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
-                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
-
-    # write splits
-    root_path = os.path.join(os.path.expanduser(root), BachClassDataset.folder)
-    for split in ["train", "val", "test"]:
-        asset_filename = os.path.join(root_path, "{0}.json".format(split))
-        with open(asset_filename, 'w') as f:
-            json.dump(targets_split[split], f)
-
+import numpy as np
+import os
+import json
+import h5py
+from tqdm import tqdm
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class Bach(CombinationMetaDataset):
+    """The Bach dataset """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False, process_features=True, min_num_samples_per_class=1):
+        """
+        Bach Choral Harmony dataset [1], [2]
+        open-ml-id: 4552
+        https://archive.ics.uci.edu/ml/datasets/Bach+Choral+Harmony
+
+        Abstract: The data set is composed of 60 chorales (5665 events) by
+        J.S. Bach (1675-1750). Each event of each chorale is labelled using 1
+        among 101 chord labels and described through 14 features.
+
+        Data Set Information:
+
+        Pitch classes information has been extracted from MIDI sources downloaded
+        from (JSB Chorales)[http://www.jsbchorales.net/]. Meter information has
+        been computed through the Meter program which is part of the Melisma
+        music analyser (Melisma)[http://www.link.cs.cmu.edu/music-analysis/].
+        Chord labels have been manually annotated by a human expert.
+
+        Attribute Information:
+
+        1. Choral ID: corresponding to the file names from (Bach Central)[http://www.bachcentral.com/].
+        2. Event number: index (starting from 1) of the event inside the chorale.
+        3-14. Pitch classes: YES/NO depending on whether a given pitch is present.
+        Pitch classes/attribute correspondence is as follows:
+        C -> 3
+        C#/Db -> 4
+        D -> 5
+        ...
+        B -> 14
+        15. Bass: Pitch class of the bass note
+        16. Meter: integers from 1 to 5. Lower numbers denote less accented events,
+        higher numbers denote more accented events.
+        17. Chord label: Chord resonating during the given event.
+
+        Notes
+        ----------
+
+        The features V1 and V2 are dropped during the processing. V1 is the Choral ID. V2 is
+        the event number of the event inside the chorale.
+
+        Parameters
+        ----------
+        root : string
+            Root directory where the dataset folder `bach` exists.
+
+        num_classes_per_task : int
+            Number of classes per tasks. This corresponds to "N" in "N-way"
+            classification.
+
+        meta_train : bool (default: `False`)
+            Use the meta-train split of the dataset. If set to `True`, then the
+            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
+            of these three arguments must be set to `True`.
+
+        meta_val : bool (default: `False`)
+            Use the meta-validation split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_test : bool (default: `False`)
+            Use the meta-test split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_split : string in {'train', 'val', 'test'}, optional
+            Name of the split to use. This overrides the arguments `meta_train`,
+            `meta_val` and `meta_test` if all three are set to `False`.
+
+        transform : callable, optional
+            A function/transform that takes a numpy array or a pytorch array
+            (depending when the transforms is applied), and returns a transformed
+            version.
+
+        target_transform : callable, optional
+            A function/transform that takes a target, and returns a transformed
+            version.
+
+        dataset_transform : callable, optional
+            A function/transform that takes a dataset (ie. a task), and returns a
+            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+        class_augmentations : list of callable, optional
+            A list of functions that augment the dataset with new classes. These
+            classes are transformations of existing classes.
+
+        download : bool (default: `False`)
+            If `True`, downloads the original files and processes the dataset in the
+            root directory (under the `bach' folder). If the dataset
+            is already available, this does not download/process the dataset again.
+
+        process_features : bool (default: `True`)
+            If `True`, normalizes the numeric feature f according to (f-lower) / (upper - lower) where upper
+            and lower are the min and max values of feature f of the meta-train dataset.
+            And also one-hot encodes the categorical features.
+
+        min_num_samples_per_class : int (default: 1)
+            Minimal number of samples per class that need to be present for the class to be used.
+
+        References
+        -----
+
+        [1] D. P. Radicioni and R. Esposito. Advances in Music Information Retrieval,
+        chapter BREVE: an HMPerceptron-Based Chord Recognition System.
+        Studies in Computational Intelligence,
+        Zbigniew W. Ras and Alicja Wieczorkowska (Editors), Springer, 2010.
+
+        [2] Esposito, R. and Radicioni, D. P., CarpeDiem: Optimizing the Viterbi
+        Algorithm and Applications to Supervised Sequential Learning, Journal
+        of Machine Learning Research, 10(Aug):1851-1880, 2009.
+        """
+        dataset = BachClassDataset(root,
+                                   meta_train=meta_train,
+                                   meta_val=meta_val,
+                                   meta_test=meta_test,
+                                   meta_split=meta_split,
+                                   transform=transform,
+                                   class_augmentations=class_augmentations,
+                                   download=download,
+                                   process_features=process_features,
+                                   min_num_samples_per_class=min_num_samples_per_class)
+        super(Bach, self).__init__(dataset,
+                                   num_classes_per_task,
+                                   target_transform=target_transform,
+                                   dataset_transform=dataset_transform)
+
+
+class BachClassDataset(ClassDataset):
+
+    open_ml_id = 4552
+    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
+    dataset_name = "bach"
+
+    folder = "bach"
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+    filename_meta_data = 'meta_data.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
+                 class_augmentations=None, download=False, process_features=True, min_num_samples_per_class=None):
+        super(BachClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
+                                               meta_split=meta_split, class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
+        self.split_filename_meta_data = os.path.join(self.root, self.filename_meta_data)
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+
+        self._meta_data = None
+        self._lower_upper = None
+        self._categories = None
+
+        if download:
+            self.download(process_features, min_num_samples_per_class)
+
+        if min_num_samples_per_class != self.meta_data["min_num_data_per_class"]:
+            raise ValueError("min_num_samples_per_class given ({0}) does not match existing value"
+                             "({1}).".format(min_num_samples_per_class, self.meta_data["min_num_data_per_class"]))
+
+        if not self._check_integrity():
+            raise RuntimeError('Bach integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+        return BachDataset(index, data, label, transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    @property
+    def meta_data(self):
+        if self._meta_data is None:
+            with open(self.split_filename_meta_data, 'r') as f:
+                self._meta_data = json.load(f)
+        return self._meta_data
+
+    @property
+    def lower_upper(self):
+        if self._lower_upper is None:
+            self._lower_upper = {"lower": self.meta_data["lower"],
+                                 "upper": self.meta_data["upper"],
+                                 "feature_names_numerical":  self.meta_data["feature_names_numerical"]}
+        return self._lower_upper
+
+    @property
+    def categories(self):
+        if self._categories is None:
+            self._categories = {"categories": self.meta_data["categories"],
+                                "feature_names_categorical": self.meta_data["feature_names_categorical"]}
+        return self._categories
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data is not None:
+            self._data.close()
+            self._data = None
+
+    def download(self, process_features, min_num_samples_per_class):
+
+        if self._check_integrity():
+            return
+
+        from sklearn.datasets import fetch_openml
+
+        data = fetch_openml(data_id=self.open_ml_id)
+        features = data.data
+        targets = data.target
+        feature_names = np.array(data.feature_names)
+
+        # drop V1 and V2. V1 is the index of the choral, and V2 is the event number: index
+        # (starting from 1) of the event inside the chorale.
+        features_to_drop = np.array(['V1', 'V2'])
+        idx_drop = [np.where(feature_names == v)[0][0] for v in features_to_drop]
+        idx_keep = np.array([True] * feature_names.shape[0])
+        for i in idx_drop:
+            idx_keep[i] = False
+
+        features = features[:, idx_keep]
+        feature_names = feature_names[idx_keep]
+
+        # get categorical feature names
+        feature_names_cat = []
+        for v in feature_names:
+            if v in data.categories.keys():
+                feature_names_cat.append(v)
+        feature_names_cat = np.array(feature_names_cat)
+
+        # get numerical feature names
+        feature_names_num = []
+        for fname in feature_names:
+            if fname not in feature_names_cat:
+                feature_names_num.append(fname)
+        feature_names_num = np.array(feature_names_num)
+
+        assert feature_names_num.shape[0] + feature_names_cat.shape[0] == len(feature_names)
+
+        is_categorical = np.array([feature_name in feature_names_cat for feature_name in feature_names])
+        is_numerical = np.array([feature_name in feature_names_num for feature_name in feature_names])
+
+        # get categories
+        categories = []
+        for i in range(feature_names_cat.shape[0]):
+            categories_i = np.unique(features[:, is_categorical][:, i])
+            categories.append(categories_i.tolist())
+
+        if process_features:
+            from sklearn.preprocessing import OneHotEncoder
+            ohe = OneHotEncoder(categories=categories, sparse=False, dtype=np.float)
+
+        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
+        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
+        for s, split in enumerate(['train', 'val', 'test']):
+            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
+
+            is_in_split = [t in targets_assets_split for t in targets]
+            features_split = features[is_in_split, :]
+            targets_split = targets[is_in_split]
+            assert targets_split.shape[0] == features_split.shape[0]
+
+            unique_targets_split = np.unique(targets_split)
+
+            # first we check how many data-points are associated with each class. If it is less than the threshold,
+            # min_num_samples_per_class, then we discard the whole class.
+            num_dat_per_class = []
+            for label in unique_targets_split:
+                num_dat_per_class.append(features_split[targets_split == label, :].shape[0])
+            num_dat_per_class = np.array(num_dat_per_class)
+
+            # remove labels which have less data-points associate with them than the threshold min_num_data_per_class.
+            classes_to_keep = num_dat_per_class >= min_num_samples_per_class
+            unique_targets_with_enough_data_split = unique_targets_split[classes_to_keep]
+
+            if unique_targets_with_enough_data_split.shape[0] < unique_targets_split.shape[0]:
+                print("split: ({2}): number of unique targets with enough data ({0}) is smaller than "
+                      "number of unique targets in assets ({1})".format(
+                    unique_targets_with_enough_data_split.shape[0], unique_targets_split.shape[0], split))
+
+            # write unique targets to json file.
+            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(unique_targets_with_enough_data_split.tolist(), f)
+
+            # get pre-processing stats from the meta-train split
+            if split == 'train':
+                # numerical features
+                lower, upper = np.zeros(features.shape[1]), np.ones(features.shape[1])
+                if process_features:
+                    # lower upper
+                    lower = np.min(features[:, is_numerical], axis=0)
+                    upper = np.max(features[:, is_numerical], axis=0)
+                self._lower_upper = {'lower': lower.tolist(), 'upper': upper.tolist(),
+                                     'features_names': feature_names_num.tolist()}
+
+            # apply pre-processing of features
+            if process_features:
+                features_split_num = np.true_divide((features_split[:, is_numerical] - lower), (upper - lower))
+                features_split_cat = ohe.fit_transform(features_split[:, is_categorical])
+                features_split = np.hstack([features_split_num, features_split_cat])
+
+            # write data (features and class labels)
+            filename = os.path.join(self.root, self.filename.format(split))
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+
+                for i, label in enumerate(tqdm(unique_targets_with_enough_data_split, desc=filename)):
+                    data_class = features_split[targets_split == label, :]
+                    group.create_dataset(label, data=data_class)
+
+        # store meta-data of the dataset (not the meta-dataset).
+        # Extend this dictionary if you want to store more meta-data of the meta-dataset.
+        meta_data = {"min_num_data_per_class": min_num_samples_per_class,
+                     "lower": lower.tolist(),
+                     "upper": upper.tolist(),
+                     "feature_names_numerical": feature_names_num.tolist(),
+                     "feature_names_categorical": feature_names_cat.tolist(),
+                     "categories": categories,
+                     "dropped_features": features_to_drop.tolist()}
+
+        with open(self.split_filename_meta_data, 'w') as f:
+            json.dump(meta_data, f)
+
+
+class BachDataset(Dataset):
+    def __init__(self, index, data, label, transform=None, target_transform=None):
+        super(BachDataset, self).__init__(index, transform=transform, target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        features = self.data[index, :]
+        target = self.label
+
+        if self.transform is not None:
+            features = self.transform(features)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return features, target
+
+
+def create_asset(root='data', fractions=None, seed=42):
+    """This methods creates the assets of the Bach dataset. These are the meta-dataset splits from the
+    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
+    this directory: torchmeta.datasets.assets.bach. You can also manually change the assets."""
+
+    # split fractions: train, valid, test
+    if fractions is None:
+        fractions = [0.6, 0.2, 0.2]
+    assert sum(fractions) == 1
+
+    from sklearn.datasets import fetch_openml
+
+    data = fetch_openml(data_id=BachClassDataset.open_ml_id)
+    unique_targets = np.unique(data.target)
+    num_unique_targets = len(unique_targets)
+
+    num_split = [int(f * num_unique_targets) for f in fractions]
+    num_split[2] = num_unique_targets - num_split[0] - num_split[1]
+    assert sum(num_split) == num_unique_targets
+
+    # split unique labels randomly
+    np.random.seed(seed)
+    perm = np.random.permutation(num_unique_targets)
+    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
+                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
+                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
+
+    # write splits
+    root_path = os.path.join(os.path.expanduser(root), BachClassDataset.folder)
+    for split in ["train", "val", "test"]:
+        asset_filename = os.path.join(root_path, "{0}.json".format(split))
+        with open(asset_filename, 'w') as f:
+            json.dump(targets_split[split], f)
+
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-import os
-import json
-
-from lightningdata.thirdparty.torchmeta.datasets.cifar100.base import CIFAR100ClassDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-from lightningdata.thirdparty.torchmeta.utils.data import ClassDataset, CombinationMetaDataset
-
-
-class CIFARFS(CombinationMetaDataset):
-    """
-    The CIFAR-FS dataset, introduced in [1]. This dataset contains
-    images of 100 different classes from the CIFAR100 dataset [2].
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `cifar100` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to `N` in `N-way` 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the root 
-        directory (under the `cifar100` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The meta train/validation/test splits are over 64/16/20 classes from the
-    CIFAR100 dataset.
-
-    References
-    ----------
-    .. [1] Bertinetto L., Henriques J. F., Torr P. H.S., Vedaldi A. (2019).
-           Meta-learning with differentiable closed-form solvers. In International
-           Conference on Learning Representations (https://arxiv.org/abs/1805.08136)
-
-    .. [2] Krizhevsky A. (2009). Learning Multiple Layers of Features from Tiny
-           Images. (https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf)
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = CIFARFSClassDataset(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-        super(CIFARFS, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-
-class CIFARFSClassDataset(CIFAR100ClassDataset):
-    subfolder = 'cifar-fs'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(CIFARFSClassDataset, self).__init__(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-
-    def download(self):
-        if self._check_integrity():
-            return
-        super(CIFARFSClassDataset, self).download()
-
-        subfolder = os.path.join(self.root, self.subfolder)
-        if not os.path.exists(subfolder):
-            os.makedirs(subfolder)
-
-        for split in ['train', 'val', 'test']:
-            split_filename_labels = os.path.join(subfolder,
-                self.filename_labels.format(split))
-            if os.path.isfile(split_filename_labels):
-                continue
-
-            data = get_asset(self.folder, self.subfolder,
-                '{0}.json'.format(split), dtype='json')
-            with open(split_filename_labels, 'w') as f:
-                json.dump(data, f)
+import os
+import json
+
+from lightningdata.thirdparty.torchmeta.datasets.cifar100.base import CIFAR100ClassDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+from lightningdata.thirdparty.torchmeta.utils.data import ClassDataset, CombinationMetaDataset
+
+
+class CIFARFS(CombinationMetaDataset):
+    """
+    The CIFAR-FS dataset, introduced in [1]. This dataset contains
+    images of 100 different classes from the CIFAR100 dataset [2].
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `cifar100` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to `N` in `N-way` 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the root 
+        directory (under the `cifar100` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The meta train/validation/test splits are over 64/16/20 classes from the
+    CIFAR100 dataset.
+
+    References
+    ----------
+    .. [1] Bertinetto L., Henriques J. F., Torr P. H.S., Vedaldi A. (2019).
+           Meta-learning with differentiable closed-form solvers. In International
+           Conference on Learning Representations (https://arxiv.org/abs/1805.08136)
+
+    .. [2] Krizhevsky A. (2009). Learning Multiple Layers of Features from Tiny
+           Images. (https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf)
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = CIFARFSClassDataset(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+        super(CIFARFS, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+
+class CIFARFSClassDataset(CIFAR100ClassDataset):
+    subfolder = 'cifar-fs'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(CIFARFSClassDataset, self).__init__(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+
+    def download(self):
+        if self._check_integrity():
+            return
+        super(CIFARFSClassDataset, self).download()
+
+        subfolder = os.path.join(self.root, self.subfolder)
+        if not os.path.exists(subfolder):
+            os.makedirs(subfolder)
+
+        for split in ['train', 'val', 'test']:
+            split_filename_labels = os.path.join(subfolder,
+                self.filename_labels.format(split))
+            if os.path.isfile(split_filename_labels):
+                continue
+
+            data = get_asset(self.folder, self.subfolder,
+                '{0}.json'.format(split), dtype='json')
+            with open(split_filename_labels, 'w') as f:
+                json.dump(data, f)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import os
-import json
-
-from lightningdata.thirdparty.torchmeta.datasets.cifar100.base import CIFAR100ClassDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-from lightningdata.thirdparty.torchmeta.utils.data import ClassDataset, CombinationMetaDataset
-
-
-class FC100(CombinationMetaDataset):
-    """
-    The Fewshot-CIFAR100 dataset, introduced in [1]. This dataset contains
-    images of 100 different classes from the CIFAR100 dataset [2].
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `cifar100` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to `N` in `N-way` 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the root 
-        directory (under the `cifar100` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The meta train/validation/test splits are over 12/4/4 superclasses from the
-    CIFAR100 dataset. The meta train/validation/test splits contain 60/20/20
-    classes.
-
-    References
-    ----------
-    .. [1] Oreshkin B. N., Rodriguez P., Lacoste A. (2018). TADAM: Task dependent
-           adaptive metric for improved few-shot learning. In Advances in Neural 
-           Information Processing Systems (https://arxiv.org/abs/1805.10123)
-
-    .. [2] Krizhevsky A. (2009). Learning Multiple Layers of Features from Tiny
-           Images. (https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf)
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = FC100ClassDataset(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-        super(FC100, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-
-class FC100ClassDataset(CIFAR100ClassDataset):
-    subfolder = 'fc100'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(FC100ClassDataset, self).__init__(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-
-    def download(self):
-        if self._check_integrity():
-            return
-        super(FC100ClassDataset, self).download()
-
-        subfolder = os.path.join(self.root, self.subfolder)
-        if not os.path.exists(subfolder):
-            os.makedirs(subfolder)
-
-        filename_fine_names = os.path.join(self.root, self.filename_fine_names)
-        with open(filename_fine_names, 'r') as f:
-            fine_names = json.load(f)
-
-        for split in ['train', 'val', 'test']:
-            split_filename_labels = os.path.join(subfolder,
-                self.filename_labels.format(split))
-            if os.path.isfile(split_filename_labels):
-                continue
-
-            data = get_asset(self.folder, self.subfolder,
-                '{0}.json'.format(split), dtype='json')
-            with open(split_filename_labels, 'w') as f:
-                labels = [[coarse_name, fine_name] for coarse_name in data
-                    for fine_name in fine_names[coarse_name]]
-                json.dump(labels, f)
+import os
+import json
+
+from lightningdata.thirdparty.torchmeta.datasets.cifar100.base import CIFAR100ClassDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+from lightningdata.thirdparty.torchmeta.utils.data import ClassDataset, CombinationMetaDataset
+
+
+class FC100(CombinationMetaDataset):
+    """
+    The Fewshot-CIFAR100 dataset, introduced in [1]. This dataset contains
+    images of 100 different classes from the CIFAR100 dataset [2].
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `cifar100` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to `N` in `N-way` 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the root 
+        directory (under the `cifar100` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The meta train/validation/test splits are over 12/4/4 superclasses from the
+    CIFAR100 dataset. The meta train/validation/test splits contain 60/20/20
+    classes.
+
+    References
+    ----------
+    .. [1] Oreshkin B. N., Rodriguez P., Lacoste A. (2018). TADAM: Task dependent
+           adaptive metric for improved few-shot learning. In Advances in Neural 
+           Information Processing Systems (https://arxiv.org/abs/1805.10123)
+
+    .. [2] Krizhevsky A. (2009). Learning Multiple Layers of Features from Tiny
+           Images. (https://www.cs.toronto.edu/~kriz/learning-features-2009-TR.pdf)
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = FC100ClassDataset(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+        super(FC100, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+
+class FC100ClassDataset(CIFAR100ClassDataset):
+    subfolder = 'fc100'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(FC100ClassDataset, self).__init__(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+
+    def download(self):
+        if self._check_integrity():
+            return
+        super(FC100ClassDataset, self).download()
+
+        subfolder = os.path.join(self.root, self.subfolder)
+        if not os.path.exists(subfolder):
+            os.makedirs(subfolder)
+
+        filename_fine_names = os.path.join(self.root, self.filename_fine_names)
+        with open(filename_fine_names, 'r') as f:
+            fine_names = json.load(f)
+
+        for split in ['train', 'val', 'test']:
+            split_filename_labels = os.path.join(subfolder,
+                self.filename_labels.format(split))
+            if os.path.isfile(split_filename_labels):
+                continue
+
+            data = get_asset(self.folder, self.subfolder,
+                '{0}.json'.format(split), dtype='json')
+            with open(split_filename_labels, 'w') as f:
+                labels = [[coarse_name, fine_name] for coarse_name in data
+                    for fine_name in fine_names[coarse_name]]
+                json.dump(labels, f)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/cub.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,244 +1,253 @@
-import numpy as np
-from PIL import Image
-import os
-import io
-import json
-import glob
-import h5py
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-# QKFIX: See torchmeta.datasets.utils for more informations
-from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class CUB(CombinationMetaDataset):
-    """
-    The Caltech-UCSD Birds dataset, introduced in [1]. This dataset is based on
-    images from 200 species of birds from the Caltech-UCSD Birds dataset [2].
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `cub` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way" 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the root 
-        directory (under the `cub` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The dataset is downloaded from [2]. The dataset contains images from 200
-    classes. The meta train/validation/test splits are over 100/50/50 classes.
-    The splits are taken from [3] ([code](https://github.com/wyharveychen/CloserLookFewShot)
-    for reproducibility).
-
-    References
-    ----------
-    .. [1] Hilliard, N., Phillips, L., Howland, S., Yankov, A., Corley, C. D.,
-           Hodas, N. O. (2018). Few-Shot Learning with Metric-Agnostic Conditional
-           Embeddings. (https://arxiv.org/abs/1802.04376)
-    .. [2] Wah, C., Branson, S., Welinder, P., Perona, P., Belongie, S. (2011).
-           The Caltech-UCSD Birds-200-2011 Dataset
-           (http://www.vision.caltech.edu/visipedia/CUB-200-2011.html)
-    .. [3] Chen, W., Liu, Y. and Kira, Z. and Wang, Y. and  Huang, J. (2019).
-           A Closer Look at Few-shot Classification. International Conference on
-           Learning Representations (https://openreview.net/forum?id=HkxLXnAcFQ)
-
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = CUBClassDataset(root, meta_train=meta_train, meta_val=meta_val,
-            meta_test=meta_test, meta_split=meta_split, transform=transform,
-            class_augmentations=class_augmentations, download=download)
-        super(CUB, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-
-class CUBClassDataset(ClassDataset):
-    folder = 'cub'
-    # # Google Drive ID from http://www.vision.caltech.edu/visipedia-data/CUB-200-2011/CUB_200_2011.tgz
-    gdrive_id = '1hbzc_P1FuxMkcabkgn9ZKinBwW683j45'
-    tgz_filename = 'CUB_200_2011.tgz'
-    tgz_md5 = '97eceeb196236b17998738112f37df78'
-    image_folder = 'CUB_200_2011/images'
-
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(CUBClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root,
-            self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root,
-            self.filename_labels.format(self.meta_split))
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('CUB integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return CUBDataset(index, data, label, transform=transform,
-                          target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-    
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data_file is not None:
-            self._data_file.close()
-            self._data_file = None
-            self._data = None
-
-    def download(self):
-        import tarfile
-        import shutil
-        import glob
-        from tqdm import tqdm
-
-        if self._check_integrity():
-            return
-
-        download_file_from_google_drive(self.gdrive_id, self.root,
-            self.tgz_filename, md5=self.tgz_md5)
-
-        tgz_filename = os.path.join(self.root, self.tgz_filename)
-        with tarfile.open(tgz_filename, 'r') as f:
-            f.extractall(self.root)
-        image_folder = os.path.join(self.root, self.image_folder)
-
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename.format(split))
-            if os.path.isfile(filename):
-                continue
-
-            labels = get_asset(self.folder, '{0}.json'.format(split))
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(labels, f)
-
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-                dtype = h5py.special_dtype(vlen=np.uint8)
-                for i, label in enumerate(tqdm(labels, desc=filename)):
-                    images = glob.glob(os.path.join(image_folder, label, '*.jpg'))
-                    images.sort()
-                    dataset = group.create_dataset(label, (len(images),), dtype=dtype)
-                    for i, image in enumerate(images):
-                        with open(image, 'rb') as f:
-                            array = bytearray(f.read())
-                            dataset[i] = np.asarray(array, dtype=np.uint8)
-
-        tar_folder, _ = os.path.splitext(tgz_filename)
-        if os.path.isdir(tar_folder):
-            shutil.rmtree(tar_folder)
-
-        attributes_filename = os.path.join(self.root, 'attributes.txt')
-        if os.path.isfile(attributes_filename):
-            os.remove(attributes_filename)
-
-
-class CUBDataset(Dataset):
-    def __init__(self, index, data, label,
-                 transform=None, target_transform=None):
-        super(CUBDataset, self).__init__(index, transform=transform,
-                                         target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        image = Image.open(io.BytesIO(self.data[index])).convert('RGB')
-        target = self.label
-
-        if self.transform is not None:
-            image = self.transform(image)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (image, target)
+import numpy as np
+from PIL import Image
+import os
+import io
+import json
+import glob
+import h5py
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+# QKFIX: See torchmeta.datasets.utils for more informations
+from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class TripleMNIST(CombinationMetaDataset):
+    """
+    The Triple MNIST dataset, introduced in [1]. This dataset is based on
+    the MNIST dataset [2]. It consists of sampled images from MNIST
+    that are put together to create images with multiple digits. It contains
+    1,000,000 images from 1000 different classes (1000 images per class, for 
+    the numbers 000 to 999).
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `triplemnist` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way" 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+        one of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+        one of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These
+        classes are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the
+        root directory (under the `triplemnist` folder). If the dataset is
+        already available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The dataset is downloaded from the Multi-digit MNIST repository
+    [1](https://github.com/shaohua0116/MultiDigitMNIST). The dataset contains
+    images (MNIST triple digits) from 1000 classes, for the numbers 000 to 999.
+    The meta train/validation/test splits are 640/160/200 classes.
+    The splits are taken from [1].
+
+    References
+    ----------
+    .. [1] Sun, S. (2019). Multi-digit MNIST for Few-shot Learning.
+    (https://github.com/shaohua0116/MultiDigitMNIST)
+
+    .. [2] LeCun, Y., Cortes, C., and Burges, CJ. (2010). MNIST Handwritten
+    Digit Database. (http://yann.lecun.com/exdb/mnist)
+
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = TripleMNISTClassDataset(root,
+            meta_train=meta_train, meta_val=meta_val,
+            meta_test=meta_test, meta_split=meta_split, transform=transform,
+            class_augmentations=class_augmentations, download=download)
+        super(TripleMNIST, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform,
+            dataset_transform=dataset_transform)
+
+
+class TripleMNISTClassDataset(ClassDataset):
+    folder = 'triplemnist'
+    # Google Drive ID from https://github.com/shaohua0116/MultiDigitMNIST
+    gdrive_id = '1xqyW289seXYaDSqD2jaBPMKVAAjPP9ee'
+    zip_filename = 'triple_mnist_seed_123_image_size_84_84.zip'
+    zip_md5 = '9508b047f9fbb834c02bc13ef44245da'
+
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+
+    image_folder = 'triple_mnist_seed_123_image_size_84_84'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(TripleMNISTClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root,
+            self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root,
+            self.filename_labels.format(self.meta_split))
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('Triple MNIST integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return TripleMNISTDataset(index, data, label, transform=transform,
+                                  target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+    
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data_file is not None:
+            self._data_file.close()
+            self._data_file = None
+            self._data = None
+
+    def download(self):
+        import zipfile
+        import shutil
+        import glob
+        from tqdm import tqdm
+
+        if self._check_integrity():
+            return
+
+        zip_filename = os.path.join(self.root, self.zip_filename)
+        if not os.path.isfile(zip_filename):
+            download_file_from_google_drive(self.gdrive_id, self.root,
+                self.zip_filename, md5=self.zip_md5)
+
+        zip_foldername = os.path.join(self.root, self.image_folder)
+        if not os.path.isdir(zip_foldername):
+            with zipfile.ZipFile(zip_filename, 'r') as f:
+                for member in tqdm(f.infolist(), desc='Extracting '):
+                    try:
+                        f.extract(member, self.root)
+                    except zipfile.BadZipFile:
+                        print('Error: Zip file is corrupted')
+
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename.format(split))
+            if os.path.isfile(filename):
+                continue
+
+            labels = get_asset(self.folder, '{0}.json'.format(split))
+            labels_filename = os.path.join(self.root,
+                                           self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(labels, f)
+
+            image_folder = os.path.join(zip_foldername, split)
+
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+                dtype = h5py.special_dtype(vlen=np.uint8)
+                for i, label in enumerate(tqdm(labels, desc=filename)):
+                    images = glob.glob(os.path.join(image_folder, label,
+                                                    '*.png'))
+                    images.sort()
+                    dataset = group.create_dataset(label, (len(images),),
+                                                   dtype=dtype)
+                    for i, image in enumerate(images):
+                        with open(image, 'rb') as f:
+                            array = bytearray(f.read())
+                            dataset[i] = np.asarray(array, dtype=np.uint8)
+
+        if os.path.isdir(zip_foldername):
+            shutil.rmtree(zip_foldername)
+
+
+class TripleMNISTDataset(Dataset):
+    def __init__(self, index, data, label,
+                 transform=None, target_transform=None):
+        super(TripleMNISTDataset, self).__init__(index, transform=transform,
+                                                 target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        image = Image.open(io.BytesIO(self.data[index])).convert('RGB')
+        target = self.label
+
+        if self.transform is not None:
+            image = self.transform(image)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (image, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/letter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,253 +1,265 @@
-import numpy as np
-from PIL import Image
-import os
-import io
-import json
-import glob
-import h5py
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-# QKFIX: See torchmeta.datasets.utils for more informations
-from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class DoubleMNIST(CombinationMetaDataset):
-    """
-    The Double MNIST dataset, introduced in [1]. This dataset is based on
-    the MNIST dataset [2]. It consists of sampled images from MNIST
-    that are put together to create images with multiple digits. It contains
-    100,000 images from 100 different classes (1000 images per class, for the 
-    numbers 00 to 99).
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `doublemnist` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way" 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-        one of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-        one of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These
-        classes are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the
-        root directory (under the `doublemnist` folder). If the dataset is
-        already available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The dataset is downloaded from the Multi-digit MNIST repository
-    [1](https://github.com/shaohua0116/MultiDigitMNIST). The dataset contains
-    images (MNIST double digits) from 100 classes, for the numbers 00 to 99.
-    The meta train/validation/test splits are 64/16/20 classes.
-    The splits are taken from [1].
-
-    References
-    ----------
-    .. [1] Sun, S. (2019). Multi-digit MNIST for Few-shot Learning.
-    (https://github.com/shaohua0116/MultiDigitMNIST)
-
-    .. [2] LeCun, Y., Cortes, C., and Burges, CJ. (2010). MNIST Handwritten
-    Digit Database. (http://yann.lecun.com/exdb/mnist)
-
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = DoubleMNISTClassDataset(root,
-            meta_train=meta_train, meta_val=meta_val,
-            meta_test=meta_test, meta_split=meta_split, transform=transform,
-            class_augmentations=class_augmentations, download=download)
-        super(DoubleMNIST, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform,
-            dataset_transform=dataset_transform)
-
-
-class DoubleMNISTClassDataset(ClassDataset):
-    folder = 'doublemnist'
-    # Google Drive ID from https://github.com/shaohua0116/MultiDigitMNIST
-    gdrive_id = '1MqQCdLt9TVE3joAMw4FwJp_B8F-htrAo'
-    zip_filename = 'double_mnist_seed_123_image_size_64_64.zip'
-    zip_md5 = '6d8b185c0cde155eb39d0e3615ab4f23'
-
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    image_folder = 'double_mnist_seed_123_image_size_64_64'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(DoubleMNISTClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root,
-            self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root,
-            self.filename_labels.format(self.meta_split))
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('Double MNIST integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return DoubleMNISTDataset(index, data, label, transform=transform,
-                                  target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-    
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data_file is not None:
-            self._data_file.close()
-            self._data_file = None
-            self._data = None
-
-    def download(self):
-        import zipfile
-        import shutil
-        import glob
-        from tqdm import tqdm
-
-        if self._check_integrity():
-            return
-
-        zip_filename = os.path.join(self.root, self.zip_filename)
-        if not os.path.isfile(zip_filename):
-            download_file_from_google_drive(self.gdrive_id, self.root,
-                self.zip_filename, md5=self.zip_md5)
-
-        zip_foldername = os.path.join(self.root, self.image_folder)
-        if not os.path.isdir(zip_foldername):
-            with zipfile.ZipFile(zip_filename, 'r') as f:
-                for member in tqdm(f.infolist(), desc='Extracting '):
-                    try:
-                        f.extract(member, self.root)
-                    except zipfile.BadZipFile:
-                        print('Error: Zip file is corrupted')
-
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename.format(split))
-            if os.path.isfile(filename):
-                continue
-
-            labels = get_asset(self.folder, '{0}.json'.format(split))
-            labels_filename = os.path.join(self.root,
-                                           self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(labels, f)
-
-            image_folder = os.path.join(zip_foldername, split)
-
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-                dtype = h5py.special_dtype(vlen=np.uint8)
-                for i, label in enumerate(tqdm(labels, desc=filename)):
-                    images = glob.glob(os.path.join(image_folder, label,
-                                                    '*.png'))
-                    images.sort()
-                    dataset = group.create_dataset(label, (len(images),),
-                                                   dtype=dtype)
-                    for i, image in enumerate(images):
-                        with open(image, 'rb') as f:
-                            array = bytearray(f.read())
-                            dataset[i] = np.asarray(array, dtype=np.uint8)
-
-        if os.path.isdir(zip_foldername):
-            shutil.rmtree(zip_foldername)
-
-
-class DoubleMNISTDataset(Dataset):
-    def __init__(self, index, data, label,
-                 transform=None, target_transform=None):
-        super(DoubleMNISTDataset, self).__init__(index, transform=transform,
-                                                 target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        image = Image.open(io.BytesIO(self.data[index])).convert('RGB')
-        target = self.label
-
-        if self.transform is not None:
-            image = self.transform(image)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (image, target)
+import numpy as np
+import os
+import json
+import h5py
+from tqdm import tqdm
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class Letter(CombinationMetaDataset):
+    """The Letter Image Recognition Dataset """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        """
+        Letter Image Recognition Data [1]:
+        open-ml-id: 6
+        https://archive.ics.uci.edu/ml/datasets/Letter+Recognition - 01-01-1991
+
+        The objective is to identify each of a large number of black-and-white
+        rectangular pixel displays as one of the 26 capital letters in the English
+        alphabet.  The character images were based on 20 different fonts and each
+        letter within these 20 fonts was randomly distorted to produce a file of
+        20,000 unique stimuli.  Each stimulus was converted into 16 primitive
+        numerical attributes (statistical moments and edge counts) which were then
+        scaled to fit into a range of integer values from 0 through 15.  We
+        typically train on the first 16000 items and then use the resulting model
+        to predict the letter category for the remaining 4000.  See the article
+        cited above for more details.
+
+        Parameters
+        ----------
+        root : string
+            Root directory where the dataset folder `letter` exists.
+
+        num_classes_per_task : int
+            Number of classes per tasks. This corresponds to "N" in "N-way"
+            classification.
+
+        meta_train : bool (default: `False`)
+            Use the meta-train split of the dataset. If set to `True`, then the
+            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
+            of these three arguments must be set to `True`.
+
+        meta_val : bool (default: `False`)
+            Use the meta-validation split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_test : bool (default: `False`)
+            Use the meta-test split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_split : string in {'train', 'val', 'test'}, optional
+            Name of the split to use. This overrides the arguments `meta_train`,
+            `meta_val` and `meta_test` if all three are set to `False`.
+
+        transform : callable, optional
+            A function/transform that takes a numpy array or a pytorch array
+            (depending when the transforms is applied), and returns a transformed
+            version.
+
+        target_transform : callable, optional
+            A function/transform that takes a target, and returns a transformed
+            version.
+
+        dataset_transform : callable, optional
+            A function/transform that takes a dataset (ie. a task), and returns a
+            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+        class_augmentations : list of callable, optional
+            A list of functions that augment the dataset with new classes. These
+            classes are transformations of existing classes.
+
+        download : bool (default: `False`)
+            If `True`, downloads the original files and processes the dataset in the
+            root directory (under the `letter` folder). If the dataset
+            is already available, this does not download/process the dataset again.
+
+        References
+        -----
+        [1] P. W. Frey and D. J. Slate. "Letter Recognition Using Holland-style
+        Adaptive Classifiers". Machine Learning 6(2), 1991
+        """
+        dataset = LetterClassDataset(root,
+                                     meta_train=meta_train,
+                                     meta_val=meta_val,
+                                     meta_test=meta_test,
+                                     meta_split=meta_split,
+                                     transform=transform,
+                                     class_augmentations=class_augmentations,
+                                     download=download)
+        super(Letter, self).__init__(dataset,
+                                     num_classes_per_task,
+                                     target_transform=target_transform,
+                                     dataset_transform=dataset_transform)
+
+
+class LetterClassDataset(ClassDataset):
+
+    open_ml_id = 6
+    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
+    dataset_name = "letter"
+
+    folder = "letter"
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
+                 class_augmentations=None, download=False):
+        super(LetterClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
+                                                 meta_split=meta_split, class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('Letter integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return LetterDataset(index, data, label, transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data is not None:
+            self._data.close()
+            self._data = None
+
+    def download(self):
+
+        if self._check_integrity():
+            return
+
+        from sklearn.datasets import fetch_openml
+
+        data = fetch_openml(data_id=self.open_ml_id)
+        features = data.data
+        targets = data.target
+
+        os.makedirs(self.root, exist_ok=True)
+
+        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
+        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
+        for s, split in enumerate(['train', 'val', 'test']):
+            labels_assets_split = get_asset(self.folder, '{0}.json'.format(split))
+
+            is_in_split = [t in labels_assets_split for t in targets]
+            features_split = features.loc[is_in_split]
+            targets_split = targets.loc[is_in_split]
+            assert targets_split.shape[0] == features_split.shape[0]
+
+            unique_targets_split = np.unique(targets_split)
+            if len(labels_assets_split) > unique_targets_split.shape[0]:
+                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
+                      f"given by assets ({len(labels_assets_split)}). Proceeding with unique set of labels.")
+
+            # write unique targets to json file.
+            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(unique_targets_split.tolist(), f)
+
+            # write data (features and class labels)
+            filename = os.path.join(self.root, self.filename.format(split))
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+
+                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
+                    data_class = features_split.loc[targets_split == label]
+                    group.create_dataset(label, data=data_class)
+
+
+class LetterDataset(Dataset):
+    def __init__(self, index, data, label, transform=None, target_transform=None):
+        super(LetterDataset, self).__init__(index, transform=transform, target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        features = self.data[index, :]
+        target = self.label
+
+        if self.transform is not None:
+            features = self.transform(features)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return features, target
+
+
+def create_asset(root='data', num_split=None, numpy_seed=42):
+    """This methods creates the assets of the letter dataset. These are the meta-dataset splits from the
+    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
+    this directory: torchmeta.datasets.assets.letter. You can also manually change the assets."""
+
+    # number of classes per split: train, valid, test (26 classes in total)
+    if num_split is None:
+        num_split = {"train": 15, "val": 5, "test": 6}
+    num_classes = 0
+    for key in num_split:
+        num_classes += num_split[key]
+
+    from sklearn.datasets import fetch_openml
+
+    data = fetch_openml(data_id=LetterClassDataset.open_ml_id)
+    unique_targets = np.unique(data.target)
+    num_unique_targets = len(unique_targets)
+
+    assert num_classes == num_unique_targets
+
+    # split unique labels randomly
+    np.random.seed(numpy_seed)
+    perm = np.random.permutation(num_unique_targets)
+    targets_split = {'train': [unique_targets[i] for i in perm[:num_split['train']]],
+                     'val': [unique_targets[i] for i in perm[num_split['train']: num_split['train'] + num_split['val']]],
+                     'test': [unique_targets[i] for i in perm[num_split['train'] + num_split['val']:]]}
+
+    # write splits
+    root_path = os.path.join(os.path.expanduser(root), LetterClassDataset.folder)
+    for split in ["train", "val", "test"]:
+        asset_filename = os.path.join(root_path, "{0}.json".format(split))
+        with open(asset_filename, 'w') as f:
+            json.dump(targets_split[split], f)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/helpers.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,414 +1,414 @@
-import warnings
-
-from lightningdata.thirdparty.torchmeta.datasets import (Omniglot, MiniImagenet, TieredImagenet, CIFARFS,
-                                FC100, CUB, DoubleMNIST, TripleMNIST, Pascal5i)
-from lightningdata.thirdparty.torchmeta.transforms import Categorical, ClassSplitter, Rotation, SegmentationPairTransform
-from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor
-
-__all__ = [
-    'omniglot',
-    'miniimagenet',
-    'tieredimagenet',
-    'cifar_fs',
-    'fc100',
-    'cub',
-    'doublemnist',
-    'triplemnist'
-]
-
-def helper_with_default(klass, folder, shots, ways, shuffle=True,
-                        test_shots=None, seed=None, defaults={}, **kwargs):
-    if 'num_classes_per_task' in kwargs:
-        warnings.warn('Both arguments `ways` and `num_classes_per_task` were '
-            'set in the helper function for the number of classes per task. '
-            'Ignoring the argument `ways`.', stacklevel=2)
-        ways = kwargs['num_classes_per_task']
-    if 'transform' not in kwargs:
-        kwargs['transform'] = defaults.get('transform', ToTensor())
-    if 'target_transform' not in kwargs:
-        kwargs['target_transform'] = defaults.get('target_transform',
-                                                  Categorical(ways))
-    if 'class_augmentations' not in kwargs:
-        kwargs['class_augmentations'] = defaults.get('class_augmentations', None)
-    if test_shots is None:
-        test_shots = shots
-    dataset = klass(folder, num_classes_per_task=ways, **kwargs)
-    dataset = ClassSplitter(dataset, shuffle=shuffle,
-        num_train_per_class=shots, num_test_per_class=test_shots)
-    dataset.seed(seed)
-
-    return dataset
-
-def omniglot(folder, shots, ways, shuffle=True, test_shots=None,
-             seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Omniglot dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `omniglot` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `Omniglot` class.
-
-    See also
-    --------
-    `datasets.Omniglot` : Meta-dataset for the Omniglot dataset.
-    """
-    defaults = {
-        'transform': Compose([Resize(28), ToTensor()]),
-        'class_augmentations': [Rotation([90, 180, 270])]
-    }
-
-    return helper_with_default(Omniglot, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults=defaults, **kwargs)
-
-def miniimagenet(folder, shots, ways, shuffle=True, test_shots=None,
-                 seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Mini-Imagenet dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `miniimagenet` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `MiniImagenet` class.
-
-    See also
-    --------
-    `datasets.MiniImagenet` : Meta-dataset for the Mini-Imagenet dataset.
-    """
-    defaults = {
-        'transform': Compose([Resize(84), ToTensor()])
-    }
-
-    return helper_with_default(MiniImagenet, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults=defaults, **kwargs)
-
-def tieredimagenet(folder, shots, ways, shuffle=True, test_shots=None,
-                   seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Tiered-Imagenet dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `tieredimagenet` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `TieredImagenet` class.
-
-    See also
-    --------
-    `datasets.TieredImagenet` : Meta-dataset for the Tiered-Imagenet dataset.
-    """
-    defaults = {
-        'transform': Compose([Resize(84), ToTensor()])
-    }
-
-    return helper_with_default(TieredImagenet, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults=defaults, **kwargs)
-
-def cifar_fs(folder, shots, ways, shuffle=True, test_shots=None,
-             seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the CIFAR-FS dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `cifar100` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `CIFARFS` class.
-
-    See also
-    --------
-    `datasets.cifar100.CIFARFS` : Meta-dataset for the CIFAR-FS dataset.
-    """
-    return helper_with_default(CIFARFS, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults={}, **kwargs)
-
-def fc100(folder, shots, ways, shuffle=True, test_shots=None,
-          seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the FC100 dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `cifar100` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `FC100` class.
-
-    See also
-    --------
-    `datasets.cifar100.FC100` : Meta-dataset for the FC100 dataset.
-    """
-    return helper_with_default(FC100, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults={}, **kwargs)
-
-def cub(folder, shots, ways, shuffle=True, test_shots=None,
-        seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Caltech-UCSD Birds dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `cub` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `CUB` class.
-
-    See also
-    --------
-    `datasets.cub.CUB` : Meta-dataset for the Caltech-UCSD Birds dataset.
-    """
-    image_size = 84
-    defaults = {
-        'transform': Compose([
-                        Resize(int(image_size * 1.5)),
-                        CenterCrop(image_size),
-                        ToTensor()
-                    ])
-    }
-
-    return helper_with_default(CUB, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults=defaults, **kwargs)
-
-def doublemnist(folder, shots, ways, shuffle=True, test_shots=None,
-                seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Double MNIST dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `doublemnist` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `DoubleMNIST` class.
-
-    See also
-    --------
-    `datasets.doublemnist.DoubleMNIST` : Meta-dataset for the Double MNIST dataset.
-    """
-    return helper_with_default(DoubleMNIST, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults={}, **kwargs)
-
-def triplemnist(folder, shots, ways, shuffle=True, test_shots=None,
-                seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Triple MNIST dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `triplemnist` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds 
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way` 
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the 
-        number of test examples is equal to the number of training examples per 
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `TripleMNIST` class.
-
-    See also
-    --------
-    `datasets.triplemnist.TripleMNIST` : Meta-dataset for the Triple MNIST dataset.
-    """
-    return helper_with_default(TripleMNIST, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults={}, **kwargs)
-
-def pascal5i(folder, shots, ways=1, shuffle=True, test_shots=None,
-             seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the PASCAL-VOC dataset.
-
-    Parameters
-    ----------
-    folder : string
-        Root directory where the dataset folder `omniglot` exists.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification. Only supports 1-way currently
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `Omniglot` class.
-
-    """
-    defaults = {
-        'transform': SegmentationPairTransform(500),
-        'class_augmentations': []
-    }
-    return helper_with_default(Pascal5i, folder, shots, ways,
-                               shuffle=shuffle, test_shots=test_shots,
-                               seed=seed, defaults=defaults, **kwargs)
+import warnings
+
+from lightningdata.thirdparty.torchmeta.datasets import (Omniglot, MiniImagenet, TieredImagenet, CIFARFS,
+                                FC100, CUB, DoubleMNIST, TripleMNIST, Pascal5i)
+from lightningdata.thirdparty.torchmeta.transforms import Categorical, ClassSplitter, Rotation, SegmentationPairTransform
+from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor
+
+__all__ = [
+    'omniglot',
+    'miniimagenet',
+    'tieredimagenet',
+    'cifar_fs',
+    'fc100',
+    'cub',
+    'doublemnist',
+    'triplemnist'
+]
+
+def helper_with_default(klass, folder, shots, ways, shuffle=True,
+                        test_shots=None, seed=None, defaults={}, **kwargs):
+    if 'num_classes_per_task' in kwargs:
+        warnings.warn('Both arguments `ways` and `num_classes_per_task` were '
+            'set in the helper function for the number of classes per task. '
+            'Ignoring the argument `ways`.', stacklevel=2)
+        ways = kwargs['num_classes_per_task']
+    if 'transform' not in kwargs:
+        kwargs['transform'] = defaults.get('transform', ToTensor())
+    if 'target_transform' not in kwargs:
+        kwargs['target_transform'] = defaults.get('target_transform',
+                                                  Categorical(ways))
+    if 'class_augmentations' not in kwargs:
+        kwargs['class_augmentations'] = defaults.get('class_augmentations', None)
+    if test_shots is None:
+        test_shots = shots
+    dataset = klass(folder, num_classes_per_task=ways, **kwargs)
+    dataset = ClassSplitter(dataset, shuffle=shuffle,
+        num_train_per_class=shots, num_test_per_class=test_shots)
+    dataset.seed(seed)
+
+    return dataset
+
+def omniglot(folder, shots, ways, shuffle=True, test_shots=None,
+             seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Omniglot dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `omniglot` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `Omniglot` class.
+
+    See also
+    --------
+    `datasets.Omniglot` : Meta-dataset for the Omniglot dataset.
+    """
+    defaults = {
+        'transform': Compose([Resize(28), ToTensor()]),
+        'class_augmentations': [Rotation([90, 180, 270])]
+    }
+
+    return helper_with_default(Omniglot, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults=defaults, **kwargs)
+
+def miniimagenet(folder, shots, ways, shuffle=True, test_shots=None,
+                 seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Mini-Imagenet dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `miniimagenet` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `MiniImagenet` class.
+
+    See also
+    --------
+    `datasets.MiniImagenet` : Meta-dataset for the Mini-Imagenet dataset.
+    """
+    defaults = {
+        'transform': Compose([Resize(84), ToTensor()])
+    }
+
+    return helper_with_default(MiniImagenet, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults=defaults, **kwargs)
+
+def tieredimagenet(folder, shots, ways, shuffle=True, test_shots=None,
+                   seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Tiered-Imagenet dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `tieredimagenet` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `TieredImagenet` class.
+
+    See also
+    --------
+    `datasets.TieredImagenet` : Meta-dataset for the Tiered-Imagenet dataset.
+    """
+    defaults = {
+        'transform': Compose([Resize(84), ToTensor()])
+    }
+
+    return helper_with_default(TieredImagenet, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults=defaults, **kwargs)
+
+def cifar_fs(folder, shots, ways, shuffle=True, test_shots=None,
+             seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the CIFAR-FS dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `cifar100` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `CIFARFS` class.
+
+    See also
+    --------
+    `datasets.cifar100.CIFARFS` : Meta-dataset for the CIFAR-FS dataset.
+    """
+    return helper_with_default(CIFARFS, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults={}, **kwargs)
+
+def fc100(folder, shots, ways, shuffle=True, test_shots=None,
+          seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the FC100 dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `cifar100` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `FC100` class.
+
+    See also
+    --------
+    `datasets.cifar100.FC100` : Meta-dataset for the FC100 dataset.
+    """
+    return helper_with_default(FC100, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults={}, **kwargs)
+
+def cub(folder, shots, ways, shuffle=True, test_shots=None,
+        seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Caltech-UCSD Birds dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `cub` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `CUB` class.
+
+    See also
+    --------
+    `datasets.cub.CUB` : Meta-dataset for the Caltech-UCSD Birds dataset.
+    """
+    image_size = 84
+    defaults = {
+        'transform': Compose([
+                        Resize(int(image_size * 1.5)),
+                        CenterCrop(image_size),
+                        ToTensor()
+                    ])
+    }
+
+    return helper_with_default(CUB, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults=defaults, **kwargs)
+
+def doublemnist(folder, shots, ways, shuffle=True, test_shots=None,
+                seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Double MNIST dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `doublemnist` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `DoubleMNIST` class.
+
+    See also
+    --------
+    `datasets.doublemnist.DoubleMNIST` : Meta-dataset for the Double MNIST dataset.
+    """
+    return helper_with_default(DoubleMNIST, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults={}, **kwargs)
+
+def triplemnist(folder, shots, ways, shuffle=True, test_shots=None,
+                seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Triple MNIST dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `triplemnist` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds 
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way` 
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the 
+        number of test examples is equal to the number of training examples per 
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `TripleMNIST` class.
+
+    See also
+    --------
+    `datasets.triplemnist.TripleMNIST` : Meta-dataset for the Triple MNIST dataset.
+    """
+    return helper_with_default(TripleMNIST, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults={}, **kwargs)
+
+def pascal5i(folder, shots, ways=1, shuffle=True, test_shots=None,
+             seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the PASCAL-VOC dataset.
+
+    Parameters
+    ----------
+    folder : string
+        Root directory where the dataset folder `omniglot` exists.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification. Only supports 1-way currently
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `Omniglot` class.
+
+    """
+    defaults = {
+        'transform': SegmentationPairTransform(500),
+        'class_augmentations': []
+    }
+    return helper_with_default(Pascal5i, folder, shots, ways,
+                               shuffle=shuffle, test_shots=test_shots,
+                               seed=seed, defaults=defaults, **kwargs)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-import warnings
-
-from lightningdata.thirdparty.torchmeta.datasets import Letter, PlantsTexture, PlantsShape, PlantsMargin, Bach
-from lightningdata.thirdparty.torchmeta.transforms import Categorical, ClassSplitter
-from lightningdata.thirdparty.torchmeta.transforms.tabular_transforms import NumpyToTorch
-
-__all__ = [
-    'letter',
-    'plants_texture',
-    'plants_shape',
-    'plants_margin',
-    'bach'
-]
-
-
-def helper_with_default_tabular(klass, folder, shots, ways, shuffle=True,
-                                test_shots=None, seed=None, defaults=None, **kwargs):
-    """
-    Parameters
-    ----------
-    klass : CombinationMetaDataset
-        the class corresponding to the meta-dataset, e.g., Covertype
-
-    folder : string
-        Root directory where the dataset folder exists, e.g., `covertype_task_id_2118`.
-
-    shots : int
-        Number of (training) examples per class in each task. This corresponds
-        to `k` in `k-shot` classification.
-
-    ways : int
-        Number of classes per task. This corresponds to `N` in `N-way`
-        classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples per class in each task. If `None`, then the
-        number of test examples is equal to the number of training examples per
-        class.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `TieredImagenet` class.
-
-    Returns
-    -------
-    klass
-        The meta-dataset with ClassSplitter applied, e.g., Covertype.
-    """
-
-    if defaults is None:
-        defaults = {}
-
-    if 'num_classes_per_task' in kwargs:
-        warnings.warn('Both arguments `ways` and `num_classes_per_task` were '
-            'set in the helper function for the number of classes per task. '
-            'Ignoring the argument `ways`.', stacklevel=2)
-        ways = kwargs['num_classes_per_task']
-
-    if 'transform' not in kwargs:
-        kwargs['transform'] = defaults.get('transform', NumpyToTorch())
-
-    if 'target_transform' not in kwargs:
-        kwargs['target_transform'] = defaults.get('target_transform',
-                                                  Categorical(ways))
-    if 'class_augmentations' not in kwargs:
-        kwargs['class_augmentations'] = defaults.get('class_augmentations', None)
-
-    if test_shots is None:
-        test_shots = shots
-    dataset = klass(folder,
-                    num_classes_per_task=ways,
-                    **kwargs)
-    dataset = ClassSplitter(dataset,
-                            shuffle=shuffle,
-                            num_train_per_class=shots,
-                            num_test_per_class=test_shots)
-    dataset.seed(seed)
-
-    return dataset
-
-
-def letter(folder: str, shots: int, ways: int, shuffle: bool=True,
-              test_shots: int=None, seed: int=None, **kwargs) -> Letter:
-    """
-    Wrapper that creates a meta-dataset for the Letter tabular dataset.
-
-    Notes
-    --------
-    Letter has 26 classes in total with default splits train/val/test : 15/5/6.
-
-    See also
-    --------
-    `datasets.Letter` : CombinationMetaDataset for the Letter dataset.
-    """
-    return helper_with_default_tabular(Letter, folder, shots, ways, shuffle=shuffle,
-                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
-
-
-def plants_texture(folder: str, shots: int, ways: int, shuffle: bool=True,
-                   test_shots: int=None, seed: int=None, **kwargs) -> PlantsTexture:
-    """
-    Wrapper that creates a meta-dataset for the PlantsTexture tabular dataset.
-
-    Notes
-    --------
-    PlantsTexture has 100 classes in total with default splits train/val/test : 70/15/15.
-
-    See also
-    --------
-    `datasets.PlantsTexture` : CombinationMetaDataset for the PlantsTexture dataset.
-    """
-    return helper_with_default_tabular(PlantsTexture, folder, shots, ways, shuffle=shuffle,
-                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
-
-
-def plants_shape(folder: str, shots: int, ways: int, shuffle: bool=True,
-                 test_shots: int=None, seed: int=None, **kwargs) -> PlantsShape:
-    """
-    Wrapper that creates a meta-dataset for the PlantsShape tabular dataset.
-
-    Notes
-    --------
-    PlantsShape has 100 classes in total with default splits train/val/test : 70/15/15.
-
-    See also
-    --------
-    `datasets.PlantsShape` : Meta-dataset for the PlantsShape dataset.
-    """
-    return helper_with_default_tabular(PlantsShape, folder, shots, ways, shuffle=shuffle,
-                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
-
-
-def plants_margin(folder: str, shots: int, ways: int, shuffle: bool=True,
-                  test_shots: int=None, seed: int=None, **kwargs) -> PlantsMargin:
-    """
-    Wrapper that creates a meta-dataset for the PlantsMargin tabular dataset.
-
-    Notes
-    --------
-    PlantsMargin has 100 classes in total with default splits train/val/test : 70/15/15.
-
-    See also
-    --------
-    `datasets.PlantsMargin` : CombinationMetaDataset for the PlantsMargin dataset.
-    """
-    return helper_with_default_tabular(PlantsMargin, folder, shots, ways, shuffle=shuffle,
-                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
-
-
-def bach(folder: str, shots: int, ways: int, shuffle: bool=True, test_shots: int=None,
-         min_num_samples_per_class: int=None, seed: int=None, **kwargs) -> Bach:
-    """
-    Wrapper that creates a meta-dataset for the Bach tabular dataset.
-
-    Notes
-    --------
-    Bach has 101 classes in total with default splits train/val/test : 70/15/15. # Todo change
-
-    See also
-    --------
-    `datasets.Bach` : CombinationMetaDataset for the Bach dataset.
-    """
-    if min_num_samples_per_class is None:
-        if test_shots is None:
-            min_num_samples_per_class = int(2 * shots)
-        else:
-            min_num_samples_per_class = int(test_shots + shots)
-    return helper_with_default_tabular(Bach, folder, shots, ways, shuffle=shuffle,
-                                       test_shots=test_shots, seed=seed, defaults=None,
-                                       min_num_samples_per_class=min_num_samples_per_class, **kwargs)
+import warnings
+
+from lightningdata.thirdparty.torchmeta.datasets import Letter, PlantsTexture, PlantsShape, PlantsMargin, Bach
+from lightningdata.thirdparty.torchmeta.transforms import Categorical, ClassSplitter
+from lightningdata.thirdparty.torchmeta.transforms.tabular_transforms import NumpyToTorch
+
+__all__ = [
+    'letter',
+    'plants_texture',
+    'plants_shape',
+    'plants_margin',
+    'bach'
+]
+
+
+def helper_with_default_tabular(klass, folder, shots, ways, shuffle=True,
+                                test_shots=None, seed=None, defaults=None, **kwargs):
+    """
+    Parameters
+    ----------
+    klass : CombinationMetaDataset
+        the class corresponding to the meta-dataset, e.g., Covertype
+
+    folder : string
+        Root directory where the dataset folder exists, e.g., `covertype_task_id_2118`.
+
+    shots : int
+        Number of (training) examples per class in each task. This corresponds
+        to `k` in `k-shot` classification.
+
+    ways : int
+        Number of classes per task. This corresponds to `N` in `N-way`
+        classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples per class in each task. If `None`, then the
+        number of test examples is equal to the number of training examples per
+        class.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `TieredImagenet` class.
+
+    Returns
+    -------
+    klass
+        The meta-dataset with ClassSplitter applied, e.g., Covertype.
+    """
+
+    if defaults is None:
+        defaults = {}
+
+    if 'num_classes_per_task' in kwargs:
+        warnings.warn('Both arguments `ways` and `num_classes_per_task` were '
+            'set in the helper function for the number of classes per task. '
+            'Ignoring the argument `ways`.', stacklevel=2)
+        ways = kwargs['num_classes_per_task']
+
+    if 'transform' not in kwargs:
+        kwargs['transform'] = defaults.get('transform', NumpyToTorch())
+
+    if 'target_transform' not in kwargs:
+        kwargs['target_transform'] = defaults.get('target_transform',
+                                                  Categorical(ways))
+    if 'class_augmentations' not in kwargs:
+        kwargs['class_augmentations'] = defaults.get('class_augmentations', None)
+
+    if test_shots is None:
+        test_shots = shots
+    dataset = klass(folder,
+                    num_classes_per_task=ways,
+                    **kwargs)
+    dataset = ClassSplitter(dataset,
+                            shuffle=shuffle,
+                            num_train_per_class=shots,
+                            num_test_per_class=test_shots)
+    dataset.seed(seed)
+
+    return dataset
+
+
+def letter(folder: str, shots: int, ways: int, shuffle: bool=True,
+              test_shots: int=None, seed: int=None, **kwargs) -> Letter:
+    """
+    Wrapper that creates a meta-dataset for the Letter tabular dataset.
+
+    Notes
+    --------
+    Letter has 26 classes in total with default splits train/val/test : 15/5/6.
+
+    See also
+    --------
+    `datasets.Letter` : CombinationMetaDataset for the Letter dataset.
+    """
+    return helper_with_default_tabular(Letter, folder, shots, ways, shuffle=shuffle,
+                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
+
+
+def plants_texture(folder: str, shots: int, ways: int, shuffle: bool=True,
+                   test_shots: int=None, seed: int=None, **kwargs) -> PlantsTexture:
+    """
+    Wrapper that creates a meta-dataset for the PlantsTexture tabular dataset.
+
+    Notes
+    --------
+    PlantsTexture has 100 classes in total with default splits train/val/test : 70/15/15.
+
+    See also
+    --------
+    `datasets.PlantsTexture` : CombinationMetaDataset for the PlantsTexture dataset.
+    """
+    return helper_with_default_tabular(PlantsTexture, folder, shots, ways, shuffle=shuffle,
+                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
+
+
+def plants_shape(folder: str, shots: int, ways: int, shuffle: bool=True,
+                 test_shots: int=None, seed: int=None, **kwargs) -> PlantsShape:
+    """
+    Wrapper that creates a meta-dataset for the PlantsShape tabular dataset.
+
+    Notes
+    --------
+    PlantsShape has 100 classes in total with default splits train/val/test : 70/15/15.
+
+    See also
+    --------
+    `datasets.PlantsShape` : Meta-dataset for the PlantsShape dataset.
+    """
+    return helper_with_default_tabular(PlantsShape, folder, shots, ways, shuffle=shuffle,
+                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
+
+
+def plants_margin(folder: str, shots: int, ways: int, shuffle: bool=True,
+                  test_shots: int=None, seed: int=None, **kwargs) -> PlantsMargin:
+    """
+    Wrapper that creates a meta-dataset for the PlantsMargin tabular dataset.
+
+    Notes
+    --------
+    PlantsMargin has 100 classes in total with default splits train/val/test : 70/15/15.
+
+    See also
+    --------
+    `datasets.PlantsMargin` : CombinationMetaDataset for the PlantsMargin dataset.
+    """
+    return helper_with_default_tabular(PlantsMargin, folder, shots, ways, shuffle=shuffle,
+                                       test_shots=test_shots, seed=seed, defaults=None, **kwargs)
+
+
+def bach(folder: str, shots: int, ways: int, shuffle: bool=True, test_shots: int=None,
+         min_num_samples_per_class: int=None, seed: int=None, **kwargs) -> Bach:
+    """
+    Wrapper that creates a meta-dataset for the Bach tabular dataset.
+
+    Notes
+    --------
+    Bach has 101 classes in total with default splits train/val/test : 70/15/15. # Todo change
+
+    See also
+    --------
+    `datasets.Bach` : CombinationMetaDataset for the Bach dataset.
+    """
+    if min_num_samples_per_class is None:
+        if test_shots is None:
+            min_num_samples_per_class = int(2 * shots)
+        else:
+            min_num_samples_per_class = int(test_shots + shots)
+    return helper_with_default_tabular(Bach, folder, shots, ways, shuffle=shuffle,
+                                       test_shots=test_shots, seed=seed, defaults=None,
+                                       min_num_samples_per_class=min_num_samples_per_class, **kwargs)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/letter.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/omniglot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-import numpy as np
-import os
-import json
-import h5py
-from tqdm import tqdm
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class Letter(CombinationMetaDataset):
-    """The Letter Image Recognition Dataset """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        """
-        Letter Image Recognition Data [1]:
-        open-ml-id: 6
-        https://archive.ics.uci.edu/ml/datasets/Letter+Recognition - 01-01-1991
-
-        The objective is to identify each of a large number of black-and-white
-        rectangular pixel displays as one of the 26 capital letters in the English
-        alphabet.  The character images were based on 20 different fonts and each
-        letter within these 20 fonts was randomly distorted to produce a file of
-        20,000 unique stimuli.  Each stimulus was converted into 16 primitive
-        numerical attributes (statistical moments and edge counts) which were then
-        scaled to fit into a range of integer values from 0 through 15.  We
-        typically train on the first 16000 items and then use the resulting model
-        to predict the letter category for the remaining 4000.  See the article
-        cited above for more details.
-
-        Parameters
-        ----------
-        root : string
-            Root directory where the dataset folder `letter` exists.
-
-        num_classes_per_task : int
-            Number of classes per tasks. This corresponds to "N" in "N-way"
-            classification.
-
-        meta_train : bool (default: `False`)
-            Use the meta-train split of the dataset. If set to `True`, then the
-            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
-            of these three arguments must be set to `True`.
-
-        meta_val : bool (default: `False`)
-            Use the meta-validation split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_test : bool (default: `False`)
-            Use the meta-test split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_split : string in {'train', 'val', 'test'}, optional
-            Name of the split to use. This overrides the arguments `meta_train`,
-            `meta_val` and `meta_test` if all three are set to `False`.
-
-        transform : callable, optional
-            A function/transform that takes a numpy array or a pytorch array
-            (depending when the transforms is applied), and returns a transformed
-            version.
-
-        target_transform : callable, optional
-            A function/transform that takes a target, and returns a transformed
-            version.
-
-        dataset_transform : callable, optional
-            A function/transform that takes a dataset (ie. a task), and returns a
-            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-        class_augmentations : list of callable, optional
-            A list of functions that augment the dataset with new classes. These
-            classes are transformations of existing classes.
-
-        download : bool (default: `False`)
-            If `True`, downloads the original files and processes the dataset in the
-            root directory (under the `letter` folder). If the dataset
-            is already available, this does not download/process the dataset again.
-
-        References
-        -----
-        [1] P. W. Frey and D. J. Slate. "Letter Recognition Using Holland-style
-        Adaptive Classifiers". Machine Learning 6(2), 1991
-        """
-        dataset = LetterClassDataset(root,
-                                     meta_train=meta_train,
-                                     meta_val=meta_val,
-                                     meta_test=meta_test,
-                                     meta_split=meta_split,
-                                     transform=transform,
-                                     class_augmentations=class_augmentations,
-                                     download=download)
-        super(Letter, self).__init__(dataset,
-                                     num_classes_per_task,
-                                     target_transform=target_transform,
-                                     dataset_transform=dataset_transform)
-
-
-class LetterClassDataset(ClassDataset):
-
-    open_ml_id = 6
-    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
-    dataset_name = "letter"
-
-    folder = "letter"
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
-                 class_augmentations=None, download=False):
-        super(LetterClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
-                                                 meta_split=meta_split, class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('Letter integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return LetterDataset(index, data, label, transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data is not None:
-            self._data.close()
-            self._data = None
-
-    def download(self):
-
-        if self._check_integrity():
-            return
-
-        from sklearn.datasets import fetch_openml
-
-        data = fetch_openml(data_id=self.open_ml_id)
-        features = data.data
-        targets = data.target
-
-        os.makedirs(self.root, exist_ok=True)
-
-        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
-        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
-        for s, split in enumerate(['train', 'val', 'test']):
-            labels_assets_split = get_asset(self.folder, '{0}.json'.format(split))
-
-            is_in_split = [t in labels_assets_split for t in targets]
-            features_split = features.loc[is_in_split]
-            targets_split = targets.loc[is_in_split]
-            assert targets_split.shape[0] == features_split.shape[0]
-
-            unique_targets_split = np.unique(targets_split)
-            if len(labels_assets_split) > unique_targets_split.shape[0]:
-                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
-                      f"given by assets ({len(labels_assets_split)}). Proceeding with unique set of labels.")
-
-            # write unique targets to json file.
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(unique_targets_split.tolist(), f)
-
-            # write data (features and class labels)
-            filename = os.path.join(self.root, self.filename.format(split))
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-
-                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
-                    data_class = features_split.loc[targets_split == label]
-                    group.create_dataset(label, data=data_class)
-
-
-class LetterDataset(Dataset):
-    def __init__(self, index, data, label, transform=None, target_transform=None):
-        super(LetterDataset, self).__init__(index, transform=transform, target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        features = self.data[index, :]
-        target = self.label
-
-        if self.transform is not None:
-            features = self.transform(features)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return features, target
-
-
-def create_asset(root='data', num_split=None, numpy_seed=42):
-    """This methods creates the assets of the letter dataset. These are the meta-dataset splits from the
-    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
-    this directory: torchmeta.datasets.assets.letter. You can also manually change the assets."""
-
-    # number of classes per split: train, valid, test (26 classes in total)
-    if num_split is None:
-        num_split = {"train": 15, "val": 5, "test": 6}
-    num_classes = 0
-    for key in num_split:
-        num_classes += num_split[key]
-
-    from sklearn.datasets import fetch_openml
-
-    data = fetch_openml(data_id=LetterClassDataset.open_ml_id)
-    unique_targets = np.unique(data.target)
-    num_unique_targets = len(unique_targets)
-
-    assert num_classes == num_unique_targets
-
-    # split unique labels randomly
-    np.random.seed(numpy_seed)
-    perm = np.random.permutation(num_unique_targets)
-    targets_split = {'train': [unique_targets[i] for i in perm[:num_split['train']]],
-                     'val': [unique_targets[i] for i in perm[num_split['train']: num_split['train'] + num_split['val']]],
-                     'test': [unique_targets[i] for i in perm[num_split['train'] + num_split['val']:]]}
-
-    # write splits
-    root_path = os.path.join(os.path.expanduser(root), LetterClassDataset.folder)
-    for split in ["train", "val", "test"]:
-        asset_filename = os.path.join(root_path, "{0}.json".format(split))
-        with open(asset_filename, 'w') as f:
-            json.dump(targets_split[split], f)
+import os
+import json
+import glob
+import h5py
+from PIL import Image, ImageOps
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from torchvision.datasets.utils import list_dir, download_url
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class Omniglot(CombinationMetaDataset):
+    """
+    The Omniglot dataset [1]. A dataset of 1623 handwritten characters from 
+    50 different alphabets. 
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `omniglot` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way" 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    use_vinyals_split : bool (default: `True`)
+        If set to `True`, the dataset uses the splits defined in [3]. If `False`, 
+        then the meta-train split corresponds to `images_background`, and the 
+        meta-test split corresponds to `images_evaluation` (raises an error when 
+        calling the meta-validation split).
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the zip files and processes the dataset in the root 
+        directory (under the `omniglot` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The dataset is downloaded from the original [Omniglot repository]
+    (https://github.com/brendenlake/omniglot). The meta train/validation/test 
+    splits used in [3] are taken from [this repository]
+    (https://github.com/jakesnell/prototypical-networks). These splits are 
+    over 1028/172/423 classes (characters).
+
+    References
+    ----------
+    .. [1] Lake, B. M., Salakhutdinov, R., and Tenenbaum, J. B. (2015). Human-level 
+           concept learning through probabilistic program induction. Science, 350(6266), 
+           1332-1338 (http://www.sciencemag.org/content/350/6266/1332.short)
+
+    .. [2] Lake, B. M., Salakhutdinov, R., and Tenenbaum, J. B. (2019). The Omniglot 
+           Challenge: A 3-Year Progress Report (https://arxiv.org/abs/1902.03477)
+
+    .. [3] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016). 
+           Matching Networks for One Shot Learning. In Advances in Neural 
+           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 use_vinyals_split=True, transform=None, target_transform=None,
+                 dataset_transform=None, class_augmentations=None, download=False):
+        dataset = OmniglotClassDataset(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test,
+            use_vinyals_split=use_vinyals_split, transform=transform,
+            meta_split=meta_split, class_augmentations=class_augmentations,
+            download=download)
+        super(Omniglot, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+
+class OmniglotClassDataset(ClassDataset):
+    folder = 'omniglot'
+    download_url_prefix = 'https://github.com/brendenlake/omniglot/raw/master/python'
+    zips_md5 = {
+        'images_background': '68d2efa1b9178cc56df9314c21c6e718',
+        'images_evaluation': '6b91aef0f799c5bb55b94e3f2daec811'
+    }
+
+    filename = 'data.hdf5'
+    filename_labels = '{0}{1}_labels.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, use_vinyals_split=True, transform=None,
+                 class_augmentations=None, download=False):
+        super(OmniglotClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+
+        if self.meta_val and (not use_vinyals_split):
+            raise ValueError('Trying to use the meta-validation without the '
+                'Vinyals split. You must set `use_vinyals_split=True` to use '
+                'the meta-validation split.')
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.use_vinyals_split = use_vinyals_split
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root, self.filename)
+        self.split_filename_labels = os.path.join(self.root,
+            self.filename_labels.format('vinyals_' if use_vinyals_split else '',
+            self.meta_split))
+
+        self._data = None
+        self._labels = None
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('Omniglot integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        character_name = '/'.join(self.labels[index % self.num_classes])
+        data = self.data[character_name]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return OmniglotDataset(index, data, character_name,
+            transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data = h5py.File(self.split_filename, 'r')
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data is not None:
+            self._data.close()
+            self._data = None
+
+    def download(self):
+        import zipfile
+        import shutil
+
+        if self._check_integrity():
+            return
+
+        for name in self.zips_md5:
+            zip_filename = '{0}.zip'.format(name)
+            filename = os.path.join(self.root, zip_filename)
+            if os.path.isfile(filename):
+                continue
+
+            url = '{0}/{1}'.format(self.download_url_prefix, zip_filename)
+            download_url(url, self.root, zip_filename, self.zips_md5[name])
+
+            with zipfile.ZipFile(filename, 'r') as f:
+                f.extractall(self.root)
+
+        filename = os.path.join(self.root, self.filename)
+        with h5py.File(filename, 'w') as f:
+            for name in self.zips_md5:
+                group = f.create_group(name)
+
+                alphabets = list_dir(os.path.join(self.root, name))
+                characters = [(name, alphabet, character) for alphabet in alphabets
+                    for character in list_dir(os.path.join(self.root, name, alphabet))]
+
+                split = 'train' if name == 'images_background' else 'test'
+                labels_filename = os.path.join(self.root,
+                    self.filename_labels.format('', split))
+                with open(labels_filename, 'w') as f_labels:
+                    labels = sorted(characters)
+                    json.dump(labels, f_labels)
+
+                for _, alphabet, character in characters:
+                    filenames = glob.glob(os.path.join(self.root, name,
+                        alphabet, character, '*.png'))
+                    dataset = group.create_dataset('{0}/{1}'.format(alphabet,
+                        character), (len(filenames), 105, 105), dtype='uint8')
+
+                    for i, char_filename in enumerate(filenames):
+                        image = Image.open(char_filename, mode='r').convert('L')
+                        dataset[i] = ImageOps.invert(image)
+
+                shutil.rmtree(os.path.join(self.root, name))
+
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename_labels.format(
+                'vinyals_', split))
+            data = get_asset(self.folder, '{0}.json'.format(split), dtype='json')
+
+            with open(filename, 'w') as f:
+                labels = sorted([('images_{0}'.format(name), alphabet, character)
+                    for (name, alphabets) in data.items()
+                    for (alphabet, characters) in alphabets.items()
+                    for character in characters])
+                json.dump(labels, f)
+
+
+class OmniglotDataset(Dataset):
+    def __init__(self, index, data, character_name,
+                 transform=None, target_transform=None):
+        super(OmniglotDataset, self).__init__(index, transform=transform,
+                                              target_transform=target_transform)
+        self.data = data
+        self.character_name = character_name
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        image = Image.fromarray(self.data[index])
+        target = self.character_name
+
+        if self.transform is not None:
+            image = self.transform(image)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (image, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-import os
-import pickle
-from PIL import Image
-import h5py
-import json
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-# QKFIX: See torchmeta.datasets.utils for more informations
-from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
-
-
-class MiniImagenet(CombinationMetaDataset):
-    """
-    The Mini-Imagenet dataset, introduced in [1]. This dataset contains images 
-    of 100 different classes from the ILSVRC-12 dataset (Imagenet challenge). 
-    The meta train/validation/test splits are taken from [2] for reproducibility.
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `miniimagenet` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way" 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the root 
-        directory (under the `miniimagenet` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The dataset is downloaded from [this repository]
-    (https://github.com/renmengye/few-shot-ssl-public/). The meta train/
-    validation/test splits are over 64/16/20 classes.
-
-    References
-    ----------
-    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016). 
-           Matching Networks for One Shot Learning. In Advances in Neural 
-           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
-
-    .. [2] Ravi, S. and Larochelle, H. (2016). Optimization as a Model for 
-           Few-Shot Learning. (https://openreview.net/forum?id=rJY0-Kcll)
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = MiniImagenetClassDataset(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-        super(MiniImagenet, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-
-class MiniImagenetClassDataset(ClassDataset):
-    folder = 'miniimagenet'
-    # Google Drive ID from https://github.com/renmengye/few-shot-ssl-public
-    gdrive_id = '16V_ZlkW4SsnNDtnGmaBRq2OoPmUOc5mY'
-    gz_filename = 'mini-imagenet.tar.gz'
-    gz_md5 = 'b38f1eb4251fb9459ecc8e7febf9b2eb'
-    pkl_filename = 'mini-imagenet-cache-{0}.pkl'
-
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(MiniImagenetClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-        
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root,
-            self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root,
-            self.filename_labels.format(self.meta_split))
-
-        self._data = None
-        self._labels = None
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('MiniImagenet integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        class_name = self.labels[index % self.num_classes]
-        data = self.data[class_name]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return MiniImagenetDataset(index, data, class_name,
-            transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data_file is not None:
-            self._data_file.close()
-            self._data_file = None
-            self._data = None
-
-    def download(self):
-        import tarfile
-
-        if self._check_integrity():
-            return
-
-        download_file_from_google_drive(self.gdrive_id, self.root,
-            self.gz_filename, md5=self.gz_md5)
-
-        filename = os.path.join(self.root, self.gz_filename)
-        with tarfile.open(filename, 'r') as f:
-            f.extractall(self.root)
-
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename.format(split))
-            if os.path.isfile(filename):
-                continue
-
-            pkl_filename = os.path.join(self.root, self.pkl_filename.format(split))
-            if not os.path.isfile(pkl_filename):
-                raise IOError()
-            with open(pkl_filename, 'rb') as f:
-                data = pickle.load(f)
-                images, classes = data['image_data'], data['class_dict']
-
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-                for name, indices in classes.items():
-                    group.create_dataset(name, data=images[indices])
-
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                labels = sorted(list(classes.keys()))
-                json.dump(labels, f)
-
-            if os.path.isfile(pkl_filename):
-                os.remove(pkl_filename)
-
-
-class MiniImagenetDataset(Dataset):
-    def __init__(self, index, data, class_name,
-                 transform=None, target_transform=None):
-        super(MiniImagenetDataset, self).__init__(index, transform=transform,
-                                                  target_transform=target_transform)
-        self.data = data
-        self.class_name = class_name
-
-    def __len__(self):
-        return self.data.shape[0]
-
-    def __getitem__(self, index):
-        image = Image.fromarray(self.data[index])
-        target = self.class_name
-
-        if self.transform is not None:
-            image = self.transform(image)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (image, target)
+import os
+import pickle
+from PIL import Image
+import h5py
+import json
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+# QKFIX: See torchmeta.datasets.utils for more informations
+from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
+
+
+class MiniImagenet(CombinationMetaDataset):
+    """
+    The Mini-Imagenet dataset, introduced in [1]. This dataset contains images 
+    of 100 different classes from the ILSVRC-12 dataset (Imagenet challenge). 
+    The meta train/validation/test splits are taken from [2] for reproducibility.
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `miniimagenet` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way" 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the root 
+        directory (under the `miniimagenet` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The dataset is downloaded from [this repository]
+    (https://github.com/renmengye/few-shot-ssl-public/). The meta train/
+    validation/test splits are over 64/16/20 classes.
+
+    References
+    ----------
+    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016). 
+           Matching Networks for One Shot Learning. In Advances in Neural 
+           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
+
+    .. [2] Ravi, S. and Larochelle, H. (2016). Optimization as a Model for 
+           Few-Shot Learning. (https://openreview.net/forum?id=rJY0-Kcll)
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = MiniImagenetClassDataset(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+        super(MiniImagenet, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+
+class MiniImagenetClassDataset(ClassDataset):
+    folder = 'miniimagenet'
+    # Google Drive ID from https://github.com/renmengye/few-shot-ssl-public
+    gdrive_id = '16V_ZlkW4SsnNDtnGmaBRq2OoPmUOc5mY'
+    gz_filename = 'mini-imagenet.tar.gz'
+    gz_md5 = 'b38f1eb4251fb9459ecc8e7febf9b2eb'
+    pkl_filename = 'mini-imagenet-cache-{0}.pkl'
+
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(MiniImagenetClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+        
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root,
+            self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root,
+            self.filename_labels.format(self.meta_split))
+
+        self._data = None
+        self._labels = None
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('MiniImagenet integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        class_name = self.labels[index % self.num_classes]
+        data = self.data[class_name]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return MiniImagenetDataset(index, data, class_name,
+            transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data_file is not None:
+            self._data_file.close()
+            self._data_file = None
+            self._data = None
+
+    def download(self):
+        import tarfile
+
+        if self._check_integrity():
+            return
+
+        download_file_from_google_drive(self.gdrive_id, self.root,
+            self.gz_filename, md5=self.gz_md5)
+
+        filename = os.path.join(self.root, self.gz_filename)
+        with tarfile.open(filename, 'r') as f:
+            f.extractall(self.root)
+
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename.format(split))
+            if os.path.isfile(filename):
+                continue
+
+            pkl_filename = os.path.join(self.root, self.pkl_filename.format(split))
+            if not os.path.isfile(pkl_filename):
+                raise IOError()
+            with open(pkl_filename, 'rb') as f:
+                data = pickle.load(f)
+                images, classes = data['image_data'], data['class_dict']
+
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+                for name, indices in classes.items():
+                    group.create_dataset(name, data=images[indices])
+
+            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                labels = sorted(list(classes.keys()))
+                json.dump(labels, f)
+
+            if os.path.isfile(pkl_filename):
+                os.remove(pkl_filename)
+
+
+class MiniImagenetDataset(Dataset):
+    def __init__(self, index, data, class_name,
+                 transform=None, target_transform=None):
+        super(MiniImagenetDataset, self).__init__(index, transform=transform,
+                                                  target_transform=target_transform)
+        self.data = data
+        self.class_name = class_name
+
+    def __len__(self):
+        return self.data.shape[0]
+
+    def __getitem__(self, index):
+        image = Image.fromarray(self.data[index])
+        target = self.class_name
+
+        if self.transform is not None:
+            image = self.transform(image)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (image, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,319 +1,320 @@
-import numpy as np
-import os
-import json
-import h5py
-from tqdm import tqdm
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class PlantsMargin(CombinationMetaDataset):
-    """The PlantsMargin dataset """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False, process_features=False):
-        """
-        One-hundred plant species leaves dataset (Class = Margin) [1], [2], [3]
-        open-ml-id: 1491
-        https://archive.ics.uci.edu/ml/datasets/One-hundred+plant+species+leaves+data+set) - 2010
-
-
-           (a) Original owners of colour Leaves Samples:
-
-         James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.
-         The colour images are not included.
-         The Leaves were collected in the Royal Botanic Gardens, Kew, UK.
-         email: james.cope@kingston.ac.uk
-
-           (b) This dataset consists of work carried out by James Cope, Charles Mallah, and James Orwell.
-         Donor of database Charles Mallah: charles.mallah@kingston.ac.uk; James Cope:  james.cope@kingston.ac.uk
-
-        The original data directory contains the binary images (masks) of the leaf samples (colour images not included).
-        There are three features for each image: Shape, Margin and Texture.
-        For each feature, a 64 element vector is given per leaf sample.
-        These vectors are taken as a contiguous descriptor (for shape) or histograms (for texture and margin).
-        So, there are three different files, one for each feature problem:
-         * 'data_Sha_64.txt' -> prediction based on shape
-         * 'data_Tex_64.txt' -> prediction based on texture
-         * 'data_Mar_64.txt' -> prediction based on margin [dataset provided here]
-
-        Each row has a 64-element feature vector followed by the Class label.
-        There is a total of 1600 samples with 16 samples per leaf class (100 classes), and no missing values.
-
-        Three 64 element feature vectors per sample.
-
-        Parameters
-        ----------
-        root : string
-            Root directory where the dataset folder `one_hundred_plants_margin` exists.
-
-        num_classes_per_task : int
-            Number of classes per tasks. This corresponds to "N" in "N-way"
-            classification.
-
-        meta_train : bool (default: `False`)
-            Use the meta-train split of the dataset. If set to `True`, then the
-            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
-            of these three arguments must be set to `True`.
-
-        meta_val : bool (default: `False`)
-            Use the meta-validation split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_test : bool (default: `False`)
-            Use the meta-test split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_split : string in {'train', 'val', 'test'}, optional
-            Name of the split to use. This overrides the arguments `meta_train`,
-            `meta_val` and `meta_test` if all three are set to `False`.
-
-        transform : callable, optional
-            A function/transform that takes a numpy array or a pytorch array
-            (depending when the transforms is applied), and returns a transformed
-            version.
-
-        target_transform : callable, optional
-            A function/transform that takes a target, and returns a transformed
-            version.
-
-        dataset_transform : callable, optional
-            A function/transform that takes a dataset (ie. a task), and returns a
-            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-        class_augmentations : list of callable, optional
-            A list of functions that augment the dataset with new classes. These
-            classes are transformations of existing classes.
-
-        download : bool (default: `False`)
-            If `True`, downloads the original files and processes the dataset in the
-            root directory (under the `one_hundred_plants_margin' folder). If the dataset
-            is already available, this does not download/process the dataset again.
-
-        process_features : bool (default: `False`)
-            If `True`, normalizes each feature f with (f-lower) / (upper - lower) where upper
-            and lower are the min and max values of feature f of the meta-train dataset.
-
-        References
-        -----
-        [1] Charles Mallah, James Cope, James Orwell.
-        Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features.
-        Signal Processing, Pattern Recognition and Applications, in press.
-
-        [2] J. Cope, P. Remagnino, S. Barman, and P. Wilkin.
-        Plant texture classification using gabor co-occurrences.
-        Advances in Visual Computing, pages 699-677, 2010.
-
-        [3] T. Beghin, J. Cope, P. Remagnino, and S. Barman.
-        Shape and texture based plant leaf classification.
-        In: Advanced Concepts for Intelligent Vision Systems, pages 345-353. Springer, 2010.
-
-        """
-        dataset = PlantsMarginClassDataset(root,
-                                           meta_train=meta_train,
-                                           meta_val=meta_val,
-                                           meta_test=meta_test,
-                                           meta_split=meta_split,
-                                           transform=transform,
-                                           class_augmentations=class_augmentations,
-                                           download=download,
-                                           normalize=process_features)
-        super(PlantsMargin, self).__init__(dataset,
-                                           num_classes_per_task,
-                                           target_transform=target_transform,
-                                           dataset_transform=dataset_transform)
-
-
-class PlantsMarginClassDataset(ClassDataset):
-
-    open_ml_id = 1491
-    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
-    dataset_name = "one_hundred_plants_margin"
-
-    folder = "one_hundred_plants_margin"
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-    filename_lower_upper = 'features_lower_upper.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
-                 class_augmentations=None, download=False, normalize=True):
-        super(PlantsMarginClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
-                                                       meta_split=meta_split, class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
-        self.split_filename_lower_upper = os.path.join(self.root, self.filename_lower_upper)
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-        self._lower_upper = None
-
-        if download:
-            self.download(normalize)
-
-        if not self._check_integrity():
-            raise RuntimeError('PlantsMargin integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-        return PlantsMarginDataset(index, data, label, transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    @property
-    def lower_upper(self):
-        if self._lower_upper is None:
-            with open(self.split_filename_lower_upper, 'r') as f:
-                self._lower_upper = json.load(f)
-        return self._lower_upper['lower'], self._lower_upper['upper']
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data is not None:
-            self._data.close()
-            self._data = None
-
-    def download(self, normalize):
-
-        if self._check_integrity():
-            return
-
-        from sklearn.datasets import fetch_openml
-
-        data = fetch_openml(data_id=self.open_ml_id)
-        features = data.data
-        targets = data.target
-
-        os.makedirs(self.root, exist_ok=True)
-
-        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
-        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
-        for s, split in enumerate(['train', 'val', 'test']):
-            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
-
-            is_in_split = [t in targets_assets_split for t in targets]
-            features_split = features.loc[is_in_split]
-            targets_split = targets.loc[is_in_split]
-            assert targets_split.shape[0] == features_split.shape[0]
-
-            unique_targets_split = np.unique(targets_split)
-            if len(targets_assets_split) > unique_targets_split.shape[0]:
-                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
-                      f"given by assets ({len(targets_assets_split)}). Proceeding with unique set of labels.")
-
-            # write unique targets to json file.
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(unique_targets_split.tolist(), f)
-
-            # normalize between 0 and 1 with stats from 'train' split only
-            if split == 'train':
-                lower, upper = np.zeros(features.shape[1]), np.ones(features.shape[1])
-                if normalize:
-                    lower = np.min(features_split, axis=0)
-                    upper = np.max(features_split, axis=0)
-                self._lower_upper = {'lower': lower.tolist(), 'upper': upper.tolist()}
-                lower_upper_filename = os.path.join(self.root, self.filename_lower_upper)
-                with open(lower_upper_filename, 'w') as f:
-                    json.dump(self._lower_upper, f)
-
-            lower, upper = self.lower_upper
-            lower = np.array(lower)
-            upper = np.array(upper)
-            features_split = np.true_divide((features_split - lower), (upper - lower))
-
-            # write data (features and class labels)
-            filename = os.path.join(self.root, self.filename.format(split))
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-
-                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
-                    data_class = features_split.loc[targets_split == label]
-                    group.create_dataset(label, data=data_class)
-
-
-class PlantsMarginDataset(Dataset):
-    def __init__(self, index, data, label, transform=None, target_transform=None):
-        super(PlantsMarginDataset, self).__init__(index, transform=transform, target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        features = self.data[index, :]
-        target = self.label
-
-        if self.transform is not None:
-            features = self.transform(features)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return features, target
-
-
-def create_asset(root='data', fractions=None, seed=42):
-    """This methods creates the assets of the PlantsMargin dataset. These are the meta-dataset splits from the
-    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
-    this directory: torchmeta.datasets.assets.one_hundred_plants_margin. You can also manually change the assets."""
-
-    # split fractions: train, valid, test
-    if fractions is None:
-        fractions = [0.7, 0.15, 0.15]
-    assert sum(fractions) == 1
-
-    from sklearn.datasets import fetch_openml
-
-    data = fetch_openml(data_id=PlantsMarginClassDataset.open_ml_id)
-    unique_targets = np.unique(data.target)
-    num_unique_targets = len(unique_targets)
-
-    num_split = [int(f * num_unique_targets) for f in fractions]
-    num_split[1] = num_unique_targets - num_split[0] - num_split[2]
-    assert sum(num_split) == num_unique_targets
-
-    # split unique labels randomly
-    np.random.seed(seed)
-    perm = np.random.permutation(num_unique_targets)
-    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
-                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
-                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
-
-    # write splits
-    root_path = os.path.join(os.path.expanduser(root), PlantsMarginClassDataset.folder)
-    for split in ["train", "val", "test"]:
-        asset_filename = os.path.join(root_path, "{0}.json".format(split))
-        with open(asset_filename, 'w') as f:
-            json.dump(targets_split[split], f)
+import numpy as np
+import os
+import json
+import h5py
+from tqdm import tqdm
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class PlantsShape(CombinationMetaDataset):
+    """The PlantsShape dataset """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False, process_features=False):
+        """
+        One-hundred plant species leaves dataset (Class = Shape) [1], [2], [3]
+        open-ml-id: 1492
+        https://archive.ics.uci.edu/ml/datasets/One-hundred+plant+species+leaves+data+set) - 2010
+
+
+           (a) Original owners of colour Leaves Samples:
+
+         James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.
+         The colour images are not included.
+         The Leaves were collected in the Royal Botanic Gardens, Kew, UK.
+         email: james.cope@kingston.ac.uk
+
+           (b) This dataset consists of work carried out by James Cope, Charles Mallah, and James Orwell.
+         Donor of database Charles Mallah: charles.mallah@kingston.ac.uk; James Cope:  james.cope@kingston.ac.uk
+
+        The original data directory contains the binary images (masks) of the leaf samples (colour images not included).
+        There are three features for each image: Shape, Margin and Texture.
+        For each feature, a 64 element vector is given per leaf sample.
+        These vectors are taken as a contiguous descriptor (for shape) or histograms (for texture and margin).
+        So, there are three different files, one for each feature problem:
+         * 'data_Sha_64.txt' -> prediction based on shape [dataset provided here]
+         * 'data_Tex_64.txt' -> prediction based on texture
+         * 'data_Mar_64.txt' -> prediction based on margin
+
+        Each row has a 64-element feature vector followed by the Class label.
+        There is a total of 1600 samples with 16 samples per leaf class (100 classes), and no missing values.
+
+        Three 64 element feature vectors per sample.
+
+        Parameters
+        ----------
+        root : string
+            Root directory where the dataset folder `one_hundred_plants_shape` exists.
+
+        num_classes_per_task : int
+            Number of classes per tasks. This corresponds to "N" in "N-way"
+            classification.
+
+        meta_train : bool (default: `False`)
+            Use the meta-train split of the dataset. If set to `True`, then the
+            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
+            of these three arguments must be set to `True`.
+
+        meta_val : bool (default: `False`)
+            Use the meta-validation split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_test : bool (default: `False`)
+            Use the meta-test split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_split : string in {'train', 'val', 'test'}, optional
+            Name of the split to use. This overrides the arguments `meta_train`,
+            `meta_val` and `meta_test` if all three are set to `False`.
+
+        transform : callable, optional
+            A function/transform that takes a numpy array or a pytorch array
+            (depending when the transforms is applied), and returns a transformed
+            version.
+
+        target_transform : callable, optional
+            A function/transform that takes a target, and returns a transformed
+            version.
+
+        dataset_transform : callable, optional
+            A function/transform that takes a dataset (ie. a task), and returns a
+            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+        class_augmentations : list of callable, optional
+            A list of functions that augment the dataset with new classes. These
+            classes are transformations of existing classes.
+
+        download : bool (default: `False`)
+            If `True`, downloads the original files and processes the dataset in the
+            root directory (under the `one_hundred_plants_shape' folder). If the dataset
+            is already available, this does not download/process the dataset again.
+
+        process_features : bool (default: `False`)
+            If `True`, normalizes each feature f according to (f-mean) / (std + 1e-10) where
+            mean and std are the mean and standard deviation of the feature f of the meta-train dataset.
+
+        References
+        -----
+        [1] Charles Mallah, James Cope, James Orwell.
+        Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features.
+        Signal Processing, Pattern Recognition and Applications, in press.
+
+        [2] J. Cope, P. Remagnino, S. Barman, and P. Wilkin.
+        Plant texture classification using gabor co-occurrences.
+        Advances in Visual Computing, pages 699-677, 2010.
+
+        [3] T. Beghin, J. Cope, P. Remagnino, and S. Barman.
+        Shape and texture based plant leaf classification.
+        In: Advanced Concepts for Intelligent Vision Systems, pages 345-353. Springer, 2010.
+
+        """
+        dataset = PlantsShapeClassDataset(root,
+                                          meta_train=meta_train,
+                                          meta_val=meta_val,
+                                          meta_test=meta_test,
+                                          meta_split=meta_split,
+                                          transform=transform,
+                                          class_augmentations=class_augmentations,
+                                          download=download,
+                                          normalize=process_features)
+        super(PlantsShape, self).__init__(dataset,
+                                            num_classes_per_task,
+                                            target_transform=target_transform,
+                                            dataset_transform=dataset_transform)
+
+
+class PlantsShapeClassDataset(ClassDataset):
+
+    open_ml_id = 1492
+    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
+    dataset_name = "one_hundred_plants_shape"
+
+    folder = "one_hundred_plants_shape"
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+    filename_mean_std = 'features_mean_std.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
+                 class_augmentations=None, download=False, normalize=True):
+        super(PlantsShapeClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
+                                                      meta_split=meta_split, class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
+        self.split_filename_mean_std = os.path.join(self.root, self.filename_mean_std)
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+        self._mean_std = None
+
+        if download:
+            self.download(normalize)
+
+        if not self._check_integrity():
+            raise RuntimeError('PlantsShape integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+        return PlantsShapeDataset(index, data, label, transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    @property
+    def mean_std(self):
+        if self._mean_std is None:
+            with open(self.split_filename_mean_std, 'r') as f:
+                self._mean_std = json.load(f)
+        return self._mean_std
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data is not None:
+            self._data.close()
+            self._data = None
+
+    def download(self, normalize):
+
+        if self._check_integrity():
+            return
+
+        from sklearn.datasets import fetch_openml
+
+        data = fetch_openml(data_id=self.open_ml_id)
+        features = data.data
+        targets = data.target
+
+        os.makedirs(self.root, exist_ok=True)
+
+        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
+        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
+        for s, split in enumerate(['train', 'val', 'test']):
+            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
+
+            is_in_split = [t in targets_assets_split for t in targets]
+            features_split = features.loc[is_in_split]
+            targets_split = targets.loc[is_in_split]
+            assert targets_split.shape[0] == features_split.shape[0]
+
+            unique_targets_split = np.sort(np.unique(targets_split))
+            if len(targets_assets_split) > unique_targets_split.shape[0]:
+                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
+                      f"given by assets ({len(targets_assets_split)}). Proceeding with unique set of labels.")
+
+            # write unique targets to json file.
+            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(unique_targets_split.tolist(), f)
+
+            # normalize to zero mean and standard deviation 1 with stats from 'train' split only
+            if split == 'train':
+                mean, std = np.zeros(features.shape[1]), np.ones(features.shape[1])
+                if normalize:
+                    mean = np.mean(features_split, axis=0)
+                    std = np.std(features_split, axis=0)
+
+                self._mean_std = {'mean': mean.tolist(), 'std': std.tolist()}
+                mean_std_filename = os.path.join(self.root, self.filename_mean_std)
+                with open(mean_std_filename, 'w') as f:
+                    json.dump(self._mean_std, f)
+
+            mean_std = self.mean_std
+            mean = np.array(mean_std['mean'])
+            std = np.array(mean_std['std'])
+            features_split = (features_split - mean) / (std + 1e-10)
+
+            # write data (features and class labels)
+            filename = os.path.join(self.root, self.filename.format(split))
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+
+                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
+                    data_class = features_split.loc[targets_split == label]
+                    group.create_dataset(label, data=data_class)
+
+
+class PlantsShapeDataset(Dataset):
+    def __init__(self, index, data, label, transform=None, target_transform=None):
+        super(PlantsShapeDataset, self).__init__(index, transform=transform, target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        features = self.data[index, :]
+        target = self.label
+
+        if self.transform is not None:
+            features = self.transform(features)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return features, target
+
+
+def create_asset(root='data', fractions=None, seed=42):
+    """This methods creates the assets of the PlantsShape dataset. These are the meta-dataset splits from the
+    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
+    this directory: torchmeta.datasets.assets.one_hundred_plants_shape. You can also manually change the assets."""
+
+    # split fractions: train, valid, test
+    if fractions is None:
+        fractions = [0.7, 0.15, 0.15]
+    assert sum(fractions) == 1
+
+    from sklearn.datasets import fetch_openml
+
+    data = fetch_openml(data_id=PlantsShapeClassDataset.open_ml_id)
+    unique_targets = np.unique(data.target)
+    num_unique_targets = len(unique_targets)
+
+    num_split = [int(f * num_unique_targets) for f in fractions]
+    num_split[1] = num_unique_targets - num_split[0] - num_split[2]
+    assert sum(num_split) == num_unique_targets
+
+    # split unique labels randomly
+    np.random.seed(seed)
+    perm = np.random.permutation(num_unique_targets)
+    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
+                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
+                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
+
+    # write splits
+    root_path = os.path.join(os.path.expanduser(root), PlantsShapeClassDataset.folder)
+    for split in ["train", "val", "test"]:
+        asset_filename = os.path.join(root_path, "{0}.json".format(split))
+        with open(asset_filename, 'w') as f:
+            json.dump(targets_split[split], f)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,320 +1,319 @@
-import numpy as np
-import os
-import json
-import h5py
-from tqdm import tqdm
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class PlantsShape(CombinationMetaDataset):
-    """The PlantsShape dataset """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False, process_features=False):
-        """
-        One-hundred plant species leaves dataset (Class = Shape) [1], [2], [3]
-        open-ml-id: 1492
-        https://archive.ics.uci.edu/ml/datasets/One-hundred+plant+species+leaves+data+set) - 2010
-
-
-           (a) Original owners of colour Leaves Samples:
-
-         James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.
-         The colour images are not included.
-         The Leaves were collected in the Royal Botanic Gardens, Kew, UK.
-         email: james.cope@kingston.ac.uk
-
-           (b) This dataset consists of work carried out by James Cope, Charles Mallah, and James Orwell.
-         Donor of database Charles Mallah: charles.mallah@kingston.ac.uk; James Cope:  james.cope@kingston.ac.uk
-
-        The original data directory contains the binary images (masks) of the leaf samples (colour images not included).
-        There are three features for each image: Shape, Margin and Texture.
-        For each feature, a 64 element vector is given per leaf sample.
-        These vectors are taken as a contiguous descriptor (for shape) or histograms (for texture and margin).
-        So, there are three different files, one for each feature problem:
-         * 'data_Sha_64.txt' -> prediction based on shape [dataset provided here]
-         * 'data_Tex_64.txt' -> prediction based on texture
-         * 'data_Mar_64.txt' -> prediction based on margin
-
-        Each row has a 64-element feature vector followed by the Class label.
-        There is a total of 1600 samples with 16 samples per leaf class (100 classes), and no missing values.
-
-        Three 64 element feature vectors per sample.
-
-        Parameters
-        ----------
-        root : string
-            Root directory where the dataset folder `one_hundred_plants_shape` exists.
-
-        num_classes_per_task : int
-            Number of classes per tasks. This corresponds to "N" in "N-way"
-            classification.
-
-        meta_train : bool (default: `False`)
-            Use the meta-train split of the dataset. If set to `True`, then the
-            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
-            of these three arguments must be set to `True`.
-
-        meta_val : bool (default: `False`)
-            Use the meta-validation split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_test : bool (default: `False`)
-            Use the meta-test split of the dataset. If set to `True`, then the
-            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-            one of these three arguments must be set to `True`.
-
-        meta_split : string in {'train', 'val', 'test'}, optional
-            Name of the split to use. This overrides the arguments `meta_train`,
-            `meta_val` and `meta_test` if all three are set to `False`.
-
-        transform : callable, optional
-            A function/transform that takes a numpy array or a pytorch array
-            (depending when the transforms is applied), and returns a transformed
-            version.
-
-        target_transform : callable, optional
-            A function/transform that takes a target, and returns a transformed
-            version.
-
-        dataset_transform : callable, optional
-            A function/transform that takes a dataset (ie. a task), and returns a
-            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-        class_augmentations : list of callable, optional
-            A list of functions that augment the dataset with new classes. These
-            classes are transformations of existing classes.
-
-        download : bool (default: `False`)
-            If `True`, downloads the original files and processes the dataset in the
-            root directory (under the `one_hundred_plants_shape' folder). If the dataset
-            is already available, this does not download/process the dataset again.
-
-        process_features : bool (default: `False`)
-            If `True`, normalizes each feature f according to (f-mean) / (std + 1e-10) where
-            mean and std are the mean and standard deviation of the feature f of the meta-train dataset.
-
-        References
-        -----
-        [1] Charles Mallah, James Cope, James Orwell.
-        Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features.
-        Signal Processing, Pattern Recognition and Applications, in press.
-
-        [2] J. Cope, P. Remagnino, S. Barman, and P. Wilkin.
-        Plant texture classification using gabor co-occurrences.
-        Advances in Visual Computing, pages 699-677, 2010.
-
-        [3] T. Beghin, J. Cope, P. Remagnino, and S. Barman.
-        Shape and texture based plant leaf classification.
-        In: Advanced Concepts for Intelligent Vision Systems, pages 345-353. Springer, 2010.
-
-        """
-        dataset = PlantsShapeClassDataset(root,
-                                          meta_train=meta_train,
-                                          meta_val=meta_val,
-                                          meta_test=meta_test,
-                                          meta_split=meta_split,
-                                          transform=transform,
-                                          class_augmentations=class_augmentations,
-                                          download=download,
-                                          normalize=process_features)
-        super(PlantsShape, self).__init__(dataset,
-                                            num_classes_per_task,
-                                            target_transform=target_transform,
-                                            dataset_transform=dataset_transform)
-
-
-class PlantsShapeClassDataset(ClassDataset):
-
-    open_ml_id = 1492
-    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
-    dataset_name = "one_hundred_plants_shape"
-
-    folder = "one_hundred_plants_shape"
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-    filename_mean_std = 'features_mean_std.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
-                 class_augmentations=None, download=False, normalize=True):
-        super(PlantsShapeClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
-                                                      meta_split=meta_split, class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
-        self.split_filename_mean_std = os.path.join(self.root, self.filename_mean_std)
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-        self._mean_std = None
-
-        if download:
-            self.download(normalize)
-
-        if not self._check_integrity():
-            raise RuntimeError('PlantsShape integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-        return PlantsShapeDataset(index, data, label, transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    @property
-    def mean_std(self):
-        if self._mean_std is None:
-            with open(self.split_filename_mean_std, 'r') as f:
-                self._mean_std = json.load(f)
-        return self._mean_std
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data is not None:
-            self._data.close()
-            self._data = None
-
-    def download(self, normalize):
-
-        if self._check_integrity():
-            return
-
-        from sklearn.datasets import fetch_openml
-
-        data = fetch_openml(data_id=self.open_ml_id)
-        features = data.data
-        targets = data.target
-
-        os.makedirs(self.root, exist_ok=True)
-
-        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
-        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
-        for s, split in enumerate(['train', 'val', 'test']):
-            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
-
-            is_in_split = [t in targets_assets_split for t in targets]
-            features_split = features.loc[is_in_split]
-            targets_split = targets.loc[is_in_split]
-            assert targets_split.shape[0] == features_split.shape[0]
-
-            unique_targets_split = np.sort(np.unique(targets_split))
-            if len(targets_assets_split) > unique_targets_split.shape[0]:
-                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
-                      f"given by assets ({len(targets_assets_split)}). Proceeding with unique set of labels.")
-
-            # write unique targets to json file.
-            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(unique_targets_split.tolist(), f)
-
-            # normalize to zero mean and standard deviation 1 with stats from 'train' split only
-            if split == 'train':
-                mean, std = np.zeros(features.shape[1]), np.ones(features.shape[1])
-                if normalize:
-                    mean = np.mean(features_split, axis=0)
-                    std = np.std(features_split, axis=0)
-
-                self._mean_std = {'mean': mean.tolist(), 'std': std.tolist()}
-                mean_std_filename = os.path.join(self.root, self.filename_mean_std)
-                with open(mean_std_filename, 'w') as f:
-                    json.dump(self._mean_std, f)
-
-            mean_std = self.mean_std
-            mean = np.array(mean_std['mean'])
-            std = np.array(mean_std['std'])
-            features_split = (features_split - mean) / (std + 1e-10)
-
-            # write data (features and class labels)
-            filename = os.path.join(self.root, self.filename.format(split))
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-
-                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
-                    data_class = features_split.loc[targets_split == label]
-                    group.create_dataset(label, data=data_class)
-
-
-class PlantsShapeDataset(Dataset):
-    def __init__(self, index, data, label, transform=None, target_transform=None):
-        super(PlantsShapeDataset, self).__init__(index, transform=transform, target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        features = self.data[index, :]
-        target = self.label
-
-        if self.transform is not None:
-            features = self.transform(features)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return features, target
-
-
-def create_asset(root='data', fractions=None, seed=42):
-    """This methods creates the assets of the PlantsShape dataset. These are the meta-dataset splits from the
-    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
-    this directory: torchmeta.datasets.assets.one_hundred_plants_shape. You can also manually change the assets."""
-
-    # split fractions: train, valid, test
-    if fractions is None:
-        fractions = [0.7, 0.15, 0.15]
-    assert sum(fractions) == 1
-
-    from sklearn.datasets import fetch_openml
-
-    data = fetch_openml(data_id=PlantsShapeClassDataset.open_ml_id)
-    unique_targets = np.unique(data.target)
-    num_unique_targets = len(unique_targets)
-
-    num_split = [int(f * num_unique_targets) for f in fractions]
-    num_split[1] = num_unique_targets - num_split[0] - num_split[2]
-    assert sum(num_split) == num_unique_targets
-
-    # split unique labels randomly
-    np.random.seed(seed)
-    perm = np.random.permutation(num_unique_targets)
-    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
-                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
-                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
-
-    # write splits
-    root_path = os.path.join(os.path.expanduser(root), PlantsShapeClassDataset.folder)
-    for split in ["train", "val", "test"]:
-        asset_filename = os.path.join(root_path, "{0}.json".format(split))
-        with open(asset_filename, 'w') as f:
-            json.dump(targets_split[split], f)
+import numpy as np
+import os
+import json
+import h5py
+from tqdm import tqdm
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class PlantsTexture(CombinationMetaDataset):
+    """The PlantsTexture dataset """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False, process_features=False):
+        """
+        One-hundred plant species leaves dataset (Class = Texture) [1], [2], [3]
+        open-ml-id: 1493
+        https://archive.ics.uci.edu/ml/datasets/One-hundred+plant+species+leaves+data+set) - 2010
+
+
+           (a) Original owners of colour Leaves Samples:
+
+         James Cope, Thibaut Beghin, Paolo Remagnino, Sarah Barman.
+         The colour images are not included.
+         The Leaves were collected in the Royal Botanic Gardens, Kew, UK.
+         email: james.cope@kingston.ac.uk
+
+           (b) This dataset consists of work carried out by James Cope, Charles Mallah, and James Orwell.
+         Donor of database Charles Mallah: charles.mallah@kingston.ac.uk; James Cope:  james.cope@kingston.ac.uk
+
+        The original data directory contains the binary images (masks) of the leaf samples (colour images not included).
+        There are three features for each image: Shape, Margin and Texture.
+        For each feature, a 64 element vector is given per leaf sample.
+        These vectors are taken as a contiguous descriptor (for shape) or histograms (for texture and margin).
+        So, there are three different files, one for each feature problem:
+         * 'data_Sha_64.txt' -> prediction based on shape
+         * 'data_Tex_64.txt' -> prediction based on texture [dataset provided here]
+         * 'data_Mar_64.txt' -> prediction based on margin
+
+        Each row has a 64-element feature vector followed by the Class label.
+        There is a total of 1600 samples with 16 samples per leaf class (100 classes), and no missing values.
+
+        Three 64 element feature vectors per sample.
+
+        Parameters
+        ----------
+        root : string
+            Root directory where the dataset folder `one_hundred_plants_texture` exists.
+
+        num_classes_per_task : int
+            Number of classes per tasks. This corresponds to "N" in "N-way"
+            classification.
+
+        meta_train : bool (default: `False`)
+            Use the meta-train split of the dataset. If set to `True`, then the
+            arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
+            of these three arguments must be set to `True`.
+
+        meta_val : bool (default: `False`)
+            Use the meta-validation split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_test : bool (default: `False`)
+            Use the meta-test split of the dataset. If set to `True`, then the
+            arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+            one of these three arguments must be set to `True`.
+
+        meta_split : string in {'train', 'val', 'test'}, optional
+            Name of the split to use. This overrides the arguments `meta_train`,
+            `meta_val` and `meta_test` if all three are set to `False`.
+
+        transform : callable, optional
+            A function/transform that takes a numpy array or a pytorch array
+            (depending when the transforms is applied), and returns a transformed
+            version.
+
+        target_transform : callable, optional
+            A function/transform that takes a target, and returns a transformed
+            version.
+
+        dataset_transform : callable, optional
+            A function/transform that takes a dataset (ie. a task), and returns a
+            transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+        class_augmentations : list of callable, optional
+            A list of functions that augment the dataset with new classes. These
+            classes are transformations of existing classes.
+
+        download : bool (default: `False`)
+            If `True`, downloads the original files and processes the dataset in the
+            root directory (under the `one_hundred_plants_texture' folder). If the dataset
+            is already available, this does not download/process the dataset again.
+
+        process_features : bool (default: `False`)
+            If `True`, normalizes each feature f with (f-lower) / (upper - lower) where upper
+            and lower are the min and max values of feature f of the meta-train dataset.
+
+        References
+        -----
+        [1] Charles Mallah, James Cope, James Orwell.
+        Plant Leaf Classification Using Probabilistic Integration of Shape, Texture and Margin Features.
+        Signal Processing, Pattern Recognition and Applications, in press.
+
+        [2] J. Cope, P. Remagnino, S. Barman, and P. Wilkin.
+        Plant texture classification using gabor co-occurrences.
+        Advances in Visual Computing, pages 699-677, 2010.
+
+        [3] T. Beghin, J. Cope, P. Remagnino, and S. Barman.
+        Shape and texture based plant leaf classification.
+        In: Advanced Concepts for Intelligent Vision Systems, pages 345-353. Springer, 2010.
+
+        """
+        dataset = PlantsTextureClassDataset(root,
+                                            meta_train=meta_train,
+                                            meta_val=meta_val,
+                                            meta_test=meta_test,
+                                            meta_split=meta_split,
+                                            transform=transform,
+                                            class_augmentations=class_augmentations,
+                                            download=download,
+                                            normalize=process_features)
+        super(PlantsTexture, self).__init__(dataset,
+                                            num_classes_per_task,
+                                            target_transform=target_transform,
+                                            dataset_transform=dataset_transform)
+
+
+class PlantsTextureClassDataset(ClassDataset):
+
+    open_ml_id = 1493
+    open_ml_url = 'https://www.openml.org/d/' + str(open_ml_id)
+    dataset_name = "one_hundred_plants_texture"
+
+    folder = "one_hundred_plants_texture"
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+    filename_lower_upper = 'features_lower_upper.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None, transform=None,
+                 class_augmentations=None, download=False, normalize=True):
+        super(PlantsTextureClassDataset, self).__init__(meta_train=meta_train, meta_val=meta_val, meta_test=meta_test,
+                                                        meta_split=meta_split, class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root, self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root, self.filename_labels.format(self.meta_split))
+        self.split_filename_lower_upper = os.path.join(self.root, self.filename_lower_upper)
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+        self._lower_upper = None
+
+        if download:
+            self.download(normalize)
+
+        if not self._check_integrity():
+            raise RuntimeError('PlantsTexture integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+        return PlantsTextureDataset(index, data, label, transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    @property
+    def lower_upper(self):
+        if self._lower_upper is None:
+            with open(self.split_filename_lower_upper, 'r') as f:
+                self._lower_upper = json.load(f)
+        return self._lower_upper
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data is not None:
+            self._data.close()
+            self._data = None
+
+    def download(self, normalize):
+
+        if self._check_integrity():
+            return
+
+        from sklearn.datasets import fetch_openml
+
+        data = fetch_openml(data_id=self.open_ml_id)
+        features = data.data
+        targets = data.target
+
+        os.makedirs(self.root, exist_ok=True)
+
+        # for each meta-data-split, get the labels, then check which data-point belongs to the set (via a mask).
+        # then, retrieve the features and targets belonging to the set. Then create hdf5 file for these features.
+        for s, split in enumerate(['train', 'val', 'test']):
+            targets_assets_split = get_asset(self.folder, '{0}.json'.format(split))
+
+            is_in_split = [t in targets_assets_split for t in targets]
+            features_split = features.loc[is_in_split]
+            targets_split = targets.loc[is_in_split]
+            assert targets_split.shape[0] == features_split.shape[0]
+
+            unique_targets_split = np.unique(targets_split)
+            if len(targets_assets_split) > unique_targets_split.shape[0]:
+                print(f"unique set of labels ({(unique_targets_split.shape[0])}) is smaller than set of labels "
+                      f"given by assets ({len(targets_assets_split)}). Proceeding with unique set of labels.")
+
+            # write unique targets to json file.
+            labels_filename = os.path.join(self.root, self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(unique_targets_split.tolist(), f)
+
+            # normalize between 0 and 1 with stats from 'train' split only
+            if split == 'train':
+                lower, upper = np.zeros(features.shape[1]), np.ones(features.shape[1])
+                if normalize:
+                    lower = np.min(features_split, axis=0)
+                    upper = np.max(features_split, axis=0)
+                self._lower_upper = {'lower': lower.tolist(), 'upper': upper.tolist()}
+                lower_upper_filename = os.path.join(self.root, self.filename_lower_upper)
+                with open(lower_upper_filename, 'w') as f:
+                    json.dump(self._lower_upper, f)
+
+            lower_upper = self.lower_upper
+            lower = np.array(lower_upper['lower'])
+            upper = np.array(lower_upper['upper'])
+            features_split = np.true_divide((features_split - lower), (upper - lower))
+
+            # write data (features and class labels)
+            filename = os.path.join(self.root, self.filename.format(split))
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+
+                for i, label in enumerate(tqdm(unique_targets_split, desc=filename)):
+                    data_class = features_split.loc[targets_split == label]
+                    group.create_dataset(label, data=data_class)
+
+
+class PlantsTextureDataset(Dataset):
+    def __init__(self, index, data, label, transform=None, target_transform=None):
+        super(PlantsTextureDataset, self).__init__(index, transform=transform, target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        features = self.data[index, :]
+        target = self.label
+
+        if self.transform is not None:
+            features = self.transform(features)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return features, target
+
+
+def create_asset(root='data', fractions=None, seed=42):
+    """This methods creates the assets of the PlantsTexture dataset. These are the meta-dataset splits from the
+    original data. Only run this method in case you want to create new assets. Once created, copy the assets to
+    this directory: torchmeta.datasets.assets.one_hundred_plants_texture. You can also manually change the assets."""
+
+    # split fractions: train, valid, test
+    if fractions is None:
+        fractions = [0.7, 0.15, 0.15]
+    assert sum(fractions) == 1
+
+    from sklearn.datasets import fetch_openml
+
+    data = fetch_openml(data_id=PlantsTextureClassDataset.open_ml_id)
+    unique_targets = np.unique(data.target)
+    num_unique_targets = len(unique_targets)
+
+    num_split = [int(f * num_unique_targets) for f in fractions]
+    num_split[1] = num_unique_targets - num_split[0] - num_split[2]
+    assert sum(num_split) == num_unique_targets
+
+    # split unique labels randomly
+    np.random.seed(seed)
+    perm = np.random.permutation(num_unique_targets)
+    targets_split = {'train': [unique_targets[i] for i in perm[:num_split[0]]],
+                     'val': [unique_targets[i] for i in perm[num_split[0]: num_split[0] + num_split[1]]],
+                     'test': [unique_targets[i] for i in perm[num_split[0] + num_split[1]:]]}
+
+    # write splits
+    root_path = os.path.join(os.path.expanduser(root), PlantsTextureClassDataset.folder)
+    for split in ["train", "val", "test"]:
+        asset_filename = os.path.join(root_path, "{0}.json".format(split))
+        with open(asset_filename, 'w') as f:
+            json.dump(targets_split[split], f)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-"""
-;==========================================
-; Title: Pascal-5i Dataset for Few-shot Object Segmentation
-; Author: Mennatullah Siam
-; Company: Huawei Technologies
-; Date:   18 March 2020
-;==========================================
-"""
-import os
-import json
-import glob
-import h5py
-from PIL import Image, ImageOps
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-from torchvision.datasets.utils import list_dir, download_url
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-import numpy as np
-
-class Pascal5i(CombinationMetaDataset):
-    """
-    Pascal5i dataset [1]. A dataset for few-shot object segmentation supporting 4 folds
-    each fold has 15 training classes and 5 testing classes.
-    Using Preprocessed Masks from [2]
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `omniglot` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way"
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`,
-        and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes
-        are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the zip files and processes the dataset in the root
-        directory (under the `omniglot` folder). If the dataset is already
-        available, this does not download/process the dataset again.
-
-    fold : int (default: 0)
-        Fold number ranges between 0-3 that controls training(15) and testing(5) classes.
-
-    Notes
-    -----
-    Currently Only 1-way is supported
-
-    References
-    ----------
-    .. [1] Shaban, Amirreza, et al. "One-shot learning for semantic segmentation."
-            arXiv preprint arXiv:1709.03410 (2017).
-    .. [2] Zhang, Chi, et al. "Canet: Class-agnostic segmentation networks with
-            iterative refinement and attentive few-shot learning."
-            Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019.
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_test=False, meta_split=None,
-                 transform=None, target_transform=None,
-                 dataset_transform=None, class_augmentations=None,
-                 download=False, fold=0):
-
-        dataset = Pascal5iClassDataset(root, meta_train=meta_train,
-                                       meta_test=meta_test, transform=transform,
-                                       meta_split=meta_split, class_augmentations=class_augmentations,
-                                       download=download, fold=fold)
-
-        super(Pascal5i, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-class Pascal5iClassDataset(ClassDataset):
-    folder = 'pascal5i'
-
-    downloads = [
-    {
-        'url' : 'http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar',
-        'filename' : 'VOCtrainval_11-May-2012.tar',
-        'md5' : '6cd6e144f989b92b3379bac3b3de84fd'
-    },
-    {
-        'url' : 'https://github.com/icoz69/CaNet/raw/master/Binary_map_aug.zip',
-        'filename': 'Binary_map_aug.zip',
-        'md5': None
-    },
-    {
-        'url' : 'https://raw.github.com/NVIDIA/DIGITS/master/examples/semantic-segmentation/pascal-voc-classes.txt',
-        'filename' : 'pascal-voc-classes.txt',
-        'md5' : None
-    }
-    ]
-    split_filename_labels = 'pascal-voc-classes.txt'
-
-    def __init__(self, root, meta_train=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False, fold=0):
-
-        super(Pascal5iClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=False, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.fold = fold
-
-        self._data = None
-        self._labels = None
-        self._masks = None
-
-        if download:
-            self.download()
-
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        class_name = self.labels[index % self.num_classes]
-        data, masks = self.data[0][class_name], self.data[1][class_name]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-        class_id = self.read_labels().index(class_name)
-
-        return PascalDataset(index, (data, masks), class_id,
-            transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    def load_dict_per_class(self):
-        new_exist_class_list = {}
-
-        if self.meta_split == 'train':
-            fold_list=[0, 1, 2, 3]
-            fold_list.remove(self.fold)
-        else:
-            fold_list = [self.fold]
-
-        for fold in fold_list:
-            f = open(os.path.join(self.root, 'Binary_map_aug', self.meta_split,
-                                  'split%1d_%s.txt'%(fold, self.meta_split)))
-            while True:
-                item = f.readline()
-                if item == '':
-                    break
-                img_name = item[:11]
-                cat = int(item[13:15])
-                if cat not in new_exist_class_list:
-                    new_exist_class_list[cat] = []
-                new_exist_class_list[cat].append(img_name)
-
-        images = {}
-        masks = {}
-        classes_names = self.read_labels()
-
-        for k, v in new_exist_class_list.items():
-            cname = classes_names[k]
-            for path in v:
-                fname = os.path.join(self.root, 'VOCdevkit/VOC2012/JPEGImages', path + '.jpg')
-                if cname not in images:
-                    images[cname] = []
-                images[cname].append(fname)
-                fname = os.path.join(self.root, 'Binary_map_aug', self.meta_split, str(k),
-                                               path + '.png')
-                if cname not in masks:
-                    masks[cname] = []
-                masks[cname].append(fname)
-        return images, masks
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data, self._masks = self.load_dict_per_class()
-        return self._data, self._masks
-
-    def read_labels(self, fold=None):
-        labels = []
-        if fold is not None:
-            if self.meta_train:
-                in_classes = set(range(21)) - \
-                                set(range(fold*5+1, (fold+1)*5+1))
-            else:
-                in_classes = set(range(fold*5+1, (fold+1)*5+1))
-        else:
-            in_classes = set(range(21))
-
-        with open(os.path.join(self.root, self.split_filename_labels), 'r') as f:
-            for it, line in enumerate(f):
-                if line.strip() == '':
-                    break
-                if it in in_classes:
-                    labels.append(line.strip())
-        return labels
-
-    @property
-    def labels(self):
-        if self._labels is None:
-           self._labels = self.read_labels(self.fold)
-        return self._labels[1:]
-
-    def download(self):
-        import zipfile
-        import tarfile
-        import shutil
-
-        for dload in self.downloads:
-            filename = os.path.join(self.root, dload['filename'])
-            if os.path.isfile(filename):
-                continue
-
-            download_url(dload['url'], self.root, dload['filename'], dload['md5'])
-
-            if 'zip' in dload['filename']:
-                with zipfile.ZipFile(filename, 'r') as f:
-                    f.extractall(self.root)
-            elif 'tar' in dload['filename']:
-                with tarfile.open(filename, 'r') as f:
-                    f.extractall(self.root)
-
-class PascalDataset(Dataset):
-    def __init__(self, index, data, class_id,
-                 transform=None, target_transform=None):
-        super(PascalDataset, self).__init__(index, transform=transform,
-            target_transform=target_transform)
-        self.data, self.masks = data
-        self.class_id = class_id
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        image = Image.open(self.data[index])
-        mask = Image.open(self.masks[index])
-        target = self.class_id
-
-        if self.transform is not None:
-            image, mask = self.transform(image, mask)
-
-        return (image, mask, target)
+"""
+;==========================================
+; Title: Pascal-5i Dataset for Few-shot Object Segmentation
+; Author: Mennatullah Siam
+; Company: Huawei Technologies
+; Date:   18 March 2020
+;==========================================
+"""
+import os
+import json
+import glob
+import h5py
+from PIL import Image, ImageOps
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+from torchvision.datasets.utils import list_dir, download_url
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+import numpy as np
+
+class Pascal5i(CombinationMetaDataset):
+    """
+    Pascal5i dataset [1]. A dataset for few-shot object segmentation supporting 4 folds
+    each fold has 15 training classes and 5 testing classes.
+    Using Preprocessed Masks from [2]
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `omniglot` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way"
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`,
+        and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes
+        are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the zip files and processes the dataset in the root
+        directory (under the `omniglot` folder). If the dataset is already
+        available, this does not download/process the dataset again.
+
+    fold : int (default: 0)
+        Fold number ranges between 0-3 that controls training(15) and testing(5) classes.
+
+    Notes
+    -----
+    Currently Only 1-way is supported
+
+    References
+    ----------
+    .. [1] Shaban, Amirreza, et al. "One-shot learning for semantic segmentation."
+            arXiv preprint arXiv:1709.03410 (2017).
+    .. [2] Zhang, Chi, et al. "Canet: Class-agnostic segmentation networks with
+            iterative refinement and attentive few-shot learning."
+            Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2019.
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_test=False, meta_split=None,
+                 transform=None, target_transform=None,
+                 dataset_transform=None, class_augmentations=None,
+                 download=False, fold=0):
+
+        dataset = Pascal5iClassDataset(root, meta_train=meta_train,
+                                       meta_test=meta_test, transform=transform,
+                                       meta_split=meta_split, class_augmentations=class_augmentations,
+                                       download=download, fold=fold)
+
+        super(Pascal5i, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+class Pascal5iClassDataset(ClassDataset):
+    folder = 'pascal5i'
+
+    downloads = [
+    {
+        'url' : 'http://host.robots.ox.ac.uk/pascal/VOC/voc2012/VOCtrainval_11-May-2012.tar',
+        'filename' : 'VOCtrainval_11-May-2012.tar',
+        'md5' : '6cd6e144f989b92b3379bac3b3de84fd'
+    },
+    {
+        'url' : 'https://github.com/icoz69/CaNet/raw/master/Binary_map_aug.zip',
+        'filename': 'Binary_map_aug.zip',
+        'md5': None
+    },
+    {
+        'url' : 'https://raw.github.com/NVIDIA/DIGITS/master/examples/semantic-segmentation/pascal-voc-classes.txt',
+        'filename' : 'pascal-voc-classes.txt',
+        'md5' : None
+    }
+    ]
+    split_filename_labels = 'pascal-voc-classes.txt'
+
+    def __init__(self, root, meta_train=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False, fold=0):
+
+        super(Pascal5iClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=False, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.fold = fold
+
+        self._data = None
+        self._labels = None
+        self._masks = None
+
+        if download:
+            self.download()
+
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        class_name = self.labels[index % self.num_classes]
+        data, masks = self.data[0][class_name], self.data[1][class_name]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+        class_id = self.read_labels().index(class_name)
+
+        return PascalDataset(index, (data, masks), class_id,
+            transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    def load_dict_per_class(self):
+        new_exist_class_list = {}
+
+        if self.meta_split == 'train':
+            fold_list=[0, 1, 2, 3]
+            fold_list.remove(self.fold)
+        else:
+            fold_list = [self.fold]
+
+        for fold in fold_list:
+            f = open(os.path.join(self.root, 'Binary_map_aug', self.meta_split,
+                                  'split%1d_%s.txt'%(fold, self.meta_split)))
+            while True:
+                item = f.readline()
+                if item == '':
+                    break
+                img_name = item[:11]
+                cat = int(item[13:15])
+                if cat not in new_exist_class_list:
+                    new_exist_class_list[cat] = []
+                new_exist_class_list[cat].append(img_name)
+
+        images = {}
+        masks = {}
+        classes_names = self.read_labels()
+
+        for k, v in new_exist_class_list.items():
+            cname = classes_names[k]
+            for path in v:
+                fname = os.path.join(self.root, 'VOCdevkit/VOC2012/JPEGImages', path + '.jpg')
+                if cname not in images:
+                    images[cname] = []
+                images[cname].append(fname)
+                fname = os.path.join(self.root, 'Binary_map_aug', self.meta_split, str(k),
+                                               path + '.png')
+                if cname not in masks:
+                    masks[cname] = []
+                masks[cname].append(fname)
+        return images, masks
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data, self._masks = self.load_dict_per_class()
+        return self._data, self._masks
+
+    def read_labels(self, fold=None):
+        labels = []
+        if fold is not None:
+            if self.meta_train:
+                in_classes = set(range(21)) - \
+                                set(range(fold*5+1, (fold+1)*5+1))
+            else:
+                in_classes = set(range(fold*5+1, (fold+1)*5+1))
+        else:
+            in_classes = set(range(21))
+
+        with open(os.path.join(self.root, self.split_filename_labels), 'r') as f:
+            for it, line in enumerate(f):
+                if line.strip() == '':
+                    break
+                if it in in_classes:
+                    labels.append(line.strip())
+        return labels
+
+    @property
+    def labels(self):
+        if self._labels is None:
+           self._labels = self.read_labels(self.fold)
+        return self._labels[1:]
+
+    def download(self):
+        import zipfile
+        import tarfile
+        import shutil
+
+        for dload in self.downloads:
+            filename = os.path.join(self.root, dload['filename'])
+            if os.path.isfile(filename):
+                continue
+
+            download_url(dload['url'], self.root, dload['filename'], dload['md5'])
+
+            if 'zip' in dload['filename']:
+                with zipfile.ZipFile(filename, 'r') as f:
+                    f.extractall(self.root)
+            elif 'tar' in dload['filename']:
+                with tarfile.open(filename, 'r') as f:
+                    f.extractall(self.root)
+
+class PascalDataset(Dataset):
+    def __init__(self, index, data, class_id,
+                 transform=None, target_transform=None):
+        super(PascalDataset, self).__init__(index, transform=transform,
+            target_transform=target_transform)
+        self.data, self.masks = data
+        self.class_id = class_id
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        image = Image.open(self.data[index])
+        mask = Image.open(self.masks[index])
+        target = self.class_id
+
+        if self.transform is not None:
+            image, mask = self.transform(image, mask)
+
+        return (image, mask, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/tcga.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tcga.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,528 +1,528 @@
-import os
-import json
-import h5py
-import numpy as np
-import torch
-import copy
-
-from ordered_set import OrderedSet
-from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class TCGA(MetaDataset):
-    """
-    The TCGA dataset [1]. A dataset of classification tasks over the values of
-    an attribute, based on the gene expression data from patients diagnosed with
-    specific types of cancer. This dataset is based on data from the Cancer
-    Genome Atlas Program from the National Cancer Institute.
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `omniglot` exists.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    min_samples_per_class : int (default: 5)
-        Minimum number of samples per class in each classification task. This
-        filters tasks for which the amount of data for one of the classes is
-        too small.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `transforms.ClassSplitter()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the files and processes the dataset in the root 
-        directory (under the `tcga` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    chunksize : int (default: 100)
-        Size of the chunks to be processed when reading the CSV file. This is
-        only used while downloading and converting the dataset to HDF5.
-
-    preload : bool (default: `True`)
-        Opens the gene expression dataset and keeps a reference to it in memory.
-        This decreases the loading time of individual tasks.
-
-    Notes
-    -----
-    A task is the combination of a cancer type and an attribute. The data is the
-    gene expression of patients diagnosed with the cancer defined by the task.
-    It consists in a vector of size `(20530,)`. The task is to classify the
-    patients according to the attribute given by the task definition. The meta
-    train/validation/test splits are over 137/29/29 tasks (ie. types of cancer).
-    However, the number of tasks depends on the minimum number of samples per
-    class specified by `min_samples_per_class`.
-
-    References
-    ----------
-    .. [1] Samiei, M., Wurfl, T., Deleu, T., Weiss, M., Dutil, F., Fevens, T.,
-           Boucher, G., Lemieux, S., and Cohen, J. P. (2019). The TCGA
-           Meta-Dataset Clinical Benchmark. (https://arxiv.org/abs/1910.08636)
-    """
-    folder = 'tcga'
-    clinical_matrix_url = 'https://tcga.xenahubs.net/download/TCGA.{0}.sampleMap/{0}_clinicalMatrix.gz'
-    clinical_matrix_filename, _ = os.path.splitext(os.path.basename(clinical_matrix_url))
-    gene_expression_filename = 'TCGA_HiSeqV2.hdf5'
-    gene_expression_torrent = 'e4081b995625f9fc599ad860138acf7b6eb1cf6f'
-
-    filename_tasks = '{0}_labels.json'
-
-    _task_variables = None
-    _cancers = None
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None,
-                 min_samples_per_class=5, transform=None, target_transform=None,
-                 dataset_transform=None, download=False, chunksize=100, preload=True):
-        super(TCGA, self).__init__(meta_train, meta_val, meta_test, meta_split,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.min_samples_per_class = min_samples_per_class
-        self.transform = transform
-
-        self._all_sample_ids = None
-        self._gene_ids = None
-        self._tasks = None
-
-        if download:
-            self.download(chunksize)
-
-        self.preloaded = False
-        self.gene_expression_data = None
-        self.gene_expression_file = None
-        if preload:
-            self._preload_gene_expression_data()
-            self.preloaded = True
-
-        self.task_ids = self.get_task_ids()
-        self.split_filename_tasks = os.path.join(self.root,
-            self.filename_tasks.format(self.meta_split))
-
-    def __len__(self):
-        return len(self.task_ids)
-
-    @property
-    def gene_expression_path(self):
-        filename = os.path.join(self.root, self.gene_expression_filename)
-        if not os.path.isfile(filename):
-            raise IOError('Gene expression data not found at {}'.format(filename))
-        return filename
-
-    @property
-    def tasks(self):
-        if self._tasks is None:
-            with open(self.split_filename_tasks, 'r') as f:
-                self._tasks = [task for task in json.load(f) if tuple(task) in self.task_ids]
-        return self._tasks
-
-    @property
-    def cancers(self):
-        if self._cancers is None:
-            self._cancers = get_cancers()
-        return self._cancers
-
-    @property
-    def task_variables(self):
-        if self._task_variables is None:
-            self._task_variables = frozenset(get_task_variables())
-        return self._task_variables
-
-    @property
-    def gene_ids(self):
-        if self._gene_ids is None:
-            gene_ids_file = os.path.join(self.root, 'gene_ids.json')
-            if not os.path.isfile(gene_ids_file):
-                raise IOError('Gene id data not found at {}'.format(gene_ids_file))
-            with open(gene_ids_file, 'r') as f:
-                self._gene_ids = set(json.load(f))
-        return self._gene_ids
-
-    @property
-    def all_sample_ids(self):
-        if self._all_sample_ids is None:
-            all_sample_ids_file = os.path.join(self.root, 'all_sample_ids.json')
-            if not os.path.isfile(all_sample_ids_file):
-                raise IOError('All sample id data not found at {}'.format(all_sample_ids_file))
-            with open(all_sample_ids_file, 'r') as f:
-                all_sample_ids = json.load(f)
-            self._all_sample_ids = dict((v, k) for (k, v) in enumerate(all_sample_ids))
-        return self._all_sample_ids
-
-    def get_processed_filename(self, cancer):
-        processed_folder = os.path.join(self.root, 'clinicalMatrices', 'processed')
-        filename = '{0}.tsv'.format(self.clinical_matrix_filename.format(cancer))
-        filepath = os.path.join(processed_folder, filename)
-        if not os.path.isfile(filepath):
-            raise IOError('Clinical matrix file not found at {}'.format(filepath))
-        return filepath
-
-    def __getitem__(self, index):
-        import pandas as pd
-
-        label, cancer = self.tasks[index]
-        filename = self.get_processed_filename(cancer)
-        dataframe = pd.read_csv(filename, sep='\t', index_col=0, header=0)
-        labels = dataframe[label].dropna().astype('category')
-        labels = labels[self.task_ids[(label, cancer)]]
-
-        if self.gene_expression_file is not None:
-            data = self.gene_expression_data[labels.index]
-        else:
-            with h5py.File(self.gene_expression_path, 'r') as f:
-                data = f['expression_data'][labels.index]
-
-        task = TCGATask((label, cancer), data, labels.cat.codes.tolist(),
-                        labels.cat.categories.tolist(), transform=self.transform,
-                        target_transform=self.target_transform)
-
-        if self.dataset_transform is not None:
-            task = self.dataset_transform(task)
-
-        return task
-
-    def _preload_gene_expression_data(self):
-        self.gene_expression_file = h5py.File(self.gene_expression_path, 'r')
-        self.gene_expression_data = self.gene_expression_file['expression_data']
-
-    def _process_clinical_matrices(self):
-        import pandas as pd
-        clinical_matrices_folder = os.path.join(self.root, 'clinicalMatrices')
-        processed_folder = os.path.join(clinical_matrices_folder, 'processed')
-        if not os.path.exists(processed_folder):
-            os.makedirs(processed_folder)
-
-        col_in_task_variables = lambda col: (col == 'sampleID') or (col in self.task_variables)
-
-        for cancer in self.cancers:
-            filename = self.clinical_matrix_filename.format(cancer)
-            filepath = os.path.join(clinical_matrices_folder, '{0}.tsv'.format(filename))
-            processed = os.path.join(processed_folder, '{0}.tsv'.format(filename))
-
-            if not os.path.isfile(processed):
-                raw_df = pd.read_csv(filepath, sep='\t', index_col=0, header=0,
-                                     usecols=col_in_task_variables)
-                dataframe = raw_df[raw_df.index.isin(self.all_sample_ids)]
-                dataframe.index = dataframe.index.map(lambda index: self.all_sample_ids[index])
-                dataframe.index.names = ['index']
-                dataframe = dataframe.sort_index(axis=0)
-                dataframe.to_csv(processed, sep='\t')
-        return True
-
-    def get_task_ids(self):
-        tasks = get_task_id_splits(self.meta_split)
-        task_ids = dict()
-
-        for task_id in tasks:
-            indices, counts = tasks[task_id]
-            enough_samples = all(count > self.min_samples_per_class for count in counts.values())
-            if enough_samples:
-                task_id = tuple(task_id.split('|', 1))
-                task_ids[task_id] = indices
-
-        return task_ids
-
-    def download(self, chunksize=100):
-        try:
-            import gzip
-            import shutil
-            import pandas as pd
-            from six.moves import urllib
-            import academictorrents as at
-        except ImportError as exception:
-            raise ImportError('{0}. To use the TCGA dataset, you need to '
-                'install the necessary dependencies with '
-                '`pip install torchmeta[tcga]`.'.format(exception.message))
-
-        clinical_matrices_folder = os.path.join(self.root, 'clinicalMatrices')
-        if not os.path.exists(clinical_matrices_folder):
-            os.makedirs(clinical_matrices_folder)
-
-        for cancer in self.cancers:
-            filename = self.clinical_matrix_filename.format(cancer)
-            rawpath = os.path.join(clinical_matrices_folder, '{0}.gz'.format(filename))
-            filepath = os.path.join(clinical_matrices_folder, '{0}.tsv'.format(filename))
-
-            if os.path.isfile(filepath):
-                continue
-
-            if not os.path.exists(rawpath):
-                print('Downloading `{0}.gz`...'.format(filename))
-                url = self.clinical_matrix_url.format(cancer)
-                urllib.request.urlretrieve(url, rawpath)
-
-            print('Extracting `{0}.gz`...'.format(filename))
-            with gzip.open(rawpath, 'rb') as gzf:
-                with open(filepath, 'wb') as f:
-                    shutil.copyfileobj(gzf, f)
-
-        gene_expression_file = os.path.join(self.root, self.gene_expression_filename)
-        if not os.path.isfile(gene_expression_file):
-            from tqdm import tqdm
-            print('Downloading `{0}` using `academictorrents`...'.format(
-                self.gene_expression_filename))
-            csv_file = at.get(self.gene_expression_torrent, datastore=self.root)
-            print('Downloaded to: `{0}`'.format(csv_file))
-
-            print('Converting TCGA CSV dataset to HDF5. This may take a while, '
-                  'but only happens on the first run.')
-            reader = pd.read_csv(csv_file, compression='gzip', sep='\t',
-                                 header=0, index_col=0, chunksize=chunksize)
-            shape = (10459, 20530)
-
-            with tqdm(total=shape[1]) as pbar:
-                with h5py.File(gene_expression_file, 'w') as f:
-                    dataset = f.create_dataset('expression_data',
-                                               shape=shape, dtype='f4')
-                    gene_ids = []
-                    for idx, chunk in enumerate(reader):
-                        slice_ = slice(idx * chunksize, (idx + 1) * chunksize)
-                        dataset[:, slice_] = chunk.T
-                        gene_ids.extend(chunk.index)
-                        pbar.update(chunk.shape[0])
-                    all_sample_ids = chunk.columns.tolist()
-
-            gene_ids_file = os.path.join(self.root, 'gene_ids.json')
-            with open(gene_ids_file, 'w') as f:
-                json.dump(gene_ids, f)
-
-            all_sample_ids_file = os.path.join(self.root, 'all_sample_ids.json')
-            with open(all_sample_ids_file, 'w') as f:
-                json.dump(all_sample_ids, f)
-
-            if os.path.isfile(csv_file):
-                os.remove(csv_file)
-
-            print('Done')
-
-        self._process_clinical_matrices()
-
-        # Create label files
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename_tasks.format(split))
-            data = get_asset(self.folder, '{0}.json'.format(split), dtype='json')
-
-            with open(filename, 'w') as f:
-                labels = sorted([key.split('|', 1) for key in data])
-                json.dump(labels, f)
-
-        # Clean up
-        for cancer in self.cancers:
-            filename = self.clinical_matrix_filename.format(cancer)
-            rawpath = os.path.join(clinical_matrices_folder, '{0}.gz'.format(filename))
-            if os.path.isfile(rawpath):
-                os.remove(rawpath)
-
-    def close(self):
-        if self.preloaded:
-            self.gene_expression_file.close()
-            self.gene_expression_data = None
-            self.gene_expression_file = None
-            self.preloaded = False
-
-    def open(self):
-        if self.preloaded:
-            self._preload_gene_expression_data()
-            self.preloaded = True
-
-
-class TCGATask(Task):
-    @classmethod
-    def from_id(cls, root, task_id, transform=None, target_transform=None):
-        import pandas as pd
-        root = os.path.join(os.path.expanduser(root), TCGA.folder)
-        gene_filepath = os.path.join(root, TCGA.gene_expression_filename)
-        if not os.path.isfile(gene_filepath):
-            raise IOError()
-
-        label, cancer = task_id
-
-        processed_folder = os.path.join(root, 'clinicalMatrices', 'processed')
-        filename = '{0}.tsv'.format(TCGA.clinical_matrix_filename.format(cancer))
-        filepath = os.path.join(processed_folder, filename)
-        if not os.path.isfile(filepath):
-            raise IOError()
-
-        dataframe = pd.read_csv(filepath, sep='\t', index_col=0, header=0)
-        labels = dataframe[label].dropna().astype('category')
-
-        with h5py.File(gene_filepath, 'r') as f:
-            data = f['expression_data'][labels.index]
-
-        return cls(task_id, data, labels.cat.codes.tolist(),
-                   labels.cat.categories.tolist(), transform=transform,
-                   target_transform=target_transform)
-
-    def __init__(self, task_id, data, labels, categories,
-                 transform=None, target_transform=None):
-        super(TCGATask, self).__init__(task_id, len(categories),
-            transform=transform, target_transform=target_transform)
-        self.id = task_id
-        self.data = data
-        self.labels = labels
-        self.categories = categories
-
-    @property
-    def input_size(self):
-        return len(self.data[0])
-
-    def __len__(self):
-        return len(self.labels)
-
-    def __iter__(self):
-        for index in range(len(self)):
-            yield self[index]
-
-    def __getitem__(self, index):
-        sample = self.data[index]
-        target = self.labels[index]
-
-        if self.transform is not None:
-            sample = self.transform(sample)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (sample, target)
-
-
-def _assign_samples(tcga_metadataset):
-    import pandas as pd
-    import munkres
-
-    blacklist = []
-    sample_to_task_assignment = {}
-    for cancer in get_cancers():
-        filename = tcga_metadataset.get_processed_filename(cancer)
-        dataframe = pd.read_csv(filename, sep='\t', index_col=0, header=0)
-        dataframe = dataframe.drop(blacklist, errors='ignore')
-        permutation = dataframe.index[torch.randperm(len(dataframe.index))]
-        dataframe = dataframe.reindex(permutation)
-        labels = dataframe.notna()
-        labels = labels.applymap(lambda x: 1. if x else munkres.DISALLOWED)
-        all_disallowed = labels.apply(lambda x: True if all(x == munkres.DISALLOWED) else False, axis=1)
-        labels = labels.drop(labels[all_disallowed].index)
-
-        matrix = labels.values
-        shape = matrix.shape
-        # The +5 allows for some slack in the assignment
-        # which is necessary for the used implementation to converge on BRCA
-        repeats = np.int(np.ceil(shape[0] / shape[1])) + 5
-        expanded_matrix = np.tile(matrix, (1, repeats))
-
-        indices = munkres.Munkres().compute(expanded_matrix)
-        mapped_indices = [(a, b % shape[1]) for a, b in indices]
-
-        for index, mapped_index in mapped_indices:
-            sample_to_task_assignment.setdefault((dataframe.columns[mapped_index], cancer), []).append(
-                dataframe.index[index])
-
-        blacklist.extend(dataframe.index.tolist())
-
-    return sample_to_task_assignment
-
-
-def _expand_sample_usage(meta_dataset, all_allowed_samples, additional_samples):
-    expanded_metadataset = {}
-    all_samples_of_metadataset = OrderedSet()
-    for key, value in meta_dataset.items():
-        all_samples_of_metadataset.update(value)
-    all_samples_of_metadataset.update(additional_samples)
-
-    used_additional_samples = OrderedSet()
-    for key in meta_dataset.keys():
-        allowed_samples = set(all_allowed_samples[key])
-        intersection = allowed_samples.intersection(all_samples_of_metadataset)
-        expanded_metadataset[key] = list(intersection)
-        used_additional_samples = additional_samples.intersection(intersection)
-
-    return expanded_metadataset, used_additional_samples
-
-
-def _split_tcga(tcga_metadataset, counts):
-    all_allowed_samples = tcga_metadataset.task_ids
-
-    # We first uniquely assing every sample to a task
-    sample_to_task_assignment = _assign_samples(tcga_metadataset)
-
-    keys = [i for i in all_allowed_samples.keys()]
-    difference = set(sample_to_task_assignment.keys()).difference(set(keys))
-
-    unassigned_samples = OrderedSet()
-    for key in difference:
-        unassigned_samples.update(sample_to_task_assignment[key])
-
-    # Second we split the metadataset
-    # with a torch-based random sample
-    permutation = torch.randperm(len(keys)).numpy()
-
-    metadatasets = []
-    start = 0
-    end = 0
-    for count in counts:
-        end += count
-        current_keys = [keys[index] for index in permutation[start:end]]
-        metadatasets.append({key: sample_to_task_assignment[key] for key in current_keys})
-        start = end
-
-    expanded_metadatasets = [None] * len(metadatasets)
-    order = np.argsort([len(metadataset) for metadataset in metadatasets])
-
-    # Finally we expand the tasks by reusing samples wherever possible in the sets
-    blacklist = OrderedSet()
-    for i in order:
-        additional_samples = unassigned_samples.difference(blacklist)
-        expanded_metadataset, used_additional_samples = _expand_sample_usage(
-            metadatasets[i], all_allowed_samples, additional_samples)
-        expanded_metadatasets[i] = (expanded_metadataset)
-        blacklist.update(used_additional_samples)
-
-    tcga_metadatasets = []
-    tcga_metadataset.close()
-    preloaded = tcga_metadataset.preloaded
-    for metadataset in expanded_metadatasets:
-        current_tcga_metadataset = copy.deepcopy(tcga_metadataset)
-        current_tcga_metadataset.task_ids = metadataset
-        if preloaded:
-            current_tcga_metadataset.open()
-        tcga_metadatasets.append(current_tcga_metadataset)
-
-    return tcga_metadatasets
-
-
-def get_cancers():
-    return get_asset(TCGA.folder, 'cancers.json', dtype='json')
-
-
-def get_task_variables():
-    return get_asset(TCGA.folder, 'task_variables.json', dtype='json')
-
-
-def get_task_id_splits(meta_split):
-    return get_asset(TCGA.folder, '{}.json'.format(meta_split), dtype='json')
+import os
+import json
+import h5py
+import numpy as np
+import torch
+import copy
+
+from ordered_set import OrderedSet
+from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class TCGA(MetaDataset):
+    """
+    The TCGA dataset [1]. A dataset of classification tasks over the values of
+    an attribute, based on the gene expression data from patients diagnosed with
+    specific types of cancer. This dataset is based on data from the Cancer
+    Genome Atlas Program from the National Cancer Institute.
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `omniglot` exists.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    min_samples_per_class : int (default: 5)
+        Minimum number of samples per class in each classification task. This
+        filters tasks for which the amount of data for one of the classes is
+        too small.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `transforms.ClassSplitter()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the files and processes the dataset in the root 
+        directory (under the `tcga` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    chunksize : int (default: 100)
+        Size of the chunks to be processed when reading the CSV file. This is
+        only used while downloading and converting the dataset to HDF5.
+
+    preload : bool (default: `True`)
+        Opens the gene expression dataset and keeps a reference to it in memory.
+        This decreases the loading time of individual tasks.
+
+    Notes
+    -----
+    A task is the combination of a cancer type and an attribute. The data is the
+    gene expression of patients diagnosed with the cancer defined by the task.
+    It consists in a vector of size `(20530,)`. The task is to classify the
+    patients according to the attribute given by the task definition. The meta
+    train/validation/test splits are over 137/29/29 tasks (ie. types of cancer).
+    However, the number of tasks depends on the minimum number of samples per
+    class specified by `min_samples_per_class`.
+
+    References
+    ----------
+    .. [1] Samiei, M., Wurfl, T., Deleu, T., Weiss, M., Dutil, F., Fevens, T.,
+           Boucher, G., Lemieux, S., and Cohen, J. P. (2019). The TCGA
+           Meta-Dataset Clinical Benchmark. (https://arxiv.org/abs/1910.08636)
+    """
+    folder = 'tcga'
+    clinical_matrix_url = 'https://tcga.xenahubs.net/download/TCGA.{0}.sampleMap/{0}_clinicalMatrix.gz'
+    clinical_matrix_filename, _ = os.path.splitext(os.path.basename(clinical_matrix_url))
+    gene_expression_filename = 'TCGA_HiSeqV2.hdf5'
+    gene_expression_torrent = 'e4081b995625f9fc599ad860138acf7b6eb1cf6f'
+
+    filename_tasks = '{0}_labels.json'
+
+    _task_variables = None
+    _cancers = None
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False, meta_split=None,
+                 min_samples_per_class=5, transform=None, target_transform=None,
+                 dataset_transform=None, download=False, chunksize=100, preload=True):
+        super(TCGA, self).__init__(meta_train, meta_val, meta_test, meta_split,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.min_samples_per_class = min_samples_per_class
+        self.transform = transform
+
+        self._all_sample_ids = None
+        self._gene_ids = None
+        self._tasks = None
+
+        if download:
+            self.download(chunksize)
+
+        self.preloaded = False
+        self.gene_expression_data = None
+        self.gene_expression_file = None
+        if preload:
+            self._preload_gene_expression_data()
+            self.preloaded = True
+
+        self.task_ids = self.get_task_ids()
+        self.split_filename_tasks = os.path.join(self.root,
+            self.filename_tasks.format(self.meta_split))
+
+    def __len__(self):
+        return len(self.task_ids)
+
+    @property
+    def gene_expression_path(self):
+        filename = os.path.join(self.root, self.gene_expression_filename)
+        if not os.path.isfile(filename):
+            raise IOError('Gene expression data not found at {}'.format(filename))
+        return filename
+
+    @property
+    def tasks(self):
+        if self._tasks is None:
+            with open(self.split_filename_tasks, 'r') as f:
+                self._tasks = [task for task in json.load(f) if tuple(task) in self.task_ids]
+        return self._tasks
+
+    @property
+    def cancers(self):
+        if self._cancers is None:
+            self._cancers = get_cancers()
+        return self._cancers
+
+    @property
+    def task_variables(self):
+        if self._task_variables is None:
+            self._task_variables = frozenset(get_task_variables())
+        return self._task_variables
+
+    @property
+    def gene_ids(self):
+        if self._gene_ids is None:
+            gene_ids_file = os.path.join(self.root, 'gene_ids.json')
+            if not os.path.isfile(gene_ids_file):
+                raise IOError('Gene id data not found at {}'.format(gene_ids_file))
+            with open(gene_ids_file, 'r') as f:
+                self._gene_ids = set(json.load(f))
+        return self._gene_ids
+
+    @property
+    def all_sample_ids(self):
+        if self._all_sample_ids is None:
+            all_sample_ids_file = os.path.join(self.root, 'all_sample_ids.json')
+            if not os.path.isfile(all_sample_ids_file):
+                raise IOError('All sample id data not found at {}'.format(all_sample_ids_file))
+            with open(all_sample_ids_file, 'r') as f:
+                all_sample_ids = json.load(f)
+            self._all_sample_ids = dict((v, k) for (k, v) in enumerate(all_sample_ids))
+        return self._all_sample_ids
+
+    def get_processed_filename(self, cancer):
+        processed_folder = os.path.join(self.root, 'clinicalMatrices', 'processed')
+        filename = '{0}.tsv'.format(self.clinical_matrix_filename.format(cancer))
+        filepath = os.path.join(processed_folder, filename)
+        if not os.path.isfile(filepath):
+            raise IOError('Clinical matrix file not found at {}'.format(filepath))
+        return filepath
+
+    def __getitem__(self, index):
+        import pandas as pd
+
+        label, cancer = self.tasks[index]
+        filename = self.get_processed_filename(cancer)
+        dataframe = pd.read_csv(filename, sep='\t', index_col=0, header=0)
+        labels = dataframe[label].dropna().astype('category')
+        labels = labels[self.task_ids[(label, cancer)]]
+
+        if self.gene_expression_file is not None:
+            data = self.gene_expression_data[labels.index]
+        else:
+            with h5py.File(self.gene_expression_path, 'r') as f:
+                data = f['expression_data'][labels.index]
+
+        task = TCGATask((label, cancer), data, labels.cat.codes.tolist(),
+                        labels.cat.categories.tolist(), transform=self.transform,
+                        target_transform=self.target_transform)
+
+        if self.dataset_transform is not None:
+            task = self.dataset_transform(task)
+
+        return task
+
+    def _preload_gene_expression_data(self):
+        self.gene_expression_file = h5py.File(self.gene_expression_path, 'r')
+        self.gene_expression_data = self.gene_expression_file['expression_data']
+
+    def _process_clinical_matrices(self):
+        import pandas as pd
+        clinical_matrices_folder = os.path.join(self.root, 'clinicalMatrices')
+        processed_folder = os.path.join(clinical_matrices_folder, 'processed')
+        if not os.path.exists(processed_folder):
+            os.makedirs(processed_folder)
+
+        col_in_task_variables = lambda col: (col == 'sampleID') or (col in self.task_variables)
+
+        for cancer in self.cancers:
+            filename = self.clinical_matrix_filename.format(cancer)
+            filepath = os.path.join(clinical_matrices_folder, '{0}.tsv'.format(filename))
+            processed = os.path.join(processed_folder, '{0}.tsv'.format(filename))
+
+            if not os.path.isfile(processed):
+                raw_df = pd.read_csv(filepath, sep='\t', index_col=0, header=0,
+                                     usecols=col_in_task_variables)
+                dataframe = raw_df[raw_df.index.isin(self.all_sample_ids)]
+                dataframe.index = dataframe.index.map(lambda index: self.all_sample_ids[index])
+                dataframe.index.names = ['index']
+                dataframe = dataframe.sort_index(axis=0)
+                dataframe.to_csv(processed, sep='\t')
+        return True
+
+    def get_task_ids(self):
+        tasks = get_task_id_splits(self.meta_split)
+        task_ids = dict()
+
+        for task_id in tasks:
+            indices, counts = tasks[task_id]
+            enough_samples = all(count > self.min_samples_per_class for count in counts.values())
+            if enough_samples:
+                task_id = tuple(task_id.split('|', 1))
+                task_ids[task_id] = indices
+
+        return task_ids
+
+    def download(self, chunksize=100):
+        try:
+            import gzip
+            import shutil
+            import pandas as pd
+            from six.moves import urllib
+            import academictorrents as at
+        except ImportError as exception:
+            raise ImportError('{0}. To use the TCGA dataset, you need to '
+                'install the necessary dependencies with '
+                '`pip install torchmeta[tcga]`.'.format(exception.message))
+
+        clinical_matrices_folder = os.path.join(self.root, 'clinicalMatrices')
+        if not os.path.exists(clinical_matrices_folder):
+            os.makedirs(clinical_matrices_folder)
+
+        for cancer in self.cancers:
+            filename = self.clinical_matrix_filename.format(cancer)
+            rawpath = os.path.join(clinical_matrices_folder, '{0}.gz'.format(filename))
+            filepath = os.path.join(clinical_matrices_folder, '{0}.tsv'.format(filename))
+
+            if os.path.isfile(filepath):
+                continue
+
+            if not os.path.exists(rawpath):
+                print('Downloading `{0}.gz`...'.format(filename))
+                url = self.clinical_matrix_url.format(cancer)
+                urllib.request.urlretrieve(url, rawpath)
+
+            print('Extracting `{0}.gz`...'.format(filename))
+            with gzip.open(rawpath, 'rb') as gzf:
+                with open(filepath, 'wb') as f:
+                    shutil.copyfileobj(gzf, f)
+
+        gene_expression_file = os.path.join(self.root, self.gene_expression_filename)
+        if not os.path.isfile(gene_expression_file):
+            from tqdm import tqdm
+            print('Downloading `{0}` using `academictorrents`...'.format(
+                self.gene_expression_filename))
+            csv_file = at.get(self.gene_expression_torrent, datastore=self.root)
+            print('Downloaded to: `{0}`'.format(csv_file))
+
+            print('Converting TCGA CSV dataset to HDF5. This may take a while, '
+                  'but only happens on the first run.')
+            reader = pd.read_csv(csv_file, compression='gzip', sep='\t',
+                                 header=0, index_col=0, chunksize=chunksize)
+            shape = (10459, 20530)
+
+            with tqdm(total=shape[1]) as pbar:
+                with h5py.File(gene_expression_file, 'w') as f:
+                    dataset = f.create_dataset('expression_data',
+                                               shape=shape, dtype='f4')
+                    gene_ids = []
+                    for idx, chunk in enumerate(reader):
+                        slice_ = slice(idx * chunksize, (idx + 1) * chunksize)
+                        dataset[:, slice_] = chunk.T
+                        gene_ids.extend(chunk.index)
+                        pbar.update(chunk.shape[0])
+                    all_sample_ids = chunk.columns.tolist()
+
+            gene_ids_file = os.path.join(self.root, 'gene_ids.json')
+            with open(gene_ids_file, 'w') as f:
+                json.dump(gene_ids, f)
+
+            all_sample_ids_file = os.path.join(self.root, 'all_sample_ids.json')
+            with open(all_sample_ids_file, 'w') as f:
+                json.dump(all_sample_ids, f)
+
+            if os.path.isfile(csv_file):
+                os.remove(csv_file)
+
+            print('Done')
+
+        self._process_clinical_matrices()
+
+        # Create label files
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename_tasks.format(split))
+            data = get_asset(self.folder, '{0}.json'.format(split), dtype='json')
+
+            with open(filename, 'w') as f:
+                labels = sorted([key.split('|', 1) for key in data])
+                json.dump(labels, f)
+
+        # Clean up
+        for cancer in self.cancers:
+            filename = self.clinical_matrix_filename.format(cancer)
+            rawpath = os.path.join(clinical_matrices_folder, '{0}.gz'.format(filename))
+            if os.path.isfile(rawpath):
+                os.remove(rawpath)
+
+    def close(self):
+        if self.preloaded:
+            self.gene_expression_file.close()
+            self.gene_expression_data = None
+            self.gene_expression_file = None
+            self.preloaded = False
+
+    def open(self):
+        if self.preloaded:
+            self._preload_gene_expression_data()
+            self.preloaded = True
+
+
+class TCGATask(Task):
+    @classmethod
+    def from_id(cls, root, task_id, transform=None, target_transform=None):
+        import pandas as pd
+        root = os.path.join(os.path.expanduser(root), TCGA.folder)
+        gene_filepath = os.path.join(root, TCGA.gene_expression_filename)
+        if not os.path.isfile(gene_filepath):
+            raise IOError()
+
+        label, cancer = task_id
+
+        processed_folder = os.path.join(root, 'clinicalMatrices', 'processed')
+        filename = '{0}.tsv'.format(TCGA.clinical_matrix_filename.format(cancer))
+        filepath = os.path.join(processed_folder, filename)
+        if not os.path.isfile(filepath):
+            raise IOError()
+
+        dataframe = pd.read_csv(filepath, sep='\t', index_col=0, header=0)
+        labels = dataframe[label].dropna().astype('category')
+
+        with h5py.File(gene_filepath, 'r') as f:
+            data = f['expression_data'][labels.index]
+
+        return cls(task_id, data, labels.cat.codes.tolist(),
+                   labels.cat.categories.tolist(), transform=transform,
+                   target_transform=target_transform)
+
+    def __init__(self, task_id, data, labels, categories,
+                 transform=None, target_transform=None):
+        super(TCGATask, self).__init__(task_id, len(categories),
+            transform=transform, target_transform=target_transform)
+        self.id = task_id
+        self.data = data
+        self.labels = labels
+        self.categories = categories
+
+    @property
+    def input_size(self):
+        return len(self.data[0])
+
+    def __len__(self):
+        return len(self.labels)
+
+    def __iter__(self):
+        for index in range(len(self)):
+            yield self[index]
+
+    def __getitem__(self, index):
+        sample = self.data[index]
+        target = self.labels[index]
+
+        if self.transform is not None:
+            sample = self.transform(sample)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (sample, target)
+
+
+def _assign_samples(tcga_metadataset):
+    import pandas as pd
+    import munkres
+
+    blacklist = []
+    sample_to_task_assignment = {}
+    for cancer in get_cancers():
+        filename = tcga_metadataset.get_processed_filename(cancer)
+        dataframe = pd.read_csv(filename, sep='\t', index_col=0, header=0)
+        dataframe = dataframe.drop(blacklist, errors='ignore')
+        permutation = dataframe.index[torch.randperm(len(dataframe.index))]
+        dataframe = dataframe.reindex(permutation)
+        labels = dataframe.notna()
+        labels = labels.applymap(lambda x: 1. if x else munkres.DISALLOWED)
+        all_disallowed = labels.apply(lambda x: True if all(x == munkres.DISALLOWED) else False, axis=1)
+        labels = labels.drop(labels[all_disallowed].index)
+
+        matrix = labels.values
+        shape = matrix.shape
+        # The +5 allows for some slack in the assignment
+        # which is necessary for the used implementation to converge on BRCA
+        repeats = np.int(np.ceil(shape[0] / shape[1])) + 5
+        expanded_matrix = np.tile(matrix, (1, repeats))
+
+        indices = munkres.Munkres().compute(expanded_matrix)
+        mapped_indices = [(a, b % shape[1]) for a, b in indices]
+
+        for index, mapped_index in mapped_indices:
+            sample_to_task_assignment.setdefault((dataframe.columns[mapped_index], cancer), []).append(
+                dataframe.index[index])
+
+        blacklist.extend(dataframe.index.tolist())
+
+    return sample_to_task_assignment
+
+
+def _expand_sample_usage(meta_dataset, all_allowed_samples, additional_samples):
+    expanded_metadataset = {}
+    all_samples_of_metadataset = OrderedSet()
+    for key, value in meta_dataset.items():
+        all_samples_of_metadataset.update(value)
+    all_samples_of_metadataset.update(additional_samples)
+
+    used_additional_samples = OrderedSet()
+    for key in meta_dataset.keys():
+        allowed_samples = set(all_allowed_samples[key])
+        intersection = allowed_samples.intersection(all_samples_of_metadataset)
+        expanded_metadataset[key] = list(intersection)
+        used_additional_samples = additional_samples.intersection(intersection)
+
+    return expanded_metadataset, used_additional_samples
+
+
+def _split_tcga(tcga_metadataset, counts):
+    all_allowed_samples = tcga_metadataset.task_ids
+
+    # We first uniquely assing every sample to a task
+    sample_to_task_assignment = _assign_samples(tcga_metadataset)
+
+    keys = [i for i in all_allowed_samples.keys()]
+    difference = set(sample_to_task_assignment.keys()).difference(set(keys))
+
+    unassigned_samples = OrderedSet()
+    for key in difference:
+        unassigned_samples.update(sample_to_task_assignment[key])
+
+    # Second we split the metadataset
+    # with a torch-based random sample
+    permutation = torch.randperm(len(keys)).numpy()
+
+    metadatasets = []
+    start = 0
+    end = 0
+    for count in counts:
+        end += count
+        current_keys = [keys[index] for index in permutation[start:end]]
+        metadatasets.append({key: sample_to_task_assignment[key] for key in current_keys})
+        start = end
+
+    expanded_metadatasets = [None] * len(metadatasets)
+    order = np.argsort([len(metadataset) for metadataset in metadatasets])
+
+    # Finally we expand the tasks by reusing samples wherever possible in the sets
+    blacklist = OrderedSet()
+    for i in order:
+        additional_samples = unassigned_samples.difference(blacklist)
+        expanded_metadataset, used_additional_samples = _expand_sample_usage(
+            metadatasets[i], all_allowed_samples, additional_samples)
+        expanded_metadatasets[i] = (expanded_metadataset)
+        blacklist.update(used_additional_samples)
+
+    tcga_metadatasets = []
+    tcga_metadataset.close()
+    preloaded = tcga_metadataset.preloaded
+    for metadataset in expanded_metadatasets:
+        current_tcga_metadataset = copy.deepcopy(tcga_metadataset)
+        current_tcga_metadataset.task_ids = metadataset
+        if preloaded:
+            current_tcga_metadataset.open()
+        tcga_metadatasets.append(current_tcga_metadataset)
+
+    return tcga_metadatasets
+
+
+def get_cancers():
+    return get_asset(TCGA.folder, 'cancers.json', dtype='json')
+
+
+def get_task_variables():
+    return get_asset(TCGA.folder, 'task_variables.json', dtype='json')
+
+
+def get_task_id_splits(meta_split):
+    return get_asset(TCGA.folder, '{}.json'.format(meta_split), dtype='json')
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-import numpy as np
-from PIL import Image
-import h5py
-import json
-import os
-import io
-import pickle
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-# QKFIX: See torchmeta.datasets.utils for more informations
-from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
-
-
-class TieredImagenet(CombinationMetaDataset):
-    """
-    The Tiered-Imagenet dataset, introduced in [1]. This dataset contains images 
-    of 608 different classes from the ILSVRC-12 dataset (Imagenet challenge).
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `tieredimagenet` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way" 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the root 
-        directory (under the `tieredimagenet` folder). If the dataset is already 
-        available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The dataset is downloaded from [this repository]
-    (https://github.com/renmengye/few-shot-ssl-public/). The dataset contains 
-    images from 34 categories. The meta train/validation/test splits are over 
-    20/6/8 categories. Each category contains between 10 and 30 classes. The 
-    splits over categories (instead of over classes) ensures that all the training 
-    classes are sufficiently distinct from the test classes (unlike Mini-Imagenet).
-
-    References
-    ----------
-    .. [1] Ren, M., Triantafillou, E., Ravi, S., Snell, J., Swersky, K., 
-           Tenenbaum, J.B., Larochelle, H. and Zemel, R.S. (2018). Meta-learning 
-           for semi-supervised few-shot classification. International Conference 
-           on Learning Representations. (https://arxiv.org/abs/1803.00676)
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = TieredImagenetClassDataset(root, meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            transform=transform, class_augmentations=class_augmentations,
-            download=download)
-        super(TieredImagenet, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform, dataset_transform=dataset_transform)
-
-
-class TieredImagenetClassDataset(ClassDataset):
-    folder = 'tieredimagenet'
-    # Google Drive ID from https://github.com/renmengye/few-shot-ssl-public
-    gdrive_id = '1g1aIDy2Ar_MViF2gDXFYDBTR-HYecV07'
-    tar_filename = 'tiered-imagenet.tar'
-    tar_md5 = 'e07e811b9f29362d159a9edd0d838c62'
-    tar_folder = 'tiered-imagenet'
-
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(TieredImagenetClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        self.split_filename = os.path.join(self.root,
-            self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root,
-            self.filename_labels.format(self.meta_split))
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('TieredImagenet integrity check failed')
-        self._num_classes = len(self.labels)
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def __getitem__(self, index):
-        specific_class_name = self.labels[index % self.num_classes]
-        data = self.data[specific_class_name]
-        general_class_name = data.attrs['label_general']
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return TieredImagenetDataset(index, data,
-            general_class_name, specific_class_name,
-            transform=transform, target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    def close(self):
-        if self._data_file is not None:
-            self._data_file.close()
-            self._data_file = None
-            self._data = None
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def download(self):
-        import tarfile
-        import shutil
-        from tqdm import tqdm
-
-        if self._check_integrity():
-            return
-
-        download_file_from_google_drive(self.gdrive_id, self.root,
-            self.tar_filename, md5=self.tar_md5)
-
-        filename = os.path.join(self.root, self.tar_filename)
-        with tarfile.open(filename, 'r') as f:
-            f.extractall(self.root)
-        tar_folder = os.path.join(self.root, self.tar_folder)
-
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename.format(split))
-            if os.path.isfile(filename):
-                continue
-
-            images_filename = os.path.join(tar_folder, '{0}_images_png.pkl'.format(split))
-            if not os.path.isfile(images_filename):
-                raise IOError(images_filename)
-            with open(images_filename, 'rb') as f:
-                images = pickle.load(f, encoding='bytes')
-
-            labels_filename = os.path.join(tar_folder, '{0}_labels.pkl'.format(split))
-            if not os.path.isfile(labels_filename):
-                raise IOError()
-            with open(labels_filename, 'rb') as f:
-                labels = pickle.load(f, encoding='latin1')
-
-            labels_str = labels['label_specific_str']
-            general_labels_str = labels['label_general_str']
-            general_labels = labels['label_general']
-            with open(os.path.join(self.root, self.filename_labels.format(split)), 'w') as f:
-                json.dump(labels_str, f)
-
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-                dtype = h5py.special_dtype(vlen=np.uint8)
-                for i, label in enumerate(tqdm(labels_str, desc=filename)):
-                    indices, = np.where(labels['label_specific'] == i)
-                    dataset = group.create_dataset(label, (len(indices),), dtype=dtype)
-                    general_idx = general_labels[indices[0]]
-                    dataset.attrs['label_general'] = (general_labels_str[general_idx]
-                        if general_idx < len(general_labels_str) else '')
-                    dataset.attrs['label_specific'] = label
-                    for j, k in enumerate(indices):
-                        dataset[j] = np.squeeze(images[k])
-
-        if os.path.isdir(tar_folder):
-            shutil.rmtree(tar_folder)
-
-
-class TieredImagenetDataset(Dataset):
-    def __init__(self, index, data, general_class_name, specific_class_name,
-                 transform=None, target_transform=None):
-        super(TieredImagenetDataset, self).__init__(index, transform=transform,
-                                                    target_transform=target_transform)
-        self.data = data
-        self.general_class_name = general_class_name
-        self.specific_class_name = specific_class_name
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        image = Image.open(io.BytesIO(self.data[index]))
-        target = (self.general_class_name, self.specific_class_name)
-
-        if self.transform is not None:
-            image = self.transform(image)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (image, target)
+import numpy as np
+from PIL import Image
+import h5py
+import json
+import os
+import io
+import pickle
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+# QKFIX: See torchmeta.datasets.utils for more informations
+from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
+
+
+class TieredImagenet(CombinationMetaDataset):
+    """
+    The Tiered-Imagenet dataset, introduced in [1]. This dataset contains images 
+    of 608 different classes from the ILSVRC-12 dataset (Imagenet challenge).
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `tieredimagenet` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way" 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the root 
+        directory (under the `tieredimagenet` folder). If the dataset is already 
+        available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The dataset is downloaded from [this repository]
+    (https://github.com/renmengye/few-shot-ssl-public/). The dataset contains 
+    images from 34 categories. The meta train/validation/test splits are over 
+    20/6/8 categories. Each category contains between 10 and 30 classes. The 
+    splits over categories (instead of over classes) ensures that all the training 
+    classes are sufficiently distinct from the test classes (unlike Mini-Imagenet).
+
+    References
+    ----------
+    .. [1] Ren, M., Triantafillou, E., Ravi, S., Snell, J., Swersky, K., 
+           Tenenbaum, J.B., Larochelle, H. and Zemel, R.S. (2018). Meta-learning 
+           for semi-supervised few-shot classification. International Conference 
+           on Learning Representations. (https://arxiv.org/abs/1803.00676)
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = TieredImagenetClassDataset(root, meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            transform=transform, class_augmentations=class_augmentations,
+            download=download)
+        super(TieredImagenet, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform, dataset_transform=dataset_transform)
+
+
+class TieredImagenetClassDataset(ClassDataset):
+    folder = 'tieredimagenet'
+    # Google Drive ID from https://github.com/renmengye/few-shot-ssl-public
+    gdrive_id = '1g1aIDy2Ar_MViF2gDXFYDBTR-HYecV07'
+    tar_filename = 'tiered-imagenet.tar'
+    tar_md5 = 'e07e811b9f29362d159a9edd0d838c62'
+    tar_folder = 'tiered-imagenet'
+
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(TieredImagenetClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+
+        self.split_filename = os.path.join(self.root,
+            self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root,
+            self.filename_labels.format(self.meta_split))
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('TieredImagenet integrity check failed')
+        self._num_classes = len(self.labels)
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def __getitem__(self, index):
+        specific_class_name = self.labels[index % self.num_classes]
+        data = self.data[specific_class_name]
+        general_class_name = data.attrs['label_general']
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return TieredImagenetDataset(index, data,
+            general_class_name, specific_class_name,
+            transform=transform, target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    def close(self):
+        if self._data_file is not None:
+            self._data_file.close()
+            self._data_file = None
+            self._data = None
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def download(self):
+        import tarfile
+        import shutil
+        from tqdm import tqdm
+
+        if self._check_integrity():
+            return
+
+        download_file_from_google_drive(self.gdrive_id, self.root,
+            self.tar_filename, md5=self.tar_md5)
+
+        filename = os.path.join(self.root, self.tar_filename)
+        with tarfile.open(filename, 'r') as f:
+            f.extractall(self.root)
+        tar_folder = os.path.join(self.root, self.tar_folder)
+
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename.format(split))
+            if os.path.isfile(filename):
+                continue
+
+            images_filename = os.path.join(tar_folder, '{0}_images_png.pkl'.format(split))
+            if not os.path.isfile(images_filename):
+                raise IOError(images_filename)
+            with open(images_filename, 'rb') as f:
+                images = pickle.load(f, encoding='bytes')
+
+            labels_filename = os.path.join(tar_folder, '{0}_labels.pkl'.format(split))
+            if not os.path.isfile(labels_filename):
+                raise IOError()
+            with open(labels_filename, 'rb') as f:
+                labels = pickle.load(f, encoding='latin1')
+
+            labels_str = labels['label_specific_str']
+            general_labels_str = labels['label_general_str']
+            general_labels = labels['label_general']
+            with open(os.path.join(self.root, self.filename_labels.format(split)), 'w') as f:
+                json.dump(labels_str, f)
+
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+                dtype = h5py.special_dtype(vlen=np.uint8)
+                for i, label in enumerate(tqdm(labels_str, desc=filename)):
+                    indices, = np.where(labels['label_specific'] == i)
+                    dataset = group.create_dataset(label, (len(indices),), dtype=dtype)
+                    general_idx = general_labels[indices[0]]
+                    dataset.attrs['label_general'] = (general_labels_str[general_idx]
+                        if general_idx < len(general_labels_str) else '')
+                    dataset.attrs['label_specific'] = label
+                    for j, k in enumerate(indices):
+                        dataset[j] = np.squeeze(images[k])
+
+        if os.path.isdir(tar_folder):
+            shutil.rmtree(tar_folder)
+
+
+class TieredImagenetDataset(Dataset):
+    def __init__(self, index, data, general_class_name, specific_class_name,
+                 transform=None, target_transform=None):
+        super(TieredImagenetDataset, self).__init__(index, transform=transform,
+                                                    target_transform=target_transform)
+        self.data = data
+        self.general_class_name = general_class_name
+        self.specific_class_name = specific_class_name
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        image = Image.open(io.BytesIO(self.data[index]))
+        target = (self.general_class_name, self.specific_class_name)
+
+        if self.transform is not None:
+            image = self.transform(image)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (image, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-import numpy as np
-from PIL import Image
-import os
-import io
-import json
-import glob
-import h5py
-
-from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
-# QKFIX: See torchmeta.datasets.utils for more informations
-from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
-from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
-
-
-class TripleMNIST(CombinationMetaDataset):
-    """
-    The Triple MNIST dataset, introduced in [1]. This dataset is based on
-    the MNIST dataset [2]. It consists of sampled images from MNIST
-    that are put together to create images with multiple digits. It contains
-    1,000,000 images from 1000 different classes (1000 images per class, for 
-    the numbers 000 to 999).
-
-    Parameters
-    ----------
-    root : string
-        Root directory where the dataset folder `triplemnist` exists.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to "N" in "N-way" 
-        classification.
-
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly
-        one of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly
-        one of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test` if all three are set to `False`.
-
-    transform : callable, optional
-        A function/transform that takes a `PIL` image, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These
-        classes are transformations of existing classes. E.g.
-        `torchmeta.transforms.HorizontalFlip()`.
-
-    download : bool (default: `False`)
-        If `True`, downloads the pickle files and processes the dataset in the
-        root directory (under the `triplemnist` folder). If the dataset is
-        already available, this does not download/process the dataset again.
-
-    Notes
-    -----
-    The dataset is downloaded from the Multi-digit MNIST repository
-    [1](https://github.com/shaohua0116/MultiDigitMNIST). The dataset contains
-    images (MNIST triple digits) from 1000 classes, for the numbers 000 to 999.
-    The meta train/validation/test splits are 640/160/200 classes.
-    The splits are taken from [1].
-
-    References
-    ----------
-    .. [1] Sun, S. (2019). Multi-digit MNIST for Few-shot Learning.
-    (https://github.com/shaohua0116/MultiDigitMNIST)
-
-    .. [2] LeCun, Y., Cortes, C., and Burges, CJ. (2010). MNIST Handwritten
-    Digit Database. (http://yann.lecun.com/exdb/mnist)
-
-    """
-    def __init__(self, root, num_classes_per_task=None, meta_train=False,
-                 meta_val=False, meta_test=False, meta_split=None,
-                 transform=None, target_transform=None, dataset_transform=None,
-                 class_augmentations=None, download=False):
-        dataset = TripleMNISTClassDataset(root,
-            meta_train=meta_train, meta_val=meta_val,
-            meta_test=meta_test, meta_split=meta_split, transform=transform,
-            class_augmentations=class_augmentations, download=download)
-        super(TripleMNIST, self).__init__(dataset, num_classes_per_task,
-            target_transform=target_transform,
-            dataset_transform=dataset_transform)
-
-
-class TripleMNISTClassDataset(ClassDataset):
-    folder = 'triplemnist'
-    # Google Drive ID from https://github.com/shaohua0116/MultiDigitMNIST
-    gdrive_id = '1xqyW289seXYaDSqD2jaBPMKVAAjPP9ee'
-    zip_filename = 'triple_mnist_seed_123_image_size_84_84.zip'
-    zip_md5 = '9508b047f9fbb834c02bc13ef44245da'
-
-    filename = '{0}_data.hdf5'
-    filename_labels = '{0}_labels.json'
-
-    image_folder = 'triple_mnist_seed_123_image_size_84_84'
-
-    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, transform=None, class_augmentations=None,
-                 download=False):
-        super(TripleMNISTClassDataset, self).__init__(meta_train=meta_train,
-            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
-            class_augmentations=class_augmentations)
-
-        self.root = os.path.join(os.path.expanduser(root), self.folder)
-        self.transform = transform
-
-        self.split_filename = os.path.join(self.root,
-            self.filename.format(self.meta_split))
-        self.split_filename_labels = os.path.join(self.root,
-            self.filename_labels.format(self.meta_split))
-
-        self._data_file = None
-        self._data = None
-        self._labels = None
-
-        if download:
-            self.download()
-
-        if not self._check_integrity():
-            raise RuntimeError('Triple MNIST integrity check failed')
-        self._num_classes = len(self.labels)
-
-    def __getitem__(self, index):
-        label = self.labels[index % self.num_classes]
-        data = self.data[label]
-        transform = self.get_transform(index, self.transform)
-        target_transform = self.get_target_transform(index)
-
-        return TripleMNISTDataset(index, data, label, transform=transform,
-                                  target_transform=target_transform)
-
-    @property
-    def num_classes(self):
-        return self._num_classes
-
-    @property
-    def data(self):
-        if self._data is None:
-            self._data_file = h5py.File(self.split_filename, 'r')
-            self._data = self._data_file['datasets']
-        return self._data
-    
-    @property
-    def labels(self):
-        if self._labels is None:
-            with open(self.split_filename_labels, 'r') as f:
-                self._labels = json.load(f)
-        return self._labels
-
-    def _check_integrity(self):
-        return (os.path.isfile(self.split_filename)
-            and os.path.isfile(self.split_filename_labels))
-
-    def close(self):
-        if self._data_file is not None:
-            self._data_file.close()
-            self._data_file = None
-            self._data = None
-
-    def download(self):
-        import zipfile
-        import shutil
-        import glob
-        from tqdm import tqdm
-
-        if self._check_integrity():
-            return
-
-        zip_filename = os.path.join(self.root, self.zip_filename)
-        if not os.path.isfile(zip_filename):
-            download_file_from_google_drive(self.gdrive_id, self.root,
-                self.zip_filename, md5=self.zip_md5)
-
-        zip_foldername = os.path.join(self.root, self.image_folder)
-        if not os.path.isdir(zip_foldername):
-            with zipfile.ZipFile(zip_filename, 'r') as f:
-                for member in tqdm(f.infolist(), desc='Extracting '):
-                    try:
-                        f.extract(member, self.root)
-                    except zipfile.BadZipFile:
-                        print('Error: Zip file is corrupted')
-
-        for split in ['train', 'val', 'test']:
-            filename = os.path.join(self.root, self.filename.format(split))
-            if os.path.isfile(filename):
-                continue
-
-            labels = get_asset(self.folder, '{0}.json'.format(split))
-            labels_filename = os.path.join(self.root,
-                                           self.filename_labels.format(split))
-            with open(labels_filename, 'w') as f:
-                json.dump(labels, f)
-
-            image_folder = os.path.join(zip_foldername, split)
-
-            with h5py.File(filename, 'w') as f:
-                group = f.create_group('datasets')
-                dtype = h5py.special_dtype(vlen=np.uint8)
-                for i, label in enumerate(tqdm(labels, desc=filename)):
-                    images = glob.glob(os.path.join(image_folder, label,
-                                                    '*.png'))
-                    images.sort()
-                    dataset = group.create_dataset(label, (len(images),),
-                                                   dtype=dtype)
-                    for i, image in enumerate(images):
-                        with open(image, 'rb') as f:
-                            array = bytearray(f.read())
-                            dataset[i] = np.asarray(array, dtype=np.uint8)
-
-        if os.path.isdir(zip_foldername):
-            shutil.rmtree(zip_foldername)
-
-
-class TripleMNISTDataset(Dataset):
-    def __init__(self, index, data, label,
-                 transform=None, target_transform=None):
-        super(TripleMNISTDataset, self).__init__(index, transform=transform,
-                                                 target_transform=target_transform)
-        self.data = data
-        self.label = label
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        image = Image.open(io.BytesIO(self.data[index])).convert('RGB')
-        target = self.label
-
-        if self.transform is not None:
-            image = self.transform(image)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (image, target)
+import numpy as np
+from PIL import Image
+import os
+import io
+import json
+import glob
+import h5py
+
+from lightningdata.thirdparty.torchmeta.utils.data import Dataset, ClassDataset, CombinationMetaDataset
+# QKFIX: See torchmeta.datasets.utils for more informations
+from lightningdata.thirdparty.torchmeta.datasets.utils import download_file_from_google_drive
+from lightningdata.thirdparty.torchmeta.datasets.utils import get_asset
+
+
+class DoubleMNIST(CombinationMetaDataset):
+    """
+    The Double MNIST dataset, introduced in [1]. This dataset is based on
+    the MNIST dataset [2]. It consists of sampled images from MNIST
+    that are put together to create images with multiple digits. It contains
+    100,000 images from 100 different classes (1000 images per class, for the 
+    numbers 00 to 99).
+
+    Parameters
+    ----------
+    root : string
+        Root directory where the dataset folder `doublemnist` exists.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to "N" in "N-way" 
+        classification.
+
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly
+        one of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly
+        one of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test` if all three are set to `False`.
+
+    transform : callable, optional
+        A function/transform that takes a `PIL` image, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These
+        classes are transformations of existing classes. E.g.
+        `torchmeta.transforms.HorizontalFlip()`.
+
+    download : bool (default: `False`)
+        If `True`, downloads the pickle files and processes the dataset in the
+        root directory (under the `doublemnist` folder). If the dataset is
+        already available, this does not download/process the dataset again.
+
+    Notes
+    -----
+    The dataset is downloaded from the Multi-digit MNIST repository
+    [1](https://github.com/shaohua0116/MultiDigitMNIST). The dataset contains
+    images (MNIST double digits) from 100 classes, for the numbers 00 to 99.
+    The meta train/validation/test splits are 64/16/20 classes.
+    The splits are taken from [1].
+
+    References
+    ----------
+    .. [1] Sun, S. (2019). Multi-digit MNIST for Few-shot Learning.
+    (https://github.com/shaohua0116/MultiDigitMNIST)
+
+    .. [2] LeCun, Y., Cortes, C., and Burges, CJ. (2010). MNIST Handwritten
+    Digit Database. (http://yann.lecun.com/exdb/mnist)
+
+    """
+    def __init__(self, root, num_classes_per_task=None, meta_train=False,
+                 meta_val=False, meta_test=False, meta_split=None,
+                 transform=None, target_transform=None, dataset_transform=None,
+                 class_augmentations=None, download=False):
+        dataset = DoubleMNISTClassDataset(root,
+            meta_train=meta_train, meta_val=meta_val,
+            meta_test=meta_test, meta_split=meta_split, transform=transform,
+            class_augmentations=class_augmentations, download=download)
+        super(DoubleMNIST, self).__init__(dataset, num_classes_per_task,
+            target_transform=target_transform,
+            dataset_transform=dataset_transform)
+
+
+class DoubleMNISTClassDataset(ClassDataset):
+    folder = 'doublemnist'
+    # Google Drive ID from https://github.com/shaohua0116/MultiDigitMNIST
+    gdrive_id = '1MqQCdLt9TVE3joAMw4FwJp_B8F-htrAo'
+    zip_filename = 'double_mnist_seed_123_image_size_64_64.zip'
+    zip_md5 = '6d8b185c0cde155eb39d0e3615ab4f23'
+
+    filename = '{0}_data.hdf5'
+    filename_labels = '{0}_labels.json'
+
+    image_folder = 'double_mnist_seed_123_image_size_64_64'
+
+    def __init__(self, root, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, transform=None, class_augmentations=None,
+                 download=False):
+        super(DoubleMNISTClassDataset, self).__init__(meta_train=meta_train,
+            meta_val=meta_val, meta_test=meta_test, meta_split=meta_split,
+            class_augmentations=class_augmentations)
+
+        self.root = os.path.join(os.path.expanduser(root), self.folder)
+        self.transform = transform
+
+        self.split_filename = os.path.join(self.root,
+            self.filename.format(self.meta_split))
+        self.split_filename_labels = os.path.join(self.root,
+            self.filename_labels.format(self.meta_split))
+
+        self._data_file = None
+        self._data = None
+        self._labels = None
+
+        if download:
+            self.download()
+
+        if not self._check_integrity():
+            raise RuntimeError('Double MNIST integrity check failed')
+        self._num_classes = len(self.labels)
+
+    def __getitem__(self, index):
+        label = self.labels[index % self.num_classes]
+        data = self.data[label]
+        transform = self.get_transform(index, self.transform)
+        target_transform = self.get_target_transform(index)
+
+        return DoubleMNISTDataset(index, data, label, transform=transform,
+                                  target_transform=target_transform)
+
+    @property
+    def num_classes(self):
+        return self._num_classes
+
+    @property
+    def data(self):
+        if self._data is None:
+            self._data_file = h5py.File(self.split_filename, 'r')
+            self._data = self._data_file['datasets']
+        return self._data
+    
+    @property
+    def labels(self):
+        if self._labels is None:
+            with open(self.split_filename_labels, 'r') as f:
+                self._labels = json.load(f)
+        return self._labels
+
+    def _check_integrity(self):
+        return (os.path.isfile(self.split_filename)
+            and os.path.isfile(self.split_filename_labels))
+
+    def close(self):
+        if self._data_file is not None:
+            self._data_file.close()
+            self._data_file = None
+            self._data = None
+
+    def download(self):
+        import zipfile
+        import shutil
+        import glob
+        from tqdm import tqdm
+
+        if self._check_integrity():
+            return
+
+        zip_filename = os.path.join(self.root, self.zip_filename)
+        if not os.path.isfile(zip_filename):
+            download_file_from_google_drive(self.gdrive_id, self.root,
+                self.zip_filename, md5=self.zip_md5)
+
+        zip_foldername = os.path.join(self.root, self.image_folder)
+        if not os.path.isdir(zip_foldername):
+            with zipfile.ZipFile(zip_filename, 'r') as f:
+                for member in tqdm(f.infolist(), desc='Extracting '):
+                    try:
+                        f.extract(member, self.root)
+                    except zipfile.BadZipFile:
+                        print('Error: Zip file is corrupted')
+
+        for split in ['train', 'val', 'test']:
+            filename = os.path.join(self.root, self.filename.format(split))
+            if os.path.isfile(filename):
+                continue
+
+            labels = get_asset(self.folder, '{0}.json'.format(split))
+            labels_filename = os.path.join(self.root,
+                                           self.filename_labels.format(split))
+            with open(labels_filename, 'w') as f:
+                json.dump(labels, f)
+
+            image_folder = os.path.join(zip_foldername, split)
+
+            with h5py.File(filename, 'w') as f:
+                group = f.create_group('datasets')
+                dtype = h5py.special_dtype(vlen=np.uint8)
+                for i, label in enumerate(tqdm(labels, desc=filename)):
+                    images = glob.glob(os.path.join(image_folder, label,
+                                                    '*.png'))
+                    images.sort()
+                    dataset = group.create_dataset(label, (len(images),),
+                                                   dtype=dtype)
+                    for i, image in enumerate(images):
+                        with open(image, 'rb') as f:
+                            array = bytearray(f.read())
+                            dataset[i] = np.asarray(array, dtype=np.uint8)
+
+        if os.path.isdir(zip_foldername):
+            shutil.rmtree(zip_foldername)
+
+
+class DoubleMNISTDataset(Dataset):
+    def __init__(self, index, data, label,
+                 transform=None, target_transform=None):
+        super(DoubleMNISTDataset, self).__init__(index, transform=transform,
+                                                 target_transform=target_transform)
+        self.data = data
+        self.label = label
+
+    def __len__(self):
+        return len(self.data)
+
+    def __getitem__(self, index):
+        image = Image.open(io.BytesIO(self.data[index])).convert('RGB')
+        target = self.label
+
+        if self.transform is not None:
+            image = self.transform(image)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (image, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/datasets/utils.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/datasets/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import os
-import json
-from torchvision.datasets.utils import download_file_from_google_drive as download
-
-def get_asset_path(*args):
-    basedir = os.path.dirname(__file__)
-    return os.path.join(basedir, 'assets', *args)
-
-
-def get_asset(*args, dtype=None):
-    filename = get_asset_path(*args)
-    if not os.path.isfile(filename):
-        raise IOError('{} not found'.format(filename))
-
-    if dtype is None:
-        _, dtype = os.path.splitext(filename)
-        dtype = dtype[1:]
-
-    if dtype == 'json':
-        with open(filename, 'r') as f:
-            data = json.load(f)
-    else:
-        raise NotImplementedError()
-    return data
-
-# QKFIX: The current version of `download_file_from_google_drive` (as of torchvision==0.8.1)
-# is inconsistent, and a temporary fix has been added to the bleeding-edge version of
-# Torchvision. The temporary fix removes the behaviour of `_quota_exceeded`, whenever the
-# quota has exceeded for the file to be downloaded. As a consequence, this means that there
-# is currently no protection against exceeded quotas. If you get an integrity error in Torchmeta
-# (e.g. "MiniImagenet integrity check failed" for MiniImagenet), then this means that the quota
-# has exceeded for this dataset. See also: https://github.com/tristandeleu/pytorch-meta/issues/54
-# 
-# See also: https://github.com/pytorch/vision/issues/2992
-# 
-# The following functions are taken from
-# https://github.com/pytorch/vision/blob/cd0268cd408d19d91f870e36fdffd031085abe13/torchvision/datasets/utils.py
-
-from torchvision.datasets.utils import _save_response_content, check_integrity
-
-def _quota_exceeded(response: "requests.models.Response"):
-    return False
-    # See https://github.com/pytorch/vision/issues/2992 for details
-    # return "Google Drive - Quota exceeded" in response.text
-
-
-def download_file_from_google_drive(file_id, root, filename=None, md5=None):
-    return download(file_id, root, filename, md5)
+import os
+import json
+from torchvision.datasets.utils import download_file_from_google_drive as download
+
+def get_asset_path(*args):
+    basedir = os.path.dirname(__file__)
+    return os.path.join(basedir, 'assets', *args)
+
+
+def get_asset(*args, dtype=None):
+    filename = get_asset_path(*args)
+    if not os.path.isfile(filename):
+        raise IOError('{} not found'.format(filename))
+
+    if dtype is None:
+        _, dtype = os.path.splitext(filename)
+        dtype = dtype[1:]
+
+    if dtype == 'json':
+        with open(filename, 'r') as f:
+            data = json.load(f)
+    else:
+        raise NotImplementedError()
+    return data
+
+# QKFIX: The current version of `download_file_from_google_drive` (as of torchvision==0.8.1)
+# is inconsistent, and a temporary fix has been added to the bleeding-edge version of
+# Torchvision. The temporary fix removes the behaviour of `_quota_exceeded`, whenever the
+# quota has exceeded for the file to be downloaded. As a consequence, this means that there
+# is currently no protection against exceeded quotas. If you get an integrity error in Torchmeta
+# (e.g. "MiniImagenet integrity check failed" for MiniImagenet), then this means that the quota
+# has exceeded for this dataset. See also: https://github.com/tristandeleu/pytorch-meta/issues/54
+# 
+# See also: https://github.com/pytorch/vision/issues/2992
+# 
+# The following functions are taken from
+# https://github.com/pytorch/vision/blob/cd0268cd408d19d91f870e36fdffd031085abe13/torchvision/datasets/utils.py
+
+from torchvision.datasets.utils import _save_response_content, check_integrity
+
+def _quota_exceeded(response: "requests.models.Response"):
+    return False
+    # See https://github.com/pytorch/vision/issues/2992 for details
+    # return "Google Drive - Quota exceeded" in response.text
+
+
+def download_file_from_google_drive(file_id, root, filename=None, md5=None):
+    return download(file_id, root, filename, md5)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from lightningdata.thirdparty.torchmeta.modules.activation import MetaMultiheadAttention
-from lightningdata.thirdparty.torchmeta.modules.batchnorm import MetaBatchNorm1d, MetaBatchNorm2d, MetaBatchNorm3d
-from lightningdata.thirdparty.torchmeta.modules.container import MetaSequential
-from lightningdata.thirdparty.torchmeta.modules.conv import MetaConv1d, MetaConv2d, MetaConv3d
-from lightningdata.thirdparty.torchmeta.modules.linear import MetaLinear, MetaBilinear
-from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
-from lightningdata.thirdparty.torchmeta.modules.normalization import MetaLayerNorm
-from lightningdata.thirdparty.torchmeta.modules.parallel import DataParallel
-from lightningdata.thirdparty.torchmeta.modules.sparse import MetaEmbedding, MetaEmbeddingBag
-
-__all__ = [
-    'MetaMultiheadAttention',
-    'MetaBatchNorm1d', 'MetaBatchNorm2d', 'MetaBatchNorm3d',
-    'MetaSequential',
-    'MetaConv1d', 'MetaConv2d', 'MetaConv3d',
-    'MetaLinear', 'MetaBilinear',
-    'MetaModule',
-    'MetaLayerNorm',
-    'DataParallel',
-    'MetaEmbedding', 'MetaEmbeddingBag',
+from lightningdata.thirdparty.torchmeta.modules.activation import MetaMultiheadAttention
+from lightningdata.thirdparty.torchmeta.modules.batchnorm import MetaBatchNorm1d, MetaBatchNorm2d, MetaBatchNorm3d
+from lightningdata.thirdparty.torchmeta.modules.container import MetaSequential
+from lightningdata.thirdparty.torchmeta.modules.conv import MetaConv1d, MetaConv2d, MetaConv3d
+from lightningdata.thirdparty.torchmeta.modules.linear import MetaLinear, MetaBilinear
+from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
+from lightningdata.thirdparty.torchmeta.modules.normalization import MetaLayerNorm
+from lightningdata.thirdparty.torchmeta.modules.parallel import DataParallel
+from lightningdata.thirdparty.torchmeta.modules.sparse import MetaEmbedding, MetaEmbeddingBag
+
+__all__ = [
+    'MetaMultiheadAttention',
+    'MetaBatchNorm1d', 'MetaBatchNorm2d', 'MetaBatchNorm3d',
+    'MetaSequential',
+    'MetaConv1d', 'MetaConv2d', 'MetaConv3d',
+    'MetaLinear', 'MetaBilinear',
+    'MetaModule',
+    'MetaLayerNorm',
+    'DataParallel',
+    'MetaEmbedding', 'MetaEmbeddingBag',
 ]
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/batchnorm.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/batchnorm.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import torch.nn as nn
-import torch.nn.functional as F
-
-from collections import OrderedDict
-from torch.nn.modules.batchnorm import _BatchNorm
-from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
-
-class _MetaBatchNorm(_BatchNorm, MetaModule):
-    def forward(self, input, params=None):
-        self._check_input_dim(input)
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-
-        # exponential_average_factor is self.momentum set to
-        # (when it is available) only so that if gets updated
-        # in ONNX graph when this node is exported to ONNX.
-        if self.momentum is None:
-            exponential_average_factor = 0.0
-        else:
-            exponential_average_factor = self.momentum
-
-        if self.training and self.track_running_stats:
-            if self.num_batches_tracked is not None:
-                self.num_batches_tracked += 1
-                if self.momentum is None:  # use cumulative moving average
-                    exponential_average_factor = 1.0 / float(self.num_batches_tracked)
-                else:  # use exponential moving average
-                    exponential_average_factor = self.momentum
-
-        weight = params.get('weight', None)
-        bias = params.get('bias', None)
-
-        return F.batch_norm(
-            input, self.running_mean, self.running_var, weight, bias,
-            self.training or not self.track_running_stats,
-            exponential_average_factor, self.eps)
-
-class MetaBatchNorm1d(_MetaBatchNorm):
-    __doc__ = nn.BatchNorm1d.__doc__
-
-    def _check_input_dim(self, input):
-        if input.dim() != 2 and input.dim() != 3:
-            raise ValueError('expected 2D or 3D input (got {}D input)'
-                             .format(input.dim()))
-
-class MetaBatchNorm2d(_MetaBatchNorm):
-    __doc__ = nn.BatchNorm2d.__doc__
-
-    def _check_input_dim(self, input):
-        if input.dim() != 4:
-            raise ValueError('expected 4D input (got {}D input)'
-                             .format(input.dim()))
-
-class MetaBatchNorm3d(_MetaBatchNorm):
-    __doc__ = nn.BatchNorm3d.__doc__
-
-    def _check_input_dim(self, input):
-        if input.dim() != 5:
-            raise ValueError('expected 5D input (got {}D input)'
-                             .format(input.dim()))
+import torch.nn as nn
+import torch.nn.functional as F
+
+from collections import OrderedDict
+from torch.nn.modules.batchnorm import _BatchNorm
+from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
+
+class _MetaBatchNorm(_BatchNorm, MetaModule):
+    def forward(self, input, params=None):
+        self._check_input_dim(input)
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+
+        # exponential_average_factor is self.momentum set to
+        # (when it is available) only so that if gets updated
+        # in ONNX graph when this node is exported to ONNX.
+        if self.momentum is None:
+            exponential_average_factor = 0.0
+        else:
+            exponential_average_factor = self.momentum
+
+        if self.training and self.track_running_stats:
+            if self.num_batches_tracked is not None:
+                self.num_batches_tracked += 1
+                if self.momentum is None:  # use cumulative moving average
+                    exponential_average_factor = 1.0 / float(self.num_batches_tracked)
+                else:  # use exponential moving average
+                    exponential_average_factor = self.momentum
+
+        weight = params.get('weight', None)
+        bias = params.get('bias', None)
+
+        return F.batch_norm(
+            input, self.running_mean, self.running_var, weight, bias,
+            self.training or not self.track_running_stats,
+            exponential_average_factor, self.eps)
+
+class MetaBatchNorm1d(_MetaBatchNorm):
+    __doc__ = nn.BatchNorm1d.__doc__
+
+    def _check_input_dim(self, input):
+        if input.dim() != 2 and input.dim() != 3:
+            raise ValueError('expected 2D or 3D input (got {}D input)'
+                             .format(input.dim()))
+
+class MetaBatchNorm2d(_MetaBatchNorm):
+    __doc__ = nn.BatchNorm2d.__doc__
+
+    def _check_input_dim(self, input):
+        if input.dim() != 4:
+            raise ValueError('expected 4D input (got {}D input)'
+                             .format(input.dim()))
+
+class MetaBatchNorm3d(_MetaBatchNorm):
+    __doc__ = nn.BatchNorm3d.__doc__
+
+    def _check_input_dim(self, input):
+        if input.dim() != 5:
+            raise ValueError('expected 5D input (got {}D input)'
+                             .format(input.dim()))
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/conv.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/conv.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import torch.nn as nn
-import torch.nn.functional as F
-
-from collections import OrderedDict
-from torch.nn.modules.utils import _single, _pair, _triple
-from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
-
-class MetaConv1d(nn.Conv1d, MetaModule):
-    __doc__ = nn.Conv1d.__doc__
-
-    def forward(self, input, params=None):
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-        bias = params.get('bias', None)
-        return self._conv_forward(input, params['weight'], bias)
-
-
-class MetaConv2d(nn.Conv2d, MetaModule):
-    __doc__ = nn.Conv2d.__doc__
-
-    def forward(self, input, params=None):
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-        bias = params.get('bias', None)
-        return self._conv_forward(input, params['weight'], bias)
-
-
-class MetaConv3d(nn.Conv3d, MetaModule):
-    __doc__ = nn.Conv3d.__doc__
-
-    def forward(self, input, params=None):
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-        bias = params.get('bias', None)
-        return self._conv_forward(input, params['weight'], bias)
+import torch.nn as nn
+import torch.nn.functional as F
+
+from collections import OrderedDict
+from torch.nn.modules.utils import _single, _pair, _triple
+from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
+
+class MetaConv1d(nn.Conv1d, MetaModule):
+    __doc__ = nn.Conv1d.__doc__
+
+    def forward(self, input, params=None):
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+        bias = params.get('bias', None)
+        return self._conv_forward(input, params['weight'], bias)
+
+
+class MetaConv2d(nn.Conv2d, MetaModule):
+    __doc__ = nn.Conv2d.__doc__
+
+    def forward(self, input, params=None):
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+        bias = params.get('bias', None)
+        return self._conv_forward(input, params['weight'], bias)
+
+
+class MetaConv3d(nn.Conv3d, MetaModule):
+    __doc__ = nn.Conv3d.__doc__
+
+    def forward(self, input, params=None):
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+        bias = params.get('bias', None)
+        return self._conv_forward(input, params['weight'], bias)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/module.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/module.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import torch
-import torch.nn as nn
-import re
-import warnings
-
-from collections import OrderedDict
-
-
-class MetaModule(nn.Module):
-    """
-    Base class for PyTorch meta-learning modules. These modules accept an
-    additional argument `params` in their `forward` method.
-
-    Notes
-    -----
-    Objects inherited from `MetaModule` are fully compatible with PyTorch
-    modules from `torch.nn.Module`. The argument `params` is a dictionary of
-    tensors, with full support of the computation graph (for differentiation).
-    """
-    def __init__(self):
-        super(MetaModule, self).__init__()
-        self._children_modules_parameters_cache = dict()
-
-    def meta_named_parameters(self, prefix='', recurse=True):
-        gen = self._named_members(
-            lambda module: module._parameters.items()
-            if isinstance(module, MetaModule) else [],
-            prefix=prefix, recurse=recurse)
-        for elem in gen:
-            yield elem
-
-    def meta_parameters(self, recurse=True):
-        for name, param in self.meta_named_parameters(recurse=recurse):
-            yield param
-
-    def get_subdict(self, params, key=None):
-        if params is None:
-            return None
-
-        all_names = tuple(params.keys())
-        if (key, all_names) not in self._children_modules_parameters_cache:
-            if key is None:
-                self._children_modules_parameters_cache[(key, all_names)] = all_names
-
-            else:
-                key_escape = re.escape(key)
-                key_re = re.compile(r'^{0}\.(.+)'.format(key_escape))
-
-                self._children_modules_parameters_cache[(key, all_names)] = [
-                    key_re.sub(r'\1', k) for k in all_names if key_re.match(k) is not None]
-
-        names = self._children_modules_parameters_cache[(key, all_names)]
-        if not names:
-            warnings.warn('Module `{0}` has no parameter corresponding to the '
-                          'submodule named `{1}` in the dictionary `params` '
-                          'provided as an argument to `forward()`. Using the '
-                          'default parameters for this submodule. The list of '
-                          'the parameters in `params`: [{2}].'.format(
-                          self.__class__.__name__, key, ', '.join(all_names)),
-                          stacklevel=2)
-            return None
-
-        return OrderedDict([(name, params[f'{key}.{name}']) for name in names])
+import torch
+import torch.nn as nn
+import re
+import warnings
+
+from collections import OrderedDict
+
+
+class MetaModule(nn.Module):
+    """
+    Base class for PyTorch meta-learning modules. These modules accept an
+    additional argument `params` in their `forward` method.
+
+    Notes
+    -----
+    Objects inherited from `MetaModule` are fully compatible with PyTorch
+    modules from `torch.nn.Module`. The argument `params` is a dictionary of
+    tensors, with full support of the computation graph (for differentiation).
+    """
+    def __init__(self):
+        super(MetaModule, self).__init__()
+        self._children_modules_parameters_cache = dict()
+
+    def meta_named_parameters(self, prefix='', recurse=True):
+        gen = self._named_members(
+            lambda module: module._parameters.items()
+            if isinstance(module, MetaModule) else [],
+            prefix=prefix, recurse=recurse)
+        for elem in gen:
+            yield elem
+
+    def meta_parameters(self, recurse=True):
+        for name, param in self.meta_named_parameters(recurse=recurse):
+            yield param
+
+    def get_subdict(self, params, key=None):
+        if params is None:
+            return None
+
+        all_names = tuple(params.keys())
+        if (key, all_names) not in self._children_modules_parameters_cache:
+            if key is None:
+                self._children_modules_parameters_cache[(key, all_names)] = all_names
+
+            else:
+                key_escape = re.escape(key)
+                key_re = re.compile(r'^{0}\.(.+)'.format(key_escape))
+
+                self._children_modules_parameters_cache[(key, all_names)] = [
+                    key_re.sub(r'\1', k) for k in all_names if key_re.match(k) is not None]
+
+        names = self._children_modules_parameters_cache[(key, all_names)]
+        if not names:
+            warnings.warn('Module `{0}` has no parameter corresponding to the '
+                          'submodule named `{1}` in the dictionary `params` '
+                          'provided as an argument to `forward()`. Using the '
+                          'default parameters for this submodule. The list of '
+                          'the parameters in `params`: [{2}].'.format(
+                          self.__class__.__name__, key, ', '.join(all_names)),
+                          stacklevel=2)
+            return None
+
+        return OrderedDict([(name, params[f'{key}.{name}']) for name in names])
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/parallel.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/parallel.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import torch
-import warnings
-
-from torch.nn import DataParallel as DataParallel_
-from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
-from collections import OrderedDict
-
-from torch.nn.parallel import parallel_apply
-from torch.nn.parallel.scatter_gather import scatter_kwargs
-from torch.nn.parallel.replicate import _broadcast_coalesced_reshape
-
-
-class DataParallel(DataParallel_, MetaModule):
-    __doc__ = DataParallel_.__doc__
-
-    def scatter(self, inputs, kwargs, device_ids):
-        if not isinstance(self.module, MetaModule):
-            return super(DataParallel, self).scatter(inputs, kwargs, device_ids)
-
-        params = kwargs.pop('params', None)
-        inputs_, kwargs_ = scatter_kwargs(inputs, kwargs, device_ids, dim=self.dim)
-        # Add params argument unchanged back in kwargs
-        replicas = self._replicate_params(params, inputs_, device_ids,
-                                          detach=not torch.is_grad_enabled())
-        kwargs_ = tuple(dict(params=replica, **kwarg)
-                        for (kwarg, replica) in zip(kwargs_, replicas))
-        return inputs_, kwargs_
-
-    def _replicate_params(self, params, inputs, device_ids, detach=False):
-        if params is None:
-            module_params = OrderedDict(self.module.named_parameters())
-        else:
-            # Temporarily disable the warning if no parameter with key prefix
-            # `module` was found. In that case, the original params dictionary
-            # is used.
-            with warnings.catch_warnings():
-                warnings.simplefilter('ignore')
-                module_params = self.get_subdict(params, key='module')
-            if module_params is None:
-                module_params = params
-
-        replicas = _broadcast_coalesced_reshape(list(module_params.values()),
-                                                device_ids[:len(inputs)],
-                                                detach)
-        replicas = tuple(OrderedDict(zip(module_params.keys(), replica))
-                         for replica in replicas)
-        return replicas
+import torch
+import warnings
+
+from torch.nn import DataParallel as DataParallel_
+from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
+from collections import OrderedDict
+
+from torch.nn.parallel import parallel_apply
+from torch.nn.parallel.scatter_gather import scatter_kwargs
+from torch.nn.parallel.replicate import _broadcast_coalesced_reshape
+
+
+class DataParallel(DataParallel_, MetaModule):
+    __doc__ = DataParallel_.__doc__
+
+    def scatter(self, inputs, kwargs, device_ids):
+        if not isinstance(self.module, MetaModule):
+            return super(DataParallel, self).scatter(inputs, kwargs, device_ids)
+
+        params = kwargs.pop('params', None)
+        inputs_, kwargs_ = scatter_kwargs(inputs, kwargs, device_ids, dim=self.dim)
+        # Add params argument unchanged back in kwargs
+        replicas = self._replicate_params(params, inputs_, device_ids,
+                                          detach=not torch.is_grad_enabled())
+        kwargs_ = tuple(dict(params=replica, **kwarg)
+                        for (kwarg, replica) in zip(kwargs_, replicas))
+        return inputs_, kwargs_
+
+    def _replicate_params(self, params, inputs, device_ids, detach=False):
+        if params is None:
+            module_params = OrderedDict(self.module.named_parameters())
+        else:
+            # Temporarily disable the warning if no parameter with key prefix
+            # `module` was found. In that case, the original params dictionary
+            # is used.
+            with warnings.catch_warnings():
+                warnings.simplefilter('ignore')
+                module_params = self.get_subdict(params, key='module')
+            if module_params is None:
+                module_params = params
+
+        replicas = _broadcast_coalesced_reshape(list(module_params.values()),
+                                                device_ids[:len(inputs)],
+                                                detach)
+        replicas = tuple(OrderedDict(zip(module_params.keys(), replica))
+                         for replica in replicas)
+        return replicas
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/modules/sparse.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/modules/sparse.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import torch.nn as nn
-import torch.nn.functional as F
-
-from collections import OrderedDict
-from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
-
-class MetaEmbedding(nn.Embedding, MetaModule):
-    __doc__ = nn.Embedding.__doc__
-
-    def forward(self, input, params=None):
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-        return F.embedding(
-            input, params['weight'], self.padding_idx, self.max_norm,
-            self.norm_type, self.scale_grad_by_freq, self.sparse)
-
-class MetaEmbeddingBag(nn.EmbeddingBag, MetaModule):
-    __doc__ = nn.EmbeddingBag.__doc__
-
-    def forward(self, input, offsets=None, per_sample_weights=None, params=None):
-        if params is None:
-            params = OrderedDict(self.named_parameters())
-        return F.embedding_bag(input, params['weight'], offsets,
-                               self.max_norm, self.norm_type,
-                               self.scale_grad_by_freq, self.mode, self.sparse,
-                               per_sample_weights, self.include_last_offset)
+import torch.nn as nn
+import torch.nn.functional as F
+
+from collections import OrderedDict
+from lightningdata.thirdparty.torchmeta.modules.module import MetaModule
+
+class MetaEmbedding(nn.Embedding, MetaModule):
+    __doc__ = nn.Embedding.__doc__
+
+    def forward(self, input, params=None):
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+        return F.embedding(
+            input, params['weight'], self.padding_idx, self.max_norm,
+            self.norm_type, self.scale_grad_by_freq, self.sparse)
+
+class MetaEmbeddingBag(nn.EmbeddingBag, MetaModule):
+    __doc__ = nn.EmbeddingBag.__doc__
+
+    def forward(self, input, offsets=None, per_sample_weights=None, params=None):
+        if params is None:
+            params = OrderedDict(self.named_parameters())
+        return F.embedding_bag(input, params['weight'], offsets,
+                               self.max_norm, self.norm_type,
+                               self.scale_grad_by_freq, self.mode, self.sparse,
+                               per_sample_weights, self.include_last_offset)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/harmonic.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/harmonic.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import numpy as np
-
-from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
-
-
-class Harmonic(MetaDataset):
-    """
-    Simple regression task, based on the sum of two sine waves, as introduced
-    in [1].
-
-    Parameters
-    ----------
-    num_samples_per_task : int
-        Number of examples per task.
-
-    num_tasks : int (default: 5,000)
-        Overall number of tasks to sample.
-
-    noise_std : float, optional
-        Amount of noise to include in the targets for each task. If `None`, then
-        nos noise is included, and the target is the sum of 2 sine functions of
-        the input.
-
-    transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the input.
-
-    target_transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the target.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    Notes
-    -----
-    The tasks are created randomly as the sum of two sinusoid functions, with
-    a frequency ratio of 2. The amplitudes vary within [5.0, 7.0], the phases
-    within [0, 2 * pi], and the inputs are sampled according to N(mu_x, 1), with
-    mu_x varying in [-4.0, 4.0]. Due to the way PyTorch handles datasets, the
-    number of tasks to be sampled needs to be fixed ahead of time (with
-    `num_tasks`). This will typically be equal to `meta_batch_size * num_batches`.
-
-    References
-    ----------
-    .. [1] Lacoste A., Oreshkin B., Chung W., Boquet T., Rostamzadeh N.,
-           Krueger D. (2018). Uncertainty in Multitask Transfer Learning. In
-           Advances in Neural Information Processing Systems (https://arxiv.org/abs/1806.07528)
-    """
-    def __init__(self, num_samples_per_task, num_tasks=5000,
-                 noise_std=None, transform=None, target_transform=None,
-                 dataset_transform=None):
-        super(Harmonic, self).__init__(meta_split='train',
-            target_transform=target_transform, dataset_transform=dataset_transform)
-        self.num_samples_per_task = num_samples_per_task
-        self.num_tasks = num_tasks
-        self.noise_std = noise_std
-        self.transform = transform
-
-        self._domain_range = np.array([-4.0, 4.0])
-        self._frequency_range = np.array([5.0, 7.0])
-        self._phase_range = np.array([0, 2 * np.pi])
-
-        self._domains = None
-        self._frequencies = None
-        self._phases = None
-        self._amplitudes = None
-
-    @property
-    def domains(self):
-        if self._domains is None:
-            self._domains = self.np_random.uniform(self._domain_range[0],
-                self._domain_range[1], size=self.num_tasks)
-        return self._domains
-
-    @property
-    def frequencies(self):
-        if self._frequencies is None:
-            self._frequencies = self.np_random.uniform(self._frequency_range[0],
-                self._frequency_range[1], size=self.num_tasks)
-        return self._frequencies
-
-    @property
-    def phases(self):
-        if self._phases is None:
-            self._phases = self.np_random.uniform(self._phase_range[0],
-                self._phase_range[1], size=(self.num_tasks, 2))
-        return self._phases
-
-    @property
-    def amplitudes(self):
-        if self._amplitudes is None:
-            self._amplitudes = self.np_random.randn(self.num_tasks, 2)
-        return self._amplitudes
-
-    def __len__(self):
-        return self.num_tasks
-
-    def __getitem__(self, index):
-        domain = self.domains[index]
-        frequency = self.frequencies[index]
-        phases = self.phases[index]
-        amplitudes = self.amplitudes[index]
-
-        task = HarmonicTask(index, domain, frequency, phases, amplitudes,
-            self.noise_std, self.num_samples_per_task, self.transform,
-            self.target_transform, np_random=self.np_random)
-
-        if self.dataset_transform is not None:
-            task = self.dataset_transform(task)
-
-        return task
-
-
-class HarmonicTask(Task):
-    def __init__(self, index, domain, frequency, phases, amplitudes,
-                 noise_std, num_samples, transform=None,
-                 target_transform=None, np_random=None):
-        super(HarmonicTask, self).__init__(index, None) # Regression task
-        self.domain = domain
-        self.frequency = frequency
-        self.phases = phases
-        self.amplitudes = amplitudes
-        self.noise_std = noise_std
-        self.num_samples = num_samples
-
-        self.transform = transform
-        self.target_transform = target_transform
-
-        if np_random is None:
-            np_random = np.random.RandomState(None)
-
-        a_1, a_2 = self.amplitudes
-        b_1, b_2 = self.phases
-
-        self._inputs = self.domain + np_random.randn(num_samples, 1)
-        self._targets = (a_1 * np.sin(frequency * self._inputs + b_1)
-            + a_2 * np.sin(2 * frequency * self._inputs + b_2))
-        if (noise_std is not None) and (noise_std > 0.):
-            self._targets += noise_std * np_random.randn(num_samples, 1)
-
-    def __len__(self):
-        return self.num_samples
-
-    def __getitem__(self, index):
-        input, target = self._inputs[index], self._targets[index]
-
-        if self.transform is not None:
-            input = self.transform(input)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (input, target)
+import numpy as np
+
+from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
+
+
+class Harmonic(MetaDataset):
+    """
+    Simple regression task, based on the sum of two sine waves, as introduced
+    in [1].
+
+    Parameters
+    ----------
+    num_samples_per_task : int
+        Number of examples per task.
+
+    num_tasks : int (default: 5,000)
+        Overall number of tasks to sample.
+
+    noise_std : float, optional
+        Amount of noise to include in the targets for each task. If `None`, then
+        nos noise is included, and the target is the sum of 2 sine functions of
+        the input.
+
+    transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the input.
+
+    target_transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the target.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    Notes
+    -----
+    The tasks are created randomly as the sum of two sinusoid functions, with
+    a frequency ratio of 2. The amplitudes vary within [5.0, 7.0], the phases
+    within [0, 2 * pi], and the inputs are sampled according to N(mu_x, 1), with
+    mu_x varying in [-4.0, 4.0]. Due to the way PyTorch handles datasets, the
+    number of tasks to be sampled needs to be fixed ahead of time (with
+    `num_tasks`). This will typically be equal to `meta_batch_size * num_batches`.
+
+    References
+    ----------
+    .. [1] Lacoste A., Oreshkin B., Chung W., Boquet T., Rostamzadeh N.,
+           Krueger D. (2018). Uncertainty in Multitask Transfer Learning. In
+           Advances in Neural Information Processing Systems (https://arxiv.org/abs/1806.07528)
+    """
+    def __init__(self, num_samples_per_task, num_tasks=5000,
+                 noise_std=None, transform=None, target_transform=None,
+                 dataset_transform=None):
+        super(Harmonic, self).__init__(meta_split='train',
+            target_transform=target_transform, dataset_transform=dataset_transform)
+        self.num_samples_per_task = num_samples_per_task
+        self.num_tasks = num_tasks
+        self.noise_std = noise_std
+        self.transform = transform
+
+        self._domain_range = np.array([-4.0, 4.0])
+        self._frequency_range = np.array([5.0, 7.0])
+        self._phase_range = np.array([0, 2 * np.pi])
+
+        self._domains = None
+        self._frequencies = None
+        self._phases = None
+        self._amplitudes = None
+
+    @property
+    def domains(self):
+        if self._domains is None:
+            self._domains = self.np_random.uniform(self._domain_range[0],
+                self._domain_range[1], size=self.num_tasks)
+        return self._domains
+
+    @property
+    def frequencies(self):
+        if self._frequencies is None:
+            self._frequencies = self.np_random.uniform(self._frequency_range[0],
+                self._frequency_range[1], size=self.num_tasks)
+        return self._frequencies
+
+    @property
+    def phases(self):
+        if self._phases is None:
+            self._phases = self.np_random.uniform(self._phase_range[0],
+                self._phase_range[1], size=(self.num_tasks, 2))
+        return self._phases
+
+    @property
+    def amplitudes(self):
+        if self._amplitudes is None:
+            self._amplitudes = self.np_random.randn(self.num_tasks, 2)
+        return self._amplitudes
+
+    def __len__(self):
+        return self.num_tasks
+
+    def __getitem__(self, index):
+        domain = self.domains[index]
+        frequency = self.frequencies[index]
+        phases = self.phases[index]
+        amplitudes = self.amplitudes[index]
+
+        task = HarmonicTask(index, domain, frequency, phases, amplitudes,
+            self.noise_std, self.num_samples_per_task, self.transform,
+            self.target_transform, np_random=self.np_random)
+
+        if self.dataset_transform is not None:
+            task = self.dataset_transform(task)
+
+        return task
+
+
+class HarmonicTask(Task):
+    def __init__(self, index, domain, frequency, phases, amplitudes,
+                 noise_std, num_samples, transform=None,
+                 target_transform=None, np_random=None):
+        super(HarmonicTask, self).__init__(index, None) # Regression task
+        self.domain = domain
+        self.frequency = frequency
+        self.phases = phases
+        self.amplitudes = amplitudes
+        self.noise_std = noise_std
+        self.num_samples = num_samples
+
+        self.transform = transform
+        self.target_transform = target_transform
+
+        if np_random is None:
+            np_random = np.random.RandomState(None)
+
+        a_1, a_2 = self.amplitudes
+        b_1, b_2 = self.phases
+
+        self._inputs = self.domain + np_random.randn(num_samples, 1)
+        self._targets = (a_1 * np.sin(frequency * self._inputs + b_1)
+            + a_2 * np.sin(2 * frequency * self._inputs + b_2))
+        if (noise_std is not None) and (noise_std > 0.):
+            self._targets += noise_std * np_random.randn(num_samples, 1)
+
+    def __len__(self):
+        return self.num_samples
+
+    def __getitem__(self, index):
+        input, target = self._inputs[index], self._targets[index]
+
+        if self.transform is not None:
+            input = self.transform(input)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (input, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/helpers.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/helpers.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import warnings
-
-from lightningdata.thirdparty.torchmeta.toy import Sinusoid, Harmonic
-from lightningdata.thirdparty.torchmeta.transforms import ClassSplitter
-
-def sinusoid(shots, shuffle=True, test_shots=None, seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Sinusoid toy dataset.
-
-    Parameters
-    ----------
-    shots : int
-        Number of (training) examples in each task. This corresponds to `k` in
-        `k-shot` classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples in each task. If `None`, then the number of test
-        examples is equal to the number of training examples in each task.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `Sinusoid` class.
-
-    See also
-    --------
-    `torchmeta.toy.Sinusoid` : Meta-dataset for the Sinusoid toy dataset.
-    """
-    if 'num_samples_per_task' in kwargs:
-        warnings.warn('Both arguments `shots` and `num_samples_per_task` were '
-            'set in the helper function for the number of samples in each task. '
-            'Ignoring the argument `shots`.', stacklevel=2)
-        if test_shots is not None:
-            shots = kwargs['num_samples_per_task'] - test_shots
-            if shots <= 0:
-                raise ValueError('The argument `test_shots` ({0}) is greater '
-                    'than the number of samples per task ({1}). Either use the '
-                    'argument `shots` instead of `num_samples_per_task`, or '
-                    'increase the value of `num_samples_per_task`.'.format(
-                    test_shots, kwargs['num_samples_per_task']))
-        else:
-            shots = kwargs['num_samples_per_task'] // 2
-    if test_shots is None:
-        test_shots = shots
-
-    dataset = Sinusoid(num_samples_per_task=shots + test_shots, **kwargs)
-    dataset = ClassSplitter(dataset, shuffle=shuffle,
-        num_train_per_class=shots, num_test_per_class=test_shots)
-    dataset.seed(seed)
-
-    return dataset
-
-def harmonic(shots, shuffle=True, test_shots=None, seed=None, **kwargs):
-    """Helper function to create a meta-dataset for the Harmonic toy dataset.
-
-    Parameters
-    ----------
-    shots : int
-        Number of (training) examples in each task. This corresponds to `k` in
-        `k-shot` classification.
-
-    shuffle : bool (default: `True`)
-        Shuffle the examples when creating the tasks.
-
-    test_shots : int, optional
-        Number of test examples in each task. If `None`, then the number of test
-        examples is equal to the number of training examples in each task.
-
-    seed : int, optional
-        Random seed to be used in the meta-dataset.
-
-    kwargs
-        Additional arguments passed to the `Harmonic` class.
-
-    See also
-    --------
-    `torchmeta.toy.Harmonic` : Meta-dataset for the Harmonic toy dataset.
-    """
-    if 'num_samples_per_task' in kwargs:
-        warnings.warn('Both arguments `shots` and `num_samples_per_task` were '
-            'set in the helper function for the number of samples in each task. '
-            'Ignoring the argument `shots`.', stacklevel=2)
-        if test_shots is not None:
-            shots = kwargs['num_samples_per_task'] - test_shots
-            if shots <= 0:
-                raise ValueError('The argument `test_shots` ({0}) is greater '
-                    'than the number of samples per task ({1}). Either use the '
-                    'argument `shots` instead of `num_samples_per_task`, or '
-                    'increase the value of `num_samples_per_task`.'.format(
-                    test_shots, kwargs['num_samples_per_task']))
-        else:
-            shots = kwargs['num_samples_per_task'] // 2
-    if test_shots is None:
-        test_shots = shots
-
-    dataset = Harmonic(num_samples_per_task=shots + test_shots, **kwargs)
-    dataset = ClassSplitter(dataset, shuffle=shuffle,
-        num_train_per_class=shots, num_test_per_class=test_shots)
-    dataset.seed(seed)
-
-    return dataset
+import warnings
+
+from lightningdata.thirdparty.torchmeta.toy import Sinusoid, Harmonic
+from lightningdata.thirdparty.torchmeta.transforms import ClassSplitter
+
+def sinusoid(shots, shuffle=True, test_shots=None, seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Sinusoid toy dataset.
+
+    Parameters
+    ----------
+    shots : int
+        Number of (training) examples in each task. This corresponds to `k` in
+        `k-shot` classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples in each task. If `None`, then the number of test
+        examples is equal to the number of training examples in each task.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `Sinusoid` class.
+
+    See also
+    --------
+    `torchmeta.toy.Sinusoid` : Meta-dataset for the Sinusoid toy dataset.
+    """
+    if 'num_samples_per_task' in kwargs:
+        warnings.warn('Both arguments `shots` and `num_samples_per_task` were '
+            'set in the helper function for the number of samples in each task. '
+            'Ignoring the argument `shots`.', stacklevel=2)
+        if test_shots is not None:
+            shots = kwargs['num_samples_per_task'] - test_shots
+            if shots <= 0:
+                raise ValueError('The argument `test_shots` ({0}) is greater '
+                    'than the number of samples per task ({1}). Either use the '
+                    'argument `shots` instead of `num_samples_per_task`, or '
+                    'increase the value of `num_samples_per_task`.'.format(
+                    test_shots, kwargs['num_samples_per_task']))
+        else:
+            shots = kwargs['num_samples_per_task'] // 2
+    if test_shots is None:
+        test_shots = shots
+
+    dataset = Sinusoid(num_samples_per_task=shots + test_shots, **kwargs)
+    dataset = ClassSplitter(dataset, shuffle=shuffle,
+        num_train_per_class=shots, num_test_per_class=test_shots)
+    dataset.seed(seed)
+
+    return dataset
+
+def harmonic(shots, shuffle=True, test_shots=None, seed=None, **kwargs):
+    """Helper function to create a meta-dataset for the Harmonic toy dataset.
+
+    Parameters
+    ----------
+    shots : int
+        Number of (training) examples in each task. This corresponds to `k` in
+        `k-shot` classification.
+
+    shuffle : bool (default: `True`)
+        Shuffle the examples when creating the tasks.
+
+    test_shots : int, optional
+        Number of test examples in each task. If `None`, then the number of test
+        examples is equal to the number of training examples in each task.
+
+    seed : int, optional
+        Random seed to be used in the meta-dataset.
+
+    kwargs
+        Additional arguments passed to the `Harmonic` class.
+
+    See also
+    --------
+    `torchmeta.toy.Harmonic` : Meta-dataset for the Harmonic toy dataset.
+    """
+    if 'num_samples_per_task' in kwargs:
+        warnings.warn('Both arguments `shots` and `num_samples_per_task` were '
+            'set in the helper function for the number of samples in each task. '
+            'Ignoring the argument `shots`.', stacklevel=2)
+        if test_shots is not None:
+            shots = kwargs['num_samples_per_task'] - test_shots
+            if shots <= 0:
+                raise ValueError('The argument `test_shots` ({0}) is greater '
+                    'than the number of samples per task ({1}). Either use the '
+                    'argument `shots` instead of `num_samples_per_task`, or '
+                    'increase the value of `num_samples_per_task`.'.format(
+                    test_shots, kwargs['num_samples_per_task']))
+        else:
+            shots = kwargs['num_samples_per_task'] // 2
+    if test_shots is None:
+        test_shots = shots
+
+    dataset = Harmonic(num_samples_per_task=shots + test_shots, **kwargs)
+    dataset = ClassSplitter(dataset, shuffle=shuffle,
+        num_train_per_class=shots, num_test_per_class=test_shots)
+    dataset.seed(seed)
+
+    return dataset
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/sinusoid.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import numpy as np
-
-from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
-
-
-class Sinusoid(MetaDataset):
-    """
-    Simple regression task, based on sinusoids, as introduced in [1].
-
-    Parameters
-    ----------
-    num_samples_per_task : int
-        Number of examples per task.
-
-    num_tasks : int (default: 1,000,000)
-        Overall number of tasks to sample.
-
-    noise_std : float, optional
-        Amount of noise to include in the targets for each task. If `None`, then
-        nos noise is included, and the target is a sine function of the input.
-
-    transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the input.
-
-    target_transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the target.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    Notes
-    -----
-    The tasks are created randomly as random sinusoid function. The amplitude
-    varies within [0.1, 5.0], the phase within [0, pi], and the inputs are
-    sampled uniformly in [-5.0, 5.0]. Due to the way PyTorch handles datasets,
-    the number of tasks to be sampled needs to be fixed ahead of time (with
-    `num_tasks`). This will typically be equal to `meta_batch_size * num_batches`.
-
-    References
-    ----------
-    .. [1] Finn C., Abbeel P., and Levine, S. (2017). Model-Agnostic Meta-Learning
-           for Fast Adaptation of Deep Networks. International Conference on
-           Machine Learning (ICML) (https://arxiv.org/abs/1703.03400)
-    """
-    def __init__(self, num_samples_per_task, num_tasks=1000000,
-                 noise_std=None, transform=None, target_transform=None,
-                 dataset_transform=None):
-        super(Sinusoid, self).__init__(meta_split='train',
-            target_transform=target_transform, dataset_transform=dataset_transform)
-        self.num_samples_per_task = num_samples_per_task
-        self.num_tasks = num_tasks
-        self.noise_std = noise_std
-        self.transform = transform
-
-        self._input_range = np.array([-5.0, 5.0])
-        self._amplitude_range = np.array([0.1, 5.0])
-        self._phase_range = np.array([0, np.pi])
-
-        self._amplitudes = None
-        self._phases = None
-
-    @property
-    def amplitudes(self):
-        if self._amplitudes is None:
-            self._amplitudes = self.np_random.uniform(self._amplitude_range[0],
-                self._amplitude_range[1], size=self.num_tasks)
-        return self._amplitudes
-
-    @property
-    def phases(self):
-        if self._phases is None:
-            self._phases = self.np_random.uniform(self._phase_range[0],
-                self._phase_range[1], size=self.num_tasks)
-        return self._phases
-
-    def __len__(self):
-        return self.num_tasks
-
-    def __getitem__(self, index):
-        amplitude, phase = self.amplitudes[index], self.phases[index]
-        task = SinusoidTask(index, amplitude, phase, self._input_range,
-            self.noise_std, self.num_samples_per_task, self.transform,
-            self.target_transform, np_random=self.np_random)
-
-        if self.dataset_transform is not None:
-            task = self.dataset_transform(task)
-
-        return task
-
-
-class SinusoidTask(Task):
-    def __init__(self, index, amplitude, phase, input_range, noise_std,
-                 num_samples, transform=None, target_transform=None,
-                 np_random=None):
-        super(SinusoidTask, self).__init__(index, None) # Regression task
-        self.amplitude = amplitude
-        self.phase = phase
-        self.input_range = input_range
-        self.num_samples = num_samples
-        self.noise_std = noise_std
-
-        self.transform = transform
-        self.target_transform = target_transform
-
-        if np_random is None:
-            np_random = np.random.RandomState(None)
-
-        self._inputs = np_random.uniform(input_range[0], input_range[1],
-            size=(num_samples, 1))
-        self._targets = amplitude * np.sin(self._inputs - phase)
-        if (noise_std is not None) and (noise_std > 0.):
-            self._targets += noise_std * np_random.randn(num_samples, 1)
-
-    def __len__(self):
-        return self.num_samples
-
-    def __getitem__(self, index):
-        input, target = self._inputs[index], self._targets[index]
-
-        if self.transform is not None:
-            input = self.transform(input)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (input, target)
+import numpy as np
+
+from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
+
+
+class Sinusoid(MetaDataset):
+    """
+    Simple regression task, based on sinusoids, as introduced in [1].
+
+    Parameters
+    ----------
+    num_samples_per_task : int
+        Number of examples per task.
+
+    num_tasks : int (default: 1,000,000)
+        Overall number of tasks to sample.
+
+    noise_std : float, optional
+        Amount of noise to include in the targets for each task. If `None`, then
+        nos noise is included, and the target is a sine function of the input.
+
+    transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the input.
+
+    target_transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the target.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    Notes
+    -----
+    The tasks are created randomly as random sinusoid function. The amplitude
+    varies within [0.1, 5.0], the phase within [0, pi], and the inputs are
+    sampled uniformly in [-5.0, 5.0]. Due to the way PyTorch handles datasets,
+    the number of tasks to be sampled needs to be fixed ahead of time (with
+    `num_tasks`). This will typically be equal to `meta_batch_size * num_batches`.
+
+    References
+    ----------
+    .. [1] Finn C., Abbeel P., and Levine, S. (2017). Model-Agnostic Meta-Learning
+           for Fast Adaptation of Deep Networks. International Conference on
+           Machine Learning (ICML) (https://arxiv.org/abs/1703.03400)
+    """
+    def __init__(self, num_samples_per_task, num_tasks=1000000,
+                 noise_std=None, transform=None, target_transform=None,
+                 dataset_transform=None):
+        super(Sinusoid, self).__init__(meta_split='train',
+            target_transform=target_transform, dataset_transform=dataset_transform)
+        self.num_samples_per_task = num_samples_per_task
+        self.num_tasks = num_tasks
+        self.noise_std = noise_std
+        self.transform = transform
+
+        self._input_range = np.array([-5.0, 5.0])
+        self._amplitude_range = np.array([0.1, 5.0])
+        self._phase_range = np.array([0, np.pi])
+
+        self._amplitudes = None
+        self._phases = None
+
+    @property
+    def amplitudes(self):
+        if self._amplitudes is None:
+            self._amplitudes = self.np_random.uniform(self._amplitude_range[0],
+                self._amplitude_range[1], size=self.num_tasks)
+        return self._amplitudes
+
+    @property
+    def phases(self):
+        if self._phases is None:
+            self._phases = self.np_random.uniform(self._phase_range[0],
+                self._phase_range[1], size=self.num_tasks)
+        return self._phases
+
+    def __len__(self):
+        return self.num_tasks
+
+    def __getitem__(self, index):
+        amplitude, phase = self.amplitudes[index], self.phases[index]
+        task = SinusoidTask(index, amplitude, phase, self._input_range,
+            self.noise_std, self.num_samples_per_task, self.transform,
+            self.target_transform, np_random=self.np_random)
+
+        if self.dataset_transform is not None:
+            task = self.dataset_transform(task)
+
+        return task
+
+
+class SinusoidTask(Task):
+    def __init__(self, index, amplitude, phase, input_range, noise_std,
+                 num_samples, transform=None, target_transform=None,
+                 np_random=None):
+        super(SinusoidTask, self).__init__(index, None) # Regression task
+        self.amplitude = amplitude
+        self.phase = phase
+        self.input_range = input_range
+        self.num_samples = num_samples
+        self.noise_std = noise_std
+
+        self.transform = transform
+        self.target_transform = target_transform
+
+        if np_random is None:
+            np_random = np.random.RandomState(None)
+
+        self._inputs = np_random.uniform(input_range[0], input_range[1],
+            size=(num_samples, 1))
+        self._targets = amplitude * np.sin(self._inputs - phase)
+        if (noise_std is not None) and (noise_std > 0.):
+            self._targets += noise_std * np_random.randn(num_samples, 1)
+
+    def __len__(self):
+        return self.num_samples
+
+    def __getitem__(self, index):
+        input, target = self._inputs[index], self._targets[index]
+
+        if self.transform is not None:
+            input = self.transform(input)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (input, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-import numpy as np
-
-from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
-from lightningdata.thirdparty.torchmeta.toy.sinusoid import SinusoidTask
-
-
-class SinusoidAndLine(MetaDataset):
-    """
-    Simple multimodal regression task, based on sinusoids and lines, as
-    introduced in [1].
-
-    Parameters
-    ----------
-    num_samples_per_task : int
-        Number of examples per task.
-
-    num_tasks : int (default: 1,000,000)
-        Overall number of tasks to sample.
-
-    noise_std : float, optional
-        Amount of noise to include in the targets for each task. If `None`, then
-        nos noise is included, and the target is either a sine function, or a
-        linear function of the input.
-
-    transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the input.
-
-    target_transform : callable, optional
-        A function/transform that takes a numpy array of size (1,) and returns a
-        transformed version of the target.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
-
-    Notes
-    -----
-    The tasks are created randomly as either random sinusoid functions, or
-    random linear functions. The amplitude of the sinusoids varies within
-    [0.1, 5.0] and the phase within [0, pi]. The slope and intercept of the lines
-    vary in [-3.0, 3.0]. The inputs are sampled uniformly in [-5.0, 5.0]. Due to
-    the way PyTorch handles datasets, the number of tasks to be sampled needs to
-    be fixed ahead of time (with `num_tasks`). This will typically be equal to
-    `meta_batch_size * num_batches`.
-
-    References
-    ----------
-    .. [1] Finn C., Xu K., Levine S. (2018). Probabilistic Model-Agnostic
-           Meta-Learning. In Advances in Neural Information Processing Systems
-           (https://arxiv.org/abs/1806.02817)
-    """
-    def __init__(self, num_samples_per_task, num_tasks=1000000,
-                 noise_std=None, transform=None, target_transform=None,
-                 dataset_transform=None):
-        super(SinusoidAndLine, self).__init__(meta_split='train',
-            target_transform=target_transform, dataset_transform=dataset_transform)
-        self.num_samples_per_task = num_samples_per_task
-        self.num_tasks = num_tasks
-        self.noise_std = noise_std
-        self.transform = transform
-
-        self._input_range = np.array([-5.0, 5.0])
-        self._amplitude_range = np.array([0.1, 5.0])
-        self._phase_range = np.array([0, np.pi])
-        self._slope_range = np.array([-3.0, 3.0])
-        self._intercept_range = np.array([-3.0, 3.0])
-
-        
-        self._is_sinusoid = None
-        self._amplitudes = None
-        self._phases = None
-        self._slopes = None
-        self._intercepts = None
-
-    @property
-    def amplitudes(self):
-        if self._amplitudes is None:
-            self._amplitudes = self.np_random.uniform(self._amplitude_range[0],
-                self._amplitude_range[1], size=self.num_tasks)
-        return self._amplitudes
-
-    @property
-    def phases(self):
-        if self._phases is None:
-            self._phases = self.np_random.uniform(self._phase_range[0],
-                self._phase_range[1], size=self.num_tasks)
-        return self._phases
-
-    @property
-    def slopes(self):
-        if self._slopes is None:
-            self._slopes = self.np_random.uniform(self._slope_range[0],
-                self._slope_range[1], size=self.num_tasks)
-        return self._slopes
-
-    @property
-    def intercepts(self):
-        if self._intercepts is None:
-            self._intercepts = self.np_random.uniform(self._intercept_range[0],
-                self._intercept_range[1], size=self.num_tasks)
-        return self._intercepts
-
-    @property
-    def is_sinusoid(self):
-        if self._is_sinusoid is None:
-            self._is_sinusoid = np.zeros((self.num_tasks,), dtype=np.bool_)
-            self._is_sinusoid[self.num_tasks // 2:] = True
-            self.np_random.shuffle(self._is_sinusoid)
-        return self._is_sinusoid
-
-    def __len__(self):
-        return self.num_tasks
-
-    def __getitem__(self, index):
-        if self.is_sinusoid[index]:
-            amplitude, phase = self.amplitudes[index], self.phases[index]
-            task = SinusoidTask(index, amplitude, phase, self._input_range,
-                self.noise_std, self.num_samples_per_task, self.transform,
-                self.target_transform, np_random=self.np_random)
-        else:
-            slope, intercept = self.slopes[index], self.intercepts[index]
-            task = LinearTask(index, slope, intercept, self._input_range,
-                self.noise_std, self.num_samples_per_task, self.transform,
-                self.target_transform, np_random=self.np_random)
-
-        if self.dataset_transform is not None:
-            task = self.dataset_transform(task)
-
-        return task
-
-
-class LinearTask(Task):
-    def __init__(self, index, slope, intercept, input_range, noise_std,
-                 num_samples, transform=None, target_transform=None,
-                 np_random=None):
-        super(LinearTask, self).__init__(index, None) # Regression task
-        self.slope = slope
-        self.intercept = intercept
-        self.input_range = input_range
-        self.num_samples = num_samples
-        self.noise_std = noise_std
-
-        self.transform = transform
-        self.target_transform = target_transform
-
-        if np_random is None:
-            np_random = np.random.RandomState(None)
-
-        self._inputs = np_random.uniform(input_range[0], input_range[1],
-            size=(num_samples, 1))
-        self._targets = intercept + slope * self._inputs
-        if (noise_std is not None) and (noise_std > 0.):
-            self._targets += noise_std * np_random.randn(num_samples, 1)
-
-    def __len__(self):
-        return self.num_samples
-
-    def __getitem__(self, index):
-        input, target = self._inputs[index], self._targets[index]
-
-        if self.transform is not None:
-            input = self.transform(input)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return (input, target)
+import numpy as np
+
+from lightningdata.thirdparty.torchmeta.utils.data import Task, MetaDataset
+from lightningdata.thirdparty.torchmeta.toy.sinusoid import SinusoidTask
+
+
+class SinusoidAndLine(MetaDataset):
+    """
+    Simple multimodal regression task, based on sinusoids and lines, as
+    introduced in [1].
+
+    Parameters
+    ----------
+    num_samples_per_task : int
+        Number of examples per task.
+
+    num_tasks : int (default: 1,000,000)
+        Overall number of tasks to sample.
+
+    noise_std : float, optional
+        Amount of noise to include in the targets for each task. If `None`, then
+        nos noise is included, and the target is either a sine function, or a
+        linear function of the input.
+
+    transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the input.
+
+    target_transform : callable, optional
+        A function/transform that takes a numpy array of size (1,) and returns a
+        transformed version of the target.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `torchmeta.transforms.ClassSplitter()`.
+
+    Notes
+    -----
+    The tasks are created randomly as either random sinusoid functions, or
+    random linear functions. The amplitude of the sinusoids varies within
+    [0.1, 5.0] and the phase within [0, pi]. The slope and intercept of the lines
+    vary in [-3.0, 3.0]. The inputs are sampled uniformly in [-5.0, 5.0]. Due to
+    the way PyTorch handles datasets, the number of tasks to be sampled needs to
+    be fixed ahead of time (with `num_tasks`). This will typically be equal to
+    `meta_batch_size * num_batches`.
+
+    References
+    ----------
+    .. [1] Finn C., Xu K., Levine S. (2018). Probabilistic Model-Agnostic
+           Meta-Learning. In Advances in Neural Information Processing Systems
+           (https://arxiv.org/abs/1806.02817)
+    """
+    def __init__(self, num_samples_per_task, num_tasks=1000000,
+                 noise_std=None, transform=None, target_transform=None,
+                 dataset_transform=None):
+        super(SinusoidAndLine, self).__init__(meta_split='train',
+            target_transform=target_transform, dataset_transform=dataset_transform)
+        self.num_samples_per_task = num_samples_per_task
+        self.num_tasks = num_tasks
+        self.noise_std = noise_std
+        self.transform = transform
+
+        self._input_range = np.array([-5.0, 5.0])
+        self._amplitude_range = np.array([0.1, 5.0])
+        self._phase_range = np.array([0, np.pi])
+        self._slope_range = np.array([-3.0, 3.0])
+        self._intercept_range = np.array([-3.0, 3.0])
+
+        
+        self._is_sinusoid = None
+        self._amplitudes = None
+        self._phases = None
+        self._slopes = None
+        self._intercepts = None
+
+    @property
+    def amplitudes(self):
+        if self._amplitudes is None:
+            self._amplitudes = self.np_random.uniform(self._amplitude_range[0],
+                self._amplitude_range[1], size=self.num_tasks)
+        return self._amplitudes
+
+    @property
+    def phases(self):
+        if self._phases is None:
+            self._phases = self.np_random.uniform(self._phase_range[0],
+                self._phase_range[1], size=self.num_tasks)
+        return self._phases
+
+    @property
+    def slopes(self):
+        if self._slopes is None:
+            self._slopes = self.np_random.uniform(self._slope_range[0],
+                self._slope_range[1], size=self.num_tasks)
+        return self._slopes
+
+    @property
+    def intercepts(self):
+        if self._intercepts is None:
+            self._intercepts = self.np_random.uniform(self._intercept_range[0],
+                self._intercept_range[1], size=self.num_tasks)
+        return self._intercepts
+
+    @property
+    def is_sinusoid(self):
+        if self._is_sinusoid is None:
+            self._is_sinusoid = np.zeros((self.num_tasks,), dtype=np.bool_)
+            self._is_sinusoid[self.num_tasks // 2:] = True
+            self.np_random.shuffle(self._is_sinusoid)
+        return self._is_sinusoid
+
+    def __len__(self):
+        return self.num_tasks
+
+    def __getitem__(self, index):
+        if self.is_sinusoid[index]:
+            amplitude, phase = self.amplitudes[index], self.phases[index]
+            task = SinusoidTask(index, amplitude, phase, self._input_range,
+                self.noise_std, self.num_samples_per_task, self.transform,
+                self.target_transform, np_random=self.np_random)
+        else:
+            slope, intercept = self.slopes[index], self.intercepts[index]
+            task = LinearTask(index, slope, intercept, self._input_range,
+                self.noise_std, self.num_samples_per_task, self.transform,
+                self.target_transform, np_random=self.np_random)
+
+        if self.dataset_transform is not None:
+            task = self.dataset_transform(task)
+
+        return task
+
+
+class LinearTask(Task):
+    def __init__(self, index, slope, intercept, input_range, noise_std,
+                 num_samples, transform=None, target_transform=None,
+                 np_random=None):
+        super(LinearTask, self).__init__(index, None) # Regression task
+        self.slope = slope
+        self.intercept = intercept
+        self.input_range = input_range
+        self.num_samples = num_samples
+        self.noise_std = noise_std
+
+        self.transform = transform
+        self.target_transform = target_transform
+
+        if np_random is None:
+            np_random = np.random.RandomState(None)
+
+        self._inputs = np_random.uniform(input_range[0], input_range[1],
+            size=(num_samples, 1))
+        self._targets = intercept + slope * self._inputs
+        if (noise_std is not None) and (noise_std > 0.):
+            self._targets += noise_std * np_random.randn(num_samples, 1)
+
+    def __len__(self):
+        return self.num_samples
+
+    def __getitem__(self, index):
+        input, target = self._inputs[index], self._targets[index]
+
+        if self.transform is not None:
+            input = self.transform(input)
+
+        if self.target_transform is not None:
+            target = self.target_transform(target)
+
+        return (input, target)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-from lightningdata.thirdparty.torchmeta.transforms.categorical import Categorical, FixedCategory
-from lightningdata.thirdparty.torchmeta.transforms.augmentations import Rotation, HorizontalFlip, VerticalFlip
-from lightningdata.thirdparty.torchmeta.transforms.splitters import Splitter, ClassSplitter, WeightedClassSplitter
-from lightningdata.thirdparty.torchmeta.transforms.target_transforms import TargetTransform, DefaultTargetTransform, SegmentationPairTransform
-from lightningdata.thirdparty.torchmeta.transforms.tabular_transforms import NumpyToTorch
+from lightningdata.thirdparty.torchmeta.transforms.categorical import Categorical, FixedCategory
+from lightningdata.thirdparty.torchmeta.transforms.augmentations import Rotation, HorizontalFlip, VerticalFlip
+from lightningdata.thirdparty.torchmeta.transforms.splitters import Splitter, ClassSplitter, WeightedClassSplitter
+from lightningdata.thirdparty.torchmeta.transforms.target_transforms import TargetTransform, DefaultTargetTransform, SegmentationPairTransform
+from lightningdata.thirdparty.torchmeta.transforms.tabular_transforms import NumpyToTorch
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/augmentations.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/augmentations.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import torchvision.transforms.functional as F
-
-class Rotation(object):
-    def __init__(self, angle, resample=False, expand=False, center=None):
-        super(Rotation, self).__init__()
-        if isinstance(angle, (list, tuple)):
-            self._angles = angle
-            self.angle = None
-        else:
-            self._angles = [angle]
-            self.angle = angle
-            if angle % 360 == 0:
-                import warnings
-                warnings.warn('Applying a rotation of {0} degrees (`{1}`) as a '
-                    'class augmentation on a dataset is equivalent to the original '
-                    'dataset.'.format(angle, self), UserWarning, stacklevel=2)
-
-        self.resample = resample
-        self.expand = expand
-        self.center = center
-
-    def __iter__(self):
-        return iter(Rotation(angle, resample=self.resample, expand=self.expand,
-            center=self.center) for angle in self._angles)
-
-    def __call__(self, image):
-        if self.angle is None:
-            raise ValueError('The value of the angle is unspecified.')
-        # QKFIX: Explicitly compute the pixel fill value due to an
-        # incompatibility between Torchvision 0.5 and Pillow 7.0.0
-        # https://github.com/pytorch/vision/issues/1759#issuecomment-583826810
-        # Will be fixed in Torchvision 0.6
-        fill = tuple([0] * len(image.getbands()))
-        return F.rotate(image, self.angle % 360, self.resample,
-                        self.expand, self.center, fill=fill)
-
-    def __hash__(self):
-        return hash(repr(self))
-
-    def __eq__(self, other):
-        if (self.angle is None) or (other.angle is None):
-            return self._angles == other._angles
-        return (self.angle % 360) == (other.angle % 360)
-
-    def __repr__(self):
-        if self.angle is None:
-            return 'Rotation({0})'.format(', '.join(map(str, self._angles)))
-        else:
-            return 'Rotation({0})'.format(self.angle % 360)
-
-    def __str__(self):
-        if self.angle is None:
-            return 'Rotation({0})'.format(', '.join(map(str, self._angles)))
-        else:
-            return 'Rotation({0})'.format(self.angle)
-
-class HorizontalFlip(object):
-    def __iter__(self):
-        return iter([HorizontalFlip()])
-
-    def __call__(self, image):
-        return F.hflip(image)
-
-    def __repr__(self):
-        return 'HorizontalFlip()'
-
-class VerticalFlip(object):
-    def __iter__(self):
-        return iter([VerticalFlip()])
-
-    def __call__(self, image):
-        return F.vflip(image)
-
-    def __repr__(self):
-        return 'VerticalFlip()'
+import torchvision.transforms.functional as F
+
+class Rotation(object):
+    def __init__(self, angle, resample=False, expand=False, center=None):
+        super(Rotation, self).__init__()
+        if isinstance(angle, (list, tuple)):
+            self._angles = angle
+            self.angle = None
+        else:
+            self._angles = [angle]
+            self.angle = angle
+            if angle % 360 == 0:
+                import warnings
+                warnings.warn('Applying a rotation of {0} degrees (`{1}`) as a '
+                    'class augmentation on a dataset is equivalent to the original '
+                    'dataset.'.format(angle, self), UserWarning, stacklevel=2)
+
+        self.resample = resample
+        self.expand = expand
+        self.center = center
+
+    def __iter__(self):
+        return iter(Rotation(angle, resample=self.resample, expand=self.expand,
+            center=self.center) for angle in self._angles)
+
+    def __call__(self, image):
+        if self.angle is None:
+            raise ValueError('The value of the angle is unspecified.')
+        # QKFIX: Explicitly compute the pixel fill value due to an
+        # incompatibility between Torchvision 0.5 and Pillow 7.0.0
+        # https://github.com/pytorch/vision/issues/1759#issuecomment-583826810
+        # Will be fixed in Torchvision 0.6
+        fill = tuple([0] * len(image.getbands()))
+        return F.rotate(image, self.angle % 360, self.resample,
+                        self.expand, self.center, fill=fill)
+
+    def __hash__(self):
+        return hash(repr(self))
+
+    def __eq__(self, other):
+        if (self.angle is None) or (other.angle is None):
+            return self._angles == other._angles
+        return (self.angle % 360) == (other.angle % 360)
+
+    def __repr__(self):
+        if self.angle is None:
+            return 'Rotation({0})'.format(', '.join(map(str, self._angles)))
+        else:
+            return 'Rotation({0})'.format(self.angle % 360)
+
+    def __str__(self):
+        if self.angle is None:
+            return 'Rotation({0})'.format(', '.join(map(str, self._angles)))
+        else:
+            return 'Rotation({0})'.format(self.angle)
+
+class HorizontalFlip(object):
+    def __iter__(self):
+        return iter([HorizontalFlip()])
+
+    def __call__(self, image):
+        return F.hflip(image)
+
+    def __repr__(self):
+        return 'HorizontalFlip()'
+
+class VerticalFlip(object):
+    def __iter__(self):
+        return iter([VerticalFlip()])
+
+    def __call__(self, image):
+        return F.vflip(image)
+
+    def __repr__(self):
+        return 'VerticalFlip()'
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/transforms/categorical.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/transforms/categorical.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import torch
-from lightningdata.thirdparty.torchmeta.transforms.utils import apply_wrapper
-from collections import defaultdict
-
-from lightningdata.thirdparty.torchmeta.transforms.target_transforms import TargetTransform
-
-
-class Categorical(TargetTransform):
-    """Target transform to return labels in `[0, num_classes)`.
-
-    Parameters
-    ----------
-    num_classes : int, optional
-        Number of classes. If `None`, then the number of classes is inferred
-        from the number of individual labels encountered.
-
-    Examples
-    --------
-    >>> dataset = Omniglot('data', num_classes_per_task=5, meta_train=True)
-    >>> task = dataset.sample_task()
-    >>> task[0]
-    (<PIL.Image.Image image mode=L size=105x105 at 0x11EC797F0>,
-    ('images_evaluation/Glagolitic/character12', None))
-
-    >>> dataset = Omniglot('data', num_classes_per_task=5, meta_train=True,
-    ... target_transform=Categorical(5))
-    >>> task = dataset.sample_task()
-    >>> task[0]
-    (<PIL.Image.Image image mode=L size=105x105 at 0x11ED3F668>, 2)
-    """
-    def __init__(self, num_classes=None):
-        super(Categorical, self).__init__()
-        self.num_classes = num_classes
-        self._classes = None
-        self._labels = None
-
-    def reset(self):
-        self._classes = None
-        self._labels = None
-
-    @property
-    def classes(self):
-        if self._classes is None:
-            self._classes = defaultdict(None)
-            if self.num_classes is None:
-                default_factory = lambda: len(self._classes)
-            else:
-                default_factory = lambda: self.labels[len(self._classes)]
-            self._classes.default_factory = default_factory
-        if (self.num_classes is not None) and (len(self._classes) > self.num_classes):
-            raise ValueError('The number of individual labels ({0}) is greater '
-                'than the number of classes defined by `num_classes` '
-                '({1}).'.format(len(self._classes), self.num_classes))
-        return self._classes
-
-    @property
-    def labels(self):
-        if (self._labels is None) and (self.num_classes is not None):
-            # TODO: Replace torch.randperm with seed-friendly counterpart
-            self._labels = torch.randperm(self.num_classes).tolist()
-        return self._labels
-
-    def __call__(self, target):
-        return self.classes[target]
-
-    def __repr__(self):
-        return '{0}({1})'.format(self.__class__.__name__, self.num_classes or '')
-
-
-class FixedCategory(object):
-    def __init__(self, transform=None):
-        self.transform = transform
-
-    def __call__(self, index):
-        return (index, self.transform)
-
-    def __repr__(self):
-        return ('{0}({1})'.format(self.__class__.__name__, self.transform))
+import torch
+from lightningdata.thirdparty.torchmeta.transforms.utils import apply_wrapper
+from collections import defaultdict
+
+from lightningdata.thirdparty.torchmeta.transforms.target_transforms import TargetTransform
+
+
+class Categorical(TargetTransform):
+    """Target transform to return labels in `[0, num_classes)`.
+
+    Parameters
+    ----------
+    num_classes : int, optional
+        Number of classes. If `None`, then the number of classes is inferred
+        from the number of individual labels encountered.
+
+    Examples
+    --------
+    >>> dataset = Omniglot('data', num_classes_per_task=5, meta_train=True)
+    >>> task = dataset.sample_task()
+    >>> task[0]
+    (<PIL.Image.Image image mode=L size=105x105 at 0x11EC797F0>,
+    ('images_evaluation/Glagolitic/character12', None))
+
+    >>> dataset = Omniglot('data', num_classes_per_task=5, meta_train=True,
+    ... target_transform=Categorical(5))
+    >>> task = dataset.sample_task()
+    >>> task[0]
+    (<PIL.Image.Image image mode=L size=105x105 at 0x11ED3F668>, 2)
+    """
+    def __init__(self, num_classes=None):
+        super(Categorical, self).__init__()
+        self.num_classes = num_classes
+        self._classes = None
+        self._labels = None
+
+    def reset(self):
+        self._classes = None
+        self._labels = None
+
+    @property
+    def classes(self):
+        if self._classes is None:
+            self._classes = defaultdict(None)
+            if self.num_classes is None:
+                default_factory = lambda: len(self._classes)
+            else:
+                default_factory = lambda: self.labels[len(self._classes)]
+            self._classes.default_factory = default_factory
+        if (self.num_classes is not None) and (len(self._classes) > self.num_classes):
+            raise ValueError('The number of individual labels ({0}) is greater '
+                'than the number of classes defined by `num_classes` '
+                '({1}).'.format(len(self._classes), self.num_classes))
+        return self._classes
+
+    @property
+    def labels(self):
+        if (self._labels is None) and (self.num_classes is not None):
+            # TODO: Replace torch.randperm with seed-friendly counterpart
+            self._labels = torch.randperm(self.num_classes).tolist()
+        return self._labels
+
+    def __call__(self, target):
+        return self.classes[target]
+
+    def __repr__(self):
+        return '{0}({1})'.format(self.__class__.__name__, self.num_classes or '')
+
+
+class FixedCategory(object):
+    def __init__(self, transform=None):
+        self.transform = transform
+
+    def __call__(self, index):
+        return (index, self.transform)
+
+    def __repr__(self):
+        return ('{0}({1})'.format(self.__class__.__name__, self.transform))
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from lightningdata.thirdparty.torchmeta.utils import data
-from lightningdata.thirdparty.torchmeta.utils.gradient_based import gradient_update_parameters
-from lightningdata.thirdparty.torchmeta.utils.metrics import hardness_metric
-from lightningdata.thirdparty.torchmeta.utils.prototype import get_num_samples, get_prototypes, prototypical_loss
-from lightningdata.thirdparty.torchmeta.utils.matching import pairwise_cosine_similarity, matching_log_probas, matching_probas, matching_loss
-from lightningdata.thirdparty.torchmeta.utils.r2d2 import ridge_regression
-
-__all__ = [
-    'data',
-    'gradient_update_parameters',
-    'hardness_metric',
-    'get_num_samples',
-    'get_prototypes',
-    'prototypical_loss',
-    'pairwise_cosine_similarity',
-    'matching_log_probas',
-    'matching_probas',
-    'matching_loss',
-    'ridge_regression'
-]
+from lightningdata.thirdparty.torchmeta.utils import data
+from lightningdata.thirdparty.torchmeta.utils.gradient_based import gradient_update_parameters
+from lightningdata.thirdparty.torchmeta.utils.metrics import hardness_metric
+from lightningdata.thirdparty.torchmeta.utils.prototype import get_num_samples, get_prototypes, prototypical_loss
+from lightningdata.thirdparty.torchmeta.utils.matching import pairwise_cosine_similarity, matching_log_probas, matching_probas, matching_loss
+from lightningdata.thirdparty.torchmeta.utils.r2d2 import ridge_regression
+
+__all__ = [
+    'data',
+    'gradient_update_parameters',
+    'hardness_metric',
+    'get_num_samples',
+    'get_prototypes',
+    'prototypical_loss',
+    'pairwise_cosine_similarity',
+    'matching_log_probas',
+    'matching_probas',
+    'matching_loss',
+    'ridge_regression'
+]
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/__init__.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from lightningdata.thirdparty.torchmeta.utils.data.dataloader import MetaDataLoader, BatchMetaDataLoader
-from lightningdata.thirdparty.torchmeta.utils.data.dataset import ClassDataset, MetaDataset, CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.utils.data.sampler import CombinationSequentialSampler, CombinationRandomSampler
-from lightningdata.thirdparty.torchmeta.utils.data.task import Dataset, Task, ConcatTask, SubsetTask
-from lightningdata.thirdparty.torchmeta.utils.data.wrappers import NonEpisodicWrapper
-
-__all__ = [
-    'MetaDataLoader',
-    'BatchMetaDataLoader',
-    'ClassDataset',
-    'MetaDataset',
-    'CombinationMetaDataset',
-    'CombinationSequentialSampler',
-    'CombinationRandomSampler',
-    'Dataset',
-    'Task',
-    'ConcatTask',
-    'SubsetTask',
-    'NonEpisodicWrapper'
-]
+from lightningdata.thirdparty.torchmeta.utils.data.dataloader import MetaDataLoader, BatchMetaDataLoader
+from lightningdata.thirdparty.torchmeta.utils.data.dataset import ClassDataset, MetaDataset, CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.utils.data.sampler import CombinationSequentialSampler, CombinationRandomSampler
+from lightningdata.thirdparty.torchmeta.utils.data.task import Dataset, Task, ConcatTask, SubsetTask
+from lightningdata.thirdparty.torchmeta.utils.data.wrappers import NonEpisodicWrapper
+
+__all__ = [
+    'MetaDataLoader',
+    'BatchMetaDataLoader',
+    'ClassDataset',
+    'MetaDataset',
+    'CombinationMetaDataset',
+    'CombinationSequentialSampler',
+    'CombinationRandomSampler',
+    'Dataset',
+    'Task',
+    'ConcatTask',
+    'SubsetTask',
+    'NonEpisodicWrapper'
+]
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from collections import OrderedDict
-
-from torch.utils.data import DataLoader
-from torch.utils.data.dataloader import default_collate
-from torch.utils.data.dataset import Dataset as TorchDataset
-
-from lightningdata.thirdparty.torchmeta.utils.data.dataset import CombinationMetaDataset
-from lightningdata.thirdparty.torchmeta.utils.data.sampler import (CombinationSequentialSampler,
-                                          CombinationRandomSampler)
-
-class BatchMetaCollate(object):
-
-    def __init__(self, collate_fn):
-        super().__init__()
-        self.collate_fn = collate_fn
-
-    def collate_task(self, task):
-        if isinstance(task, TorchDataset):
-            return self.collate_fn([task[idx] for idx in range(len(task))])
-        elif isinstance(task, OrderedDict):
-            return OrderedDict([(key, self.collate_task(subtask))
-                for (key, subtask) in task.items()])
-        else:
-            raise NotImplementedError()
-
-    def __call__(self, batch):
-        return self.collate_fn([self.collate_task(task) for task in batch])
-
-def no_collate(batch):
-    return batch
-
-class MetaDataLoader(DataLoader):
-    def __init__(self, dataset, batch_size=1, shuffle=True, sampler=None,
-                 batch_sampler=None, num_workers=0, collate_fn=None,
-                 pin_memory=False, drop_last=False, timeout=0,
-                 worker_init_fn=None):
-        if collate_fn is None:
-            collate_fn = no_collate
-
-        if isinstance(dataset, CombinationMetaDataset) and (sampler is None):
-            if shuffle:
-                sampler = CombinationRandomSampler(dataset)
-            else:
-                sampler = CombinationSequentialSampler(dataset)
-            shuffle = False
-
-        super(MetaDataLoader, self).__init__(dataset, batch_size=batch_size,
-            shuffle=shuffle, sampler=sampler, batch_sampler=batch_sampler,
-            num_workers=num_workers, collate_fn=collate_fn,
-            pin_memory=pin_memory, drop_last=drop_last, timeout=timeout,
-            worker_init_fn=worker_init_fn)
-
-
-class BatchMetaDataLoader(MetaDataLoader):
-    def __init__(self, dataset, batch_size=1, shuffle=True, sampler=None, num_workers=0,
-                 pin_memory=False, drop_last=False, timeout=0, worker_init_fn=None):
-        collate_fn = BatchMetaCollate(default_collate)
-
-        super(BatchMetaDataLoader, self).__init__(dataset,
-            batch_size=batch_size, shuffle=shuffle, sampler=sampler,
-            batch_sampler=None, num_workers=num_workers,
-            collate_fn=collate_fn, pin_memory=pin_memory, drop_last=drop_last,
-            timeout=timeout, worker_init_fn=worker_init_fn)
+from collections import OrderedDict
+
+from torch.utils.data import DataLoader
+from torch.utils.data.dataloader import default_collate
+from torch.utils.data.dataset import Dataset as TorchDataset
+
+from lightningdata.thirdparty.torchmeta.utils.data.dataset import CombinationMetaDataset
+from lightningdata.thirdparty.torchmeta.utils.data.sampler import (CombinationSequentialSampler,
+                                          CombinationRandomSampler)
+
+class BatchMetaCollate(object):
+
+    def __init__(self, collate_fn):
+        super().__init__()
+        self.collate_fn = collate_fn
+
+    def collate_task(self, task):
+        if isinstance(task, TorchDataset):
+            return self.collate_fn([task[idx] for idx in range(len(task))])
+        elif isinstance(task, OrderedDict):
+            return OrderedDict([(key, self.collate_task(subtask))
+                for (key, subtask) in task.items()])
+        else:
+            raise NotImplementedError()
+
+    def __call__(self, batch):
+        return self.collate_fn([self.collate_task(task) for task in batch])
+
+def no_collate(batch):
+    return batch
+
+class MetaDataLoader(DataLoader):
+    def __init__(self, dataset, batch_size=1, shuffle=True, sampler=None,
+                 batch_sampler=None, num_workers=0, collate_fn=None,
+                 pin_memory=False, drop_last=False, timeout=0,
+                 worker_init_fn=None):
+        if collate_fn is None:
+            collate_fn = no_collate
+
+        if isinstance(dataset, CombinationMetaDataset) and (sampler is None):
+            if shuffle:
+                sampler = CombinationRandomSampler(dataset)
+            else:
+                sampler = CombinationSequentialSampler(dataset)
+            shuffle = False
+
+        super(MetaDataLoader, self).__init__(dataset, batch_size=batch_size,
+            shuffle=shuffle, sampler=sampler, batch_sampler=batch_sampler,
+            num_workers=num_workers, collate_fn=collate_fn,
+            pin_memory=pin_memory, drop_last=drop_last, timeout=timeout,
+            worker_init_fn=worker_init_fn)
+
+
+class BatchMetaDataLoader(MetaDataLoader):
+    def __init__(self, dataset, batch_size=1, shuffle=True, sampler=None, num_workers=0,
+                 pin_memory=False, drop_last=False, timeout=0, worker_init_fn=None):
+        collate_fn = BatchMetaCollate(default_collate)
+
+        super(BatchMetaDataLoader, self).__init__(dataset,
+            batch_size=batch_size, shuffle=shuffle, sampler=sampler,
+            batch_sampler=None, num_workers=num_workers,
+            collate_fn=collate_fn, pin_memory=pin_memory, drop_last=drop_last,
+            timeout=timeout, worker_init_fn=worker_init_fn)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/dataset.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/dataset.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,321 +1,321 @@
-import sys
-import numpy as np
-import warnings
-from copy import deepcopy
-
-from itertools import combinations
-from ordered_set import OrderedSet
-
-from torchvision.transforms import Compose
-
-from lightningdata.thirdparty.torchmeta.utils.data.task import ConcatTask
-from lightningdata.thirdparty.torchmeta.transforms import FixedCategory, Categorical, DefaultTargetTransform
-from lightningdata.thirdparty.torchmeta.transforms.utils import wrap_transform
-
-__all__ = ['ClassDataset', 'MetaDataset', 'CombinationMetaDataset']
-
-
-class ClassDataset(object):
-    """Base class for a dataset of classes. Each item from a `ClassDataset` is 
-    a dataset containing examples from the same class.
-
-    Parameters
-    ----------
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test`.
-
-    class_augmentations : list of callable, optional
-        A list of functions that augment the dataset with new classes. These classes 
-        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
-    """
-    def __init__(self, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, class_augmentations=None):
-        if meta_train + meta_val + meta_test == 0:
-            if meta_split is None:
-                raise ValueError('The meta-split is undefined. Use either the '
-                    'argument `meta_train=True` (or `meta_val`/`meta_test`), or '
-                    'the argument `meta_split="train"` (or "val"/"test").')
-            elif meta_split not in ['train', 'val', 'test']:
-                raise ValueError('Unknown meta-split name `{0}`. The meta-split '
-                    'must be in [`train`, `val`, `test`].'.format(meta_split))
-            meta_train = (meta_split == 'train')
-            meta_val = (meta_split == 'val')
-            meta_test = (meta_split == 'test')
-        elif meta_train + meta_val + meta_test > 1:
-            raise ValueError('Multiple arguments among `meta_train`, `meta_val` '
-                'and `meta_test` are set to `True`. Exactly one must be set to '
-                '`True`.')
-        self.meta_train = meta_train
-        self.meta_val = meta_val
-        self.meta_test = meta_test
-        self._meta_split = meta_split
-
-        if class_augmentations is not None:
-            if not isinstance(class_augmentations, list):
-                raise TypeError('Unknown type for `class_augmentations`. '
-                    'Expected `list`, got `{0}`.'.format(type(class_augmentations)))
-            unique_augmentations = OrderedSet()
-            for augmentations in class_augmentations:
-                for transform in augmentations:
-                    if transform in unique_augmentations:
-                        warnings.warn('The class augmentation `{0}` already '
-                            'exists in the list of class augmentations (`{1}`). '
-                            'To avoid any duplicate, this transformation is '
-                            'ignored.'.format(transform, repr(transform)),
-                            UserWarning, stacklevel=2)
-                    unique_augmentations.add(transform)
-            class_augmentations = list(unique_augmentations)
-        else:
-            class_augmentations = []
-        self.class_augmentations = class_augmentations
-
-    def get_class_augmentation(self, index):
-        transform_index = (index // self.num_classes) - 1
-        if transform_index < 0:
-            return None
-        return self.class_augmentations[transform_index]
-
-    def get_transform(self, index, transform=None):
-        class_transform = self.get_class_augmentation(index)
-        if class_transform is None:
-            return transform
-        if transform is None:
-            return class_transform
-        return Compose([class_transform, transform])
-
-    def get_target_transform(self, index):
-        class_transform = self.get_class_augmentation(index)
-        return FixedCategory(class_transform)
-
-    @property
-    def meta_split(self):
-        if self._meta_split is None:
-            if self.meta_train:
-                self._meta_split = 'train'
-            elif self.meta_val:
-                self._meta_split = 'val'
-            elif self.meta_test:
-                self._meta_split = 'test'
-            else:
-                raise NotImplementedError()
-        return self._meta_split
-
-    def __getitem__(self, index):
-        raise NotImplementedError()
-
-    @property
-    def num_classes(self):
-        raise NotImplementedError()
-
-    def __len__(self):
-        return self.num_classes * (len(self.class_augmentations) + 1)
-
-
-class MetaDataset(object):
-    """Base class for a meta-dataset.
-
-    Parameters
-    ----------
-    meta_train : bool (default: `False`)
-        Use the meta-train split of the dataset. If set to `True`, then the
-        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_val : bool (default: `False`)
-        Use the meta-validation split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_test : bool (default: `False`)
-        Use the meta-test split of the dataset. If set to `True`, then the 
-        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
-        of these three arguments must be set to `True`.
-
-    meta_split : string in {'train', 'val', 'test'}, optional
-        Name of the split to use. This overrides the arguments `meta_train`, 
-        `meta_val` and `meta_test`.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `transforms.ClassSplitter()`.
-    """
-    def __init__(self, meta_train=False, meta_val=False, meta_test=False,
-                 meta_split=None, target_transform=None, dataset_transform=None):
-        if meta_train + meta_val + meta_test == 0:
-            if meta_split is None:
-                raise ValueError('The meta-split is undefined. Use either the '
-                    'argument `meta_train=True` (or `meta_val`/`meta_test`), or '
-                    'the argument `meta_split="train"` (or "val"/"test").')
-            elif meta_split not in ['train', 'val', 'test']:
-                raise ValueError('Unknown meta-split name `{0}`. The meta-split '
-                    'must be in [`train`, `val`, `test`].'.format(meta_split))
-            meta_train = (meta_split == 'train')
-            meta_val = (meta_split == 'val')
-            meta_test = (meta_split == 'test')
-        elif meta_train + meta_val + meta_test > 1:
-            raise ValueError('Multiple arguments among `meta_train`, `meta_val` '
-                'and `meta_test` are set to `True`. Exactly one must be set to '
-                '`True`.')
-        self.meta_train = meta_train
-        self.meta_val = meta_val
-        self.meta_test = meta_test
-        self._meta_split = meta_split
-        self.target_transform = target_transform
-        self.dataset_transform = dataset_transform
-        self.seed()
-
-    @property
-    def meta_split(self):
-        if self._meta_split is None:
-            if self.meta_train:
-                self._meta_split = 'train'
-            elif self.meta_val:
-                self._meta_split = 'val'
-            elif self.meta_test:
-                self._meta_split = 'test'
-            else:
-                raise NotImplementedError()
-        return self._meta_split
-
-    def seed(self, seed=None):
-        self.np_random = np.random.RandomState(seed=seed)
-        # Seed the dataset transform
-        _seed_dataset_transform(self.dataset_transform, seed=seed)
-
-    def __iter__(self):
-        for index in range(len(self)):
-            yield self[index]
-
-    def sample_task(self):
-        index = self.np_random.randint(len(self))
-        return self[index]
-
-    def __getitem__(self, index):
-        raise NotImplementedError()
-
-    def __len__(self):
-        raise NotImplementedError()
-
-
-class CombinationMetaDataset(MetaDataset):
-    """Base class for a meta-dataset, where the classification tasks are over 
-    multiple classes from a `ClassDataset`.
-
-    Parameters
-    ----------
-    dataset : `ClassDataset` instance
-        A dataset of classes. Each item of `dataset` is a dataset, containing 
-        all the examples from the same class.
-
-    num_classes_per_task : int
-        Number of classes per tasks. This corresponds to `N` in `N-way` 
-        classification.
-
-    target_transform : callable, optional
-        A function/transform that takes a target, and returns a transformed 
-        version. See also `torchvision.transforms`.
-
-    dataset_transform : callable, optional
-        A function/transform that takes a dataset (ie. a task), and returns a 
-        transformed version of it. E.g. `transforms.ClassSplitter()`.
-    """
-    def __init__(self, dataset, num_classes_per_task, target_transform=None,
-                 dataset_transform=None):
-        if not isinstance(num_classes_per_task, int):
-            raise TypeError('Unknown type for `num_classes_per_task`. Expected '
-                '`int`, got `{0}`.'.format(type(num_classes_per_task)))
-        self.dataset = dataset
-        self.num_classes_per_task = num_classes_per_task
-        # If no target_transform, then use a default target transform that
-        # is well behaved for the `default_collate` function (assign class
-        # augmentations ot integers).
-        if target_transform is None:
-            target_transform = DefaultTargetTransform(dataset.class_augmentations)
-
-        super(CombinationMetaDataset, self).__init__(meta_train=dataset.meta_train,
-            meta_val=dataset.meta_val, meta_test=dataset.meta_test,
-            meta_split=dataset.meta_split, target_transform=target_transform,
-            dataset_transform=dataset_transform)
-
-    def __iter__(self):
-        num_classes = len(self.dataset)
-        for index in combinations(num_classes, self.num_classes_per_task):
-            yield self[index]
-
-    def sample_task(self):
-        index = self.np_random.choice(len(self.dataset),
-            size=self.num_classes_per_task, replace=False)
-        return self[tuple(index)]
-
-    def __getitem__(self, index):
-        if isinstance(index, int):
-            raise ValueError('The index of a `CombinationMetaDataset` must be '
-                'a tuple of integers, and not an integer. For example, call '
-                '`dataset[({0})]` to get a task with classes from 0 to {1} '
-                '(got `{2}`).'.format(', '.join([str(idx)
-                for idx in range(self.num_classes_per_task)]),
-                self.num_classes_per_task - 1, index))
-        assert len(index) == self.num_classes_per_task
-        datasets = [self.dataset[i] for i in index]
-        # Use deepcopy on `Categorical` target transforms, to avoid any side
-        # effect across tasks.
-        task = ConcatTask(datasets, self.num_classes_per_task,
-            target_transform=wrap_transform(self.target_transform,
-            self._copy_categorical, transform_type=Categorical))
-
-        if self.dataset_transform is not None:
-            task = self.dataset_transform(task)
-
-        return task
-
-    def _copy_categorical(self, transform):
-        assert isinstance(transform, Categorical)
-        transform.reset()
-        if transform.num_classes is None:
-            transform.num_classes = self.num_classes_per_task
-        return deepcopy(transform)
-
-    def __len__(self):
-        num_classes, length = len(self.dataset), 1
-        for i in range(1, self.num_classes_per_task + 1):
-            length *= (num_classes - i + 1) / i
-
-        if length > sys.maxsize:
-            warnings.warn('The number of possible tasks in {0} is '
-                'combinatorially large (equal to C({1}, {2})), and exceeds '
-                'machine precision. Setting the length of the dataset to the '
-                'maximum integer value, which undervalues the actual number of '
-                'possible tasks in the dataset. Therefore the value returned by '
-                '`len(dataset)` should not be trusted as being representative '
-                'of the true number of tasks.'.format(self, len(self.dataset),
-                self.num_classes_per_task), UserWarning, stacklevel=2)
-            length = sys.maxsize
-        return int(length)
-
-
-def _seed_dataset_transform(transform, seed=None):
-    if isinstance(transform, Compose):
-        for subtransform in transform.transforms:
-            _seed_dataset_transform(subtransform, seed=seed)
-    elif hasattr(transform, 'seed'):
-        transform.seed(seed=seed)
+import sys
+import numpy as np
+import warnings
+from copy import deepcopy
+
+from itertools import combinations
+from ordered_set import OrderedSet
+
+from torchvision.transforms import Compose
+
+from lightningdata.thirdparty.torchmeta.utils.data.task import ConcatTask
+from lightningdata.thirdparty.torchmeta.transforms import FixedCategory, Categorical, DefaultTargetTransform
+from lightningdata.thirdparty.torchmeta.transforms.utils import wrap_transform
+
+__all__ = ['ClassDataset', 'MetaDataset', 'CombinationMetaDataset']
+
+
+class ClassDataset(object):
+    """Base class for a dataset of classes. Each item from a `ClassDataset` is 
+    a dataset containing examples from the same class.
+
+    Parameters
+    ----------
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test`.
+
+    class_augmentations : list of callable, optional
+        A list of functions that augment the dataset with new classes. These classes 
+        are transformations of existing classes. E.g. `transforms.HorizontalFlip()`.
+    """
+    def __init__(self, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, class_augmentations=None):
+        if meta_train + meta_val + meta_test == 0:
+            if meta_split is None:
+                raise ValueError('The meta-split is undefined. Use either the '
+                    'argument `meta_train=True` (or `meta_val`/`meta_test`), or '
+                    'the argument `meta_split="train"` (or "val"/"test").')
+            elif meta_split not in ['train', 'val', 'test']:
+                raise ValueError('Unknown meta-split name `{0}`. The meta-split '
+                    'must be in [`train`, `val`, `test`].'.format(meta_split))
+            meta_train = (meta_split == 'train')
+            meta_val = (meta_split == 'val')
+            meta_test = (meta_split == 'test')
+        elif meta_train + meta_val + meta_test > 1:
+            raise ValueError('Multiple arguments among `meta_train`, `meta_val` '
+                'and `meta_test` are set to `True`. Exactly one must be set to '
+                '`True`.')
+        self.meta_train = meta_train
+        self.meta_val = meta_val
+        self.meta_test = meta_test
+        self._meta_split = meta_split
+
+        if class_augmentations is not None:
+            if not isinstance(class_augmentations, list):
+                raise TypeError('Unknown type for `class_augmentations`. '
+                    'Expected `list`, got `{0}`.'.format(type(class_augmentations)))
+            unique_augmentations = OrderedSet()
+            for augmentations in class_augmentations:
+                for transform in augmentations:
+                    if transform in unique_augmentations:
+                        warnings.warn('The class augmentation `{0}` already '
+                            'exists in the list of class augmentations (`{1}`). '
+                            'To avoid any duplicate, this transformation is '
+                            'ignored.'.format(transform, repr(transform)),
+                            UserWarning, stacklevel=2)
+                    unique_augmentations.add(transform)
+            class_augmentations = list(unique_augmentations)
+        else:
+            class_augmentations = []
+        self.class_augmentations = class_augmentations
+
+    def get_class_augmentation(self, index):
+        transform_index = (index // self.num_classes) - 1
+        if transform_index < 0:
+            return None
+        return self.class_augmentations[transform_index]
+
+    def get_transform(self, index, transform=None):
+        class_transform = self.get_class_augmentation(index)
+        if class_transform is None:
+            return transform
+        if transform is None:
+            return class_transform
+        return Compose([class_transform, transform])
+
+    def get_target_transform(self, index):
+        class_transform = self.get_class_augmentation(index)
+        return FixedCategory(class_transform)
+
+    @property
+    def meta_split(self):
+        if self._meta_split is None:
+            if self.meta_train:
+                self._meta_split = 'train'
+            elif self.meta_val:
+                self._meta_split = 'val'
+            elif self.meta_test:
+                self._meta_split = 'test'
+            else:
+                raise NotImplementedError()
+        return self._meta_split
+
+    def __getitem__(self, index):
+        raise NotImplementedError()
+
+    @property
+    def num_classes(self):
+        raise NotImplementedError()
+
+    def __len__(self):
+        return self.num_classes * (len(self.class_augmentations) + 1)
+
+
+class MetaDataset(object):
+    """Base class for a meta-dataset.
+
+    Parameters
+    ----------
+    meta_train : bool (default: `False`)
+        Use the meta-train split of the dataset. If set to `True`, then the
+        arguments `meta_val` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_val : bool (default: `False`)
+        Use the meta-validation split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_test` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_test : bool (default: `False`)
+        Use the meta-test split of the dataset. If set to `True`, then the 
+        arguments `meta_train` and `meta_val` must be set to `False`. Exactly one 
+        of these three arguments must be set to `True`.
+
+    meta_split : string in {'train', 'val', 'test'}, optional
+        Name of the split to use. This overrides the arguments `meta_train`, 
+        `meta_val` and `meta_test`.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `transforms.ClassSplitter()`.
+    """
+    def __init__(self, meta_train=False, meta_val=False, meta_test=False,
+                 meta_split=None, target_transform=None, dataset_transform=None):
+        if meta_train + meta_val + meta_test == 0:
+            if meta_split is None:
+                raise ValueError('The meta-split is undefined. Use either the '
+                    'argument `meta_train=True` (or `meta_val`/`meta_test`), or '
+                    'the argument `meta_split="train"` (or "val"/"test").')
+            elif meta_split not in ['train', 'val', 'test']:
+                raise ValueError('Unknown meta-split name `{0}`. The meta-split '
+                    'must be in [`train`, `val`, `test`].'.format(meta_split))
+            meta_train = (meta_split == 'train')
+            meta_val = (meta_split == 'val')
+            meta_test = (meta_split == 'test')
+        elif meta_train + meta_val + meta_test > 1:
+            raise ValueError('Multiple arguments among `meta_train`, `meta_val` '
+                'and `meta_test` are set to `True`. Exactly one must be set to '
+                '`True`.')
+        self.meta_train = meta_train
+        self.meta_val = meta_val
+        self.meta_test = meta_test
+        self._meta_split = meta_split
+        self.target_transform = target_transform
+        self.dataset_transform = dataset_transform
+        self.seed()
+
+    @property
+    def meta_split(self):
+        if self._meta_split is None:
+            if self.meta_train:
+                self._meta_split = 'train'
+            elif self.meta_val:
+                self._meta_split = 'val'
+            elif self.meta_test:
+                self._meta_split = 'test'
+            else:
+                raise NotImplementedError()
+        return self._meta_split
+
+    def seed(self, seed=None):
+        self.np_random = np.random.RandomState(seed=seed)
+        # Seed the dataset transform
+        _seed_dataset_transform(self.dataset_transform, seed=seed)
+
+    def __iter__(self):
+        for index in range(len(self)):
+            yield self[index]
+
+    def sample_task(self):
+        index = self.np_random.randint(len(self))
+        return self[index]
+
+    def __getitem__(self, index):
+        raise NotImplementedError()
+
+    def __len__(self):
+        raise NotImplementedError()
+
+
+class CombinationMetaDataset(MetaDataset):
+    """Base class for a meta-dataset, where the classification tasks are over 
+    multiple classes from a `ClassDataset`.
+
+    Parameters
+    ----------
+    dataset : `ClassDataset` instance
+        A dataset of classes. Each item of `dataset` is a dataset, containing 
+        all the examples from the same class.
+
+    num_classes_per_task : int
+        Number of classes per tasks. This corresponds to `N` in `N-way` 
+        classification.
+
+    target_transform : callable, optional
+        A function/transform that takes a target, and returns a transformed 
+        version. See also `torchvision.transforms`.
+
+    dataset_transform : callable, optional
+        A function/transform that takes a dataset (ie. a task), and returns a 
+        transformed version of it. E.g. `transforms.ClassSplitter()`.
+    """
+    def __init__(self, dataset, num_classes_per_task, target_transform=None,
+                 dataset_transform=None):
+        if not isinstance(num_classes_per_task, int):
+            raise TypeError('Unknown type for `num_classes_per_task`. Expected '
+                '`int`, got `{0}`.'.format(type(num_classes_per_task)))
+        self.dataset = dataset
+        self.num_classes_per_task = num_classes_per_task
+        # If no target_transform, then use a default target transform that
+        # is well behaved for the `default_collate` function (assign class
+        # augmentations ot integers).
+        if target_transform is None:
+            target_transform = DefaultTargetTransform(dataset.class_augmentations)
+
+        super(CombinationMetaDataset, self).__init__(meta_train=dataset.meta_train,
+            meta_val=dataset.meta_val, meta_test=dataset.meta_test,
+            meta_split=dataset.meta_split, target_transform=target_transform,
+            dataset_transform=dataset_transform)
+
+    def __iter__(self):
+        num_classes = len(self.dataset)
+        for index in combinations(num_classes, self.num_classes_per_task):
+            yield self[index]
+
+    def sample_task(self):
+        index = self.np_random.choice(len(self.dataset),
+            size=self.num_classes_per_task, replace=False)
+        return self[tuple(index)]
+
+    def __getitem__(self, index):
+        if isinstance(index, int):
+            raise ValueError('The index of a `CombinationMetaDataset` must be '
+                'a tuple of integers, and not an integer. For example, call '
+                '`dataset[({0})]` to get a task with classes from 0 to {1} '
+                '(got `{2}`).'.format(', '.join([str(idx)
+                for idx in range(self.num_classes_per_task)]),
+                self.num_classes_per_task - 1, index))
+        assert len(index) == self.num_classes_per_task
+        datasets = [self.dataset[i] for i in index]
+        # Use deepcopy on `Categorical` target transforms, to avoid any side
+        # effect across tasks.
+        task = ConcatTask(datasets, self.num_classes_per_task,
+            target_transform=wrap_transform(self.target_transform,
+            self._copy_categorical, transform_type=Categorical))
+
+        if self.dataset_transform is not None:
+            task = self.dataset_transform(task)
+
+        return task
+
+    def _copy_categorical(self, transform):
+        assert isinstance(transform, Categorical)
+        transform.reset()
+        if transform.num_classes is None:
+            transform.num_classes = self.num_classes_per_task
+        return deepcopy(transform)
+
+    def __len__(self):
+        num_classes, length = len(self.dataset), 1
+        for i in range(1, self.num_classes_per_task + 1):
+            length *= (num_classes - i + 1) / i
+
+        if length > sys.maxsize:
+            warnings.warn('The number of possible tasks in {0} is '
+                'combinatorially large (equal to C({1}, {2})), and exceeds '
+                'machine precision. Setting the length of the dataset to the '
+                'maximum integer value, which undervalues the actual number of '
+                'possible tasks in the dataset. Therefore the value returned by '
+                '`len(dataset)` should not be trusted as being representative '
+                'of the true number of tasks.'.format(self, len(self.dataset),
+                self.num_classes_per_task), UserWarning, stacklevel=2)
+            length = sys.maxsize
+        return int(length)
+
+
+def _seed_dataset_transform(transform, seed=None):
+    if isinstance(transform, Compose):
+        for subtransform in transform.transforms:
+            _seed_dataset_transform(subtransform, seed=seed)
+    elif hasattr(transform, 'seed'):
+        transform.seed(seed=seed)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/sampler.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/sampler.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import random
-import warnings
-from itertools import combinations
-from torch.utils.data.sampler import SequentialSampler, RandomSampler
-
-from lightningdata.thirdparty.torchmeta.utils.data.dataset import CombinationMetaDataset
-
-__all__ = ['CombinationSequentialSampler', 'CombinationRandomSampler']
-
-
-class CombinationSequentialSampler(SequentialSampler):
-    def __init__(self, data_source):
-        if not isinstance(data_source, CombinationMetaDataset):
-            raise TypeError('Expected `data_source` to be an instance of '
-                            '`CombinationMetaDataset`, but found '
-                            '{0}'.format(type(data_source)))
-        super(CombinationSequentialSampler, self).__init__(data_source)
-
-    def __iter__(self):
-        num_classes = len(self.data_source.dataset)
-        num_classes_per_task = self.data_source.num_classes_per_task
-        return combinations(range(num_classes), num_classes_per_task)
-
-
-class CombinationRandomSampler(RandomSampler):
-    def __init__(self, data_source):
-        if not isinstance(data_source, CombinationMetaDataset):
-            raise TypeError('Expected `data_source` to be an instance of '
-                            '`CombinationMetaDataset`, but found '
-                            '{0}'.format(type(data_source)))
-        # Temporarily disable the warning if the length of the length of the 
-        # dataset exceeds the machine precision. This avoids getting this
-        # warning shown with MetaDataLoader, even though MetaDataLoader itself
-        # does not use the length of the dataset.
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore')
-            super(CombinationRandomSampler, self).__init__(data_source,
-                                                           replacement=True)
-
-    def __iter__(self):
-        num_classes = len(self.data_source.dataset)
-        num_classes_per_task = self.data_source.num_classes_per_task
-        for _ in combinations(range(num_classes), num_classes_per_task):
-            yield tuple(random.sample(range(num_classes), num_classes_per_task))
+import random
+import warnings
+from itertools import combinations
+from torch.utils.data.sampler import SequentialSampler, RandomSampler
+
+from lightningdata.thirdparty.torchmeta.utils.data.dataset import CombinationMetaDataset
+
+__all__ = ['CombinationSequentialSampler', 'CombinationRandomSampler']
+
+
+class CombinationSequentialSampler(SequentialSampler):
+    def __init__(self, data_source):
+        if not isinstance(data_source, CombinationMetaDataset):
+            raise TypeError('Expected `data_source` to be an instance of '
+                            '`CombinationMetaDataset`, but found '
+                            '{0}'.format(type(data_source)))
+        super(CombinationSequentialSampler, self).__init__(data_source)
+
+    def __iter__(self):
+        num_classes = len(self.data_source.dataset)
+        num_classes_per_task = self.data_source.num_classes_per_task
+        return combinations(range(num_classes), num_classes_per_task)
+
+
+class CombinationRandomSampler(RandomSampler):
+    def __init__(self, data_source):
+        if not isinstance(data_source, CombinationMetaDataset):
+            raise TypeError('Expected `data_source` to be an instance of '
+                            '`CombinationMetaDataset`, but found '
+                            '{0}'.format(type(data_source)))
+        # Temporarily disable the warning if the length of the length of the 
+        # dataset exceeds the machine precision. This avoids getting this
+        # warning shown with MetaDataLoader, even though MetaDataLoader itself
+        # does not use the length of the dataset.
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            super(CombinationRandomSampler, self).__init__(data_source,
+                                                           replacement=True)
+
+    def __iter__(self):
+        num_classes = len(self.data_source.dataset)
+        num_classes_per_task = self.data_source.num_classes_per_task
+        for _ in combinations(range(num_classes), num_classes_per_task):
+            yield tuple(random.sample(range(num_classes), num_classes_per_task))
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/data/task.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/data/task.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from torch.utils.data import ConcatDataset, Subset
-from torch.utils.data import Dataset as Dataset_
-from torchvision.transforms import Compose
-
-__all__ = ['Dataset', 'Task', 'ConcatTask', 'SubsetTask']
-
-
-class Dataset(Dataset_):
-    def __init__(self, index, transform=None, target_transform=None):
-        self.index = index
-        self.transform = transform
-        self.target_transform = target_transform
-
-    def target_transform_append(self, transform):
-        if transform is None:
-            return
-        if self.target_transform is None:
-            self.target_transform = transform
-        else:
-            self.target_transform = Compose([self.target_transform, transform])
-
-    def __hash__(self):
-        return hash(self.index)
-
-
-class Task(Dataset):
-    """Base class for a classification task.
-
-    Parameters
-    ----------
-    num_classes : int
-        Number of classes for the classification task.
-    """
-    def __init__(self, index, num_classes,
-                 transform=None, target_transform=None):
-        super(Task, self).__init__(index, transform=transform,
-                                   target_transform=target_transform)
-        self.num_classes = num_classes
-
-
-class ConcatTask(Task, ConcatDataset):
-    def __init__(self, datasets, num_classes, target_transform=None):
-        index = tuple(task.index for task in datasets)
-        Task.__init__(self, index, num_classes)
-        ConcatDataset.__init__(self, datasets)
-        for task in self.datasets:
-            task.target_transform_append(target_transform)
-
-    def __getitem__(self, index):
-        return ConcatDataset.__getitem__(self, index)
-
-
-class SubsetTask(Task, Subset):
-    def __init__(self, dataset, indices, num_classes=None,
-                 target_transform=None):
-        if num_classes is None:
-            num_classes = dataset.num_classes
-        Task.__init__(self, dataset.index, num_classes)
-        Subset.__init__(self, dataset, indices)
-        self.dataset.target_transform_append(target_transform)
-
-    def __getitem__(self, index):
-        return Subset.__getitem__(self, index)
-
-    def __hash__(self):
-        return hash((self.index, tuple(self.indices)))
+from torch.utils.data import ConcatDataset, Subset
+from torch.utils.data import Dataset as Dataset_
+from torchvision.transforms import Compose
+
+__all__ = ['Dataset', 'Task', 'ConcatTask', 'SubsetTask']
+
+
+class Dataset(Dataset_):
+    def __init__(self, index, transform=None, target_transform=None):
+        self.index = index
+        self.transform = transform
+        self.target_transform = target_transform
+
+    def target_transform_append(self, transform):
+        if transform is None:
+            return
+        if self.target_transform is None:
+            self.target_transform = transform
+        else:
+            self.target_transform = Compose([self.target_transform, transform])
+
+    def __hash__(self):
+        return hash(self.index)
+
+
+class Task(Dataset):
+    """Base class for a classification task.
+
+    Parameters
+    ----------
+    num_classes : int
+        Number of classes for the classification task.
+    """
+    def __init__(self, index, num_classes,
+                 transform=None, target_transform=None):
+        super(Task, self).__init__(index, transform=transform,
+                                   target_transform=target_transform)
+        self.num_classes = num_classes
+
+
+class ConcatTask(Task, ConcatDataset):
+    def __init__(self, datasets, num_classes, target_transform=None):
+        index = tuple(task.index for task in datasets)
+        Task.__init__(self, index, num_classes)
+        ConcatDataset.__init__(self, datasets)
+        for task in self.datasets:
+            task.target_transform_append(target_transform)
+
+    def __getitem__(self, index):
+        return ConcatDataset.__getitem__(self, index)
+
+
+class SubsetTask(Task, Subset):
+    def __init__(self, dataset, indices, num_classes=None,
+                 target_transform=None):
+        if num_classes is None:
+            num_classes = dataset.num_classes
+        Task.__init__(self, dataset.index, num_classes)
+        Subset.__init__(self, dataset, indices)
+        self.dataset.target_transform_append(target_transform)
+
+    def __getitem__(self, index):
+        return Subset.__getitem__(self, index)
+
+    def __hash__(self):
+        return hash((self.index, tuple(self.indices)))
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/gradient_based.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/gradient_based.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import torch
-
-from collections import OrderedDict
-from lightningdata.thirdparty.torchmeta.modules import MetaModule
-
-
-def gradient_update_parameters(model,
-                               loss,
-                               params=None,
-                               step_size=0.5,
-                               first_order=False):
-    """Update of the meta-parameters with one step of gradient descent on the
-    loss function.
-
-    Parameters
-    ----------
-    model : `torchmeta.modules.MetaModule` instance
-        The model.
-
-    loss : `torch.Tensor` instance
-        The value of the inner-loss. This is the result of the training dataset
-        through the loss function.
-
-    params : `collections.OrderedDict` instance, optional
-        Dictionary containing the meta-parameters of the model. If `None`, then
-        the values stored in `model.meta_named_parameters()` are used. This is
-        useful for running multiple steps of gradient descent as the inner-loop.
-
-    step_size : int, `torch.Tensor`, or `collections.OrderedDict` instance (default: 0.5)
-        The step size in the gradient update. If an `OrderedDict`, then the
-        keys must match the keys in `params`.
-
-    first_order : bool (default: `False`)
-        If `True`, then the first order approximation of MAML is used.
-
-    Returns
-    -------
-    updated_params : `collections.OrderedDict` instance
-        Dictionary containing the updated meta-parameters of the model, with one
-        gradient update wrt. the inner-loss.
-    """
-    if not isinstance(model, MetaModule):
-        raise ValueError('The model must be an instance of `torchmeta.modules.'
-                         'MetaModule`, got `{0}`'.format(type(model)))
-
-    if params is None:
-        params = OrderedDict(model.meta_named_parameters())
-
-    grads = torch.autograd.grad(loss,
-                                params.values(),
-                                create_graph=not first_order)
-
-    updated_params = OrderedDict()
-
-    if isinstance(step_size, (dict, OrderedDict)):
-        for (name, param), grad in zip(params.items(), grads):
-            updated_params[name] = param - step_size[name] * grad
-
-    else:
-        for (name, param), grad in zip(params.items(), grads):
-            updated_params[name] = param - step_size * grad
-
-    return updated_params
+import torch
+
+from collections import OrderedDict
+from lightningdata.thirdparty.torchmeta.modules import MetaModule
+
+
+def gradient_update_parameters(model,
+                               loss,
+                               params=None,
+                               step_size=0.5,
+                               first_order=False):
+    """Update of the meta-parameters with one step of gradient descent on the
+    loss function.
+
+    Parameters
+    ----------
+    model : `torchmeta.modules.MetaModule` instance
+        The model.
+
+    loss : `torch.Tensor` instance
+        The value of the inner-loss. This is the result of the training dataset
+        through the loss function.
+
+    params : `collections.OrderedDict` instance, optional
+        Dictionary containing the meta-parameters of the model. If `None`, then
+        the values stored in `model.meta_named_parameters()` are used. This is
+        useful for running multiple steps of gradient descent as the inner-loop.
+
+    step_size : int, `torch.Tensor`, or `collections.OrderedDict` instance (default: 0.5)
+        The step size in the gradient update. If an `OrderedDict`, then the
+        keys must match the keys in `params`.
+
+    first_order : bool (default: `False`)
+        If `True`, then the first order approximation of MAML is used.
+
+    Returns
+    -------
+    updated_params : `collections.OrderedDict` instance
+        Dictionary containing the updated meta-parameters of the model, with one
+        gradient update wrt. the inner-loss.
+    """
+    if not isinstance(model, MetaModule):
+        raise ValueError('The model must be an instance of `torchmeta.modules.'
+                         'MetaModule`, got `{0}`'.format(type(model)))
+
+    if params is None:
+        params = OrderedDict(model.meta_named_parameters())
+
+    grads = torch.autograd.grad(loss,
+                                params.values(),
+                                create_graph=not first_order)
+
+    updated_params = OrderedDict()
+
+    if isinstance(step_size, (dict, OrderedDict)):
+        for (name, param), grad in zip(params.items(), grads):
+            updated_params[name] = param - step_size[name] * grad
+
+    else:
+        for (name, param), grad in zip(params.items(), grads):
+            updated_params[name] = param - step_size * grad
+
+    return updated_params
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/matching.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/matching.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-import torch
-import torch.nn.functional as F
-
-__all__ = [
-    'pairwise_cosine_similarity',
-    'matching_log_probas',
-    'matching_probas',
-    'matching_loss'
-]
-
-
-def pairwise_cosine_similarity(embeddings1, embeddings2, eps=1e-8):
-    r"""Computes the pairwise cosine similarity between two tensors of embeddings.
-
-    Parameters
-    ----------
-    embeddings1 : `torch.Tensor` instance
-        A tensor containing embeddings with shape
-        `(batch_size, N, embedding_size)`.
-
-    embeddings2 : `torch.Tensor` instance
-        A tensor containing embeddings with shape
-        `(batch_size, M, embedding_size)`.
-
-    eps: float (default: 1e-8)
-        Small value to avoid division by zero.
-
-    Returns
-    -------
-    similarities : `torch.Tensor` instance
-        A tensor containing the pairwise cosine similarities between the vectors
-        in `embeddings1` and `embeddings2`. This tensor has shape
-        `(batch_size, N, M)`.
-
-    Notes
-    -----
-    The cosine similarity is computed as
-
-        .. math ::
-            \text{similarity} = \dfrac{x_1 \cdot x_2}{\max(\Vert x_1 \Vert _2 \cdot \Vert x_2 \Vert _2, \epsilon)}
-    """
-    sq_norm1 = torch.sum(embeddings1 ** 2, dim=2, keepdim=True)
-    sq_norm2 = torch.sum(embeddings2 ** 2, dim=2).unsqueeze(1)
-    dot_product = torch.bmm(embeddings1, embeddings2.transpose(1, 2))
-    inverse_norm = torch.rsqrt(torch.clamp(sq_norm1 * sq_norm2, min=eps ** 2))
-    return dot_product * inverse_norm
-
-
-def matching_log_probas(embeddings, targets, test_embeddings, num_classes, eps=1e-8):
-    """Computes the log-probability of test samples given the training dataset
-    for the matching network [1].
-
-    Parameters
-    ----------
-    embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the train/support inputs. This
-        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
-
-    targets : `torch.LongTensor` instance
-        A tensor containing the targets of the train/support dataset. This tensor
-        has shape `(batch_size, num_train_samples)`.
-
-    test_embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the test/query inputs. This tensor
-        has shape `(batch_size, num_test_samples, embedding_size)`.
-
-    num_classes : int
-        Number of classes (i.e. `N` in "N-way classification") in the
-        classification task.
-
-    eps : float (default: 1e-8)
-        Small value to avoid division by zero.
-
-    Returns
-    -------
-    log_probas : `torch.Tensor` instance
-        A tensor containing the log-probabilities of the test samples given the
-        training dataset for the matching network. This tensor has shape
-        `(batch_size, num_classes, num_test_samples)`.
-
-    References
-    ----------
-    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
-           Matching Networks for One Shot Learning. In Advances in Neural
-           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
-    """
-    batch_size, num_samples, _ = test_embeddings.shape
-    similarities = pairwise_cosine_similarity(embeddings, test_embeddings, eps=eps)
-    logsumexp = torch.logsumexp(similarities, dim=1, keepdim=True)
-
-    max_similarities, _ = torch.max(similarities, dim=1, keepdim=True)
-    exp_similarities = torch.exp(similarities - max_similarities)
-
-    sum_exp = exp_similarities.new_zeros((batch_size, num_classes, num_samples))
-    indices = targets.unsqueeze(-1).expand_as(exp_similarities)
-    sum_exp.scatter_add_(1, indices, exp_similarities)
-
-    return torch.log(sum_exp) + max_similarities - logsumexp
-
-
-def matching_probas(embeddings, targets, test_embeddings, num_classes, eps=1e-8):
-    """Computes the probability of test samples given the training dataset for
-    the matching network [1].
-
-    Parameters
-    ----------
-    embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the train/support inputs. This
-        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
-
-    targets : `torch.LongTensor` instance
-        A tensor containing the targets of the train/support dataset. This tensor
-        has shape `(batch_size, num_train_samples)`.
-
-    test_embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the test/query inputs. This tensor
-        has shape `(batch_size, num_test_samples, embedding_size)`.
-
-    num_classes : int
-        Number of classes (i.e. `N` in "N-way classification") in the
-        classification task.
-
-    eps : float (default: 1e-8)
-        Small value to avoid division by zero.
-
-    Returns
-    -------
-    probas : `torch.Tensor` instance
-        A tensor containing the probabilities of the test samples given the
-        training dataset for the matching network. This tensor has shape
-        `(batch_size, num_classes, num_test_samples)`.
-
-    References
-    ----------
-    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
-           Matching Networks for One Shot Learning. In Advances in Neural
-           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
-    """
-    log_probas = matching_log_probas(embeddings,
-                                     targets,
-                                     test_embeddings,
-                                     num_classes,
-                                     eps=eps)
-    return log_probas.exp()
-
-
-def matching_loss(train_embeddings,
-                  train_targets,
-                  test_embeddings,
-                  test_targets,
-                  num_classes,
-                  eps=1e-8,
-                  **kwargs):
-    """Compute the loss (i.e. negative log-likelihood) for the matching network
-    on the test/query samples [1].
-
-    Parameters
-    ----------
-    train_embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the train/support inputs. This
-        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
-
-    train_targets : `torch.LongTensor` instance
-        A tensor containing the targets of the train/support dataset. This tensor
-        has shape `(batch_size, num_train_samples)`.
-
-    test_embeddings : `torch.Tensor` instance
-        A tensor containing the embeddings of the test/query inputs. This tensor
-        has shape `(batch_size, num_test_samples, embedding_size)`.
-
-    test_targets : `torch.LongTensor` instance
-        A tensor containing the targets of the test/query dataset. This tensor
-        has shape `(batch_size, num_test_samples)`.
-
-    num_classes : int
-        Number of classes (i.e. `N` in "N-way classification") in the
-        classification task.
-
-    eps : float (default: 1e-8)
-        Small value to avoid division by zero.
-
-    kwargs :
-        Additional keyword arguments to be forwarded to the loss function. See
-        `torch.nn.functional.cross_entropy` for details.
-
-    Returns
-    -------
-    loss : `torch.Tensor` instance
-        A tensor containing the loss for the matching network.
-
-    References
-    ----------
-    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
-           Matching Networks for One Shot Learning. In Advances in Neural
-           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
-    """
-    logits = matching_log_probas(train_embeddings,
-                                 train_targets,
-                                 test_embeddings,
-                                 num_classes,
-                                 eps=eps)
-    return F.nll_loss(logits, test_targets, **kwargs)
+import torch
+import torch.nn.functional as F
+
+__all__ = [
+    'pairwise_cosine_similarity',
+    'matching_log_probas',
+    'matching_probas',
+    'matching_loss'
+]
+
+
+def pairwise_cosine_similarity(embeddings1, embeddings2, eps=1e-8):
+    r"""Computes the pairwise cosine similarity between two tensors of embeddings.
+
+    Parameters
+    ----------
+    embeddings1 : `torch.Tensor` instance
+        A tensor containing embeddings with shape
+        `(batch_size, N, embedding_size)`.
+
+    embeddings2 : `torch.Tensor` instance
+        A tensor containing embeddings with shape
+        `(batch_size, M, embedding_size)`.
+
+    eps: float (default: 1e-8)
+        Small value to avoid division by zero.
+
+    Returns
+    -------
+    similarities : `torch.Tensor` instance
+        A tensor containing the pairwise cosine similarities between the vectors
+        in `embeddings1` and `embeddings2`. This tensor has shape
+        `(batch_size, N, M)`.
+
+    Notes
+    -----
+    The cosine similarity is computed as
+
+        .. math ::
+            \text{similarity} = \dfrac{x_1 \cdot x_2}{\max(\Vert x_1 \Vert _2 \cdot \Vert x_2 \Vert _2, \epsilon)}
+    """
+    sq_norm1 = torch.sum(embeddings1 ** 2, dim=2, keepdim=True)
+    sq_norm2 = torch.sum(embeddings2 ** 2, dim=2).unsqueeze(1)
+    dot_product = torch.bmm(embeddings1, embeddings2.transpose(1, 2))
+    inverse_norm = torch.rsqrt(torch.clamp(sq_norm1 * sq_norm2, min=eps ** 2))
+    return dot_product * inverse_norm
+
+
+def matching_log_probas(embeddings, targets, test_embeddings, num_classes, eps=1e-8):
+    """Computes the log-probability of test samples given the training dataset
+    for the matching network [1].
+
+    Parameters
+    ----------
+    embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the train/support inputs. This
+        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
+
+    targets : `torch.LongTensor` instance
+        A tensor containing the targets of the train/support dataset. This tensor
+        has shape `(batch_size, num_train_samples)`.
+
+    test_embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the test/query inputs. This tensor
+        has shape `(batch_size, num_test_samples, embedding_size)`.
+
+    num_classes : int
+        Number of classes (i.e. `N` in "N-way classification") in the
+        classification task.
+
+    eps : float (default: 1e-8)
+        Small value to avoid division by zero.
+
+    Returns
+    -------
+    log_probas : `torch.Tensor` instance
+        A tensor containing the log-probabilities of the test samples given the
+        training dataset for the matching network. This tensor has shape
+        `(batch_size, num_classes, num_test_samples)`.
+
+    References
+    ----------
+    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
+           Matching Networks for One Shot Learning. In Advances in Neural
+           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
+    """
+    batch_size, num_samples, _ = test_embeddings.shape
+    similarities = pairwise_cosine_similarity(embeddings, test_embeddings, eps=eps)
+    logsumexp = torch.logsumexp(similarities, dim=1, keepdim=True)
+
+    max_similarities, _ = torch.max(similarities, dim=1, keepdim=True)
+    exp_similarities = torch.exp(similarities - max_similarities)
+
+    sum_exp = exp_similarities.new_zeros((batch_size, num_classes, num_samples))
+    indices = targets.unsqueeze(-1).expand_as(exp_similarities)
+    sum_exp.scatter_add_(1, indices, exp_similarities)
+
+    return torch.log(sum_exp) + max_similarities - logsumexp
+
+
+def matching_probas(embeddings, targets, test_embeddings, num_classes, eps=1e-8):
+    """Computes the probability of test samples given the training dataset for
+    the matching network [1].
+
+    Parameters
+    ----------
+    embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the train/support inputs. This
+        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
+
+    targets : `torch.LongTensor` instance
+        A tensor containing the targets of the train/support dataset. This tensor
+        has shape `(batch_size, num_train_samples)`.
+
+    test_embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the test/query inputs. This tensor
+        has shape `(batch_size, num_test_samples, embedding_size)`.
+
+    num_classes : int
+        Number of classes (i.e. `N` in "N-way classification") in the
+        classification task.
+
+    eps : float (default: 1e-8)
+        Small value to avoid division by zero.
+
+    Returns
+    -------
+    probas : `torch.Tensor` instance
+        A tensor containing the probabilities of the test samples given the
+        training dataset for the matching network. This tensor has shape
+        `(batch_size, num_classes, num_test_samples)`.
+
+    References
+    ----------
+    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
+           Matching Networks for One Shot Learning. In Advances in Neural
+           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
+    """
+    log_probas = matching_log_probas(embeddings,
+                                     targets,
+                                     test_embeddings,
+                                     num_classes,
+                                     eps=eps)
+    return log_probas.exp()
+
+
+def matching_loss(train_embeddings,
+                  train_targets,
+                  test_embeddings,
+                  test_targets,
+                  num_classes,
+                  eps=1e-8,
+                  **kwargs):
+    """Compute the loss (i.e. negative log-likelihood) for the matching network
+    on the test/query samples [1].
+
+    Parameters
+    ----------
+    train_embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the train/support inputs. This
+        tensor has shape `(batch_size, num_train_samples, embedding_size)`.
+
+    train_targets : `torch.LongTensor` instance
+        A tensor containing the targets of the train/support dataset. This tensor
+        has shape `(batch_size, num_train_samples)`.
+
+    test_embeddings : `torch.Tensor` instance
+        A tensor containing the embeddings of the test/query inputs. This tensor
+        has shape `(batch_size, num_test_samples, embedding_size)`.
+
+    test_targets : `torch.LongTensor` instance
+        A tensor containing the targets of the test/query dataset. This tensor
+        has shape `(batch_size, num_test_samples)`.
+
+    num_classes : int
+        Number of classes (i.e. `N` in "N-way classification") in the
+        classification task.
+
+    eps : float (default: 1e-8)
+        Small value to avoid division by zero.
+
+    kwargs :
+        Additional keyword arguments to be forwarded to the loss function. See
+        `torch.nn.functional.cross_entropy` for details.
+
+    Returns
+    -------
+    loss : `torch.Tensor` instance
+        A tensor containing the loss for the matching network.
+
+    References
+    ----------
+    .. [1] Vinyals, O., Blundell, C., Lillicrap, T. and Wierstra, D. (2016).
+           Matching Networks for One Shot Learning. In Advances in Neural
+           Information Processing Systems (pp. 3630-3638) (https://arxiv.org/abs/1606.04080)
+    """
+    logits = matching_log_probas(train_embeddings,
+                                 train_targets,
+                                 test_embeddings,
+                                 num_classes,
+                                 eps=eps)
+    return F.nll_loss(logits, test_targets, **kwargs)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/metrics.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/metrics.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import torch
-import torch.nn.functional as F
-
-from lightningdata.thirdparty.torchmeta.utils.prototype import get_prototypes
-
-__all__ = ['hardness_metric']
-
-
-def _pad_images(inputs, size=(224, 224), **kwargs):
-    height, width = inputs.shape[-2:]
-    pad_height, pad_width = (size[0] - height) // 2, (size[1] - width) // 2
-    padding = (pad_width, size[1] - width - pad_width,
-               pad_height, size[0] - height - pad_height)
-    return F.pad(inputs, padding, **kwargs)
-
-
-def hardness_metric(batch, num_classes):
-    """Hardness metric of an episode, as defined in [1].
-
-    Parameters
-    ----------
-    batch : dict
-        The batch of tasks over which the metric is computed. The batch of tasks
-        is a dictionary containing the keys `train` (or `support`) and `test`
-        (or `query`). This is typically the output of `BatchMetaDataLoader`.
-
-    num_classes : int
-        The number of classes in the classification task. This corresponds to
-        the number of ways in an `N`-way classification problem.
-
-    Returns
-    -------
-    metric : `torch.FloatTensor` instance
-        Values of the hardness metric for each task in the batch.
-
-    References
-    ----------
-    .. [1] Dhillon, G. S., Chaudhari, P., Ravichandran, A. and Soatto S. (2019).
-           A Baseline for Few-Shot Image Classification. (https://arxiv.org/abs/1909.02729)
-    """
-    if ('train' not in batch) and ('support' not in batch):
-        raise ValueError('The tasks do not contain any training/support set. '
-                         'Make sure the tasks contain either the "train" or the '
-                         '"support" key.')
-    if ('test' not in batch) and ('query' not in batch):
-        raise ValueError('The tasks do not contain any test/query set. Make '
-                         'sure the tasks contain either the "test" of the '
-                         '"query" key.')
-
-    train = 'train' if ('train' in batch) else 'support'
-    test = 'test' if ('test' in batch) else 'query'
-
-    with torch.no_grad():
-        # Load a pre-trained backbone Resnet-152 model from PyTorch Hub
-        backbone = torch.hub.load('pytorch/vision:v0.5.0',
-                                  'resnet152',
-                                  pretrained=True,
-                                  verbose=False)
-        backbone.eval()
-
-        train_inputs, train_targets = batch[train]
-        test_inputs, test_targets = batch[test]
-        batch_size, num_images, num_channels = train_inputs.shape[:3]
-        num_test_images = test_inputs.size(1)
-
-        backbone.to(device=train_inputs.device)
-
-        if num_channels != 3:
-            raise ValueError('The images must be RGB images.')
-
-        # Pad the images so that they are compatible with the pre-trained model
-        padded_train_inputs = _pad_images(train_inputs,
-            size=(224, 224), mode='constant', value=0.)
-        padded_test_inputs = _pad_images(test_inputs,
-            size=(224, 224), mode='constant', value=0.)
-
-        # Compute the features from the logits returned by the pre-trained
-        # model on the train/support examples. These features are z(x, theta)_+,
-        # averaged for each class
-        train_logits = backbone(padded_train_inputs.view(-1, 3, 224, 224))
-        train_logits = F.relu(train_logits.view(batch_size, num_images, -1))
-        train_features = get_prototypes(train_logits, train_targets, num_classes)
-
-        # Get the weights by normalizing the features
-        weights = F.normalize(train_features, p=2, dim=2)
-
-        # Compute and normalize the logits of the test/query examples
-        test_logits = backbone(padded_test_inputs.view(-1, 3, 224, 224))
-        test_logits = test_logits.view(batch_size, num_test_images, -1)
-        test_logits = F.normalize(test_logits, p=2, dim=2)
-
-        # Compute the log probabilities of the test/query examples
-        test_logits = torch.bmm(weights, test_logits.transpose(1, 2))
-        test_log_probas = -F.cross_entropy(test_logits, test_targets,
-                                           reduction='none')
-
-        # Compute the log-odds ratios for each image of the test/query set
-        log_odds_ratios = torch.log1p(-test_log_probas.exp()) - test_log_probas
-
-    return torch.mean(log_odds_ratios, dim=1)
+import torch
+import torch.nn.functional as F
+
+from lightningdata.thirdparty.torchmeta.utils.prototype import get_prototypes
+
+__all__ = ['hardness_metric']
+
+
+def _pad_images(inputs, size=(224, 224), **kwargs):
+    height, width = inputs.shape[-2:]
+    pad_height, pad_width = (size[0] - height) // 2, (size[1] - width) // 2
+    padding = (pad_width, size[1] - width - pad_width,
+               pad_height, size[0] - height - pad_height)
+    return F.pad(inputs, padding, **kwargs)
+
+
+def hardness_metric(batch, num_classes):
+    """Hardness metric of an episode, as defined in [1].
+
+    Parameters
+    ----------
+    batch : dict
+        The batch of tasks over which the metric is computed. The batch of tasks
+        is a dictionary containing the keys `train` (or `support`) and `test`
+        (or `query`). This is typically the output of `BatchMetaDataLoader`.
+
+    num_classes : int
+        The number of classes in the classification task. This corresponds to
+        the number of ways in an `N`-way classification problem.
+
+    Returns
+    -------
+    metric : `torch.FloatTensor` instance
+        Values of the hardness metric for each task in the batch.
+
+    References
+    ----------
+    .. [1] Dhillon, G. S., Chaudhari, P., Ravichandran, A. and Soatto S. (2019).
+           A Baseline for Few-Shot Image Classification. (https://arxiv.org/abs/1909.02729)
+    """
+    if ('train' not in batch) and ('support' not in batch):
+        raise ValueError('The tasks do not contain any training/support set. '
+                         'Make sure the tasks contain either the "train" or the '
+                         '"support" key.')
+    if ('test' not in batch) and ('query' not in batch):
+        raise ValueError('The tasks do not contain any test/query set. Make '
+                         'sure the tasks contain either the "test" of the '
+                         '"query" key.')
+
+    train = 'train' if ('train' in batch) else 'support'
+    test = 'test' if ('test' in batch) else 'query'
+
+    with torch.no_grad():
+        # Load a pre-trained backbone Resnet-152 model from PyTorch Hub
+        backbone = torch.hub.load('pytorch/vision:v0.5.0',
+                                  'resnet152',
+                                  pretrained=True,
+                                  verbose=False)
+        backbone.eval()
+
+        train_inputs, train_targets = batch[train]
+        test_inputs, test_targets = batch[test]
+        batch_size, num_images, num_channels = train_inputs.shape[:3]
+        num_test_images = test_inputs.size(1)
+
+        backbone.to(device=train_inputs.device)
+
+        if num_channels != 3:
+            raise ValueError('The images must be RGB images.')
+
+        # Pad the images so that they are compatible with the pre-trained model
+        padded_train_inputs = _pad_images(train_inputs,
+            size=(224, 224), mode='constant', value=0.)
+        padded_test_inputs = _pad_images(test_inputs,
+            size=(224, 224), mode='constant', value=0.)
+
+        # Compute the features from the logits returned by the pre-trained
+        # model on the train/support examples. These features are z(x, theta)_+,
+        # averaged for each class
+        train_logits = backbone(padded_train_inputs.view(-1, 3, 224, 224))
+        train_logits = F.relu(train_logits.view(batch_size, num_images, -1))
+        train_features = get_prototypes(train_logits, train_targets, num_classes)
+
+        # Get the weights by normalizing the features
+        weights = F.normalize(train_features, p=2, dim=2)
+
+        # Compute and normalize the logits of the test/query examples
+        test_logits = backbone(padded_test_inputs.view(-1, 3, 224, 224))
+        test_logits = test_logits.view(batch_size, num_test_images, -1)
+        test_logits = F.normalize(test_logits, p=2, dim=2)
+
+        # Compute the log probabilities of the test/query examples
+        test_logits = torch.bmm(weights, test_logits.transpose(1, 2))
+        test_log_probas = -F.cross_entropy(test_logits, test_targets,
+                                           reduction='none')
+
+        # Compute the log-odds ratios for each image of the test/query set
+        log_odds_ratios = torch.log1p(-test_log_probas.exp()) - test_log_probas
+
+    return torch.mean(log_odds_ratios, dim=1)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/prototype.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/prototype.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import torch
-import torch.nn.functional as F
-
-__all__ = ['get_num_samples', 'get_prototypes', 'prototypical_loss']
-
-
-def get_num_samples(targets, num_classes, dtype=None):
-    batch_size = targets.size(0)
-    with torch.no_grad():
-        ones = torch.ones_like(targets, dtype=dtype)
-        num_samples = ones.new_zeros((batch_size, num_classes))
-        num_samples.scatter_add_(1, targets, ones)
-    return num_samples
-
-
-def get_prototypes(embeddings, targets, num_classes):
-    """Compute the prototypes (the mean vector of the embedded training/support 
-    points belonging to its class) for each classes in the task.
-
-    Parameters
-    ----------
-    embeddings : `torch.FloatTensor` instance
-        A tensor containing the embeddings of the support points. This tensor 
-        has shape `(batch_size, num_examples, embedding_size)`.
-
-    targets : `torch.LongTensor` instance
-        A tensor containing the targets of the support points. This tensor has 
-        shape `(batch_size, num_examples)`.
-
-    num_classes : int
-        Number of classes in the task.
-
-    Returns
-    -------
-    prototypes : `torch.FloatTensor` instance
-        A tensor containing the prototypes for each class. This tensor has shape
-        `(batch_size, num_classes, embedding_size)`.
-    """
-    batch_size, embedding_size = embeddings.size(0), embeddings.size(-1)
-    
-    num_samples = get_num_samples(targets, num_classes, dtype=embeddings.dtype)
-    num_samples.unsqueeze_(-1)
-    num_samples = torch.max(num_samples, torch.ones_like(num_samples))
-
-    prototypes = embeddings.new_zeros((batch_size, num_classes, embedding_size))
-    indices = targets.unsqueeze(-1).expand_as(embeddings)
-    prototypes.scatter_add_(1, indices, embeddings).div_(num_samples)
-
-    return prototypes
-
-
-def prototypical_loss(prototypes, embeddings, targets, **kwargs):
-    """Compute the loss (i.e. negative log-likelihood) for the prototypical 
-    network, on the test/query points.
-
-    Parameters
-    ----------
-    prototypes : `torch.FloatTensor` instance
-        A tensor containing the prototypes for each class. This tensor has shape 
-        `(batch_size, num_classes, embedding_size)`.
-
-    embeddings : `torch.FloatTensor` instance
-        A tensor containing the embeddings of the query points. This tensor has 
-        shape `(batch_size, num_examples, embedding_size)`.
-
-    targets : `torch.LongTensor` instance
-        A tensor containing the targets of the query points. This tensor has 
-        shape `(batch_size, num_examples)`.
-
-    Returns
-    -------
-    loss : `torch.FloatTensor` instance
-        The negative log-likelihood on the query points.
-    """
-    squared_distances = torch.sum((prototypes.unsqueeze(2)
-        - embeddings.unsqueeze(1)) ** 2, dim=-1)
-    return F.cross_entropy(-squared_distances, targets, **kwargs)
+import torch
+import torch.nn.functional as F
+
+__all__ = ['get_num_samples', 'get_prototypes', 'prototypical_loss']
+
+
+def get_num_samples(targets, num_classes, dtype=None):
+    batch_size = targets.size(0)
+    with torch.no_grad():
+        ones = torch.ones_like(targets, dtype=dtype)
+        num_samples = ones.new_zeros((batch_size, num_classes))
+        num_samples.scatter_add_(1, targets, ones)
+    return num_samples
+
+
+def get_prototypes(embeddings, targets, num_classes):
+    """Compute the prototypes (the mean vector of the embedded training/support 
+    points belonging to its class) for each classes in the task.
+
+    Parameters
+    ----------
+    embeddings : `torch.FloatTensor` instance
+        A tensor containing the embeddings of the support points. This tensor 
+        has shape `(batch_size, num_examples, embedding_size)`.
+
+    targets : `torch.LongTensor` instance
+        A tensor containing the targets of the support points. This tensor has 
+        shape `(batch_size, num_examples)`.
+
+    num_classes : int
+        Number of classes in the task.
+
+    Returns
+    -------
+    prototypes : `torch.FloatTensor` instance
+        A tensor containing the prototypes for each class. This tensor has shape
+        `(batch_size, num_classes, embedding_size)`.
+    """
+    batch_size, embedding_size = embeddings.size(0), embeddings.size(-1)
+    
+    num_samples = get_num_samples(targets, num_classes, dtype=embeddings.dtype)
+    num_samples.unsqueeze_(-1)
+    num_samples = torch.max(num_samples, torch.ones_like(num_samples))
+
+    prototypes = embeddings.new_zeros((batch_size, num_classes, embedding_size))
+    indices = targets.unsqueeze(-1).expand_as(embeddings)
+    prototypes.scatter_add_(1, indices, embeddings).div_(num_samples)
+
+    return prototypes
+
+
+def prototypical_loss(prototypes, embeddings, targets, **kwargs):
+    """Compute the loss (i.e. negative log-likelihood) for the prototypical 
+    network, on the test/query points.
+
+    Parameters
+    ----------
+    prototypes : `torch.FloatTensor` instance
+        A tensor containing the prototypes for each class. This tensor has shape 
+        `(batch_size, num_classes, embedding_size)`.
+
+    embeddings : `torch.FloatTensor` instance
+        A tensor containing the embeddings of the query points. This tensor has 
+        shape `(batch_size, num_examples, embedding_size)`.
+
+    targets : `torch.LongTensor` instance
+        A tensor containing the targets of the query points. This tensor has 
+        shape `(batch_size, num_examples)`.
+
+    Returns
+    -------
+    loss : `torch.FloatTensor` instance
+        The negative log-likelihood on the query points.
+    """
+    squared_distances = torch.sum((prototypes.unsqueeze(2)
+        - embeddings.unsqueeze(1)) ** 2, dim=-1)
+    return F.cross_entropy(-squared_distances, targets, **kwargs)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata/thirdparty/torchmeta/utils/r2d2.py` & `lightningdata-modules-0.1.6/lightningdata/thirdparty/torchmeta/utils/r2d2.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import torch
-import torch.nn.functional as F
-import warnings
-
-from collections import namedtuple
-from math import sqrt
-
-__all__ = ['ridge_regression']
-
-
-_RR_weight_bias = namedtuple('_RR_weight_bias', 'weight bias')
-
-def ridge_regression(embeddings,
-                     targets,
-                     reg_lambda,
-                     num_classes=None,
-                     use_woodbury=None,
-                     scale=True,
-                     bias=True):
-    r"""Closed-form solution of a linear function of the embeddings, found 
-    using ridge regression.
-
-        W^{*} = argmin_{W} ||XW - Y||^{2} + \lambda ||W||^{2}
-              = (X^{T}X + \lambda I)^{-1}X^{T}Y
-
-    Parameters
-    ----------
-    embeddings : `torch.FloatTensor` instance
-        A tensor containing the embeddings of the support points from a single
-        task. This tensor has shape `(num_examples, embedding_size)`.
-
-    targets : `torch.LongTensor` or `torch.FloatTensor` instance
-        A tensor containing the targets of the support points from a single
-        task. If this tensor is a `torch.LongTensor` instance (i.e.
-        classification task), then it has shape `(num_examples,)`. If this
-        tensor is a `torch.FloatTensor` instance (i.e. regression task), then
-        it has shape `(num_examples, output_size)`.
-
-    reg_lambda : float or `torch.FloatTensor` instance
-        The regularization constant lambda in the L2-regularized MSE loss. This
-        constant can be a tensor.
-
-    num_classes : int (optional)
-        Number of classes in the task. If `None`, then `targets` must be a
-        `torch.FloatTensor` instance (i.e. regression task).
-
-    use_woodbury : bool (optional)
-        If `True`, then the Woodbury formula is used to solve the ridge
-        regression. If `None`, then use the Woodbury formula only in cases
-        where the number of samples in the support set is smaller than the
-        embedding size (standard in few-shot learning).
-
-    scale : bool (default: `True`)
-        If `True`, scales the embeddings and targets by the number of
-        support points.
-
-    bias : bool (default: `True`)
-        If `True`, fit an affine function and return the weights and bias.
-
-    Returns
-    -------
-    solution : namedtuple instance
-        A namedtuple, with fields `weight` and `bias`, containing the weight
-        (and bias, if `bias=True`) of the linear function. If `bias=False`,
-        then `solution.bias == None`.
-
-    References
-    ----------
-    .. [1] Bertinetto L., Henriques J. F., Torr P. H.S., Vedaldi A. (2019).
-           Meta-learning with differentiable closed-form solvers. In International
-           Conference on Learning Representations (https://arxiv.org/abs/1805.08136)
-    """
-    num_samples, embedding_size = embeddings.size()
-    is_regression_task = targets.dtype.is_floating_point
-    if num_classes is None:
-        if is_regression_task and (targets.ndim != 2):
-            raise ValueError('The `targets` tensor has invalid shape `{0}`. '
-                             'This tensor must have shape `(num_examples, '
-                             'output_size)`.'.format(targets.shape))
-
-        elif not is_regression_task:
-            warnings.warn('The number of classes was not given as an input to '
-                          '`ridge_regression`. Using the number of classes '
-                          'found in `targets`. If you know the number of '
-                          'classes (i.e. N in `N-way` classification), then it '
-                          'is recommended to provide it to `ridge_regression`.',
-                          stacklevel=2)
-            num_classes = -1
-
-    if not is_regression_task:
-        targets = (F.one_hot(targets, num_classes=num_classes)
-                    .to(dtype=embeddings.dtype))
-
-    if use_woodbury is None:
-        use_woodbury = (num_samples <= embedding_size + bias)
-
-    if bias:
-        ones = embeddings.new_ones((num_samples, 1))
-        embeddings = torch.cat([ones, embeddings], dim=1)
-
-    if scale:
-        embeddings = embeddings / sqrt(num_samples)
-        targets = targets / sqrt(num_samples)
-
-    if use_woodbury:
-        eye = torch.eye(num_samples,
-                        dtype=embeddings.dtype,
-                        device=embeddings.device)
-        A = torch.matmul(embeddings, embeddings.t()) + reg_lambda * eye
-        solution = torch.linalg.solve(A, targets)
-        weight_bias = torch.matmul(embeddings.t(), solution)
-    else:
-        eye = torch.eye(embedding_size + bias,
-                        dtype=embeddings.dtype,
-                        device=embeddings.device)
-        A = torch.matmul(embeddings.t(), embeddings) + reg_lambda * eye
-        b = torch.matmul(embeddings.t(), targets)
-        weight_bias = torch.linalg.solve(A, b)
-
-    if bias:
-        return _RR_weight_bias(weight=weight_bias[1:].t(), bias=weight_bias[0])
-    else:
-        return _RR_weight_bias(weight=weight_bias.t(), bias=None)
+import torch
+import torch.nn.functional as F
+import warnings
+
+from collections import namedtuple
+from math import sqrt
+
+__all__ = ['ridge_regression']
+
+
+_RR_weight_bias = namedtuple('_RR_weight_bias', 'weight bias')
+
+def ridge_regression(embeddings,
+                     targets,
+                     reg_lambda,
+                     num_classes=None,
+                     use_woodbury=None,
+                     scale=True,
+                     bias=True):
+    r"""Closed-form solution of a linear function of the embeddings, found 
+    using ridge regression.
+
+        W^{*} = argmin_{W} ||XW - Y||^{2} + \lambda ||W||^{2}
+              = (X^{T}X + \lambda I)^{-1}X^{T}Y
+
+    Parameters
+    ----------
+    embeddings : `torch.FloatTensor` instance
+        A tensor containing the embeddings of the support points from a single
+        task. This tensor has shape `(num_examples, embedding_size)`.
+
+    targets : `torch.LongTensor` or `torch.FloatTensor` instance
+        A tensor containing the targets of the support points from a single
+        task. If this tensor is a `torch.LongTensor` instance (i.e.
+        classification task), then it has shape `(num_examples,)`. If this
+        tensor is a `torch.FloatTensor` instance (i.e. regression task), then
+        it has shape `(num_examples, output_size)`.
+
+    reg_lambda : float or `torch.FloatTensor` instance
+        The regularization constant lambda in the L2-regularized MSE loss. This
+        constant can be a tensor.
+
+    num_classes : int (optional)
+        Number of classes in the task. If `None`, then `targets` must be a
+        `torch.FloatTensor` instance (i.e. regression task).
+
+    use_woodbury : bool (optional)
+        If `True`, then the Woodbury formula is used to solve the ridge
+        regression. If `None`, then use the Woodbury formula only in cases
+        where the number of samples in the support set is smaller than the
+        embedding size (standard in few-shot learning).
+
+    scale : bool (default: `True`)
+        If `True`, scales the embeddings and targets by the number of
+        support points.
+
+    bias : bool (default: `True`)
+        If `True`, fit an affine function and return the weights and bias.
+
+    Returns
+    -------
+    solution : namedtuple instance
+        A namedtuple, with fields `weight` and `bias`, containing the weight
+        (and bias, if `bias=True`) of the linear function. If `bias=False`,
+        then `solution.bias == None`.
+
+    References
+    ----------
+    .. [1] Bertinetto L., Henriques J. F., Torr P. H.S., Vedaldi A. (2019).
+           Meta-learning with differentiable closed-form solvers. In International
+           Conference on Learning Representations (https://arxiv.org/abs/1805.08136)
+    """
+    num_samples, embedding_size = embeddings.size()
+    is_regression_task = targets.dtype.is_floating_point
+    if num_classes is None:
+        if is_regression_task and (targets.ndim != 2):
+            raise ValueError('The `targets` tensor has invalid shape `{0}`. '
+                             'This tensor must have shape `(num_examples, '
+                             'output_size)`.'.format(targets.shape))
+
+        elif not is_regression_task:
+            warnings.warn('The number of classes was not given as an input to '
+                          '`ridge_regression`. Using the number of classes '
+                          'found in `targets`. If you know the number of '
+                          'classes (i.e. N in `N-way` classification), then it '
+                          'is recommended to provide it to `ridge_regression`.',
+                          stacklevel=2)
+            num_classes = -1
+
+    if not is_regression_task:
+        targets = (F.one_hot(targets, num_classes=num_classes)
+                    .to(dtype=embeddings.dtype))
+
+    if use_woodbury is None:
+        use_woodbury = (num_samples <= embedding_size + bias)
+
+    if bias:
+        ones = embeddings.new_ones((num_samples, 1))
+        embeddings = torch.cat([ones, embeddings], dim=1)
+
+    if scale:
+        embeddings = embeddings / sqrt(num_samples)
+        targets = targets / sqrt(num_samples)
+
+    if use_woodbury:
+        eye = torch.eye(num_samples,
+                        dtype=embeddings.dtype,
+                        device=embeddings.device)
+        A = torch.matmul(embeddings, embeddings.t()) + reg_lambda * eye
+        solution = torch.linalg.solve(A, targets)
+        weight_bias = torch.matmul(embeddings.t(), solution)
+    else:
+        eye = torch.eye(embedding_size + bias,
+                        dtype=embeddings.dtype,
+                        device=embeddings.device)
+        A = torch.matmul(embeddings.t(), embeddings) + reg_lambda * eye
+        b = torch.matmul(embeddings.t(), targets)
+        weight_bias = torch.linalg.solve(A, b)
+
+    if bias:
+        return _RR_weight_bias(weight=weight_bias[1:].t(), bias=weight_bias[0])
+    else:
+        return _RR_weight_bias(weight=weight_bias.t(), bias=None)
```

### Comparing `lightningdata-modules-0.1.5/lightningdata_modules.egg-info/PKG-INFO` & `lightningdata-modules-0.1.6/lightningdata_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.5/lightningdata_modules.egg-info/SOURCES.txt` & `lightningdata-modules-0.1.6/lightningdata_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.5/setup.py` & `lightningdata-modules-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 required_packages = [
     "getfilelistpy", "lmdb", "matplotlib", "numpy", "Pillow", "pytorch_lightning", "setuptools",
     "six", "torch", "torchvision", "py7zr"
 ]
 
 setup(
     name="lightningdata-modules",
-    version="0.1.5",
+    version="0.1.6",
     description="Pre-packages Pytorch-Lightning datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ManuelRoeder/lightningdata-modules",
     author="Manuel Roeder",
     author_email="manuel.roeder@web.de",
     license="MIT",
```

