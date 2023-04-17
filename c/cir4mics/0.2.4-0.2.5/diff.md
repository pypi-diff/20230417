# Comparing `tmp/cir4mics-0.2.4.tar.gz` & `tmp/cir4mics-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cir4mics-0.2.4.tar", max compression
+gzip compressed data, was "cir4mics-0.2.5.tar", max compression
```

## Comparing `cir4mics-0.2.4.tar` & `cir4mics-0.2.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1068 2023-04-12 14:30:48.348102 cir4mics-0.2.4/LICENSE
--rw-r--r--   0        0        0       67 2023-04-12 14:59:50.266838 cir4mics-0.2.4/READMEpypi.md
--rw-r--r--   0        0        0  1033056 2023-04-12 15:34:17.430636 cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/Dynamics-checkpoint.ipynb
--rw-r--r--   0        0        0   110965 2023-04-12 14:30:48.372103 cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/Include_models-checkpoint.ipynb
--rw-r--r--   0        0        0  1013844 2023-04-14 12:51:25.778620 cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/NPC_testlab-checkpoint.ipynb
--rwxr-xr-x   0        0        0    21337 2023-04-12 14:30:48.352102 cir4mics-0.2.4/cir4mics/Analyse_deformed.py
--rwxr-xr-x   0        0        0    34716 2023-04-14 12:49:51.018067 cir4mics-0.2.4/cir4mics/DeformNPC.py
--rw-r--r--   0        0        0  1033056 2023-04-12 15:34:17.430636 cir4mics-0.2.4/cir4mics/Dynamics.ipynb
--rw-r--r--   0        0        0   110965 2023-04-12 15:34:52.338891 cir4mics-0.2.4/cir4mics/Include_models.ipynb
--rwxr-xr-x   0        0        0    46387 2023-04-14 12:46:22.672881 cir4mics-0.2.4/cir4mics/NPC_plotting.py
--rw-r--r--   0        0        0  1013844 2023-04-14 12:51:25.778620 cir4mics-0.2.4/cir4mics/NPC_testlab.ipynb
--rwxr-xr-x   0        0        0    87897 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/Nups_Info.py
--rw-r--r--   0        0        0        0 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/__init__.py
--rwxr-xr-x   0        0        0     4487 2023-04-14 12:48:13.909508 cir4mics-0.2.4/cir4mics/call_functions.py
--rwxr-xr-x   0        0        0     1540 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/config.yaml
--rw-r--r--   0        0        0    97163 2023-04-14 12:51:41.794714 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-14 12:51:41.794714 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 14:41:46.991998 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 14:41:46.991998 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 14:42:47.021021 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 14:42:47.021021 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 14:50:22.122689 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 14:50:22.122689 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97665 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0      845 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 15:34:52.562893 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 15:34:52.562893 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-12 14:53:41.671850 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-12 14:53:41.671850 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    97163 2023-04-14 12:35:49.509796 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0      773 2023-04-14 12:35:49.509796 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    13749 2023-04-14 12:48:50.885719 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0      703 2023-04-14 12:48:50.885719 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    13749 2023-04-14 12:50:03.310138 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0      703 2023-04-14 12:50:03.310138 cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt
--rw-r--r--   0        0        0    18997 2023-04-14 12:51:41.826714 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0    19032 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-12 14:41:47.023999 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-12 14:42:47.045022 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-12 14:50:22.146689 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    18951 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-12 15:34:52.586893 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-12 14:53:41.703850 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    18997 2023-04-14 12:35:49.537796 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0     2857 2023-04-14 12:48:50.889720 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0     2857 2023-04-14 12:50:03.314138 cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-14 12:51:41.850714 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 14:41:47.043999 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 14:42:47.073022 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 14:50:22.166689 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    68911 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 15:34:52.614893 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-12 14:53:41.731850 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    68839 2023-04-14 12:35:49.561796 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0    11018 2023-04-14 12:48:50.889720 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0    11018 2023-04-14 12:50:03.314138 cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-14 12:51:41.866715 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0    34473 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-12 14:41:47.068000 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-12 14:42:47.093023 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-12 14:50:22.182689 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    34504 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-12 15:34:52.634894 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-12 14:53:41.751850 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
--rw-r--r--   0        0        0    34467 2023-04-14 12:35:49.585796 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
--rw-r--r--   0        0        0     5288 2023-04-14 12:48:50.889720 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0     5288 2023-04-14 12:50:03.314138 cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
--rw-r--r--   0        0        0     1622 2023-04-12 14:30:48.388103 cir4mics-0.2.4/cir4mics/dynamics.yaml
--rwxr-xr-x   0        0        0    20327 2023-04-14 12:46:46.085012 cir4mics-0.2.4/cir4mics/exportCSV.py
--rwxr-xr-x   0        0        0     3999 2023-04-12 14:30:48.392103 cir4mics-0.2.4/cir4mics/newModels/ModifyChimeraOutput.py
--rwxr-xr-x   0        0        0     6190 2023-04-12 14:30:48.392103 cir4mics-0.2.4/cir4mics/newModels/parse_NPC_cifs.py
--rwxr-xr-x   0        0        0     3901 2023-04-14 12:34:12.297447 cir4mics-0.2.4/cir4mics/npc.py
--rw-r--r--   0        0        0      684 2023-04-12 14:30:48.392103 cir4mics-0.2.4/cir4mics/utility.py
--rw-r--r--   0        0        0      677 2023-04-14 12:58:24.373132 cir4mics-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 cir4mics-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-12 14:30:48.348102 cir4mics-0.2.5/LICENSE
+-rw-r--r--   0        0        0       67 2023-04-12 14:59:50.266838 cir4mics-0.2.5/READMEpypi.md
+-rw-r--r--   0        0        0  1033056 2023-04-12 15:34:17.430636 cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/Dynamics-checkpoint.ipynb
+-rw-r--r--   0        0        0   110965 2023-04-12 14:30:48.372103 cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/Include_models-checkpoint.ipynb
+-rw-r--r--   0        0        0  1013844 2023-04-14 12:51:25.778620 cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/NPC_testlab-checkpoint.ipynb
+-rwxr-xr-x   0        0        0    21337 2023-04-12 14:30:48.352102 cir4mics-0.2.5/cir4mics/Analyse_deformed.py
+-rwxr-xr-x   0        0        0    34716 2023-04-14 13:51:25.155894 cir4mics-0.2.5/cir4mics/DeformNPC.py
+-rw-r--r--   0        0        0  1033056 2023-04-12 15:34:17.430636 cir4mics-0.2.5/cir4mics/Dynamics.ipynb
+-rw-r--r--   0        0        0   110965 2023-04-12 15:34:52.338891 cir4mics-0.2.5/cir4mics/Include_models.ipynb
+-rwxr-xr-x   0        0        0    46387 2023-04-14 13:51:25.159894 cir4mics-0.2.5/cir4mics/NPC_plotting.py
+-rw-r--r--   0        0        0  1013844 2023-04-14 12:51:25.778620 cir4mics-0.2.5/cir4mics/NPC_testlab.ipynb
+-rwxr-xr-x   0        0        0    87897 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/Nups_Info.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/__init__.py
+-rwxr-xr-x   0        0        0     4487 2023-04-14 13:51:25.159894 cir4mics-0.2.5/cir4mics/call_functions.py
+-rwxr-xr-x   0        0        0     1540 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/config.yaml
+-rw-r--r--   0        0        0    97163 2023-04-14 12:51:41.794714 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-14 12:51:41.794714 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 14:41:46.991998 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 14:41:46.991998 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 14:42:47.021021 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 14:42:47.021021 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 14:50:22.122689 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 14:50:22.122689 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97665 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0      845 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 15:34:52.562893 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 15:34:52.562893 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-12 14:53:41.671850 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-12 14:53:41.671850 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    97163 2023-04-14 12:35:49.509796 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0      773 2023-04-14 12:35:49.509796 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    13749 2023-04-14 12:48:50.885719 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0      703 2023-04-14 12:48:50.885719 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    13749 2023-04-14 12:50:03.310138 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0      703 2023-04-14 12:50:03.310138 cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt
+-rw-r--r--   0        0        0    18997 2023-04-14 12:51:41.826714 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0    19032 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-12 14:41:47.023999 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-12 14:42:47.045022 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-12 14:50:22.146689 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    18951 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-12 15:34:52.586893 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-12 14:53:41.703850 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    18997 2023-04-14 12:35:49.537796 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0     2857 2023-04-14 12:48:50.889720 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0     2857 2023-04-14 12:50:03.314138 cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-14 12:51:41.850714 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 14:41:47.043999 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 14:42:47.073022 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 14:50:22.166689 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    68911 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 15:34:52.614893 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-12 14:53:41.731850 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    68839 2023-04-14 12:35:49.561796 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0    11018 2023-04-14 12:48:50.889720 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0    11018 2023-04-14 12:50:03.314138 cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-14 12:51:41.866715 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0    34473 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-12 14:41:47.068000 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-12 14:42:47.093023 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-12 14:50:22.182689 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    34504 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-12 15:34:52.634894 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-12 14:53:41.751850 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv
+-rw-r--r--   0        0        0    34467 2023-04-14 12:35:49.585796 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv
+-rw-r--r--   0        0        0     5288 2023-04-14 12:48:50.889720 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0     5288 2023-04-14 12:50:03.314138 cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv
+-rw-r--r--   0        0        0     1622 2023-04-12 14:30:48.388103 cir4mics-0.2.5/cir4mics/dynamics.yaml
+-rwxr-xr-x   0        0        0    20327 2023-04-14 13:51:25.159894 cir4mics-0.2.5/cir4mics/exportCSV.py
+-rwxr-xr-x   0        0        0     3999 2023-04-12 14:30:48.392103 cir4mics-0.2.5/cir4mics/newModels/ModifyChimeraOutput.py
+-rwxr-xr-x   0        0        0     6190 2023-04-12 14:30:48.392103 cir4mics-0.2.5/cir4mics/newModels/parse_NPC_cifs.py
+-rwxr-xr-x   0        0        0     3901 2023-04-14 12:34:12.297447 cir4mics-0.2.5/cir4mics/npc.py
+-rw-r--r--   0        0        0      684 2023-04-12 14:30:48.392103 cir4mics-0.2.5/cir4mics/utility.py
+-rw-r--r--   0        0        0      677 2023-04-17 13:39:40.665124 cir4mics-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 cir4mics-0.2.5/PKG-INFO
```

### Comparing `cir4mics-0.2.4/LICENSE` & `cir4mics-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/Dynamics-checkpoint.ipynb` & `cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/Dynamics-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/Include_models-checkpoint.ipynb` & `cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/Include_models-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/.ipynb_checkpoints/NPC_testlab-checkpoint.ipynb` & `cir4mics-0.2.5/cir4mics/.ipynb_checkpoints/NPC_testlab-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/Analyse_deformed.py` & `cir4mics-0.2.5/cir4mics/Analyse_deformed.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/DeformNPC.py` & `cir4mics-0.2.5/cir4mics/DeformNPC.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/Dynamics.ipynb` & `cir4mics-0.2.5/cir4mics/Dynamics.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/Include_models.ipynb` & `cir4mics-0.2.5/cir4mics/Include_models.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/NPC_plotting.py` & `cir4mics-0.2.5/cir4mics/NPC_plotting.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/NPC_testlab.ipynb` & `cir4mics-0.2.5/cir4mics/NPC_testlab.ipynb`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/Nups_Info.py` & `cir4mics-0.2.5/cir4mics/Nups_Info.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/call_functions.py` & `cir4mics-0.2.5/cir4mics/call_functions.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/config.yaml` & `cir4mics-0.2.5/cir4mics/config.yaml`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt` & `cir4mics-0.2.5/cir4mics/data/Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023_metadata.txt`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_rings_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1a95ce8a-dac3-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_1ffa9444-cfd0-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_26c3b610-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_4a8a3114-d940-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_59ce772e-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_81c3f16e-cfcd-11ed-b54c-73ea736ccdcf_31-Mar-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_9182beae-d947-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_d0be8ff4-d941-11ed-8231-a36a306c38e7_12-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_C_x49_model_7r5J_deformmagxy_20_e2fab758-dac0-11ed-a38c-59574f773563_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_b4b934ee-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv` & `cir4mics-0.2.5/cir4mics/data/NPC_features_subcomplex_Ch_0_nup107_N_x7_model_5a9q_deformmagxy_20_dfe43dd0-dac2-11ed-840e-d43b042cf5ab_14-Apr-2023.csv`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/dynamics.yaml` & `cir4mics-0.2.5/cir4mics/dynamics.yaml`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/exportCSV.py` & `cir4mics-0.2.5/cir4mics/exportCSV.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/newModels/ModifyChimeraOutput.py` & `cir4mics-0.2.5/cir4mics/newModels/ModifyChimeraOutput.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/newModels/parse_NPC_cifs.py` & `cir4mics-0.2.5/cir4mics/newModels/parse_NPC_cifs.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/npc.py` & `cir4mics-0.2.5/cir4mics/npc.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/cir4mics/utility.py` & `cir4mics-0.2.5/cir4mics/utility.py`

 * *Files identical despite different names*

### Comparing `cir4mics-0.2.4/pyproject.toml` & `cir4mics-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cir4mics"
-version = "0.2.4"
+version = "0.2.5"
 description = "Simulating structurally variable NPCs or other ring-like structures for Microscopy"
 authors = ["MariaTheiss <theiss@ebi.ac.uk>"]
 license = "MIT"
 readme = "READMEpypi.md"
 packages = [{include = "cir4mics"}]
 
 [tool.poetry.dependencies]
@@ -12,19 +12,19 @@
 numpy = "^1.19.2, <= 1.23"
 circle-fit = "^0.2.0"
 pyyaml = "^6.0"
 scikit-learn = "^1.2.2"
 numba = "^0.56.4"
 seaborn = "^0.12.2"
 sympy = "^1.11.1"
-jupyterlab = "^3.6.1"
 ipympl = "^0.9.3"
 gemmi = "^0.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 spyder = "^5.4.2"
 black = "^23.3.0"
+jupyterlab = "^3.6.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cir4mics-0.2.4/PKG-INFO` & `cir4mics-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: cir4mics
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simulating structurally variable NPCs or other ring-like structures for Microscopy
 License: MIT
 Author: MariaTheiss
 Author-email: theiss@ebi.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: circle-fit (>=0.2.0,<0.3.0)
 Requires-Dist: gemmi (>=0.6.0,<0.7.0)
 Requires-Dist: ipympl (>=0.9.3,<0.10.0)
-Requires-Dist: jupyterlab (>=3.6.1,<4.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.19.2,<=1.23)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sympy (>=1.11.1,<2.0.0)
 Description-Content-Type: text/markdown
```

