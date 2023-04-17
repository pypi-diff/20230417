# Comparing `tmp/torch-conduit-0.1.7.tar.gz` & `tmp/torch_conduit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-conduit-0.1.7.tar", max compression
+gzip compressed data, was "torch_conduit-0.2.0.tar", max compression
```

## Comparing `torch-conduit-0.1.7.tar` & `torch_conduit-0.2.0.tar`

### file list

```diff
@@ -1,92 +1,95 @@
--rw-r--r--   0        0        0     1081 2022-03-16 16:46:34.972737 torch-conduit-0.1.7/LICENSE
--rw-r--r--   0        0        0       91 2022-03-16 16:46:34.972839 torch-conduit-0.1.7/README.md
--rw-r--r--   0        0        0       12 2022-03-16 16:46:34.973000 torch-conduit-0.1.7/conduit/__init__.py
--rw-r--r--   0        0        0     1448 2022-03-18 11:18:24.897894 torch-conduit-0.1.7/conduit/conf/configen.yaml
--rw-r--r--   0        0        0      102 2022-03-18 22:29:58.799587 torch-conduit-0.1.7/conduit/data/__init__.py
--rw-r--r--   0        0        0      219 2022-03-18 15:57:36.611686 torch-conduit-0.1.7/conduit/data/constants.py
--rw-r--r--   0        0        0       63 2022-03-16 16:46:34.973788 torch-conduit-0.1.7/conduit/data/datamodules/__init__.py
--rw-r--r--   0        0        0       28 2022-03-16 16:46:34.973923 torch-conduit-0.1.7/conduit/data/datamodules/audio/__init__.py
--rw-r--r--   0        0        0     2682 2022-05-24 11:32:38.828093 torch-conduit-0.1.7/conduit/data/datamodules/audio/base.py
--rw-r--r--   0        0        0     3094 2022-07-21 10:31:30.318530 torch-conduit-0.1.7/conduit/data/datamodules/audio/ecoacoustics.py
--rw-r--r--   0        0        0    12173 2022-08-04 09:57:07.299538 torch-conduit-0.1.7/conduit/data/datamodules/base.py
--rw-r--r--   0        0        0        0 2022-03-16 16:46:34.974557 torch-conduit-0.1.7/conduit/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0     1069 2022-03-16 16:46:34.974694 torch-conduit-0.1.7/conduit/data/datamodules/tabular/dummy.py
--rw-r--r--   0        0        0      156 2022-07-29 10:56:30.054597 torch-conduit-0.1.7/conduit/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0     4056 2022-08-12 14:30:04.065348 torch-conduit-0.1.7/conduit/data/datamodules/vision/base.py
--rw-r--r--   0        0        0     2905 2022-03-29 12:47:28.253769 torch-conduit-0.1.7/conduit/data/datamodules/vision/camelyon17.py
--rw-r--r--   0        0        0     2382 2022-03-29 12:37:17.343582 torch-conduit-0.1.7/conduit/data/datamodules/vision/celeba.py
--rw-r--r--   0        0        0     3673 2022-03-29 12:46:43.542027 torch-conduit-0.1.7/conduit/data/datamodules/vision/cmnist.py
--rw-r--r--   0        0        0     1125 2022-03-23 18:10:07.468554 torch-conduit-0.1.7/conduit/data/datamodules/vision/dummy.py
--rw-r--r--   0        0        0     2203 2022-03-29 12:45:57.092574 torch-conduit-0.1.7/conduit/data/datamodules/vision/nico.py
--rw-r--r--   0        0        0     1874 2022-07-29 10:56:30.055137 torch-conduit-0.1.7/conduit/data/datamodules/vision/pacs.py
--rw-r--r--   0        0        0     2598 2022-03-29 12:46:08.963961 torch-conduit-0.1.7/conduit/data/datamodules/vision/waterbirds.py
--rw-r--r--   0        0        0      108 2022-07-28 18:08:14.926965 torch-conduit-0.1.7/conduit/data/datasets/__init__.py
--rw-r--r--   0        0        0       28 2022-03-16 16:46:34.976492 torch-conduit-0.1.7/conduit/data/datasets/audio/__init__.py
--rw-r--r--   0        0        0     2803 2022-04-28 15:54:10.610641 torch-conduit-0.1.7/conduit/data/datasets/audio/base.py
--rw-r--r--   0        0        0    11380 2022-07-21 10:31:30.320704 torch-conduit-0.1.7/conduit/data/datasets/audio/ecoacoustics.py
--rw-r--r--   0        0        0     9639 2022-09-09 14:04:16.860566 torch-conduit-0.1.7/conduit/data/datasets/base.py
--rw-r--r--   0        0        0       20 2022-03-16 16:46:34.977678 torch-conduit-0.1.7/conduit/data/datasets/tabular/__init__.py
--rw-r--r--   0        0        0     1812 2022-03-16 16:46:34.978011 torch-conduit-0.1.7/conduit/data/datasets/tabular/base.py
--rw-r--r--   0        0        0     1796 2022-03-16 16:46:34.978300 torch-conduit-0.1.7/conduit/data/datasets/tabular/dummy.py
--rw-r--r--   0        0        0    30558 2022-09-09 14:04:16.861844 torch-conduit-0.1.7/conduit/data/datasets/utils.py
--rw-r--r--   0        0        0      215 2022-12-16 16:33:37.764353 torch-conduit-0.1.7/conduit/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0     4889 2022-07-26 11:07:32.139056 torch-conduit-0.1.7/conduit/data/datasets/vision/base.py
--rw-r--r--   0        0        0     6255 2022-03-23 18:10:07.472632 torch-conduit-0.1.7/conduit/data/datasets/vision/camelyon17.py
--rw-r--r--   0        0        0     4975 2022-03-27 12:12:47.847163 torch-conduit-0.1.7/conduit/data/datasets/vision/celeba.py
--rw-r--r--   0        0        0     9826 2022-03-23 18:10:07.473450 torch-conduit-0.1.7/conduit/data/datasets/vision/cmnist.py
--rw-r--r--   0        0        0     1247 2022-03-23 18:10:07.473975 torch-conduit-0.1.7/conduit/data/datasets/vision/dummy.py
--rw-r--r--   0        0        0    12290 2022-03-23 18:10:07.474400 torch-conduit-0.1.7/conduit/data/datasets/vision/isic.py
--rw-r--r--   0        0        0     7315 2022-05-04 13:48:43.601508 torch-conduit-0.1.7/conduit/data/datasets/vision/nico.py
--rw-r--r--   0        0        0     7860 2022-12-16 16:33:37.764842 torch-conduit-0.1.7/conduit/data/datasets/vision/nih.py
--rw-r--r--   0        0        0     6482 2022-08-03 15:09:53.395631 torch-conduit-0.1.7/conduit/data/datasets/vision/pacs.py
--rw-r--r--   0        0        0     3937 2022-03-23 18:10:07.475205 torch-conduit-0.1.7/conduit/data/datasets/vision/ssrp.py
--rw-r--r--   0        0        0     3687 2022-12-16 16:33:37.765838 torch-conduit-0.1.7/conduit/data/datasets/vision/waterbirds.py
--rw-r--r--   0        0        0     8444 2022-05-24 11:32:38.832171 torch-conduit-0.1.7/conduit/data/datasets/wrappers.py
--rw-r--r--   0        0        0    18748 2022-09-09 14:04:16.862824 torch-conduit-0.1.7/conduit/data/structures.py
--rw-r--r--   0        0        0        0 2022-06-06 15:57:26.323043 torch-conduit-0.1.7/conduit/fair/__init__.py
--rw-r--r--   0        0        0       51 2022-03-16 16:46:34.982193 torch-conduit-0.1.7/conduit/fair/data/__init__.py
--rw-r--r--   0        0        0       68 2022-03-16 16:46:34.982442 torch-conduit-0.1.7/conduit/fair/data/datamodules/__init__.py
--rw-r--r--   0        0        0      214 2022-03-16 16:46:34.982689 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0      692 2022-12-16 14:08:00.925096 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/admissions.py
--rw-r--r--   0        0        0      814 2022-12-16 14:07:57.510142 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/adult.py
--rw-r--r--   0        0        0     6157 2022-12-16 14:07:55.022772 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/base.py
--rw-r--r--   0        0        0      625 2022-12-16 14:07:52.538374 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/compas.py
--rw-r--r--   0        0        0      645 2022-12-16 14:07:50.258668 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/credit.py
--rw-r--r--   0        0        0      642 2022-12-16 14:07:47.554572 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/crime.py
--rw-r--r--   0        0        0      606 2022-12-16 14:07:44.567227 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/german.py
--rw-r--r--   0        0        0      608 2022-12-16 14:07:41.777071 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/health.py
--rw-r--r--   0        0        0      573 2022-12-16 14:07:38.945731 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/law.py
--rw-r--r--   0        0        0      579 2022-12-16 14:07:36.080094 torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/sqf.py
--rw-r--r--   0        0        0        0 2022-03-16 16:46:34.984612 torch-conduit-0.1.7/conduit/fair/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0       66 2022-03-16 16:46:34.984868 torch-conduit-0.1.7/conduit/fair/data/datasets/__init__.py
--rw-r--r--   0        0        0      972 2022-03-16 16:46:34.985046 torch-conduit-0.1.7/conduit/fair/data/datasets/dummy.py
--rw-r--r--   0        0        0     2336 2022-11-02 16:54:44.380710 torch-conduit-0.1.7/conduit/fair/data/datasets/ethicml.py
--rw-r--r--   0        0        0        0 2022-03-16 16:46:34.985463 torch-conduit-0.1.7/conduit/fair/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0       20 2022-03-16 16:46:34.985743 torch-conduit-0.1.7/conduit/fair/losses/__init__.py
--rw-r--r--   0        0        0     1056 2022-03-16 16:46:34.985925 torch-conduit-0.1.7/conduit/fair/losses/loss.py
--rw-r--r--   0        0        0     5947 2022-03-18 11:18:28.149681 torch-conduit-0.1.7/conduit/hydra/conduit/data/datamodules/conf.py
--rw-r--r--   0        0        0     4101 2022-03-18 11:18:28.144297 torch-conduit-0.1.7/conduit/hydra/conduit/data/datasets/conf.py
--rw-r--r--   0        0        0     6455 2022-11-02 16:54:44.381080 torch-conduit-0.1.7/conduit/hydra/conduit/fair/data/datamodules/conf.py
--rw-r--r--   0        0        0     2928 2022-03-18 11:18:29.138410 torch-conduit-0.1.7/conduit/hydra/conduit/fair/models/conf.py
--rw-r--r--   0        0        0      660 2022-03-18 11:18:28.151850 torch-conduit-0.1.7/conduit/hydra/conduit/models/conf.py
--rw-r--r--   0        0        0     2486 2022-03-18 11:18:28.139906 torch-conduit-0.1.7/conduit/hydra/conduit/models/self_supervised/conf.py
--rw-r--r--   0        0        0      347 2022-08-05 10:04:29.903189 torch-conduit-0.1.7/conduit/logging.py
--rw-r--r--   0        0        0    17928 2022-11-02 16:54:44.381743 torch-conduit-0.1.7/conduit/metrics.py
--rw-r--r--   0        0        0       21 2022-06-06 15:57:26.323673 torch-conduit-0.1.7/conduit/models/__init__.py
--rw-r--r--   0        0        0    14920 2022-09-21 09:32:14.365459 torch-conduit-0.1.7/conduit/models/self_supervised/loss.py
--rw-r--r--   0        0        0     2477 2022-06-06 15:57:26.325386 torch-conduit-0.1.7/conduit/models/self_supervised/memory_bank.py
--rw-r--r--   0        0        0     1418 2022-03-28 15:36:51.051542 torch-conduit-0.1.7/conduit/models/utils.py
--rw-r--r--   0        0        0     8890 2022-08-05 10:04:29.903597 torch-conduit-0.1.7/conduit/progress.py
--rw-r--r--   0        0        0       64 2022-03-16 16:46:34.996268 torch-conduit-0.1.7/conduit/py.typed
--rw-r--r--   0        0        0     1723 2022-03-16 16:46:34.996444 torch-conduit-0.1.7/conduit/relay.py
--rw-r--r--   0        0        0      416 2022-03-16 16:46:34.996677 torch-conduit-0.1.7/conduit/structures.py
--rw-r--r--   0        0        0       65 2022-04-28 15:54:10.619574 torch-conduit-0.1.7/conduit/transforms/__init__.py
--rw-r--r--   0        0        0     3216 2022-05-24 11:32:38.833753 torch-conduit-0.1.7/conduit/transforms/audio.py
--rw-r--r--   0        0        0     2550 2022-06-06 15:57:26.325687 torch-conduit-0.1.7/conduit/transforms/fixmatch.py
--rw-r--r--   0        0        0     3271 2022-06-06 14:32:09.857788 torch-conduit-0.1.7/conduit/transforms/image.py
--rw-r--r--   0        0        0     8999 2022-06-06 15:57:26.326208 torch-conduit-0.1.7/conduit/transforms/multicrop.py
--rw-r--r--   0        0        0     6217 2022-03-16 16:46:34.997453 torch-conduit-0.1.7/conduit/transforms/tabular.py
--rw-r--r--   0        0        0     1526 2022-07-26 11:07:32.141369 torch-conduit-0.1.7/conduit/types.py
--rw-r--r--   0        0        0     4552 2022-12-16 16:36:47.171101 torch-conduit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 torch-conduit-0.1.7/setup.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 torch-conduit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-01-09 18:24:01.201254 torch_conduit-0.2.0/LICENSE
+-rw-r--r--   0        0        0      408 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/README.md
+-rw-r--r--   0        0        0       12 2022-12-18 12:46:23.375194 torch_conduit-0.2.0/conduit/__init__.py
+-rw-r--r--   0        0        0     1329 2022-12-19 15:56:41.671401 torch_conduit-0.2.0/conduit/conf/configen.yaml
+-rw-r--r--   0        0        0       51 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/__init__.py
+-rw-r--r--   0        0        0      208 2022-12-19 15:56:41.671401 torch_conduit-0.2.0/conduit/data/constants.py
+-rw-r--r--   0        0        0       20 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datamodules/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.247194 torch_conduit-0.2.0/conduit/data/datamodules/audio/__init__.py
+-rw-r--r--   0        0        0     2558 2023-03-22 19:05:02.482581 torch_conduit-0.2.0/conduit/data/datamodules/audio/base.py
+-rw-r--r--   0        0        0     2869 2022-12-19 15:56:41.671401 torch_conduit-0.2.0/conduit/data/datamodules/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    12126 2023-03-22 15:35:36.662964 torch_conduit-0.2.0/conduit/data/datamodules/base.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.255194 torch_conduit-0.2.0/conduit/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0     1091 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datamodules/tabular/dummy.py
+-rw-r--r--   0        0        0      156 2022-12-18 12:46:23.243194 torch_conduit-0.2.0/conduit/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0     3987 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datamodules/vision/base.py
+-rw-r--r--   0        0        0     2678 2022-12-19 15:56:41.671401 torch_conduit-0.2.0/conduit/data/datamodules/vision/camelyon17.py
+-rw-r--r--   0        0        0     2155 2022-12-19 15:56:41.671401 torch_conduit-0.2.0/conduit/data/datamodules/vision/celeba.py
+-rw-r--r--   0        0        0     3430 2023-02-01 11:04:32.428283 torch_conduit-0.2.0/conduit/data/datamodules/vision/cmnist.py
+-rw-r--r--   0        0        0     1145 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datamodules/vision/dummy.py
+-rw-r--r--   0        0        0     1976 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/data/datamodules/vision/nico.py
+-rw-r--r--   0        0        0     1647 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/data/datamodules/vision/pacs.py
+-rw-r--r--   0        0        0     2337 2023-02-02 17:36:21.303492 torch_conduit-0.2.0/conduit/data/datamodules/vision/waterbirds.py
+-rw-r--r--   0        0        0       65 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.295194 torch_conduit-0.2.0/conduit/data/datasets/audio/__init__.py
+-rw-r--r--   0        0        0     2798 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/data/datasets/audio/base.py
+-rw-r--r--   0        0        0    11276 2023-01-18 10:25:37.423919 torch_conduit-0.2.0/conduit/data/datasets/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    10725 2023-02-02 17:36:21.303492 torch_conduit-0.2.0/conduit/data/datasets/base.py
+-rw-r--r--   0        0        0       41 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/tabular/__init__.py
+-rw-r--r--   0        0        0     1811 2023-01-18 10:25:37.423919 torch_conduit-0.2.0/conduit/data/datasets/tabular/base.py
+-rw-r--r--   0        0        0     1832 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/tabular/dummy.py
+-rw-r--r--   0        0        0    27567 2023-03-28 14:48:18.044388 torch_conduit-0.2.0/conduit/data/datasets/utils.py
+-rw-r--r--   0        0        0      304 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0     4834 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/base.py
+-rw-r--r--   0        0        0     6351 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/camelyon17.py
+-rw-r--r--   0        0        0     5310 2023-02-25 16:39:35.362547 torch_conduit-0.2.0/conduit/data/datasets/vision/celeba.py
+-rw-r--r--   0        0        0     9862 2023-02-25 16:39:35.362547 torch_conduit-0.2.0/conduit/data/datasets/vision/cmnist.py
+-rw-r--r--   0        0        0     1131 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/dummy.py
+-rw-r--r--   0        0        0     8944 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/fmow.py
+-rw-r--r--   0        0        0    12403 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/isic.py
+-rw-r--r--   0        0        0     7475 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/iwildcam.py
+-rw-r--r--   0        0        0     7221 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/nico.py
+-rw-r--r--   0        0        0     7912 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/data/datasets/vision/nih.py
+-rw-r--r--   0        0        0     6291 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/pacs.py
+-rw-r--r--   0        0        0     3917 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/ssrp.py
+-rw-r--r--   0        0        0     3610 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/data/datasets/vision/utils.py
+-rw-r--r--   0        0        0       26 2023-02-02 17:36:21.303492 torch_conduit-0.2.0/conduit/data/datasets/vision/waterbirds/__init__.py
+-rw-r--r--   0        0        0     5094 2023-02-02 17:36:21.303492 torch_conduit-0.2.0/conduit/data/datasets/vision/waterbirds/waterbirds.py
+-rw-r--r--   0        0        0   156339 2023-02-02 17:36:21.303492 torch_conduit-0.2.0/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip
+-rw-r--r--   0        0        0     2998 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/vision/wrappers.py
+-rw-r--r--   0        0        0     5673 2023-01-19 16:12:52.451248 torch_conduit-0.2.0/conduit/data/datasets/wrappers.py
+-rw-r--r--   0        0        0    18277 2023-03-27 10:33:44.654089 torch_conduit-0.2.0/conduit/data/structures.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.359194 torch_conduit-0.2.0/conduit/fair/__init__.py
+-rw-r--r--   0        0        0       51 2022-12-18 12:46:23.343194 torch_conduit-0.2.0/conduit/fair/data/__init__.py
+-rw-r--r--   0        0        0       68 2022-12-18 12:46:23.343194 torch_conduit-0.2.0/conduit/fair/data/datamodules/__init__.py
+-rw-r--r--   0        0        0      214 2022-12-18 12:46:23.343194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0      692 2022-12-18 12:46:23.335194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/admissions.py
+-rw-r--r--   0        0        0      814 2022-12-18 12:46:23.335194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/adult.py
+-rw-r--r--   0        0        0     6015 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/base.py
+-rw-r--r--   0        0        0      625 2022-12-18 12:46:23.327194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/compas.py
+-rw-r--r--   0        0        0      645 2022-12-18 12:46:23.331194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/credit.py
+-rw-r--r--   0        0        0      642 2022-12-18 12:46:23.323194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/crime.py
+-rw-r--r--   0        0        0      606 2022-12-18 12:46:23.339194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/german.py
+-rw-r--r--   0        0        0      608 2022-12-18 12:46:23.323194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/health.py
+-rw-r--r--   0        0        0      573 2022-12-18 12:46:23.327194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/law.py
+-rw-r--r--   0        0        0      579 2022-12-18 12:46:23.331194 torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/sqf.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.319194 torch_conduit-0.2.0/conduit/fair/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0       66 2022-12-18 12:46:23.355194 torch_conduit-0.2.0/conduit/fair/data/datasets/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-19 16:39:10.546686 torch_conduit-0.2.0/conduit/fair/data/datasets/dummy.py
+-rw-r--r--   0        0        0     2336 2022-12-18 12:46:23.351194 torch_conduit-0.2.0/conduit/fair/data/datasets/ethicml.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.347194 torch_conduit-0.2.0/conduit/fair/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0       20 2022-12-18 12:46:23.359194 torch_conduit-0.2.0/conduit/fair/losses/__init__.py
+-rw-r--r--   0        0        0     1041 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/fair/losses/loss.py
+-rw-r--r--   0        0        0     5992 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/hydra/conduit/data/datamodules/conf.py
+-rw-r--r--   0        0        0     4195 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/hydra/conduit/data/datasets/conf.py
+-rw-r--r--   0        0        0     6455 2022-12-19 15:18:44.170868 torch_conduit-0.2.0/conduit/hydra/conduit/fair/data/datamodules/conf.py
+-rw-r--r--   0        0        0      457 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/hydra/conduit/models/self_supervised/loss/conf.py
+-rw-r--r--   0        0        0      399 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/hydra/conduit/models/self_supervised/memory_bank/conf.py
+-rw-r--r--   0        0        0      347 2022-12-18 12:46:23.375194 torch_conduit-0.2.0/conduit/logging.py
+-rw-r--r--   0        0        0    20901 2023-02-25 16:39:35.362547 torch_conduit-0.2.0/conduit/metrics.py
+-rw-r--r--   0        0        0       21 2022-12-18 12:46:23.383194 torch_conduit-0.2.0/conduit/models/__init__.py
+-rw-r--r--   0        0        0    14963 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/models/self_supervised/loss.py
+-rw-r--r--   0        0        0     2386 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/models/self_supervised/memory_bank.py
+-rw-r--r--   0        0        0     1425 2022-12-19 15:56:41.675401 torch_conduit-0.2.0/conduit/models/utils.py
+-rw-r--r--   0        0        0     9867 2023-04-17 20:52:30.804691 torch_conduit-0.2.0/conduit/progress.py
+-rw-r--r--   0        0        0       64 2022-01-09 18:24:01.201254 torch_conduit-0.2.0/conduit/py.typed
+-rw-r--r--   0        0        0      416 2022-12-18 12:46:23.319194 torch_conduit-0.2.0/conduit/structures.py
+-rw-r--r--   0        0        0       65 2022-12-18 12:46:23.371194 torch_conduit-0.2.0/conduit/transforms/__init__.py
+-rw-r--r--   0        0        0     3216 2022-12-18 12:46:23.371194 torch_conduit-0.2.0/conduit/transforms/audio.py
+-rw-r--r--   0        0        0     2490 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/transforms/fixmatch.py
+-rw-r--r--   0        0        0     3271 2022-12-18 12:46:23.363194 torch_conduit-0.2.0/conduit/transforms/image.py
+-rw-r--r--   0        0        0     8902 2023-02-01 11:04:32.432283 torch_conduit-0.2.0/conduit/transforms/multicrop.py
+-rw-r--r--   0        0        0     6014 2023-01-18 10:25:37.427919 torch_conduit-0.2.0/conduit/transforms/tabular.py
+-rw-r--r--   0        0        0     1583 2023-04-17 20:52:30.804691 torch_conduit-0.2.0/conduit/types.py
+-rw-r--r--   0        0        0     5650 2023-04-17 20:52:40.764756 torch_conduit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 torch_conduit-0.2.0/PKG-INFO
```

### Comparing `torch-conduit-0.1.7/LICENSE` & `torch_conduit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/conf/configen.yaml` & `torch_conduit-0.2.0/conduit/conf/configen.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -13,18 +13,20 @@
     # isort:skip_file
     # flake8: noqa
 
   module_path_pattern: "{{module_path}}/conf.py"
 
   # list of modules to generate configs for
   modules:
-    - name: conduit.models.self_supervised
+    - name: conduit.models.self_supervised.loss
       classes:
-        - MoCoV2
-        - DINO
+        - DecoupledContrastiveLoss
+    - name: conduit.models.self_supervised.memory_bank
+      classes:
+        - MemoryBank
     - name: conduit.data.datasets
       classes:
         - CelebA
         - ColoredMNIST
         - ISIC
         - NICO
         - SSRP
@@ -37,31 +39,18 @@
         - CelebADataModule
         - ColoredMNISTDataModule
         - NICODataModule
         - WaterbirdsDataModule
         - Camelyon17DataModule
         - EcoacousticsDataModule
 
-    - name: conduit.models
-      classes:
-        - ERMClassifier
-
     - name: conduit.fair.data.datamodules
       classes:
         - AdmissionsDataModule
         - AdultDataModule
         - CompasDataModule
         - CreditDataModule
         - CrimeDataModule
         - GermanDataModule
         - HealthDataModule
         - LawDataModule
         - SqfDataModule
-
-    - name: conduit.fair.models
-      classes:
-        - DANN
-        - ERMClassifierF
-        - FairMixup
-        - GPD
-        - KC
-        - LAFTR
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/audio/base.py` & `torch_conduit-0.2.0/conduit/data/datamodules/audio/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Base class for audio datasets."""
-from typing import Optional, TypeVar
+from typing import Optional, TypeVar, final
 
-import albumentations as A  # type: ignore
 import attr
-from ranzen.decorators import implements
 import torchaudio.transforms as T  # type: ignore
-from typing_extensions import final
+from typing_extensions import override
 
 from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datasets.base import I
 from conduit.data.datasets.utils import AudioTform
 from conduit.data.datasets.wrappers import AudioTransformer, InstanceWeightedDataset
 from conduit.data.structures import SizedDataset
 from conduit.types import Stage
@@ -17,30 +15,29 @@
 __all__ = ["CdtAudioDataModule"]
 
 D = TypeVar("D", bound=SizedDataset)
 
 
 @attr.define(kw_only=True)
 class CdtAudioDataModule(CdtDataModule[D, I]):
-
     root: str = attr.field(kw_only=False)
     _train_transforms: Optional[AudioTform] = None
     _test_transforms: Optional[AudioTform] = None
 
     @property
     @final
     def train_transforms(self) -> AudioTform:
         return (
             self._default_train_transforms
             if self._train_transforms is None
             else self._train_transforms
         )
 
     @train_transforms.setter
-    def train_transforms(self, transform: Optional[AudioTform]) -> None:  # type: ignore
+    def train_transforms(self, transform: Optional[AudioTform]) -> None:
         self._train_transforms = transform
         if isinstance(self._train_data, AudioTransformer):
             self._train_data.transform = transform
 
     @property
     @final
     def test_transforms(self) -> AudioTform:
@@ -48,30 +45,30 @@
             self._default_test_transforms
             if self._test_transforms is None
             else self._test_transforms
         )
 
     @test_transforms.setter
     @final
-    def test_transforms(self, transform: Optional[AudioTform]) -> None:  # type: ignore
+    def test_transforms(self, transform: Optional[AudioTform]) -> None:
         self._test_transforms = transform
         if isinstance(self._val_data, AudioTransformer):
             self._val_data.transform = transform
         if isinstance(self._test_data, AudioTransformer):
             self._test_data.transform = transform
 
     @property
     def _default_train_transforms(self) -> T.Spectrogram:
         return T.Spectrogram()
 
     @property
     def _default_test_transforms(self) -> T.Spectrogram:
         return T.Spectrogram()
 
-    @implements(CdtDataModule)
+    @override
     @final
     def _setup(self, stage: Optional[Stage] = None) -> None:
         train, val, test = self._get_splits()
         train = AudioTransformer(train, transform=self.train_transforms)
         if self.instance_weighting:
             train = InstanceWeightedDataset(train)
         self._train_data = train
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/audio/ecoacoustics.py` & `torch_conduit-0.2.0/conduit/data/datamodules/audio/ecoacoustics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Ecoacoustics data-module."""
 from typing import Any, List, Optional, Sequence
 
 import attr
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
 from torch.utils.data import Sampler
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datasets.audio.ecoacoustics import Ecoacoustics, SoundscapeAttr
 from conduit.data.datasets.utils import AudioTform, CdtDataLoader
 from conduit.data.structures import BinarySample, TernarySample, TrainValTestSplit
 from conduit.transforms.audio import Compose, Framing, LogMelSpectrogram
 
 from .base import CdtAudioDataModule
 
@@ -47,38 +45,38 @@
             pin_memory=self.pin_memory,
             drop_last=drop_last,
             persistent_workers=self.persist_workers,
             batch_sampler=batch_sampler,
             converter=self._batch_converter,
         )
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         Ecoacoustics(
             root=self.root,
             download=True,
             segment_len=self.segment_len,
             target_attrs=self.target_attrs,
         )
 
     @property
     def _default_transform(self) -> Compose:
         return Compose([LogMelSpectrogram(), Framing()])
 
-    @property  # type: ignore[misc]
-    @implements(CdtAudioDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> AudioTform:
         return self._default_transform
 
-    @property  # type: ignore[misc]
-    @implements(CdtAudioDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> AudioTform:
         return self._default_transform
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[Ecoacoustics]:
         all_data = Ecoacoustics(
             root=self.root,
             transform=None,  # Transform is applied in `CdtAudioDataModule._setup`
             segment_len=self.segment_len,
             target_attrs=self.target_attrs,
             sample_rate=self.sample_rate,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/base.py` & `torch_conduit-0.2.0/conduit/data/datamodules/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Base class from which all data-modules in conduit inherit."""
 from abc import abstractmethod
 import logging
-from typing import Generic, Optional, Sequence, Tuple, TypeVar, cast
+from typing import Generic, Optional, Sequence, Tuple, TypeVar, cast, final
 
 import attr
 import pytorch_lightning as pl
-from ranzen import implements
 from ranzen.torch import SequentialBatchSampler, StratifiedBatchSampler, TrainingMode
 from ranzen.torch.data import num_batches_per_epoch
 import torch
 from torch.utils.data import Sampler
-from typing_extensions import final
+from typing_extensions import override
 
 from conduit.data.datasets.base import CdtDataset
 from conduit.data.datasets.utils import (
     CdtDataLoader,
     extract_base_dataset,
     get_group_ids,
 )
@@ -62,15 +61,15 @@
 
     :param training_mode: Which mode to use for sampling with the train-dataloader. If `epoch` then
         the train-dataloader will be exhausted after a complete pass though the data. If `step` then
         samples will be drawn ad infinitum by the dataloader.
     """
 
     train_batch_size: int = 64
-    _eval_batch_size: Optional[int] = None
+    _eval_batch_size: Optional[int] = attr.field(alias="eval_batch_size", default=None)
     val_prop: float = 0.2
     test_prop: float = 0.2
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
@@ -163,17 +162,18 @@
 
         if self.stratified_sampling:
             group_ids = get_group_ids(self.train_data)
             num_groups = len(group_ids.unique())
             num_samples_per_group = batch_size // num_groups
             if batch_size % num_groups:
                 self.logger.info(
-                    f"For stratified sampling, the batch size must be a multiple of the number of groups."
-                    f"Since the batch size is not integer divisible by the number of groups ({num_groups}),"
-                    f"the batch size is being reduced to {num_samples_per_group * num_groups}."
+                    "For stratified sampling, the batch size must be a multiple of the number of"
+                    " groups.Since the batch size is not integer divisible by the number of groups"
+                    f" ({num_groups}),the batch size is being reduced to"
+                    f" {num_samples_per_group * num_groups}."
                 )
             batch_sampler = StratifiedBatchSampler(
                 group_ids=group_ids.squeeze().tolist(),
                 num_samples_per_group=num_samples_per_group,
                 shuffle=shuffle,
                 base_sampler="sequential",
                 training_mode=self.training_mode,
@@ -187,19 +187,19 @@
                 training_mode=self.training_mode,
                 drop_last=drop_last,
             )
         return self.make_dataloader(
             ds=self.train_data, batch_size=self.train_batch_size, batch_sampler=batch_sampler
         )
 
-    @implements(pl.LightningDataModule)
+    @override
     def val_dataloader(self) -> CdtDataLoader[I]:
         return self.make_dataloader(batch_size=self.eval_batch_size, ds=self.val_data)
 
-    @implements(pl.LightningDataModule)
+    @override
     def test_dataloader(self) -> CdtDataLoader[I]:
         return self.make_dataloader(batch_size=self.eval_batch_size, ds=self.test_data)
 
     @property
     def dim_x(self) -> Tuple[int, ...]:
         """
         Returns the dimensions of the first input (x).
@@ -218,18 +218,18 @@
         :returns: Tuple containing the dimensions of the (first) input.
         """
         return self.dim_x
 
     @final
     def _num_samples(self, dataset: D) -> int:
         if hasattr(dataset, "__len__"):
-            return len(dataset)  # type: ignore
+            return len(dataset)
         raise AttributeError(
-            f"Number of samples cannot be determined as dataset of type '{dataset.__class__.__name__}' "
-            "has no '__len__' attribute defined."
+            "Number of samples cannot be determined as dataset of type"
+            f" '{dataset.__class__.__name__}' has no '__len__' attribute defined."
         )
 
     @property
     @final
     def num_train_samples(self) -> int:
         return self._num_samples(self.train_data)
 
@@ -326,14 +326,14 @@
         self._val_data_base = extract_base_dataset(
             dataset=self.val_data, return_subset_indices=False
         )
         self._test_data_base = extract_base_dataset(
             dataset=self.test_data, return_subset_indices=False
         )
 
-    @implements(pl.LightningDataModule)
+    @override
     @final
     def setup(self, stage: Optional[Stage] = None, force_reset: bool = False) -> None:
         # Only perform the setup if it hasn't already been done
         if force_reset or (not self.is_set_up):
             self._setup(stage=stage)
             self._post_setup()
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/tabular/dummy.py` & `torch_conduit-0.2.0/conduit/data/datamodules/tabular/dummy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Optional
 
 import attr
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data import CdtDataModule, TrainValTestSplit
-from conduit.data.datasets.tabular.dummy import RandomTabularDataset
+from conduit.data import TrainValTestSplit
+from conduit.data.datamodules import CdtDataModule
+from conduit.data.datasets.tabular import RandomTabularDataset
 
 
 @attr.define(kw_only=True)
 class DummyTabularDataModule(CdtDataModule):
     num_samples: int
     num_disc_features: int
     num_cont_features: int
     seed: int = 8
     s_card: Optional[int] = None
     y_card: Optional[int] = None
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[RandomTabularDataset]:
         # Split the data randomly according to val- and test-prop
         data = RandomTabularDataset(
             num_cont_features=self.num_cont_features,
             num_disc_features=self.num_disc_features,
             num_samples=self.num_samples,
             seed=self.seed,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/base.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Base class for vision datasets."""
 from pathlib import Path
 from typing import List, Optional, TypeVar, Union
 
 import albumentations as A  # type: ignore
 from albumentations.pytorch import ToTensorV2  # type: ignore
 import attr
-from ranzen import implements
-from typing_extensions import final
+from typing_extensions import final, override
 
 from conduit.data.constants import IMAGENET_STATS
 from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datasets.base import I
-from conduit.data.datasets.utils import AlbumentationsTform, ImageTform
-from conduit.data.datasets.wrappers import ImageTransformer, InstanceWeightedDataset
+from conduit.data.datasets.vision import (
+    AlbumentationsTform,
+    ImageTform,
+    ImageTransformer,
+)
+from conduit.data.datasets.wrappers import InstanceWeightedDataset
 from conduit.data.structures import ImageSize, MeanStd, SizedDataset
 from conduit.types import Stage
 
 __all__ = ["CdtVisionDataModule"]
 
 D = TypeVar("D", bound=SizedDataset)
 
 
 @attr.define(kw_only=True)
 class CdtVisionDataModule(CdtDataModule[D, I]):
-
     root: Union[str, Path] = attr.field(kw_only=False)
     _train_transforms: Optional[ImageTform] = None
     _test_transforms: Optional[ImageTform] = None
     norm_values: Optional[MeanStd] = attr.field(default=IMAGENET_STATS, init=False)
 
     @property
     @final
@@ -35,15 +37,15 @@
         return (
             self._default_train_transforms
             if self._train_transforms is None
             else self._train_transforms
         )
 
     @train_transforms.setter
-    def train_transforms(self, transform: Optional[ImageTform]) -> None:  # type: ignore
+    def train_transforms(self, transform: Optional[ImageTform]) -> None:
         self._train_transforms = transform
         if isinstance(self._train_data, ImageTransformer):
             self._train_data.transform = transform
 
     @property
     @final
     def test_transforms(self) -> ImageTform:
@@ -51,15 +53,15 @@
             self._default_test_transforms
             if self._test_transforms is None
             else self._test_transforms
         )
 
     @test_transforms.setter
     @final
-    def test_transforms(self, transform: Optional[ImageTform]) -> None:  # type: ignore
+    def test_transforms(self, transform: Optional[ImageTform]) -> None:
         self._test_transforms = transform
         if isinstance(self._val_data, ImageTransformer):
             self._val_data.transform = transform
         if isinstance(self._test_data, ImageTransformer):
             self._test_data.transform = transform
 
     @property
@@ -72,15 +74,15 @@
                     mean=self.norm_values.mean, std=self.norm_values.std, max_pixel_value=1.0
                 )
             )
         transform_ls.append(ToTensorV2())
         return A.Compose(transform_ls)
 
     @property
-    @implements(CdtDataModule)
+    @override
     def dim_x(self) -> ImageSize:
         """
         Returns the dimensions of the first input (x).
 
         :returns: ImageSize object containing the dimensions (C, H, W) of the (first) input.
         """
         return ImageSize(*super().dim_x)
@@ -96,15 +98,15 @@
     def _default_test_transforms(self) -> A.Compose:
         transform_ls: List[AlbumentationsTform] = [A.ToFloat()]
         if self.norm_values is not None:
             transform_ls.append(A.Normalize(mean=self.norm_values.mean, std=self.norm_values.std))
         transform_ls.append(ToTensorV2())
         return A.Compose(transform_ls)
 
-    @implements(CdtDataModule)
+    @override
     def _setup(self, stage: Optional[Stage] = None) -> None:
         train, val, test = self._get_splits()
         train = ImageTransformer(train, transform=self.train_transforms)
         if self.instance_weighting:
             train = InstanceWeightedDataset(train)
         self._train_data = train
         self._val_data = ImageTransformer(val, transform=self.test_transforms)
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/camelyon17.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/camelyon17.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Camelyon17 data-module."""
 from typing import Any
 
 import albumentations as A  # type: ignore
 import attr
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.camelyon17 import (
     Camelyon17,
     Camelyon17Attr,
     Camelyon17Split,
     Camelyon17SplitScheme,
     SampleType,
@@ -21,52 +19,52 @@
 
 
 @attr.define(kw_only=True)
 class Camelyon17DataModule(CdtVisionDataModule[Camelyon17, SampleType]):
     """Data-module for the Camelyon17 dataset."""
 
     image_size: int = 96
-    superclass: Camelyon17Attr = Camelyon17Attr.tumor
-    subclass: Camelyon17Attr = Camelyon17Attr.center
+    superclass: Camelyon17Attr = Camelyon17Attr.TUMOR
+    subclass: Camelyon17Attr = Camelyon17Attr.CENTER
     use_predefined_splits: bool = False
-    split_scheme: Camelyon17SplitScheme = Camelyon17SplitScheme.official
+    split_scheme: Camelyon17SplitScheme = Camelyon17SplitScheme.OFFICIAL
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         Camelyon17(root=self.root, download=True)
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> A.Compose:
         base_transforms = A.Compose(
             [
                 A.Resize(self.image_size, self.image_size),
                 A.CenterCrop(self.image_size, self.image_size),
                 A.HorizontalFlip(),
                 A.RandomCrop(self.image_size, self.image_size),
             ]
         )
         normalization = super()._default_train_transforms
 
         return A.Compose([base_transforms, normalization])
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> A.Compose:
         base_transforms = A.Compose(
             [
                 A.Resize(self.image_size, self.image_size),
                 A.CenterCrop(self.image_size, self.image_size),
             ]
         )
         normalization = super()._default_train_transforms
 
         return A.Compose([base_transforms, normalization])
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[Camelyon17]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
                 Camelyon17(root=self.root, split=split, split_scheme=self.split_scheme)
                 for split in Camelyon17Split
             )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/celeba.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/celeba.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """CelebA data-module."""
 from typing import Any
 
 import albumentations as A  # type: ignore
 import attr
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.celeba import (
     CelebA,
     CelebASplit,
     CelebAttr,
     SampleType,
 )
@@ -20,40 +18,40 @@
 
 
 @attr.define(kw_only=True)
 class CelebADataModule(CdtVisionDataModule[CelebA, SampleType]):
     """Data-module for the CelebA dataset."""
 
     image_size: int = 224
-    superclass: CelebAttr = CelebAttr.Smiling
-    subclass: CelebAttr = CelebAttr.Male
+    superclass: CelebAttr = CelebAttr.SMILING
+    subclass: CelebAttr = CelebAttr.MALE
     use_predefined_splits: bool = False
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         CelebA(root=self.root, download=True)
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> A.Compose:
         base_transforms = A.Compose(
             [
                 A.Resize(self.image_size, self.image_size),
                 A.CenterCrop(self.image_size, self.image_size),
             ]
         )
         normalization = super()._default_train_transforms
         return A.Compose([base_transforms, normalization])
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[CelebA]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
                 CelebA(root=self.root, superclass=self.superclass, transform=None, split=split)
                 for split in CelebASplit
             )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/cmnist.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/cmnist.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 from functools import partial
 from typing import Any, Dict, List, Optional
 
 import albumentations as A  # type: ignore
 from albumentations.pytorch.transforms import ToTensorV2  # type: ignore
 import attr
 import numpy as np
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
 from torchvision.datasets import MNIST  # type: ignore
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.vision.cmnist import (
     ColoredMNIST,
     ColoredMNISTSplit,
     SampleType,
 )
 from conduit.data.structures import MeanStd, TrainValTestSplit
@@ -35,36 +33,36 @@
     scale: float = 0.2
     correlation: float = 1.0
     binarize: bool = False
     greyscale: bool = False
     background: bool = False
     black: bool = True
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> A.Compose:
         transforms = [A.Compose([A.Resize(self.image_size, self.image_size)])]
         if self.norm_values is not None:
             normalization = A.Compose(
                 [A.Normalize(mean=self.norm_values.mean, std=self.norm_values.std), ToTensorV2()]
             )
-            transforms.append(normalization)  # type: ignore
+            transforms.append(normalization)
         return A.Compose(transforms)
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         MNIST(root=str(self.root), download=True, train=True)
         MNIST(root=str(self.root), download=True, train=False)
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[ColoredMNIST]:
         # TODO: Add more sophisticated (e.g. biased) splits
         fact_func = partial(
             ColoredMNIST,
             root=self.root,
             background=self.background,
             black=self.black,
@@ -73,16 +71,16 @@
             colors=self.colors,
             num_colors=self.num_colors,
             label_map=self.label_map,
         )
         # Use the predefined train and test splits, sampling the val split
         # randomly from the train split
         if self.use_predefined_splits:
-            train_data = fact_func(split=ColoredMNISTSplit.train)
-            test_data = fact_func(split=ColoredMNISTSplit.test)
+            train_data = fact_func(split=ColoredMNISTSplit.TRAIN)
+            test_data = fact_func(split=ColoredMNISTSplit.TEST)
             val_data, train_data = train_data.random_split(props=self.val_prop)
         else:
             # Split the data randomly according to val- and test-prop
             train_data = fact_func(split=None)
             val_data, test_data, train_data = train_data.random_split(
                 props=(self.val_prop, self.test_prop), seed=self.seed
             )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/dummy.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/dummy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Dummy data-module."""
 import attr
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data import CdtDataModule, CdtVisionDataModule, TrainValTestSplit
+from conduit.data import TrainValTestSplit
+from conduit.data.datamodules.vision import CdtVisionDataModule
 from conduit.data.datasets.vision.dummy import DummyVisionDataset, SampleType
 
 
 @attr.define(kw_only=True)
 class DummyVisionDataModule(CdtVisionDataModule[DummyVisionDataset, SampleType]):
     num_samples: int = 1_000
     seed: int = 8
@@ -14,15 +15,15 @@
     height: int = 32
     width: int = 32
     channels: int = 3
     batch_size: int = 32
     s_card: int = 2
     y_card: int = 2
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[DummyVisionDataset]:
         # Split the data randomly according to val- and test-prop
         data = DummyVisionDataset(
             channels=self.channels,
             height=self.height,
             width=self.width,
             num_samples=self.num_samples,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/nico.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/nico.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 """NICO data-module."""
 from typing import Any, Optional
 
 import albumentations as A  # type: ignore
 import attr
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
 from conduit.data.datasets.utils import stratified_split
 from conduit.data.datasets.vision.nico import NICO, NicoSuperclass, SampleType
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["NICODataModule"]
 
 
 @attr.define(kw_only=True)
 class NICODataModule(CdtVisionDataModule[NICO, SampleType]):
     """Data-module for the NICO dataset."""
 
     image_size: int = 224
     class_train_props: Optional[dict] = None
-    superclass: NicoSuperclass = NicoSuperclass.animals
+    superclass: NicoSuperclass = NicoSuperclass.ANIMALS
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> A.Compose:
         base_transforms = A.Compose(
             [
                 A.Resize(self.image_size, self.image_size),
                 A.CenterCrop(self.image_size, self.image_size),
             ]
         )
         normalization = super()._default_train_transforms
         return A.Compose([base_transforms, normalization])
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         NICO(root=self.root, download=True)
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[NICO]:
         all_data = NICO(root=self.root, superclass=self.superclass, transform=None)
         train_val_prop = 1 - self.test_prop
         train_val_data, test_data = stratified_split(
             all_data,
             default_train_prop=train_val_prop,
             train_props=self.class_train_props,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datamodules/vision/waterbirds.py` & `torch_conduit-0.2.0/conduit/data/datamodules/vision/waterbirds.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 """Waterbirds data-module."""
 from typing import Any
 
 import albumentations as A  # type: ignore
 import attr
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
+from typing_extensions import override
 
-from conduit.data.datamodules.base import CdtDataModule
 from conduit.data.datamodules.vision.base import CdtVisionDataModule
-from conduit.data.datasets.vision.waterbirds import (
-    SampleType,
-    Waterbirds,
-    WaterbirdsSplit,
-)
+from conduit.data.datasets.vision.waterbirds import Waterbirds
 from conduit.data.structures import TrainValTestSplit
 
 __all__ = ["WaterbirdsDataModule"]
 
 
 @attr.define(kw_only=True)
-class WaterbirdsDataModule(CdtVisionDataModule[Waterbirds, SampleType]):
+class WaterbirdsDataModule(CdtVisionDataModule[Waterbirds, Waterbirds.SampleType]):
     """Data-module for the Waterbirds dataset."""
 
     image_size: int = 224
     use_predefined_splits: bool = False
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         Waterbirds(root=self.root, download=True)
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_train_transforms(self) -> A.Compose:
         # We use the transoform pipeline described in https://arxiv.org/abs/2008.06775
         # rather than that described in the paper in which the dataset was first introduced
         # (Sagawa et al); these differ in in the respect that the latter center-crops the images
         # before resizing - not doing so makes the task more difficult due to the background
         # (serving as a spurious attribute) being more prominent.
         base_transforms = A.Compose(
             [
                 A.Resize(self.image_size, self.image_size),
             ]
         )
         normalization = super()._default_train_transforms
         return A.Compose([base_transforms, normalization])
 
-    @property  # type: ignore[misc]
-    @implements(CdtVisionDataModule)
+    @property
+    @override
     def _default_test_transforms(self) -> A.Compose:
         return self._default_train_transforms
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[Waterbirds]:
         # Split the data according to the pre-defined split indices
         if self.use_predefined_splits:
             train_data, val_data, test_data = (
-                Waterbirds(root=self.root, split=split) for split in WaterbirdsSplit
+                Waterbirds(root=self.root, split=split) for split in Waterbirds.Split
             )
         # Split the data randomly according to test- and val-prop
         else:
             all_data = Waterbirds(root=self.root, transform=None)
             val_data, test_data, train_data = all_data.random_split(
                 props=(self.val_prop, self.test_prop), seed=self.seed
             )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/audio/base.py` & `torch_conduit-0.2.0/conduit/data/datasets/audio/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import List, Optional, Union, overload
 
 import numpy as np
 import numpy.typing as npt
-from ranzen import implements
 import torch
 from torch import Tensor
 import torchaudio  # type: ignore
+from typing_extensions import override
 
 from conduit.data.datasets.base import CdtDataset, I, S, Y
 from conduit.data.datasets.utils import (
     AudioLoadingBackend,
     AudioTform,
     apply_audio_transform,
     infer_al_backend,
@@ -73,13 +73,13 @@
     def _sample_x(self, index: int, *, coerce_to_tensor: bool = ...) -> Tensor:
         ...
 
     @overload
     def _sample_x(self, index: List[int], *, coerce_to_tensor: bool = ...) -> List[Tensor]:
         ...
 
-    @implements(CdtDataset)
+    @override
     def _sample_x(
         self, index: IndexType, *, coerce_to_tensor: bool = False
     ) -> Union[Tensor, List[Tensor]]:
         waveform = self.load_sample(index)
         return apply_audio_transform(waveform, transform=None)
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/audio/ecoacoustics.py` & `torch_conduit-0.2.0/conduit/data/datasets/audio/ecoacoustics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 """Ecoacostics dataset provided A. Eldridge et al.
     Alice Eldridge, Paola Moscoso, Patrice Guyot, & Mika Peck. (2018).
     Data for "Sounding out Ecoacoustic Metrics: Avian species richness
     is predicted by acoustic indices in temperate but not tropical
     habitats" (Final) [Data set].
     Zenodo. https://doi.org/10.5281/zenodo.1255218
 """
-from enum import Enum, auto
+from enum import auto
 import math
 from pathlib import Path
 import shutil
-from typing import ClassVar, List, Optional, Tuple, Union, cast
+from typing import ClassVar, Final, List, Optional, Tuple, Union
 import zipfile
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_categorical_dtype, is_object_dtype
-from ranzen import parsable
-from ranzen.decorators import enum_name_str, implements
-from ranzen.misc import str_to_enum
+from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
 import torchaudio  # type: ignore
-from tqdm import tqdm  # type: ignore
-from typing_extensions import Final, TypeAlias
+from tqdm import tqdm
+from typing_extensions import TypeAlias, override
 
 from conduit.data.datasets.audio.base import CdtAudioDataset
 from conduit.data.datasets.utils import AudioTform, UrlFileInfo, download_from_url
 from conduit.data.structures import TernarySample
 
-__all__ = [
-    "Ecoacoustics",
-    "SoundscapeAttr",
-]
+__all__ = ["Ecoacoustics", "SoundscapeAttr"]
 
 
-@enum_name_str
-class SoundscapeAttr(Enum):
-    habitat = auto()
-    site = auto()
-    time = auto()
-    NN = auto()
-    N0 = auto()
+class SoundscapeAttr(StrEnum):
+    HABITAT = auto()
+    SITE = auto()
+    TIME = auto()
+    NN = "NN"
+    N0 = "N0"
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class Ecoacoustics(CdtAudioDataset[SampleType, Tensor, Tensor]):
     """Dataset for audio data collected in various geographic locations."""
@@ -94,17 +88,15 @@
         self.labels_dir = self.base_dir / self._INDICES_DIR / self._INDICES_DIR
         self.sample_rate = sample_rate  # set prior to segment length
         self.segment_len = segment_len
         self._metadata_path = self.base_dir / self._METADATA_FILENAME
         self.ec_labels_path = self.labels_dir / self._EC_LABELS_FILENAME
         self.uk_labels_path = self.labels_dir / self._UK_LABELS_FILENAME
         # map provided attributes (as string or enum) to permitted attributes (as strings)
-        self.target_attrs = [
-            str_to_enum(str_=elem, enum=SoundscapeAttr).name for elem in target_attrs
-        ]
+        self.target_attrs = [str(SoundscapeAttr(elem)) for elem in target_attrs]
 
         if self.download:
             self._download_files()
         self._check_files()
 
         # Extract labels from indices files.
         if not self._metadata_path.exists():
@@ -173,16 +165,16 @@
         # Create necessary directories if they don't already exist.
         self.base_dir.mkdir(parents=True, exist_ok=True)
 
         for finfo in self._FILE_INFO:
             download_from_url(
                 file_info=finfo, root=self.base_dir, logger=self.logger, remove_finished=True
             )
-        if (self.base_dir / "__MACOSX").exists():
-            shutil.rmtree(self.base_dir / "__MACOSX")
+        if (macosx_dir := self.base_dir / "__MACOSX").exists():
+            shutil.rmtree(macosx_dir)
 
     def _extract_metadata(self) -> None:
         """Extract information such as labels from relevant csv files, combining them along with
         information on processed files to produce a master file."""
 
         self.logger.info("Extracting metadata.")
         # Process the metadata for samples from Ecuador.
@@ -190,15 +182,15 @@
         ec_labels["filePath"] = "EC_BIRD/" + ec_labels["fileName"]
         # Process the metadata for samples from the UK.
         uk_labels = pd.read_csv(self.uk_labels_path, encoding="ISO-8859-1")
         # Some waveforms use full names for location i.e. BALMER and KNEPP, change indices file to do the same.
         uk_labels.replace(regex={"BA-": "BALMER-", "KN-": "KNEPP-"}, inplace=True)
         uk_labels["filePath"] = "UK_BIRD/" + uk_labels["fileName"]
 
-        metadata = cast(pd.DataFrame, pd.concat([uk_labels, ec_labels]))
+        metadata = pd.concat([uk_labels, ec_labels])
         metadata = metadata[[(self.base_dir / fp).exists() for fp in metadata["filePath"]]]
         # metadata = self._label_encode_metadata(metadata)
         metadata.to_csv(self._metadata_path, index=False)
 
     def _preprocess_files(self) -> None:
         """
         Segment the waveform files based on :py:attr:`segment_len` and cache the file-segments.
@@ -215,29 +207,33 @@
             waveform, sr = torchaudio.load(path)  # type: ignore
             audio_len = waveform.size(-1) / sr
             frac_remainder, num_segments = math.modf(audio_len / self.segment_len)
             num_segments = int(num_segments)
 
             if frac_remainder >= 0.5:
                 self.logger.debug(
-                    f"Length of audio file '{path.resolve()}' is not integer-divisible by "
-                    f"{self.segment_len}: terminally zero-padding the file along the "
-                    f"time-axis to compensate.",
+                    (
+                        f"Length of audio file '{path.resolve()}' is not integer-divisible by "
+                        f"{self.segment_len}: terminally zero-padding the file along the "
+                        "time-axis to compensate."
+                    ),
                 )
                 padding = torch.zeros(
                     waveform.size(0),
                     int((self.segment_len - (frac_remainder * self.segment_len)) * sr),
                 )
                 waveform = torch.cat((waveform, padding), dim=-1)
                 num_segments += 1
             if 0 < frac_remainder < 0.5:
                 self.logger.debug(
-                    f"Length of audio file '{path.resolve()}' is not integer-divisible by "
-                    f"{self.segment_len} and not of sufficient length to be padded "
-                    f"(fractional remainder must be greater than 0.5): discarding terminal segment.",
+                    (
+                        f"Length of audio file '{path.resolve()}' is not integer-divisible by"
+                        f" {self.segment_len} and not of sufficient length to be padded (fractional"
+                        " remainder must be greater than 0.5): discarding terminal segment."
+                    ),
                 )
                 waveform = waveform[:, : int(num_segments * self.segment_len * sr)]
 
             waveform_segments = waveform.chunk(chunks=num_segments, dim=-1)
             for seg_idx, segment in enumerate(waveform_segments):
                 segment_filename = f"{waveform_filename}_{seg_idx}.wav"
                 segment_filepath = processed_audio_dir / segment_filename
@@ -250,15 +246,15 @@
                     (waveform_filename, str(segment_filepath.relative_to(self.base_dir)))
                 )
 
         pd.DataFrame(segment_filenames, columns=["fileName", "filePath"]).to_csv(
             processed_audio_dir / "filepaths.csv", index=False
         )
 
-    @implements(CdtAudioDataset)
+    @override
     def load_sample(self, index: int) -> Tensor:
         path = self.audio_dir / self.x[index]
 
         # get metadata first
         metadata = torchaudio.info(path)  # type: ignore
 
         # compute number of frames to take with the real sample rate
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/base.py` & `torch_conduit-0.2.0/conduit/data/datasets/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     cast,
     final,
     overload,
 )
 
 import numpy as np
 import numpy.typing as npt
-from ranzen import implements
 from ranzen.misc import gcopy
 import torch
 from torch import Tensor
-from typing_extensions import Self
+from typing_extensions import Self, override
 
 from conduit.data.structures import (
     BinarySample,
     LoadedData,
     NamedSample,
     SizedDataset,
     SubgroupSample,
     TargetData,
     TernarySample,
     UnloadedData,
 )
 from conduit.logging import init_logger
+from conduit.metrics import merge_indices
 from conduit.types import IndexType
 
 __all__ = ["CdtDataset", "I", "S", "X", "Y"]
 
 X = TypeVar("X", bound=UnloadedData)
 S = TypeVar("S", bound=Optional[Tensor])
 Y = TypeVar("Y", bound=Optional[Tensor])
@@ -50,16 +50,16 @@
         self, *, x: X, y: Optional[TargetData] = None, s: Optional[TargetData] = None
     ) -> None:
         self.x = x
         if isinstance(y, np.ndarray):
             y = torch.as_tensor(y)
         if isinstance(s, np.ndarray):
             s = torch.as_tensor(s)
-        self.y: Y = y if y is None else y.squeeze()
-        self.s: S = s if s is None else s.squeeze()
+        self.y = cast(Y, y if y is None else y.squeeze())
+        self.s = cast(S, s if s is None else s.squeeze())
 
         self._dim_x: Optional[torch.Size] = None
         self._dim_s: Optional[torch.Size] = None
         self._dim_y: Optional[torch.Size] = None
         self._card_y: Optional[int] = None
         self._card_s: Optional[int] = None
 
@@ -163,29 +163,50 @@
             raise AttributeError(
                 f"'{cls_name}.card_s' cannot be determined as '{cls_name}.s' is 'None'"
             )
         if self._card_s is None:
             self._card_s = len(self.s.unique())
         return self._card_s
 
+    @property
+    @final
+    def groups(
+        self,
+    ) -> Tensor:
+        valid_s = (self.s is not None) and (self.s.dtype is torch.long)
+        valid_y = (self.y is not None) and (self.y.dtype is torch.long)
+        if not valid_y and not valid_s:
+            raise AttributeError(
+                "Unable to compute group ids for dataset because 'y' and 's' are both 'None' or are"
+                "not of dtype `torch.long`."
+            )
+        indices = []
+        # 'merge_indices' takes the last element of the 'indices' argument as the seed
+        # for the merged index set -- for consistency we use the 'y' label as the seed
+        # such that the binary version of merge_indices produces the bijective mapping
+        # g <- y * card(s) + s.
+        if valid_s:
+            indices.append(cast(Tensor, self.s))
+        if valid_y:
+            indices.append(cast(Tensor, self.y))
+        return merge_indices(*indices, return_cardinalities=False)
+
     def subset(
         self: Self,
         indices: Union[List[int], npt.NDArray[np.uint64], Tensor, slice],
         *,
         deep: bool = False,
     ) -> Self:
         """Create a subset of the dataset from the given indices.
 
-        :param indices: The sample-indices from which to create the subset.
-        In the case of being a numpy array or tensor, said array or tensor
-        must be 0- or 1-dimensional.
-
-        :param deep: Whether to create a copy of the underlying dataset as
-        a basis for the subset. If False then the data of the subset will be
-        a view of original dataset's data.
+        :param indices: The sample-indices from which to create the subset. In the case of being a
+            numpy array or tensor, said array or tensor must be 0- or 1-dimensional.
+
+        :param deep: Whether to create a copy of the underlying dataset as a basis for the subset.
+            If False then the data of the subset will be a view of original dataset's data.
 
         :returns: A subset of the dataset from the given indices.
         """
         # lazily import make_subset to prevent it being a circular import
         from conduit.data.datasets.utils import make_subset
 
         return make_subset(dataset=self, indices=indices, deep=deep)
@@ -219,48 +240,49 @@
         deep: bool = False,
         as_indices: bool = False,
         seed: Optional[int] = None,
     ) -> Union[List[Self], List[List[int]]]:
         """Randomly split the dataset into subsets according to the given proportions.
 
         :param props: The fractional size of each subset into which to randomly split the data.
-        Elements must be non-negative and sum to 1 or less; if less then the size of the final
-        split will be computed by complement.
+            Elements must be non-negative and sum to 1 or less; if less then the size of the final
+            split will be computed by complement.
 
-        :param deep: Whether to create a copy of the underlying dataset as
-        a basis for the random subsets. If False then the data of the subsets will be
-        views of original dataset's data.
+        :param deep: Whether to create a copy of the underlying dataset as a basis for the random
+            subsets. If False then the data of the subsets will be views of original dataset's data.
 
         :param as_indices: Whether to return the raw train/test indices instead of subsets of the
-        dataset constructed from them.
+            dataset constructed from them.
 
         :param seed: PRNG seed to use for splitting the data.
 
         :returns: Random subsets of the data of the requested proportions.
         """
         # lazily import ``random_split`` to prevent it from being a circular import
         from conduit.data.datasets.utils import random_split
 
         return random_split(self, props=props, deep=deep, seed=seed, as_indices=as_indices)
 
     @overload
-    def cat(self: Self, other: Self, *, inplace: Literal[True] = ..., deep: bool = False) -> None:
+    def cat(self, other: Self, *, inplace: Literal[True], deep: bool = ...) -> None:
         ...
 
     @overload
-    def cat(self: Self, other: Self, *, inplace: Literal[False] = ..., deep: bool = False) -> Self:
+    def cat(self, other: Self, *, inplace: Literal[False] = ..., deep: bool = ...) -> Self:
         ...
 
-    def cat(
-        self: Self, other: Self, *, inplace: bool = False, deep: bool = False
-    ) -> Optional[Self]:
-        """
-        Concatenate this ``self`` with another dataset of the same type.
+    @overload
+    def cat(self, other: Self, *, inplace: bool = ..., deep: bool = ...) -> Optional[Self]:
+        ...
+
+    def cat(self, other: Self, *, inplace: bool = False, deep: bool = False) -> Optional[Self]:
+        """Concatenate this ``self`` with another dataset of the same type.
 
-        :parma other: Other dataset to concatenate with this instance
+        :param other: Other dataset to concatenate with this instance
+        :param inplace: Whether to concatenate in place.
         :param deep: Whether to create a deep copy of this dataset as the basis for the superset.
 
         :returns: A concatenation of ``self`` with ``other``.
 
         .. note::
             All data-independent attributes will be inherited from ``self``.
         """
@@ -274,30 +296,29 @@
             superset.s = torch.cat([superset.s, other.s], dim=0)
         if (superset.y is not None) and (other.y is not None):
             superset.y = torch.cat([superset.y, other.y], dim=0)
 
         if not inplace:
             return superset
 
-    @implements(SizedDataset)
-    @final
+    @override
     def __getitem__(self: Self, index: IndexType) -> I:
         x = self._sample_x(index, coerce_to_tensor=False)
         y = self._sample_y(index)
         s = self._sample_s(index)
         # Fetch the appropriate 'Sample' class
         if y is None:
             sample = NamedSample(x=x) if s is None else SubgroupSample(x=x, s=s)
         elif s is None:
             sample = BinarySample(x=x, y=y)
         else:
             sample = TernarySample(x=x, y=y, s=s)
         return sample  # type: ignore
 
-    @implements(SizedDataset)
+    @override
     def __len__(self) -> int:
         return len(self.x)
 
     def __iadd__(self, other: Self) -> Self:
         self.cat(other, inplace=True, deep=False)
         return self
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/tabular/base.py` & `torch_conduit-0.2.0/conduit/data/datasets/tabular/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from conduit.data.structures import TargetData
 from conduit.transforms.tabular import TabularTransform
 
 __all__ = ["CdtTabularDataset"]
 
 
 class CdtTabularDataset(CdtDataset):
-
     x: Tensor
 
     def __init__(
         self,
         *,
         x: Union[Tensor, npt.NDArray[np.floating], npt.NDArray[np.integer]],
         y: Optional[TargetData] = None,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/tabular/dummy.py` & `torch_conduit-0.2.0/conduit/data/datasets/tabular/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import numpy as np
 import pandas as pd
 import torch
 
 from conduit.data.datasets.tabular import CdtTabularDataset
 
+__all__ = ["RandomTabularDataset"]
+
 
 class RandomTabularDataset(CdtTabularDataset):
     def __init__(
         self,
         num_disc_features: int = 3,
         num_cont_features: int = 5,
         num_samples: int = 256,
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/utils.py` & `torch_conduit-0.2.0/conduit/data/datasets/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,170 +15,75 @@
     List,
     Literal,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Type,
+    TypedDict,
     TypeVar,
     Union,
     cast,
-    get_args,
     overload,
 )
 from zipfile import BadZipFile
 
-from PIL import Image
-import albumentations as A  # type: ignore
-import cv2
 import numpy as np
 import numpy.typing as npt
 from ranzen.misc import gcopy
 from ranzen.torch.data import Subset, prop_random_split
 import torch
 from torch import Tensor
-from torch._six import string_classes
 from torch.utils.data import ConcatDataset
 from torch.utils.data._utils.collate import (
     default_collate_err_msg_format,
     np_str_obj_array_pattern,
 )
 from torch.utils.data.dataloader import DataLoader, _worker_init_fn_t
 from torch.utils.data.sampler import Sampler
 from torchvision.datasets.utils import (  # type: ignore
     _detect_file_type,
     download_url,
     extract_archive,
 )
-from torchvision.transforms import functional as TF  # type: ignore
-from typing_extensions import TypeAlias, TypeGuard
+from typing_extensions import TypeAlias, TypeGuard, Unpack
 
 from conduit.data.datasets.base import CdtDataset
 from conduit.data.structures import (
     BinarySample,
     Dataset,
     LoadedData,
     NamedSample,
     PseudoCdtDataset,
-    RawImage,
     SampleBase,
     SizedDataset,
     TernarySample,
     TrainTestSplit,
 )
 
 __all__ = [
-    "AlbumentationsTform",
     "AudioTform",
     "CdtDataLoader",
     "GdriveFileInfo",
-    "ImageLoadingBackend",
-    "ImageTform",
-    "PillowTform",
     "UrlFileInfo",
-    "apply_image_transform",
     "cdt_collate",
     "check_integrity",
     "download_from_gdrive",
     "download_from_url",
     "extract_base_dataset",
     "extract_labels_from_dataset",
     "get_group_ids",
-    "img_to_tensor",
     "infer_al_backend",
-    "infer_il_backend",
     "infer_sample_cls",
     "is_tensor_list",
-    "load_image",
     "make_subset",
     "stratified_split",
 ]
 
 
-ImageLoadingBackend: TypeAlias = Literal["opencv", "pillow"]
-
-
-@overload
-def load_image(
-    filepath: Union[Path, str], *, backend: Literal["opencv"] = ...
-) -> npt.NDArray[np.integer]:
-    ...
-
-
-@overload
-def load_image(filepath: Union[Path, str], *, backend: Literal["pillow"] = ...) -> Image.Image:
-    ...
-
-
-def load_image(filepath: Union[Path, str], *, backend: ImageLoadingBackend = "opencv") -> RawImage:
-    """Load an image from disk using the requested backend.
-
-    :param: The path of the image-file to be loaded.
-    :param backend: Backed to use for loading the image: either 'opencv' or 'pillow'.
-
-    :returns: The loaded image file as a numpy array if 'opencv' was the selected backend
-    and a PIL image otherwise.
-    """
-    if backend == "opencv":
-        if isinstance(filepath, Path):
-            # cv2 can only read string filepaths
-            filepath = str(filepath)
-        image = cv2.imread(filepath)  # type: ignore
-        if image is None:
-            raise OSError(f"Image-file could not be read from location '{filepath}'")
-        return cv2.cvtColor(image, cv2.COLOR_BGR2RGB)  # type: ignore
-    return Image.open(filepath)
-
-
-AlbumentationsTform: TypeAlias = Union[A.Compose, A.BasicTransform]
-PillowTform: TypeAlias = Callable[[Image.Image], Any]
-ImageTform: TypeAlias = Union[AlbumentationsTform, PillowTform]
-
-
-def infer_il_backend(transform: Optional[ImageTform]) -> ImageLoadingBackend:
-    """Infer which image-loading backend to use based on the type of the image-transform.
-
-    :param transform: The image transform from which to infer the image-loading backend.
-    If the transform is derived from Albumentations, then 'opencv' will be selected as the
-    backend, else 'pillow' will be selected.
-
-    :returns: The backend to load images with based on the supplied image-transform: either
-    'opencv' or 'pillow'.
-    """
-    # Default to openccv is transform is None as numpy arrays are generally
-    # more tractable
-    if transform is None or isinstance(transform, get_args(AlbumentationsTform)):
-        return "opencv"
-    return "pillow"
-
-
-def apply_image_transform(
-    image: RawImage, *, transform: Optional[ImageTform]
-) -> Union[RawImage, Tensor]:
-    image_ = image
-    if transform is not None:
-        if isinstance(transform, (A.Compose, A.BasicTransform)):
-            if isinstance(image, Image.Image):
-                image = np.array(image)
-            image_ = transform(image=image)["image"]
-        else:
-            if isinstance(image, np.ndarray):
-                image = Image.fromarray(image)
-            image_ = transform(image)
-    return image_
-
-
-def img_to_tensor(img: Union[Image.Image, np.ndarray]) -> Tensor:
-    if isinstance(img, Image.Image):
-        return TF.pil_to_tensor(img)
-    return torch.from_numpy(
-        np.moveaxis(img / (255.0 if img.dtype == np.uint8 else 1), -1, 0).astype(np.float32)
-    )
-
-
 AudioLoadingBackend: TypeAlias = Literal["sox_io", "soundfile"]
 
 
 def infer_al_backend() -> AudioLoadingBackend:
     """Infer which audio-loading backend to use based on the operating system."""
     soundfile: Final = "soundfile"
     sox: Final = "sox_io"
@@ -213,20 +118,19 @@
 
     Nested datasets are inferred based on the existence of a 'dataset'
     attribute and the base dataset is extracted by recursive application
     of this rule.
 
     :param dataset: The dataset from which to extract the base dataset.
 
-    :param return_subset_indices: Whether to return the indices from which
-    the overall subset of the dataset was created (works for multiple levels of
-    subsetting).
+    :param return_subset_indices: Whether to return the indices from which the overall subset of the
+        dataset was created (works for multiple levels of subsetting).
 
-    :returns: The base dataset, which may be the original dataset if one does not
-    exist or cannot be determined.
+    :returns: The base dataset, which may be the original dataset if one does not exist or cannot be
+        determined.
     """
 
     def _closure(
         dataset: Dataset, rel_indices_ls: Optional[List[List[int]]] = None
     ) -> Union[Dataset, Tuple[Dataset, Union[Tensor, slice]]]:
         if rel_indices_ls is None:
             rel_indices_ls = []
@@ -254,18 +158,18 @@
     """Attempt to extract s/y labels from a dataset."""
     base_dataset = dataset
 
     def _closure(dataset: Dataset) -> Tuple[Optional[Tensor], Optional[Tensor]]:
         base_dataset, indices = extract_base_dataset(dataset=dataset, return_subset_indices=True)
         _s = None
         _y = None
-        if getattr(base_dataset, "s", None) is not None:
-            _s = base_dataset.s[indices]  # type: ignore
-        if getattr(base_dataset, "y", None) is not None:
-            _y = base_dataset.y[indices]  # type: ignore
+        if (s := getattr(base_dataset, "s", None)) is not None:
+            _s = s[indices]
+        if (y := getattr(base_dataset, "y", None)) is not None:
+            _y = y[indices]
 
         _s = torch.from_numpy(_s) if isinstance(_s, np.ndarray) else _s
         _y = torch.from_numpy(_y) if isinstance(_y, np.ndarray) else _y
 
         return _s, _y
 
     if isinstance(base_dataset, (ConcatDataset)):
@@ -322,23 +226,25 @@
     dataset: Union[PCD, Subset[PCD]],
     *,
     indices: Optional[Union[List[int], npt.NDArray[np.uint64], Tensor, slice]],
     deep: bool = False,
 ) -> PCD:
     """Create a subset of the dataset from the given indices.
 
+    :param dataset: The dataset to split.
     :param indices: The sample-indices from which to create the subset.
-    In the case of being a numpy array or tensor, said array or tensor
-    must be 0- or 1-dimensional.
+        In the case of being a numpy array or tensor, said array or tensor
+        must be 0- or 1-dimensional.
 
-    :param deep: Whether to create a copy of the underlying dataset as
-    a basis for the subset. If False then the data of the subset will be
-    a view of original dataset's data.
+    :param deep: Whether to create a copy of the underlying dataset as a basis for the subset.
+        If False then the data of the subset will be a view of original dataset's data.
 
     :returns: A subset of the dataset from the given indices.
+    :raises ValueError: if the indices don't have the correct shape.
+    :raises TypeError: if the dataset is not an instance of ``CdtDataset``.
     """
     if isinstance(indices, (np.ndarray, Tensor)):
         if indices.ndim > 1:
             raise ValueError("If 'indices' is an array it must be a 0- or 1-dimensional.")
         indices = cast(List[int], indices.tolist())
 
     current_indices = None
@@ -416,16 +322,16 @@
                 out = elem.new(storage).resize_(len(batch), *list(elem.size()))
             ndims = elem.dim()
             # If 'batch' is a sequence of sub-batched tensors we concatenate the elements along the
             # batch dimesion. Note, the problem of inferring whether the tensors are sub-batched or
             # not is ill-posed given that the dimensionality of samples varies with modality; the
             # current solution is tailored for tabular and image data.
             if (ndims > 0) and ((ndims % 2) == 0):
-                return torch.cat(batch, dim=0, out=out)  # type: ignore
-            return torch.stack(batch, dim=0, out=out)  # type: ignore
+                return torch.cat(batch, dim=0, out=out)
+            return torch.stack(batch, dim=0, out=out)
         # NumPy array
         elif (
             elem_type.__module__ == "numpy"
             and elem_type.__name__ != "str_"
             and elem_type.__name__ != "string_"
         ):
             elem = batch[0]
@@ -437,15 +343,15 @@
         # Float
         elif isinstance(elem, float):
             return torch.tensor(batch, dtype=torch.float32)
         # Integer
         elif isinstance(elem, int):
             return torch.tensor(batch)
         # String
-        elif isinstance(elem, string_classes):
+        elif isinstance(elem, str):
             return batch
         # Mapping
         elif isinstance(elem, Mapping):
             return elem_type({key: self._collate([d[key] for d in batch]) for key in elem})
         # NamedTuple
         elif isinstance(elem, tuple) and hasattr(elem, "_fields"):  # namedtuple
             return elem_type(**(self._collate(samples) for samples in zip(*batch)))
@@ -475,51 +381,51 @@
                 )
         return collated_batch
 
 
 I = TypeVar("I", bound=NamedSample)
 
 
+class _DataLoaderKwargs(TypedDict, total=False):
+    """Dictionary of keyword arguments used to avoid specifying the default values."""
+
+    batch_size: Optional[int]
+    shuffle: bool
+    sampler: Optional[Sampler[int]]
+    batch_sampler: Optional[Sampler[Sequence[int]]]
+    num_workers: int
+    pin_memory: bool
+    drop_last: bool
+    timeout: float
+    worker_init_fn: Optional[_worker_init_fn_t]
+    multiprocessing_context: Optional[Union[BaseContext, str]]
+    generator: Optional[torch.Generator]
+    prefetch_factor: int
+    persistent_workers: bool
+    pin_memory_device: str
+
+
 class CdtDataLoader(DataLoader[I]):
     def __init__(
         self,
         dataset: SizedDataset[I],
         *,
-        batch_size: Optional[int] = 1,
-        shuffle: bool = False,
-        sampler: Optional[Sampler[int]] = None,
-        batch_sampler: Optional[Sampler[Sequence[int]]] = None,
-        num_workers: int = 0,
-        pin_memory: bool = False,
-        drop_last: bool = False,
-        timeout: float = 0,
-        worker_init_fn: Optional[_worker_init_fn_t] = None,
-        multiprocessing_context: Optional[Union[BaseContext, str]] = None,
-        generator: Optional[torch.Generator] = None,
-        prefetch_factor: int = 2,
-        persistent_workers: bool = False,
         cast_to_sample: bool = True,
         converter: Optional[Union[Type[Any], Callable]] = None,
+        **kwargs: Unpack[_DataLoaderKwargs],
     ) -> None:
+        # pytorch_lightning inspects the signature and if it sees `**kwargs`, it assumes that
+        # the __init__ takes all arguments that DataLoader.__init__ takes, so we have to
+        # manually remove "collate_fn" here in order to avoid passing it in *twice*.
+        if "collate_fn" in kwargs:
+            del kwargs["collate_fn"]  # type: ignore
         super().__init__(
             dataset,  # type: ignore
-            batch_size=batch_size,
-            shuffle=shuffle,
-            sampler=sampler,
-            batch_sampler=batch_sampler,
-            num_workers=num_workers,
             collate_fn=cdt_collate(cast_to_sample=cast_to_sample, converter=converter),
-            pin_memory=pin_memory,
-            drop_last=drop_last,
-            timeout=timeout,
-            worker_init_fn=worker_init_fn,
-            multiprocessing_context=multiprocessing_context,
-            generator=generator,
-            prefetch_factor=prefetch_factor,
-            persistent_workers=persistent_workers,
+            **kwargs,
         )
 
     def __iter__(self) -> Iterator[I]:
         return super().__iter__()
 
 
 def check_integrity(*, filepath: Path, md5: Optional[str]) -> None:
@@ -539,15 +445,14 @@
 def download_from_url(
     *,
     file_info: Union[UrlFileInfo, List[UrlFileInfo]],
     root: Union[Path, str],
     logger: Optional[logging.Logger] = None,
     remove_finished: bool = True,
 ) -> None:
-
     logger = logging.getLogger(__name__) if logger is None else logger
     file_info_ls = file_info if isinstance(file_info, list) else [file_info]
     if not isinstance(root, Path):
         root = Path(root).expanduser()
     # Create the specified root directory if it doesn't already exist
     root.mkdir(parents=True, exist_ok=True)
 
@@ -677,30 +582,30 @@
     props: Union[Sequence[float], float],
     deep: bool = False,
     as_indices: bool = False,
     seed: Optional[int] = None,
 ) -> Union[List[PCD], List[List[int]]]:
     """Randomly split the dataset into subsets according to the given proportions.
 
+    :param dataset: The dataset to split.
     :param props: The fractional size of each subset into which to randomly split the data.
-    Elements must be non-negative and sum to 1 or less; if less then the size of the final
-    split will be computed by complement.
+        Elements must be non-negative and sum to 1 or less; if less then the size of the final
+        split will be computed by complement.
 
-    :param deep: Whether to create a copy of the underlying dataset as
-    a basis for the random subsets. If False then the data of the subsets will be
-    views of original dataset's data.
+    :param deep: Whether to create a copy of the underlying dataset as a basis for the random
+        subsets. If False then the data of the subsets will be views of original dataset's data.
 
     :param as_indices: Whether to return the raw train/test indices instead of subsets of the
-    dataset constructed from them.
+        dataset constructed from them.
 
     :param seed: PRNG seed to use for splitting the data.
 
     :returns: Random subsets of the data (or their associated indices) of the requested proportions.
     """
-    split_indices = prop_random_split(dataset=dataset, props=props, as_indices=True, seed=seed)
+    split_indices = prop_random_split(dataset, props=props, as_indices=True, seed=seed)
     if as_indices:
         return split_indices
     splits = [make_subset(dataset, indices=indices, deep=deep) for indices in split_indices]
     return splits
 
 
 @overload
@@ -745,29 +650,28 @@
     default_train_prop: float,
     train_props: Optional[Dict[int, Union[Dict[int, float], float]]] = None,
     seed: Optional[int] = None,
     as_indices: bool = False,
 ) -> Union[TrainTestSplit[PCD], TrainTestSplit[List[int]]]:
     """Splits the data into train/test sets conditional on super- and sub-class labels.
 
+    :param dataset: The dataset to split.
     :param default_train_prop: Proportion of samples for a given to sample for
-    the training set for those y-s combinations not specified in ``train_props``.
-
+        the training set for those y-s combinations not specified in ``train_props``.
     :param train_props: Proportion of each superclass-subclass combination to sample for
-    the training set. Keys correspond to the superclass while values can be either a float,
-    in which case the proportion is applied to the superclass as a whole, or a dict, in which
-    case the sampling is applied only to the subclasses of the superclass given by the keys.
-    If ``None`` then the function reduces to a simple random split of the data.
-
+        the training set. Keys correspond to the superclass while values can be either a float,
+        in which case the proportion is applied to the superclass as a whole, or a dict, in which
+        case the sampling is applied only to the subclasses of the superclass given by the keys.
+        If ``None`` then the function reduces to a simple random split of the data.
     :param as_indices: Whether to return the raw train/test indices instead of subsets of the
-    dataset constructed from them.
-
+        dataset constructed from them.
     :param seed: PRNG seed to use for determining the splits.
-
     :returns: Train-test subsets (``as_indices=False``) or indices (``as_indices=True``).
+    :raises TypeError: if no superclass labels are available.
+    :raises ValueError: if the labels are not as expected.
     """
     if dataset.y is None:
         raise TypeError(
             f"Dataset of type {dataset.__class__.__name__} has no superclass labels to use "
             "for stratification."
         )
     train_props = {} if train_props is None else train_props
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/base.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from functools import reduce
 import operator
 from pathlib import Path
 from typing import List, Optional, Sequence, Union, cast, overload
 
 import numpy as np
 import numpy.typing as npt
-from ranzen import implements
 from ranzen.types import Addable
 import torch
 from torch import Tensor
-from typing_extensions import Self, TypeAlias
+from typing_extensions import Self, TypeAlias, override
 
 from conduit.data.datasets.base import CdtDataset, I, S, Y
-from conduit.data.datasets.utils import (
+from conduit.data.datasets.vision.utils import (
     ImageLoadingBackend,
     ImageTform,
     RawImage,
     apply_image_transform,
     img_to_tensor,
     infer_il_backend,
     load_image,
@@ -73,15 +72,15 @@
     def _sample_x(self, index: int, *, coerce_to_tensor: bool = ...) -> ItemType:
         ...
 
     @overload
     def _sample_x(self, index: List[int], *, coerce_to_tensor: bool = ...) -> List[ItemType]:
         ...
 
-    @implements(CdtDataset)
+    @override
     def _sample_x(
         self, index: IndexType, *, coerce_to_tensor: bool = False
     ) -> Union[ItemType, List[ItemType]]:
         if isinstance(index, slice):
             index = list(range(len(self)))[index]
         if isinstance(index, list):
             sample_ls = [self._sample_x(index=i, coerce_to_tensor=coerce_to_tensor) for i in index]
@@ -101,30 +100,28 @@
         if coerce_to_tensor and (not isinstance(image, Tensor)):
             if isinstance(image, Sequence):
                 image = [img_to_tensor(subimage) for subimage in image]
             else:
                 image = img_to_tensor(image)
         return image
 
-    @implements(CdtDataset)
+    @override
     def subset(
-        self: Self,
+        self,
         indices: Union[List[int], npt.NDArray[np.uint64], Tensor, slice],
         deep: bool = False,
         transform: Optional[ImageTform] = None,
     ) -> Self:
         """Create a subset of the dataset from the given indices.
 
-        :param indices: The sample-indices from which to create the subset.
-        In the case of being a numpy array or tensor, said array or tensor
-        must be 0- or 1-dimensional.
-
-        :param deep: Whether to create a copy of the underlying dataset as
-        a basis for the subset. If False then the data of the subset will be
-        a view of original dataset's data.
+        :param indices: The sample-indices from which to create the subset. In the case of being a
+            numpy array or tensor, said array or tensor must be 0- or 1-dimensional.
+
+        :param deep: Whether to create a copy of the underlying dataset as a basis for the subset.
+            If False then the data of the subset will be a view of original dataset's data.
 
         :param transform: Image transform to assign to the resulting subset.
 
         :returns: A subset of the dataset from the given indices.
         """
         subset = super().subset(indices=indices, deep=deep)
         if transform is not None:
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/camelyon17.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/camelyon17.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 from enum import Enum, auto
 from pathlib import Path
-from typing import ClassVar, Optional, Union, cast
+from typing import ClassVar, Optional, Union
 
 import pandas as pd
-from ranzen.decorators import enum_name_str, parsable
-from ranzen.misc import str_to_enum
+from ranzen.decorators import parsable
+from ranzen.misc import StrEnum
 import torch
 from torch import Tensor
 from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import ImageTform, UrlFileInfo, download_from_url
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.datasets import UrlFileInfo, download_from_url
 from conduit.data.structures import TernarySample
 
-__all__ = [
-    "Camelyon17",
-    "Camelyon17Split",
-    "Camelyon17SplitScheme",
-]
+from .base import CdtVisionDataset
+from .utils import ImageTform
 
+__all__ = ["Camelyon17", "Camelyon17Split", "Camelyon17SplitScheme"]
 
-@enum_name_str
-class Camelyon17SplitScheme(Enum):
-    official = auto()
+
+class Camelyon17SplitScheme(StrEnum):
+    OFFICIAL = auto()
     """Oficial split."""
 
-    mixed_to_test = auto()
+    MIXED_TO_TEST = auto()
     """ 
     For the mixed-to-test setting, slide 23 (corresponding to patient 042, node 3 in the
     original dataset) is moved from the test set to the training set
     """
 
 
 class Camelyon17Split(Enum):
-    train = 0
-    id_val = 1
-    test = 2
-    val = 3
+    TRAIN = 0
+    ID_VAL = 1
+    TEST = 2
+    VAL = 3
 
 
-@enum_name_str
-class Camelyon17Attr(Enum):
-    tumor = auto()
-    center = auto()
-    slide = auto()
+class Camelyon17Attr(StrEnum):
+    TUMOR = auto()
+    CENTER = auto()
+    SLIDE = auto()
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class Camelyon17(CdtVisionDataset[SampleType, Tensor, Tensor]):
-    """
-    The CAMELYON17-WILDS histopathology dataset.
+    """The CAMELYON17-WILDS histopathology dataset.
+
     This is a modified version of the original CAMELYON17 dataset.
 
-    Supported `split_scheme`:
+    Supported ``split_scheme``:
         - 'official'
         - 'mixed-to-test'
 
     Input (x):
         96x96 image patches extracted from histopathology slides.
 
     Label (y):
@@ -68,30 +64,41 @@
         Each patch is annotated with the ID of the hospital it came from (integer from 0 to 4)
         and the slide it came from (integer from 0 to 49).
 
     Website:
         https://camelyon17.grand-challenge.org/
 
     Original publication:
+
+    .. code-block:: bibtex
+
         @article{bandi2018detection,
-          title={From detection of individual metastases to classification of lymph node status at the patient level: the camelyon17 challenge},
-          author={Bandi, Peter and Geessink, Oscar and Manson, Quirine and Van Dijk, Marcory and Balkenhol, Maschenka and Hermsen, Meyke and Bejnordi, Babak Ehteshami and Lee, Byungjae and Paeng, Kyunghyun and Zhong, Aoxiao and others},
+          title={From detection of individual metastases to classification of lymph node status at
+                 the patient level: the camelyon17 challenge},
+          author={Bandi, Peter and Geessink, Oscar and Manson, Quirine and Van Dijk, Marcory
+                  and Balkenhol, Maschenka and Hermsen, Meyke and Bejnordi, Babak Ehteshami
+                  and Lee, Byungjae and Paeng, Kyunghyun and Zhong, Aoxiao and others},
           journal={IEEE transactions on medical imaging},
           volume={38},
           number={2},
           pages={550--560},
           year={2018},
           publisher={IEEE}
         }
 
     License:
         This dataset is in the public domain and is distributed under CC0.
         https://creativecommons.org/publicdomain/zero/1.0/
     """
 
+    SampleType: TypeAlias = TernarySample
+    Attr: TypeAlias = Camelyon17Attr
+    Split: TypeAlias = Camelyon17Split
+    SplitScheme: TypeAlias = Camelyon17SplitScheme
+
     _FILE_INFO: ClassVar[UrlFileInfo] = UrlFileInfo(
         name="camelyon17_v1.0.tar.gz",
         url="https://worksheets.codalab.org/rest/bundles/0xe45e15f39fb54e9d9e919556af67aabe/contents/blob/",
         md5=None,
     )
     _TEST_CENTER: ClassVar[int] = 2
     _VAL_CENTER: ClassVar[int] = 1
@@ -100,30 +107,25 @@
     def __init__(
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
         split: Optional[Union[Camelyon17Split, str]] = None,
-        split_scheme: Union[Camelyon17SplitScheme, str] = Camelyon17SplitScheme.official,
-        superclass: Union[Camelyon17Attr, str] = Camelyon17Attr.tumor,
-        subclass: Union[Camelyon17Attr, str] = Camelyon17Attr.center,
+        split_scheme: Union[Camelyon17SplitScheme, str] = Camelyon17SplitScheme.OFFICIAL,
+        superclass: Union[Camelyon17Attr, str] = Camelyon17Attr.TUMOR,
+        subclass: Union[Camelyon17Attr, str] = Camelyon17Attr.CENTER,
     ) -> None:
-
-        self.superclass = str_to_enum(str_=superclass, enum=Camelyon17Attr)
-        self.subclass = str_to_enum(str_=subclass, enum=Camelyon17Attr)
-
-        self.split = (
-            str_to_enum(str_=split, enum=Camelyon17Split) if isinstance(split, str) else split
-        )
+        self.superclass = Camelyon17Attr(superclass) if isinstance(split, str) else split
+        self.subclass = Camelyon17Attr(subclass) if isinstance(split, str) else split
+        self.split = Camelyon17Split[split.upper()] if isinstance(split, str) else split
         self.split_scheme = (
-            str_to_enum(str_=split_scheme, enum=Camelyon17SplitScheme)
-            if isinstance(split_scheme, str)
-            else split_scheme
+            Camelyon17SplitScheme(split_scheme) if isinstance(split_scheme, str) else split_scheme
         )
+
         self.root = Path(root)
         self._base_dir = self.root / "camelyon17_v1.0"
         self.download = download
         if self.download:
             download_from_url(
                 file_info=self._FILE_INFO,
                 root=self.root,
@@ -136,30 +138,30 @@
             )
 
         # Read in metadata
         # Note: metadata is one-indexed.
         self.metadata = pd.read_csv(
             self._base_dir / 'metadata.csv', index_col=0, dtype={"patient": "str"}
         )
-        if self.split_scheme is Camelyon17SplitScheme.mixed_to_test:
+        if self.split_scheme is Camelyon17SplitScheme.MIXED_TO_TEST:
             # For the mixed-to-test setting,
             # we move slide 23 (corresponding to patient 042, node 3 in the original dataset)
             # from the test set to the training set
             slide_mask = self.metadata["slide"] == 23
-            self.metadata.loc[slide_mask, "split"] = Camelyon17Split.train.value
+            self.metadata.loc[slide_mask, "split"] = Camelyon17Split.TRAIN.value
         # Use an official split of the data, if 'split' is specified, else just use all
         # of the data
         val_center_mask = self.metadata["center"] == self._VAL_CENTER
         test_center_mask = self.metadata["center"] == self._TEST_CENTER
-        self.metadata.loc[val_center_mask, "split"] = Camelyon17Split.val.value
-        self.metadata.loc[test_center_mask, "split"] = Camelyon17Split.test.value
+        self.metadata.loc[val_center_mask, "split"] = Camelyon17Split.VAL.value
+        self.metadata.loc[test_center_mask, "split"] = Camelyon17Split.TEST.value
 
         if self.split is not None:
             split_indices = self.metadata["split"] == self.split.value
-            self.metadata = cast(pd.DataFrame, self.metadata[split_indices])
+            self.metadata = self.metadata.loc[split_indices]
 
         # Construct filepaths from metadata
         def build_fp(row: pd.DataFrame) -> str:
             return "patches/patient_{0}_node_{1}/patch_patient_{0}_node_{1}_x_{2}_y_{3}.png".format(
                 *row
             )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/cmnist.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/cmnist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 """ColoredMNIST Dataset."""
-from enum import Enum
+from enum import auto
 from pathlib import Path
 from typing import ClassVar, Dict, List, Optional, Tuple, Union, cast
 
 from PIL import Image
 import numpy as np
 import numpy.typing as npt
-from ranzen.decorators import implements, parsable
-from ranzen.misc import str_to_enum
+from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
 from torchvision.datasets import MNIST  # type: ignore
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, override
 
-from conduit.data.datasets.utils import ImageTform, RawImage
-from conduit.data.datasets.vision.base import CdtVisionDataset
 from conduit.data.structures import TernarySample
 from conduit.types import NDArrayR
 
-__all__ = [
-    "ColoredMNIST",
-    "ColoredMNISTSplit",
-    "MNISTColorizer",
-]
+from .base import CdtVisionDataset
+from .utils import ImageTform, RawImage
+
+__all__ = ["ColoredMNIST", "ColoredMNISTSplit", "MNISTColorizer"]
 
 
 class MNISTColorizer:
     """Convert a greyscale MNIST image to RGB."""
 
     COLORS: ClassVar[Tensor] = torch.tensor(
         [
@@ -67,15 +63,15 @@
         :param max_val: Maximum value the input data can take (needed for clamping).
         :param scale: Standard deviation of the multivariate normal distributions from which
             the colors are drawn. Lower values correspond to higher bias. Defaults to 0.02.
         :param binarize: Whether to the binarize the grayscale data before colorisation.
         :param background: Whether to color the background instead of the foreground.
         :param black: Whether not to invert the black. Defaults to True.
         :param greyscale: Whether to greyscale the colorised images. Defaults to False.
-        :param color_indices: Choose specific colors if you don't need all 10
+        :param color_indices: Choose specific colors if you don't need all 10.
         :param seed: Random seed used for sampling colors.
         """
         super().__init__()
         self.min_val = min_val
         self.max_val = max_val
         self.binarize = binarize
         self.background = background
@@ -100,16 +96,18 @@
         )
 
     def __call__(
         self, images: Union[Tensor, NDArrayR], *, labels: Union[Tensor, NDArrayR]
     ) -> Tensor:
         """Apply the transformation.
 
-        :param images:  Greyscale images to be colorized. Expected to be unnormalized (in the range [0, 255]).
-        :param labels: Indexes (0-9) indicating the gaussian distribution from which to sample each image's color.
+        :param images:  Greyscale images to be colorized. Expected to be unnormalized (in the range
+            [0, 255]).
+        :param labels: Indexes (0-9) indicating the gaussian distribution from which to sample each
+            image's color.
         :returns: Images converted to RGB.
         """
         if isinstance(images, np.ndarray):
             images = torch.as_tensor(images, dtype=torch.float32)
         if isinstance(labels, np.ndarray):
             labels = torch.as_tensor(labels, dtype=torch.long)
         # Add a singular channel dimension if one isn't already there.
@@ -153,17 +151,17 @@
     for old_label, new_label in label_map.items():
         mask = targets == int(old_label)
         targets[mask] = new_label
         final_mask |= mask
     return data[final_mask], targets[final_mask]
 
 
-class ColoredMNISTSplit(Enum):
-    train = 1
-    test = 0
+class ColoredMNISTSplit(StrEnum):
+    TRAIN = auto()
+    TEST = auto()
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class ColoredMNIST(CdtVisionDataset[SampleType, Tensor, Tensor]):
     x: npt.NDArray[np.floating]
@@ -180,56 +178,58 @@
         num_colors: int = 10,
         scale: float = 0.2,
         correlation: Optional[float] = None,
         binarize: bool = False,
         greyscale: bool = False,
         background: bool = False,
         black: bool = True,
-        split: Optional[Union[ColoredMNISTSplit, str]] = None,
+        split: Optional[Union[ColoredMNISTSplit, str, List[int]]] = None,
         seed: Optional[int] = 42,
     ) -> None:
-        self.split = (
-            str_to_enum(str_=split, enum=ColoredMNISTSplit) if isinstance(split, str) else split
-        )
+        self.split = ColoredMNISTSplit(split) if isinstance(split, str) else split
         self.label_map = label_map
         self.scale = scale
         self.num_colors = num_colors
         self.colors = colors
         self.background = background
         self.binarize = binarize
         self.black = black
         self.greyscale = greyscale
         self.seed = seed
         # Note: a correlation coefficient of '1' corresponds to perfect correlation between
         # digit and class while a correlation coefficient of '-1' corresponds to perfect
         # anti-correlation.
         if correlation is None:
-            correlation = 1.0 if split is ColoredMNISTSplit.train else 0.5
+            correlation = 1.0 if split is ColoredMNISTSplit.TRAIN else 0.5
         if not 0 <= correlation <= 1:
             raise ValueError(
                 "Strength of correlation between colour and targets must be between 0 and 1."
             )
         self.correlation = correlation
 
-        if self.split is None:
+        if isinstance(self.split, ColoredMNISTSplit):
+            base_dataset = MNIST(
+                root=str(root), download=download, train=self.split is ColoredMNISTSplit.train
+            )
+            x = base_dataset.data
+            y = base_dataset.targets
+        else:
             x_ls, y_ls = [], []
             for _split in ColoredMNISTSplit:
                 base_dataset = MNIST(
-                    root=str(root), download=download, train=_split is ColoredMNISTSplit.train
+                    root=str(root), download=download, train=_split is ColoredMNISTSplit.TRAIN
                 )
                 x_ls.append(base_dataset.data)
                 y_ls.append(base_dataset.targets)
             x = torch.cat(x_ls, dim=0)
             y = torch.cat(y_ls, dim=0)
-        else:
-            base_dataset = MNIST(
-                root=str(root), download=download, train=self.split is ColoredMNISTSplit.train
-            )
-            x = base_dataset.data
-            y = base_dataset.targets
+            # custom split
+            if self.split is not None:
+                x = x[self.split]
+                y = y[self.split]
 
         if self.label_map is not None:
             x, y = _filter_data_by_labels(data=x, targets=y, label_map=self.label_map)
         s = y % self.num_colors
         s_unique, s_unique_inv = s.unique(return_inverse=True)
 
         generator = (
@@ -244,15 +244,15 @@
             num_to_flip = round((1 - flip_prop) * len(s))
             to_flip = torch.randperm(len(s), generator=generator)[:num_to_flip]
             s_unique_inv[to_flip] += torch.randint(low=1, high=len(s_unique), size=(num_to_flip,))
             # s labels live inside the Z/(num_colors * Z) ring
             s_unique_inv[to_flip] %= len(s_unique)
             s = s_unique[s_unique_inv]
 
-        # Convert the greyscale iamges of shape ( H, W ) into 'colour' images of shape ( C, H, W )
+        # Convert the greyscale images of shape ( H, W ) into 'colour' images of shape ( C, H, W )
         colorizer = MNISTColorizer(
             scale=self.scale,
             background=self.background,
             black=self.black,
             binarize=self.binarize,
             greyscale=self.greyscale,
             color_indices=self.colors,
@@ -260,13 +260,13 @@
         )
         x_colorized = colorizer(images=x, labels=s)
         # Convert to HWC format for compatibility with transforms
         x_colorized = x_colorized.movedim(1, -1).numpy().astype(np.uint8)
 
         super().__init__(x=x_colorized, y=y, s=s, transform=transform, image_dir=root)
 
-    @implements(CdtVisionDataset)
+    @override
     def _load_image(self, index: int) -> RawImage:
         image = self.x[index]
         if self._il_backend == "pillow":
             image = Image.fromarray(image)
         return image
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/dummy.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Optional, cast
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
-from ranzen import implements
 import torch
 from torch import Tensor
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, override
 
-from conduit.data.datasets.vision.base import CdtVisionDataset
 from conduit.data.structures import TernarySample
 
+from .base import CdtVisionDataset
+
 SampleType: TypeAlias = TernarySample
 
 
 class DummyVisionDataset(CdtVisionDataset[SampleType, Tensor, Tensor]):
     def __init__(
         self,
         channels: int,
@@ -27,14 +27,12 @@
         self.height = height
         self.width = width
         s = torch.randint(s_card, (num_samples,)) if s_card is not None else None
         y = torch.randint(y_card, (num_samples,)) if y_card is not None else None
         x = np.array([""] * num_samples)
         super().__init__(x=x, s=s, y=y, image_dir="")
 
-    @implements(CdtVisionDataset)
+    @override
     def _load_image(self, index: int) -> npt.NDArray[np.uint8]:
-
-        return cast(
-            npt.NDArray[np.uint8],
-            np.random.randint(0, 256, size=(self.height, self.width, self.channels), dtype="uint8"),
+        return np.random.randint(
+            0, 256, size=(self.height, self.width, self.channels), dtype="uint8"
         )
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/isic.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/isic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 """ISIC Dataset."""
 from __future__ import annotations
-from enum import Enum, auto
+from enum import auto
 from itertools import islice
 import os
 from pathlib import Path
 import shutil
 from typing import ClassVar, Iterable, Iterator, List, Optional, TypeVar, Union
 import zipfile
 
 from PIL import Image
 import pandas as pd
-from ranzen import flatten_dict
-from ranzen.decorators import enum_name_str, parsable
+from ranzen import StrEnum, flatten_dict
+from ranzen.decorators import parsable
 import requests
 import torch
 from torch import Tensor
-from tqdm import tqdm  # type: ignore
+from tqdm import tqdm
 from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import ImageTform
-from conduit.data.datasets.vision.base import CdtVisionDataset
 from conduit.data.structures import TernarySample
 
+from .base import CdtVisionDataset
+from .utils import ImageTform
+
 __all__ = ["IsicAttr", "ISIC"]
 
 
-@enum_name_str
-class IsicAttr(Enum):
-    histo = auto()
-    malignant = auto()
-    patch = auto()
+class IsicAttr(StrEnum):
+    HISTO = auto()
+    MALIGNANT = auto()
+    PATCH = auto()
 
 
 T = TypeVar("T")
 SampleType: TypeAlias = TernarySample
 
 
 class ISIC(CdtVisionDataset[SampleType, Tensor, Tensor]):
     """PyTorch Dataset for the ISIC 2018 dataset from
     'Skin Lesion Analysis Toward Melanoma Detection 2018: A Challenge Hosted by the International
     Skin Imaging Collaboration (ISIC)',"""
 
+    SampleType: TypeAlias = TernarySample
+    Attr: TypeAlias = IsicAttr
+
     LABELS_FILENAME: ClassVar[str] = "labels.csv"
     METADATA_FILENAME: ClassVar[str] = "metadata.csv"
     _PBAR_COL: ClassVar[str] = "#fac000"
     _REST_API_URL: ClassVar[str] = "https://isic-archive.com/api/v1"
 
     @parsable
     def __init__(
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         max_samples: int = 25_000,  # default is the number of samples used for the NSLB paper
-        context_attr: IsicAttr = IsicAttr.histo,
-        target_attr: IsicAttr = IsicAttr.malignant,
+        target_attr: IsicAttr = IsicAttr.MALIGNANT,
+        context_attr: IsicAttr = IsicAttr.HISTO,
         transform: Optional[ImageTform] = None,
     ) -> None:
+        self.target_attr = IsicAttr(target_attr) if isinstance(target_attr, str) else target_attr
+        self.context_attr = (
+            IsicAttr(context_attr) if isinstance(context_attr, str) else context_attr
+        )
 
         self.root = Path(root)
         self.download = download
         self._base_dir = self.root / self.__class__.__name__
         self._processed_dir = self._base_dir / "processed"
         self._raw_dir = self._base_dir / "raw"
 
@@ -76,16 +83,16 @@
                 "Have you downloaded it?"
             )
 
         self.metadata = pd.read_csv(self._processed_dir / self.LABELS_FILENAME)
         # Divide up the dataframe into its constituent arrays because indexing with pandas is
         # considerably slower than indexing with numpy/torch
         x = self.metadata["path"].to_numpy()
-        s = torch.as_tensor(self.metadata[str(context_attr)], dtype=torch.int32)
-        y = torch.as_tensor(self.metadata[str(target_attr)], dtype=torch.int32)
+        s = torch.as_tensor(self.metadata[str(self.context_attr)], dtype=torch.int32)
+        y = torch.as_tensor(self.metadata[str(self.target_attr)], dtype=torch.int32)
 
         super().__init__(x=x, y=y, s=s, transform=transform, image_dir=self._processed_dir)
 
     def _check_downloaded(self) -> bool:
         return (self._raw_dir / "images").exists() and (
             self._raw_dir / self.METADATA_FILENAME
         ).exists()
@@ -101,16 +108,15 @@
         it = iter(it)
         return iter(lambda: list(islice(it, size)), [])  # this is magic from stackoverflow
 
     def _download_isic_metadata(self) -> pd.DataFrame:
         """Downloads the metadata CSV from the ISIC website."""
         self._raw_dir.mkdir(parents=True, exist_ok=True)
         req = requests.get(
-            f"{self._REST_API_URL}/image?limit={self.max_samples}"
-            f"&sort=name&sortdir=1&detail=false"
+            f"{self._REST_API_URL}/image?limit={self.max_samples}&sort=name&sortdir=1&detail=false"
         )
         image_ids = req.json()
         image_ids = [image_id["_id"] for image_id in image_ids]
 
         template_start = "?limit=300&sort=name&sortdir=1&detail=true&imageIds=%5B%22"
         template_sep = "%22%2C%22"
         template_end = "%22%5D"
@@ -140,15 +146,15 @@
 
     def _download_isic_images(self) -> None:
         """Given the metadata CSV, downloads the ISIC images."""
         metadata_path = self._raw_dir / self.METADATA_FILENAME
         if not metadata_path.is_file():
             raise FileNotFoundError(
                 f"{self.METADATA_FILENAME} not downloaded. "
-                f"Run 'download_isic_data` before this function."
+                "Run 'download_isic_data` before this function."
             )
         metadata_df = pd.read_csv(metadata_path)
         metadata_df = metadata_df.set_index("_id")
 
         template_start = "?include=images&imageIds=%5B%22"
         template_sep = "%22%2C%22"
         template_end = "%22%5D"
@@ -185,15 +191,15 @@
             )
         metadata_df = pd.read_csv(metadata_path)
         metadata_df = metadata_df.set_index("_id")
         labels_df = self._remove_uncertain_diagnoses(metadata_df)
         labels_df = self._add_patch_column(labels_df)
 
         labels_df["path"] = (
-            str(self._processed_dir)  # type: ignore
+            str(self._processed_dir)
             + os.sep
             + "ISIC-images"
             + os.sep
             + labels_df["dataset.name"]
             + os.sep
             + labels_df["name"]
             + ".jpg"
@@ -241,26 +247,26 @@
         malignant_mask = labels_df["meta.clinical.benign_malignant"] == "malignant"
         labels_df["malignant"] = malignant_mask.astype("uint8")
 
         labels_df["meta.clinical.diagnosis_confirm_type"].fillna(
             value="non-histopathology", inplace=True
         )
         histopathology_mask = labels_df["meta.clinical.diagnosis_confirm_type"] == "histopathology"
-        labels_df["histo"] = histopathology_mask.astype("uint8")  # type: ignore[arg-type]
+        labels_df["histo"] = histopathology_mask.astype("uint8")
 
         return labels_df
 
     @staticmethod
     def _add_patch_column(labels_df: pd.DataFrame) -> pd.DataFrame:
         """Adds a patch column to the input DataFrame."""
         patch_mask = labels_df["dataset.name"] == "SONIC"
         # add to labels_df
         labels_df["patch"] = None
-        labels_df.loc[patch_mask, "patch"] = 1  # type: ignore[index]
-        labels_df.loc[~patch_mask, "patch"] = 0  # type: ignore[index]
+        labels_df.loc[patch_mask, "patch"] = 1
+        labels_df.loc[~patch_mask, "patch"] = 0
         assert all(patch is not None for patch in labels_df["patch"])
         return labels_df
 
     def _download_data(self) -> None:
         """Attempt to download data if files cannot be found in the base folder."""
         # # Check whether the data has already been downloaded - if it has and the integrity
         # # of the files can be confirmed, then we are done
@@ -279,16 +285,16 @@
     def _preprocess_data(self) -> None:
         """Preprocess the downloaded data if the processed image-directory/metadata don't exist."""
         # If the data has already been processed, skip this operation
         if self._check_processed():
             self.logger.info("Metadata and images already preprocessed.")
             return
         self.logger.info(
-            f"Preprocessing metadata (adding columns, removing uncertain diagnoses) and saving into "
-            f"{str(self._processed_dir / self.LABELS_FILENAME)}..."
+            "Preprocessing metadata (adding columns, removing uncertain diagnoses) and saving into"
+            f" {str(self._processed_dir / self.LABELS_FILENAME)}..."
         )
         self._preprocess_isic_metadata()
         self.logger.info(
-            f"Preprocessing images (transforming to 3-channel RGB, resizing to 224x224) and saving "
+            "Preprocessing images (transforming to 3-channel RGB, resizing to 224x224) and saving "
             f"into{str(self._processed_dir / 'ISIC-images')}..."
         )
         self._preprocess_isic_images()
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/nico.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/nico.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,73 @@
 """NICO Dataset."""
-from enum import Enum, auto
+from enum import auto
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union, cast
 
 from PIL import Image, UnidentifiedImageError
 import pandas as pd
-from ranzen import parsable, str_to_enum
-from ranzen.decorators import enum_name_str
+from ranzen import StrEnum, parsable
 import torch
 from torch import Tensor
 from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import GdriveFileInfo, ImageTform, download_from_gdrive
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample
 
+from .base import CdtVisionDataset
+from .utils import ImageTform
+
 __all__ = [
     "NICO",
     "NicoSuperclass",
 ]
 
 
-@enum_name_str
-class NicoSuperclass(Enum):
-    animals = auto()
-    vehicles = auto()
+class NicoSuperclass(StrEnum):
+    ANIMALS = auto()
+    VEHICLES = auto()
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class NICO(CdtVisionDataset[TernarySample, Tensor, Tensor]):
     """Datset for Non-I.I.D. image classification introduced in
     'Towards Non-I.I.D. Image Classification: A Dataset and Baselines'
     """
 
+    SampleType: TypeAlias = TernarySample
+    Superclass: TypeAlias = NicoSuperclass
+
     _FILE_INFO: ClassVar[GdriveFileInfo] = GdriveFileInfo(
         name="NICO.zip",
         id="1L6cHNhuwwvrolukBklFyhFu7Y8WUUIQ7",
         md5="78c686f84e31ad6b6c052f97ed5f532b",
     )
 
     @parsable
     def __init__(
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
-        superclass: Optional[Union[NicoSuperclass, str]] = NicoSuperclass.animals,
+        superclass: Optional[Union[NicoSuperclass, str]] = NicoSuperclass.ANIMALS,
     ) -> None:
-
-        self.superclass = (
-            str_to_enum(str_=superclass, enum=NicoSuperclass)
-            if isinstance(superclass, str)
-            else superclass
-        )
+        self.superclass = NicoSuperclass(superclass) if isinstance(superclass, str) else superclass
         self.root = Path(root)
         self.download = download
         self._base_dir = self.root / self.__class__.__name__
         self._metadata_path = self._base_dir / "metadata.csv"
 
         if self.download:
             download_from_gdrive(file_info=self._FILE_INFO, root=self.root, logger=self.logger)
         elif not self._check_unzipped():
             raise FileNotFoundError(
-                f"Data not found at location {self._base_dir.resolve()}. " "Have you downloaded it?"
+                f"Data not found at location {self._base_dir.resolve()}. Have you downloaded it?"
             )
         if not self._metadata_path.exists():
             self._extract_metadata()
 
         self.metadata = pd.read_csv(self._base_dir / "metadata.csv")
         self.class_tree = (
             self.metadata[["concept", "context"]]
@@ -104,15 +102,15 @@
         image_paths: List[Path] = []
         for ext in ("jpg", "jpeg", "png"):
             image_paths.extend(self._base_dir.glob(f"**/*.{ext}"))
         image_paths_str = [str(image.relative_to(self._base_dir)) for image in image_paths]
         filepaths = pd.Series(image_paths_str)
         metadata = cast(
             pd.DataFrame,
-            filepaths.str.split("/", expand=True).rename(  # type: ignore[attr-defined]
+            filepaths.str.split("/", expand=True).rename(
                 columns={0: "superclass", 1: "concept", 2: "context", 3: "filename"}
             ),
         )
         metadata["filepath"] = filepaths
         metadata.sort_index(axis=1, inplace=True)
         metadata.sort_values(by=["filepath"], axis=0, inplace=True)
         metadata = self._label_encode_metadata(metadata)
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/nih.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/nih.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, Optional, Union, cast
 
-import pandas as pd  # type: ignore
+import pandas as pd
 from ranzen import parsable, str_to_enum
-from sklearn.preprocessing import MultiLabelBinarizer  # type: ignore
+from sklearn.preprocessing import MultiLabelBinarizer
 import torch
+from torch import Tensor
 from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import ImageTform
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.structures import TernarySample
 
-__all__ = [
-    "NIHChestXRays",
-    "NIHSplit",
-    "NIHSubgroup",
-    "NIHTarget",
-]
+from .base import CdtVisionDataset
+from .utils import ImageTform
+
+__all__ = ["NIHChestXRays", "NIHSplit", "NIHSubgroup", "NIHTarget"]
 
 
 class NIHSplit(Enum):
     TRAIN = "train_val_list.txt"
     TEST = "test_list.txt"
 
 
@@ -63,29 +61,30 @@
     NODULE = "Nodule"
     PLEURAL_THICKENING = "Pleural_Thickening"
     PNEUMONIA = "Pneumonia"
     PNEUMOTHORAX = "Pneumothorax"
     FINDING = "No Finding"
 
 
-class NIHChestXRays(CdtVisionDataset):
+class NIHChestXRays(CdtVisionDataset[TernarySample, Tensor, Tensor]):
     """ "
     National Institutes of Health (NIH) chest X-Rays dataset.
     This NIH Chest X-rays dataset is comprised of 112,120 X-ray images with disease labels from
     30,805 unique patients. To create these labels, the authors used Natural Language Processing to
     text-mine disease classifications from the associated radiological reports. The labels are
     expected to be >90% accurate and suitable for weakly-supervised learning. The original radiology
     reports are not publicly available but you can find more details on the labeling process in
     `this
     <https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community>`__
     Open Access paper.
 
     The dataset can be downloaded by following the above link or from `kaggle <https://www.kaggle.com/datasets/nih-chest-xrays/data>`__
     """
 
+    SampleType: TypeAlias = TernarySample
     Target: TypeAlias = NIHTarget
     Subgroup: TypeAlias = NIHSubgroup
     Split: TypeAlias = NIHSplit
 
     _METADATA_FILENAME: ClassVar[str] = "Data_Entry_2017.csv"
     _BASE_DIR_NAME: ClassVar[str] = "nih_chest_x_rays"
 
@@ -98,25 +97,25 @@
         subgroup: Union[NIHSubgroup, str] = NIHSubgroup.GENDER,
         split: Optional[Union[NIHSplit, str]] = None,
         transform: Optional[ImageTform] = None,
         num_quantiles: Optional[float] = 4,
         download: bool = True,
     ) -> None:
         """
-        :param root: Root directory of dataset.
+        :param root: Root directory of the dataset.
         :param target: Attribute to set as the target attribute ('y').
         :param subgroup: Attribute to set as the subgroup attribute ('s').
         :param split: Which predefined split of the dataset to use. If ``None`` then the full
             (unsplit) dataset will be returned.
         :param transform: A function/transform that takes in a PIL or ndarray image and returns a
             transformed version. E.g, ``transforms.RandomCrop``.
         :param num_quantiles: Number of quantiles (equal-sized buckets) to bin 'Patient Age' into
             (only applicable when ``sens_attr=NIHSensAttr.AGE``). E.g. 10 for deciles, 4 for
             quartiles.
-        :param download: If ``True``, down;oads the dataset from the internet and puts it in the
+        :param download: If ``True``, downloads the dataset from the internet and puts it in the
             root directory. If the dataset is already downloaded, it is not downloaded again.
             This requires kaggle credentials.
         :raises FileNotFoundError: If ``download=False`` and an existing dataset cannot be found in
             the root directory.
         """
         self.root = Path(root)
         self._base_dir = self.root / self._BASE_DIR_NAME
@@ -149,24 +148,24 @@
         if self.split is not None:
             split_info = pd.read_csv(
                 self._base_dir / self.split.value, header=None, names=["Image Index"]
             )
             self.metadata = self.metadata.merge(split_info, on="Image Index")
 
         # In the case of Patient Gender, factorize yields the mapping: M -> 0, F -> 1
-        s_pd = cast(pd.Series, self.metadata[self.subgroup.value])
+        s_pd = self.metadata[self.subgroup.value]
         if (self.subgroup is NIHSubgroup.AGE) and (num_quantiles is not None):
             s_pd = cast(pd.Series, pd.qcut(s_pd, q=num_quantiles))
         s_pd_le = s_pd.factorize()[0]
         s = torch.as_tensor(s_pd_le, dtype=torch.long)
 
         findings_str = self.metadata["Finding Labels"].str.split("|")
         self.encoder = MultiLabelBinarizer().fit(findings_str)
         findings_ml = pd.DataFrame(
-            self.encoder.transform(findings_str), columns=self.encoder.classes_
+            self.encoder.transform(findings_str), columns=self.encoder.classes_  # type: ignore
         )
         self.metadata = pd.concat((self.metadata, findings_ml), axis=1)
         if self.target is None:
             findings_ml.drop("No Finding", axis=1, inplace=True)
         else:
             findings_ml = findings_ml[self.target.value]
             if self.target is NIHTarget.FINDING:
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/pacs.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/pacs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """PACS Dataset."""
-from enum import Enum, auto
+from enum import auto
 from pathlib import Path
-from typing import ClassVar, List, Optional, Union, cast
+from typing import ClassVar, List, Optional, Union
 
 import numpy as np
 import pandas as pd
-from ranzen import parsable, str_to_enum
-from ranzen.decorators import enum_name_str
+from ranzen import StrEnum, parsable, str_to_enum
 import torch
 from torch import Tensor
 from typing_extensions import Self, TypeAlias
 
-from conduit.data.datasets.utils import GdriveFileInfo, ImageTform, download_from_gdrive
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample, TrainTestSplit
 
+from .base import CdtVisionDataset
+from .utils import ImageTform
+
 __all__ = [
     "PACS",
     "PacsDomain",
 ]
 
 
 SampleType: TypeAlias = TernarySample
 
 
-@enum_name_str
-class PacsDomain(Enum):
-    photo = auto()
-    art_painting = auto()
-    cartoon = auto()
-    sketch = auto()
+class PacsDomain(StrEnum):
+    PHOTO = auto()
+    ART_PAINTING = auto()
+    CARTOON = auto()
+    SKETCH = auto()
 
 
 class PACS(CdtVisionDataset[TernarySample, Tensor, Tensor]):
     """
     PACS (photo (P), art painting (A), cartoon (C), and sketch (S)) dataset for evaluating domain
     generalisation as introduced in `PACS`_ 'Deeper, Broader and Artier Domain Generalization'.
 
     .. _PACS:
         https://arxiv.org/abs/1710.03077
     """
 
+    SampleType: TypeAlias = TernarySample
     Domain: TypeAlias = PacsDomain
 
     _FILE_INFO: ClassVar[GdriveFileInfo] = GdriveFileInfo(
         name="PACS.zip",
         id="1lNOnDplyxhdDdyfb4KRIh0p0uom8aS1i",
         md5="5e43a6e01e53567923621ae5ce025f4e",
     )
@@ -54,33 +55,32 @@
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
         domains: Optional[Union[Domain, str, List[Union[str, Domain]]]] = None,
     ) -> None:
-
         if isinstance(domains, str):
-            self.domains = str_to_enum(str_=domains, enum=PacsDomain)
+            self.domains = PacsDomain(domains)
         elif isinstance(domains, list):
-            domains = [str_to_enum(str_=elem, enum=PacsDomain) for elem in domains]
-            self.domains = cast(List[PacsDomain], domains)
+            domains_ = [PacsDomain(elem) for elem in domains]
+            self.domains = domains_
         else:
             self.domains = domains
 
         self.root = Path(root)
         self.download = download
         self._base_dir = self.root / self.__class__.__name__
         self._metadata_path = self._base_dir / "metadata.csv"
 
         if self.download:
             download_from_gdrive(file_info=self._FILE_INFO, root=self.root, logger=self.logger)
         elif not self._check_unzipped():
             raise FileNotFoundError(
-                f"Data not found at location {self._base_dir.resolve()}. " "Have you downloaded it?"
+                f"Data not found at location {self._base_dir.resolve()}. Have you downloaded it?"
             )
         if not self._metadata_path.exists():
             self._extract_metadata()
 
         self.metadata = pd.read_csv(self._base_dir / "metadata.csv")
 
         # Label decoders (for mapping from the label encodings back to their original string
@@ -113,19 +113,16 @@
         """Extract domain/class information from the image filepaths and it save to csv."""
         self.logger.info("Extracting metadata.")
         image_paths: List[Path] = []
         for ext in ("jpg", "jpeg", "png"):
             image_paths.extend(self._base_dir.glob(f"**/*.{ext}"))
         image_paths_str = [str(image.relative_to(self._base_dir)) for image in image_paths]
         filepaths = pd.Series(image_paths_str)
-        metadata = cast(
-            pd.DataFrame,
-            filepaths.str.split("/", expand=True).rename(  # type: ignore[attr-defined]
-                columns={0: "domain", 1: "class", 2: "filename"}
-            ),
+        metadata = filepaths.str.split("/", expand=True).rename(
+            columns={0: "domain", 1: "class", 2: "filename"}
         )
         metadata["filepath"] = filepaths
         metadata.sort_index(axis=1, inplace=True)
         metadata.sort_values(by=["filepath"], axis=0, inplace=True)
         metadata = self._label_encode_metadata(metadata)
         metadata.to_csv(self._metadata_path)
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/ssrp.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/ssrp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 """SSRP Dataset."""
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, List, Optional, Union, cast
 
 import pandas as pd
-from ranzen import parsable, str_to_enum
+from ranzen import parsable
 import torch
 from torch import Tensor
+from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import GdriveFileInfo, ImageTform, download_from_gdrive
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.datasets.utils import GdriveFileInfo, download_from_gdrive
 from conduit.data.structures import TernarySample
 
+from .base import CdtVisionDataset
+from .utils import ImageTform
+
 __all__ = ["SSRP", "SSRPSplit"]
 
 
 class SSRPSplit(Enum):
-    task = "Task"
-    pretrain = "Pre_Train"
+    TASK = "Task"
+    PRETRAIN = "Pre_Train"
 
 
 class SSRP(CdtVisionDataset[TernarySample, Tensor, Tensor]):
+    SampleType: TypeAlias = TernarySample
+    Split: TypeAlias = SSRPSplit
+
     _FILE_INFO: ClassVar[GdriveFileInfo] = GdriveFileInfo(
         name="ghaziabad.zip", id="1RE4srtC63VnyU0e1qx16QNdjyyQXg2hj"
     )
 
     @parsable
     def __init__(
         self,
         root: Union[str, Path],
         *,
-        split: Union[SSRPSplit, str] = SSRPSplit.pretrain,
+        split: Union[SSRPSplit, str] = SSRPSplit.PRETRAIN,
         download: bool = True,
         transform: Optional[ImageTform] = None,
     ) -> None:
         self.root = Path(root)
         self._base_dir = self.root / self.__class__.__name__
         self._metadata_path = self._base_dir / "metadata.csv"
         self.download = download
-        self.split = str_to_enum(str_=split, enum=SSRPSplit)
+        self.split = SSRPSplit(split)
 
         if self.download:
             download_from_gdrive(file_info=self._FILE_INFO, root=self._base_dir, logger=self.logger)
         if not self._check_unzipped():
             raise FileNotFoundError(
                 f"Data not found at location {self._base_dir.resolve()}. Have you downloaded it?"
             )
         if not self._metadata_path.exists():
             self._extract_metadata()
 
         self.metadata = pd.read_csv(self._base_dir / "metadata.csv")
-        self.metadata = cast(
-            pd.DataFrame, self.metadata[self.metadata.split.values == self.split.value]
-        )
+        self.metadata = self.metadata.loc[self.metadata["split"].to_numpy() == self.split.value]
 
         x = self.metadata["filepath"].to_numpy()
         y = torch.as_tensor(self.metadata["class_le"].to_numpy(), dtype=torch.long)
         s = torch.as_tensor(self.metadata["season_le"].to_numpy(), dtype=torch.long)
 
         super().__init__(x=x, y=y, s=s, transform=transform, image_dir=self._base_dir)
 
@@ -70,20 +74,20 @@
         for ext in ("jpg", "jpeg", "png"):
             # Glob images from child folders recusrively, excluding hidden files
             image_paths.extend(self._base_dir.glob(f"**/[!.]*.{ext}"))
         image_paths_str = [str(image.relative_to(self._base_dir)) for image in image_paths]
         filepaths = pd.Series(image_paths_str)
         metadata = cast(
             pd.DataFrame,
-            filepaths.str.split("/", expand=True)  # type: ignore[attr-defined]
+            filepaths.str.split("/", expand=True)
             .dropna(axis=1)
             .rename(columns={0: "region", 1: "split", 2: "class", 3: "filename"}),
         )
         # Extract the seasonal metadata from the filenames
-        metadata["season"] = metadata["filename"].str.split(r"\((.*?)\s.*", expand=True)[1]  # type: ignore[attr-defined]
+        metadata["season"] = metadata["filename"].str.split(r"\((.*?)\s.*", expand=True)[1]
         metadata["filepath"] = filepaths
         metadata.sort_index(axis=1, inplace=True)
         metadata.sort_values(by=["filepath"], axis=0, inplace=True)
         metadata = self._label_encode_metadata(metadata)
         metadata.to_csv(self._metadata_path)
 
     @staticmethod
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/vision/waterbirds.py` & `torch_conduit-0.2.0/conduit/data/datasets/vision/waterbirds/waterbirds.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,119 @@
 from enum import Enum
 from pathlib import Path
-from typing import ClassVar, Optional, Union, cast
+from typing import ClassVar, Optional, Union
 
 import pandas as pd
-from ranzen import parsable, str_to_enum
+from ranzen import parsable
 import torch
 from torch import Tensor
 from typing_extensions import TypeAlias
 
-from conduit.data.datasets.utils import ImageTform, UrlFileInfo, download_from_url
-from conduit.data.datasets.vision.base import CdtVisionDataset
+from conduit.data.datasets.utils import UrlFileInfo, download_from_url
+from conduit.data.datasets.vision import CdtVisionDataset, ImageTform
 from conduit.data.structures import TernarySample
 
-__all__ = ["Waterbirds", "WaterbirdsSplit"]
+__all__ = [
+    "Waterbirds",
+    "WaterbirdsSplit",
+    "SampleType",
+]
 
 
 class WaterbirdsSplit(Enum):
-    train = 0
-    val = 1
-    test = 2
+    TRAIN = 0
+    VAL = 1
+    TEST = 2
 
 
 SampleType: TypeAlias = TernarySample
 
 
 class Waterbirds(CdtVisionDataset[TernarySample, Tensor, Tensor]):
-    """The Waterbirds dataset.
+    """The Waterbirds dataset introduced in `GDRO`_.
 
     The dataset was constructed by cropping out birds from the Caltech-UCSD Birds-200-2011 (CUB) dataset
     and transferring them onto backgrounds from the Places dataset.
 
     The train-test split is the same as the one used for the CUB dataset, with 20% of the training data chosen to
     serve as a validation set. For the validation and test sets, landbirds and waterbirds are equally
     distributed across land and water backgrounds (i.e., there are the same number of landbirds on land
     vs. water backgrounds, and separately, the same number of waterbirds on land vs. water backgrounds).
     This allows us to more accurately measure the performance of the rare groups, and it is particularly
     important for the Waterbirds dataset because of its relatively small size; otherwise, the smaller groups
     (waterbirds on land and landbirds on water) would have too few samples to accurately estimate performance on.
+
+    .. _GDRO:
+        Generalization<https://arxiv.org/abs/1911.08731>`__
     """
 
+    SampleType: TypeAlias = TernarySample
+    Split: TypeAlias = WaterbirdsSplit
+
+    _BASE_DIR_NAME: ClassVar[str] = "Waterbirds"
+    _ORIGINAL_METADATA_FILENAME: ClassVar[str] = "metadata.csv"
+    # Path to the 'fixed' metadata featured in 'MaskTune' and downloaded from the link provided in
+    # the official repo of said paper:
+    # 'https://drive.google.com/file/d/1xPNYQskEXuPhuqT5Hj4hXPeJa9jh7liL/view'.
+    # To quote the paper:
+    # "We discovered and fixed two problems with the Waterbirds dataset: a) Because the background
+    # images in the Places dataset (Zhou et al., 2017) may already contain bird images, multiple
+    # birds may appear in an image after overlaying the segmented bird images from the Caltech-UCSD
+    # Birds- 200-2011 (CUB) dataset (Wah et al., 2011). For example, the label of an image may be
+    # “landbird”, but the image contains both land and water birds. Such images were removed from
+    # the dataset. b) Because the names of the species are similar, some land birds have been
+    # mislabeled as waterbirds"
+    _FIXED_METADATA_FILEPATH: ClassVar[Path] = Path(__file__).parent / "waterbirds_fixed.csv.zip"
+
     _FILE_INFO: ClassVar[UrlFileInfo] = UrlFileInfo(
         name="Waterbirds.tar.gz",
         url="https://worksheets.codalab.org/rest/bundles/0x505056d5cdea4e4eaa0e242cbfe2daa4/contents/blob/",
         md5=None,
     )
 
     @parsable
     def __init__(
         self,
         root: Union[str, Path],
         *,
         download: bool = True,
         transform: Optional[ImageTform] = None,
         split: Optional[Union[WaterbirdsSplit, str]] = None,
+        fixed: bool = False,
     ) -> None:
-
-        self.split = (
-            str_to_enum(str_=split, enum=WaterbirdsSplit) if isinstance(split, str) else split
-        )
+        self.split = WaterbirdsSplit[split.upper()] if isinstance(split, str) else split
         self.root = Path(root)
-        self._base_dir = self.root / self.__class__.__name__
+        self._base_dir = self.root / self._BASE_DIR_NAME
+        self.fixed = fixed
         self.download = download
         if self.download:
             download_from_url(
                 file_info=self._FILE_INFO,
                 root=self.root,
                 logger=self.logger,
                 remove_finished=True,
             )
         elif not self._check_unzipped():
             raise FileNotFoundError(
                 f"Data not found at location {self._base_dir.resolve()}. Have you downloaded it?"
             )
 
+        metadata_fp = (
+            self._FIXED_METADATA_FILEPATH
+            if self.fixed
+            else self._base_dir / self._ORIGINAL_METADATA_FILENAME
+        )
         # Read in metadata
         # Note: metadata is one-indexed.
-        self.metadata = pd.read_csv(self._base_dir / 'metadata.csv')
+        self.metadata = pd.read_csv(metadata_fp)
         # Use an official split of the data, if specified, else just use all
         # of the data
         if self.split is not None:
             split_indices = self.metadata["split"] == self.split.value
-            self.metadata = cast(pd.DataFrame, self.metadata[split_indices])
+            self.metadata = self.metadata.loc[split_indices]
 
         # Extract filenames
         x = self.metadata['img_filename'].to_numpy()
         # Extract class (land- vs. water-bird) labels
         y = torch.as_tensor(self.metadata["y"].to_numpy(), dtype=torch.long)
         # Extract place (land vs. water) labels
         s = torch.as_tensor(self.metadata["place"].to_numpy(), dtype=torch.long)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torch-conduit-0.1.7/conduit/data/datasets/wrappers.py` & `torch_conduit-0.2.0/conduit/data/datasets/wrappers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,124 +1,55 @@
 """Dataset wrappers."""
 from dataclasses import is_dataclass, replace
 from typing import Any, Optional, Tuple, Union
 
-from PIL import Image
-import numpy as np
-from ranzen.decorators import implements
-import torch
 from torch import Tensor
+from typing_extensions import override
 
 from conduit.data.datasets.utils import (
     AudioTform,
-    ImageTform,
     apply_audio_transform,
-    apply_image_transform,
     compute_instance_weights,
-    extract_base_dataset,
 )
-from conduit.data.datasets.vision.base import CdtVisionDataset
 from conduit.data.structures import (
     BinarySample,
     BinarySampleIW,
     Dataset,
     DatasetWrapper,
     NamedSample,
-    RawImage,
     SampleBase,
     SubgroupSample,
     TernarySample,
     TernarySampleIW,
     _BinarySampleMixin,
     shallow_asdict,
 )
 from conduit.transforms.tabular import TabularTransform
 
 __all__ = [
     "AudioTransformer",
-    "ImageTransformer",
     "InstanceWeightedDataset",
     "TabularTransformer",
 ]
 
 
-class ImageTransformer(DatasetWrapper[Any]):
-    """
-    Wrapper class for applying image transformations.
-
-    Useful when wanting to have different transformations for different subsets of the data
-    that share the same underlying dataset.
-    """
-
-    def __init__(self, dataset: Dataset, *, transform: Optional[ImageTform]) -> None:
-        self.dataset = dataset
-        self._transform: Optional[ImageTform] = None
-        self.transform = transform
-
-    @property
-    def transform(self) -> Optional[ImageTform]:
-        return self._transform
-
-    @transform.setter
-    def transform(self, transform: Optional[ImageTform]) -> None:
-        base_dataset = extract_base_dataset(self.dataset, return_subset_indices=False)
-        if isinstance(base_dataset, CdtVisionDataset):
-            base_dataset.update_il_backend(transform)
-        self._transform = transform
-
-    @implements(DatasetWrapper)
-    def __getitem__(self, index: int) -> Any:
-        sample = self.dataset[index]
-
-        def _transform_sample(
-            _sample: Union[RawImage, SampleBase, Tuple[Union[RawImage, Image.Image], ...]]
-        ) -> Any:
-            if self.transform is None:
-                return _sample
-            if isinstance(_sample, (Image.Image, np.ndarray)):
-                return apply_image_transform(image=_sample, transform=self.transform)
-            elif isinstance(_sample, SampleBase):
-                image = _sample.x
-                if isinstance(image, list):
-                    image = [_transform_sample(elem) for elem in image]
-                    if isinstance(image[0], Tensor):
-                        image = torch.stack(image, dim=0)
-                    elif isinstance(image[0], np.ndarray):
-                        image = np.stack(image, axis=0)
-
-                elif not isinstance(image, (Image.Image, np.ndarray)):
-                    raise TypeError(
-                        f"Image transform cannot be applied to input of type '{type(image)}'"
-                        "(must be a PIL Image or a numpy array)."
-                    )
-                else:
-                    image = apply_image_transform(image=image, transform=self.transform)
-                return replace(_sample, x=image)
-            else:
-                image = apply_image_transform(image=_sample[0], transform=self.transform)
-                data_type = type(_sample)
-                return data_type(image, *_sample[1:])  # type: ignore
-
-        return _transform_sample(sample)
-
-
 class AudioTransformer(DatasetWrapper[Any]):
     """
     Wrapper class for applying image transformations.
 
     Useful when wanting to have different transformations for different subsets of the data
     that share the same underlying dataset.
     """
 
     def __init__(self, dataset: Dataset, *, transform: Optional[AudioTform]) -> None:
         self.dataset = dataset
-        self._transform: Optional[ImageTform] = None
+        self._transform: Optional[AudioTform] = None
         self.transform = transform
 
-    @implements(DatasetWrapper)
+    @override
     def __getitem__(self, index: int) -> Any:
         sample = self.dataset[index]
         if self.transform is not None:
             if isinstance(sample, SampleBase):
                 if not isinstance(sample.x, Tensor):
                     raise TypeError(
                         f"Audio transform cannot be applied to input of type '{type(sample.x)}'"
@@ -150,15 +81,15 @@
         transform: Optional[TabularTransform],
         target_transform: Optional[TabularTransform],
     ) -> None:
         self.dataset = dataset
         self.transform = transform
         self.target_transform = target_transform
 
-    @implements(DatasetWrapper)
+    @override
     def __getitem__(self, index: int) -> Any:
         sample = self.dataset[index]
         if self.transform is not None:
             if isinstance(sample, SampleBase):
                 if not isinstance(sample.x, Tensor):
                     raise TypeError(
                         f"Tabular transform cannot be applied to input of type '{type(sample.x)}'"
@@ -191,15 +122,15 @@
 class InstanceWeightedDataset(DatasetWrapper[Any]):
     """Wrapper endowing datasets with instance-weights."""
 
     def __init__(self, dataset: Dataset) -> None:
         self.dataset = dataset
         self.iw = compute_instance_weights(dataset)
 
-    @implements(DatasetWrapper)
+    @override
     def __getitem__(self, index: int) -> Union[NamedSample, Tuple[Any, ...]]:
         sample = self.dataset[index]
         iw = self.iw[index]
         if isinstance(sample, (BinarySample, SubgroupSample, TernarySample)):
             return sample.add_field(iw=iw)
         elif isinstance(sample, tuple):
             if len(sample) == 2:
```

### Comparing `torch-conduit-0.1.7/conduit/data/structures.py` & `torch_conduit-0.2.0/conduit/data/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     Optional,
     Protocol,
     Tuple,
     TypeVar,
     Union,
     cast,
     overload,
+    runtime_checkable,
 )
 
 from PIL import Image
 import attr
 import numpy as np
 import numpy.typing as npt
-from ranzen.decorators import implements
 from ranzen.misc import gcopy, reduce_add
 from ranzen.types import Addable
 import torch
 from torch import Tensor
-from typing_extensions import Self, TypeAlias, runtime_checkable
+from typing_extensions import Self, TypeAlias, override
 
 from conduit.types import IndexType, Sized
 
 __all__ = [
     "BinarySample",
     "BinarySampleIW",
     "Dataset",
@@ -91,17 +91,15 @@
 X_co = TypeVar("X_co", bound=LoadedData, covariant=True)
 XI = TypeVar("XI", bound=IndexabledData)
 
 TargetData: TypeAlias = Union[Tensor, npt.NDArray[np.floating], npt.NDArray[np.integer]]
 
 
 def concatenate_inputs(x1: X, x2: X, *, is_batched: bool) -> X:
-    if type(x1) != type(x2) or (
-        isinstance(x1, list) and type(x1[0]) != type(cast(List, x2)[0])  # type: ignore
-    ):
+    if type(x1) != type(x2) or (isinstance(x1, list) and type(x1[0]) != type(cast(List, x2)[0])):
         raise AttributeError("Only data of the same type can be concatenated (added) together.")
     if isinstance(x1, Tensor):
         # if the number of dimensions is different by 1, append a batch dimension.
         ndim_diff = x1.ndim - x2.ndim  # type: ignore
         if ndim_diff == 1:
             x2 = x2.unsqueeze(0)  # type: ignore
         elif ndim_diff == -1:
@@ -141,20 +139,20 @@
 
         :param sequence: Sequence of containers to be collated.
 
         :returns: A collated container.
         """
         return reduce_add(sequence)
 
-    @implements(Sized)
+    @override
     def __len__(self) -> int:
         """Total number of samples in the container."""
         ...
 
-    @implements(Addable)
+    @override
     def __add__(self, other: Self) -> Self:
         ...
 
     def to(
         self,
         device: Optional[Union[torch.device, str]],
         *,
@@ -172,60 +170,60 @@
     local_crops: List[Tensor] = field(default_factory=list)
 
     @property
     def all_crops(self) -> List[Tensor]:
         return self.global_crops + self.local_crops
 
     @property
-    def global_crop_sizes(self):
+    def global_crop_sizes(self) -> List[torch.Size]:
         return [crop.shape[-3:] for crop in self.global_crops]
 
     @property
-    def local_crop_sizes(self):
+    def local_crop_sizes(self) -> List[torch.Size]:
         return [crop.shape[-3:] for crop in self.local_crops]
 
     @property
-    def shape(self):
+    def shape(self) -> torch.Size:
         """Shape of the global crops - for compatibility with DMs."""
         return self.global_crops[0].shape
 
-    @implements(InputContainer)
+    @override
     def __len__(self) -> int:
         """Total number of crops."""
         return len(self.global_crops) + len(self.local_crops)
 
     def __iadd__(self, other: Self) -> Self:
         self.global_crops += other.global_crops
         self.local_crops += other.local_crops
         return self
 
-    @implements(InputContainer)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.global_crops = copy.global_crops + other.global_crops
         copy.local_crops = copy.local_crops + other.local_crops
         return copy
 
 
 IS = TypeVar("IS", bound="SampleBase[IndexabledData]")
 
 
 @dataclass
 class SampleBase(InputContainer[X]):
     x: X
 
-    @implements(InputContainer)
+    @override
     def __len__(self) -> int:
-        return len(self.__dataclass_fields__)  # type: ignore[attr-defined]
+        return len(self.__dataclass_fields__)
 
     @abstractmethod
     def __iter__(self) -> Iterator[X]:
         ...
 
-    @implements(InputContainer)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.x = concatenate_inputs(copy.x, other.x, is_batched=True)
         return copy
 
     def astuple(self, deep=False) -> Tuple[X]:
         tuple_ = tuple(iter(self))
@@ -273,19 +271,19 @@
                     return TernarySampleIW(x=self.x, s=s, y=y, iw=iw)
                 return TernarySample(x=self.x, s=s, y=y)
             if iw is not None:
                 return BinarySampleIW(x=self.x, y=y, iw=iw)
             return BinarySample(x=self.x, y=y)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[X]:
         yield self.x
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "NamedSample[XI]", index: IndexType) -> "NamedSample[XI]":
         return gcopy(self, deep=False, x=self.x[index])
 
 
 @dataclass
 class _BinarySampleMixin:
     y: Tensor
@@ -321,26 +319,26 @@
             if iw is not None:
                 return TernarySampleIW(x=self.x, s=s, y=self.y, iw=iw)
             return TernarySample(x=self.x, s=s, y=self.y)
         if iw is not None:
             return BinarySampleIW(x=self.x, y=self.y, iw=iw)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.y)
 
-    @implements(NamedSample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.y = torch.cat([copy.y, other.y], dim=0)
         copy.x = concatenate_inputs(copy.x, other.x, is_batched=len(copy.y) > 1)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "BinarySample[XI]", index: IndexType) -> "BinarySample[XI]":
         return gcopy(self, deep=False, x=self.x[index], y=self.y[index])
 
 
 @dataclass
 class SubgroupSample(NamedSample[X], _SubgroupSampleMixin):
     @overload
@@ -366,26 +364,26 @@
             if iw is not None:
                 return TernarySampleIW(x=self.x, s=self.s, y=y, iw=iw)
             return TernarySample(x=self.x, s=self.s, y=y)
         if iw is not None:
             return SubgroupSampleIW(x=self.x, s=self.s, iw=iw)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.s)
 
-    @implements(NamedSample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.s = torch.cat([copy.s, other.s], dim=0)
         copy.x = concatenate_inputs(copy.x, other.x, is_batched=len(copy.s) > 1)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "SubgroupSample[XI]", index: IndexType) -> "SubgroupSample[XI]":
         return gcopy(self, deep=False, x=self.x[index], s=self.s[index])
 
 
 @dataclass
 class _IwMixin:
     iw: Tensor
@@ -402,25 +400,25 @@
         ...
 
     def add_field(self, s: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
         if s is not None:
             return TernarySampleIW(x=self.x, s=s, y=self.y, iw=self.iw)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.y, self.iw)
 
-    @implements(BinarySample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = super().__add__(other)
         copy.iw = torch.cat([copy.iw, other.iw], dim=0)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "BinarySampleIW[XI]", index: IndexType) -> "BinarySampleIW[XI]":
         return gcopy(self, deep=False, x=self.x[index], y=self.y[index], iw=self.iw[index])
 
 
 @dataclass
 class SubgroupSampleIW(SubgroupSample[X], _IwMixin):
     @overload
@@ -432,25 +430,25 @@
         ...
 
     def add_field(self, y: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
         if y is not None:
             return TernarySampleIW(x=self.x, s=self.s, y=y, iw=self.iw)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.s, self.iw)
 
-    @implements(SubgroupSample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = super().__add__(other)
         copy.iw = torch.cat([copy.iw, other.iw], dim=0)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "SubgroupSampleIW[XI]", index: IndexType) -> "SubgroupSampleIW[XI]":
         return gcopy(self, deep=False, x=self.x[index], s=self.s[index], iw=self.iw[index])
 
 
 @dataclass
 class TernarySample(BinarySample[X], _SubgroupSampleMixin):
     @overload
@@ -462,45 +460,45 @@
         ...
 
     def add_field(self, iw: Optional[Tensor] = None) -> Union[Self, "TernarySampleIW"]:
         if iw is not None:
             return TernarySampleIW(x=self.x, s=self.s, y=self.y, iw=iw)
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.y, self.s)
 
-    @implements(BinarySample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = super().__add__(other)
         copy.s = torch.cat([copy.s, other.s], dim=0)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "TernarySample[XI]", index: IndexType) -> "TernarySample[XI]":
         return gcopy(self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index])
 
 
 @dataclass
 class TernarySampleIW(TernarySample[X], _IwMixin):
     def add_field(self) -> Self:
         return self
 
-    @implements(SampleBase)
+    @override
     def __iter__(self) -> Iterator[LoadedData]:
         yield from (self.x, self.y, self.s, self.iw)
 
-    @implements(TernarySample)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = super().__add__(other)
         copy.iw = torch.cat([copy.iw, other.iw], dim=0)
         return copy
 
-    @implements(SampleBase)
+    @override
     def __getitem__(self: "TernarySampleIW[XI]", index: IndexType) -> "TernarySampleIW[XI]":
         return gcopy(
             self, deep=False, x=self.x[index], y=self.y[index], s=self.s[index], iw=self.iw[index]
         )
 
 
 def shallow_astuple(dataclass: object) -> Tuple[Any, ...]:
@@ -578,19 +576,19 @@
 class Dataset(Protocol[R_co]):
     def __getitem__(self, index: int) -> R_co:
         ...
 
 
 @runtime_checkable
 class SizedDataset(Dataset[R_co], Sized, Protocol):
-    @implements(Dataset)
+    @override
     def __getitem__(self, index: int) -> R_co:
         ...
 
-    @implements(Sized)
+    @override
     def __len__(self) -> int:
         ...
 
 
 X2 = TypeVar("X2", bound=UnloadedData)
 Y = TypeVar("Y", Tensor, None)
 S = TypeVar("S", Tensor, None)
@@ -612,28 +610,27 @@
 D = TypeVar("D", bound=Union[Dataset, Tensor, List[int]])
 
 
 @runtime_checkable
 class DatasetWrapper(SizedDataset[R_co], Protocol):
     dataset: Dataset
 
-    @implements(SizedDataset)
+    @override
     def __getitem__(self, index: int) -> R_co:
         ...
 
-    @implements(SizedDataset)
+    @override
     def __len__(self) -> Optional[int]:
         if isinstance(self.dataset, SizedDataset):
             return len(self.dataset)
         return None
 
 
 @attr.define(kw_only=True)
 class TrainTestSplit(Generic[D]):
-
     train: D
     test: D
 
     def __iter__(self) -> Iterator[D]:
         yield from (self.train, self.test)
```

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/admissions.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/admissions.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/adult.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/adult.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/base.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Tabular data-module."""
 from abc import abstractmethod
 from typing import Dict, List, Optional, Union, cast
 
 import attr
 import ethicml as em
 from ethicml.data import Dataset, FeatureOrder
-from pytorch_lightning import LightningDataModule
-from ranzen import implements
-from sklearn.preprocessing import StandardScaler  # type: ignore
-from typing_extensions import final
+from sklearn.preprocessing import StandardScaler
+from typing_extensions import final, override
 
 from conduit.data.datamodules import CdtDataModule
 from conduit.data.structures import TrainValTestSplit
 from conduit.fair.data.datasets import DataTupleDataset
 
 __all__ = ["EthicMlDataModule"]
 
@@ -55,19 +53,19 @@
             train_len -= test_len
             splits = [train_len, test_len]
         else:
             raise ValueError(f"Unsupported type {type(test_prop)}")
 
         return splits
 
-    @implements(LightningDataModule)
+    @override
     def prepare_data(self) -> None:
         self.make_feature_groups()
 
-    @implements(CdtDataModule)
+    @override
     def _get_splits(self) -> TrainValTestSplit[DataTupleDataset]:
         self._datatuple = self.em_dataset.load(order=FeatureOrder.disc_first)
 
         data_len = int(self._datatuple.x.shape[0])
         num_train_val, num_test = self._get_split_sizes(data_len, test_prop=self.test_prop)
         train_val, test_data = em.train_test_split(
             data=self._datatuple,
@@ -78,15 +76,15 @@
         train_data, val_data = em.train_test_split(
             data=train_val,
             train_percentage=(1 - (num_val / num_train_val)),
             random_seed=self.seed,
         )
 
         self._train_datatuple, self.scaler = em.scale_continuous(
-            self.em_dataset, datatuple=train_data, scaler=self.scaler  # type: ignore
+            self.em_dataset, datatuple=train_data, scaler=self.scaler
         )
         self._val_datatuple, _ = em.scale_continuous(
             self.em_dataset, datatuple=val_data, scaler=self.scaler, fit=False
         )
         self._test_datatuple, _ = em.scale_continuous(
             self.em_dataset, datatuple=test_data, scaler=self.scaler, fit=False
         )
```

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/compas.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/compas.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/credit.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/credit.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/crime.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/crime.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/german.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/german.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/health.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/health.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/law.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/law.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datamodules/tabular/sqf.py` & `torch_conduit-0.2.0/conduit/fair/data/datamodules/tabular/sqf.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datasets/dummy.py` & `torch_conduit-0.2.0/conduit/fair/data/datasets/dummy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from conduit.data.datasets.base import CdtDataset
 
 __all__ = ["DummyDataset"]
 
 
 class DummyDataset(CdtDataset):
-    """Generate a dummy dataset."""
+    """Generate a dummy dataset.
+
+    :param shapes: list of shapes
+    :param num_samples: how many samples to use in this dataset
+    :param seed: random seed
+    """
 
     def __init__(
         self, *shapes: Tuple[int, ...], num_samples: int = 10000, seed: Optional[int] = None
     ) -> None:
-        """
-        :param *shapes: list of shapes
-        :param num_samples: how many samples to use in this dataset
-        """
         self.shapes = shapes
         self.num_samples = num_samples
 
         self.generator = (
             torch.default_generator if seed is None else torch.Generator().manual_seed(seed)
         )
```

### Comparing `torch-conduit-0.1.7/conduit/fair/data/datasets/ethicml.py` & `torch_conduit-0.2.0/conduit/fair/data/datasets/ethicml.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/fair/losses/loss.py` & `torch_conduit-0.2.0/conduit/fair/losses/loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ranzen.decorators import implements
 from torch import Tensor, nn
+from typing_extensions import override
 
 from conduit.types import Loss
 
 __all__ = ["OnlineReweightingLoss"]
 
 
 class OnlineReweightingLoss(nn.Module):
@@ -12,15 +12,15 @@
     def __init__(self, loss_fn: Loss) -> None:
         super().__init__()
         # the base loss function needs to produce instance-wise losses for the
         # reweighting (determined by subgroup cardinality) to be applied
         loss_fn.reduction = "none"
         self.loss_fn = loss_fn
 
-    @implements(nn.Module)
+    @override
     def forward(self, logits: Tensor, targets: Tensor, subgroup_inf: Tensor) -> Tensor:
         unweighted_loss = self.loss_fn(logits, targets)
         for _y in targets.unique():
             for _s in subgroup_inf.unique():
                 # compute the cardinality of each subgroup and use this to weight the sample-losses
                 mask = (targets == _y) & (subgroup_inf == _s)
                 unweighted_loss[mask] /= mask.sum()
```

### Comparing `torch-conduit-0.1.7/conduit/hydra/conduit/data/datamodules/conf.py` & `torch_conduit-0.2.0/conduit/hydra/conduit/data/datamodules/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 # See https://github.com/facebookresearch/hydra/tree/master/tools/configen
 # fmt: off
 # isort:skip_file
 # flake8: noqa
 
 from dataclasses import dataclass, field
 from builtins import dict
+from conduit.data.datasets.audio.ecoacoustics import SoundscapeAttr
 from conduit.data.datasets.vision.camelyon17 import Camelyon17Attr
 from conduit.data.datasets.vision.camelyon17 import Camelyon17SplitScheme
 from conduit.data.datasets.vision.celeba import CelebAttr
 from conduit.data.datasets.vision.nico import NicoSuperclass
 from omegaconf import MISSING
+from pathlib import Path
 from ranzen.torch.data import TrainingMode
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Union
 
 
 @dataclass
 class CelebADataModuleConf:
     _target_: str = "conduit.data.datamodules.CelebADataModule"
     train_batch_size: int = 64
     eval_batch_size: Optional[int] = None
@@ -28,20 +31,20 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
-    train_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    test_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    root: Union[str, Path] = MISSING
+    train_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    test_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     image_size: int = 224
-    superclass: CelebAttr = CelebAttr.Smiling
-    subclass: CelebAttr = CelebAttr.Male
+    superclass: CelebAttr = CelebAttr.SMILING
+    subclass: CelebAttr = CelebAttr.MALE
     use_predefined_splits: bool = False
 
 
 @dataclass
 class ColoredMNISTDataModuleConf:
     _target_: str = "conduit.data.datamodules.ColoredMNISTDataModule"
     train_batch_size: int = 64
@@ -51,17 +54,17 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
-    train_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    test_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    root: Union[str, Path] = MISSING
+    train_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    test_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     image_size: int = 32
     use_predefined_splits: bool = False
     label_map: Optional[Dict[str, int]] = None
     colors: Optional[List[int]] = None
     num_colors: int = 10
     scale: float = 0.2
     correlation: float = 1.0
@@ -81,20 +84,20 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
-    train_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    test_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    root: Union[str, Path] = MISSING
+    train_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    test_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     image_size: int = 224
     class_train_props: Optional[dict] = None
-    superclass: NicoSuperclass = NicoSuperclass.animals
+    superclass: NicoSuperclass = NicoSuperclass.ANIMALS
 
 
 @dataclass
 class WaterbirdsDataModuleConf:
     _target_: str = "conduit.data.datamodules.WaterbirdsDataModule"
     train_batch_size: int = 64
     eval_batch_size: Optional[int] = None
@@ -103,17 +106,17 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
-    train_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    test_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    root: Union[str, Path] = MISSING
+    train_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    test_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     image_size: int = 224
     use_predefined_splits: bool = False
 
 
 @dataclass
 class Camelyon17DataModuleConf:
     _target_: str = "conduit.data.datamodules.Camelyon17DataModule"
@@ -124,22 +127,22 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
-    train_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    test_transforms: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    root: Union[str, Path] = MISSING
+    train_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    test_transforms: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     image_size: int = 96
-    superclass: Camelyon17Attr = Camelyon17Attr.tumor
-    subclass: Camelyon17Attr = Camelyon17Attr.center
+    superclass: Camelyon17Attr = Camelyon17Attr.TUMOR
+    subclass: Camelyon17Attr = Camelyon17Attr.CENTER
     use_predefined_splits: bool = False
-    split_scheme: Camelyon17SplitScheme = Camelyon17SplitScheme.official
+    split_scheme: Camelyon17SplitScheme = Camelyon17SplitScheme.OFFICIAL
 
 
 @dataclass
 class EcoacousticsDataModuleConf:
     _target_: str = "conduit.data.datamodules.EcoacousticsDataModule"
     train_batch_size: int = 64
     eval_batch_size: Optional[int] = None
@@ -148,12 +151,13 @@
     num_workers: int = 0
     seed: int = 47
     persist_workers: bool = False
     pin_memory: bool = True
     stratified_sampling: bool = False
     instance_weighting: bool = False
     training_mode: TrainingMode = TrainingMode.epoch
-    root: Any = MISSING  # Union[str, Path]
+    root: str = MISSING
     train_transforms: Any = None  # Optional[Callable[[Tensor], Tensor]]
     test_transforms: Any = None  # Optional[Callable[[Tensor], Tensor]]
     segment_len: float = 15
-    target_attrs: Any = MISSING  # Union[SoundscapeAttr, str, List[Union[SoundscapeAttr, str]]]
+    sample_rate: int = 48000
+    target_attrs: List[SoundscapeAttr] = MISSING
```

### Comparing `torch-conduit-0.1.7/conduit/hydra/conduit/data/datasets/conf.py` & `torch_conduit-0.2.0/conduit/hydra/conduit/data/datasets/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,108 +3,114 @@
 # fmt: off
 # isort:skip_file
 # flake8: noqa
 
 from dataclasses import dataclass, field
 from conduit.data.datasets.audio.ecoacoustics import SoundscapeAttr
 from conduit.data.datasets.vision.camelyon17 import Camelyon17Attr
+from conduit.data.datasets.vision.camelyon17 import Camelyon17Split
 from conduit.data.datasets.vision.camelyon17 import Camelyon17SplitScheme
+from conduit.data.datasets.vision.celeba import CelebASplit
 from conduit.data.datasets.vision.celeba import CelebAttr
+from conduit.data.datasets.vision.cmnist import ColoredMNISTSplit
 from conduit.data.datasets.vision.isic import IsicAttr
 from conduit.data.datasets.vision.nico import NicoSuperclass
 from conduit.data.datasets.vision.ssrp import SSRPSplit
+from conduit.data.datasets.vision.waterbirds import WaterbirdsSplit
 from omegaconf import MISSING
+from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Union
 
 
 @dataclass
 class CelebAConf:
     _target_: str = "conduit.data.datasets.CelebA"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
-    superclass: Any = CelebAttr.Smiling  # Union[CelebAttr, str]
-    subclass: Any = CelebAttr.Male  # Union[CelebAttr, str]
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    split: Any = None  # Union[CelebASplit, str, NoneType]
+    superclass: Union[CelebAttr, str] = CelebAttr.SMILING
+    subclass: Union[CelebAttr, str] = CelebAttr.MALE
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    split: Optional[Union[CelebASplit, str]] = None
 
 
 @dataclass
 class ColoredMNISTConf:
     _target_: str = "conduit.data.datasets.ColoredMNIST"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
     label_map: Optional[Dict[str, int]] = None
     colors: Optional[List[int]] = None
     num_colors: int = 10
     scale: float = 0.2
     correlation: Optional[float] = None
     binarize: bool = False
     greyscale: bool = False
     background: bool = False
     black: bool = True
-    split: Any = None  # Union[ColoredMNISTSplit, str, NoneType]
+    split: Optional[Union[ColoredMNISTSplit, str]] = None
     seed: Optional[int] = 42
 
 
 @dataclass
 class ISICConf:
     _target_: str = "conduit.data.datasets.ISIC"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
     max_samples: int = 25000
-    context_attr: IsicAttr = IsicAttr.histo
-    target_attr: IsicAttr = IsicAttr.malignant
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    context_attr: IsicAttr = IsicAttr.HISTO
+    target_attr: IsicAttr = IsicAttr.MALIGNANT
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
 
 
 @dataclass
 class NICOConf:
     _target_: str = "conduit.data.datasets.NICO"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    superclass: Any = NicoSuperclass.animals  # Union[NicoSuperclass, str, NoneType]
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    superclass: Optional[Union[NicoSuperclass, str]] = NicoSuperclass.ANIMALS
 
 
 @dataclass
 class SSRPConf:
     _target_: str = "conduit.data.datasets.SSRP"
-    root: Any = MISSING  # Union[str, Path]
-    split: Any = SSRPSplit.pretrain  # Union[SSRPSplit, str]
+    root: Union[str, Path] = MISSING
+    split: Union[SSRPSplit, str] = SSRPSplit.PRETRAIN
     download: bool = True
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
 
 
 @dataclass
 class WaterbirdsConf:
     _target_: str = "conduit.data.datasets.Waterbirds"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    split: Any = None  # Union[WaterbirdsSplit, str, NoneType]
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    split: Optional[Union[WaterbirdsSplit, str]] = None
 
 
 @dataclass
 class Camelyon17Conf:
     _target_: str = "conduit.data.datasets.Camelyon17"
-    root: Any = MISSING  # Union[str, Path]
+    root: Union[str, Path] = MISSING
     download: bool = True
-    transform: Any = None  # Union[Compose, BasicTransform, Callable[[Image], Any], NoneType]
-    split: Any = None  # Union[Camelyon17Split, str, NoneType]
-    split_scheme: Any = Camelyon17SplitScheme.official  # Union[Camelyon17SplitScheme, str]
-    superclass: Any = Camelyon17Attr.tumor  # Union[Camelyon17Attr, str]
-    subclass: Any = Camelyon17Attr.center  # Union[Camelyon17Attr, str]
+    transform: Any = None  # Optional[Union[Compose, BasicTransform, Callable[[Image], Any]]]
+    split: Optional[Union[Camelyon17Split, str]] = None
+    split_scheme: Union[Camelyon17SplitScheme, str] = Camelyon17SplitScheme.OFFICIAL
+    superclass: Union[Camelyon17Attr, str] = Camelyon17Attr.TUMOR
+    subclass: Union[Camelyon17Attr, str] = Camelyon17Attr.CENTER
 
 
 @dataclass
 class EcoacousticsConf:
     _target_: str = "conduit.data.datasets.Ecoacoustics"
-    root: Any = MISSING  # Union[str, Path]
+    root: str = MISSING
+    target_attrs: List[SoundscapeAttr] = MISSING
     transform: Any = None  # Optional[Callable[[Tensor], Tensor]]
     download: bool = True
-    target_attrs: Any = SoundscapeAttr.habitat  # Union[SoundscapeAttr, str, List[Union[SoundscapeAttr, str]]]
-    segment_len: Optional[float] = 15
-    preprocess: bool = False
+    segment_len: float = 15
+    sample_rate: int = 48000
```

### Comparing `torch-conduit-0.1.7/conduit/hydra/conduit/fair/data/datamodules/conf.py` & `torch_conduit-0.2.0/conduit/hydra/conduit/fair/data/datamodules/conf.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/metrics.py` & `torch_conduit-0.2.0/conduit/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import abstractmethod
 from enum import Enum
 from functools import partial, wraps
 from typing import (
     Callable,
     List,
     Literal,
     Optional,
@@ -20,36 +21,38 @@
     "Comparator",
     "accuracy",
     "accuracy_per_class",
     "accuracy_per_group",
     "accuracy_per_subclass",
     "balanced_accuracy",
     "fscore",
-    "fscore",
+    "fscore_per_class",
     "fscore_per_group",
     "fscore_per_subclass",
     "groupwise_metric",
     "hard_prediction",
     "macro_fscore",
     "max_difference_1d",
     "merge_indices",
     "nanmax",
     "nanmin",
+    "pdist_1d",
     "precision_at_k",
     "robust_accuracy",
     "robust_fscore",
     "robust_fscore_gap",
     "robust_gap",
     "robust_tnr",
     "robust_tpr",
     "subclass_balanced_accuracy",
     "subclasswise_metric",
     "tnr_per_subclass",
     "tpr_differences",
     "tpr_per_subclass",
+    "weighted_nanmean",
 ]
 
 
 @torch.no_grad()
 def hard_prediction(logits: Tensor) -> Tensor:
     logits = torch.atleast_1d(logits.squeeze())
     return (logits > 0).long() if logits.ndim == 1 else logits.argmax(dim=1)
@@ -85,62 +88,74 @@
     return res
 
 
 R = TypeVar("R", Tensor, Tuple[Tensor, Union[Tensor, slice]], covariant=True)
 
 
 class Comparator(Protocol[R]):
+    @abstractmethod
     def __call__(self, y_pred: Tensor, *, y_true: Tensor) -> R:
-        """
+        """Compare.
+
         :param y_pred: Predicted labels or raw logits of a classifier.
         :param y_true: Ground truth (correct) labels.
 
         :returns: An element-wise comparison between ``y_pred`` and ``y_true`` or a subset of them;
-        if the latter, the second element returned should be a mask indicating which samples
-        comprise that subset.
+            if the latter, the second element returned should be a mask indicating which samples
+            comprise that subset.
         """
         ...
 
 
 C = TypeVar("C", bound=Comparator)
 C_co = TypeVar("C_co", bound=Comparator, covariant=True)
 
 
 @torch.no_grad()
 def nanmax(x: Tensor) -> Tensor:
-    return torch.max(torch.nan_to_num(x, nan=float("-inf")))
+    return torch.amax(torch.nan_to_num(x, nan=-torch.inf))
 
 
 @torch.no_grad()
 def nanmin(x: Tensor) -> Tensor:
-    return torch.min(torch.nan_to_num(x, nan=float("inf")))
+    return torch.amin(torch.nan_to_num(x, nan=torch.inf))
 
 
 @torch.no_grad()
-def _pdist_1d(x: Tensor) -> Tensor:
-    return torch.pdist(x.view(-1, 1)).squeeze()
+def pdist_1d(x: Tensor) -> Tensor:
+    return (x - x.unsqueeze(-1)).abs().squeeze()
 
 
 @torch.no_grad()
 def max_difference_1d(x: Tensor) -> Tensor:
-    if x.numel() == 1:
-        return x.squeeze()
-    return nanmax(_pdist_1d(x))
+    return nanmax(pdist_1d(x))
+
+
+@torch.no_grad()
+def weighted_nanmean(x: Tensor, *, weights: Tensor) -> Tensor:
+    if x.numel() != weights.numel():
+        raise RuntimeError(
+            "'weights' and the input tensor being weighted, 'x', must match in size."
+        )
+    if torch.any(weights < 0):
+        raise RuntimeError("'weights' must contain only non-negative elements ")
+    denom = weights.nansum()
+    return (weights * x).nansum() / denom
 
 
 class Aggregator(Enum):
     MIN = (nanmin,)
     "Aggregate by taking the minimum."
     MAX = (nanmax,)
     "Aggregate by taking the maximum."
     MEAN = (torch.nanmean,)
     "Aggregate by taking the mean."
     MEADIAN = (torch.nanmedian,)
     "Aggregate by taking the median."
-    DIFF = (_pdist_1d,)
+    DIFF = (pdist_1d,)
     "Aggregate by taking the pairwise (absolute) differences."
     MAX_DIFF = (max_difference_1d,)
     "Aggregate by taking the maximum of the pairwise (absolute) differences."
 
     def __init__(self, fn: Callable[[Tensor], Tensor]) -> None:
         """
         Metric aggregator.
@@ -174,28 +189,32 @@
     *indices: Tensor, return_cardinalities: bool = False
 ) -> Union[Tensor, Tuple[Tensor, List[int]]]:
     """
     Bijectively merge a sequence of index tensors into a single index tensor, such that each
     combination of possible indices from across the elements in ``group_ids`` is assigned a unique
     index.
 
-    :param group_ids: A sequence of (long-type) index tensors.
+    :param indices: (Long-type) index tensors.
+    :param return_cardinalities: if ``True``, return sizes.
     :returns: A merged index set which uniquely indexes each possible combination in indices.
 
     :raises TypeError: If any elemnts of ``indices`` do not have dtype ``torch.long``.
     """
+    cards: Optional[List[int]] = None
+    if return_cardinalities:
+        cards = []
     group_ids_ls = list(indices)
-    index_set = group_ids_ls.pop().clone().squeeze()
-    cards = None
-    if index_set.dtype != torch.long:
+    first_elem = group_ids_ls.pop().clone().squeeze()
+    if first_elem.dtype != torch.long:
         raise TypeError("All index tensors must have dtype `torch.long'.")
+    unique_vals, unique_inv = first_elem.unique(return_inverse=True)
+    index_set = unique_inv
+    if cards is not None:
+        cards.append(len(unique_vals))
 
-    cards = None
-    if return_cardinalities:
-        cards = []
     for elem in group_ids_ls:
         elem = elem.squeeze()
         if elem.dtype != torch.long:
             raise TypeError("All index tensors must have dtype `torch.long'.")
         unique_vals, inv_indices = elem.unique(return_inverse=True)
         card = int(len(unique_vals))
         if cards is not None:
@@ -204,70 +223,78 @@
         index_set += cast(Tensor, inv_indices)
 
     if cards is None:
         return index_set
     return index_set, cards
 
 
+def nans(*sizes: int, device: Optional[torch.device] = None) -> Tensor:
+    return torch.full(tuple(sizes), fill_value=torch.nan, device=device)
+
+
+def nans_like(tensor: Tensor, *, device: Optional[torch.device] = None) -> Tensor:
+    return torch.full_like(tensor, fill_value=torch.nan, device=device)
+
+
 @torch.no_grad()
 def _apply_groupwise_metric(
     *group_ids: Tensor,
     comparator: Comparator,
     aggregator: Optional[Aggregator],
     y_pred: Tensor,
     y_true: Tensor,
 ) -> Tensor:
     """
     Computes a groupwise metric given a ``comparator`` and ``aggregator``.
 
     :param comparator: Function used to assess the correctness of ``y_pred`` with respect
-    to ``y_true``. Should return a score for each sample.
+        to ``y_true``. Should return a score for each sample.
 
     :param aggregator: Function with which to aggregate over the group-wise scores.
-    If ``None`` then no aggregation will be applied and scores will be returned for each
-    group.
+        If ``None`` then no aggregation will be applied and scores will be returned for each group.
 
     :param y_pred: Predictions to be scored
     :param y_true: Ground truth (correct) labels.
     :param group_ids: Ground truth labels indicating the group-membership of each sample.
 
     :returns: The score(s) as determined by the :attr:`comparator` and :attr:`aggregator`.
 
     :raises ValueError: If ``y_pred``, ``y_true``, and ``s`` do not match in size at dimension 0
-    (the 'batch' dimension).
-
+        (the 'batch' dimension).
     """
     y_pred = y_pred.squeeze()
     y_true = y_true.squeeze()
     index_set = None
 
     if group_ids:
         group_ids_ls = list(group_ids)
-        index_set = group_ids_ls.pop().clone().squeeze()
+        first_elem = group_ids_ls.pop().clone().squeeze()
+        index_set = first_elem.unique(return_inverse=True)[1]
 
         for elem in group_ids_ls:
             if len(y_pred) != len(y_true) != len(elem):
                 raise ValueError(
-                    "'y_pred', 'y_true', and all elements of 'group_ids' must match in size at dimension 0."
+                    "'y_pred', 'y_true', and all elements of 'group_ids' must match in size at"
+                    " dimension 0."
                 )
             elem = elem.squeeze()
             unique_vals, inv_indices = elem.unique(return_inverse=True)
-            index_set *= int(len(unique_vals))
+            index_set *= len(unique_vals)
             index_set += cast(Tensor, inv_indices)
 
     res = comparator(y_pred=y_pred, y_true=y_true)
     if isinstance(res, tuple):
         comps, comp_mask = res
     else:
         comps, comp_mask = res, slice(None)
 
     if index_set is not None:
         res = index_set.max()
         scores = torch.scatter_reduce(
-            input=torch.zeros(int(index_set.max() + 1)),
+            input=nans(int(index_set.max() + 1)),
             src=comps,
             dim=0,
             index=index_set[comp_mask],
             reduce="mean",
             include_self=False,
         )
         if aggregator is not None:
@@ -292,23 +319,21 @@
     def __call__(y_pred: Tensor, *, y_true: Tensor, s: Tensor) -> Tensor:
         ...
 
 
 def groupwise_metric(
     comparator: C, *, aggregator: A, cond_on_pred: bool = False
 ) -> GroupwiseMetric[C, A]:
-    """
-    Converts a given ``comparator`` and ``aggregator`` into a group-wise metric.
+    """Converts a given ``comparator`` and ``aggregator`` into a group-wise metric.
 
     :param comparator: Function used to assess the correctness of ``y_pred`` with respect
-    to ``y_true``. Should return a score for each sample.
-
+        to ``y_true``. Should return a score for each sample.
     :param aggregator: Function with which to aggregate over the group-wise scores.
-    If ``None`` then no aggregation will be applied and scores will be returned for each
-    group.
+        If ``None`` then no aggregation will be applied and scores will be returned for each group.
+    :param cond_on_pred: Whethr to condition on predictions.
 
     :returns: A group-wise metric formed from ``comparator`` and ``aggregator``.
     """
 
     @wraps(comparator)
     def _decorated_comparator(y_pred: Tensor, *, y_true: Tensor, s: Tensor) -> Tensor:
         return _apply_groupwise_metric(
@@ -324,23 +349,21 @@
 
 
 def subclasswise_metric(
     comparator: C,
     *,
     aggregator: A,
 ) -> GroupwiseMetric[C, A]:
-    """
-    Converts a given ``comparator`` and ``aggregator`` into a subclass-wise metric.
+    """Converts a given ``comparator`` and ``aggregator`` into a subclass-wise metric.
 
     :param comparator: Function used to assess the correctness of ``y_pred`` with respect
-    to ``y_true``. Should return a score for each sample.
+        to ``y_true``. Should return a score for each sample.
 
     :param aggregator: Function with which to aggregate over the subclass-wise scores.
-    If ``None`` then no aggregation will be applied and scores will be returned for each
-    group.
+        If ``None`` then no aggregation will be applied and scores will be returned for each group.
 
     :returns: A subclass-wise metric formed from ``comparator`` and ``aggregator``.
     """
 
     @wraps(comparator)
     def _decorated_comparator(y_pred: Tensor, *, y_true: Tensor, s: Tensor) -> Tensor:
         return _apply_groupwise_metric(
@@ -352,23 +375,22 @@
 
 def classwise_metric(
     comparator: C,
     *,
     aggregator: A,
     cond_on_pred: bool = False,
 ) -> Metric[C, A]:
-    """
-    Converts a given ``comparator`` and ``aggregator`` into a subclass-wise metric.
+    """Converts a given ``comparator`` and ``aggregator`` into a subclass-wise metric.
 
     :param comparator: Function used to assess the correctness of ``y_pred`` with respect
-    to ``y_true``. Should return a score for each sample.
+        to ``y_true``. Should return a score for each sample.
 
     :param aggregator: Function with which to aggregate over the subclass-wise scores.
-    If ``None`` then no aggregation will be applied and scores will be returned for each
-    group.
+        If ``None`` then no aggregation will be applied and scores will be returned for each group.
+    :param cond_on_pred: Whethr to condition on predictions.
 
     :returns: A subclass-wise metric formed from ``comparator`` and ``aggregator``.
     """
 
     @wraps(comparator)
     def _decorated_comparator(y_pred: Tensor, *, y_true: Tensor) -> Tensor:
         return _apply_groupwise_metric(
@@ -443,135 +465,207 @@
 )
 robust_tnr = subclasswise_metric(
     comparator=partial(conditional_equal, y_true_cond=0), aggregator=Aggregator.MIN
 )
 
 
 @torch.no_grad()
-def _pad_with_nans(n: int, *, src: Tensor, index: Tensor) -> Tensor:
-    nan_tensor = src.new_full((n,), fill_value=torch.nan)
-    return nan_tensor.scatter(0, src=src, index=index)
+def pad_to_size(size: int, *, src: Tensor, index: Tensor, value=0.0) -> Tensor:
+    padding = src.new_full((size,), fill_value=value)
+    return padding.scatter_(dim=0, src=src, index=index)
 
 
 def fscore(
     y_pred: Tensor,
     *,
     y_true: Tensor,
     s: Optional[Tensor] = None,
     beta: float = 1.0,
-    aggregator: Optional[Aggregator] = None,
     inner_summand: Optional[Literal["y_true", "s"]] = None,
+    ignore_unsupported: bool = True,
+    aggregator: Optional[Aggregator] = None,
 ) -> Tensor:
-    """
-    Computes the F-beta score between ``y_pred`` and ``y_true`` with optional subclass-conditioning.
+    """Computes F-beta score between ``y_pred`` and ``y_true`` with optional subclass-conditioning.
 
     :param y_pred: Predicted labels.
     :param y_true: Target labels.
     :param s: Subclass labels.
     :param beta: Beta coefficient that determines the weight of recall relative to precision.
-    ``beta < 1`` lends more weight to precision, while ``beta > 1`` favors recal
-
+        ``beta < 1`` lends more weight to precision, while ``beta > 1`` favors recal
     :param inner_summand: Which conditioning factor, if any, to sum over prior to the final
-    aggregation when conditioning on the subclass labels.
-
+        aggregation when conditioning on the subclass labels.
+    :param ignore_unsupported: Whether to ignore ``y_pred`` values that are unsupported by
+        ``y_true`` (labels appearing in the predicted but not ground-truth labels). Note that
+        class:`sklearn.metrics.f1_score` does *not* do this and instead includes unsupported values
+        in its aggregation, i.e. classes included only in ``y_pred`` are included in the
+        class-conditional F-scores as 0 components that influence the aggregation step.
     :param aggregator: Function with which to aggregate over the scores.
-    If ``None`` then no aggregation will be applied and scores will be returned for each
-    group.
+        If ``None`` then no aggregation will be applied and scores will be returned for each group.
 
     :returns: The (optionally aggregated) F-beta score given predictions ``y_pred`` and targets
-    ``y_pred``.
+        ``y_pred``.
     """
-    prec_ids = y_pred if s is None else merge_indices(s, y_pred)
+    # map the predicted and ground-truth labels to a common basis
+    y_unique, rel_indices = torch.unique(torch.cat((y_true, y_pred)), return_inverse=True)
+    y_true, y_pred = rel_indices.chunk(2)
+    card_y = len(y_unique)
+
+    if s is None:
+        rec_ids = y_true
+        rec_ids_u = rec_ids.unique()
+        card_s = None
+        prec_ids = y_pred
+        target_size = card_y
+    else:
+        s_u, s_inv = s.unique(return_inverse=True)
+        card_s = len(s_u)
+        prec_ids = y_pred * card_s + s_inv
+        rec_ids = y_true * card_s + s_inv
+        rec_ids_u = rec_ids.unique()
+        target_size = card_y * card_s
+
     precs = _apply_groupwise_metric(
         prec_ids,
         comparator=equal,
         y_pred=y_pred,
         y_true=y_true,
         aggregator=None,
     )
-    if s is None:
-        rec_ids = y_true
-        card_s = None
-    else:
-        rec_ids, s_card_ls = merge_indices(s, y_true, return_cardinalities=True)
-        card_s = s_card_ls[0]
     recs = _apply_groupwise_metric(
         rec_ids,
         comparator=equal,
         y_pred=y_pred,
         y_true=y_true,
         aggregator=None,
     )
-    y_true_supp = y_true.unique()
-    y_pred_supp = y_pred.unique()
-    # Pad the missing group entries with nans.
-    torch.all
-    if not torch.equal(y_true_supp, y_pred_supp):
-        card_joint = len(torch.cat((y_true_supp, y_pred_supp)).unique())
-        if card_s is not None:
-            card_joint *= card_s
-        precs = _pad_with_nans(n=card_joint, src=precs, index=prec_ids.unique())
-        recs = _pad_with_nans(n=card_joint, src=recs, index=rec_ids.unique())
+
+    if len(precs) < target_size:
+        precs = pad_to_size(size=target_size, index=prec_ids.unique(), src=precs, value=torch.nan)
+    if len(recs) < target_size:
+        recs = pad_to_size(size=target_size, index=rec_ids_u, src=recs, value=torch.nan)
 
     beta_sq = beta**2
-    f1s = (1 + beta_sq) * precs * recs / (beta_sq * precs + recs)
-    if (inner_summand is not None) and (card_s is not None):
+    f1s = (1 + beta_sq) * (precs * recs) / (beta_sq * precs + recs)
+    if ignore_unsupported:
+        # Ignore predictions that are unsupported by the ground-truth label set, supp(``y_true``).
+        f1s = f1s.gather(0, rec_ids_u)
+    f1s = f1s.nan_to_num_(nan=0.0)
+
+    if (inner_summand is not None) and (s is not None):
+        card_s = len(torch.unique(s))
         reduction_dim = int(inner_summand == "s")
         f1s = f1s.view(-1, card_s).nanmean(reduction_dim)
+
     if aggregator is None:
         return f1s
     return aggregator(f1s)
 
 
-def robust_fscore(y_pred: Tensor, *, y_true: Tensor, s: Tensor, beta: float = 1.0) -> Tensor:
+def robust_fscore(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    s: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
     return fscore(
         y_pred=y_pred,
         y_true=y_true,
         s=s,
         beta=beta,
         inner_summand="y_true",
+        ignore_unsupported=ignore_unsupported,
         aggregator=Aggregator.MIN,
     )
 
 
-def fscore_per_subclass(y_pred: Tensor, *, y_true: Tensor, s: Tensor, beta: float = 1.0) -> Tensor:
+def fscore_per_class(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
+    return fscore(
+        y_pred=y_pred,
+        y_true=y_true,
+        beta=beta,
+        inner_summand=None,
+        ignore_unsupported=ignore_unsupported,
+        aggregator=None,
+    )
+
+
+def fscore_per_subclass(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    s: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
     return fscore(
         y_pred=y_pred,
         y_true=y_true,
         s=s,
         beta=beta,
         inner_summand="y_true",
+        ignore_unsupported=ignore_unsupported,
         aggregator=None,
     )
 
 
-def macro_fscore(y_pred: Tensor, *, y_true: Tensor, beta: float = 1.0) -> Tensor:
+def macro_fscore(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
     return fscore(
         y_pred=y_pred,
         y_true=y_true,
         s=None,
         beta=beta,
         inner_summand=None,
+        ignore_unsupported=ignore_unsupported,
         aggregator=Aggregator.MEAN,
     )
 
 
-def fscore_per_group(y_pred: Tensor, *, y_true: Tensor, s: Tensor, beta: float = 1.0) -> Tensor:
+def fscore_per_group(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    s: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
     return fscore(
         y_pred=y_pred,
         y_true=y_true,
         s=s,
         beta=beta,
         inner_summand=None,
+        ignore_unsupported=ignore_unsupported,
         aggregator=None,
     )
 
 
-def robust_fscore_gap(y_pred: Tensor, *, y_true: Tensor, s: Tensor, beta: float = 1.0) -> Tensor:
+def robust_fscore_gap(
+    y_pred: Tensor,
+    *,
+    y_true: Tensor,
+    s: Tensor,
+    beta: float = 1.0,
+    ignore_unsupported: bool = True,
+) -> Tensor:
     return fscore(
         y_pred=y_pred,
         y_true=y_true,
         s=s,
         beta=beta,
         inner_summand="y_true",
+        ignore_unsupported=ignore_unsupported,
         aggregator=Aggregator.MAX_DIFF,
     )
```

### Comparing `torch-conduit-0.1.7/conduit/models/self_supervised/loss.py` & `torch_conduit-0.2.0/conduit/models/self_supervised/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Callable, Optional, Type, TypeVar, Union, cast
+from typing import Callable, Optional, TypeVar, Union, cast
 
 import torch
 from torch import Tensor
 from torch.autograd.function import Function, NestedIOFunction
 import torch.distributed
 import torch.nn as nn
 import torch.nn.functional as F
@@ -76,24 +76,26 @@
 ) -> Tensor:
     """
     Loss function used in the training of MoCo v2.
 
     :param anchors: Logits of the anchor samples.
     :param positives: Logits of the positive samples w.r.t. ``anchors`` (derived from different
         views of the same samples).
-    :negatives: Logits of the negative samples w.r.t ``anchors`` (derived from different samples).
-    :temperature: Inverse temperature parameter used for adjusting the sharpness of the softmax
-        distribution. Smaller values lead to hard negatives being overemphasized.
+    :param negatives: Logits of the negative samples w.r.t ``anchors`` (derived from different
+        samples).
+    :param temperature: Inverse temperature parameter used for adjusting the sharpness of the
+        softmax distribution. Smaller values lead to hard negatives being overemphasized.
 
-    :dcl: Whether to decouple the numerators from the denominators, meaning that the
+    :param dcl: Whether to decouple the numerators from the denominators, meaning that the
         cross-view distances (similarity between the anchors and positives) are not included in the
         negative component of the loss. This has been shown to improve convergence and stability,
         particularly when working with smaller batch sizes.
 
-    :normalize: Whether to l2 normalize the logits before computing the inter-sample similarities
+    :param normalize: Whether to l2 normalize the logits before computing the inter-sample
+        similarities.
 
     :returns: Loss as a 0-dimensional tensor.
     """
     if normalize:
         anchors = F.normalize(anchors, dim=1, p=2)
         positives = F.normalize(positives, dim=1, p=2)
         negatives = F.normalize(negatives, dim=1, p=2)
@@ -385,17 +387,16 @@
         :return: One-way loss between the embedding vectors.
         """
         return decoupled_contrastive_loss(
             z1, z2, temperature=self.temperature, weight_fn=self.weight_fn
         )
 
     @classmethod
-    def with_vmf_weighting(
-        cls: Type[Self], sigma: float = 0.5, *, temperature: float = 0.1
-    ) -> Self:
+    def with_vmf_weighting(cls, sigma: float = 0.5, *, temperature: float = 0.1) -> Self:
         """
         Initialise the DCL loss with von Mises-Fisher weighting.
 
         :param sigma: :math:`\\sigma` (scale) parameter for the weigting function.
         :param temperature: Temperature controlling the sharpness of the softmax distribution.
+        :returns: the loss object
         """
         return cls(temperature=temperature, weight_fn=_von_mises_fisher_weighting)
```

### Comparing `torch-conduit-0.1.7/conduit/models/self_supervised/memory_bank.py` & `torch_conduit-0.2.0/conduit/models/self_supervised/memory_bank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional, Type
 
-from ranzen.decorators import implements
 import torch
 from torch import Tensor, nn
 import torch.nn.functional as F
-from typing_extensions import Self
+from typing_extensions import Self, override
 
 from conduit.types import Indexable, IndexType, Sized
 
 __all__ = ["MemoryBank"]
 
 
 @torch.no_grad()
@@ -26,22 +25,20 @@
         self.capacity = memory.size(0)
         self.dim = memory.shape[1:]
         self.register_buffer(name="memory", tensor=memory)
         self._ptr_pos = 0
 
     @classmethod
     @torch.no_grad()
-    def with_l2_hypersphere_init(cls: Type[Self], capacity: int, *, dim: int) -> Self:
+    def with_l2_hypersphere_init(cls, capacity: int, *, dim: int) -> Self:
         return MemoryBank(l2_hypersphere_init(capacity=capacity, dim=dim))
 
     @classmethod
     @torch.no_grad()
-    def with_randint_init(
-        cls: Type[Self], capacity: int, *, dim: int, high: int, low: int = 0
-    ) -> Self:
+    def with_randint_init(cls, capacity: int, *, dim: int, high: int, low: int = 0) -> Self:
         return MemoryBank(torch.randint(low=low, high=high, size=(capacity, dim)))
 
     @classmethod
     @torch.no_grad()
     def with_constant_init(
         cls: Type[Self],
         capacity: int,
@@ -68,14 +65,14 @@
         if residual <= num_values:
             self.memory[self._ptr_pos :] = values[:residual]
             self.memory[:new_ptr_pos] = values[residual:]
         else:
             self.memory[self._ptr_pos : new_ptr_pos] = values
         self._ptr_pos = new_ptr_pos
 
-    @implements(Indexable)
+    @override
     def __getitem__(self, index: IndexType) -> Tensor:
         return self.memory[index]
 
-    @implements(Sized)
+    @override
     def __len__(self) -> int:
         return len(self.memory)
```

### Comparing `torch-conduit-0.1.7/conduit/models/utils.py` & `torch_conduit-0.2.0/conduit/models/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,9 +44,9 @@
 
 class PartialModule(nn.Module):
     def __init__(self, func: Callable, **kwargs: Any):
         super().__init__()
         self.func = func
         self.bound_kwargs = kwargs
 
-    def __call__(self, *args: Any, **kwargs: Any):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs, **self.bound_kwargs)
```

### Comparing `torch-conduit-0.1.7/conduit/progress.py` & `torch_conduit-0.2.0/conduit/progress.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from __future__ import annotations
 from enum import Enum
-from functools import partial
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Callable, Dict, Optional, Union, cast
 
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks.progress.rich_progress import (
     BatchesProcessedColumn,
     CustomBarColumn,
     CustomTimeColumn,
     ProcessingSpeedColumn,
     RichProgressBar,
     RichProgressBarTheme,
 )
-from ranzen.decorators import implements
+from pytorch_lightning.utilities.types import STEP_OUTPUT
 from rich.console import RenderableType
 from rich.progress import Task, TaskID, TextColumn
 from rich.table import Column
 from rich.text import Text
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, override
 
-from conduit.data.datamodules.vision.dummy import DummyVisionDataModule  # type: ignore
-
-__all__ = [
-    "CdtProgressBar",
-    "ProgressBarTheme",
-]
+__all__ = ["CdtProgressBar", "ProgressBarTheme"]
 
 
 class _FixedLengthProcessionSpeed(ProcessingSpeedColumn):
     """Renders processing speed for the progress bar with fixes length"""
 
     def __init__(self, style: Union[str, Any]) -> None:
         super().__init__(style)
@@ -77,45 +71,50 @@
         time="white",
         processing_speed="#0057e7",
         metrics="#d62d20",
     )
 
 
 class ProgressBarTheme(Enum):
-    QUATERION = partial(_quaterion_theme)
-    CYBERPUNK = partial(_cyberpunk_theme)
-    GOOGLE = partial(_google_theme)
+    QUATERION = (_quaterion_theme,)
+    CYBERPUNK = (_cyberpunk_theme,)
+    GOOGLE = (_google_theme,)
+
+    def __init__(self, load: Callable[..., RichProgressBarTheme]) -> None:
+        self.load = load
 
 
 class CdtProgressBar(RichProgressBar):
     """Custom Lightning progress bar supporting both epoch- and iteration-based training."""
 
     Theme: TypeAlias = ProgressBarTheme
 
     def __init__(
         self,
         refresh_rate: int = 1,
         *,
         leave: bool = False,
         theme: Union[RichProgressBarTheme, Theme] = Theme.CYBERPUNK,
         console_kwargs: Optional[Dict[str, Any]] = None,
+        predict_description: str = "Predicting",
     ) -> None:
         if isinstance(theme, ProgressBarTheme):
-            theme = cast(RichProgressBarTheme, theme.value())
+            theme = cast(RichProgressBarTheme, theme.load())
 
         super().__init__(
             refresh_rate=refresh_rate,
             leave=leave,
             theme=theme,
             console_kwargs=console_kwargs,
         )
         self.predict_progress_bar_id = None
+        self._predict_description = predict_description
 
-    @implements(RichProgressBar)
-    def configure_columns(self, *args: Any, **kwargs: Any) -> list:
+    @override
+    def configure_columns(self, *args: Any, **kwargs: Any) -> list:  # pyright: ignore
         return [
             TextColumn(
                 "[progress.description]{task.description}",
                 table_column=Column(
                     no_wrap=True,
                     min_width=9,  # prevents blinking during validation, length of `Validation `
                 ),
@@ -131,47 +130,48 @@
         ]
 
     @staticmethod
     def _is_iteration_based(trainer: pl.Trainer) -> bool:
         return trainer.num_training_batches == float("inf")
 
     @property
-    @implements(RichProgressBar)
+    @override
     def total_train_batches(self) -> Union[int, float]:
-        """The total number of training batches, which may change from epoch to epoch.
+        """
+        The total number of training batches, which may change from epoch to epoch.
 
-        Use this to set the total number of iterations in the progress bar. Can return ``inf`` if the training
-        dataloader is of infinite size.
+        Use this to set the total number of iterations in the progress bar. Can return ``inf`` if
+        the training dataloader is of infinite size.
         """
         if self.trainer.max_steps >= 0:
             return self.trainer.max_steps
         return self.trainer.num_training_batches
 
-    @implements(RichProgressBar)
+    @override
     def _add_task(
         self, total_batches: float, description: str, visible: bool = True
-    ) -> Optional[int]:
+    ) -> Optional[TaskID]:
         if self.progress is not None:
             return self.progress.add_task(
                 f"[{self.theme.description}]{description}", total=total_batches, visible=visible
             )
 
-    @implements(RichProgressBar)
+    @override
     def _update(self, progress_bar_id: int, current: int, visible: bool = True) -> None:
         if self.progress is not None and self.is_enabled:
             total = self.progress.tasks[progress_bar_id].total
             if not self._should_update(current, total):  # type: ignore
                 return
 
             leftover = current % self.refresh_rate
             advance = leftover if (current == total and leftover != 0) else self.refresh_rate
             self.progress.update(TaskID(progress_bar_id), advance=advance, visible=visible)
             self.refresh()
 
-    @implements(RichProgressBar)
+    @override
     def _get_train_description(self, current_epoch: Optional[int]) -> str:
         train_description = f"Training"
         if current_epoch is not None:
             train_description += f" (Epoch: {current_epoch})"
         if len(self.validation_description) > len(train_description):
             # Padding is required to avoid flickering due of uneven lengths of "Epoch X"
             # and "Validation" Bar description
@@ -179,57 +179,84 @@
             required_padding = (
                 len(self.validation_description) - len(train_description) + 1
             ) - num_digits
             for _ in range(required_padding):
                 train_description += " "
         return train_description
 
-    @implements(RichProgressBar)
-    def on_train_epoch_start(self, trainer, pl_module):
+    @property
+    def _progress_bar_id(self) -> Optional[TaskID]:
+        return getattr(self, "train_progress_bar_id", getattr(self, "main_progress_bar_id", None))
+
+    @_progress_bar_id.setter
+    def _progress_bar_id(self, value: Optional[TaskID]) -> None:
+        if hasattr(self, "train_progress_bar_id"):
+            self.train_progress_bar_id = value
+        if hasattr(self, "main_progress_bar_id"):
+            self.main_progress_bar_id = value
+
+    @override
+    def on_train_epoch_start(self, trainer: pl.Trainer, pl_module) -> None:  # pyright: ignore
         total_train_batches = self.total_train_batches
         total_val_batches = self.total_val_batches
         if total_train_batches != float("inf"):
             # val can be checked multiple times per epoch
             val_checks_per_epoch = total_train_batches // trainer.val_check_batch
             total_val_batches = total_val_batches * val_checks_per_epoch
 
         iteration_based = self._is_iteration_based(trainer)
         current_epoch = None if iteration_based else trainer.current_epoch
         train_description = self._get_train_description(current_epoch)
-        if self.main_progress_bar_id is not None and self._leave:
+        if self._progress_bar_id is not None and self._leave:
             self._stop_progress()
             self._init_progress(trainer)
-        if self.main_progress_bar_id is None:
-            self.main_progress_bar_id = self._add_task(total_train_batches, train_description)
+        if self._progress_bar_id is None:
+            self._progress_bar_id = self._add_task(total_train_batches, train_description)
         elif (not iteration_based) and (self.progress is not None):
             self.progress.reset(
-                TaskID(self.main_progress_bar_id),
+                TaskID(self._progress_bar_id),
                 total=total_train_batches,
                 description=train_description,
                 visible=True,
             )
         self.refresh()
 
-    @implements(RichProgressBar)
-    def on_validation_batch_end(self, trainer: pl.Trainer, *args: Any, **kwargs: Any) -> None:
+    @override
+    def on_validation_batch_end(
+        self,
+        trainer: pl.Trainer,
+        pl_module: pl.LightningModule,  # pyright: ignore
+        outputs: Optional[STEP_OUTPUT],  # pyright: ignore
+        batch: Any,  # pyright: ignore
+        batch_idx: int,
+        dataloader_idx: int = 0,  # pyright: ignore
+    ) -> None:
         if trainer.sanity_checking:
-            self._update(self.val_sanity_progress_bar_id, self.val_batch_idx)  # type: ignore
+            self._update(self.val_sanity_progress_bar_id, batch_idx + 1)  # type: ignore
         elif self.val_progress_bar_id is not None:
             # check to see if we should update the main training progress bar
-            self._update(self.val_progress_bar_id, self.val_batch_idx)
+            self._update(self.val_progress_bar_id, batch_idx + 1)
         self.refresh()
 
-    @implements(RichProgressBar)
+    @property
+    def predict_description(self) -> str:
+        return self._predict_description
+
+    @predict_description.setter
+    def predict_description(self, value: str) -> None:
+        self._predict_description = value
+
+    @override
     def on_predict_batch_start(
         self,
-        trainer: pl.Trainer,
-        pl_module: pl.LightningModule,
-        batch: Any,
-        batch_idx: int,
-        dataloader_idx: int,
+        trainer: pl.Trainer,  # pyright: ignore
+        pl_module: pl.LightningModule,  # pyright: ignore
+        batch: Any,  # pyright: ignore
+        batch_idx: int,  # pyright: ignore
+        dataloader_idx: int = 0,
     ) -> None:
         if self.has_dataloader_changed(dataloader_idx):
             if (self.predict_progress_bar_id is not None) and (self.progress is not None):
                 self.progress.update(TaskID(self.predict_progress_bar_id), advance=0, visible=False)
             self.predict_progress_bar_id = self._add_task(
                 self.total_predict_batches_current_dataloader, self.predict_description
             )
```

### Comparing `torch-conduit-0.1.7/conduit/transforms/audio.py` & `torch_conduit-0.2.0/conduit/transforms/audio.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/transforms/fixmatch.py` & `torch_conduit-0.2.0/conduit/transforms/fixmatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from dataclasses import dataclass
 from typing import Callable, Generic, List, Optional, TypeVar, Union
 
 from PIL import Image
 import numpy as np
-from ranzen.decorators import implements
 from ranzen.misc import gcopy
 from torch import Tensor
-from typing_extensions import Self
+from typing_extensions import Self, override
 
-from conduit.data.datasets.utils import ImageTform, apply_image_transform
+from conduit.data.datasets.vision.utils import ImageTform, apply_image_transform
 from conduit.data.structures import InputContainer, RawImage, concatenate_inputs
 
 __all__ = [
     "FixMatchPair",
     "FixMatchTransform",
 ]
 
@@ -20,21 +19,21 @@
 
 
 @dataclass
 class FixMatchPair(InputContainer[X]):
     strong: X
     weak: X
 
-    @implements(InputContainer)
+    @override
     def __len__(self) -> int:
         if isinstance(self.strong, Image.Image):
             return 1
         return len(self.strong)
 
-    @implements(InputContainer)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         is_batched = isinstance(self.strong, (Tensor, np.ndarray)) and (self.strong.ndim == 4)
         copy.strong = concatenate_inputs(copy.strong, other.strong, is_batched=is_batched)
         copy.weak = concatenate_inputs(copy.weak, other.weak, is_batched=is_batched)
 
         return copy
```

### Comparing `torch-conduit-0.1.7/conduit/transforms/image.py` & `torch_conduit-0.2.0/conduit/transforms/image.py`

 * *Files identical despite different names*

### Comparing `torch-conduit-0.1.7/conduit/transforms/multicrop.py` & `torch_conduit-0.2.0/conduit/transforms/multicrop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from dataclasses import dataclass
 from typing import Generic, List, Optional, Sequence, Tuple, TypeVar, Union, overload
 
-from ranzen.decorators import implements
 from ranzen.misc import gcopy
 import torch
 from torch import Tensor
 import torchvision.transforms as T  # type: ignore
 import torchvision.transforms.functional as TF  # type: ignore
-from typing_extensions import Self
+from typing_extensions import Self, override
 
 from conduit.data.constants import IMAGENET_STATS
-from conduit.data.datasets.utils import (
+from conduit.data.datasets.vision.utils import (
     ImageTform,
     PillowTform,
     apply_image_transform,
     img_to_tensor,
 )
 from conduit.data.structures import (
     InputContainer,
@@ -37,19 +36,19 @@
     v1: Tensor
     v2: Tensor
 
     def __post_init__(self) -> None:
         if self.v1.size() != self.v2.size():
             raise AttributeError("'v1' and 'v2' must have the same shape.")
 
-    @implements(InputContainer)
+    @override
     def __len__(self) -> int:
         return len(self.v1)
 
-    @implements(InputContainer)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         is_batched = self.v1.ndim == 4
         copy.v1 = concatenate_inputs(copy.v1, other.v1, is_batched=is_batched)
         copy.v2 = concatenate_inputs(copy.v2, other.v2, is_batched=is_batched)
 
         return copy
@@ -123,20 +122,20 @@
     def anchor(self) -> Tuple[Tensor, Tensor]:
         return (self.global_views.v1, self.local_views)
 
     @property
     def target(self) -> Tensor:
         return self.global_views.v2
 
-    @implements(InputContainer)
+    @override
     def __len__(self) -> int:
         """Total number of crops."""
         return len(self.global_views) + len(self.local_views)
 
-    @implements(InputContainer)
+    @override
     def __add__(self, other: Self) -> Self:
         copy = gcopy(self, deep=False)
         copy.global_views = copy.global_views + other.global_views
         if copy.local_views is None:
             if other.local_views is not None:
                 copy.local_views = other.local_views
         else:
@@ -213,15 +212,14 @@
         global_crop_size: Union[int, Sequence[int]] = 224,
         local_crop_size: Union[int, Sequence[int]] = 96,
         norm_values: Optional[MeanStd] = IMAGENET_STATS,
         global_crops_scale: Tuple[float, float] = (0.4, 1.0),
         local_crops_scale: Tuple[float, float] = (0.05, 0.4),
         local_crops_number: int = 8,
     ) -> "MultiCropTransform":
-
         flip_and_color_jitter = T.Compose(
             [
                 T.RandomHorizontalFlip(p=0.5),
                 T.RandomApply(
                     [T.ColorJitter(brightness=0.4, contrast=0.4, saturation=0.2, hue=0.1)], p=0.8
                 ),
                 T.RandomGrayscale(p=0.2),
```

### Comparing `torch-conduit-0.1.7/conduit/transforms/tabular.py` & `torch_conduit-0.2.0/conduit/transforms/tabular.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import abstractmethod
 import math
-from typing import ClassVar, List, Union
+from typing import ClassVar, List, Union, final
 
-from ranzen import implements
 import torch
 from torch import Tensor
-from typing_extensions import final
+from typing_extensions import override
 
 __all__ = [
     "TabularTransform",
     "MinMaxNormalize",
     "QuantileNormalize",
     "TabularNormalize",
     "ZScoreNormalize",
@@ -90,37 +89,35 @@
 
     @final
     def __call__(self, data: Tensor) -> Tensor:
         return self.transform(data)
 
 
 class ZScoreNormalize(TabularNormalize):
-
     mean: Tensor
     std: Tensor
 
-    @implements(TabularNormalize)
+    @override
     def _fit(self, data: Tensor) -> None:
         self.std, self.mean = torch.std_mean(data, dim=0, keepdim=True, unbiased=True)
 
-    @implements(TabularNormalize)
+    @override
     def _inverse_transform(self, data: Tensor) -> Tensor:
         data *= self.std
         data += self.mean
         return data
 
-    @implements(TabularNormalize)
+    @override
     def _transform(self, data: Tensor) -> Tensor:
         data -= self.mean
         data /= self.std.clamp_min(self._EPS)
         return data
 
 
 class QuantileNormalize(TabularNormalize):
-
     iqr: Tensor
     median: Tensor
 
     def __init__(self, q_min: float = 0.25, q_max: float = 0.75, inplace: bool = False) -> None:
         super().__init__(inplace=inplace)
         if not (0 <= q_min <= 1):
             raise ValueError("q_min must be in the range [0, 1]")
@@ -136,66 +133,65 @@
         q_ind_frac, q_ind_int = math.modf(q * (len(sorted_values) - 1))
         q_ind_int = int(q_ind_int)
         q_quantile = sorted_values[q_ind_int]
         if q_ind_frac > 0:
             q_quantile += (sorted_values[q_ind_int + 1] - q_quantile) * q_ind_frac
         return q_quantile
 
-    @implements(TabularNormalize)
+    @override
     def _fit(self, data: Tensor) -> None:
         sorted_values = data.sort(dim=0, descending=False).values
         # Compute the 'lower quantile'
         q_min_quantile = self._compute_quantile(q=self.q_min, sorted_values=sorted_values)
         # Compute the 'upper quantile'
         q_max_quantile = self._compute_quantile(q=self.q_max, sorted_values=sorted_values)
         # Compute the interquantile range
         self.iqr = q_max_quantile - q_min_quantile
         self.median = self._compute_quantile(q=0.5, sorted_values=sorted_values)
 
-    @implements(TabularNormalize)
+    @override
     def _inverse_transform(self, data: Tensor) -> Tensor:
         data *= self.iqr
         data += self.median
         return data
 
-    @implements(TabularNormalize)
+    @override
     def _transform(self, data: Tensor) -> Tensor:
         data -= self.median
         data /= self.iqr.clamp_min(self._EPS)
         return data
 
 
 class MinMaxNormalize(TabularNormalize):
-
     orig_max: Tensor
     orig_min: Tensor
     orig_range: Tensor
 
     def __init__(self, new_min: float = 0.0, new_max: float = 1.0, inplace: bool = False) -> None:
         super().__init__(inplace=inplace)
         if new_min > new_max:
             raise ValueError("'new_min' cannot be greater than 'new_max'.")
         self.new_min = new_min
         self.new_max = new_max
         self.new_range = self.new_max - self.new_min
 
-    @implements(TabularNormalize)
+    @override
     def _fit(self, data: Tensor) -> None:
         self.orig_min = torch.min(data, dim=0, keepdim=True).values
         self.orig_max = torch.max(data, dim=0, keepdim=True).values
         self.orig_range = self.orig_max - self.orig_min
 
-    @implements(TabularNormalize)
+    @override
     def _inverse_transform(self, data: Tensor) -> Tensor:
         data -= self.new_min
         data /= self.new_range + self._EPS
         data *= self.orig_range
         data += self.orig_min
         return data
 
-    @implements(TabularNormalize)
+    @override
     def _transform(self, data: Tensor) -> Tensor:
         data -= self.orig_min
         data /= self.orig_range.clamp_min(self._EPS)
         data *= self.new_range
         data += self.new_min
         return data
```

### Comparing `torch-conduit-0.1.7/conduit/types.py` & `torch_conduit-0.2.0/conduit/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-from enum import Enum
-from typing import Any, Dict, List, Protocol, TypeVar, Union
+from enum import auto
+from typing import Any, Dict, List, Mapping, Protocol, TypeVar, Union, runtime_checkable
 
 import numpy as np
 import numpy.typing as npt
-from pytorch_lightning.utilities.types import _METRIC_COLLECTION
-from ranzen.decorators import enum_name_str
+from ranzen import StrEnum
 from ranzen.torch.loss import ReductionType
 from torch import Tensor
 from torch.optim.lr_scheduler import CosineAnnealingWarmRestarts, ExponentialLR, StepLR
-from typing_extensions import Protocol, Self, TypeAlias, runtime_checkable
+from torchmetrics import Metric
+from typing_extensions import TypeAlias
 
 __all__ = [
     "IndexType",
     "Indexable",
     "LRScheduler",
     "Loss",
     "MetricDict",
     "NDArrayR",
     "Sized",
     "Stage",
 ]
 
+_NUMBER = Union[int, float]
+_METRIC = Union[Metric, Tensor, _NUMBER]
+_METRIC_COLLECTION = Union[_METRIC, Mapping[str, _METRIC]]
+
 
 class Loss(Protocol):
     def __call__(self, input: Tensor, target: Tensor, **kwargs: Any) -> Tensor:
         ...
 
     @property
     def reduction(self) -> Union[ReductionType, str]:
         ...
 
     @reduction.setter
     def reduction(self, value: Union[ReductionType, str]) -> None:
         ...
 
 
-@enum_name_str
-class Stage(Enum):
-    fit = "fit"
-    validate = "validate"
-    test = "test"
+class Stage(StrEnum):
+    FIT = auto()
+    VALIDATE = auto()
+    TEST = auto()
 
 
 LRScheduler: TypeAlias = Union[CosineAnnealingWarmRestarts, ExponentialLR, StepLR]
 MetricDict: TypeAlias = Dict[str, _METRIC_COLLECTION]
 NDArrayR: TypeAlias = Union[npt.NDArray[np.floating], npt.NDArray[np.integer]]
 IndexType: TypeAlias = Union[int, List[int], slice]
```

### Comparing `torch-conduit-0.1.7/pyproject.toml` & `torch_conduit-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 [tool.poetry]
 name = "torch-conduit"
-version = "0.1.7"
+version = "0.2.0"
 description = "Lightweight framework for dataloading with PyTorch and channeling the power of PyTorch Lightning"
 authors = ["PAL <info@predictive-analytics-lab.com>"]
 license = "Apache License 2.0"
 packages = [
   { include = "conduit" },
 ]
 include=["conduit/py.typed"]
 classifiers=[
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Typing :: Typed",
 ]
 keywords=["typing", "python", "pytorch", "datasets", "pytorch-lightning", "lightning-bolts"]
 repository="https://github.com/wearepal/conduit"
 readme="README.md"
 
 [tool.poetry.dependencies]
-attrs = "^21.2.0"
+attrs = ">=21.2.0"
 numpy = "^1.22.3"
 pandas = "^1.3.3"
-python = ">=3.8.0,<3.11"
-ranzen = {version = ">=2.0.0", extras = ["hydra"]}
+python = ">=3.8.0,<3.12"
+ranzen = {version = ">=2.0.0"}
 scikit-learn = "^1.2.0"
-typing-extensions = ">=4.0.0"
+typing-extensions = ">=4.4.0"
 
-[tool.poetry.group.torch.dependencies]
-pytorch-lightning = "^1.5.0"
-torch = ">=1.12.0"
-torchaudio = ">=0.12.0"
-torchvision = ">=0.10.1"
+# NOTE: the following has to be kept in sync with the groups below
+# download
+gdown = {version = "^3.13.0", optional = true}
+kaggle = {version = "^1.5.12", optional = true}
+# image
+albumentations = {version = "^1.0.0", optional = true}
+opencv-python = {version = "^4.5.3", optional = true}
+# audio
+soundfile = {version = "*", markers = "platform_system == 'Windows'", optional = true}
+sox = {version = "*", markers = "platform_system == 'Linux' or platform_system == 'macOS'", optional = true}
+# hydra
+hydra-core = {version = "^1.1.1", optional = true}
+# logging
+rich = {version = "^12.5.1", optional = true}
+# fair
+ethicml = {version = ">=1.0.2", extras = ["data"], optional = true}
 
 [tool.poetry.group.download.dependencies]
 gdown = "^3.13.0"
 kaggle = "^1.5.12"
 
 [tool.poetry.group.image.dependencies]
 albumentations = "^1.0.0"
@@ -55,25 +67,50 @@
 
 [tool.poetry.group.fair]
 optional = true
 
 [tool.poetry.group.fair.dependencies]
 ethicml = ">=1.0.2"
 
+[tool.poetry.extras]
+download = ["gdown", "kaggle"]
+image = ["albumentations", "opencv-python"]
+audio = ["soundfile", "sox"]
+hydra = ["hydra-core"]
+logging = ["rich"]
+fair = ["ethicml"]
+all = [
+    "gdown", "kaggle",  # download
+    "albumentations", "opencv-python",  # image
+    "soundfile", "sox",  # audio
+    "hydra-core",  # hydra
+    "rich",  # logging
+    "ethicml",  # fair
+]
+
+[tool.poetry.group.torch]
+optional = true
+
+[tool.poetry.group.torch.dependencies]
+pytorch-lightning = "^2.0.1.post0"
+torch = ">=1.12.0"
+torchaudio = ">=0.12.0"
+torchvision = ">=0.10.1"
+
 [tool.poetry.group.dev.dependencies]
 black = "*"
 darglint = "^1.8.0"
 isort = "*"
 mypy = "*"
 neoconfigen = {version = ">=2.3.3"}
 pre-commit = "*"
-pydocstyle = "*"
-pylint = "^2.11.1"
 pytest = "*"
-python-type-stubs = {git = "https://github.com/predictive-analytics-lab/python-type-stubs.git", branch = "main" }
+python-type-stubs = {git = "https://github.com/wearepal/python-type-stubs.git", rev = "2ea8053"}
+pandas-stubs = "*"
+types-tqdm = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
@@ -102,78 +139,71 @@
 [tool.isort]
 known_third_party = ["PIL", "albumentations", "attr", "cv2", "ethicml", "hydra", "numpy", "omegaconf", "pandas", "pytest", "pytorch_lightning", "ranzen", "requests", "rich", "sklearn", "torch", "torchaudio", "torchmetrics", "torchvision", "tqdm", "typing_extensions"]
 known_future_library = []
 extra_standard_library = ["dataclasses", "__future__", "typing_extensions"]
 line_length = 88
 profile = "black"
 force_sort_within_sections = "True"
-classes = ["MISSING"]
+classes = ["MISSING", "NICO", "PACS", "SSRP", "ISIC"]
 
 [tool.pyright]
 include = ["conduit"]
-exclude = ["**/node_modules", "**/__pycache__"]
+exclude = ["**/node_modules", "**/__pycache__", "**/.*", "**/conf.py"]
 typeCheckingMode = "basic"
 pythonVersion = "3.8"
 reportUnusedImport = "error"
 reportDuplicateImport  = "error"
 reportIncompatibleVariableOverride = "error"
 reportOverlappingOverload = "error"
 reportUntypedNamedTuple = "error"
 reportConstantRedefinition = "warning"
 reportMissingImports = "error"
 reportMissingTypeStubs = "warning"
 strictListInference = true
 strictSetInference = true
 strictParameterNoneValue = true
+reportUnnecessaryTypeIgnoreComment = "warning"
 
 [tool.mypy]
 python_version = "3.8"
 no_implicit_optional = true
 allow_redefinition = true
 strict_equality = true
 check_untyped_defs = true
 warn_unreachable = true
 disallow_any_unimported = false
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 show_error_codes = true
 warn_unused_ignores = false
+warn_redundant_casts = true
 exclude = ["conf.py"]
 
 [[tool.mypy.overrides]]
 module = [
     "albumentations.*",
     "cv2.*",
-    "ethicml.*",
     "flash.*",
     "gdown.*",
     "git.*",
-    "ranzen.*",
-    "pandas.*",
     "PIL.*",
     "pl_bolts.*",
     "pytest.*",
     "pytorch_lightning.*",
     "requests.*",
     "scipy.*",
     "sklearn.*",
     "torch.*",
     "torchmetrics.*",
     "torchvision.*",
     "typing_inspect.*",
-    "tqdm.*",
     "wandb.*"
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
-    "ethicml.*",
-    "ranzen.*",
-    "numpy.typing.*",
-    "pytest.*",
-    "pytorch_lightning.*",
     "torch.*",
     "torchmetrics.*"
 ]
 follow_imports = "skip"
-follow_imports_for_stubs = true
+#follow_imports_for_stubs = true
```

