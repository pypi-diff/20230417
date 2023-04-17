# Comparing `tmp/pyiqa-0.1.6.3.tar.gz` & `tmp/pyiqa-0.1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiqa-0.1.6.3.tar", last modified: Wed Mar 29 17:37:51 2023, max compression
+gzip compressed data, was "dist/pyiqa-0.1.6.4.tar", last modified: Mon Apr 17 18:50:01 2023, max compression
```

## Comparing `pyiqa-0.1.6.3.tar` & `pyiqa-0.1.6.4.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/LICENSE
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.6.3/LICENSE_NTU-S-Lab
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/MANIFEST.in
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    15038 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/PKG-INFO
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14162 2023-03-25 15:14:37.000000 pyiqa-0.1.6.3/README.md
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)        8 2023-03-29 17:33:08.000000 pyiqa-0.1.6.3/VERSION
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.6.3/pyiqa/api_helpers.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/archs/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8301 2023-03-23 15:14:57.000000 pyiqa-0.1.6.3/pyiqa/archs/ahiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6085 2022-09-14 13:07:19.000000 pyiqa-0.1.6.3/pyiqa/archs/arch_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7158 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/brisque_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/ckdn_arch.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25129 2023-01-11 18:50:33.000000 pyiqa-0.1.6.3/pyiqa/archs/clip_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6720 2023-03-28 11:01:26.000000 pyiqa-0.1.6.3/pyiqa/archs/clipiqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2022-11-21 12:29:26.000000 pyiqa-0.1.6.3/pyiqa/archs/cnniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.6.3/pyiqa/archs/constants.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6126 2022-09-14 13:07:48.000000 pyiqa-0.1.6.3/pyiqa/archs/dbcnn_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5207 2023-03-05 10:40:20.000000 pyiqa-0.1.6.3/pyiqa/archs/dists_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10664 2022-10-26 10:00:17.000000 pyiqa-0.1.6.3/pyiqa/archs/fid_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/fsim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6967 2023-03-29 10:09:20.000000 pyiqa-0.1.6.3/pyiqa/archs/func_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/gmsd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2023-03-25 15:09:35.000000 pyiqa-0.1.6.3/pyiqa/archs/hypernet_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/inception.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    24091 2022-09-01 11:00:34.000000 pyiqa-0.1.6.3/pyiqa/archs/iqt_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14538 2022-10-13 10:06:00.000000 pyiqa-0.1.6.3/pyiqa/archs/lpips_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11139 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/mad_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7167 2022-12-21 06:20:05.000000 pyiqa-0.1.6.3/pyiqa/archs/maniqa_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16352 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/maniqa_swin.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13552 2023-02-22 11:06:29.000000 pyiqa-0.1.6.3/pyiqa/archs/musiq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4013 2022-11-20 07:22:00.000000 pyiqa-0.1.6.3/pyiqa/archs/nima_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19672 2023-03-02 12:08:26.000000 pyiqa-0.1.6.3/pyiqa/archs/niqe_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7050 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/nlpd_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16444 2023-03-29 13:57:08.000000 pyiqa-0.1.6.3/pyiqa/archs/nrqm_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2870 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/paq2piq_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.6.3/pyiqa/archs/pieapp_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/psnr_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11245 2023-03-29 12:53:13.000000 pyiqa-0.1.6.3/pyiqa/archs/ssim_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14811 2023-02-22 14:19:42.000000 pyiqa-0.1.6.3/pyiqa/archs/tres_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/vif_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9905 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/vsi_arch.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/archs/wadiqam_arch.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/data/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4164 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/ava_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4390 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/bapps_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/data_sampler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.6.3/pyiqa/data/data_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2678 2023-02-23 14:39:44.000000 pyiqa-0.1.6.3/pyiqa/data/flive_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3325 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/general_fr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2726 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/general_nr_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2560 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/livechallenge_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.6.3/pyiqa/data/multiscale_trans_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4849 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/pieapp_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3201 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/pipal_dataset.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/prefetch_dataloader.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13759 2022-09-01 10:53:45.000000 pyiqa-0.1.6.3/pyiqa/data/transforms.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7178 2023-03-25 14:47:12.000000 pyiqa-0.1.6.3/pyiqa/default_model_configs.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/losses/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/losses/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.6.3/pyiqa/losses/iqa_losses.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/losses/loss_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.6.3/pyiqa/losses/losses.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      529 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10201 2023-03-29 12:41:27.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/functions.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/math_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/resize.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8063 2023-03-29 11:09:06.000000 pyiqa-0.1.6.3/pyiqa/matlab_utils/scfpyr_util.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/metrics/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/metrics/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/metrics/correlation_coefficient.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.6.3/pyiqa/metrics/other_metrics.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/models/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/models/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.6.3/pyiqa/models/bapps_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.6.3/pyiqa/models/base_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.6.3/pyiqa/models/dbcnn_model.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     8143 2023-01-11 18:50:33.000000 pyiqa-0.1.6.3/pyiqa/models/general_iqa_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/models/hypernet_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3027 2023-03-22 06:28:53.000000 pyiqa-0.1.6.3/pyiqa/models/inference_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/models/lr_scheduler.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2227 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/models/nima_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.6.3/pyiqa/models/pieapp_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9300 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/models/sr_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/models/wadiqam_model.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/test.py
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11007 2023-01-11 18:50:33.000000 pyiqa-0.1.6.3/pyiqa/train.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.6.3/pyiqa/train_nsplits.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa/utils/
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      934 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/__init__.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/color_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/dist_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/download_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/file_client.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7261 2022-10-26 05:47:49.000000 pyiqa-0.1.6.3/pyiqa/utils/img_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/lmdb_util.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/logger.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/misc.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/options.py
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.6.3/pyiqa/utils/registry.py
--rwxr-xr-x   0 cfchen   (25144) cfchen   (25144)      133 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa/version.py
-drwxrwxr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/pyiqa.egg-info/
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    15038 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa.egg-info/PKG-INFO
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     2653 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa.egg-info/SOURCES.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        1 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa.egg-info/dependency_links.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      170 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa.egg-info/requires.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)        6 2023-03-29 17:37:50.000000 pyiqa-0.1.6.3/pyiqa.egg-info/top_level.txt
--rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-03-29 17:32:51.000000 pyiqa-0.1.6.3/requirements.txt
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-03-29 17:37:51.000000 pyiqa-0.1.6.3/setup.cfg
--rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.6.3/setup.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    21165 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/LICENSE
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1717 2022-09-23 04:11:05.000000 pyiqa-0.1.6.4/LICENSE_NTU-S-Lab
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)       41 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/MANIFEST.in
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12233 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/PKG-INFO
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11357 2023-03-30 12:36:49.000000 pyiqa-0.1.6.4/README.md
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)        8 2023-04-17 18:44:53.000000 pyiqa-0.1.6.4/VERSION
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      322 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2137 2023-03-05 10:38:17.000000 pyiqa-0.1.6.4/pyiqa/api_helpers.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/archs/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      881 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8301 2023-04-01 06:45:12.000000 pyiqa-0.1.6.4/pyiqa/archs/ahiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6053 2023-04-01 05:18:18.000000 pyiqa-0.1.6.4/pyiqa/archs/arch_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7158 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/brisque_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12397 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/ckdn_arch.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    25129 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/archs/clip_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     6636 2023-04-01 05:18:41.000000 pyiqa-0.1.6.4/pyiqa/archs/clipiqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2425 2022-11-21 12:29:26.000000 pyiqa-0.1.6.4/pyiqa/archs/cnniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      387 2022-12-21 06:18:18.000000 pyiqa-0.1.6.4/pyiqa/archs/constants.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6126 2022-09-14 13:07:48.000000 pyiqa-0.1.6.4/pyiqa/archs/dbcnn_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5207 2023-03-05 10:40:20.000000 pyiqa-0.1.6.4/pyiqa/archs/dists_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10627 2023-04-01 05:16:09.000000 pyiqa-0.1.6.4/pyiqa/archs/fid_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18043 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/fsim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6967 2023-03-29 10:09:20.000000 pyiqa-0.1.6.4/pyiqa/archs/func_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3471 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/gmsd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7126 2023-04-01 05:19:52.000000 pyiqa-0.1.6.4/pyiqa/archs/hypernet_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12026 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/inception.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    23872 2023-04-01 05:20:23.000000 pyiqa-0.1.6.4/pyiqa/archs/iqt_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14538 2022-10-13 10:06:00.000000 pyiqa-0.1.6.4/pyiqa/archs/lpips_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11139 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/mad_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7328 2023-04-03 07:58:57.000000 pyiqa-0.1.6.4/pyiqa/archs/maniqa_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16352 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/maniqa_swin.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13552 2023-03-30 10:34:00.000000 pyiqa-0.1.6.4/pyiqa/archs/musiq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4013 2023-03-30 10:34:02.000000 pyiqa-0.1.6.4/pyiqa/archs/nima_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    19674 2023-04-01 05:20:50.000000 pyiqa-0.1.6.4/pyiqa/archs/niqe_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7050 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/nlpd_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16444 2023-03-29 13:57:08.000000 pyiqa-0.1.6.4/pyiqa/archs/nrqm_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2870 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/paq2piq_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5467 2022-12-21 06:09:37.000000 pyiqa-0.1.6.4/pyiqa/archs/pieapp_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2663 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/psnr_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    11245 2023-03-29 12:53:13.000000 pyiqa-0.1.6.4/pyiqa/archs/ssim_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    14811 2023-02-22 14:19:42.000000 pyiqa-0.1.6.4/pyiqa/archs/tres_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    29869 2023-04-01 05:17:21.000000 pyiqa-0.1.6.4/pyiqa/archs/uranker_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    18900 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/vif_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9905 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/vsi_arch.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6508 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/archs/wadiqam_arch.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/data/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4472 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4164 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/ava_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4390 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/bapps_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1812 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/data_sampler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13252 2022-09-01 10:56:27.000000 pyiqa-0.1.6.4/pyiqa/data/data_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2678 2023-02-23 14:39:44.000000 pyiqa-0.1.6.4/pyiqa/data/flive_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3325 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/general_fr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2726 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/general_nr_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2560 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/livechallenge_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7728 2022-09-01 10:54:53.000000 pyiqa-0.1.6.4/pyiqa/data/multiscale_trans_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4849 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/pieapp_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3201 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/pipal_dataset.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3131 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/prefetch_dataloader.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    13759 2022-09-01 10:53:45.000000 pyiqa-0.1.6.4/pyiqa/data/transforms.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7620 2023-04-03 07:58:04.000000 pyiqa-0.1.6.4/pyiqa/default_model_configs.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/losses/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      716 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/losses/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4348 2022-09-01 10:48:31.000000 pyiqa-0.1.6.4/pyiqa/losses/iqa_losses.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2903 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/losses/loss_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7448 2022-09-01 10:47:19.000000 pyiqa-0.1.6.4/pyiqa/losses/losses.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      529 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    10201 2023-03-29 12:41:27.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/functions.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2581 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/math_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12829 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/resize.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     8063 2023-03-29 11:09:06.000000 pyiqa-0.1.6.4/pyiqa/matlab_utils/scfpyr_util.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/metrics/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      566 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/metrics/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2041 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/metrics/correlation_coefficient.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      270 2022-09-01 10:44:09.000000 pyiqa-0.1.6.4/pyiqa/metrics/other_metrics.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/models/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1007 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/models/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     5767 2022-09-01 10:41:30.000000 pyiqa-0.1.6.4/pyiqa/models/bapps_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    16067 2022-09-01 10:43:19.000000 pyiqa-0.1.6.4/pyiqa/models/base_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1737 2022-08-14 08:39:50.000000 pyiqa-0.1.6.4/pyiqa/models/dbcnn_model.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)     8143 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/models/general_iqa_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1190 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/hypernet_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3089 2023-04-15 17:51:54.000000 pyiqa-0.1.6.4/pyiqa/models/inference_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3956 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/lr_scheduler.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2227 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/nima_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2302 2022-09-01 10:41:22.000000 pyiqa-0.1.6.4/pyiqa/models/pieapp_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     9300 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/sr_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      975 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/models/wadiqam_model.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     1720 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/test.py
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)    11007 2023-01-11 18:50:33.000000 pyiqa-0.1.6.4/pyiqa/train.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2405 2022-09-01 11:01:29.000000 pyiqa-0.1.6.4/pyiqa/train_nsplits.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa/utils/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      934 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/__init__.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7621 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/color_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2608 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/dist_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3345 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/download_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6017 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/file_client.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7261 2022-10-26 05:47:49.000000 pyiqa-0.1.6.4/pyiqa/utils/img_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7123 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/lmdb_util.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     7139 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/logger.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     4767 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/misc.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     6474 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/options.py
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2185 2022-08-14 08:39:51.000000 pyiqa-0.1.6.4/pyiqa/utils/registry.py
+-rwxr-xr-x   0 cfchen   (25144) cfchen   (25144)      133 2023-04-17 18:49:59.000000 pyiqa-0.1.6.4/pyiqa/version.py
+drwxr-xr-x   0 cfchen   (25144) cfchen   (25144)        0 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/pyiqa.egg-info/
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)    12233 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/PKG-INFO
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     2681 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/SOURCES.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)        1 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/dependency_links.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      170 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/requires.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)        6 2023-04-17 18:50:00.000000 pyiqa-0.1.6.4/pyiqa.egg-info/top_level.txt
+-rw-rw-r--   0 cfchen   (25144) cfchen   (25144)      169 2023-03-29 17:32:51.000000 pyiqa-0.1.6.4/requirements.txt
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)      333 2023-04-17 18:50:01.000000 pyiqa-0.1.6.4/setup.cfg
+-rw-r--r--   0 cfchen   (25144) cfchen   (25144)     3478 2023-03-29 17:15:09.000000 pyiqa-0.1.6.4/setup.py
```

### Comparing `pyiqa-0.1.6.3/LICENSE` & `pyiqa-0.1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/LICENSE_NTU-S-Lab` & `pyiqa-0.1.6.4/LICENSE_NTU-S-Lab`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/api_helpers.py` & `pyiqa-0.1.6.4/pyiqa/api_helpers.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/__init__.py` & `pyiqa-0.1.6.4/pyiqa/archs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/ahiq_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/ahiq_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/arch_util.py` & `pyiqa-0.1.6.4/pyiqa/archs/arch_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from builtins import ValueError
 from collections import OrderedDict
 import math
 import collections.abc
 from itertools import repeat
 import numpy as np
 from typing import Tuple
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/brisque_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/brisque_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/ckdn_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/ckdn_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/clip_model.py` & `pyiqa-0.1.6.4/pyiqa/archs/clip_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/clipiqa_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/clipiqa_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 AAAI 2023.
 
 Ref url: https://github.com/IceClear/CLIP-IQA
 Re-implmented by: Chaofeng Chen (https://github.com/chaofengc) with the following modification:
     - We assemble multiple prompts to improve the results of clipiqa model.
 
 """
-import os
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 from .constants import OPENAI_CLIP_MEAN, OPENAI_CLIP_STD
 
 from pyiqa.utils.registry import ARCH_REGISTRY
 from pyiqa.archs.arch_util import load_file_from_url
-from .func_util import extract_2d_patches
 from pyiqa.archs.arch_util import load_pretrained_network
 
 import clip
 from .clip_model import load
 
 
 default_model_urls = {
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/cnniqa_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/cnniqa_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/dbcnn_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/dbcnn_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/dists_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/dists_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/fid_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/fid_arch.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Martin Heusel, Hubert Ramsauer, Thomas Unterthiner, Bernhard Nessler, Sepp Hochreiter
     NeurIPS, 2017
     [2] On Aliased Resizing and Surprising Subtleties in GAN Evaluation
     Gaurav Parmar, Richard Zhang, Jun-Yan Zhu
     CVPR, 2022
 """
 
-from email.policy import default
 import os
 from tqdm import tqdm
 from glob import glob
 import numpy as np
 from scipy import linalg
 from PIL import Image
 
@@ -246,15 +245,15 @@
                 verbose=True,
                 ):
         
         assert mode in ['clean', 'legacy_pytorch', 'legacy_tensorflow'], 'Invalid calculation mode, should be in [clean, legacy_pytorch, legacy_tensorflow]' 
 
         # if both dirs are specified, compute FID between folders
         if fdir1 is not None and fdir2 is not None:
-            if not verbose:
+            if verbose:
                 print("compute FID between two folders")
             fbname1 = os.path.basename(fdir1)
             np_feats1 = get_folder_features(fdir1, self.model, num_workers=num_workers, batch_size=batch_size,
                                             device=device, mode=mode, description=f"FID {fbname1}: ", verbose=verbose)
 
             fbname2 = os.path.basename(fdir2)
             np_feats2 = get_folder_features(fdir2, self.model, num_workers=num_workers, batch_size=batch_size,
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/fsim_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/fsim_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/func_util.py` & `pyiqa-0.1.6.4/pyiqa/archs/func_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/gmsd_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/gmsd_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/hypernet_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/hypernet_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 
 import torch
 import torch.nn as nn
 import timm
 from pyiqa.utils.registry import ARCH_REGISTRY
-from pyiqa.archs.arch_util import dist_to_mos, load_pretrained_network
+from pyiqa.archs.arch_util import load_pretrained_network
 
 
 default_model_urls = {
     'resnet50-koniq': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/HyperIQA-resnet50-koniq10k-48579ec9.pth', 
 }
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/inception.py` & `pyiqa-0.1.6.4/pyiqa/archs/inception.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/iqt_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/iqt_arch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-from pyexpat import model
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torchvision.ops.deform_conv import DeformConv2d
 import numpy as np
-from einops import rearrange, repeat
-from einops.layers.torch import Rearrange
+from einops import repeat
 
 import timm
-from timm.models.vision_transformer import Block
-from timm.models.resnet import BasicBlock,Bottleneck
 
 from pyiqa.utils.registry import ARCH_REGISTRY
-from pyiqa.archs.arch_util import load_pretrained_network, default_init_weights, to_2tuple, ExactPadding2d
+from pyiqa.archs.arch_util import load_pretrained_network, to_2tuple
 
 
 class IQARegression(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.config = config
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/lpips_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/lpips_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/mad_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/mad_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/maniqa_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/maniqa_arch.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 Reference:
     - Official github: https://github.com/IIGROUP/MANIQA
 """
 
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 import timm
 
 from timm.models.vision_transformer import Block
 from .constants import IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
 from .maniqa_swin import SwinTransformer
 from torch import nn
 from einops import rearrange
 
 from pyiqa.utils.registry import ARCH_REGISTRY
-from .func_util import extract_2d_patches
 from pyiqa.archs.arch_util import load_pretrained_network
 
 default_model_urls = {
-    'pipal': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/MANIQA_PIPAL-ae6d356b.pth'
+    'pipal': 'https://github.com/chaofengc/IQA-PyTorch/releases/download/v0.1-weights/MANIQA_PIPAL-ae6d356b.pth',
+    'koniq': 'https://github.com/IIGROUP/MANIQA/releases/download/Koniq10k/ckpt_koniq10k.pt',
+    'kadid': 'https://github.com/IIGROUP/MANIQA/releases/download/Kadid10k/ckpt_kadid10k.pt',
 }
 
 
 def random_crop(x, sample_size=224, sample_num=8):
     b, c, h, w = x.shape
     th = tw = sample_size
     cropped_x = []
@@ -79,14 +79,15 @@
 @ARCH_REGISTRY.register()
 class MANIQA(nn.Module):
     def __init__(self, embed_dim=768, num_outputs=1, patch_size=8, drop=0.1,
                  depths=[2, 2], window_size=4, dim_mlp=768, num_heads=[4, 4],
                  img_size=224, num_tab=2, scale=0.13, test_sample=20,
                  pretrained=True,
                  pretrained_model_path=None,
+                 train_dataset='pipal',
                  default_mean=None,
                  default_std=None,
                  **kwargs):
         super().__init__()
         self.img_size = img_size
         self.patch_size = patch_size
         self.input_size = img_size // patch_size
@@ -151,15 +152,15 @@
         self.default_mean = torch.Tensor(IMAGENET_INCEPTION_MEAN).view(1, 3, 1, 1)
         self.default_std = torch.Tensor(IMAGENET_INCEPTION_STD).view(1, 3, 1, 1)
 
         if pretrained_model_path is not None:
             load_pretrained_network(self, pretrained_model_path, True, weight_keys='params')
             # load_pretrained_network(self, pretrained_model_path, True, )
         elif pretrained:
-            load_pretrained_network(self, default_model_urls['pipal'], True)
+            load_pretrained_network(self, default_model_urls[train_dataset], True)
 
     def extract_feature(self, save_output):
         x6 = save_output.outputs[6][:, 1:]
         x7 = save_output.outputs[7][:, 1:]
         x8 = save_output.outputs[8][:, 1:]
         x9 = save_output.outputs[9][:, 1:]
         x = torch.cat((x6, x7, x8, x9), dim=2)
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/maniqa_swin.py` & `pyiqa-0.1.6.4/pyiqa/archs/maniqa_swin.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/musiq_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/musiq_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/nima_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/nima_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/niqe_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/niqe_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     scaleFactorForGaussianDer = 0.28
     sigmaForDownsample = 0.9
 
     EPS = 1e-8
     scales = 3
     orientations = 4
     infConst = 10000
-    nanConst = 2000
+    # nanConst = 2000
 
     if resize:
         img = imresize(img, sizes=(normalizedWidth, normalizedWidth))
         img = img.clamp(0.0, 255.0)
 
     # crop image
     b, c, h, w = img.shape
```

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/nlpd_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/nlpd_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/nrqm_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/nrqm_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/paq2piq_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/paq2piq_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/pieapp_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/pieapp_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/psnr_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/psnr_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/ssim_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/ssim_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/tres_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/tres_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/vif_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/vif_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/vsi_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/vsi_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/archs/wadiqam_arch.py` & `pyiqa-0.1.6.4/pyiqa/archs/wadiqam_arch.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/__init__.py` & `pyiqa-0.1.6.4/pyiqa/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/ava_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/ava_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/bapps_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/bapps_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/data_sampler.py` & `pyiqa-0.1.6.4/pyiqa/data/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/data_util.py` & `pyiqa-0.1.6.4/pyiqa/data/data_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/flive_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/flive_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/general_fr_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/general_fr_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/general_nr_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/general_nr_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/livechallenge_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/livechallenge_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/multiscale_trans_util.py` & `pyiqa-0.1.6.4/pyiqa/data/multiscale_trans_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/pieapp_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/pieapp_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/pipal_dataset.py` & `pyiqa-0.1.6.4/pyiqa/data/pipal_dataset.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/prefetch_dataloader.py` & `pyiqa-0.1.6.4/pyiqa/data/prefetch_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/data/transforms.py` & `pyiqa-0.1.6.4/pyiqa/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/default_model_configs.py` & `pyiqa-0.1.6.4/pyiqa/default_model_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,14 +257,28 @@
     },
     'maniqa': {
         'metric_opts': {
             'type': 'MANIQA',
         },
         'metric_mode': 'NR',
     },
+    'maniqa-koniq': {
+        'metric_opts': {
+            'type': 'MANIQA',
+            'train_dataset': 'koniq',
+        },
+        'metric_mode': 'NR',
+    },
+    'maniqa-kadid': {
+        'metric_opts': {
+            'type': 'MANIQA',
+            'train_dataset': 'kadid',
+        },
+        'metric_mode': 'NR',
+    },
     'clipiqa': {
         'metric_opts': {
             'type': 'CLIPIQA',
         },
         'metric_mode': 'NR',
     },
     'clipiqa+': {
@@ -315,9 +329,14 @@
     },
     'hyperiqa': {
         'metric_opts': {
             'type': 'HyperNet',
         },
         'metric_mode': 'NR',
     },
-
+    'uranker': {
+        'metric_opts': {
+            'type': 'URanker',
+        },
+        'metric_mode': 'NR',
+    }
 })
```

### Comparing `pyiqa-0.1.6.3/pyiqa/losses/__init__.py` & `pyiqa-0.1.6.4/pyiqa/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/losses/iqa_losses.py` & `pyiqa-0.1.6.4/pyiqa/losses/iqa_losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/losses/loss_util.py` & `pyiqa-0.1.6.4/pyiqa/losses/loss_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/losses/losses.py` & `pyiqa-0.1.6.4/pyiqa/losses/losses.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/matlab_utils/__init__.py` & `pyiqa-0.1.6.4/pyiqa/matlab_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/matlab_utils/functions.py` & `pyiqa-0.1.6.4/pyiqa/matlab_utils/functions.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/matlab_utils/math_util.py` & `pyiqa-0.1.6.4/pyiqa/matlab_utils/math_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/matlab_utils/resize.py` & `pyiqa-0.1.6.4/pyiqa/matlab_utils/resize.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/matlab_utils/scfpyr_util.py` & `pyiqa-0.1.6.4/pyiqa/matlab_utils/scfpyr_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/metrics/__init__.py` & `pyiqa-0.1.6.4/pyiqa/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/metrics/correlation_coefficient.py` & `pyiqa-0.1.6.4/pyiqa/metrics/correlation_coefficient.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/__init__.py` & `pyiqa-0.1.6.4/pyiqa/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/bapps_model.py` & `pyiqa-0.1.6.4/pyiqa/models/bapps_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/base_model.py` & `pyiqa-0.1.6.4/pyiqa/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/dbcnn_model.py` & `pyiqa-0.1.6.4/pyiqa/models/dbcnn_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/general_iqa_model.py` & `pyiqa-0.1.6.4/pyiqa/models/general_iqa_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/hypernet_model.py` & `pyiqa-0.1.6.4/pyiqa/models/hypernet_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/inference_model.py` & `pyiqa-0.1.6.4/pyiqa/models/inference_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,29 +57,29 @@
     def to(self, device):
         self.net.to(device)
         self.device = torch.device(device)
         return self
 
     def forward(self, target, ref=None, **kwargs):
 
-        torch.set_grad_enabled(self.as_loss)
+        with torch.set_grad_enabled(self.as_loss):
 
-        if 'fid' in self.metric_name:
-            output = self.net(target, ref, device=self.device, **kwargs)
-        else:
-            if not torch.is_tensor(target):
-                target = imread2tensor(target)
-                target = target.unsqueeze(0)
-                if self.metric_mode == 'FR':
-                    assert ref is not None, 'Please specify reference image for Full Reference metric'
-                    ref = imread2tensor(ref)
-                    ref = ref.unsqueeze(0)
+            if 'fid' in self.metric_name:
+                output = self.net(target, ref, device=self.device, **kwargs)
+            else:
+                if not torch.is_tensor(target):
+                    target = imread2tensor(target)
+                    target = target.unsqueeze(0)
+                    if self.metric_mode == 'FR':
+                        assert ref is not None, 'Please specify reference image for Full Reference metric'
+                        ref = imread2tensor(ref)
+                        ref = ref.unsqueeze(0)
 
-            if self.metric_mode == 'FR':
-                output = self.net(target.to(self.device), ref.to(self.device), **kwargs)
-            elif self.metric_mode == 'NR':
-                output = self.net(target.to(self.device), **kwargs)
+                if self.metric_mode == 'FR':
+                    output = self.net(target.to(self.device), ref.to(self.device), **kwargs)
+                elif self.metric_mode == 'NR':
+                    output = self.net(target.to(self.device), **kwargs)
 
         if self.as_loss:
             return weight_reduce_loss(output, self.loss_weight, self.loss_reduction)
         else:
             return output
```

### Comparing `pyiqa-0.1.6.3/pyiqa/models/lr_scheduler.py` & `pyiqa-0.1.6.4/pyiqa/models/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/nima_model.py` & `pyiqa-0.1.6.4/pyiqa/models/nima_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/pieapp_model.py` & `pyiqa-0.1.6.4/pyiqa/models/pieapp_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/sr_model.py` & `pyiqa-0.1.6.4/pyiqa/models/sr_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/models/wadiqam_model.py` & `pyiqa-0.1.6.4/pyiqa/models/wadiqam_model.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/test.py` & `pyiqa-0.1.6.4/pyiqa/test.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/train.py` & `pyiqa-0.1.6.4/pyiqa/train.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/train_nsplits.py` & `pyiqa-0.1.6.4/pyiqa/train_nsplits.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/__init__.py` & `pyiqa-0.1.6.4/pyiqa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/color_util.py` & `pyiqa-0.1.6.4/pyiqa/utils/color_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/dist_util.py` & `pyiqa-0.1.6.4/pyiqa/utils/dist_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/download_util.py` & `pyiqa-0.1.6.4/pyiqa/utils/download_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/file_client.py` & `pyiqa-0.1.6.4/pyiqa/utils/file_client.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/img_util.py` & `pyiqa-0.1.6.4/pyiqa/utils/img_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/lmdb_util.py` & `pyiqa-0.1.6.4/pyiqa/utils/lmdb_util.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/logger.py` & `pyiqa-0.1.6.4/pyiqa/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/misc.py` & `pyiqa-0.1.6.4/pyiqa/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/options.py` & `pyiqa-0.1.6.4/pyiqa/utils/options.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa/utils/registry.py` & `pyiqa-0.1.6.4/pyiqa/utils/registry.py`

 * *Files identical despite different names*

### Comparing `pyiqa-0.1.6.3/pyiqa.egg-info/SOURCES.txt` & `pyiqa-0.1.6.4/pyiqa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 pyiqa/archs/nlpd_arch.py
 pyiqa/archs/nrqm_arch.py
 pyiqa/archs/paq2piq_arch.py
 pyiqa/archs/pieapp_arch.py
 pyiqa/archs/psnr_arch.py
 pyiqa/archs/ssim_arch.py
 pyiqa/archs/tres_arch.py
+pyiqa/archs/uranker_arch.py
 pyiqa/archs/vif_arch.py
 pyiqa/archs/vsi_arch.py
 pyiqa/archs/wadiqam_arch.py
 pyiqa/data/__init__.py
 pyiqa/data/ava_dataset.py
 pyiqa/data/bapps_dataset.py
 pyiqa/data/data_sampler.py
```

### Comparing `pyiqa-0.1.6.3/setup.py` & `pyiqa-0.1.6.4/setup.py`

 * *Files identical despite different names*

