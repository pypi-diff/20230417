# Comparing `tmp/Simba-UW-tf-dev-1.56.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.56.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.3.tar", last modified: Sat Apr 15 19:01:08 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.56.4.tar", last modified: Mon Apr 17 19:27:42 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.56.3.tar` & `Simba-UW-tf-dev-1.56.4.tar`

### file list

```diff
@@ -1,389 +1,397 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.3/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-03-21 14:26:03.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/misc.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7227 2023-03-21 11:41:26.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/data_extractors.py
--rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/dbcv.py
--rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/umap_embedder.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/
--rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/vtk_embeddings.py
--rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/ui_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6642 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19445 2023-04-14 17:48:54.000000 Simba-UW-tf-dev-1.56.3/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-13 14:09:44.000000 Simba-UW-tf-dev-1.56.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21399 2023-04-11 16:58:31.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-11 20:41:01.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36715 2023-04-14 16:41:10.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.3/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.3/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34563 2023-04-10 20:12:42.000000 Simba-UW-tf-dev-1.56.3/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.3/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.3/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.3/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14398 2023-04-10 19:08:11.000000 Simba-UW-tf-dev-1.56.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.3/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    46716 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.3/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.3/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.3/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     3798 2023-04-12 13:45:31.000000 Simba-UW-tf-dev-1.56.3/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.3/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.3/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.3/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.3/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.3/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.3/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.3/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56820 2023-04-15 18:59:15.000000 Simba-UW-tf-dev-1.56.3/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.3/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.3/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.3/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.3/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.3/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-13 18:18:32.000000 Simba-UW-tf-dev-1.56.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.3/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.3/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.3/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.3/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.3/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.3/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.3/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.3/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13203 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      638 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-15 19:01:07.000000 Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.3/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1895 2023-04-15 19:00:54.000000 Simba-UW-tf-dev-1.56.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-15 19:01:08.000000 Simba-UW-tf-dev-1.56.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.56.4/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.56.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    10851 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5554 2023-04-16 21:21:48.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/misc.py
+-rw-r--r--   0 simon      (501) staff       (20)     1727 2023-04-17 15:19:16.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7227 2023-04-16 17:14:22.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4061 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/data_extractors.py
+-rw-r--r--   0 simon      (501) staff       (20)    10405 2023-04-17 17:36:52.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/umap_embedder_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    11192 2023-03-21 20:14:50.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/dbcv.py
+-rw-r--r--   0 simon      (501) staff       (20)    11456 2023-03-21 18:17:26.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7526 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     6998 2023-04-17 19:17:34.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/grd_search_img_visualizer_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     6885 2023-04-16 21:07:58.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/dataset_creator_2.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/visualization_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     2019 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/visualization_tools/vtk_embeddings.py
+-rw-r--r--   0 simon      (501) staff       (20)      150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/ui_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)     8392 2023-04-17 17:37:22.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/hdbscan_clusterer_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    49992 2023-03-22 15:08:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-03-21 15:42:27.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6702 2023-04-17 16:45:09.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3789 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5630 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19468 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.4/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-17 14:05:31.000000 Simba-UW-tf-dev-1.56.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-17 19:14:16.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.56.4/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.4/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.56.4/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    41904 2023-04-14 10:42:10.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-04-07 13:58:40.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4865 2023-04-17 19:13:41.000000 Simba-UW-tf-dev-1.56.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.56.4/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.4/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12866 2023-04-10 14:41:24.000000 Simba-UW-tf-dev-1.56.4/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.56.4/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.4/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.56.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.4/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.56.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.56.4/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.4/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    46716 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.56.4/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.56.4/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.56.4/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.4/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.56.4/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.56.4/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.56.4/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9874 2023-04-14 13:15:44.000000 Simba-UW-tf-dev-1.56.4/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.56.4/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.56.4/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.56.4/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14661 2023-04-10 20:11:46.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.56.4/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56820 2023-04-15 18:59:15.000000 Simba-UW-tf-dev-1.56.4/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.56.4/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.56.4/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.56.4/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.56.4/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    17627 2023-04-10 20:01:08.000000 Simba-UW-tf-dev-1.56.4/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64354 2023-04-13 18:53:02.000000 Simba-UW-tf-dev-1.56.4/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-17 19:14:16.000000 Simba-UW-tf-dev-1.56.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.56.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.56.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.56.4/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     8101 2023-04-15 18:49:21.000000 Simba-UW-tf-dev-1.56.4/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.56.4/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20742 2023-04-10 19:52:46.000000 Simba-UW-tf-dev-1.56.4/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24896 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10882 2023-04-09 17:57:09.000000 Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.56.4/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.56.4/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.56.4/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.56.4/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13557 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      638 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.56.4/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.56.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.56.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1895 2023-04-17 19:27:40.000000 Simba-UW-tf-dev-1.56.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-17 19:27:42.000000 Simba-UW-tf-dev-1.56.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.56.3/PKG-INFO` & `Simba-UW-tf-dev-1.56.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.3
+Version: 1.56.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/video_processing.py` & `Simba-UW-tf-dev-1.56.4/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/misc.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,50 +6,30 @@
                                    QuantileTransformer)
 from sklearn.feature_selection import VarianceThreshold
 from simba.feature_extractors.unit_tests import read_video_info
 from simba.enums import Options
 from simba.misc_tools import detect_bouts
 from joblib import Parallel, delayed
 import numpy as np
+from simba.utils.errors import DirectoryNotEmptyError
 from joblib.externals.loky import get_reusable_executor
 
-
-def read_pickle(data_path: str) -> dict:
-    if os.path.isdir(data_path):
-        data = {}
-        files_found = glob.glob(data_path + '/*.pickle')
-        if len(files_found) == 0:
-            print(f'SIMBA ERROR: Zero pickle files found in {data_path}.')
-            raise ValueError
-        for file_cnt, file_path in enumerate(files_found):
-            with open(file_path, 'rb') as f:
-                data[file_cnt] = pickle.load(f)
-    if os.path.isfile(data_path):
-        with open(data_path, 'rb') as f:
-            data = pickle.load(f)
-
-    return data
-
-
 def write_pickle(data: dict, save_path: str):
     with open(save_path, 'wb') as f:
         pickle.dump(data, f, protocol=pickle.HIGHEST_PROTOCOL)
 
 
 def check_that_directory_is_empty(directory: str) -> None:
     try:
         all_files_in_folder = [f for f in next(os.walk(directory))[2] if not f[0] == '.']
     except StopIteration:
         return 0
     else:
         if len(all_files_in_folder) > 0:
-            print('''ssss''')
-            print(f'SIMBA ERROR: The {directory} is not empty and contains {str(len(all_files_in_folder))} files. Use a directory that is empty.')
-            raise ValueError()
-
+            raise DirectoryNotEmptyError(msg=f'The {directory} is not empty and contains {str(len(all_files_in_folder))} files. Use a directory that is empty.')
 
 def get_cluster_cnt(data: np.array,
                     clusterer_name: str,
                     minimum_clusters: int = 1) -> int:
     cnt = np.unique(data).shape[0]
     if cnt < minimum_clusters:
         print(f'SIMBA ERROR: Clustrer {clusterer_name} has {str(cnt)} clusters, but {str(minimum_clusters)} clusters is required for the operation.')
@@ -60,24 +40,15 @@
 def check_directory_exists(directory: str) -> None:
     if not os.path.isdir(directory):
         print(f'SIMBA ERROR: {directory} is not a valid directory.')
         raise NotADirectoryError
     else:
         pass
 
-def define_scaler(scaler_name: str):
-    if scaler_name not in Options.SCALER_NAMES.value:
-        print('SIMBA ERROR: {} is not a valid scaler option (VALID OPTIONS: {}'.format(scaler_name, Options.SCALER_NAMES.value))
-        raise ValueError()
-    if scaler_name == 'MIN-MAX':
-        return MinMaxScaler()
-    elif scaler_name == 'STANDARD':
-        return StandardScaler()
-    elif scaler_name == 'QUANTILE':
-        return QuantileTransformer()
+
 
 def find_low_variance_fields(data: pd.DataFrame, variance: float):
     feature_selector = VarianceThreshold(threshold=round((variance / 100), 2))
     feature_selector.fit(data)
     return [c for c in data.columns if c not in data.columns[feature_selector.get_support()]]
 
 
@@ -105,16 +76,16 @@
 
 def bout_aggregator(data: pd.DataFrame,
                     clfs: list,
                     feature_names: list,
                     aggregator: str,
                     min_bout_length: int,
                     video_info: pd.DataFrame):
-    print('Calculating bout aggregate statistics...')
 
+    print('Calculating bout aggregate statistics...')
     def bout_aggregator_mp(frms, data, clf_name):
         bout_df = data.iloc[frms[0]: frms[1]+1]
         bout_video, start_frm, end_frm = bout_df['VIDEO'].values[0], bout_df['FRAME'].values[0], bout_df['FRAME'].values[-1]
         if aggregator == 'MEAN':
             agg_df = pd.DataFrame(bout_df[feature_names].mean()).T
             agg_df['PROBABILITY'] = bout_df[f'Probability_{clf_name}'].mean()
         elif aggregator == 'MEDIAN':
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/data_extractors.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/data_extractors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/dbcv.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/dbcv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualizers.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/visualization_tools/vtk_embeddings.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/visualization_tools/vtk_embeddings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,25 @@
 
 class HDBSCANClusterer(object):
     def __init__(self,
                  data_path: str,
                  save_dir: str):
 
         self.datetime, self.save_dir, self.data_path = datetime.now().strftime('%Y%m%d%H%M%S'), save_dir, data_path
-        check_directory_exists(directory=data_path)
+        if os.path.isdir(data_path):
+            check_directory_exists(directory=data_path)
+            self.data_paths = glob.glob(data_path + '/*.pickle')
+            check_if_filepath_list_is_empty(filepaths=self.data_paths, error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
+        else:
+        os.path.isdir(data_path):
+
+
         check_directory_exists(directory=save_dir)
         check_that_directory_is_empty(directory=save_dir)
-        self.data_paths = glob.glob(data_path + '/*.pickle')
-        check_if_filepath_list_is_empty(filepaths=self.data_paths,
-                                        error_msg=f'SIMBA ERROR: No pickle files in {data_path}')
+
         model_names_dir = os.path.join(os.path.dirname(simba.__file__), Paths.UNSUPERVISED_MODEL_NAMES.value)
         self.model_names = list(pd.read_parquet(model_names_dir)['NAMES'])
         self.timer = SimbaTimer()
         self.timer.start_timer()
 
     def fit(self,
             hyper_parameters: dict):
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.56.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/enums.py` & `Simba-UW-tf-dev-1.56.4/simba/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     MP4_CODEC = 'mp4v'
     AVI_CODEC = 'XVID'
     LABELFRAME_HEADER_FORMAT = ('Helvetica', 12, 'bold')
     LABELFRAME_HEADER_CLICKABLE_FORMAT = ('Helvetica', 12, 'bold', 'underline')
     LABELFRAME_HEADER_CLICKABLE_COLOR = f'#{5:02x}{99:02x}{193:02x}'
     CSV = 'csv'
     PARQUET = 'parquet'
+    PICKLE = 'parquet'
     PERIMETER = 'perimeter'
     AREA = 'area'
     H5 = 'h5'
     ROOT_WINDOW_SIZE = "750x750"
     FONT = cv2.FONT_HERSHEY_TRIPLEX
     TKINTER_FONT = ("Rockwell", 11)
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.56.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -329,24 +329,24 @@
 00001480: 0809 5f10 187b 7b33 3934 2c20 3138 317d  .._..{{394, 181}
 00001490: 2c20 7b37 3730 2c20 3433 367d 7d09 0817  , {770, 436}}...
 000014a0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 000014b0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 000014c0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 000014d0: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
 000014e0: 7600 6900 7300 6500 646c 6731 5363 6f6d  v.i.s.e.dlg1Scom
-000014f0: 7000 0000 0000 0575 f500 0000 0c00 7500  p......u......u.
+000014f0: 7000 0000 0000 05bb b700 0000 0c00 7500  p.............u.
 00001500: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
 00001510: 7300 6500 646d 6f44 4462 6c6f 6200 0000  s.e.dmoDDblob...
-00001520: 0839 4439 c4a8 e5c4 4100 0000 0c00 7500  .9D9....A.....u.
+00001520: 08ff 2f6f 7569 f6c4 4100 0000 0c00 7500  ../oui..A.....u.
 00001530: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
 00001540: 7300 6500 646d 6f64 4462 6c6f 6200 0000  s.e.dmodDblob...
-00001550: 0839 4439 c4a8 e5c4 4100 0000 0c00 7500  .9D9....A.....u.
+00001550: 08ff 2f6f 7569 f6c4 4100 0000 0c00 7500  ../oui..A.....u.
 00001560: 6e00 7300 7500 7000 6500 7200 7600 6900  n.s.u.p.e.r.v.i.
 00001570: 7300 6500 6470 6831 5363 6f6d 7000 0000  s.e.dph1Scomp...
-00001580: 0000 0690 0000 0000 0c00 7500 6e00 7300  ..........u.n.s.
+00001580: 0000 0700 0000 0000 0c00 7500 6e00 7300  ..........u.n.s.
 00001590: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
 000015a0: 6476 5372 6e6c 6f6e 6700 0000 0100 0000  dvSrnlong.......
 000015b0: 0500 7500 7400 6900 6c00 7362 7773 7062  ..u.t.i.l.sbwspb
 000015c0: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
 000015d0: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
 000015e0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
 000015f0: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
@@ -358,15 +358,15 @@
 00001650: 3230 7d2c 207b 3737 302c 2034 3336 7d7d  20}, {770, 436}}
 00001660: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
 00001670: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 00001680: 0000 0000 0000 0000 0000 0000 0000 009a  ................
 00001690: 0000 0005 0075 0074 0069 006c 0073 6473  .....u.t.i.l.sds
 000016a0: 636c 626f 6f6c 0000 0000 0500 7500 7400  clbool......u.t.
 000016b0: 6900 6c00 736c 6731 5363 6f6d 7000 0000  i.l.slg1Scomp...
-000016c0: 0000 0113 9c00 0000 0500 7500 7400 6900  ..........u.t.i.
+000016c0: 0000 011c 5a00 0000 0500 7500 7400 6900  ....Z.....u.t.i.
 000016d0: 6c00 736c 7376 4362 6c6f 6200 0002 9762  l.slsvCblob....b
 000016e0: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
 000016f0: 090a 0b19 494a 0a4c 5f10 1276 6965 774f  ....IJ.L_..viewO
 00001700: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00001710: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00001720: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 00001730: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
@@ -442,15 +442,15 @@
 00001b90: 0147 0148 014a 014b 0154 0156 0157 0159  .G.H.J.K.T.V.W.Y
 00001ba0: 015a 0163 0165 0166 0168 0169 0172 0174  .Z.c.e.f.h.i.r.t
 00001bb0: 0175 0177 0178 0181 0183 0184 0187 0188  .u.w.x..........
 00001bc0: 0191 0192 0193 0194 019d 01a2 01a3 0000  ................
 00001bd0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001be0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00001bf0: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001c00: 626c 6f62 0000 0008 2102 3a7c 75f3 c441  blob....!.:|u..A
+00001c00: 626c 6f62 0000 0008 8551 cb34 d5f4 c441  blob.....Q.4...A
 00001c10: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
 00001c20: 6444 626c 6f62 0000 0008 b191 97e3 46f2  dDblob........F.
 00001c30: c441 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
 00001c40: 7068 3153 636f 6d70 0000 0000 0001 6000  ph1Scomp......`.
 00001c50: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
 00001c60: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -509,23 +509,23 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0041 45b4 0000 000b 005f 005f 0070  ...AE......_._.p
+00002030: 0000 0042 095a 0000 000b 005f 005f 0070  ...B.Z....._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 4f80 e6bf  moDDblob....O...
-00002060: 86f3 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 08d6 dc03  moDDblob........
+00002060: dff4 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00002080: 6444 626c 6f62 0000 0008 5667 2fa4 52f2  dDblob....Vg/.R.
+00002080: 6444 626c 6f62 0000 0008 08d6 dc03 dff4  dDblob..........
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000020b0: 636f 6d70 0000 0000 004f 1000 0000 0006  comp.....O......
+000020b0: 636f 6d70 0000 0000 004f f000 0000 0006  comp.....O......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
 000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
@@ -533,15 +533,15 @@
 00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
 00002150: 7208 0809 0809 5f10 177b 7b33 342c 2039  r....._..{{34, 9
 00002160: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
 00002170: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
 00002180: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 00002190: 0000 0000 0000 0000 0000 0000 0000 0099  ................
 000021a0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021b0: 6c67 3153 636f 6d70 0000 0000 007d c8d6  lg1Scomp.....}..
+000021b0: 6c67 3153 636f 6d70 0000 0000 007d d138  lg1Scomp.....}.8
 000021c0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
 000021d0: 6c73 7643 626c 6f62 0000 02b0 6270 6c69  lsvCblob....bpli
 000021e0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 000021f0: 0c0d 1848 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
 00002200: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 00002210: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 00002220: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
@@ -628,15 +628,15 @@
 00002730: 0000 0000 0000 0000 0000 0001 dd00 0000  ................
 00002740: 0600 6100 7300 7300 6500 7400 736d 6f44  ..a.s.s.e.t.smoD
 00002750: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
 00002760: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
 00002770: 736d 6f64 4462 6c6f 6200 0000 08cf 958c  smodDblob.......
 00002780: e8d0 e1c4 4100 0000 0600 6100 7300 7300  ....A.....a.s.s.
 00002790: 6500 7400 7370 6831 5363 6f6d 7000 0000  e.t.sph1Scomp...
-000027a0: 0000 8180 0000 0000 0600 6100 7300 7300  ..........a.s.s.
+000027a0: 0000 8190 0000 0000 0600 6100 7300 7300  ..........a.s.s.
 000027b0: 6500 7400 7376 5372 6e6c 6f6e 6700 0000  e.t.svSrnlong...
 000027c0: 0100 0000 1400 6200 6100 7400 6300 6800  ......b.a.t.c.h.
 000027d0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000027e0: 5f00 7600 6900 6400 6500 6f00 7362 7773  _.v.i.d.e.o.sbws
 000027f0: 7062 6c6f 6200 0000 ca62 706c 6973 7430  pblob....bplist0
 00002800: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
 00002810: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
@@ -946,98 +946,98 @@
 00003b10: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
 00003b20: 0000 0290 0000 0000 0f00 6300 7500 6500  ..........c.u.e.
 00003b30: 5f00 6c00 6900 6700 6800 7400 5f00 7400  _.l.i.g.h.t._.t.
 00003b40: 6f00 6f00 6c00 7376 5372 6e6c 6f6e 6700  o.o.l.svSrnlong.
 00003b50: 0000 0100 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
 00003b60: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00003b70: 6100 6300 7400 6f00 7200 7362 7773 7062  a.c.t.o.r.sbwspb
-00003b80: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
+00003b80: 6c6f 6200 0000 c862 706c 6973 7430 30d7  lob....bplist00.
 00003b90: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
 00003ba0: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
 00003bb0: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
 00003bc0: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
 00003bd0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
 00003be0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
 00003bf0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00003c00: 0808 0908 095f 1019 7b7b 3932 302c 2031  ....._..{{920, 1
-00003c10: 3531 7d2c 207b 3130 3736 2c20 3435 317d  51}, {1076, 451}
-00003c20: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00003c30: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-00003c40: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00003c50: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
-00003c60: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-00003c70: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
-00003c80: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
-00003c90: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
-00003ca0: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00003cb0: 6d70 0000 0000 0011 dfa2 0000 0012 0066  mp.............f
-00003cc0: 0065 0061 0074 0075 0072 0065 005f 0065  .e.a.t.u.r.e._.e
-00003cd0: 0078 0074 0072 0061 0063 0074 006f 0072  .x.t.r.a.c.t.o.r
-00003ce0: 0073 6c73 7643 626c 6f62 0000 02b8 6270  .slsvCblob....bp
-00003cf0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-00003d00: 0a0b 0c0d 1a48 4948 4a4b 0c5f 1012 7669  .....HIHJK._..vi
-00003d10: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00003d20: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00003d30: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00003d40: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
-00003d50: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
-00003d60: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
-00003d70: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
-00003d80: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-00003d90: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00003da0: 6573 1001 09ab 0e17 1c21 252a 2f34 393e  es.......!%*/49>
-00003db0: 43d4 0f10 1112 1314 0c0c 5a69 6465 6e74  C.........Zident
-00003dc0: 6966 6965 7255 7769 6474 6859 6173 6365  ifierUwidthYasce
-00003dd0: 6e64 696e 6757 7669 7369 626c 6554 6e61  ndingWvisibleTna
-00003de0: 6d65 1101 a609 09d4 0f10 1112 1819 1a1a  me..............
-00003df0: 5875 6269 7175 6974 7910 2308 08d4 0f10  Xubiquity.#.....
-00003e00: 1112 1d1e 1a0c 5c64 6174 654d 6f64 6966  ......\dateModif
-00003e10: 6965 6410 b508 09d4 0f10 1112 221e 1a1a  ied........."...
-00003e20: 5b64 6174 6543 7265 6174 6564 0808 d40f  [dateCreated....
-00003e30: 1011 1226 271a 0c54 7369 7a65 1061 0809  ...&'..Tsize.a..
-00003e40: d40f 1011 122b 2c0c 0c54 6b69 6e64 1073  .....+,..Tkind.s
-00003e50: 0909 d40f 1011 1230 310c 1a55 6c61 6265  .......01..Ulabe
-00003e60: 6c10 6409 08d4 0f10 1112 3536 0c1a 5776  l.d.......56..Wv
-00003e70: 6572 7369 6f6e 104b 0908 d40f 1011 123a  ersion.K.......:
-00003e80: 3b0c 1a58 636f 6d6d 656e 7473 1101 2c09  ;..Xcomments..,.
-00003e90: 08d4 0f10 1112 3f40 1a1a 5e64 6174 654c  ......?@..^dateL
-00003ea0: 6173 744f 7065 6e65 6410 c808 08d4 0f10  astOpened.......
-00003eb0: 1112 441e 1a1a 5964 6174 6541 6464 6564  ..D...YdateAdded
-00003ec0: 0808 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00003ed0: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
-00003ee0: 6564 2340 3000 0000 0000 0009 0008 001d  ed#@0...........
-00003ef0: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00003f00: 00a1 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
-00003f10: 00e7 00ef 00f4 00f7 00f8 00f9 0102 010b  ................
-00003f20: 010d 010e 010f 0118 0125 0127 0128 0129  .........%.'.(.)
-00003f30: 0132 013e 013f 0140 0149 014e 0150 0151  .2.>.?.@.I.N.P.Q
-00003f40: 0152 015b 0160 0162 0163 0164 016d 0173  .R.[.`.b.c.d.m.s
-00003f50: 0175 0176 0177 0180 0188 018a 018b 018c  .u.v.w..........
-00003f60: 0195 019e 01a1 01a2 01a3 01ac 01bb 01bd  ................
-00003f70: 01be 01bf 01c8 01d2 01d3 01d4 01d5 01de  ................
-00003f80: 01e7 01f4 01fd 0000 0000 0000 0201 0000  ................
-00003f90: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-00003fa0: 0000 0000 01fe 0000 0000 0000 0000 0000  ................
+00003c00: 0808 0908 095f 1017 7b7b 3334 2c20 3930  ....._..{{34, 90
+00003c10: 7d2c 207b 3130 3135 2c20 3736 377d 7d09  }, {1015, 767}}.
+00003c20: 0817 2531 3d49 606d 797a 7b7c 7d7e 9800  ..%1=I`myz{|}~..
+00003c30: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00003c40: 0000 0000 0000 0000 0000 0000 0000 9900  ................
+00003c50: 0000 1200 6600 6500 6100 7400 7500 7200  ....f.e.a.t.u.r.
+00003c60: 6500 5f00 6500 7800 7400 7200 6100 6300  e._.e.x.t.r.a.c.
+00003c70: 7400 6f00 7200 7364 7363 6c62 6f6f 6c00  t.o.r.sdsclbool.
+00003c80: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
+00003c90: 0065 005f 0065 0078 0074 0072 0061 0063  .e._.e.x.t.r.a.c
+00003ca0: 0074 006f 0072 0073 6c67 3153 636f 6d70  .t.o.r.slg1Scomp
+00003cb0: 0000 0000 0012 686f 0000 0012 0066 0065  ......ho.....f.e
+00003cc0: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
+00003cd0: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
+00003ce0: 6c73 7643 626c 6f62 0000 02b8 6270 6c69  lsvCblob....bpli
+00003cf0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00003d00: 0c0d 1a48 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
+00003d10: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00003d20: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00003d30: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00003d40: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00003d50: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+00003d60: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+00003d70: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+00003d80: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+00003d90: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00003da0: 1001 09ab 0e17 1c21 252a 2f34 393e 43d4  .......!%*/49>C.
+00003db0: 0f10 1112 1314 0c0c 5a69 6465 6e74 6966  ........Zidentif
+00003dc0: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
+00003dd0: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
+00003de0: 1101 a609 09d4 0f10 1112 1819 1a1a 5875  ..............Xu
+00003df0: 6269 7175 6974 7910 2308 08d4 0f10 1112  biquity.#.......
+00003e00: 1d1e 1a0c 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00003e10: 6410 b508 09d4 0f10 1112 221e 1a1a 5b64  d........."...[d
+00003e20: 6174 6543 7265 6174 6564 0808 d40f 1011  ateCreated......
+00003e30: 1226 271a 0c54 7369 7a65 1061 0809 d40f  .&'..Tsize.a....
+00003e40: 1011 122b 2c0c 0c54 6b69 6e64 1073 0909  ...+,..Tkind.s..
+00003e50: d40f 1011 1230 310c 1a55 6c61 6265 6c10  .....01..Ulabel.
+00003e60: 6409 08d4 0f10 1112 3536 0c1a 5776 6572  d.......56..Wver
+00003e70: 7369 6f6e 104b 0908 d40f 1011 123a 3b0c  sion.K.......:;.
+00003e80: 1a58 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
+00003e90: 0f10 1112 3f40 1a1a 5e64 6174 654c 6173  ....?@..^dateLas
+00003ea0: 744f 7065 6e65 6410 c808 08d4 0f10 1112  tOpened.........
+00003eb0: 441e 1a1a 5964 6174 6541 6464 6564 0808  D...YdateAdded..
+00003ec0: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
+00003ed0: 0000 005c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00003ee0: 2340 3000 0000 0000 0009 0008 001d 0032  #@0............2
+00003ef0: 0044 004c 0060 0072 007b 008d 0098 00a1  .D.L.`.r.{......
+00003f00: 00b4 00b6 00b7 00c3 00cc 00d7 00dd 00e7  ................
+00003f10: 00ef 00f4 00f7 00f8 00f9 0102 010b 010d  ................
+00003f20: 010e 010f 0118 0125 0127 0128 0129 0132  .......%.'.(.).2
+00003f30: 013e 013f 0140 0149 014e 0150 0151 0152  .>.?.@.I.N.P.Q.R
+00003f40: 015b 0160 0162 0163 0164 016d 0173 0175  .[.`.b.c.d.m.s.u
+00003f50: 0176 0177 0180 0188 018a 018b 018c 0195  .v.w............
+00003f60: 019e 01a1 01a2 01a3 01ac 01bb 01bd 01be  ................
+00003f70: 01bf 01c8 01d2 01d3 01d4 01d5 01de 01e7  ................
+00003f80: 01f4 01fd 0000 0000 0000 0201 0000 0000  ................
+00003f90: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+00003fa0: 0000 01fe 0000 0000 0000 0000 0000 0000  ................
 00003fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004000: 0000 0000 0000 0000 0000 0015 0000 0012  ................
 00004010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00004020: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 00004030: 0072 0073 6d6f 4444 626c 6f62 0000 0008  .r.smoDDblob....
-00004040: ec48 4ecf 38f2 c441 0000 0012 0066 0065  .HN.8..A.....f.e
+00004040: ae8b 457c 94f5 c441 0000 0012 0066 0065  ..E|...A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
-00004070: 6d6f 6444 626c 6f62 0000 0008 ec48 4ecf  modDblob.....HN.
-00004080: 38f2 c441 0000 0012 0066 0065 0061 0074  8..A.....f.e.a.t
+00004070: 6d6f 6444 626c 6f62 0000 0008 ae8b 457c  modDblob......E|
+00004080: 94f5 c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
-000040b0: 636f 6d70 0000 0000 0014 2000 0000 0012  comp...... .....
+000040b0: 636f 6d70 0000 0000 0014 d000 0000 0012  comp............
 000040c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 000040d0: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 000040e0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 000040f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00004100: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00004110: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
 00004120: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
@@ -1049,21 +1049,21 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 017f c400 0000 0600 6d00 6900 7800  ..........m.i.x.
+000041f0: 0000 01a4 2400 0000 0600 6d00 6900 7800  ....$.....m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 08a1 1c42 882c f0c4 4100 0000 0600 6d00  ...B.,..A.....m.
+00004210: 08ef 201d a05b f6c4 4100 0000 0600 6d00  .. ..[..A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
-00004230: 6200 0000 08a1 1c42 882c f0c4 4100 0000  b......B.,..A...
+00004230: 6200 0000 08ef 201d a05b f6c4 4100 0000  b..... ..[..A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
-00004250: 5363 6f6d 7000 0000 0000 01c0 0000 0000  Scomp...........
+00004250: 5363 6f6d 7000 0000 0000 0200 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
 00004290: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
 000042a0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000042b0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 000042c0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
@@ -1239,44 +1239,44 @@
 00004d60: 013e 013f 0140 0149 014e 0150 0151 0152  .>.?.@.I.N.P.Q.R
 00004d70: 015b 0160 0162 0163 0164 016d 0173 0175  .[.`.b.c.d.m.s.u
 00004d80: 0176 0177 0180 0188 018a 018b 018c 0195  .v.w............
 00004d90: 019e 01a1 01a2 01a3 01ac 01bb 01bd 01be  ................
 00004da0: 01bf 01c8 01d2 01d3 01d4 01d5 01de 01e7  ................
 00004db0: 01f0 01f5 01fe 0000 0000 0000 0201 0000  ................
 00004dc0: 0000 0000 004e 0000 0000 0000 0000 0000  .....N..........
-00004dd0: 0000 0000 01ff 7669 7369 626c 6554 6e61  ......visibleTna
-00004de0: 6d65 1101 a609 09d4 0f10 1112 1819 1a1a  me..............
-00004df0: 5875 6269 7175 6974 7910 2308 08d4 0f10  Xubiquity.#.....
-00004e00: 1112 1d1e 1a0c 5c64 6174 654d 6f64 6966  ......\dateModif
-00004e10: 6965 6410 b508 09d4 0f10 1112 221e 1a1a  ied........."...
-00004e20: 5b64 6174 6543 7265 6174 6564 0808 d40f  [dateCreated....
-00004e30: 1011 1226 271a 0c54 7369 7a65 1061 0809  ...&'..Tsize.a..
-00004e40: d40f 1011 122b 2c0c 0c54 6b69 6e64 1073  .....+,..Tkind.s
-00004e50: 0909 d40f 1011 1230 310c 1a55 6c61 6265  .......01..Ulabe
-00004e60: 6c10 6409 08d4 0f10 1112 3536 0c1a 5776  l.d.......56..Wv
-00004e70: 6572 7369 6f6e 104b 0908 d40f 1011 123a  ersion.K.......:
-00004e80: 3b0c 1a58 636f 6d6d 656e 7473 1101 2c09  ;..Xcomments..,.
-00004e90: 08d4 0f10 1112 3f40 1a1a 5e64 6174 654c  ......?@..^dateL
-00004ea0: 6173 744f 7065 6e65 6410 c808 08d4 0f10  astOpened.......
-00004eb0: 1112 441e 1a1a 5964 6174 6541 6464 6564  ..D...YdateAdded
-00004ec0: 0808 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00004ed0: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
-00004ee0: 6564 2340 3000 0000 0000 0009 0008 001d  ed#@0...........
-00004ef0: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00004f00: 00a1 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
-00004f10: 00e7 00ef 00f4 00f7 00f8 00f9 0102 010b  ................
-00004f20: 010d 010e 010f 0118 0125 0127 0128 0129  .........%.'.(.)
-00004f30: 0132 013e 013f 0140 0149 014e 0150 0151  .2.>.?.@.I.N.P.Q
-00004f40: 0152 015b 0160 0162 0163 0164 016d 0173  .R.[.`.b.c.d.m.s
-00004f50: 0175 0176 0177 0180 0188 018a 018b 018c  .u.v.w..........
-00004f60: 0195 019e 01a1 01a2 01a3 01ac 01bb 01bd  ................
-00004f70: 01be 01bf 01c8 01d2 01d3 01d4 01d5 01de  ................
-00004f80: 01e7 01f4 01fd 0000 0000 0000 0201 0000  ................
-00004f90: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-00004fa0: 0000 0000 01fe 0000 0000 0000 0000 0000  ................
+00004dd0: 0000 0000 01ff 7369 626c 6554 6e61 6d65  ......sibleTname
+00004de0: 1101 a609 09d4 0f10 1112 1819 1a1a 5875  ..............Xu
+00004df0: 6269 7175 6974 7910 2308 08d4 0f10 1112  biquity.#.......
+00004e00: 1d1e 1a0c 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00004e10: 6410 b508 09d4 0f10 1112 221e 1a1a 5b64  d........."...[d
+00004e20: 6174 6543 7265 6174 6564 0808 d40f 1011  ateCreated......
+00004e30: 1226 271a 0c54 7369 7a65 1061 0809 d40f  .&'..Tsize.a....
+00004e40: 1011 122b 2c0c 0c54 6b69 6e64 1073 0909  ...+,..Tkind.s..
+00004e50: d40f 1011 1230 310c 1a55 6c61 6265 6c10  .....01..Ulabel.
+00004e60: 6409 08d4 0f10 1112 3536 0c1a 5776 6572  d.......56..Wver
+00004e70: 7369 6f6e 104b 0908 d40f 1011 123a 3b0c  sion.K.......:;.
+00004e80: 1a58 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
+00004e90: 0f10 1112 3f40 1a1a 5e64 6174 654c 6173  ....?@..^dateLas
+00004ea0: 744f 7065 6e65 6410 c808 08d4 0f10 1112  tOpened.........
+00004eb0: 441e 1a1a 5964 6174 6541 6464 6564 0808  D...YdateAdded..
+00004ec0: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
+00004ed0: 0000 005c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00004ee0: 2340 3000 0000 0000 0009 0008 001d 0032  #@0............2
+00004ef0: 0044 004c 0060 0072 007b 008d 0098 00a1  .D.L.`.r.{......
+00004f00: 00b4 00b6 00b7 00c3 00cc 00d7 00dd 00e7  ................
+00004f10: 00ef 00f4 00f7 00f8 00f9 0102 010b 010d  ................
+00004f20: 010e 010f 0118 0125 0127 0128 0129 0132  .......%.'.(.).2
+00004f30: 013e 013f 0140 0149 014e 0150 0151 0152  .>.?.@.I.N.P.Q.R
+00004f40: 015b 0160 0162 0163 0164 016d 0173 0175  .[.`.b.c.d.m.s.u
+00004f50: 0176 0177 0180 0188 018a 018b 018c 0195  .v.w............
+00004f60: 019e 01a1 01a2 01a3 01ac 01bb 01bd 01be  ................
+00004f70: 01bf 01c8 01d2 01d3 01d4 01d5 01de 01e7  ................
+00004f80: 01f4 01fd 0000 0000 0000 0201 0000 0000  ................
+00004f90: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+00004fa0: 0000 01fe 0000 0000 0000 0000 0000 0000  ................
 00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
 00005010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
@@ -1430,15 +1430,15 @@
 00005950: 0809 0809 5f10 187b 7b31 3930 2c20 3332  ...._..{{190, 32
 00005960: 7d2c 207b 3132 3530 2c20 3736 317d 7d09  }, {1250, 761}}.
 00005970: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 00005980: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 00005990: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 000059a0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
 000059b0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
-000059c0: 6731 5363 6f6d 7000 0000 0000 03b9 c400  g1Scomp.........
+000059c0: 6731 5363 6f6d 7000 0000 0000 03b9 6300  g1Scomp.......c.
 000059d0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
 000059e0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
 000059f0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 00005a00: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 00005a10: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 00005a20: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00005a30: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
@@ -1516,15 +1516,15 @@
 00005eb0: 0168 0169 016b 016c 016e 0177 0178 017a  .h.i.k.l.n.w.x.z
 00005ec0: 017b 017d 0186 0187 0189 018a 018c 0195  .{.}............
 00005ed0: 0196 0199 019a 019c 019d 01a6 01ab 0000  ................
 00005ee0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00005ef0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00005f00: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
 00005f10: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-00005f20: 4444 626c 6f62 0000 0008 be76 2985 44f2  DDblob.....v).D.
+00005f20: 4444 626c 6f62 0000 0008 0b30 86dc dcf4  DDblob.....0....
 00005f30: c441 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 00005f40: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 00005f50: 0073 6d6f 6444 626c 6f62 0000 0008 be76  .smodDblob.....v
 00005f60: 2985 44f2 c441 0000 000e 0070 006f 0073  ).D..A.....p.o.s
 00005f70: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00005f80: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
 00005f90: 0000 0004 4000 0000 000e 0070 006f 0073  ....@......p.o.s
@@ -1942,15 +1942,15 @@
 00007950: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
 00007960: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
 00007970: bb01 c400 0000 0000 0002 0100 0000 0000  ................
 00007980: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
 00007990: 0001 c500 0000 0000 0000 0000 0000 9a00  ................
 000079a0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
 000079b0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
-000079c0: 6731 5363 6f6d 7000 0000 0000 03b9 c400  g1Scomp.........
+000079c0: 6731 5363 6f6d 7000 0000 0000 03b9 6300  g1Scomp.......c.
 000079d0: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
 000079e0: 6d00 7000 6f00 7200 7400 6500 7200 736c  m.p.o.r.t.e.r.sl
 000079f0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 00007a00: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 00007a10: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 00007a20: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00007a30: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
@@ -2028,15 +2028,15 @@
 00007eb0: 0168 0169 016b 016c 016e 0177 0178 017a  .h.i.k.l.n.w.x.z
 00007ec0: 017b 017d 0186 0187 0189 018a 018c 0195  .{.}............
 00007ed0: 0196 0199 019a 019c 019d 01a6 01ab 0000  ................
 00007ee0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00007ef0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00007f00: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
 00007f10: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-00007f20: 4444 626c 6f62 0000 0008 be76 2985 44f2  DDblob.....v).D.
+00007f20: 4444 626c 6f62 0000 0008 0b30 86dc dcf4  DDblob.....0....
 00007f30: c441 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 00007f40: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 00007f50: 0073 6d6f 6444 626c 6f62 0000 0008 be76  .smodDblob.....v
 00007f60: 2985 44f2 c441 0000 000e 0070 006f 0073  ).D..A.....p.o.s
 00007f70: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00007f80: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
 00007f90: 0000 0004 4000 0000 000e 0070 006f 0073  ....@......p.o.s
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,14 @@
         compass_lookup = [int(i) for i in compass_lookup]
         compasFaceList_bracket, compasFaceList_digit = [], []
         for compasDirection in compass_lookup:
             compasFaceList_bracket.append(self.compass_brackets[compasDirection])
             compasFaceList_digit.append(self.compass_brackets_digits[compasDirection])
         self.csv_df_combined['Compass_direction'] = compasFaceList_bracket
         self.csv_df_combined['Compass_digit'] = compasFaceList_digit
-
         for i in self.roll_windows_values:
             column_name = f'Mean_angle_time_window_{i}'
             self.csv_df_combined[column_name] = self.csv_df_combined['Clockwise_angle_degrees'].rolling(i, min_periods=1).mean()
 
     def hot_end_encode_compass(self):
         compass_hot_end = pd.get_dummies(self.csv_df_combined['Compass_direction'], prefix='Direction')
         compass_hot_end = compass_hot_end.T.reindex(self.compass_brackets_long).T.fillna(0)
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -276,18 +276,18 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 000b e25d 0000 000b 005f 005f 0070  .....]....._._.p
+000011a0: 0000 000b e20e 0000 000b 005f 005f 0070  ..........._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 33a8 ef60  moDDblob....3..`
-000011d0: 48f2 c441 0000 000b 005f 005f 0070 0079  H..A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 4cb8 15d8  moDDblob....L...
+000011d0: dcf4 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 000011f0: 6444 626c 6f62 0000 0008 0a8c 6973 23f2  dDblob......is#.
 00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 000c 9000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
@@ -296,21 +296,21 @@
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000012a0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000012b0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 000012c0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000012e0: 6261 7208 0809 0809 5f10 177b 7b35 302c  bar....._..{{50,
-000012f0: 2036 357d 2c20 7b31 3037 362c 2034 3531   65}, {1076, 451
+000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
+000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
 00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
 00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
 00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
-00001340: 3153 636f 6d70 0000 0000 0001 dac4 0000  1Scomp..........
+00001340: 3153 636f 6d70 0000 0000 0002 7de8 0000  1Scomp......}...
 00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
 00001360: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
 00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
 00001380: 4a4b 0c5f 1012 7669 6577 4f70 7469 6f6e  JK._..viewOption
 00001390: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 000013a0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 000013b0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -391,19 +391,19 @@
 00001860: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
 00001870: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
 00001880: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
 00001890: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
 000018a0: d301 dc00 0000 0000 0002 0100 0000 0000  ................
 000018b0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 000018c0: 0001 dd00 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
-000018d0: 6f44 4462 6c6f 6200 0000 0848 ebac 9be4  oDDblob....H....
-000018e0: f2c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
-000018f0: 6f64 4462 6c6f 6200 0000 0848 ebac 9be4  odDblob....H....
-00001900: f2c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
-00001910: 6831 5363 6f6d 7000 0000 0000 0280 0000  h1Scomp.........
+000018d0: 6f44 4462 6c6f 6200 0000 081a 1af6 afc4  oDDblob.........
+000018e0: f6c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
+000018f0: 6f64 4462 6c6f 6200 0000 081a 1af6 afc4  odDblob.........
+00001900: f6c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
+00001910: 6831 5363 6f6d 7000 0000 0000 0360 0000  h1Scomp......`..
 00001920: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
 00001930: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/extract_features_9bp.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from simba.feature_extractors.unit_tests import check_minimum_roll_windows, read_video_info_csv, read_video_info
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from simba.feature_extractors.unit_tests import read_video_info
 
 from simba.drop_bp_cords import get_fn_ext
 from simba.rw_dfs import read_df, save_df
 
-def extract_features_wotarget_9(inifile):
+def extract_features_wotarget_9(config_path: str):
     config = ConfigParser()
-    config.read(str(inifile))
+    config.read(str(config_path))
     csv_dir = config.get('General settings', 'csv_path')
     csv_dir_in = os.path.join(csv_dir, 'outlier_corrected_movement_location')
     csv_dir_out = os.path.join(csv_dir, 'features_extracted')
     project_path = config.get('General settings', 'project_path')
     vidinfDf = read_video_info_csv(os.path.join(project_path, 'logs', 'video_info.csv'))
 
     if not os.path.exists(csv_dir_out):
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.56.4/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.56.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/severity_processor.py` & `Simba-UW-tf-dev-1.56.4/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.56.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.56.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.56.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.56.4/simba/machine_model_settings_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.create_meta_data_file_var = BooleanVar()
         self.create_example_decision_tree_graphviz_var = BooleanVar()
         self.create_example_decision_tree_dtreeviz_var = BooleanVar()
         self.create_clf_report_var = BooleanVar()
         self.create_clf_importance_bars_var = BooleanVar()
         self.feature_permutation_importance_var = BooleanVar()
         self.create_pr_curve_var = BooleanVar()
-        self.partial_dependency_var =BooleanVar()
+        self.partial_dependency_var = BooleanVar()
         self.calc_shap_scores_var = BooleanVar()
         self.learning_curve_var = BooleanVar()
 
         self.meta_data_file_cb = Checkbutton(self.evaluations_frm,text='Create model meta data file', variable=self.create_meta_data_file_var)
         self.decision_tree_graphviz_cb = Checkbutton(self.evaluations_frm, text='Create Example Decision Tree (requires "graphviz")', variable=self.create_example_decision_tree_graphviz_var)
         self.decision_tree_dtreeviz_cb = Checkbutton(self.evaluations_frm, text='Create Fancy Example Decision Tree (requires "dtreeviz")', variable=self.create_example_decision_tree_dtreeviz_var)
         self.clf_report_cb = Checkbutton(self.evaluations_frm, text='Create Classification Report', variable=self.create_clf_report_var)
@@ -109,15 +109,15 @@
         self.learning_curve_cb = Checkbutton(self.evaluations_frm, text='Create Learning Curves (Note: CPU intensive)', variable=self.learning_curve_var, command=lambda: self.enable_entrybox_from_checkbox(check_box_var=self.learning_curve_var, entry_boxes=[self.learning_curve_k_splits_entry_box, self.learning_curve_data_splits_entry_box]))
         self.create_pr_curve_cb = Checkbutton(self.evaluations_frm, text='Create Precision Recall Curves', variable=self.create_pr_curve_var)
         self.shap_present = Entry_Box(self.evaluations_frm, '# target present', '25', status=DISABLED, validation='numeric')
         self.shap_absent = Entry_Box(self.evaluations_frm, '# target absent', '25', status=DISABLED,  validation='numeric')
         self.shap_save_it_dropdown = DropDownMenu(self.evaluations_frm, 'SHAP save cadence: ', [1, 10, 100, 1000, 'ALL FRAMES'],  '25')
         self.shap_save_it_dropdown.setChoices('ALL FRAMES')
         self.shap_save_it_dropdown.disable()
-        self.partial_dependency_cb = Checkbutton(self.evaluations_frm, text='Calculate partial dependencies', variable=self.partial_dependency_var)
+        self.partial_dependency_cb = Checkbutton(self.evaluations_frm, text='Calculate partial dependencies (Note: CPU intensive)', variable=self.partial_dependency_var)
         self.calculate_shap_scores_cb = Checkbutton(self.evaluations_frm, text='Calculate SHAP scores', variable=self.calc_shap_scores_var, command=lambda: [self.enable_entrybox_from_checkbox(check_box_var=self.calc_shap_scores_var, entry_boxes=[self.shap_present,self.shap_absent]),
                                                                                                                                                              self.enable_dropdown_from_checkbox(check_box_var=self.calc_shap_scores_var, dropdown_menus=[self.shap_save_it_dropdown])])
         self.save_frame = LabelFrame(main, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         save_global_btn = Button(self.save_frame, text='SAVE SETTINGS (GLOBAL ENVIRONMENT)', font=('Helvetica', 12, 'bold'), fg='blue', command=lambda: self.save_global())
         save_meta_btn = Button(self.save_frame, text='SAVE SETTINGS (SPECIFIC MODEL)', font=('Helvetica', 12, 'bold'), fg='green', command=lambda: self.save_config())
         clear_cache_btn = Button(self.save_frame,text='CLEAR CACHE', font=('Helvetica', 12, 'bold'),fg='red', command=lambda: self.clear_cache())
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.56.4/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.56.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.56.4/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.56.4/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.56.4/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/video_info_table.py` & `Simba-UW-tf-dev-1.56.4/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.56.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.56.4/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.56.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.56.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.56.4/simba/utils/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,19 @@
 
 class AnnotationFileNotFoundError(SimbaError):
     def __init__(self, video_name: str, show_window: bool = False):
         msg = f'SIMBA THIRD-PARTY ANNOTATION ERROR: NO ANNOTATION DATA FOR VIDEO {video_name} FOUND'
         super().__init__(msg=msg, show_window=show_window)
         self.print_msg(msg=msg)
 
+class DirectoryNotEmptyError(SimbaError):
+    def __init__(self, msg: str, show_window: bool = False):
+        super().__init__(msg=msg, show_window=show_window)
+        self.print_msg(msg=f'SIMBA DIRECTORY NOT EMPTY ERROR: {msg}')
+
 
 
 #####
 
 
 class ThirdPartyAnnotationFileNotFoundError(SimbaError):
     def __init__(self, video_name: str, show_window: bool = False):
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.56.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.56.4/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.56.4/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.56.4/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.56.4/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/movement_processor.py` & `Simba-UW-tf-dev-1.56.4/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pybursts.py` & `Simba-UW-tf-dev-1.56.4/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.56.4/simba/rw_dfs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 from simba.utils.errors import InvalidFileTypeError
 from simba.enums import Formats
 from simba.read_config_unit_tests import check_file_exist_and_readable
 import pyarrow as pa
 import numpy as np
+import pickle
 from pyarrow import csv
 
 
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
-#WRITE_OPTIONS = csv.WriteOptions(delimiter=r',')
 
 def read_df(file_path: str,
             file_type: str,
             idx=0,
             remove_columns: list or None=None,
             usecols: list or None=None):
     """
@@ -78,23 +78,29 @@
     Returns
     -------
     None
     """
 
     if file_type == Formats.CSV.value:
         df = df.drop('scorer', axis=1, errors='ignore')
-        # df.to_csv(save_path, index=True)
         idx = np.arange(len(df)).astype(str)
         df.insert(0, '', idx)
         df = pa.Table.from_pandas(df=df)
         csv.write_csv(df, save_path)
     elif file_type == Formats.PARQUET.value:
-        df.to_parquet(file_type)
+        df.to_parquet(save_path)
+    elif file_type == Formats.PICKLE.value:
+        try:
+            with open(save_path, 'wb') as f:
+                pickle.dump(df, f, protocol=pickle.HIGHEST_PROTOCOL)
+        except Exception as e:
+            print(e.args[0])
+            raise InvalidFileTypeError(msg='Data could not be saved as a pickle.')
     else:
-        raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [csv, parquet]')
+        raise InvalidFileTypeError(msg=f'{file_type} is not a valid filetype OPTIONS: [csv, pickle, parquet]')
 
 # df = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv/Together_1.csv', file_type='csv')
 # df = df.loc[2:]
 # df = pd.concat([df, df, df,df, df, df,df, df, df]).reset_index(drop=True)
 # df = pd.concat([df, df, df]).reset_index(drop=True)
 # df = pd.concat([df, df,df, df, df]).reset_index(drop=True)
 # df = pd.concat([df, df, df, df], axis=1).reset_index(drop=True)
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.56.4/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.56.4/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.56.4/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/setting_menu.py` & `Simba-UW-tf-dev-1.56.4/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.56.4/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/run_inference.py` & `Simba-UW-tf-dev-1.56.4/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.56.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.56.4/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.56.4/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/dash_app.py` & `Simba-UW-tf-dev-1.56.4/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.56.4/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.56.4/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.56.4/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.56.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/misc_tools.py` & `Simba-UW-tf-dev-1.56.4/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.56.4/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.56.4/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.56.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.56.4/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.56.4/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.56.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/pose_reset.py` & `Simba-UW-tf-dev-1.56.4/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.56.4/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.56.4/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.56.4/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.56.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.56.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -484,19 +484,19 @@
 00001e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00001e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00001e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00001e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00001e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00001e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00001e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00001ea0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+00001ea0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
 00001eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-00001ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+00001ec0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
 00001ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-00001ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+00001ee0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
 00001ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00001f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
 00001f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00001f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00001f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00001f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
@@ -522,15 +522,15 @@
 00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
 000020a0: 0809 0809 5f10 187b 7b34 3134 2c20 3136  ...._..{{414, 16
 000020b0: 317d 2c20 7b37 3730 2c20 3433 367d 7d09  1}, {770, 436}}.
 000020c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
 000020d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
 000020f0: 0000 0500 6900 6300 6f00 6e00 736c 6731  ....i.c.o.n.slg1
-00002100: 5363 6f6d 7000 0000 0000 0590 7700 0000  Scomp.......w...
+00002100: 5363 6f6d 7000 0000 0000 0598 d900 0000  Scomp...........
 00002110: 0500 6900 6300 6f00 6e00 736c 7376 4362  ..i.c.o.n.slsvCb
 00002120: 6c6f 6200 0002 af62 706c 6973 7430 30da  lob....bplist00.
 00002130: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
 00002140: 484a 0c4c 5f10 1276 6965 774f 7074 696f  HJ.L_..viewOptio
 00002150: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
 00002160: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
 00002170: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
@@ -611,20 +611,20 @@
 00002620: 016b 016c 016d 016f 0178 0179 017b 017c  .k.l.m.o.x.y.{.|
 00002630: 017e 0187 0188 018a 018b 018d 0196 0197  .~..............
 00002640: 0199 019a 019c 01a5 01a6 01a8 01a9 01ab  ................
 00002650: 01b4 01b5 01b7 01b8 01ba 01bb 01c4 01cd  ................
 00002660: 01d2 01d3 0000 0000 0000 0201 0000 0000  ................
 00002670: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
 00002680: 0000 01dc 0000 0005 0069 0063 006f 006e  .........i.c.o.n
-00002690: 0073 6d6f 4444 626c 6f62 0000 0008 da62  .smoDDblob.....b
-000026a0: afb9 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+00002690: 0073 6d6f 4444 626c 6f62 0000 0008 c1fc  .smoDDblob......
+000026a0: 2155 22f4 c441 0000 0005 0069 0063 006f  !U"..A.....i.c.o
 000026b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-000026c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+000026c0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
 000026d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-000026e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+000026e0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
 000026f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00002700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
 00002710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00002720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
@@ -868,19 +868,19 @@
 00003630: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003640: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003650: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003660: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003670: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003680: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003690: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-000036a0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+000036a0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
 000036b0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-000036c0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+000036c0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
 000036d0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-000036e0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+000036e0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
 000036f0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00003700: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
 00003710: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00003720: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00003730: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00003740: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00003750: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
@@ -996,19 +996,19 @@
 00003e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003ea0: 01c5 1af0 c441 0000 0005 0069 0063 006f  .....A.....i.c.o
+00003ea0: 01c5 22f4 c441 0000 0005 0069 0063 006f  .."..A.....i.c.o
 00003eb0: 006e 0073 6d6f 6444 626c 6f62 0000 0008  .n.smodDblob....
-00003ec0: da62 afb9 1af0 c441 0000 0005 0069 0063  .b.....A.....i.c
+00003ec0: c1fc 2155 22f4 c441 0000 0005 0069 0063  ..!U"..A.....i.c
 00003ed0: 006f 006e 0073 7068 3153 636f 6d70 0000  .o.n.sph1Scomp..
-00003ee0: 0000 0007 f000 0000 0005 0069 0063 006f  ...........i.c.o
+00003ee0: 0000 0008 0000 0000 0005 0069 0063 006f  ...........i.c.o
 00003ef0: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00003f00: 0000 0003 0069 006d 0067 6277 7370 626c  .....i.m.gbwspbl
 00003f10: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00003f20: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00003f30: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00003f40: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00003f50: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
```

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.56.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.56.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.56.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.56.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.56.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.56.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.56.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.56.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.56.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.56.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.56.4/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.56.4/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.56.4/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.56.4/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/train_single_model.py` & `Simba-UW-tf-dev-1.56.4/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.56.4/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.56.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.56.4/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.56.4/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.56.4/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.56.3
+Version: 1.56.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -212,26 +212,29 @@
 simba/feature_extractors/misc/convex_hull_scratch_1.py
 simba/feature_extractors/misc/convex_hull_scratch_2.py
 simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/doctests.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
+simba/feature_extractors/misc/video_rotator_mp.py
 simba/mixins/.DS_Store
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/pop_up_mixin.py
+simba/mixins/unsupervised_mixin.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
 simba/outlier_tools/outlier_corrector_movement.py
 simba/outlier_tools/skip_outlier_correction.py
 simba/outlier_tools/.idea/encodings.xml
 simba/outlier_tools/.idea/misc.xml
@@ -326,21 +329,26 @@
 simba/third_party_label_appenders/third_party_appender.py
 simba/third_party_label_appenders/tools.py
 simba/unsupervised/.DS_Store
 simba/unsupervised/cluster_statistics.py
 simba/unsupervised/cluster_visualizer.py
 simba/unsupervised/data_extractors.py
 simba/unsupervised/dataset_creator.py
+simba/unsupervised/dataset_creator_2.py
 simba/unsupervised/dbcv.py
+simba/unsupervised/enums.py
+simba/unsupervised/grd_search_img_visualizer_2.py
 simba/unsupervised/hdbscan_clusterer.py
+simba/unsupervised/hdbscan_clusterer_2.py
 simba/unsupervised/misc.py
 simba/unsupervised/pop_up_classes.py
 simba/unsupervised/tsne.py
 simba/unsupervised/ui_tools.py
 simba/unsupervised/umap_embedder.py
+simba/unsupervised/umap_embedder_2.py
 simba/unsupervised/unsupervised_ui.py
 simba/unsupervised/visualizers.py
 simba/unsupervised/visualization_tools/vtk_embeddings.py
 simba/utils/.DS_Store
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
```

### Comparing `Simba-UW-tf-dev-1.56.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.56.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/LICENSE.md` & `Simba-UW-tf-dev-1.56.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/README.md` & `Simba-UW-tf-dev-1.56.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.56.3/setup.py` & `Simba-UW-tf-dev-1.56.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.56.3",
+    version="1.56.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

