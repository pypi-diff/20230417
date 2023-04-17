# Comparing `tmp/osl-dynamics-1.2.1.tar.gz` & `tmp/osl-dynamics-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osl-dynamics-1.2.1.tar", last modified: Fri Apr 14 14:57:17 2023, max compression
+gzip compressed data, was "osl-dynamics-1.2.2.tar", last modified: Mon Apr 17 12:40:43 2023, max compression
```

## Comparing `osl-dynamics-1.2.1.tar` & `osl-dynamics-1.2.2.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.768564 osl-dynamics-1.2.1/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-14 14:57:17.768810 osl-dynamics-1.2.1/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4128 2023-03-26 09:15:19.000000 osl-dynamics-1.2.1/README.rst
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.546273 osl-dynamics-1.2.1/osl_dynamics/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/__init__.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.638726 osl-dynamics-1.2.1/osl_dynamics/analysis/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      231 2023-04-06 15:27:35.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/connectivity.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6323 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/fisher_kernel.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/gmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22485 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    18679 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/power.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/regression.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    44293 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/spectral.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/static.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7333 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/statistics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/analysis/workbench.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8199 2023-03-30 19:34:59.000000 osl-dynamics-1.2.1/osl_dynamics/array_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.648697 osl-dynamics-1.2.1/osl_dynamics/config_api/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      222 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3837 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/pipeline.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    50431 2023-04-14 14:48:06.000000 osl-dynamics-1.2.1/osl_dynamics/config_api/wrappers.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.713324 osl-dynamics-1.2.1/osl_dynamics/data/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36748 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/data/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/osl.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/data/processing.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-03-23 11:26:21.000000 osl-dynamics-1.2.1/osl_dynamics/data/rw.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-03-18 14:07:34.000000 osl-dynamics-1.2.1/osl_dynamics/data/spm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-04-06 15:27:32.000000 osl-dynamics-1.2.1/osl_dynamics/data/task.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/data/tf.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.729270 osl-dynamics-1.2.1/osl_dynamics/files/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/functions.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.854311 osl-dynamics-1.2.1/osl_dynamics/files/mask/
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/__init__.py
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.954795 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-03-10 15:37:52.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.996108 osl-dynamics-1.2.1/osl_dynamics/files/scanner/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/ctf275_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.472410 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D148.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi128.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi160.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi256.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi32.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1010.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1020.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.outline
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.481494 osl-dynamics-1.2.1/osl_dynamics/files/scene/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scene/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/files/scene/mode_scene.scene
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.559530 osl-dynamics-1.2.1/osl_dynamics/inference/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/inference/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/inference/callbacks.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     7378 2023-03-20 14:13:14.000000 osl-dynamics-1.2.1/osl_dynamics/inference/initializers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    42087 2023-03-20 14:13:14.000000 osl-dynamics-1.2.1/osl_dynamics/inference/layers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/inference/metrics.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15572 2023-04-14 14:48:19.000000 osl-dynamics-1.2.1/osl_dynamics/inference/modes.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-02-13 15:05:52.000000 osl-dynamics-1.2.1/osl_dynamics/inference/regularizers.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/inference/tf_ops.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.658855 osl-dynamics-1.2.1/osl_dynamics/models/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-02-28 15:36:39.000000 osl-dynamics-1.2.1/osl_dynamics/models/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16781 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/dynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/models/dynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    41033 2023-03-21 18:26:08.000000 osl-dynamics-1.2.1/osl_dynamics/models/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    15849 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/inf_mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/mage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    20241 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/mdynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-02-19 13:57:27.000000 osl-dynamics-1.2.1/osl_dynamics/models/mdynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    16639 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/mod_base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-03-24 10:57:23.000000 osl-dynamics-1.2.1/osl_dynamics/models/sage.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    28440 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/models/sedynemo.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    29860 2023-03-20 14:13:15.000000 osl-dynamics-1.2.1/osl_dynamics/models/sedynemo_obs.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13439 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/models/state_dynemo.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.711809 osl-dynamics-1.2.1/osl_dynamics/simulation/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/base.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/hmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/hsmm.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2022-10-24 10:06:46.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/mar.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-03-21 18:25:01.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/mvn.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-01-28 15:39:30.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/sin.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-03-28 21:05:20.000000 osl-dynamics-1.2.1/osl_dynamics/simulation/sm.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:17.761643 osl-dynamics-1.2.1/osl_dynamics/utils/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2022-10-30 10:07:31.000000 osl-dynamics-1.2.1/osl_dynamics/utils/__init__.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2022-10-30 10:07:31.000000 osl-dynamics-1.2.1/osl_dynamics/utils/decorators.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/misc.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/model.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/parcellation.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)    55601 2023-04-14 14:48:30.000000 osl-dynamics-1.2.1/osl_dynamics/utils/plotting.py
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-04-11 10:48:22.000000 osl-dynamics-1.2.1/osl_dynamics/utils/topoplots.py
-drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-14 14:57:16.557973 osl-dynamics-1.2.1/osl_dynamics.egg-info/
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-14 14:57:16.555301 osl-dynamics-1.2.1/osl_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 wlo995   (37469) woolrich (37107)     8209 2023-04-14 14:57:16.555979 osl-dynamics-1.2.1/osl_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-04-14 14:57:16.556779 osl-dynamics-1.2.1/osl_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-04-14 14:57:16.557409 osl-dynamics-1.2.1/osl_dynamics.egg-info/requires.txt
--rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-04-14 14:57:16.558134 osl-dynamics-1.2.1/osl_dynamics.egg-info/top_level.txt
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1064 2023-04-14 14:57:17.769489 osl-dynamics-1.2.1/setup.cfg
--rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2022-10-17 12:20:33.000000 osl-dynamics-1.2.1/setup.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.897807 osl-dynamics-1.2.2/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-17 12:40:43.897995 osl-dynamics-1.2.2/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4128 2023-04-17 08:41:13.000000 osl-dynamics-1.2.2/README.rst
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.051322 osl-dynamics-1.2.2/osl_dynamics/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      643 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/__init__.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.130385 osl-dynamics-1.2.2/osl_dynamics/analysis/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      231 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    27101 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/connectivity.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6323 2023-04-14 14:48:30.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/fisher_kernel.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6165 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/gmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22485 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    18679 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/power.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3268 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/regression.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    44293 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/spectral.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7487 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/static.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7333 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/statistics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5688 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/analysis/workbench.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8199 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/array_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.144033 osl-dynamics-1.2.2/osl_dynamics/config_api/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      222 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      751 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/cli.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4477 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/pipeline.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    50523 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/config_api/wrappers.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.181753 osl-dynamics-1.2.2/osl_dynamics/data/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      185 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36748 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/osl.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6757 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/processing.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8574 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/rw.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2809 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/spm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2447 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/data/task.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4726 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/data/tf.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.204462 osl-dynamics-1.2.2/osl_dynamics/files/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      883 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      434 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/functions.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.461814 osl-dynamics-1.2.2/osl_dynamics/files/mask/
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     7241 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   724726 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723434 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   723505 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   713031 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   710727 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)   712178 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1649 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/__init__.py
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      971 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.517260 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41373 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9131 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      669 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    36166 2023-03-10 15:37:52.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    24111 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    33885 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    23705 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63185 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)    63835 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     5233 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.520824 osl-dynamics-1.2.2/osl_dynamics/files/scanner/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      268 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5568 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/ctf275_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.684049 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6679 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D148.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11272 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    22296 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42102 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7077 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12927 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    25461 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    46654 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7134 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5164 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5813 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5697 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi128.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      770 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7128 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi160.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11414 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi256.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1470 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi32.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2860 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5110 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5581 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5833 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6367 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11302 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11794 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7800 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6362 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3165 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2016 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2906 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2989 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6361 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15330 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3827 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1010.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1020.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5269 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6161 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6127 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     3249 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5961 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14973 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2643 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5489 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6873 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4979 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2547 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9969 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2985 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6363 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5691 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6366 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.outline
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20670 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19775 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    14079 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20655 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6565 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8696 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.686730 osl-dynamics-1.2.2/osl_dynamics/files/scene/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       82 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scene/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)  1511998 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/files/scene/mode_scene.scene
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.781106 osl-dynamics-1.2.2/osl_dynamics/inference/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      160 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/inference/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7118 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/inference/callbacks.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     7410 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/inference/initializers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    42087 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/inference/layers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11394 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/inference/metrics.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15547 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/inference/modes.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6797 2023-02-13 15:05:52.000000 osl-dynamics-1.2.2/osl_dynamics/inference/regularizers.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1647 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/inference/tf_ops.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.826545 osl-dynamics-1.2.2/osl_dynamics/models/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     1426 2023-02-28 15:36:39.000000 osl-dynamics-1.2.2/osl_dynamics/models/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16781 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/dynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11105 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/dynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    41033 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    15849 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/inf_mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    23641 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    20241 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mdynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    11366 2023-02-19 13:57:27.000000 osl-dynamics-1.2.2/osl_dynamics/models/mdynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    16639 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/mod_base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    19196 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/sage.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    28468 2023-04-17 12:34:08.000000 osl-dynamics-1.2.2/osl_dynamics/models/sedynemo.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    29860 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/sedynemo_obs.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13439 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/models/state_dynemo.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.877875 osl-dynamics-1.2.2/osl_dynamics/simulation/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      566 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      974 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/base.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    30162 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/hmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    12958 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/hsmm.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2710 2022-10-24 10:06:46.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/mar.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    26028 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/mvn.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4809 2023-01-28 15:39:30.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/sin.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    10563 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/simulation/sm.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.897102 osl-dynamics-1.2.2/osl_dynamics/utils/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      287 2022-10-30 10:07:31.000000 osl-dynamics-1.2.2/osl_dynamics/utils/__init__.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     5701 2022-10-30 10:07:31.000000 osl-dynamics-1.2.2/osl_dynamics/utils/decorators.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    13545 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/misc.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     6997 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/model.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     2206 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/parcellation.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)    55601 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/plotting.py
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     9063 2023-04-17 08:41:14.000000 osl-dynamics-1.2.2/osl_dynamics/utils/topoplots.py
+drwxr-sr-x   0 wlo995   (37469) woolrich (37107)        0 2023-04-17 12:40:43.065381 osl-dynamics-1.2.2/osl_dynamics.egg-info/
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     4441 2023-04-17 12:40:43.062030 osl-dynamics-1.2.2/osl_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)     8279 2023-04-17 12:40:43.062562 osl-dynamics-1.2.2/osl_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)        1 2023-04-17 12:40:43.063229 osl-dynamics-1.2.2/osl_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       71 2023-04-17 12:40:43.063806 osl-dynamics-1.2.2/osl_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)      141 2023-04-17 12:40:43.064729 osl-dynamics-1.2.2/osl_dynamics.egg-info/requires.txt
+-rw-r--r--   0 wlo995   (37469) woolrich (37107)       13 2023-04-17 12:40:43.065550 osl-dynamics-1.2.2/osl_dynamics.egg-info/top_level.txt
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)     1161 2023-04-17 12:40:43.898763 osl-dynamics-1.2.2/setup.cfg
+-rwxr-xr-x   0 wlo995   (37469) woolrich (37107)      189 2022-10-17 12:20:33.000000 osl-dynamics-1.2.2/setup.py
```

### Comparing `osl-dynamics-1.2.1/PKG-INFO` & `osl-dynamics-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.1
+Version: 1.2.2
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
```

### Comparing `osl-dynamics-1.2.1/README.rst` & `osl-dynamics-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/connectivity.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/connectivity.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/fisher_kernel.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/fisher_kernel.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/gmm.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/gmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/modes.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/modes.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/power.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/power.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/regression.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/regression.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/spectral.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/spectral.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/static.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/static.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/statistics.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/analysis/workbench.py` & `osl-dynamics-1.2.2/osl_dynamics/analysis/workbench.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/array_ops.py` & `osl-dynamics-1.2.2/osl_dynamics/array_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/config_api/pipeline.py` & `osl-dynamics-1.2.2/osl_dynamics/config_api/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Functions for running full pipelines via the config API.
 
 See the `toolbox examples
 <https://github.com/OHBA-analysis/osl-dynamics/tree/main/examples/toolbox_paper>`_
 for scripts that use the config API.
 """
 
-import os
 import logging
-import yaml
-import pprint
+import os
 import pickle
+import pprint
+from pathlib import Path
+
 import numpy as np
+import yaml
 
 from osl_dynamics.config_api import wrappers
 from osl_dynamics.utils.misc import override_dict_defaults
 
 _logger = logging.getLogger("osl-dynamics")
 
 
@@ -63,15 +65,15 @@
         Function to execute.
     """
     func = None
 
     # Check if the requested function is one of the custom functions
     if extra_funcs is not None:
         func_ind = [
-            idx if (f.__name__ == method) else -1 for idx, f in enumerate(extra_funcs)
+            idx if (f.__name__ == name) else -1 for idx, f in enumerate(extra_funcs)
         ]
         if np.max(func_ind) > -1:
             func = extra_funcs[np.argmax(func_ind)]
 
     # Check osl_dynamics.config_api.wrappers
     if func is None and hasattr(wrappers, name):
         func = getattr(wrappers, name)
@@ -128,7 +130,34 @@
                 func(data=data, output_dir=output_dir, **kwargs)
             except Exception as e:
                 _logger.exception(e)
 
     # Delete the temporary directory created by the Data class
     if data is not None:
         data.delete_dir()
+
+
+def run_pipeline_from_file(
+    config_file,
+    output_directory,
+    restrict: str,
+):
+    """Run a pipeline from a config file.
+
+    Parameters
+    ----------
+    config_file : str
+        Path to the config file.
+    output_directory : str
+        Path to the output directory.
+    restrict : str
+        GPU to use. Optional.
+    """
+    if restrict is not None:
+        from osl_dynamics.inference.tf_ops import gpu_growth, select_gpu
+
+        select_gpu(int(restrict))
+        gpu_growth()
+    config_path = Path(config_file)
+    config = config_path.read_text()
+
+    run_pipeline(config, output_directory)
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics/config_api/wrappers.py` & `osl-dynamics-1.2.2/osl_dynamics/config_api/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     output_dir : str
         Path to output directory.
     config_kwargs : dict
         Keyword arguments to pass to hmm.Config. Defaults to::
 
             {'sequence_length': 2000,
              'batch_size': 32,
-             'learning_rate': 0.001,
+             'learning_rate': 0.01,
              'n_epochs': 20}.
     init_kwargs : dict
         Keyword arguments to pass to :code:`Model.random_state_time_course_initialization`.
         Optional, defaults to::
 
             {'n_init': 3, 'n_epochs': 1}.
     fit_kwargs : dict
@@ -118,15 +118,15 @@
 
     # Create the model object
     _logger.info("Building model")
     default_config_kwargs = {
         "n_channels": data.n_channels,
         "sequence_length": 2000,
         "batch_size": 32,
-        "learning_rate": 0.001,
+        "learning_rate": 0.01,
         "n_epochs": 20,
     }
     config_kwargs = override_dict_defaults(default_config_kwargs, config_kwargs)
     _logger.info(f"Using config_kwargs: {config_kwargs}")
     config = hmm.Config(**config_kwargs)
     model = hmm.Model(config)
     model.summary()
@@ -258,14 +258,17 @@
     init_kwargs = override_dict_defaults(default_init_kwargs, init_kwargs)
     _logger.info(f"Using init_kwargs: {init_kwargs}")
     init_history = model.random_subset_initialization(data, **init_kwargs)
 
     # Training
     history = model.fit(data, **fit_kwargs)
 
+    # Add free energy to the history object
+    history["free_energy"] = history["loss"][-1]
+
     # Save trained model
     _logger.info(f"Saving model to: {model_dir}")
     model.save(model_dir)
     save(f"{model_dir}/init_history.pkl", init_history)
     save(f"{model_dir}/history.pkl", history)
 
     if save_inf_params:
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/base.py` & `osl-dynamics-1.2.2/osl_dynamics/data/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/osl.py` & `osl-dynamics-1.2.2/osl_dynamics/data/osl.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/processing.py` & `osl-dynamics-1.2.2/osl_dynamics/data/processing.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/rw.py` & `osl-dynamics-1.2.2/osl_dynamics/data/rw.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/spm.py` & `osl-dynamics-1.2.2/osl_dynamics/data/spm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/task.py` & `osl-dynamics-1.2.2/osl_dynamics/data/task.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/data/tf.py` & `osl-dynamics-1.2.2/osl_dynamics/data/tf.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/files/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/MNI152_T1_8mm_brain.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.L.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.midthickness.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ParcellationPilot.R.very_inflated.32k_fs_LR.surf.gii`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/mask/ft_8mm_brain_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser50_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/Glasser52_binary_space-MNI152NLin6_res-8x8x8.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/aal_cortical_merged_8mm_stacked.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fMRI_parcellation_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_3PCC_ips_reduced_2mm_ss5mm_ds8mm_adj.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_reduced_2mm_ss5mm_ds8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_6mm_exclusive.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/fmri_d100_parcellation_with_PCC_tighterMay15_v2_8mm.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/parcellation/giles_39_binary.nii.gz` & `osl-dynamics-1.2.2/osl_dynamics/files/parcellation/giles_39_binary.nii.gz`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/ctf275_channel_names.npy` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/ctf275_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D148.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D148.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/4D248_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/4D248_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF151_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/CTF275_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1005.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1010.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/EEG1020.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/EEG1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/QuikCap_NSL_128.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/acticap-64ch-standard2.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi128.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi16.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi160.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi256.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi32.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/biosemi64.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/dccn_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM1.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM1.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM10.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM10.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM11.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM11.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM14.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM14.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM15.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM15.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM16.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM16.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM17.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM17.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM20.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM20.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM22.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM22.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM23.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM23.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM24.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM24.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM25.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM25.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM3.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM3.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/easycapM7.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/easycapM7.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1005.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1010.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1010.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/elec1020.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/elec1020.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/mpi_customized_acticap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/natmeg_customized_eeg1005.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag122planar.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag122planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306all_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306cmb_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306mag_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/neuromag306planar_helmet.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/quickcap64.outline` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/quickcap64.outline`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440_old.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440ag.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440all.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440all.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/layouts/yokogawa440pg.lay`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scanner/neuromag306_channel_names.npy` & `osl-dynamics-1.2.2/osl_dynamics/files/scanner/neuromag306_channel_names.npy`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/files/scene/mode_scene.scene` & `osl-dynamics-1.2.2/osl_dynamics/files/scene/mode_scene.scene`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/callbacks.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/callbacks.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/initializers.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/initializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,16 @@
         # Get the variable (i.e. weights) we want to re-initialize
         if key == "recurrent_initializer":
             var = getattr(init_container, "recurrent_kernel")
         else:
             var = getattr(init_container, key.replace("_initializer", ""))
 
         # Assign new random values to the variable
-        var.assign(new_initializer(var.shape, var.dtype))
+        if var is not None:
+            var.assign(new_initializer(var.shape, var.dtype))
 
 
 def reinitialize_model_weights(model, keep=None):
     """Re-initialize the weights in the model.
 
     Parameters
     ----------
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/layers.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/layers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/metrics.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/metrics.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/modes.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
 
 def convert_to_mne_raw(
     alpha,
     raw,
     ch_names=None,
     n_embeddings=None,
     n_window=None,
-    extra_chans=None,
+    extra_chans="stim",
     verbose=False,
 ):
     """Convert a time series to an MNE Raw object.
 
     Parameters
     ----------
     alpha : np.ndarray
@@ -370,15 +370,15 @@
         Name for each channel. Optional. Defaults to alpha_0...alpha_{n_modes-1}.
     n_embeddings : int
         Number of embeddings that was used to prepare time-delay embedded
         training data. Optional.
     n_window : int
         Number of samples used to smooth amplitude envelope data. Optional.
     extra_chans : str or list of str
-        Extra channel types to add to the Raw object. Defaults to an empty list.
+        Extra channel types to add to the Raw object.
     verbose : bool
         Should we print a verbose?
 
     Returns
     -------
     alpha_raw : mne.io.Raw
         Raw object for alpha.
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/regularizers.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/regularizers.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/inference/tf_ops.py` & `osl-dynamics-1.2.2/osl_dynamics/inference/tf_ops.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/dynemo.py` & `osl-dynamics-1.2.2/osl_dynamics/models/dynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/dynemo_obs.py` & `osl-dynamics-1.2.2/osl_dynamics/models/dynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/hmm.py` & `osl-dynamics-1.2.2/osl_dynamics/models/hmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/inf_mod_base.py` & `osl-dynamics-1.2.2/osl_dynamics/models/inf_mod_base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/mage.py` & `osl-dynamics-1.2.2/osl_dynamics/models/mage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/mdynemo.py` & `osl-dynamics-1.2.2/osl_dynamics/models/mdynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/mdynemo_obs.py` & `osl-dynamics-1.2.2/osl_dynamics/models/mdynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/mod_base.py` & `osl-dynamics-1.2.2/osl_dynamics/models/mod_base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/sage.py` & `osl-dynamics-1.2.2/osl_dynamics/models/sage.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/sedynemo.py` & `osl-dynamics-1.2.2/osl_dynamics/models/sedynemo.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,30 +501,30 @@
             config.dev_activation,
             config.dev_dropout,
             name="means_dev_map_input",
         )
         means_dev_map_layer = layers.Dense(config.n_channels, name="means_dev_map")
 
         norm_means_dev_map_layer = layers.LayerNormalization(
-            axis=-1, name="norm_means_dev_map"
+            axis=-1, scale=False, name="norm_means_dev_map"
         )
 
         means_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_means,
             initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
             name="means_dev_mag_inf_alpha_input",
         )
         means_dev_mag_inf_alpha_layer = layers.Activation(
             "softplus", name="means_dev_mag_inf_alpha"
         )
         means_dev_mag_inf_beta_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_means,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
+            initializer=initializers.TruncatedNormal(mean=10, stddev=0.02),
             name="means_dev_mag_inf_beta_input",
         )
         means_dev_mag_inf_beta_layer = layers.Activation(
             "softplus", name="means_dev_mag_inf_beta"
         )
         means_dev_mag_layer = SampleGammaDistributionLayer(
             config.covariances_epsilon, name="means_dev_mag"
@@ -587,30 +587,30 @@
             config.dev_dropout,
             name="covs_dev_map_input",
         )
         covs_dev_map_layer = layers.Dense(
             config.n_channels * (config.n_channels + 1) // 2, name="covs_dev_map"
         )
         norm_covs_dev_map_layer = layers.LayerNormalization(
-            axis=-1, name="norm_covs_dev_map"
+            axis=-1, scale=False, name="norm_covs_dev_map"
         )
 
         covs_dev_mag_inf_alpha_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_covariances,
             initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
             name="covs_dev_mag_inf_alpha_input",
         )
         covs_dev_mag_inf_alpha_layer = layers.Activation(
             "softplus", name="covs_dev_mag_inf_alpha"
         )
         covs_dev_mag_inf_beta_input_layer = LearnableTensorLayer(
             shape=(config.n_subjects, config.n_modes, 1),
             learn=config.learn_covariances,
-            initializer=initializers.TruncatedNormal(mean=0, stddev=0.02),
+            initializer=initializers.TruncatedNormal(mean=10, stddev=0.02),
             name="covs_dev_mag_inf_beta_input",
         )
         covs_dev_mag_inf_beta_layer = layers.Activation(
             "softplus", name="covs_dev_mag_inf_beta"
         )
         covs_dev_mag_layer = SampleGammaDistributionLayer(
             config.covariances_epsilon, name="covs_dev_mag"
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/sedynemo_obs.py` & `osl-dynamics-1.2.2/osl_dynamics/models/sedynemo_obs.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/models/state_dynemo.py` & `osl-dynamics-1.2.2/osl_dynamics/models/state_dynemo.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/__init__.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/base.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/base.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/hmm.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/hmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/hsmm.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/hsmm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/mar.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/mar.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/mvn.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/mvn.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/sin.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/sin.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/simulation/sm.py` & `osl-dynamics-1.2.2/osl_dynamics/simulation/sm.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/decorators.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/misc.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/model.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/model.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/parcellation.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/parcellation.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/plotting.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics/utils/topoplots.py` & `osl-dynamics-1.2.2/osl_dynamics/utils/topoplots.py`

 * *Files identical despite different names*

### Comparing `osl-dynamics-1.2.1/osl_dynamics.egg-info/PKG-INFO` & `osl-dynamics-1.2.2/osl_dynamics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osl-dynamics
-Version: 1.2.1
+Version: 1.2.2
 Summary: Models for infering dynamics in neuroimaging data
 Home-page: https://github.com/OHBA-analysis/osl-dynamics
 License: MIT
 Project-URL: Documentation, https://osl-dynamics.readthedocs.io/en/latest/
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 ============
```

### Comparing `osl-dynamics-1.2.1/osl_dynamics.egg-info/SOURCES.txt` & `osl-dynamics-1.2.2/osl_dynamics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 setup.cfg
 setup.py
 osl_dynamics/__init__.py
 osl_dynamics/array_ops.py
 osl_dynamics.egg-info/PKG-INFO
 osl_dynamics.egg-info/SOURCES.txt
 osl_dynamics.egg-info/dependency_links.txt
+osl_dynamics.egg-info/entry_points.txt
 osl_dynamics.egg-info/requires.txt
 osl_dynamics.egg-info/top_level.txt
 osl_dynamics/analysis/__init__.py
 osl_dynamics/analysis/connectivity.py
 osl_dynamics/analysis/fisher_kernel.py
 osl_dynamics/analysis/gmm.py
 osl_dynamics/analysis/modes.py
 osl_dynamics/analysis/power.py
 osl_dynamics/analysis/regression.py
 osl_dynamics/analysis/spectral.py
 osl_dynamics/analysis/static.py
 osl_dynamics/analysis/statistics.py
 osl_dynamics/analysis/workbench.py
 osl_dynamics/config_api/__init__.py
+osl_dynamics/config_api/cli.py
 osl_dynamics/config_api/pipeline.py
 osl_dynamics/config_api/wrappers.py
 osl_dynamics/data/__init__.py
 osl_dynamics/data/base.py
 osl_dynamics/data/osl.py
 osl_dynamics/data/processing.py
 osl_dynamics/data/rw.py
```

### Comparing `osl-dynamics-1.2.1/setup.cfg` & `osl-dynamics-1.2.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osl-dynamics
-version = 1.2.1
+version = 1.2.2
 description = Models for infering dynamics in neuroimaging data
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/OHBA-analysis/osl-dynamics
 project_urls = 
 	Documentation = https://osl-dynamics.readthedocs.io/en/latest/
@@ -50,11 +50,15 @@
 [options.package_data]
 * = *
 
 [build_sphinx]
 source_dir = doc
 build_dir = build/sphinx
 
+[options.entry_points]
+console_scripts = 
+	osld-pipeline = osl_dynamics.config_api.cli:pipeline
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

