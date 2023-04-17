# Comparing `tmp/miacag-0.0.80.tar.gz` & `tmp/miacag-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miacag-0.0.80.tar", last modified: Fri Feb 17 10:32:07 2023, max compression
+gzip compressed data, was "miacag-0.0.81.tar", last modified: Mon Apr 17 09:05:13 2023, max compression
```

## Comparing `miacag-0.0.80.tar` & `miacag-0.0.81.tar`

### file list

```diff
@@ -1,167 +1,175 @@
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.80/LICENSE
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.80/MANIFEST.in
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-02-17 10:32:07.638387 miacag-0.0.80/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.80/README.md
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/configs/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/configs/classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/configs/classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/classification/_3D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/configs/classification/_3D/lca_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/classification/_3D/lca_rca/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.80/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/configs/classification/_3D/stenosis_detection_rca/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.80/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/config.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/options.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/configs/update_configs.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/dataloader/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/dataloader/Classification/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/dataloader/Classification/_2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_2D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13280 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    71072 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag/dataloader/Classification/_3D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/Classification/_3D/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9581 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    23950 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.80/miacag/dataloader/Classification/_3D/dataset_mil.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/Classification/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8869 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/Classification/get_dataloader_classification.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/DistributedWeightedSampler.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/dataloader/Representation/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/Representation/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/Representation/get_dataloader_representation.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/dataloader/dataloader_base.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    24450 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/dataloader/dataloader_base_monai.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6113 2023-02-09 10:02:46.000000 miacag-0.0.80/miacag/dataloader/get_dataloader.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/metrics/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/metrics/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/metrics/cumulativeSumming.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/metrics/metrics.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12633 2023-02-10 10:26:52.000000 miacag-0.0.80/miacag/metrics/metrics_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/model_utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9548 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/model_utils/GradCam_model.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/model_utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    11960 2023-02-16 14:53:46.000000 miacag-0.0.80/miacag/model_utils/eval_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3993 2023-02-09 13:45:35.000000 miacag-0.0.80/miacag/model_utils/get_loss_func.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/model_utils/get_optimizer.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10574 2023-02-16 15:15:54.000000 miacag-0.0.80/miacag/model_utils/get_test_pipeline.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/model_utils/grad_cam_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    12228 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/model_utils/predict_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/model_utils/scheduler.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/model_utils/siam_loss.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6704 2023-02-16 14:52:08.000000 miacag-0.0.80/miacag/model_utils/train_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8655 2022-12-09 11:43:53.000000 miacag-0.0.80/miacag/models/BuildModel.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/backbone_encoders/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/backbone_encoders/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/backbone_encoders/tabular/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/backbone_encoders/tabular/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/backbone_encoders/tabular/base_encoders.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/cnns.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5766 2022-12-16 22:02:10.000000 miacag-0.0.80/miacag/models/get_encoder.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    11806 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/models/milmodel3d.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/mlps.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     8281 2023-02-10 08:07:17.000000 miacag-0.0.80/miacag/models/modules.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/models/torchhub/2D/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D/r50/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/models/torchhub/2D/r50/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D+T/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/2D+T/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D+T/mvit_base_16x4/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D+T/mvit_base_32x3/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D+T/r2plus1_18/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/models/torchhub/2D+T/x3d_s/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/2D+T/x3d_s/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/models/torchhub/__init__.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/plots/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/plots/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/plots/angle_plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/plots/getDataFromPdf.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/plots/plot_histogram.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    10561 2023-02-09 10:02:46.000000 miacag-0.0.80/miacag/plots/plot_roc_auc_all.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/plots/plot_scatter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.80/miacag/plots/plot_test.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    32951 2023-02-17 09:58:18.000000 miacag-0.0.80/miacag/plots/plotter.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.80/miacag/plots/query_plot_agg_max.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/postprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/postprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.80/miacag/postprocessing/aggregate_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/postprocessing/append_results.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/postprocessing/count_stenosis_pr_group.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/postprocessing/estimate_vessel_disease.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/predictor.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.634387 miacag-0.0.80/miacag/preprocessing/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/add_columns.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/copy_column.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/copy_table.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/datasetFingerpring.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/datasetFingerprint.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2022-12-16 18:58:24.000000 miacag-0.0.80/miacag/preprocessing/labels_map.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/pre_process.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/preprocessing/process_labels/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/process_labels/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.80/miacag/preprocessing/process_labels/process_dominance.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2022-11-21 09:32:51.000000 miacag-0.0.80/miacag/preprocessing/process_labels/process_total_occ.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     3631 2023-02-09 12:23:35.000000 miacag-0.0.80/miacag/preprocessing/split_train_val.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.80/miacag/preprocessing/transform_missing_floats.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.80/miacag/preprocessing/transform_stenosis.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4756 2023-01-10 15:49:41.000000 miacag-0.0.80/miacag/preprocessing/transform_thresholds.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.80/miacag/preprocessing/transform_total_occlusion.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/preprocessing/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/preprocessing/utils/check_experiments.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.80/miacag/scripts/aggregate_and_plot.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/angiography_classifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/angiography_classifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4725 2022-11-01 08:35:36.000000 miacag-0.0.80/miacag/scripts/angiography_classifier/predict_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    13153 2022-11-09 16:17:09.000000 miacag-0.0.80/miacag/scripts/angiography_classifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/angiography_classifier_stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2093 2022-11-09 16:17:20.000000 miacag-0.0.80/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/stenosis_identifier/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/stenosis_identifier/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    22787 2023-01-10 15:51:19.000000 miacag-0.0.80/miacag/scripts/stenosis_identifier/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/stenosis_identifier_mil/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/stenosis_identifier_mil/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    16366 2023-01-02 10:46:44.000000 miacag-0.0.80/miacag/scripts/stenosis_identifier_mil/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/stenosis_regression/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/stenosis_regression/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)    27197 2023-02-09 12:23:20.000000 miacag-0.0.80/miacag/scripts/stenosis_regression/submit_angio.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/scripts/stenosis_regression_full/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/scripts/stenosis_regression_full/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     7208 2022-11-09 16:15:58.000000 miacag-0.0.80/miacag/scripts/stenosis_regression_full/submit_angio.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2864 2022-11-01 13:34:24.000000 miacag-0.0.80/miacag/tester.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/tests/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/tests/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/tests/test_sql_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     4804 2023-02-10 08:51:02.000000 miacag-0.0.80/miacag/trainer.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.638387 miacag-0.0.80/miacag/utils/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/utils/__init__.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     2580 2023-02-10 10:44:32.000000 miacag-0.0.80/miacag/utils/common_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.80/miacag/utils/script_utils.py
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     6208 2022-12-20 14:45:41.000000 miacag-0.0.80/miacag/utils/sql_utils.py
-drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-02-17 10:32:07.630387 miacag-0.0.80/miacag.egg-info/
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-02-17 10:32:07.000000 miacag-0.0.80/miacag.egg-info/PKG-INFO
--rw-rw-r--   0 alatar    (1000) alatar    (1000)     5050 2023-02-17 10:32:07.000000 miacag-0.0.80/miacag.egg-info/SOURCES.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-02-17 10:32:07.000000 miacag-0.0.80/miacag.egg-info/dependency_links.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-02-17 10:32:07.000000 miacag-0.0.80/miacag.egg-info/top_level.txt
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.80/pyproject.toml
--rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-02-17 10:32:07.638387 miacag-0.0.80/setup.cfg
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    35149 2022-09-01 15:05:05.000000 miacag-0.0.81/LICENSE
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      129 2022-09-01 15:05:05.000000 miacag-0.0.81/MANIFEST.in
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-04-17 09:05:13.058542 miacag-0.0.81/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      111 2022-10-20 03:13:52.000000 miacag-0.0.81/README.md
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/_3D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3800 2022-09-20 09:25:18.000000 miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9668 2022-09-20 09:25:18.000000 miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      823 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/config.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3229 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/options.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      881 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/configs/update_configs.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/_2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12802 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13280 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    71072 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_2D/dataset_mil_2d.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Classification/_3D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2088 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_avi_video.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9581 2023-04-13 12:05:57.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    23950 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    72019 2022-11-04 15:43:12.000000 miacag-0.0.81/miacag/dataloader/Classification/_3D/dataset_mil.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Classification/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8869 2023-04-16 16:02:37.000000 miacag-0.0.81/miacag/dataloader/Classification/get_dataloader_classification.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2440 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/DistributedWeightedSampler.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag/dataloader/Representation/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Representation/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10772 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/Representation/get_dataloader_representation.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5611 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/dataloader/dataloader_base.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    24663 2023-04-17 08:45:34.000000 miacag-0.0.81/miacag/dataloader/dataloader_base_monai.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6113 2023-02-09 10:02:46.000000 miacag-0.0.81/miacag/dataloader/get_dataloader.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/metrics/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1180 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/cumulativeSumming.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4969 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/metrics/metrics.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12633 2023-02-10 10:26:52.000000 miacag-0.0.81/miacag/metrics/metrics_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/model_utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9549 2023-02-20 12:20:17.000000 miacag-0.0.81/miacag/model_utils/GradCam_model.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    11960 2023-02-16 14:53:46.000000 miacag-0.0.81/miacag/model_utils/eval_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3993 2023-02-09 13:45:35.000000 miacag-0.0.81/miacag/model_utils/get_loss_func.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/get_optimizer.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10574 2023-02-16 15:15:54.000000 miacag-0.0.81/miacag/model_utils/get_test_pipeline.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     9286 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/model_utils/grad_cam_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12228 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/model_utils/predict_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1576 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/scheduler.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      785 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/model_utils/siam_loss.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6704 2023-02-16 14:52:08.000000 miacag-0.0.81/miacag/model_utils/train_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8655 2022-12-09 11:43:53.000000 miacag-0.0.81/miacag/models/BuildModel.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/backbone_encoders/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/backbone_encoders/tabular/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/tabular/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      212 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/backbone_encoders/tabular/base_encoders.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      670 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/cnns.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    12742 2023-04-17 08:46:16.000000 miacag-0.0.81/miacag/models/get_encoder.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    11806 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/milmodel3d.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1769 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/mlps.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13303 2023-04-17 08:43:21.000000 miacag-0.0.81/miacag/models/modeling_finetune.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13780 2023-04-17 07:32:41.000000 miacag-0.0.81/miacag/models/modeling_pretrain.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     8388 2023-04-17 08:44:09.000000 miacag-0.0.81/miacag/models/modules.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13824 2023-04-16 15:10:08.000000 miacag-0.0.81/miacag/models/pretrained_vit.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/torchhub/2D/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/models/torchhub/2D/r50/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/models/torchhub/2D/r50/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_16x4/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_32x3/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/mvit_base_32x3/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/r2plus1_18/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/r2plus1_18/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.050542 miacag-0.0.81/miacag/models/torchhub/2D+T/x3d_s/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/2D+T/x3d_s/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/models/torchhub/__init__.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/plots/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1983 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/angle_plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      408 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/plots/getDataFromPdf.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      795 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/plots/plot_histogram.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    10561 2023-02-09 10:02:46.000000 miacag-0.0.81/miacag/plots/plot_roc_auc_all.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1277 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/plots/plot_scatter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1245 2023-01-27 08:30:25.000000 miacag-0.0.81/miacag/plots/plot_test.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    32951 2023-02-17 09:58:18.000000 miacag-0.0.81/miacag/plots/plotter.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4543 2023-01-27 08:26:48.000000 miacag-0.0.81/miacag/plots/query_plot_agg_max.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/postprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3593 2022-12-16 18:58:11.000000 miacag-0.0.81/miacag/postprocessing/aggregate_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1880 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/append_results.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4331 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/count_stenosis_pr_group.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5354 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/postprocessing/estimate_vessel_disease.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2527 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/predictor.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1319 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/add_columns.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1412 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/copy_column.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1321 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/copy_table.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/datasetFingerpring.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    21523 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/datasetFingerprint.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3232 2022-12-16 18:58:24.000000 miacag-0.0.81/miacag/preprocessing/labels_map.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7064 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/pre_process.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/process_labels/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/process_labels/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2999 2022-12-16 18:59:24.000000 miacag-0.0.81/miacag/preprocessing/process_labels/process_dominance.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    15711 2023-03-02 17:26:57.000000 miacag-0.0.81/miacag/preprocessing/process_labels/process_total_occ.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3631 2023-02-09 12:23:35.000000 miacag-0.0.81/miacag/preprocessing/split_train_val.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2344 2022-12-16 18:58:52.000000 miacag-0.0.81/miacag/preprocessing/transform_missing_floats.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2521 2022-12-16 18:58:58.000000 miacag-0.0.81/miacag/preprocessing/transform_stenosis.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4756 2023-01-10 15:49:41.000000 miacag-0.0.81/miacag/preprocessing/transform_thresholds.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2591 2022-12-16 18:59:17.000000 miacag-0.0.81/miacag/preprocessing/transform_total_occlusion.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/preprocessing/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1402 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/preprocessing/utils/check_experiments.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.054542 miacag-0.0.81/miacag/scripts/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13571 2023-01-10 16:02:18.000000 miacag-0.0.81/miacag/scripts/aggregate_and_plot.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/angiography_classifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4725 2022-11-01 08:35:36.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/predict_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    13153 2022-11-09 16:17:09.000000 miacag-0.0.81/miacag/scripts/angiography_classifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2093 2022-11-09 16:17:20.000000 miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     3675 2023-02-28 09:02:39.000000 miacag-0.0.81/miacag/scripts/compare_PCI_notPCI.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6510 2023-03-02 16:02:03.000000 miacag-0.0.81/miacag/scripts/predict_patologi_eyeball_vs_estimated.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_identifier/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    22787 2023-01-10 15:51:19.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    16366 2023-01-02 10:46:44.000000 miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_regression/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    27197 2023-04-16 15:00:01.000000 miacag-0.0.81/miacag/scripts/stenosis_regression/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression_full/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_full/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     7208 2022-11-09 16:15:58.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_full/submit_angio.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2023-04-16 14:46:27.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)    27334 2023-04-16 14:50:42.000000 miacag-0.0.81/miacag/scripts/stenosis_regression_with_pretraining/submit_angio.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2864 2022-11-01 13:34:24.000000 miacag-0.0.81/miacag/tester.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/tests/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/tests/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2109 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/tests/test_sql_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     4804 2023-02-10 08:51:02.000000 miacag-0.0.81/miacag/trainer.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.058542 miacag-0.0.81/miacag/utils/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        0 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/utils/__init__.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     2886 2023-02-23 08:19:40.000000 miacag-0.0.81/miacag/utils/common_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     1313 2022-09-01 15:05:05.000000 miacag-0.0.81/miacag/utils/script_utils.py
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     6205 2023-02-20 16:23:18.000000 miacag-0.0.81/miacag/utils/sql_utils.py
+drwxrwxr-x   0 alatar    (1000) alatar    (1000)        0 2023-04-17 09:05:13.046542 miacag-0.0.81/miacag.egg-info/
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      547 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/PKG-INFO
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)     5377 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        1 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)        7 2023-04-17 09:05:13.000000 miacag-0.0.81/miacag.egg-info/top_level.txt
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      106 2022-09-01 15:05:05.000000 miacag-0.0.81/pyproject.toml
+-rw-rw-r--   0 alatar    (1000) alatar    (1000)      524 2023-04-17 09:05:13.062542 miacag-0.0.81/setup.cfg
```

### Comparing `miacag-0.0.80/LICENSE` & `miacag-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/PKG-INFO` & `miacag-0.0.81/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.80
+Version: 0.0.81
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.80/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml` & `miacag-0.0.81/miacag/configs/classification/_3D/lca_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml` & `miacag-0.0.81/miacag/configs/classification/_3D/stenosis_detection_rca/classification_config_angio.yaml`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/configs/config.py` & `miacag-0.0.81/miacag/configs/config.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/configs/options.py` & `miacag-0.0.81/miacag/configs/options.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/configs/update_configs.py` & `miacag-0.0.81/miacag/configs/update_configs.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py` & `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py` & `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataloader_monai_classification_2D_mil.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_2D/dataset_mil_2d.py` & `miacag-0.0.81/miacag/dataloader/Classification/_2D/dataset_mil_2d.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_avi_video.py` & `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_avi_video.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py` & `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py` & `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataloader_monai_classification_3D_mil.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/_3D/dataset_mil.py` & `miacag-0.0.81/miacag/dataloader/Classification/_3D/dataset_mil.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Classification/get_dataloader_classification.py` & `miacag-0.0.81/miacag/dataloader/Classification/get_dataloader_classification.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/DistributedWeightedSampler.py` & `miacag-0.0.81/miacag/dataloader/DistributedWeightedSampler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/Representation/get_dataloader_representation.py` & `miacag-0.0.81/miacag/dataloader/Representation/get_dataloader_representation.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/dataloader_base.py` & `miacag-0.0.81/miacag/dataloader/dataloader_base.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/dataloader/dataloader_base_monai.py` & `miacag-0.0.81/miacag/dataloader/dataloader_base_monai.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,20 @@
                         padding_mode="zeros")
         else:
             rotate = Identityd(keys=self.features)
         return rotate
 
     def maybeNormalize(self):
         if self.config['model']['backbone'] in [
-            'x3d_s', 'slowfast8x8', "mvit_base_16x4", 'mvit_base_32x3', 'debug_3d']:
+            'x3d_s', 'slowfast8x8', "mvit_base_16x4", 'mvit_base_32x3', 'debug_3d',
+            "pretrain_videomae_base_patch16_224",
+            'pretrain_videomae_small_patch16_224',
+            "vit_base_patch16_224", 
+            "vit_large_patch16_224", 
+            "vit_small_patch16_224"]:
             normalize = NormalizeIntensityd(
                 keys=self.features,
                 subtrahend=(0.45, 0.45, 0.45),#(0.43216, 0.394666, 0.37645),
                 divisor=(0.225, 0.225, 0.225),#(0.22803, 0.22145, 0.216989),
                 channel_wise=True)
         elif self.config['model']['backbone'] == 'r2plus1_18':
             normalize = NormalizeIntensityd(
```

### Comparing `miacag-0.0.80/miacag/dataloader/get_dataloader.py` & `miacag-0.0.81/miacag/dataloader/get_dataloader.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/metrics/cumulativeSumming.py` & `miacag-0.0.81/miacag/metrics/cumulativeSumming.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/metrics/metrics.py` & `miacag-0.0.81/miacag/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/metrics/metrics_utils.py` & `miacag-0.0.81/miacag/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/GradCam_model.py` & `miacag-0.0.81/miacag/model_utils/GradCam_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 import torch
 from typing import Callable, List, Tuple
-import cv2
+#import cv2
 
 
 def scale_cam_image(cam, target_size=None):
     result = []
     for img in cam:
         img = img - np.min(img)
         img = img / (1e-7 + np.max(img))
```

### Comparing `miacag-0.0.80/miacag/model_utils/eval_utils.py` & `miacag-0.0.81/miacag/model_utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/get_loss_func.py` & `miacag-0.0.81/miacag/model_utils/get_loss_func.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/get_optimizer.py` & `miacag-0.0.81/miacag/model_utils/get_optimizer.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/get_test_pipeline.py` & `miacag-0.0.81/miacag/model_utils/get_test_pipeline.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/grad_cam_utils.py` & `miacag-0.0.81/miacag/model_utils/grad_cam_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/predict_utils.py` & `miacag-0.0.81/miacag/model_utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/scheduler.py` & `miacag-0.0.81/miacag/model_utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/siam_loss.py` & `miacag-0.0.81/miacag/model_utils/siam_loss.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/model_utils/train_utils.py` & `miacag-0.0.81/miacag/model_utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/models/BuildModel.py` & `miacag-0.0.81/miacag/models/BuildModel.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/models/cnns.py` & `miacag-0.0.81/miacag/models/cnns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/models/milmodel3d.py` & `miacag-0.0.81/miacag/models/milmodel3d.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/models/mlps.py` & `miacag-0.0.81/miacag/models/mlps.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/models/modules.py` & `miacag-0.0.81/miacag/models/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,17 @@
                 raise ValueError('loss not implemented')
         self.dimension = config['model']['dimension']
 
     def forward(self, x):
         x = maybePermuteInput(x, self.config)
         p = self.encoder(x)
         if self.dimension in ['3D', '2D+T']:
-            if self.config['model']['backbone'] not in ["mvit_base_16x4", "mvit_base_32x3"]:
+            if self.config['model']['backbone'] not in [
+                "mvit_base_16x4", "mvit_base_32x3", "vit_base_patch16_224",
+                "vit_small_patch16_224", "vit_large_patch16_224"]:
                 p = p.mean(dim=(-3, -2, -1))
             else:
                 pass
         elif self.dimension == 'tabular':
             p = p
         else:
             p = p.mean(dim=(-2, -1))
```

### Comparing `miacag-0.0.80/miacag/plots/angle_plotter.py` & `miacag-0.0.81/miacag/plots/angle_plotter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/plot_histogram.py` & `miacag-0.0.81/miacag/plots/plot_histogram.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/plot_roc_auc_all.py` & `miacag-0.0.81/miacag/plots/plot_roc_auc_all.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/plot_scatter.py` & `miacag-0.0.81/miacag/plots/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/plot_test.py` & `miacag-0.0.81/miacag/plots/plot_test.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/plotter.py` & `miacag-0.0.81/miacag/plots/plotter.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/plots/query_plot_agg_max.py` & `miacag-0.0.81/miacag/plots/query_plot_agg_max.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/postprocessing/aggregate_pr_group.py` & `miacag-0.0.81/miacag/postprocessing/aggregate_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/postprocessing/append_results.py` & `miacag-0.0.81/miacag/postprocessing/append_results.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/postprocessing/count_stenosis_pr_group.py` & `miacag-0.0.81/miacag/postprocessing/count_stenosis_pr_group.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/postprocessing/estimate_vessel_disease.py` & `miacag-0.0.81/miacag/postprocessing/estimate_vessel_disease.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/predictor.py` & `miacag-0.0.81/miacag/predictor.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/add_columns.py` & `miacag-0.0.81/miacag/preprocessing/add_columns.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/copy_column.py` & `miacag-0.0.81/miacag/preprocessing/copy_column.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/copy_table.py` & `miacag-0.0.81/miacag/preprocessing/copy_table.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/datasetFingerprint.py` & `miacag-0.0.81/miacag/preprocessing/datasetFingerprint.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/labels_map.py` & `miacag-0.0.81/miacag/preprocessing/labels_map.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/pre_process.py` & `miacag-0.0.81/miacag/preprocessing/pre_process.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/process_labels/process_dominance.py` & `miacag-0.0.81/miacag/preprocessing/process_labels/process_dominance.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/process_labels/process_total_occ.py` & `miacag-0.0.81/miacag/preprocessing/process_labels/process_total_occ.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/split_train_val.py` & `miacag-0.0.81/miacag/preprocessing/split_train_val.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/transform_missing_floats.py` & `miacag-0.0.81/miacag/preprocessing/transform_missing_floats.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/transform_stenosis.py` & `miacag-0.0.81/miacag/preprocessing/transform_stenosis.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/transform_thresholds.py` & `miacag-0.0.81/miacag/preprocessing/transform_thresholds.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/transform_total_occlusion.py` & `miacag-0.0.81/miacag/preprocessing/transform_total_occlusion.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/preprocessing/utils/check_experiments.py` & `miacag-0.0.81/miacag/preprocessing/utils/check_experiments.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/aggregate_and_plot.py` & `miacag-0.0.81/miacag/scripts/aggregate_and_plot.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/angiography_classifier/predict_angio.py` & `miacag-0.0.81/miacag/scripts/angiography_classifier/predict_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/angiography_classifier/submit_angio.py` & `miacag-0.0.81/miacag/scripts/angiography_classifier/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py` & `miacag-0.0.81/miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/stenosis_identifier/submit_angio.py` & `miacag-0.0.81/miacag/scripts/stenosis_identifier/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/stenosis_identifier_mil/submit_angio.py` & `miacag-0.0.81/miacag/scripts/stenosis_identifier_mil/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/stenosis_regression/submit_angio.py` & `miacag-0.0.81/miacag/scripts/stenosis_regression/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/scripts/stenosis_regression_full/submit_angio.py` & `miacag-0.0.81/miacag/scripts/stenosis_regression_full/submit_angio.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/tester.py` & `miacag-0.0.81/miacag/tester.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/tests/test_sql_utils.py` & `miacag-0.0.81/miacag/tests/test_sql_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/trainer.py` & `miacag-0.0.81/miacag/trainer.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/utils/common_utils.py` & `miacag-0.0.81/miacag/utils/common_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,27 @@
     loss_tot = loss_tot.to(device)
     loss_tot = loss_tot.requires_grad_()
     for count_idx, loss_name in enumerate(config['loss']['groups_names']):
         labels = stack_labels(data, config, loss_name)
         loss = get_loss(
             config, outputs[count_idx],
             labels, criterion[count_idx], loss_name)
+        #print('done')
         if torch.isnan(loss) == torch.tensor(True, device=device):
-            raise ValueError('the loss is nan!')
+            #raise ValueError('the loss is nan!')
+            # # ugly hack
+            if count_idx == 0:
+                t = torch.tensor([1]).float()
+                
+              #  t.requires_grad_()
+                losses.append(t)
+            else:
+                losses.append(losses[-1])
+            loss_tot = loss_tot
+
 
         else:
             # scale loss by weights for given task
             loss = loss * config['groups_weights'][count_idx]
             losses.append(loss)
             loss_tot = loss_tot + loss
     losses = [loss_indi.item() for loss_indi in losses]
```

### Comparing `miacag-0.0.80/miacag/utils/script_utils.py` & `miacag-0.0.81/miacag/utils/script_utils.py`

 * *Files identical despite different names*

### Comparing `miacag-0.0.80/miacag/utils/sql_utils.py` & `miacag-0.0.81/miacag/utils/sql_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     FROM (VALUES %s) AS e({cols})
     WHERE e.rowid = t.rowid;""".format(
         schema_name=sql_config['schema_name'],
         table_name=sql_config['table_name'],
         cols=', '.join(cols+['rowid']),
         cols_to_set=string)
     cur = conn.cursor()
-    n = 10000   
+    n = 50000
     print('len(values): ', len(values))
     with tqdm(total=len(values)) as pbar:
         for i in range(0, len(values), n):
             psycopg2.extras.execute_values(
                 cur, update_query, values[i:i + n], template=None, page_size=n
                 )
             conn.commit()
```

### Comparing `miacag-0.0.80/miacag.egg-info/PKG-INFO` & `miacag-0.0.81/miacag.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miacag
-Version: 0.0.80
+Version: 0.0.81
 Summary: miacag angio DL tools
 Home-page: https://github.com/ChristianEschen/miacag
 Author: Christian Eschen
 Author-email: christian_eschen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miacag-0.0.80/miacag.egg-info/SOURCES.txt` & `miacag-0.0.81/miacag.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,18 @@
 miacag/model_utils/train_utils.py
 miacag/models/BuildModel.py
 miacag/models/__init__.py
 miacag/models/cnns.py
 miacag/models/get_encoder.py
 miacag/models/milmodel3d.py
 miacag/models/mlps.py
+miacag/models/modeling_finetune.py
+miacag/models/modeling_pretrain.py
 miacag/models/modules.py
+miacag/models/pretrained_vit.py
 miacag/models/backbone_encoders/__init__.py
 miacag/models/backbone_encoders/tabular/__init__.py
 miacag/models/backbone_encoders/tabular/base_encoders.py
 miacag/models/torchhub/__init__.py
 miacag/models/torchhub/2D/__init__.py
 miacag/models/torchhub/2D+T/__init__.py
 miacag/models/torchhub/2D+T/mvit_base_16x4/__init__.py
@@ -101,26 +104,30 @@
 miacag/preprocessing/process_labels/__init__.py
 miacag/preprocessing/process_labels/process_dominance.py
 miacag/preprocessing/process_labels/process_total_occ.py
 miacag/preprocessing/utils/__init__.py
 miacag/preprocessing/utils/check_experiments.py
 miacag/scripts/__init__.py
 miacag/scripts/aggregate_and_plot.py
+miacag/scripts/compare_PCI_notPCI.py
+miacag/scripts/predict_patologi_eyeball_vs_estimated.py
 miacag/scripts/angiography_classifier/__init__.py
 miacag/scripts/angiography_classifier/predict_angio.py
 miacag/scripts/angiography_classifier/submit_angio.py
 miacag/scripts/angiography_classifier_stenosis_identifier/__init__.py
 miacag/scripts/angiography_classifier_stenosis_identifier/submit_angio.py
 miacag/scripts/stenosis_identifier/__init__.py
 miacag/scripts/stenosis_identifier/submit_angio.py
 miacag/scripts/stenosis_identifier_mil/__init__.py
 miacag/scripts/stenosis_identifier_mil/submit_angio.py
 miacag/scripts/stenosis_regression/__init__.py
 miacag/scripts/stenosis_regression/submit_angio.py
 miacag/scripts/stenosis_regression_full/__init__.py
 miacag/scripts/stenosis_regression_full/submit_angio.py
+miacag/scripts/stenosis_regression_with_pretraining/__init__.py
+miacag/scripts/stenosis_regression_with_pretraining/submit_angio.py
 miacag/tests/__init__.py
 miacag/tests/test_sql_utils.py
 miacag/utils/__init__.py
 miacag/utils/common_utils.py
 miacag/utils/script_utils.py
 miacag/utils/sql_utils.py
```

### Comparing `miacag-0.0.80/setup.cfg` & `miacag-0.0.81/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = miacag
-version = 0.0.80
+version = 0.0.81
 author = Christian Eschen
 author_email = christian_eschen@hotmail.com
 description = miacag angio DL tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ChristianEschen/miacag
 classifiers =
```

