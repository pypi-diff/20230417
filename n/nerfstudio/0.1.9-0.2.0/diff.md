# Comparing `tmp/nerfstudio-0.1.9.tar.gz` & `tmp/nerfstudio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-0.1.9.tar", last modified: Fri Nov 11 06:53:22 2022, max compression
+gzip compressed data, was "nerfstudio-0.2.0.tar", last modified: Mon Apr 17 16:19:31 2023, max compression
```

## Comparing `nerfstudio-0.1.9.tar` & `nerfstudio-0.2.0.tar`

### file list

```diff
@@ -1,165 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14417 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14016 2022-11-11 06:53:15.000000 nerfstudio-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)    15282 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    18830 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     8397 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10197 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7215 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17677 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datamanagers/base_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datamanagers/semantic_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5708 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/friends_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5222 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7655 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/dataparsers/record3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3686 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8932 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/data/utils/dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5676 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15485 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/base_field_component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)    18757 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6071 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3286 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/field_components/spatial_distortions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/instant_ngp_field.py
--rw-r--r--   0 runner    (1001) docker     (121)    14901 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     6831 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/exporters.py
--rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    21186 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10549 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/model_components/scene_colliders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.267775 nerfstudio-0.1.9/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8207 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (121)    12295 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (121)    12733 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (121)    10791 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7982 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14865 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/pipelines/dynamic_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15502 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    16180 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10191 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    16940 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/app/
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/app/public/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio/viewer/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/app/src/themes/leva_theme.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     8633 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/nerfstudio/viewer/server/state/
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/video_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    31570 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/viewer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/nerfstudio/viewer/server/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.263775 nerfstudio-0.1.9/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14417 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4572 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-11 06:53:22.000000 nerfstudio-0.1.9/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.271775 nerfstudio-0.1.9/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/completions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9698 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/docs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2647 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/docs/add_nb_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1402 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/downloads/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7551 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/downloads/download_data.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1584 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (121)     4226 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/github/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3438 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/github/run_actions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37452 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/render.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8854 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-11-11 06:53:08.000000 nerfstudio-0.1.9/scripts/viewer/view_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 06:53:22.275775 nerfstudio-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.444048 nerfstudio-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-04-17 16:19:24.000000 nerfstudio-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/depth_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/sdf_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datamanagers/semantic_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.420048 nerfstudio-0.2.0/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20570 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/data/utils/nerfstudio_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.424048 nerfstudio-0.2.0/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/base_field_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/field_components/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/cuda/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/temporal_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/field_components/temporal_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/instant_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfplayer_ngp_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17598 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/generative/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.428048 nerfstudio-0.2.0/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfplayer_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/nerfplayer_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.432048 nerfstudio-0.2.0/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio/viewer/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.436048 nerfstudio-0.2.0/nerfstudio/viewer/server/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/nerfstudio/viewer/viser/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/nerfstudio/viewer/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.416048 nerfstudio-0.2.0/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 16:19:31.000000 nerfstudio-0.2.0/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/datasets/process_nuscenes_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/generative/trace_stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35406 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/scripts/viewer/sync_viser_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:19:31.444048 nerfstudio-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:19:31.440048 nerfstudio-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-17 16:19:16.000000 nerfstudio-0.2.0/tests/test_train.py
```

### Comparing `nerfstudio-0.1.9/LICENSE` & `nerfstudio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/PKG-INFO` & `nerfstudio-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 0.1.9
+Version: 0.2.0
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown
+Provides-Extra: gen
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <p align="center">
     <!-- community badges -->
     <a href="https://discord.gg/uMbNqcraFc"><img src="https://img.shields.io/badge/Join-Discord-blue.svg"/></a>
@@ -83,122 +84,165 @@
 The quickstart will help you get started with the default vanilla NeRF trained on the classic Blender Lego scene.
 For more complex changes (e.g., running with your own data/setting up a new NeRF graph, please refer to our [references](#learn-more).
 
 ## 1. Installation: Setup the environment
 
 ### Prerequisites
 
-CUDA must be installed on the system. This library has been tested with version 11.3. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
+You must have an NVIDIA video card with CUDA installed on the system. This library has been tested with version 11.3 of CUDA. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
 
 ### Create environment
 
 Nerfstudio requires `python >= 3.7`. We recommend using conda to manage dependencies. Make sure to install [Conda](https://docs.conda.io/en/latest/miniconda.html) before proceeding.
 
 ```bash
 conda create --name nerfstudio -y python=3.8
 conda activate nerfstudio
 python -m pip install --upgrade pip
 ```
 
 ### Dependencies
 
-Install pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+Install pytorch with CUDA (this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+
+For CUDA 11.3:
 
 ```bash
 pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/whl/torch_stable.html
-pip install git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+```
+
+For CUDA 11.7:
+
+```bash
+pip install torch==1.13.1 torchvision functorch --extra-index-url https://download.pytorch.org/whl/cu117
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
 ```
 
+See [Dependencies](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md#dependencies)
+in the Installation documentation for more.
+
 ### Installing nerfstudio
 
 Easy option:
 
 ```bash
 pip install nerfstudio
 ```
 
-If you want the latest and greatest:
+**OR** if you want the latest and greatest:
 
 ```bash
 git clone https://github.com/nerfstudio-project/nerfstudio.git
 cd nerfstudio
 pip install --upgrade pip setuptools
 pip install -e .
 ```
 
-## 2. Setting up the data
+**OR** if you want to skip all installation steps and directly start using nerfstudio, use the docker image:
+
+See [Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md) - **Use docker image**.
+
+## 2. Training your first model!
 
-Download the original NeRF Blender dataset. We support the major datasets and allow users to create their own dataset, described in detail [here](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html).
+The following will train a _nerfacto_ model, our recommended model for real world scenes.
 
 ```bash
-ns-download-data --dataset=blender
-ns-download-data --dataset=nerfstudio --capture=poster
+# Download some test data:
+ns-download-data nerfstudio --capture-name=poster
+# Train model
+ns-train nerfacto --data data/nerfstudio/poster
 ```
 
-### 2.x Using custom data
+If everything works, you should see training progress like the following:
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766069-cadfd34f-8833-4156-88b7-ad406d688fc0.png">
+</p>
+
+Navigating to the link at the end of the terminal will load the webviewer. If you are running on a remote machine, you will need to port forward the websocket port (defaults to 7007).
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766653-586a0daa-466b-4140-a136-6b02f2ce2c54.png">
+</p>
 
-If you have custom data in the form of a video or folder of images, we've provided some [COLMAP](https://colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to help you process your data so it is compatible with nerfstudio.
+### Resume from checkpoint / visualize existing run
 
-After installing both software, you can process your data via:
+It is possible to load a pretrained model by running
 
 ```bash
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir {PROCESSED_DATA_DIR}
-# Or if you're on a system without an attached display (i.e. colab):
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH}  --output-dir {PROCESSED_DATA_DIR} --no-gpu
+ns-train nerfacto --data data/nerfstudio/poster --load-dir {outputs/.../nerfstudio_models}
 ```
 
-## 3. Training a model
+This will automatically start training. If you do not want it to train, add `--viewer.start-train False` to your training command.
 
-To run with all the defaults, e.g., vanilla NeRF method with the Blender Lego image
+## 3. Exporting Results
 
-```bash
-# To see what models are available.
-ns-train --help
+Once you have a NeRF model you can either render out a video or export a point cloud.
 
-# To see what model-specific cli arguments are available.
-ns-train nerfacto --help
+### Render Video
 
-# Run with nerfacto model.
-ns-train nerfacto
+First we must create a path for the camera to follow. This can be done in the viewer under the "RENDER" tab. Orient your 3D view to the location where you wish the video to start, then press "ADD CAMERA". This will set the first camera key frame. Continue to new viewpoints adding additional cameras to create the camera path. We provide other parameters to further refine your camera path. Once satisfied, press "RENDER" which will display a modal that contains the command needed to render the video. Kill the training job (or create a new terminal if you have lots of compute) and run the command to generate the video.
 
-# We provide support for other models. E.g., to run instant-ngp.
-ns-train instant-ngp
+Other video export options are available, learn more by running
 
-# To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR}
+```bash
+ns-render --help
 ```
 
-### 3.x Training a model with the viewer
+### Generate Point Cloud
 
-You can visualize training in real-time using our web-based viewer.
+While NeRF models are not designed to generate point clouds, it is still possible. Navigate to the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option is selected, everything in the yellow square will be exported into a point cloud. Modify the settings as desired then run the command at the bottom of the panel in your command line.
 
-Make sure to forward a port for the websocket to localhost. The default port is 7007, which you should expose to localhost:7007.
+Alternatively you can use the CLI without the viewer. Learn about the export options by running
 
 ```bash
-# with the default port
-ns-train nerfacto --vis viewer
+ns-export pointcloud --help
+```
+
+## 4. Using Custom Data
+
+Using an existing dataset is great, but likely you want to use your own data! We support various methods for using your own data. Before it can be used in nerfstudio, the camera location and orientations must be determined and then converted into our format using `ns-process-data`. We rely on external tools for this, instructions and information can be found in the documentation.
+
+| Data                                                                                                 | Capture Device | Requirements                                                      | `ns-process-data` Speed |
+| ---------------------------------------------------------------------------------------------------- | -------------- | ----------------------------------------------------------------- | ----------------------- |
+| 📷 [Images](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)      | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📹 [Video](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)       | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 🌎 [360 Data](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#360_data)            | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📱 [Polycam](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#polycam-capture)      | IOS with LiDAR | [Polycam App](https://poly.cam/)                                  | 🐇                      |
+| 📱 [KIRI Engine](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#kiri-capture)     | IOS or Android | [KIRI Engine App](https://www.kiriengine.com/)                    | 🐇                      |
+| 📱 [Record3D](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture)    | IOS with LiDAR | [Record3D app](https://record3d.app/)                             | 🐇                      |
+| 🖥 [Metashape](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#metashape)           | Any            | [Metashape](https://www.agisoft.com/)                             | 🐇                      |
+| 🖥 [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#realitycapture) | Any            | [RealityCapture](https://www.capturingreality.com/realitycapture) | 🐇                      |
+| 🛠 [Custom](https://docs.nerf.studio/en/latest/quickstart/data_conventions.html)                      | Any            | Camera Poses                                                      | 🐇                      |
 
-# with a specified websocket port
-ns-train nerfacto --vis viewer --viewer.websocket-port=7008
+## 5. Advanced Options
 
-# port forward if running on remote
-ssh -L localhost:7008:localhost:7008 {REMOTE HOST}
+### Training models other than nerfacto
+
+We provide other models than nerfacto, for example if you want to train the original nerf model, use the following command
+
+```bash
+ns-train vanilla-nerf --data DATA_PATH
 ```
 
-For more details on how to interact with the visualizer, please visit our viewer [walk-through](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html).
+For a full list of included models run `ns-train --help`.
 
-## 4. Rendering a trajectory during inference
+### Modify Configuration
 
-After your model has trained, you can headlessly render out a video of the scene with a pre-defined trajectory.
+Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
-# assuming previously ran `ns-train nerfacto`
-ns-render --load-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --traj=spiral --output-path=renders/output.mp4
+ns-train nerfacto --help
 ```
 
+### Tensorboard / WandB
+
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
 
 | Section                                                                                            | Description                                                                                        |
@@ -215,30 +259,29 @@
 | 💻 **For Developers**                                                                              |
 | [Creating pipelines](https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html)     | Learn how to easily build new neural rendering pipelines by using and/or implementing new modules. |
 | [Creating datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html)             | Have a new dataset? Learn how to run it with nerfstudio.                                           |
 | [Contributing](https://docs.nerf.studio/en/latest/reference/contributing.html)                     | Walk-through for how you can start contributing now.                                               |
 | 💖 **Community**                                                                                   |
 | [Discord](https://discord.gg/uMbNqcraFc)                                                           | Join our community to discuss more. We would love to hear from you!                                |
 | [Twitter](https://twitter.com/nerfstudioteam)                                                      | Follow us on Twitter @nerfstudioteam to see cool updates and announcements                         |
-| [TikTok](#)                                                                                        | Coming soon! Follow us on TikTok to see some of our fan favorite results                           |
 
 # Supported Features
 
-We provide the following support structures to make life easier for getting started with NeRFs. For a full description, please refer to our [features page](#).
+We provide the following support structures to make life easier for getting started with NeRFs.
 
 **If you are looking for a feature that is not currently supported, please do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/uMbNqcraFc)!**
 
 - :mag_right: Web-based visualizer that allows you to:
   - Visualize training in real-time + interact with the scene
   - Create and render out scenes with custom camera trajectories
   - View different output types
   - And more!
 - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb), code profiling, and other built-in debugging tools
 - :chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender dataset
-- :iphone: Full pipeline support (w/ Colmap or Record3D) for going from a video on your phone to a full 3D render.
+- :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for going from a video on your phone to a full 3D render.
 
 # Built On
 
 <a href="https://github.com/brentyi/tyro">
     <img alt="tyro logo" src="https://brentyi.github.io/tyro/_static/logo-light.svg" width="150px" />
 </a>
 
@@ -250,24 +293,26 @@
 </a>
 
 - Library for accelerating NeRF renders
 - Developed by [Ruilong Li](https://www.liruilong.cn/)
 
 # Citation
 
+You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
+
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@misc{nerfstudio,
-      title={Nerfstudio: A Framework for Neural Radiance Field Development},
-      author={Matthew Tancik*, Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi,
-              Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi,
-              Abhik Ahuja, David McAllister, Angjoo Kanazawa},
-      year={2022},
-      url={https://github.com/nerfstudio-project/nerfstudio},
+@article{nerfstudio,
+    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
+            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
+    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+    journal = {arXiv preprint arXiv:2302.04264},
+    year = {2023},
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.1.9 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.0 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-docs License-File: LICENSE
+Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
+Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
                                  [nerfstudio]
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
@@ -31,71 +31,124 @@
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
 nerfstudio enables you to build faster :hammer: learn together :books: and
 contribute to our NeRF community :sparkling_heart:. # Quickstart The quickstart
 will help you get started with the default vanilla NeRF trained on the classic
 Blender Lego scene. For more complex changes (e.g., running with your own data/
 setting up a new NeRF graph, please refer to our [references](#learn-more). ##
-1. Installation: Setup the environment ### Prerequisites CUDA must be installed
-on the system. This library has been tested with version 11.3. You can find
-more information about installing CUDA [here](https://docs.nvidia.com/cuda/
-cuda-quick-start-guide/index.html) ### Create environment Nerfstudio requires
-`python >= 3.7`. We recommend using conda to manage dependencies. Make sure to
-install [Conda](https://docs.conda.io/en/latest/miniconda.html) before
-proceeding. ```bash conda create --name nerfstudio -y python=3.8 conda activate
-nerfstudio python -m pip install --upgrade pip ``` ### Dependencies Install
-pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn]
-(https://github.com/NVlabs/tiny-cuda-nn) ```bash pip install
+1. Installation: Setup the environment ### Prerequisites You must have an
+NVIDIA video card with CUDA installed on the system. This library has been
+tested with version 11.3 of CUDA. You can find more information about
+installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/
+index.html) ### Create environment Nerfstudio requires `python >= 3.7`. We
+recommend using conda to manage dependencies. Make sure to install [Conda]
+(https://docs.conda.io/en/latest/miniconda.html) before proceeding. ```bash
+conda create --name nerfstudio -y python=3.8 conda activate nerfstudio python -
+m pip install --upgrade pip ``` ### Dependencies Install pytorch with CUDA
+(this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn]
+(https://github.com/NVlabs/tiny-cuda-nn) For CUDA 11.3: ```bash pip install
 torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/
-whl/torch_stable.html pip install git+https://github.com/NVlabs/tiny-cuda-nn/
-#subdirectory=bindings/torch ``` ### Installing nerfstudio Easy option: ```bash
-pip install nerfstudio ``` If you want the latest and greatest: ```bash git
-clone https://github.com/nerfstudio-project/nerfstudio.git cd nerfstudio pip
-install --upgrade pip setuptools pip install -e . ``` ## 2. Setting up the data
-Download the original NeRF Blender dataset. We support the major datasets and
-allow users to create their own dataset, described in detail [here](https://
-docs.nerf.studio/en/latest/quickstart/custom_dataset.html). ```bash ns-
-download-data --dataset=blender ns-download-data --dataset=nerfstudio --
-capture=poster ``` ### 2.x Using custom data If you have custom data in the
-form of a video or folder of images, we've provided some [COLMAP](https://
-colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to
-help you process your data so it is compatible with nerfstudio. After
-installing both software, you can process your data via: ```bash ns-process-
-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir
-{PROCESSED_DATA_DIR} # Or if you're on a system without an attached display
-(i.e. colab): ns-process-data {video,images,insta360,record3d} --data
-{DATA_PATH} --output-dir {PROCESSED_DATA_DIR} --no-gpu ``` ## 3. Training a
-model To run with all the defaults, e.g., vanilla NeRF method with the Blender
-Lego image ```bash # To see what models are available. ns-train --help # To see
-what model-specific cli arguments are available. ns-train nerfacto --help # Run
-with nerfacto model. ns-train nerfacto # We provide support for other models.
-E.g., to run instant-ngp. ns-train instant-ngp # To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR} ``` ### 3.x Training a model with
-the viewer You can visualize training in real-time using our web-based viewer.
-Make sure to forward a port for the websocket to localhost. The default port is
-7007, which you should expose to localhost:7007. ```bash # with the default
-port ns-train nerfacto --vis viewer # with a specified websocket port ns-train
-nerfacto --vis viewer --viewer.websocket-port=7008 # port forward if running on
-remote ssh -L localhost:7008:localhost:7008 {REMOTE HOST} ``` For more details
-on how to interact with the visualizer, please visit our viewer [walk-through]
-(https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html). ## 4.
-Rendering a trajectory during inference After your model has trained, you can
-headlessly render out a video of the scene with a pre-defined trajectory.
-```bash # assuming previously ran `ns-train nerfacto` ns-render --load-
-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --
-traj=spiral --output-path=renders/output.mp4 ``` # Learn More And that's it for
-getting started with the basics of nerfstudio. If you're interested in learning
-more on how to create your own pipelines, develop with the viewer, run
-benchmarks, and more, please check out some of the quicklinks below or visit
-our [documentation](https://docs.nerf.studio/en/latest/) directly. | Section |
-Description | | ---------------------------------------------------------------
------------------------------------ | -----------------------------------------
---------------------------------------------------------- | | [Documentation]
-(https://docs.nerf.studio/en/latest/) | Full API documentation and tutorials |
-| [Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
+whl/torch_stable.html pip install ninja git+https://github.com/NVlabs/tiny-
+cuda-nn/#subdirectory=bindings/torch ``` For CUDA 11.7: ```bash pip install
+torch==1.13.1 torchvision functorch --extra-index-url https://
+download.pytorch.org/whl/cu117 pip install ninja git+https://github.com/NVlabs/
+tiny-cuda-nn/#subdirectory=bindings/torch ``` See [Dependencies](https://
+github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/
+installation.md#dependencies) in the Installation documentation for more. ###
+Installing nerfstudio Easy option: ```bash pip install nerfstudio ``` **OR** if
+you want the latest and greatest: ```bash git clone https://github.com/
+nerfstudio-project/nerfstudio.git cd nerfstudio pip install --upgrade pip
+setuptools pip install -e . ``` **OR** if you want to skip all installation
+steps and directly start using nerfstudio, use the docker image: See
+[Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/
+quickstart/installation.md) - **Use docker image**. ## 2. Training your first
+model! The following will train a _nerfacto_ model, our recommended model for
+real world scenes. ```bash # Download some test data: ns-download-data
+nerfstudio --capture-name=poster # Train model ns-train nerfacto --data data/
+nerfstudio/poster ``` If everything works, you should see training progress
+like the following:
+                                    [image]
+Navigating to the link at the end of the terminal will load the webviewer. If
+you are running on a remote machine, you will need to port forward the
+websocket port (defaults to 7007).
+                                    [image]
+### Resume from checkpoint / visualize existing run It is possible to load a
+pretrained model by running ```bash ns-train nerfacto --data data/nerfstudio/
+poster --load-dir {outputs/.../nerfstudio_models} ``` This will automatically
+start training. If you do not want it to train, add `--viewer.start-train
+False` to your training command. ## 3. Exporting Results Once you have a NeRF
+model you can either render out a video or export a point cloud. ### Render
+Video First we must create a path for the camera to follow. This can be done in
+the viewer under the "RENDER" tab. Orient your 3D view to the location where
+you wish the video to start, then press "ADD CAMERA". This will set the first
+camera key frame. Continue to new viewpoints adding additional cameras to
+create the camera path. We provide other parameters to further refine your
+camera path. Once satisfied, press "RENDER" which will display a modal that
+contains the command needed to render the video. Kill the training job (or
+create a new terminal if you have lots of compute) and run the command to
+generate the video. Other video export options are available, learn more by
+running ```bash ns-render --help ``` ### Generate Point Cloud While NeRF models
+are not designed to generate point clouds, it is still possible. Navigate to
+the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option
+is selected, everything in the yellow square will be exported into a point
+cloud. Modify the settings as desired then run the command at the bottom of the
+panel in your command line. Alternatively you can use the CLI without the
+viewer. Learn about the export options by running ```bash ns-export pointcloud
+--help ``` ## 4. Using Custom Data Using an existing dataset is great, but
+likely you want to use your own data! We support various methods for using your
+own data. Before it can be used in nerfstudio, the camera location and
+orientations must be determined and then converted into our format using `ns-
+process-data`. We rely on external tools for this, instructions and information
+can be found in the documentation. | Data | Capture Device | Requirements |
+`ns-process-data` Speed | | ---------------------------------------------------
+------------------------------------------------- | -------------- | ----------
+------------------------------------------------------- | ---------------------
+-- | | ð· [Images](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#images-and-video) | Any | [COLMAP](https://
+colmap.github.io/install.html) | ð¢ | | ð¹ [Video](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video) |
+Any | [COLMAP](https://colmap.github.io/install.html) | ð¢ | | ð [360
+Data](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#360_data) | Any | [COLMAP](https://colmap.github.io/
+install.html) | ð¢ | | ð± [Polycam](https://docs.nerf.studio/en/latest/
+quickstart/custom_dataset.html#polycam-capture) | IOS with LiDAR | [Polycam
+App](https://poly.cam/) | ð | | ð± [KIRI Engine](https://docs.nerf.studio/
+en/latest/quickstart/custom_dataset.html#kiri-capture) | IOS or Android | [KIRI
+Engine App](https://www.kiriengine.com/) | ð | | ð± [Record3D](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture) |
+IOS with LiDAR | [Record3D app](https://record3d.app/) | ð | | ð¥
+[Metashape](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#metashape) | Any | [Metashape](https://www.agisoft.com/) |
+ð | | ð¥ [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#realitycapture) | Any | [RealityCapture](https://
+www.capturingreality.com/realitycapture) | ð | | ð  [Custom](https://
+docs.nerf.studio/en/latest/quickstart/data_conventions.html) | Any | Camera
+Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
+We provide other models than nerfacto, for example if you want to train the
+original nerf model, use the following command ```bash ns-train vanilla-nerf --
+data DATA_PATH ``` For a full list of included models run `ns-train --help`.
+### Modify Configuration Each model contains many parameters that can be
+changed, too many to list here. Use the `--help` command to see the full list
+of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
+/ WandB We support three different methods to track training progress, using
+the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
+and Biases](https://wandb.ai/site). You can specify which visualizer to use by
+appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
+that only one may be used at a time. Additionally the viewer only works for
+methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
+NeRF, use the other loggers. # Learn More And that's it for getting started
+with the basics of nerfstudio. If you're interested in learning more on how to
+create your own pipelines, develop with the viewer, run benchmarks, and more,
+please check out some of the quicklinks below or visit our [documentation]
+(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+-------------------------------------------------------------------------------
+---------------- | ------------------------------------------------------------
+-------------------------------------- | | [Documentation](https://
+docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
+[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
 **Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
 nerfology/methods/index.html) | Description of all the models supported by
 nerfstudio and explanations of component parts. | | [Component Descriptions]
 (https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
 Interactive notebooks that explain notable/commonly used modules in various
 models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
 en/latest/quickstart/installation.html) | A more in-depth guide on how to get
@@ -109,31 +162,31 @@
 implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
 latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
 it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
 reference/contributing.html) | Walk-through for how you can start contributing
 now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
 our community to discuss more. We would love to hear from you! | | [Twitter]
 (https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | | [TikTok](#) | Coming soon! Follow us on
-TikTok to see some of our fan favorite results | # Supported Features We
-provide the following support structures to make life easier for getting
-started with NeRFs. For a full description, please refer to our [features page]
-(#). **If you are looking for a feature that is not currently supported, please
-do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/
-uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you to: -
-Visualize training in real-time + interact with the scene - Create and render
-out scenes with custom camera trajectories - View different output types - And
-more! - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb),
-code profiling, and other built-in debugging tools - :chart_with_upwards_trend:
-Easy-to-use benchmarking scripts on the Blender dataset - :iphone: Full
-pipeline support (w/ Colmap or Record3D) for going from a video on your phone
-to a full 3D render. # Built On [tyro_logo] - Easy-to-use config system -
-Developed by [Brent Yi](https://brentyi.com/) [tyro_logo] - Library for
-accelerating NeRF renders - Developed by [Ruilong Li](https://www.liruilong.cn/
-) # Citation If you use this library or find the documentation useful for your
-research, please consider citing: ``` @misc{nerfstudio, title={Nerfstudio: A
-Framework for Neural Radiance Field Development}, author={Matthew Tancik*,
-Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi, Terrance Wang, Alexander
-Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister,
-Angjoo Kanazawa}, year={2022}, url={https://github.com/nerfstudio-project/
-nerfstudio}, } ``` # Contributors [https://contrib.rocks/image?repo=nerfstudio-
-project/nerfstudio]
+see cool updates and announcements | # Supported Features We provide the
+following support structures to make life easier for getting started with
+NeRFs. **If you are looking for a feature that is not currently supported,
+please do not hesitate to contact the Nerfstudio Team on [Discord](https://
+discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
+to: - Visualize training in real-time + interact with the scene - Create and
+render out scenes with custom camera trajectories - View different output types
+- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
+Wandb), code profiling, and other built-in debugging tools - :
+chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
+dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
+going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
+Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
+logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
+(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
+framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
+or find the documentation useful for your research, please consider citing: ```
+@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
+and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
+Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
+and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, journal = {arXiv preprint
+arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.1.9/README.md` & `nerfstudio-0.2.0/nerfstudio.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: nerfstudio
+Version: 0.2.0
+Summary: All-in-one repository for state-of-the-art NeRFs
+License: Apache 2.0
+Project-URL: Documentation, https://docs.nerf.studio
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7.3
+Description-Content-Type: text/markdown
+Provides-Extra: gen
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 <p align="center">
     <!-- community badges -->
     <a href="https://discord.gg/uMbNqcraFc"><img src="https://img.shields.io/badge/Join-Discord-blue.svg"/></a>
     <!-- doc badges -->
     <a href='https://plenoptix-nerfstudio.readthedocs-hosted.com/en/latest/?badge=latest'>
         <img src='https://readthedocs.com/projects/plenoptix-nerfstudio/badge/?version=latest' alt='Documentation Status' />
     </a>
@@ -69,122 +84,165 @@
 The quickstart will help you get started with the default vanilla NeRF trained on the classic Blender Lego scene.
 For more complex changes (e.g., running with your own data/setting up a new NeRF graph, please refer to our [references](#learn-more).
 
 ## 1. Installation: Setup the environment
 
 ### Prerequisites
 
-CUDA must be installed on the system. This library has been tested with version 11.3. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
+You must have an NVIDIA video card with CUDA installed on the system. This library has been tested with version 11.3 of CUDA. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
 
 ### Create environment
 
 Nerfstudio requires `python >= 3.7`. We recommend using conda to manage dependencies. Make sure to install [Conda](https://docs.conda.io/en/latest/miniconda.html) before proceeding.
 
 ```bash
 conda create --name nerfstudio -y python=3.8
 conda activate nerfstudio
 python -m pip install --upgrade pip
 ```
 
 ### Dependencies
 
-Install pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+Install pytorch with CUDA (this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+
+For CUDA 11.3:
 
 ```bash
 pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/whl/torch_stable.html
-pip install git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+```
+
+For CUDA 11.7:
+
+```bash
+pip install torch==1.13.1 torchvision functorch --extra-index-url https://download.pytorch.org/whl/cu117
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
 ```
 
+See [Dependencies](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md#dependencies)
+in the Installation documentation for more.
+
 ### Installing nerfstudio
 
 Easy option:
 
 ```bash
 pip install nerfstudio
 ```
 
-If you want the latest and greatest:
+**OR** if you want the latest and greatest:
 
 ```bash
 git clone https://github.com/nerfstudio-project/nerfstudio.git
 cd nerfstudio
 pip install --upgrade pip setuptools
 pip install -e .
 ```
 
-## 2. Setting up the data
+**OR** if you want to skip all installation steps and directly start using nerfstudio, use the docker image:
+
+See [Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md) - **Use docker image**.
 
-Download the original NeRF Blender dataset. We support the major datasets and allow users to create their own dataset, described in detail [here](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html).
+## 2. Training your first model!
+
+The following will train a _nerfacto_ model, our recommended model for real world scenes.
 
 ```bash
-ns-download-data --dataset=blender
-ns-download-data --dataset=nerfstudio --capture=poster
+# Download some test data:
+ns-download-data nerfstudio --capture-name=poster
+# Train model
+ns-train nerfacto --data data/nerfstudio/poster
 ```
 
-### 2.x Using custom data
+If everything works, you should see training progress like the following:
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766069-cadfd34f-8833-4156-88b7-ad406d688fc0.png">
+</p>
+
+Navigating to the link at the end of the terminal will load the webviewer. If you are running on a remote machine, you will need to port forward the websocket port (defaults to 7007).
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766653-586a0daa-466b-4140-a136-6b02f2ce2c54.png">
+</p>
 
-If you have custom data in the form of a video or folder of images, we've provided some [COLMAP](https://colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to help you process your data so it is compatible with nerfstudio.
+### Resume from checkpoint / visualize existing run
 
-After installing both software, you can process your data via:
+It is possible to load a pretrained model by running
 
 ```bash
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir {PROCESSED_DATA_DIR}
-# Or if you're on a system without an attached display (i.e. colab):
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH}  --output-dir {PROCESSED_DATA_DIR} --no-gpu
+ns-train nerfacto --data data/nerfstudio/poster --load-dir {outputs/.../nerfstudio_models}
 ```
 
-## 3. Training a model
+This will automatically start training. If you do not want it to train, add `--viewer.start-train False` to your training command.
 
-To run with all the defaults, e.g., vanilla NeRF method with the Blender Lego image
+## 3. Exporting Results
 
-```bash
-# To see what models are available.
-ns-train --help
+Once you have a NeRF model you can either render out a video or export a point cloud.
 
-# To see what model-specific cli arguments are available.
-ns-train nerfacto --help
+### Render Video
 
-# Run with nerfacto model.
-ns-train nerfacto
+First we must create a path for the camera to follow. This can be done in the viewer under the "RENDER" tab. Orient your 3D view to the location where you wish the video to start, then press "ADD CAMERA". This will set the first camera key frame. Continue to new viewpoints adding additional cameras to create the camera path. We provide other parameters to further refine your camera path. Once satisfied, press "RENDER" which will display a modal that contains the command needed to render the video. Kill the training job (or create a new terminal if you have lots of compute) and run the command to generate the video.
 
-# We provide support for other models. E.g., to run instant-ngp.
-ns-train instant-ngp
+Other video export options are available, learn more by running
 
-# To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR}
+```bash
+ns-render --help
 ```
 
-### 3.x Training a model with the viewer
+### Generate Point Cloud
 
-You can visualize training in real-time using our web-based viewer.
+While NeRF models are not designed to generate point clouds, it is still possible. Navigate to the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option is selected, everything in the yellow square will be exported into a point cloud. Modify the settings as desired then run the command at the bottom of the panel in your command line.
 
-Make sure to forward a port for the websocket to localhost. The default port is 7007, which you should expose to localhost:7007.
+Alternatively you can use the CLI without the viewer. Learn about the export options by running
 
 ```bash
-# with the default port
-ns-train nerfacto --vis viewer
+ns-export pointcloud --help
+```
+
+## 4. Using Custom Data
+
+Using an existing dataset is great, but likely you want to use your own data! We support various methods for using your own data. Before it can be used in nerfstudio, the camera location and orientations must be determined and then converted into our format using `ns-process-data`. We rely on external tools for this, instructions and information can be found in the documentation.
+
+| Data                                                                                                 | Capture Device | Requirements                                                      | `ns-process-data` Speed |
+| ---------------------------------------------------------------------------------------------------- | -------------- | ----------------------------------------------------------------- | ----------------------- |
+| 📷 [Images](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)      | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📹 [Video](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)       | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 🌎 [360 Data](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#360_data)            | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📱 [Polycam](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#polycam-capture)      | IOS with LiDAR | [Polycam App](https://poly.cam/)                                  | 🐇                      |
+| 📱 [KIRI Engine](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#kiri-capture)     | IOS or Android | [KIRI Engine App](https://www.kiriengine.com/)                    | 🐇                      |
+| 📱 [Record3D](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture)    | IOS with LiDAR | [Record3D app](https://record3d.app/)                             | 🐇                      |
+| 🖥 [Metashape](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#metashape)           | Any            | [Metashape](https://www.agisoft.com/)                             | 🐇                      |
+| 🖥 [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#realitycapture) | Any            | [RealityCapture](https://www.capturingreality.com/realitycapture) | 🐇                      |
+| 🛠 [Custom](https://docs.nerf.studio/en/latest/quickstart/data_conventions.html)                      | Any            | Camera Poses                                                      | 🐇                      |
 
-# with a specified websocket port
-ns-train nerfacto --vis viewer --viewer.websocket-port=7008
+## 5. Advanced Options
 
-# port forward if running on remote
-ssh -L localhost:7008:localhost:7008 {REMOTE HOST}
+### Training models other than nerfacto
+
+We provide other models than nerfacto, for example if you want to train the original nerf model, use the following command
+
+```bash
+ns-train vanilla-nerf --data DATA_PATH
 ```
 
-For more details on how to interact with the visualizer, please visit our viewer [walk-through](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html).
+For a full list of included models run `ns-train --help`.
 
-## 4. Rendering a trajectory during inference
+### Modify Configuration
 
-After your model has trained, you can headlessly render out a video of the scene with a pre-defined trajectory.
+Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
-# assuming previously ran `ns-train nerfacto`
-ns-render --load-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --traj=spiral --output-path=renders/output.mp4
+ns-train nerfacto --help
 ```
 
+### Tensorboard / WandB
+
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
 
 | Section                                                                                            | Description                                                                                        |
@@ -201,30 +259,29 @@
 | 💻 **For Developers**                                                                              |
 | [Creating pipelines](https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html)     | Learn how to easily build new neural rendering pipelines by using and/or implementing new modules. |
 | [Creating datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html)             | Have a new dataset? Learn how to run it with nerfstudio.                                           |
 | [Contributing](https://docs.nerf.studio/en/latest/reference/contributing.html)                     | Walk-through for how you can start contributing now.                                               |
 | 💖 **Community**                                                                                   |
 | [Discord](https://discord.gg/uMbNqcraFc)                                                           | Join our community to discuss more. We would love to hear from you!                                |
 | [Twitter](https://twitter.com/nerfstudioteam)                                                      | Follow us on Twitter @nerfstudioteam to see cool updates and announcements                         |
-| [TikTok](#)                                                                                        | Coming soon! Follow us on TikTok to see some of our fan favorite results                           |
 
 # Supported Features
 
-We provide the following support structures to make life easier for getting started with NeRFs. For a full description, please refer to our [features page](#).
+We provide the following support structures to make life easier for getting started with NeRFs.
 
 **If you are looking for a feature that is not currently supported, please do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/uMbNqcraFc)!**
 
 - :mag_right: Web-based visualizer that allows you to:
   - Visualize training in real-time + interact with the scene
   - Create and render out scenes with custom camera trajectories
   - View different output types
   - And more!
 - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb), code profiling, and other built-in debugging tools
 - :chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender dataset
-- :iphone: Full pipeline support (w/ Colmap or Record3D) for going from a video on your phone to a full 3D render.
+- :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for going from a video on your phone to a full 3D render.
 
 # Built On
 
 <a href="https://github.com/brentyi/tyro">
     <img alt="tyro logo" src="https://brentyi.github.io/tyro/_static/logo-light.svg" width="150px" />
 </a>
 
@@ -236,24 +293,26 @@
 </a>
 
 - Library for accelerating NeRF renders
 - Developed by [Ruilong Li](https://www.liruilong.cn/)
 
 # Citation
 
+You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
+
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@misc{nerfstudio,
-      title={Nerfstudio: A Framework for Neural Radiance Field Development},
-      author={Matthew Tancik*, Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi,
-              Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi,
-              Abhik Ahuja, David McAllister, Angjoo Kanazawa},
-      year={2022},
-      url={https://github.com/nerfstudio-project/nerfstudio},
+@article{nerfstudio,
+    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
+            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
+    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+    journal = {arXiv preprint arXiv:2302.04264},
+    year = {2023},
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1 Name: nerfstudio Version: 0.2.0 Summary: All-in-one
+repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
+Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
+Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
+Description-Content-Type: text/markdown Provides-Extra: gen Provides-Extra: dev
+Provides-Extra: docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
                                  [nerfstudio]
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
@@ -25,71 +31,124 @@
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
 nerfstudio enables you to build faster :hammer: learn together :books: and
 contribute to our NeRF community :sparkling_heart:. # Quickstart The quickstart
 will help you get started with the default vanilla NeRF trained on the classic
 Blender Lego scene. For more complex changes (e.g., running with your own data/
 setting up a new NeRF graph, please refer to our [references](#learn-more). ##
-1. Installation: Setup the environment ### Prerequisites CUDA must be installed
-on the system. This library has been tested with version 11.3. You can find
-more information about installing CUDA [here](https://docs.nvidia.com/cuda/
-cuda-quick-start-guide/index.html) ### Create environment Nerfstudio requires
-`python >= 3.7`. We recommend using conda to manage dependencies. Make sure to
-install [Conda](https://docs.conda.io/en/latest/miniconda.html) before
-proceeding. ```bash conda create --name nerfstudio -y python=3.8 conda activate
-nerfstudio python -m pip install --upgrade pip ``` ### Dependencies Install
-pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn]
-(https://github.com/NVlabs/tiny-cuda-nn) ```bash pip install
+1. Installation: Setup the environment ### Prerequisites You must have an
+NVIDIA video card with CUDA installed on the system. This library has been
+tested with version 11.3 of CUDA. You can find more information about
+installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/
+index.html) ### Create environment Nerfstudio requires `python >= 3.7`. We
+recommend using conda to manage dependencies. Make sure to install [Conda]
+(https://docs.conda.io/en/latest/miniconda.html) before proceeding. ```bash
+conda create --name nerfstudio -y python=3.8 conda activate nerfstudio python -
+m pip install --upgrade pip ``` ### Dependencies Install pytorch with CUDA
+(this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn]
+(https://github.com/NVlabs/tiny-cuda-nn) For CUDA 11.3: ```bash pip install
 torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/
-whl/torch_stable.html pip install git+https://github.com/NVlabs/tiny-cuda-nn/
-#subdirectory=bindings/torch ``` ### Installing nerfstudio Easy option: ```bash
-pip install nerfstudio ``` If you want the latest and greatest: ```bash git
-clone https://github.com/nerfstudio-project/nerfstudio.git cd nerfstudio pip
-install --upgrade pip setuptools pip install -e . ``` ## 2. Setting up the data
-Download the original NeRF Blender dataset. We support the major datasets and
-allow users to create their own dataset, described in detail [here](https://
-docs.nerf.studio/en/latest/quickstart/custom_dataset.html). ```bash ns-
-download-data --dataset=blender ns-download-data --dataset=nerfstudio --
-capture=poster ``` ### 2.x Using custom data If you have custom data in the
-form of a video or folder of images, we've provided some [COLMAP](https://
-colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to
-help you process your data so it is compatible with nerfstudio. After
-installing both software, you can process your data via: ```bash ns-process-
-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir
-{PROCESSED_DATA_DIR} # Or if you're on a system without an attached display
-(i.e. colab): ns-process-data {video,images,insta360,record3d} --data
-{DATA_PATH} --output-dir {PROCESSED_DATA_DIR} --no-gpu ``` ## 3. Training a
-model To run with all the defaults, e.g., vanilla NeRF method with the Blender
-Lego image ```bash # To see what models are available. ns-train --help # To see
-what model-specific cli arguments are available. ns-train nerfacto --help # Run
-with nerfacto model. ns-train nerfacto # We provide support for other models.
-E.g., to run instant-ngp. ns-train instant-ngp # To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR} ``` ### 3.x Training a model with
-the viewer You can visualize training in real-time using our web-based viewer.
-Make sure to forward a port for the websocket to localhost. The default port is
-7007, which you should expose to localhost:7007. ```bash # with the default
-port ns-train nerfacto --vis viewer # with a specified websocket port ns-train
-nerfacto --vis viewer --viewer.websocket-port=7008 # port forward if running on
-remote ssh -L localhost:7008:localhost:7008 {REMOTE HOST} ``` For more details
-on how to interact with the visualizer, please visit our viewer [walk-through]
-(https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html). ## 4.
-Rendering a trajectory during inference After your model has trained, you can
-headlessly render out a video of the scene with a pre-defined trajectory.
-```bash # assuming previously ran `ns-train nerfacto` ns-render --load-
-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --
-traj=spiral --output-path=renders/output.mp4 ``` # Learn More And that's it for
-getting started with the basics of nerfstudio. If you're interested in learning
-more on how to create your own pipelines, develop with the viewer, run
-benchmarks, and more, please check out some of the quicklinks below or visit
-our [documentation](https://docs.nerf.studio/en/latest/) directly. | Section |
-Description | | ---------------------------------------------------------------
------------------------------------ | -----------------------------------------
---------------------------------------------------------- | | [Documentation]
-(https://docs.nerf.studio/en/latest/) | Full API documentation and tutorials |
-| [Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
+whl/torch_stable.html pip install ninja git+https://github.com/NVlabs/tiny-
+cuda-nn/#subdirectory=bindings/torch ``` For CUDA 11.7: ```bash pip install
+torch==1.13.1 torchvision functorch --extra-index-url https://
+download.pytorch.org/whl/cu117 pip install ninja git+https://github.com/NVlabs/
+tiny-cuda-nn/#subdirectory=bindings/torch ``` See [Dependencies](https://
+github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/
+installation.md#dependencies) in the Installation documentation for more. ###
+Installing nerfstudio Easy option: ```bash pip install nerfstudio ``` **OR** if
+you want the latest and greatest: ```bash git clone https://github.com/
+nerfstudio-project/nerfstudio.git cd nerfstudio pip install --upgrade pip
+setuptools pip install -e . ``` **OR** if you want to skip all installation
+steps and directly start using nerfstudio, use the docker image: See
+[Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/
+quickstart/installation.md) - **Use docker image**. ## 2. Training your first
+model! The following will train a _nerfacto_ model, our recommended model for
+real world scenes. ```bash # Download some test data: ns-download-data
+nerfstudio --capture-name=poster # Train model ns-train nerfacto --data data/
+nerfstudio/poster ``` If everything works, you should see training progress
+like the following:
+                                    [image]
+Navigating to the link at the end of the terminal will load the webviewer. If
+you are running on a remote machine, you will need to port forward the
+websocket port (defaults to 7007).
+                                    [image]
+### Resume from checkpoint / visualize existing run It is possible to load a
+pretrained model by running ```bash ns-train nerfacto --data data/nerfstudio/
+poster --load-dir {outputs/.../nerfstudio_models} ``` This will automatically
+start training. If you do not want it to train, add `--viewer.start-train
+False` to your training command. ## 3. Exporting Results Once you have a NeRF
+model you can either render out a video or export a point cloud. ### Render
+Video First we must create a path for the camera to follow. This can be done in
+the viewer under the "RENDER" tab. Orient your 3D view to the location where
+you wish the video to start, then press "ADD CAMERA". This will set the first
+camera key frame. Continue to new viewpoints adding additional cameras to
+create the camera path. We provide other parameters to further refine your
+camera path. Once satisfied, press "RENDER" which will display a modal that
+contains the command needed to render the video. Kill the training job (or
+create a new terminal if you have lots of compute) and run the command to
+generate the video. Other video export options are available, learn more by
+running ```bash ns-render --help ``` ### Generate Point Cloud While NeRF models
+are not designed to generate point clouds, it is still possible. Navigate to
+the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option
+is selected, everything in the yellow square will be exported into a point
+cloud. Modify the settings as desired then run the command at the bottom of the
+panel in your command line. Alternatively you can use the CLI without the
+viewer. Learn about the export options by running ```bash ns-export pointcloud
+--help ``` ## 4. Using Custom Data Using an existing dataset is great, but
+likely you want to use your own data! We support various methods for using your
+own data. Before it can be used in nerfstudio, the camera location and
+orientations must be determined and then converted into our format using `ns-
+process-data`. We rely on external tools for this, instructions and information
+can be found in the documentation. | Data | Capture Device | Requirements |
+`ns-process-data` Speed | | ---------------------------------------------------
+------------------------------------------------- | -------------- | ----------
+------------------------------------------------------- | ---------------------
+-- | | ð· [Images](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#images-and-video) | Any | [COLMAP](https://
+colmap.github.io/install.html) | ð¢ | | ð¹ [Video](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video) |
+Any | [COLMAP](https://colmap.github.io/install.html) | ð¢ | | ð [360
+Data](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#360_data) | Any | [COLMAP](https://colmap.github.io/
+install.html) | ð¢ | | ð± [Polycam](https://docs.nerf.studio/en/latest/
+quickstart/custom_dataset.html#polycam-capture) | IOS with LiDAR | [Polycam
+App](https://poly.cam/) | ð | | ð± [KIRI Engine](https://docs.nerf.studio/
+en/latest/quickstart/custom_dataset.html#kiri-capture) | IOS or Android | [KIRI
+Engine App](https://www.kiriengine.com/) | ð | | ð± [Record3D](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture) |
+IOS with LiDAR | [Record3D app](https://record3d.app/) | ð | | ð¥
+[Metashape](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#metashape) | Any | [Metashape](https://www.agisoft.com/) |
+ð | | ð¥ [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#realitycapture) | Any | [RealityCapture](https://
+www.capturingreality.com/realitycapture) | ð | | ð  [Custom](https://
+docs.nerf.studio/en/latest/quickstart/data_conventions.html) | Any | Camera
+Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
+We provide other models than nerfacto, for example if you want to train the
+original nerf model, use the following command ```bash ns-train vanilla-nerf --
+data DATA_PATH ``` For a full list of included models run `ns-train --help`.
+### Modify Configuration Each model contains many parameters that can be
+changed, too many to list here. Use the `--help` command to see the full list
+of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
+/ WandB We support three different methods to track training progress, using
+the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
+and Biases](https://wandb.ai/site). You can specify which visualizer to use by
+appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
+that only one may be used at a time. Additionally the viewer only works for
+methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
+NeRF, use the other loggers. # Learn More And that's it for getting started
+with the basics of nerfstudio. If you're interested in learning more on how to
+create your own pipelines, develop with the viewer, run benchmarks, and more,
+please check out some of the quicklinks below or visit our [documentation]
+(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+-------------------------------------------------------------------------------
+---------------- | ------------------------------------------------------------
+-------------------------------------- | | [Documentation](https://
+docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
+[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
 **Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
 nerfology/methods/index.html) | Description of all the models supported by
 nerfstudio and explanations of component parts. | | [Component Descriptions]
 (https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
 Interactive notebooks that explain notable/commonly used modules in various
 models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
 en/latest/quickstart/installation.html) | A more in-depth guide on how to get
@@ -103,31 +162,31 @@
 implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
 latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
 it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
 reference/contributing.html) | Walk-through for how you can start contributing
 now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
 our community to discuss more. We would love to hear from you! | | [Twitter]
 (https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | | [TikTok](#) | Coming soon! Follow us on
-TikTok to see some of our fan favorite results | # Supported Features We
-provide the following support structures to make life easier for getting
-started with NeRFs. For a full description, please refer to our [features page]
-(#). **If you are looking for a feature that is not currently supported, please
-do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/
-uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you to: -
-Visualize training in real-time + interact with the scene - Create and render
-out scenes with custom camera trajectories - View different output types - And
-more! - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb),
-code profiling, and other built-in debugging tools - :chart_with_upwards_trend:
-Easy-to-use benchmarking scripts on the Blender dataset - :iphone: Full
-pipeline support (w/ Colmap or Record3D) for going from a video on your phone
-to a full 3D render. # Built On [tyro_logo] - Easy-to-use config system -
-Developed by [Brent Yi](https://brentyi.com/) [tyro_logo] - Library for
-accelerating NeRF renders - Developed by [Ruilong Li](https://www.liruilong.cn/
-) # Citation If you use this library or find the documentation useful for your
-research, please consider citing: ``` @misc{nerfstudio, title={Nerfstudio: A
-Framework for Neural Radiance Field Development}, author={Matthew Tancik*,
-Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi, Terrance Wang, Alexander
-Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister,
-Angjoo Kanazawa}, year={2022}, url={https://github.com/nerfstudio-project/
-nerfstudio}, } ``` # Contributors [https://contrib.rocks/image?repo=nerfstudio-
-project/nerfstudio]
+see cool updates and announcements | # Supported Features We provide the
+following support structures to make life easier for getting started with
+NeRFs. **If you are looking for a feature that is not currently supported,
+please do not hesitate to contact the Nerfstudio Team on [Discord](https://
+discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
+to: - Visualize training in real-time + interact with the scene - Create and
+render out scenes with custom camera trajectories - View different output types
+- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
+Wandb), code profiling, and other built-in debugging tools - :
+chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
+dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
+going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
+Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
+logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
+(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
+framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
+or find the documentation useful for your research, please consider citing: ```
+@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
+and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
+Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
+and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, journal = {arXiv preprint
+arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.1.9/nerfstudio/__init__.py` & `nerfstudio-0.2.0/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/__init__.py` & `nerfstudio-0.2.0/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-0.2.0/nerfstudio/cameras/camera_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,25 @@
 import torch
 import tyro
 from torch import nn
 from torchtyping import TensorType
 from typing_extensions import Literal, assert_never
 
 from nerfstudio.cameras.lie_groups import exp_map_SE3, exp_map_SO3xR3
-from nerfstudio.configs import base_config as cfg
+from nerfstudio.configs.base_config import InstantiateConfig
 from nerfstudio.engine.optimizers import AdamOptimizerConfig
-from nerfstudio.engine.schedulers import SchedulerConfig
+from nerfstudio.engine.schedulers import (
+    ExponentialDecaySchedulerConfig,
+    SchedulerConfig,
+)
 from nerfstudio.utils import poses as pose_utils
 
 
 @dataclass
-class CameraOptimizerConfig(cfg.InstantiateConfig):
+class CameraOptimizerConfig(InstantiateConfig):
     """Configuration of optimization for camera poses."""
 
     _target: Type = field(default_factory=lambda: CameraOptimizer)
 
     mode: Literal["off", "SO3xR3", "SE3"] = "off"
     """Pose optimization strategy to use. If enabled, we recommend SO3xR3."""
 
@@ -49,15 +52,15 @@
 
     orientation_noise_std: float = 0.0
     """Noise to add to initial orientations. Useful for debugging."""
 
     optimizer: AdamOptimizerConfig = AdamOptimizerConfig(lr=6e-4, eps=1e-15)
     """ADAM parameters for camera optimization."""
 
-    scheduler: SchedulerConfig = SchedulerConfig(max_steps=10000)
+    scheduler: SchedulerConfig = ExponentialDecaySchedulerConfig(max_steps=10000)
     """Learning rate scheduler for camera optimizer.."""
 
     param_group: tyro.conf.Suppress[str] = "camera_opt"
     """Name of the parameter group used for pose optimization. Can be any string that doesn't conflict with other
     groups."""
 
 
@@ -100,15 +103,15 @@
         self,
         indices: TensorType["num_cameras"],
     ) -> TensorType["num_cameras", 3, 4]:
         """Indexing into camera adjustments.
         Args:
             indices: indices of Cameras to optimize.
         Returns:
-            Tranformation matrices from optimized camera coordinates coordinates
+            Transformation matrices from optimized camera coordinates
             to given camera coordinates.
         """
         outputs = []
 
         # Apply learned transformation delta.
         if self.config.mode == "off":
             pass
```

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/camera_paths.py` & `nerfstudio-0.2.0/nerfstudio/cameras/camera_paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 from typing import Any, Dict, Optional, Tuple
 
 import torch
 
 import nerfstudio.utils.poses as pose_utils
 from nerfstudio.cameras import camera_utils
 from nerfstudio.cameras.camera_utils import get_interpolated_poses_many
-from nerfstudio.cameras.cameras import Cameras
+from nerfstudio.cameras.cameras import Cameras, CameraType
 from nerfstudio.viewer.server.utils import three_js_perspective_camera_focal_length
 
 
 def get_interpolated_camera_path(cameras: Cameras, steps: int) -> Cameras:
     """Generate a camera path between two cameras.
 
     Args:
         cameras: Cameras object containing intrinsics of all cameras.
         steps: The number of steps to interpolate between the two cameras.
 
     Returns:
         A new set of cameras along a path.
     """
     Ks = cameras.get_intrinsics_matrices().cpu().numpy()
-    poses = cameras.camera_to_worlds().cpu().numpy()
+    poses = cameras.camera_to_worlds.cpu().numpy()
     poses, Ks = get_interpolated_poses_many(poses, Ks, steps_per_transition=steps)
 
     cameras = Cameras(fx=Ks[:, 0, 0], fy=Ks[:, 1, 1], cx=Ks[0, 0, 2], cy=Ks[0, 1, 2], camera_to_worlds=poses)
     return cameras
 
 
 def get_spiral_path(
@@ -50,29 +50,30 @@
     steps: int = 30,
     radius: Optional[float] = None,
     radiuses: Optional[Tuple[float]] = None,
     rots: int = 2,
     zrate: float = 0.5,
 ) -> Cameras:
     """
-    Returns a list of camera in a sprial trajectory.
+    Returns a list of camera in a spiral trajectory.
 
     Args:
         camera: The camera to start the spiral from.
         steps: The number of cameras in the generated path.
         radius: The radius of the spiral for all xyz directions.
         radiuses: The list of radii for the spiral in xyz directions.
         rots: The number of rotations to apply to the camera.
         zrate: How much to change the z position of the camera.
 
     Returns:
         A spiral camera path.
     """
 
     assert radius is not None or radiuses is not None, "Either radius or radiuses must be specified."
+    assert camera.ndim == 1, "We assume only one batch dim here"
     if radius is not None and radiuses is None:
         rad = torch.tensor([radius] * 3, device=camera.device)
     elif radiuses is not None and radius is None:
         rad = torch.tensor(radiuses, device=camera.device)
     else:
         raise ValueError("Only one of radius or radiuses must be specified.")
 
@@ -95,15 +96,25 @@
 
     new_c2ws = []
     for local_c2wh in local_c2whs:
         c2wh = torch.matmul(c2wh_global, local_c2wh)
         new_c2ws.append(c2wh[:3, :4])
     new_c2ws = torch.stack(new_c2ws, dim=0)
 
-    return Cameras(fx=camera.fx[0], fy=camera.fy[0], cx=camera.cx[0], cy=camera.cy[0], camera_to_worlds=new_c2ws)
+    times = None
+    if camera.times is not None:
+        times = torch.linspace(0, 1, steps)[:, None]
+    return Cameras(
+        fx=camera.fx[0],
+        fy=camera.fy[0],
+        cx=camera.cx[0],
+        cy=camera.cy[0],
+        camera_to_worlds=new_c2ws,
+        times=times,
+    )
 
 
 def get_path_from_json(camera_path: Dict[str, Any]) -> Cameras:
     """Takes a camera path dictionary and returns a trajectory as a Camera instance.
 
     Args:
         camera_path: A dictionary of the camera path information coming from the viewer.
@@ -111,30 +122,51 @@
     Returns:
         A Cameras instance with the camera path.
     """
 
     image_height = camera_path["render_height"]
     image_width = camera_path["render_width"]
 
+    if "camera_type" not in camera_path:
+        camera_type = CameraType.PERSPECTIVE
+    elif camera_path["camera_type"] == "fisheye":
+        camera_type = CameraType.FISHEYE
+    elif camera_path["camera_type"] == "equirectangular":
+        camera_type = CameraType.EQUIRECTANGULAR
+    else:
+        camera_type = CameraType.PERSPECTIVE
+
     c2ws = []
     fxs = []
     fys = []
     for camera in camera_path["camera_path"]:
         # pose
         c2w = torch.tensor(camera["camera_to_world"]).view(4, 4)[:3]
         c2ws.append(c2w)
-        # field of view
-        fov = camera["fov"]
-        focal_length = three_js_perspective_camera_focal_length(fov, image_height)
-        fxs.append(focal_length)
-        fys.append(focal_length)
+        if camera_type == CameraType.EQUIRECTANGULAR:
+            fxs.append(image_width / 2)
+            fys.append(image_height)
+        else:
+            # field of view
+            fov = camera["fov"]
+            focal_length = three_js_perspective_camera_focal_length(fov, image_height)
+            fxs.append(focal_length)
+            fys.append(focal_length)
+
+    # Iff ALL cameras in the path have a "time" value, construct Cameras with times
+    if all("render_time" in camera for camera in camera_path["camera_path"]):
+        times = torch.tensor([camera["render_time"] for camera in camera_path["camera_path"]])
+    else:
+        times = None
 
     camera_to_worlds = torch.stack(c2ws, dim=0)
     fx = torch.tensor(fxs)
     fy = torch.tensor(fys)
     return Cameras(
         fx=fx,
         fy=fy,
         cx=image_width / 2,
         cy=image_height / 2,
         camera_to_worlds=camera_to_worlds,
+        camera_type=camera_type,
+        times=times,
     )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/camera_utils.py` & `nerfstudio-0.2.0/nerfstudio/cameras/camera_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 """
 
 import math
 from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
+from numpy.typing import ArrayLike
 from torchtyping import TensorType
 from typing_extensions import Literal
 
 _EPS = np.finfo(float).eps * 4.0
 
 
-def unit_vector(data, axis: Optional[int] = None) -> np.ndarray:
+def unit_vector(data: ArrayLike, axis: Optional[int] = None) -> np.ndarray:
     """Return ndarray normalized by length, i.e. Euclidean norm, along axis.
 
     Args:
         axis: the axis along which to normalize into unit vector
         out: where to write out the data to. If None, returns a new np ndarray
     """
     data = np.array(data, dtype=np.float64, copy=True)
@@ -42,15 +43,15 @@
     np.sqrt(length, length)
     if axis is not None:
         length = np.expand_dims(length, axis)
     data /= length
     return data
 
 
-def quaternion_from_matrix(matrix, isprecise: bool = False) -> np.ndarray:
+def quaternion_from_matrix(matrix: ArrayLike, isprecise: bool = False) -> np.ndarray:
     """Return quaternion from rotation matrix.
 
     Args:
         matrix: rotation matrix to obtain quaternion
         isprecise: if True, input matrix is assumed to be precise rotation matrix and a faster algorithm is used.
     """
     M = np.array(matrix, dtype=np.float64, copy=False)[:4, :4]
@@ -98,15 +99,17 @@
         w, V = np.linalg.eigh(K)
         q = V[np.array([3, 0, 1, 2]), np.argmax(w)]
     if q[0] < 0.0:
         np.negative(q, q)
     return q
 
 
-def quaternion_slerp(quat0, quat1, fraction: float, spin: int = 0, shortestpath: bool = True) -> np.ndarray:
+def quaternion_slerp(
+    quat0: ArrayLike, quat1: ArrayLike, fraction: float, spin: int = 0, shortestpath: bool = True
+) -> np.ndarray:
     """Return spherical linear interpolation between two quaternions.
     Args:
         quat0: first quaternion
         quat1: second quaternion
         fraction: how much to interpolate between quat0 vs quat1 (if 0, closer to quat0; if 1, closer to quat1)
         spin: how much of an additional spin to place on the interpolation
         shortestpath: whether to return the short or long path to rotation
@@ -132,15 +135,15 @@
     isin = 1.0 / math.sin(angle)
     q0 *= math.sin((1.0 - fraction) * angle) * isin
     q1 *= math.sin(fraction * angle) * isin
     q0 += q1
     return q0
 
 
-def quaternion_matrix(quaternion) -> np.ndarray:
+def quaternion_matrix(quaternion: ArrayLike) -> np.ndarray:
     """Return homogeneous rotation matrix from quaternion.
 
     Args:
         quaternion: value to convert to matrix
     """
     q = np.array(quaternion, dtype=np.float64, copy=True)
     n = np.dot(q, q)
@@ -154,19 +157,19 @@
             [q[1, 2] + q[3, 0], 1.0 - q[1, 1] - q[3, 3], q[2, 3] - q[1, 0], 0.0],
             [q[1, 3] - q[2, 0], q[2, 3] + q[1, 0], 1.0 - q[1, 1] - q[2, 2], 0.0],
             [0.0, 0.0, 0.0, 1.0],
         ]
     )
 
 
-def get_interpolated_poses(pose_a, pose_b, steps: int = 10) -> List[float]:
+def get_interpolated_poses(pose_a: ArrayLike, pose_b: ArrayLike, steps: int = 10) -> List[float]:
     """Return interpolation of poses with specified number of steps.
     Args:
-        poseA: first pose
-        poseB: second pose
+        pose_a: first pose
+        pose_b: second pose
         steps: number of steps the interpolated pose path should contain
     """
 
     quat_a = quaternion_from_matrix(pose_a[:3, :3])
     quat_b = quaternion_from_matrix(pose_b[:3, :3])
 
     ts = np.linspace(0, 1, steps)
@@ -174,25 +177,25 @@
     trans = [(1 - t) * pose_a[:3, 3] + t * pose_b[:3, 3] for t in ts]
 
     poses_ab = []
     for quat, tran in zip(quats, trans):
         pose = np.identity(4)
         pose[:3, :3] = quaternion_matrix(quat)[:3, :3]
         pose[:3, 3] = tran
-        poses_ab.append(pose)
+        poses_ab.append(pose[:3])
     return poses_ab
 
 
 def get_interpolated_k(k_a, k_b, steps: int = 10) -> TensorType[3, 4]:
     """
     Returns interpolated path between two camera poses with specified number of steps.
 
     Args:
-        KA: camera matrix 1
-        KB: camera matrix 2
+        k_a: camera matrix 1
+        k_b: camera matrix 2
         steps: number of steps the interpolated pose path should contain
     """
     Ks = []
     ts = np.linspace(0, 1, steps)
     for t in ts:
         new_k = k_a * (1.0 - t) + k_b * t
         Ks.append(new_k)
@@ -211,30 +214,49 @@
         Ks: list of camera intrinsics
         steps_per_transition: number of steps per transition
 
     Returns:
         tuple of new poses and intrinsics
     """
     traj = []
-    Ks = []
+    k_interp = []
     for idx in range(poses.shape[0] - 1):
         pose_a = poses[idx]
         pose_b = poses[idx + 1]
         poses_ab = get_interpolated_poses(pose_a, pose_b, steps=steps_per_transition)
         traj += poses_ab
-        Ks += get_interpolated_k(Ks[idx], Ks[idx + 1], steps_per_transition)
-    return torch.stack(traj, dim=0), torch.stack(Ks, dim=0)
+        k_interp += get_interpolated_k(Ks[idx], Ks[idx + 1], steps=steps_per_transition)
+
+    traj = np.stack(traj, axis=0)
+    k_interp = np.stack(k_interp, axis=0)
+
+    return torch.tensor(traj, dtype=torch.float32), torch.tensor(k_interp, dtype=torch.float32)
 
 
-def normalize(x) -> TensorType[...]:
+def normalize(x: torch.Tensor) -> TensorType[...]:
     """Returns a normalized vector."""
     return x / torch.linalg.norm(x)
 
 
-def viewmatrix(lookat, up, pos) -> TensorType[...]:
+def normalize_with_norm(x: torch.Tensor, dim: int) -> Tuple[torch.Tensor, torch.Tensor]:
+    """Normalize tensor along axis and return normalized value with norms.
+
+    Args:
+        x: tensor to normalize.
+        dim: axis along which to normalize.
+
+    Returns:
+        Tuple of normalized tensor and corresponding norm.
+    """
+
+    norm = torch.maximum(torch.linalg.vector_norm(x, dim=dim, keepdims=True), torch.tensor([_EPS]).to(x))
+    return x / norm, norm
+
+
+def viewmatrix(lookat: torch.Tensor, up: torch.Tensor, pos: torch.Tensor) -> TensorType[...]:
     """Returns a camera transformation matrix.
 
     Args:
         lookat: The direction the camera is looking.
         up: The upward direction of the camera.
         pos: The position of the camera.
 
@@ -342,15 +364,15 @@
 def radial_and_tangential_undistort(
     coords: torch.Tensor,
     distortion_params: torch.Tensor,
     eps: float = 1e-3,
     max_iterations: int = 10,
 ) -> torch.Tensor:
     """Computes undistorted coords given opencv distortion parameters.
-    Addapted from MultiNeRF
+    Adapted from MultiNeRF
     https://github.com/google-research/multinerf/blob/b02228160d3179300c7d499dca28cb9ca3677f32/internal/camera_utils.py#L477-L509
 
     Args:
         coords: The distorted coordinates.
         distortion_params: The distortion parameters [k1, k2, k3, k4, p1, p2].
         eps: The epsilon for the convergence.
         max_iterations: The maximum number of iterations to perform.
@@ -403,61 +425,151 @@
             [v[2], 0, -v[0]],
             [-v[1], v[0], 0],
         ]
     )
     return torch.eye(3) + skew_sym_mat + skew_sym_mat @ skew_sym_mat * ((1 - c) / (s**2 + 1e-8))
 
 
+def focus_of_attention(poses: TensorType["num_poses":..., 4, 4], initial_focus: TensorType[3]) -> TensorType[3]:
+    """Compute the focus of attention of a set of cameras. Only cameras
+    that have the focus of attention in front of them are considered.
+
+     Args:
+        poses: The poses to orient.
+        initial_focus: The 3D point views to decide which cameras are initially activated.
+
+    Returns:
+        The 3D position of the focus of attention.
+    """
+    # References to the same method in third-party code:
+    # https://github.com/google-research/multinerf/blob/1c8b1c552133cdb2de1c1f3c871b2813f6662265/internal/camera_utils.py#L145
+    # https://github.com/bmild/nerf/blob/18b8aebda6700ed659cb27a0c348b737a5f6ab60/load_llff.py#L197
+    active_directions = -poses[:, :3, 2:3]
+    active_origins = poses[:, :3, 3:4]
+    # initial value for testing if the focus_pt is in front or behind
+    focus_pt = initial_focus
+    # Prune cameras which have the current have the focus_pt behind them.
+    active = torch.sum(active_directions.squeeze(-1) * (focus_pt - active_origins.squeeze(-1)), dim=-1) > 0
+    done = False
+    # We need at least two active cameras, else fallback on the previous solution.
+    # This may be the "poses" solution if no cameras are active on first iteration, e.g.
+    # they are in an outward-looking configuration.
+    while torch.sum(active.int()) > 1 and not done:
+        active_directions = active_directions[active]
+        active_origins = active_origins[active]
+        # https://en.wikipedia.org/wiki/Line–line_intersection#In_more_than_two_dimensions
+        m = torch.eye(3) - active_directions * torch.transpose(active_directions, -2, -1)
+        mt_m = torch.transpose(m, -2, -1) @ m
+        focus_pt = torch.linalg.inv(mt_m.mean(0)) @ (mt_m @ active_origins).mean(0)[:, 0]
+        active = torch.sum(active_directions.squeeze(-1) * (focus_pt - active_origins.squeeze(-1)), dim=-1) > 0
+        if active.all():
+            # the set of active cameras did not change, so we're done.
+            done = True
+    return focus_pt
+
+
 def auto_orient_and_center_poses(
-    poses: TensorType["num_poses":..., 4, 4], method: Literal["pca", "up", "none"] = "up", center_poses: bool = True
-) -> TensorType["num_poses":..., 3, 4]:
+    poses: TensorType["num_poses":..., 4, 4],
+    method: Literal["pca", "up", "vertical", "none"] = "up",
+    center_method: Literal["poses", "focus", "none"] = "poses",
+) -> Tuple[TensorType["num_poses":..., 3, 4], TensorType[3, 4]]:
     """Orients and centers the poses. We provide two methods for orientation: pca and up.
 
-    pca: Orient the poses so that the principal component of the points is aligned with the axes.
-        This method works well when all of the cameras are in the same plane.
+    pca: Orient the poses so that the principal directions of the camera centers are aligned
+        with the axes, Z corresponding to the smallest principal component.
+        This method works well when all of the cameras are in the same plane, for example when
+        images are taken using a mobile robot.
     up: Orient the poses so that the average up vector is aligned with the z axis.
         This method works well when images are not at arbitrary angles.
-
+    vertical: Orient the poses so that the Z 3D direction projects close to the
+        y axis in images. This method works better if cameras are not all
+        looking in the same 3D direction, which may happen in camera arrays or in LLFF.
+
+    There are two centering methods:
+    poses: The poses are centered around the origin.
+    focus: The origin is set to the focus of attention of all cameras (the
+        closest point to cameras optical axes). Recommended for inward-looking
+        camera configurations.
 
     Args:
         poses: The poses to orient.
         method: The method to use for orientation.
-        center_poses: If True, the poses are centered around the origin.
+        center_method: The method to use to center the poses.
 
     Returns:
-        The oriented poses.
+        Tuple of the oriented poses and the transform matrix.
     """
 
-    translation = poses[..., :3, 3]
+    origins = poses[..., :3, 3]
 
-    mean_translation = torch.mean(translation, dim=0)
-    translation_diff = translation - mean_translation
+    mean_origin = torch.mean(origins, dim=0)
+    translation_diff = origins - mean_origin
 
-    if center_poses:
-        translation = mean_translation
+    if center_method == "poses":
+        translation = mean_origin
+    elif center_method == "focus":
+        translation = focus_of_attention(poses, mean_origin)
+    elif center_method == "none":
+        translation = torch.zeros_like(mean_origin)
     else:
-        translation = torch.zeros_like(mean_translation)
+        raise ValueError(f"Unknown value for center_method: {center_method}")
 
     if method == "pca":
         _, eigvec = torch.linalg.eigh(translation_diff.T @ translation_diff)
         eigvec = torch.flip(eigvec, dims=(-1,))
 
         if torch.linalg.det(eigvec) < 0:
             eigvec[:, 2] = -eigvec[:, 2]
 
         transform = torch.cat([eigvec, eigvec @ -translation[..., None]], dim=-1)
         oriented_poses = transform @ poses
 
         if oriented_poses.mean(axis=0)[2, 1] < 0:
             oriented_poses[:, 1:3] = -1 * oriented_poses[:, 1:3]
-    elif method == "up":
+    elif method in ("up", "vertical"):
         up = torch.mean(poses[:, :3, 1], dim=0)
         up = up / torch.linalg.norm(up)
+        if method == "vertical":
+            # If cameras are not all parallel (e.g. not in an LLFF configuration),
+            # we can find the 3D direction that most projects vertically in all
+            # cameras by minimizing ||Xu|| s.t. ||u||=1. This total least squares
+            # problem is solved by SVD.
+            x_axis_matrix = poses[:, :3, 0]
+            _, S, Vh = torch.linalg.svd(x_axis_matrix, full_matrices=False)
+            # Singular values are S_i=||Xv_i|| for each right singular vector v_i.
+            # ||S|| = sqrt(n) because lines of X are all unit vectors and the v_i
+            # are an orthonormal basis.
+            # ||Xv_i|| = sqrt(sum(dot(x_axis_j,v_i)^2)), thus S_i/sqrt(n) is the
+            # RMS of cosines between x axes and v_i. If the second smallest singular
+            # value corresponds to an angle error less than 10° (cos(80°)=0.17),
+            # this is probably a degenerate camera configuration (typical values
+            # are around 5° average error for the true vertical). In this case,
+            # rather than taking the vector corresponding to the smallest singular
+            # value, we project the "up" vector on the plane spanned by the two
+            # best singular vectors. We could also just fallback to the "up"
+            # solution.
+            if S[1] > 0.17 * math.sqrt(poses.shape[0]):
+                # regular non-degenerate configuration
+                up_vertical = Vh[2, :]
+                # It may be pointing up or down. Use "up" to disambiguate the sign.
+                up = up_vertical if torch.dot(up_vertical, up) > 0 else -up_vertical
+            else:
+                # Degenerate configuration: project "up" on the plane spanned by
+                # the last two right singular vectors (which are orthogonal to the
+                # first). v_0 is a unit vector, no need to divide by its norm when
+                # projecting.
+                up = up - Vh[0, :] * torch.dot(up, Vh[0, :])
+                # re-normalize
+                up = up / torch.linalg.norm(up)
 
         rotation = rotation_matrix(up, torch.Tensor([0, 0, 1]))
         transform = torch.cat([rotation, rotation @ -translation[..., None]], dim=-1)
         oriented_poses = transform @ poses
     elif method == "none":
-        oriented_poses = poses
-        poses[:, :3, 3] -= translation
+        transform = torch.eye(4)
+        transform[:3, 3] = -translation
+        transform = transform[:3, :]
+        oriented_poses = transform @ poses
+    else:
+        raise ValueError(f"Unknown value for method: {method}")
 
-    return oriented_poses
+    return oriented_poses, transform
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/lie_groups.py` & `nerfstudio-0.2.0/nerfstudio/cameras/lie_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Compute the exponential map of the direct product group `SO(3) x R^3`.
 
     This can be used for learning pose deltas on SE(3), and is generally faster than `exp_map_SE3`.
 
     Args:
         tangent_vector: Tangent vector; length-3 translations, followed by an `so(3)` tangent vector.
     Returns:
-        [R|t] tranformation matrices.
+        [R|t] transformation matrices.
     """
     # code for SO3 map grabbed from pytorch3d and stripped down to bare-bones
     log_rot = tangent_vector[:, 3:]
     nrms = (log_rot * log_rot).sum(1)
     rot_angles = torch.clamp(nrms, 1e-4).sqrt()
     rot_angles_inv = 1.0 / rot_angles
     fac1 = rot_angles_inv * rot_angles.sin()
@@ -63,15 +63,15 @@
 
     This can be used for learning pose deltas on `SE(3)`.
 
     Args:
         tangent_vector: A tangent vector from `se(3)`.
 
     Returns:
-        [R|t] tranformation matrices.
+        [R|t] transformation matrices.
     """
 
     tangent_vector_lin = tangent_vector[:, :3].view(-1, 3, 1)
     tangent_vector_ang = tangent_vector[:, 3:].view(-1, 3, 1)
 
     theta = torch.linalg.norm(tangent_vector_ang, dim=1).unsqueeze(1)
     theta2 = theta**2
```

### Comparing `nerfstudio-0.1.9/nerfstudio/cameras/rays.py` & `nerfstudio-0.2.0/nerfstudio/cameras/rays.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 # limitations under the License.
 
 """
 Some ray datastructures.
 """
 import random
 from dataclasses import dataclass
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, Optional, Tuple, Union
 
 import torch
 from torchtyping import TensorType
 
 from nerfstudio.utils.math import Gaussians, conical_frustum_to_gaussian
 from nerfstudio.utils.tensor_dataclass import TensorDataclass
 
+TORCH_DEVICE = Union[str, torch.device]  # pylint: disable=invalid-name
+
 
 @dataclass
 class Frustums(TensorDataclass):
     """Describes region of space as a frustum."""
 
     origins: TensorType["bs":..., 3]
     """xyz coordinate for ray origin."""
@@ -36,41 +38,60 @@
     """Direction of ray."""
     starts: TensorType["bs":..., 1]
     """Where the frustum starts along a ray."""
     ends: TensorType["bs":..., 1]
     """Where the frustum ends along a ray."""
     pixel_area: TensorType["bs":..., 1]
     """Projected area of pixel a distance 1 away from origin."""
+    offsets: Optional[TensorType["bs":..., 3]] = None
+    """Offsets for each sample position"""
 
     def get_positions(self) -> TensorType[..., 3]:
-        """Calulates "center" position of frustum. Not weighted by mass.
+        """Calculates "center" position of frustum. Not weighted by mass.
+
+        Returns:
+            xyz positions.
+        """
+        pos = self.origins + self.directions * (self.starts + self.ends) / 2
+        if self.offsets is not None:
+            pos = pos + self.offsets
+        return pos
+
+    def get_start_positions(self) -> TensorType[..., 3]:
+        """Calculates "start" position of frustum.
 
         Returns:
             xyz positions.
         """
-        return self.origins + self.directions * (self.starts + self.ends) / 2
+        return self.origins + self.directions * self.starts
+
+    def set_offsets(self, offsets):
+        """Sets offsets for this frustum for computing positions"""
+        self.offsets = offsets
 
     def get_gaussian_blob(self) -> Gaussians:
         """Calculates guassian approximation of conical frustum.
 
-        Resturns:
+        Returns:
             Conical frustums approximated by gaussian distribution.
         """
         # Cone radius is set such that the square pixel_area matches the cone area.
         cone_radius = torch.sqrt(self.pixel_area) / 1.7724538509055159  # r = sqrt(pixel_area / pi)
+        if self.offsets is not None:
+            raise NotImplementedError()
         return conical_frustum_to_gaussian(
             origins=self.origins,
             directions=self.directions,
             starts=self.starts,
             ends=self.ends,
             radius=cone_radius,
         )
 
     @classmethod
-    def get_mock_frustum(cls, device="cpu") -> "Frustums":
+    def get_mock_frustum(cls, device: Optional[TORCH_DEVICE] = "cpu") -> "Frustums":
         """Helper function to generate a placeholder frustum.
 
         Returns:
             A size 1 frustum with meaningless values.
         """
         return Frustums(
             origins=torch.ones((1, 3)).to(device),
@@ -94,15 +115,18 @@
     spacing_starts: Optional[TensorType["bs":..., "num_samples", 1]] = None
     """Start of normalized bin edges along ray [0,1], before warping is applied, ie. linear in disparity sampling."""
     spacing_ends: Optional[TensorType["bs":..., "num_samples", 1]] = None
     """Start of normalized bin edges along ray [0,1], before warping is applied, ie. linear in disparity sampling."""
     spacing_to_euclidean_fn: Optional[Callable] = None
     """Function to convert bins to euclidean distance."""
     metadata: Optional[Dict[str, TensorType["bs":..., "latent_dims"]]] = None
-    """addtional information relevant to generating ray samples"""
+    """additional information relevant to generating ray samples"""
+
+    times: Optional[TensorType[..., 1]] = None
+    """Times at which rays are sampled"""
 
     def get_weights(self, densities: TensorType[..., "num_samples", 1]) -> TensorType[..., "num_samples", 1]:
         """Return weights based on predicted densities
 
         Args:
             densities: Predicted densities for samples along ray
 
@@ -116,17 +140,39 @@
         transmittance = torch.cumsum(delta_density[..., :-1, :], dim=-2)
         transmittance = torch.cat(
             [torch.zeros((*transmittance.shape[:1], 1, 1), device=densities.device), transmittance], dim=-2
         )
         transmittance = torch.exp(-transmittance)  # [..., "num_samples"]
 
         weights = alphas * transmittance  # [..., "num_samples"]
+        weights = torch.nan_to_num(weights)
 
         return weights
 
+    @staticmethod
+    def get_weights_and_transmittance_from_alphas(
+        alphas: TensorType[..., "num_samples", 1], weights_only: bool = False
+    ) -> Tuple[TensorType[..., "num_samples", 1], TensorType[..., "num_samples", 1]]:
+        """Return weights based on predicted alphas
+        Args:
+            alphas: Predicted alphas (maybe from sdf) for samples along ray
+            weights_only: If function should return only weights
+        Returns:
+            Tuple of weights and transmittance for each sample
+        """
+
+        transmittance = torch.cumprod(
+            torch.cat([torch.ones((*alphas.shape[:1], 1, 1), device=alphas.device), 1.0 - alphas + 1e-7], 1), 1
+        )
+
+        weights = alphas * transmittance[:, :-1, :]
+        if weights_only:
+            return weights
+        return weights, transmittance
+
 
 @dataclass
 class RayBundle(TensorDataclass):
     """A bundle of ray parameters."""
 
     # TODO(ethan): make sure the sizes with ... are correct
     origins: TensorType[..., 3]
@@ -139,24 +185,26 @@
     """Camera indices"""
     nears: Optional[TensorType[..., 1]] = None
     """Distance along ray to start sampling"""
     fars: Optional[TensorType[..., 1]] = None
     """Rays Distance along ray to stop sampling"""
     metadata: Optional[Dict[str, TensorType["num_rays", "latent_dims"]]] = None
     """Additional metadata or data needed for interpolation, will mimic shape of rays"""
+    times: Optional[TensorType[..., 1]] = None
+    """Times at which rays are sampled"""
 
     def set_camera_indices(self, camera_index: int) -> None:
-        """Sets all of the the camera indices to a specific camera index.
+        """Sets all the camera indices to a specific camera index.
 
         Args:
             camera_index: Camera index.
         """
         self.camera_indices = torch.ones_like(self.origins[..., 0:1]).long() * camera_index
 
-    def __len__(self):
+    def __len__(self) -> int:
         num_rays = torch.numel(self.origins) // self.origins.shape[-1]
         return num_rays
 
     def sample(self, num_rays: int) -> "RayBundle":
         """Returns a RayBundle as a subset of rays.
 
         Args:
@@ -166,15 +214,15 @@
             RayBundle with subset of rays.
         """
         assert num_rays <= len(self)
         indices = random.sample(range(len(self)), k=num_rays)
         return self[indices]
 
     def get_row_major_sliced_ray_bundle(self, start_idx: int, end_idx: int) -> "RayBundle":
-        """Flattens RayBundle and extracts chunk given start and end indicies.
+        """Flattens RayBundle and extracts chunk given start and end indices.
 
         Args:
             start_idx: Start index of RayBundle chunk.
             end_idx: End index of RayBundle chunk.
 
         Returns:
             Flattened RayBundle with end_idx-start_idx rays.
@@ -219,10 +267,11 @@
             frustums=frustums,
             camera_indices=camera_indices,  # [..., 1, 1]
             deltas=deltas,  # [..., num_samples, 1]
             spacing_starts=spacing_starts,  # [..., num_samples, 1]
             spacing_ends=spacing_ends,  # [..., num_samples, 1]
             spacing_to_euclidean_fn=spacing_to_euclidean_fn,
             metadata=shaped_raybundle_fields.metadata,
+            times=None if self.times is None else self.times[..., None],  # [..., 1, 1]
         )
 
         return ray_samples
```

### Comparing `nerfstudio-0.1.9/nerfstudio/configs/__init__.py` & `nerfstudio-0.2.0/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/configs/config_utils.py` & `nerfstudio-0.2.0/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/__init__.py` & `nerfstudio-0.2.0/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-0.2.0/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-0.2.0/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,80 +16,148 @@
 Datamanager.
 """
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Tuple, Type, Union
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 import tyro
 from rich.progress import Console
 from torch import nn
 from torch.nn import Parameter
 from torch.utils.data import Dataset
 from torch.utils.data.distributed import DistributedSampler
+from typing_extensions import Literal
 
 from nerfstudio.cameras.camera_optimizers import CameraOptimizerConfig
+from nerfstudio.cameras.cameras import CameraType
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.configs.base_config import InstantiateConfig
+from nerfstudio.data.dataparsers.arkitscenes_dataparser import (
+    ARKitScenesDataParserConfig,
+)
+from nerfstudio.data.dataparsers.base_dataparser import DataparserOutputs
 from nerfstudio.data.dataparsers.blender_dataparser import BlenderDataParserConfig
 from nerfstudio.data.dataparsers.dnerf_dataparser import DNeRFDataParserConfig
-from nerfstudio.data.dataparsers.friends_dataparser import FriendsDataParserConfig
+from nerfstudio.data.dataparsers.dycheck_dataparser import DycheckDataParserConfig
 from nerfstudio.data.dataparsers.instant_ngp_dataparser import (
     InstantNGPDataParserConfig,
 )
+from nerfstudio.data.dataparsers.minimal_dataparser import MinimalDataParserConfig
+from nerfstudio.data.dataparsers.nerfosr_dataparser import NeRFOSRDataParserConfig
 from nerfstudio.data.dataparsers.nerfstudio_dataparser import NerfstudioDataParserConfig
-from nerfstudio.data.dataparsers.record3d_dataparser import Record3DDataParserConfig
+from nerfstudio.data.dataparsers.nuscenes_dataparser import NuScenesDataParserConfig
+from nerfstudio.data.dataparsers.phototourism_dataparser import (
+    PhototourismDataParserConfig,
+)
+from nerfstudio.data.dataparsers.scannet_dataparser import ScanNetDataParserConfig
+from nerfstudio.data.dataparsers.sdfstudio_dataparser import SDFStudioDataParserConfig
+from nerfstudio.data.dataparsers.sitcoms3d_dataparser import Sitcoms3DDataParserConfig
 from nerfstudio.data.datasets.base_dataset import InputDataset
-from nerfstudio.data.pixel_samplers import PixelSampler
+from nerfstudio.data.pixel_samplers import (
+    EquirectangularPixelSampler,
+    PatchPixelSampler,
+    PixelSampler,
+)
 from nerfstudio.data.utils.dataloaders import (
     CacheDataloader,
     FixedIndicesEvalDataloader,
     RandIndicesEvalDataloader,
 )
+from nerfstudio.data.utils.nerfstudio_collate import nerfstudio_collate
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes
 from nerfstudio.model_components.ray_generators import RayGenerator
 from nerfstudio.utils.misc import IterableWrapper
 
 CONSOLE = Console(width=120)
 
+
+def variable_res_collate(batch: List[Dict]) -> Dict:
+    """Default collate function for the cached dataloader.
+    Args:
+        batch: Batch of samples from the dataset.
+    Returns:
+        Collated batch.
+    """
+    images = []
+    masks = []
+    for data in batch:
+        image = data.pop("image")
+        mask = data.pop("mask", None)
+        images.append(image)
+        if mask:
+            masks.append(mask)
+
+    new_batch: dict = nerfstudio_collate(batch)
+    new_batch["image"] = images
+    if masks:
+        new_batch["mask"] = masks
+
+    return new_batch
+
+
 AnnotatedDataParserUnion = tyro.conf.OmitSubcommandPrefixes[  # Omit prefixes of flags in subcommands.
     tyro.extras.subcommand_type_from_defaults(
         {
             "nerfstudio-data": NerfstudioDataParserConfig(),
+            "minimal-parser": MinimalDataParserConfig(),
+            "arkit-data": ARKitScenesDataParserConfig(),
             "blender-data": BlenderDataParserConfig(),
-            "friends-data": FriendsDataParserConfig(),
             "instant-ngp-data": InstantNGPDataParserConfig(),
-            "record3d-data": Record3DDataParserConfig(),
+            "nuscenes-data": NuScenesDataParserConfig(),
             "dnerf-data": DNeRFDataParserConfig(),
+            "phototourism-data": PhototourismDataParserConfig(),
+            "dycheck-data": DycheckDataParserConfig(),
+            "scannet-data": ScanNetDataParserConfig(),
+            "sdfstudio-data": SDFStudioDataParserConfig(),
+            "nerfosr-data": NeRFOSRDataParserConfig(),
+            "sitcoms3d-data": Sitcoms3DDataParserConfig(),
         },
         prefix_names=False,  # Omit prefixes in subcommands themselves.
     )
 ]
 """Union over possible dataparser types, annotated with metadata for tyro. This is the
 same as the vanilla union, but results in shorter subcommand names."""
 
 
+@dataclass
+class DataManagerConfig(InstantiateConfig):
+    """Configuration for data manager instantiation; DataManager is in charge of keeping the train/eval dataparsers;
+    After instantiation, data manager holds both train/eval datasets and is in charge of returning unpacked
+    train/eval data at each iteration
+    """
+
+    _target: Type = field(default_factory=lambda: DataManager)
+    """Target class to instantiate."""
+    data: Optional[Path] = None
+    """Source of data, may not be used by all models."""
+    camera_optimizer: Optional[CameraOptimizerConfig] = None
+    """Specifies the camera pose optimizer used during training. Helpful if poses are noisy."""
+
+
 class DataManager(nn.Module):
     """Generic data manager's abstract class
 
     This version of the data manager is designed be a monolithic way to load data and latents,
     especially since this may contain learnable parameters which need to be shared across the train
     and test data managers. The idea is that we have setup methods for train and eval separately and
     this can be a combined train/eval if you want.
 
     Usage:
     To get data, use the next_train and next_eval functions.
     This data manager's next_train and next_eval methods will return 2 things:
-        1. A Raybundle: This will contain the rays we are sampling, with latents and
-            conditionals attached (everything needed at inference)
-        2. A "batch" of auxilury information: This will contain the mask, the ground truth
-            pixels, etc needed to actually train, score, etc the model
+
+    1. A Raybundle: This will contain the rays we are sampling, with latents and
+        conditionals attached (everything needed at inference)
+    2. A "batch" of auxiliary information: This will contain the mask, the ground truth
+        pixels, etc needed to actually train, score, etc the model
 
     Rationale:
     Because of this abstraction we've added, we can support more NeRF paradigms beyond the
     vanilla nerf paradigm of single-scene, fixed-images, no-learnt-latents.
     We can now support variable scenes, variable number of images, and arbitrary latents.
 
 
@@ -130,17 +198,17 @@
         If you aren't manually calling the setup_train and setup_eval functions from an overriden
         constructor, that you call super().__init__() BEFORE you initialize any
         nn.Modules or nn.Parameters, but AFTER you've already set all the attributes you need
         for the setup functions."""
         super().__init__()
         self.train_count = 0
         self.eval_count = 0
-        if self.train_dataset:
+        if self.train_dataset and self.test_mode != "inference":
             self.setup_train()
-        if self.eval_dataset:
+        if self.eval_dataset and self.test_mode != "inference":
             self.setup_eval()
 
     def forward(self):
         """Blank forward method
 
         This is an nn.Module, and so requires a forward() method normally, although in our case
         we do not need a forward() method"""
@@ -158,69 +226,96 @@
 
         This only exists to assist the get_eval_iterable function, since we need to pass
         in an __iter__ function for our trivial iterable that we are making."""
         self.eval_count = 0
 
     def get_train_iterable(self, length=-1) -> IterableWrapper:
         """Gets a trivial pythonic iterator that will use the iter_train and next_train functions
-        as __iter__ and __next__ methods respectivley.
+        as __iter__ and __next__ methods respectively.
 
         This basically is just a little utility if you want to do something like:
         |    for ray_bundle, batch in datamanager.get_train_iterable():
         |        <eval code here>
         since the returned IterableWrapper is just an iterator with the __iter__ and __next__
         methods (methods bound to our DataManager instance in this case) specified in the constructor.
         """
         return IterableWrapper(self.iter_train, self.next_train, length)
 
     def get_eval_iterable(self, length=-1) -> IterableWrapper:
         """Gets a trivial pythonic iterator that will use the iter_eval and next_eval functions
-        as __iter__ and __next__ methods respectivley.
+        as __iter__ and __next__ methods respectively.
 
         This basically is just a little utility if you want to do something like:
         |    for ray_bundle, batch in datamanager.get_eval_iterable():
         |        <eval code here>
         since the returned IterableWrapper is just an iterator with the __iter__ and __next__
         methods (methods bound to our DataManager instance in this case) specified in the constructor.
         """
         return IterableWrapper(self.iter_eval, self.next_eval, length)
 
     @abstractmethod
     def setup_train(self):
         """Sets up the data manager for training.
 
         Here you will define any subclass specific object attributes from the attribute"""
-        raise NotImplementedError
 
     @abstractmethod
     def setup_eval(self):
         """Sets up the data manager for evaluation"""
-        raise NotImplementedError
 
     @abstractmethod
-    def next_train(self, step: int) -> Tuple:
+    def next_train(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the train data manager.
 
-        This will be a tuple of all the information that this data manager outputs.
+        Args:
+            step: the step number of the eval image to retrieve
+        Returns:
+            A tuple of the ray bundle for the image, and a dictionary of additional batch information
+            such as the groudtruth image.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def next_eval(self, step: int) -> Tuple:
+    def next_eval(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the eval data manager.
 
-        This will be a tuple of all the information that this data manager outputs.
+        Args:
+            step: the step number of the eval image to retrieve
+        Returns:
+            A tuple of the ray bundle for the image, and a dictionary of additional batch information
+            such as the groudtruth image.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def next_eval_image(self, step: int) -> Tuple[int, RayBundle, Dict]:
+        """Retreive the next eval image.
+
+        Args:
+            step: the step number of the eval image to retrieve
+        Returns:
+            A tuple of the step number, the ray bundle for the image, and a dictionary of
+            additional batch information such as the groudtruth image.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def next_eval_image(self, step: int) -> Tuple:
-        """Returns the next eval image."""
+    def get_train_rays_per_batch(self) -> int:
+        """Returns the number of rays per batch for training."""
         raise NotImplementedError
 
+    @abstractmethod
+    def get_eval_rays_per_batch(self) -> int:
+        """Returns the number of rays per batch for evaluation."""
+        raise NotImplementedError
+
+    def get_datapath(self) -> Optional[Path]:  # pylint:disable=no-self-use
+        """Returns the path to the data. This is used to determine where to save camera paths."""
+        return None
+
     def get_training_callbacks(  # pylint:disable=no-self-use
         self, training_callback_attributes: TrainingCallbackAttributes  # pylint: disable=unused-argument
     ) -> List[TrainingCallback]:
         """Returns a list of callbacks to be used during training."""
         return []
 
     @abstractmethod
@@ -230,19 +325,16 @@
         Returns:
             A list of dictionaries containing the data manager's param groups.
         """
         return {}
 
 
 @dataclass
-class VanillaDataManagerConfig(InstantiateConfig):
-    """Configuration for data manager instantiation; DataManager is in charge of keeping the train/eval dataparsers;
-    After instantiation, data manager holds both train/eval datasets and is in charge of returning unpacked
-    train/eval data at each iteration
-    """
+class VanillaDataManagerConfig(DataManagerConfig):
+    """A basic data manager"""
 
     _target: Type = field(default_factory=lambda: VanillaDataManager)
     """Target class to instantiate."""
     dataparser: AnnotatedDataParserUnion = BlenderDataParserConfig()
     """Specifies the dataparser used to unpack the data."""
     train_num_rays_per_batch: int = 1024
     """Number of rays per batch to use per training iteration."""
@@ -259,14 +351,22 @@
     """When not evaluating on all images, number of iterations before picking
     new images. If -1, never pick new images."""
     eval_image_indices: Optional[Tuple[int, ...]] = (0,)
     """Specifies the image indices to use during eval; if None, uses all."""
     camera_optimizer: CameraOptimizerConfig = CameraOptimizerConfig()
     """Specifies the camera pose optimizer used during training. Helpful if poses are noisy, such as for data from
     Record3D."""
+    collate_fn = staticmethod(nerfstudio_collate)
+    """Specifies the collate function to use for the train and eval dataloaders."""
+    camera_res_scale_factor: float = 1.0
+    """The scale factor for scaling spatial data such as images, mask, semantics
+    along with relevant information about camera intrinsics
+    """
+    patch_size: int = 1
+    """Size of patch to sample from. If >1, patch-based sampling will be used."""
 
 
 class VanillaDataManager(DataManager):  # pylint: disable=abstract-method
     """Basic stored data manager implementation.
 
     This is pretty much a port over from our old dataloading utilities, and is a little jank
     under the hood. We may clean this up a little bit under the hood with more standard dataloading
@@ -277,123 +377,179 @@
     Args:
         config: the DataManagerConfig used to instantiate class
     """
 
     config: VanillaDataManagerConfig
     train_dataset: InputDataset
     eval_dataset: InputDataset
+    train_dataparser_outputs: DataparserOutputs
+    train_pixel_sampler: Optional[PixelSampler] = None
+    eval_pixel_sampler: Optional[PixelSampler] = None
 
     def __init__(
         self,
         config: VanillaDataManagerConfig,
         device: Union[torch.device, str] = "cpu",
-        test_mode: bool = False,
+        test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
         **kwargs,  # pylint: disable=unused-argument
     ):
         self.config = config
         self.device = device
         self.world_size = world_size
         self.local_rank = local_rank
         self.sampler = None
         self.test_mode = test_mode
+        self.test_split = "test" if test_mode in ["test", "inference"] else "val"
+        self.dataparser_config = self.config.dataparser
+        if self.config.data is not None:
+            self.config.dataparser.data = Path(self.config.data)
+        else:
+            self.config.data = self.config.dataparser.data
+        self.dataparser = self.dataparser_config.setup()
+        self.train_dataparser_outputs = self.dataparser.get_dataparser_outputs(split="train")
 
         self.train_dataset = self.create_train_dataset()
         self.eval_dataset = self.create_eval_dataset()
+
+        if self.train_dataparser_outputs is not None:
+            cameras = self.train_dataparser_outputs.cameras
+            if len(cameras) > 1:
+                for i in range(1, len(cameras)):
+                    if cameras[0].width != cameras[i].width or cameras[0].height != cameras[i].height:
+                        CONSOLE.print("Variable resolution, using variable_res_collate")
+                        self.config.collate_fn = variable_res_collate
+                        break
+
         super().__init__()
 
     def create_train_dataset(self) -> InputDataset:
         """Sets up the data loaders for training"""
-        return InputDataset(self.config.dataparser.setup().get_dataparser_outputs(split="train"))
+        return InputDataset(
+            dataparser_outputs=self.train_dataparser_outputs,
+            scale_factor=self.config.camera_res_scale_factor,
+        )
 
     def create_eval_dataset(self) -> InputDataset:
         """Sets up the data loaders for evaluation"""
         return InputDataset(
-            self.config.dataparser.setup().get_dataparser_outputs(split="val" if not self.test_mode else "test")
+            dataparser_outputs=self.dataparser.get_dataparser_outputs(split=self.test_split),
+            scale_factor=self.config.camera_res_scale_factor,
         )
 
+    def _get_pixel_sampler(  # pylint: disable=no-self-use
+        self, dataset: InputDataset, *args: Any, **kwargs: Any
+    ) -> PixelSampler:
+        """Infer pixel sampler to use."""
+        if self.config.patch_size > 1:
+            return PatchPixelSampler(*args, **kwargs, patch_size=self.config.patch_size)
+
+        # If all images are equirectangular, use equirectangular pixel sampler
+        is_equirectangular = dataset.cameras.camera_type == CameraType.EQUIRECTANGULAR.value
+        if is_equirectangular.all():
+            return EquirectangularPixelSampler(*args, **kwargs)
+        # Otherwise, use the default pixel sampler
+        if is_equirectangular.any():
+            CONSOLE.print("[bold yellow]Warning: Some cameras are equirectangular, but using default pixel sampler.")
+        return PixelSampler(*args, **kwargs)
+
     def setup_train(self):
         """Sets up the data loaders for training"""
         assert self.train_dataset is not None
         CONSOLE.print("Setting up training dataset...")
         self.train_image_dataloader = CacheDataloader(
             self.train_dataset,
             num_images_to_sample_from=self.config.train_num_images_to_sample_from,
             num_times_to_repeat_images=self.config.train_num_times_to_repeat_images,
             device=self.device,
             num_workers=self.world_size * 4,
             pin_memory=True,
+            collate_fn=self.config.collate_fn,
         )
         self.iter_train_image_dataloader = iter(self.train_image_dataloader)
-        self.train_pixel_sampler = PixelSampler(self.config.train_num_rays_per_batch)
+        self.train_pixel_sampler = self._get_pixel_sampler(self.train_dataset, self.config.train_num_rays_per_batch)
         self.train_camera_optimizer = self.config.camera_optimizer.setup(
-            num_cameras=self.train_dataset.dataparser_outputs.cameras.size, device=self.device
+            num_cameras=self.train_dataset.cameras.size, device=self.device
         )
         self.train_ray_generator = RayGenerator(
-            self.train_dataset.dataparser_outputs.cameras.to(self.device),
+            self.train_dataset.cameras.to(self.device),
             self.train_camera_optimizer,
         )
 
     def setup_eval(self):
         """Sets up the data loader for evaluation"""
         assert self.eval_dataset is not None
         CONSOLE.print("Setting up evaluation dataset...")
         self.eval_image_dataloader = CacheDataloader(
             self.eval_dataset,
             num_images_to_sample_from=self.config.eval_num_images_to_sample_from,
             num_times_to_repeat_images=self.config.eval_num_times_to_repeat_images,
             device=self.device,
             num_workers=self.world_size * 4,
             pin_memory=True,
+            collate_fn=self.config.collate_fn,
         )
         self.iter_eval_image_dataloader = iter(self.eval_image_dataloader)
-        self.eval_pixel_sampler = PixelSampler(self.config.eval_num_rays_per_batch)
+        self.eval_pixel_sampler = self._get_pixel_sampler(self.eval_dataset, self.config.eval_num_rays_per_batch)
+        self.eval_camera_optimizer = self.config.camera_optimizer.setup(
+            num_cameras=self.eval_dataset.cameras.size, device=self.device
+        )
         self.eval_ray_generator = RayGenerator(
-            self.eval_dataset.dataparser_outputs.cameras.to(self.device),
-            self.train_camera_optimizer,  # should be shared between train and eval.
+            self.eval_dataset.cameras.to(self.device),
+            self.eval_camera_optimizer,
         )
         # for loading full images
         self.fixed_indices_eval_dataloader = FixedIndicesEvalDataloader(
             input_dataset=self.eval_dataset,
             device=self.device,
             num_workers=self.world_size * 4,
         )
         self.eval_dataloader = RandIndicesEvalDataloader(
             input_dataset=self.eval_dataset,
-            image_indices=self.config.eval_image_indices,
             device=self.device,
             num_workers=self.world_size * 4,
         )
 
     def next_train(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the train dataloader."""
         self.train_count += 1
         image_batch = next(self.iter_train_image_dataloader)
+        assert self.train_pixel_sampler is not None
         batch = self.train_pixel_sampler.sample(image_batch)
         ray_indices = batch["indices"]
         ray_bundle = self.train_ray_generator(ray_indices)
         return ray_bundle, batch
 
     def next_eval(self, step: int) -> Tuple[RayBundle, Dict]:
         """Returns the next batch of data from the eval dataloader."""
         self.eval_count += 1
         image_batch = next(self.iter_eval_image_dataloader)
+        assert self.eval_pixel_sampler is not None
         batch = self.eval_pixel_sampler.sample(image_batch)
         ray_indices = batch["indices"]
         ray_bundle = self.eval_ray_generator(ray_indices)
         return ray_bundle, batch
 
     def next_eval_image(self, step: int) -> Tuple[int, RayBundle, Dict]:
         for camera_ray_bundle, batch in self.eval_dataloader:
             assert camera_ray_bundle.camera_indices is not None
             image_idx = int(camera_ray_bundle.camera_indices[0, 0, 0])
             return image_idx, camera_ray_bundle, batch
         raise ValueError("No more eval images")
 
+    def get_train_rays_per_batch(self) -> int:
+        return self.config.train_num_rays_per_batch
+
+    def get_eval_rays_per_batch(self) -> int:
+        return self.config.eval_num_rays_per_batch
+
+    def get_datapath(self) -> Path:
+        return self.config.dataparser.data
+
     def get_param_groups(self) -> Dict[str, List[Parameter]]:  # pylint: disable=no-self-use
         """Get the param groups for the data manager.
         Returns:
             A list of dictionaries containing the data manager's param groups.
         """
         param_groups = {}
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datamanagers/semantic_datamanager.py` & `nerfstudio-0.2.0/nerfstudio/data/datamanagers/semantic_datamanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,13 +37,18 @@
     """Data manager implementation for data that also requires processing semantic data.
 
     Args:
         config: the DataManagerConfig used to instantiate class
     """
 
     def create_train_dataset(self) -> SemanticDataset:
-        return SemanticDataset(self.config.dataparser.setup().get_dataparser_outputs(split="train"))
+        self.train_dataparser_outputs = self.dataparser.get_dataparser_outputs(split="train")
+        return SemanticDataset(
+            dataparser_outputs=self.train_dataparser_outputs,
+            scale_factor=self.config.camera_res_scale_factor,
+        )
 
     def create_eval_dataset(self) -> SemanticDataset:
         return SemanticDataset(
-            self.config.dataparser.setup().get_dataparser_outputs(split="val" if not self.test_mode else "test")
+            dataparser_outputs=self.dataparser.get_dataparser_outputs(split=self.test_split),
+            scale_factor=self.config.camera_res_scale_factor,
         )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/blender_dataparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,10 +100,11 @@
         )
 
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             alpha_color=alpha_color_tensor,
             scene_box=scene_box,
+            dataparser_scale=self.scale_factor,
         )
 
         return dataparser_outputs
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/dnerf_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,11 +98,15 @@
             cx=cx,
             cy=cy,
             camera_type=CameraType.PERSPECTIVE,
             times=times,
         )
 
         dataparser_outputs = DataparserOutputs(
-            image_filenames=image_filenames, cameras=cameras, alpha_color=alpha_color_tensor, scene_box=scene_box
+            image_filenames=image_filenames,
+            cameras=cameras,
+            alpha_color=alpha_color_tensor,
+            scene_box=scene_box,
+            dataparser_scale=self.scale_factor,
         )
 
         return dataparser_outputs
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/friends_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Data parser for friends dataset"""
+"""Data parser for sitcoms3D dataset.
+
+The dataset is from the paper ["The One Where They Reconstructed 3D Humans and
+Environments in TV Shows"](https://ethanweber.me/sitcoms3D/)
+"""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
 import torch
@@ -32,36 +37,36 @@
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.utils.io import load_from_json
 
 CONSOLE = Console()
 
 
 @dataclass
-class FriendsDataParserConfig(DataParserConfig):
-    """Friends dataset parser config"""
+class Sitcoms3DDataParserConfig(DataParserConfig):
+    """sitcoms3D dataset parser config"""
 
-    _target: Type = field(default_factory=lambda: Friends)
+    _target: Type = field(default_factory=lambda: Sitcoms3D)
     """target class to instantiate"""
-    data: Path = Path("data/friends/TBBT-big_living_room")
+    data: Path = Path("data/sitcoms3d/TBBT-big_living_room")
     """Directory specifying location of data."""
     include_semantics: bool = True
     """whether or not to include loading of semantics data"""
     downscale_factor: int = 4
     scene_scale: float = 2.0
     """
     Sets the bounding cube to have edge length of this size.
-    The longest dimension of the Friends axis-aligned bbox will be scaled to this value.
+    The longest dimension of the Sitcoms3D axis-aligned bbox will be scaled to this value.
     """
 
 
 @dataclass
-class Friends(DataParser):
-    """Friends Dataset"""
+class Sitcoms3D(DataParser):
+    """Sitcoms3D Dataset"""
 
-    config: FriendsDataParserConfig
+    config: Sitcoms3DDataParserConfig
 
     def _generate_dataparser_outputs(self, split="train"):  # pylint: disable=unused-argument,too-many-statements
 
         cameras_json = load_from_json(self.config.data / "cameras.json")
         frames = cameras_json["frames"]
         bbox = torch.tensor(cameras_json["bbox"])
 
@@ -112,20 +117,19 @@
         longest_length = lengths[longest_dim]
         scale = scene_scale / longest_length
         scene_box.aabb = scene_box.aabb * scale  # box
         camera_to_worlds[..., 3] *= scale  # cameras
 
         # --- semantics ---
         if self.config.include_semantics:
+            empty_path = Path()
+            replace_this_path = str(empty_path / images_folder / empty_path)
+            with_this_path = str(empty_path / segmentations_folder / "thing" / empty_path)
             filenames = [
-                Path(
-                    str(image_filename)
-                    .replace(f"/{images_folder}/", f"/{segmentations_folder}/thing/")
-                    .replace(".jpg", ".png")
-                )
+                Path(str(image_filename).replace(replace_this_path, with_this_path).replace(".jpg", ".png"))
                 for image_filename in image_filenames
             ]
             panoptic_classes = load_from_json(self.config.data / "panoptic_classes.json")
             classes = panoptic_classes["thing"]
             colors = torch.tensor(panoptic_classes["thing_colors"], dtype=torch.float32) / 255.0
             semantics = Semantics(filenames=filenames, classes=classes, colors=colors, mask_classes=["person"])
 
@@ -143,9 +147,10 @@
         cameras.rescale_output_resolution(scaling_factor=1.0 / self.config.downscale_factor)
 
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             scene_box=scene_box,
             metadata={"semantics": semantics} if self.config.include_semantics else {},
+            dataparser_scale=scale,
         )
         return dataparser_outputs
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, Tuple, Type
 
+import imageio
 import numpy as np
 import torch
 from rich.console import Console
 
 from nerfstudio.cameras import camera_utils
 from nerfstudio.cameras.cameras import Cameras, CameraType
 from nerfstudio.data.dataparsers.base_dataparser import (
@@ -40,38 +41,54 @@
 @dataclass
 class InstantNGPDataParserConfig(DataParserConfig):
     """Instant-NGP dataset parser config"""
 
     _target: Type = field(default_factory=lambda: InstantNGP)
     """target class to instantiate"""
     data: Path = Path("data/ours/posterv2")
-    """Directory specifying location of data."""
-    scale_factor: float = 1.0
-    """How much to scale the camera origins by."""
-    scene_scale: float = 0.33
+    """Directory or explicit json file path specifying location of data."""
+    scene_scale: float = 0.3333
     """How much to scale the scene."""
 
 
 @dataclass
 class InstantNGP(DataParser):
     """Instant NGP Dataset"""
 
     config: InstantNGPDataParserConfig
 
     def _generate_dataparser_outputs(self, split="train"):
+        if self.config.data.suffix == ".json":
+            meta = load_from_json(self.config.data)
+            data_dir = self.config.data.parent
+        else:
+            meta = load_from_json(self.config.data / "transforms.json")
+            data_dir = self.config.data
 
-        meta = load_from_json(self.config.data / "transforms.json")
         image_filenames = []
         poses = []
         num_skipped_image_filenames = 0
         for frame in meta["frames"]:
-            fname = self.config.data / Path(frame["file_path"])
-            if not fname:
+            fname = data_dir / Path(frame["file_path"])
+            # search for png file
+            if not fname.exists():
+                fname = data_dir / Path(frame["file_path"] + ".png")
+            if not fname.exists():
+                CONSOLE.log(f"couldnt find {fname} image")
                 num_skipped_image_filenames += 1
             else:
+                if "w" not in meta:
+                    img_0 = imageio.imread(fname)
+                    h, w = img_0.shape[:2]
+                    meta["w"] = w
+                    if "h" in meta:
+                        meta_h = meta["h"]
+                        assert meta_h == h, f"height of image dont not correspond metadata {h} != {meta_h}"
+                    else:
+                        meta["h"] = h
                 image_filenames.append(fname)
                 poses.append(np.array(frame["transform_matrix"]))
         if num_skipped_image_filenames >= 0:
             CONSOLE.print(f"Skipping {num_skipped_image_filenames} files in dataset split {split}.")
         assert (
             len(image_filenames) != 0
         ), """
@@ -80,45 +97,58 @@
         """
         poses = np.array(poses).astype(np.float32)
         poses[:, :3, 3] *= self.config.scene_scale
 
         camera_to_world = torch.from_numpy(poses[:, :3])  # camera to world transform
 
         distortion_params = camera_utils.get_distortion_params(
-            k1=float(meta["k1"]), k2=float(meta["k2"]), p1=float(meta["p1"]), p2=float(meta["p2"])
+            k1=float(meta.get("k1", 0)),
+            k2=float(meta.get("k2", 0)),
+            k3=float(meta.get("k3", 0)),
+            k4=float(meta.get("k4", 0)),
+            p1=float(meta.get("p1", 0)),
+            p2=float(meta.get("p2", 0)),
         )
 
         # in x,y,z order
         # assumes that the scene is centered at the origin
-        aabb_scale = meta["aabb_scale"]
+        aabb_scale = 0.5 * meta.get("aabb_scale", 1)
+
         scene_box = SceneBox(
             aabb=torch.tensor(
                 [[-aabb_scale, -aabb_scale, -aabb_scale], [aabb_scale, aabb_scale, aabb_scale]], dtype=torch.float32
             )
         )
 
         fl_x, fl_y = InstantNGP.get_focal_lengths(meta)
 
+        w, h = meta["w"], meta["h"]
+
+        camera_type = CameraType.PERSPECTIVE
+        if meta.get("is_fisheye", False):
+            camera_type = CameraType.FISHEYE
+
         cameras = Cameras(
             fx=float(fl_x),
             fy=float(fl_y),
-            cx=float(meta["cx"]),
-            cy=float(meta["cy"]),
+            cx=float(meta.get("cx", 0.5 * w)),
+            cy=float(meta.get("cy", 0.5 * h)),
             distortion_params=distortion_params,
-            height=int(meta["h"]),
-            width=int(meta["w"]),
+            height=int(h),
+            width=int(w),
             camera_to_worlds=camera_to_world,
-            camera_type=CameraType.PERSPECTIVE,
+            camera_type=camera_type,
         )
 
         # TODO(ethan): add alpha background color
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             scene_box=scene_box,
+            dataparser_scale=self.config.scene_scale,
         )
 
         return dataparser_outputs
 
     @classmethod
     def get_focal_lengths(cls, meta: Dict) -> Tuple[float, float]:
         """Reads or computes the focal length from transforms dict.
@@ -135,18 +165,21 @@
         if "fl_x" in meta:
             fl_x = meta["fl_x"]
         elif "x_fov" in meta:
             fl_x = fov_to_focal_length(np.deg2rad(meta["x_fov"]), meta["w"])
         elif "camera_angle_x" in meta:
             fl_x = fov_to_focal_length(meta["camera_angle_x"], meta["w"])
 
-        if "fl_y" in meta:
-            fl_y = meta["fl_y"]
-        elif "y_fov" in meta:
-            fl_y = fov_to_focal_length(np.deg2rad(meta["y_fov"]), meta["h"])
-        elif "camera_angle_y" in meta:
-            fl_y = fov_to_focal_length(meta["camera_angle_y"], meta["h"])
+        if "camera_angle_y" not in meta or "y_fov" not in meta:
+            fl_y = fl_x
+        else:
+            if "fl_y" in meta:
+                fl_y = meta["fl_y"]
+            elif "y_fov" in meta:
+                fl_y = fov_to_focal_length(np.deg2rad(meta["y_fov"]), meta["h"])
+            elif "camera_angle_y" in meta:
+                fl_y = fov_to_focal_length(meta["camera_angle_y"], meta["h"])
 
         if fl_x == 0 or fl_y == 0:
             raise AttributeError("Focal length cannot be calculated from transforms.json (missing fields).")
 
         return (fl_x, fl_y)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,194 +7,186 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" Data parser for nerfstudio datasets. """
 
+"""Phototourism dataset parser. Datasets and documentation here: http://phototour.cs.washington.edu/datasets/"""
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass, field
-from pathlib import Path, PurePath
-from typing import Optional, Type
+from pathlib import Path
+from typing import Type
 
 import numpy as np
 import torch
-from PIL import Image
-from rich.console import Console
+from rich.progress import Console
 from typing_extensions import Literal
 
 from nerfstudio.cameras import camera_utils
-from nerfstudio.cameras.cameras import CAMERA_MODEL_TO_TYPE, Cameras, CameraType
+from nerfstudio.cameras.cameras import Cameras, CameraType
 from nerfstudio.data.dataparsers.base_dataparser import (
     DataParser,
     DataParserConfig,
     DataparserOutputs,
 )
 from nerfstudio.data.scene_box import SceneBox
-from nerfstudio.utils.io import load_from_json
+
+# TODO(1480) use pycolmap instead of colmap_parsing_utils
+# import pycolmap
+from nerfstudio.data.utils.colmap_parsing_utils import (
+    read_cameras_binary,
+    read_images_binary,
+)
 
 CONSOLE = Console(width=120)
-MAX_AUTO_RESOLUTION = 1600
 
 
 @dataclass
-class NerfstudioDataParserConfig(DataParserConfig):
-    """Nerfstudio dataset config"""
+class PhototourismDataParserConfig(DataParserConfig):
+    """Phototourism dataset parser config"""
 
-    _target: Type = field(default_factory=lambda: Nerfstudio)
+    _target: Type = field(default_factory=lambda: Phototourism)
     """target class to instantiate"""
-    data: Path = Path("data/nerfstudio/poster")
+    data: Path = Path("data/phototourism/brandenburg-gate")
     """Directory specifying location of data."""
-    scale_factor: float = 1.0
+    scale_factor: float = 3.0
     """How much to scale the camera origins by."""
-    downscale_factor: Optional[int] = None
-    """How much to downscale images. If not set, images are chosen such that the max dimension is <1600px."""
+    alpha_color: str = "white"
+    """alpha color of background"""
+    train_split_fraction: float = 0.9
+    """The fraction of images to use for training. The remaining images are for eval."""
     scene_scale: float = 1.0
     """How much to scale the region of interest by."""
-    orientation_method: Literal["pca", "up", "none"] = "up"
+    orientation_method: Literal["pca", "up", "vertical", "none"] = "up"
     """The method to use for orientation."""
-    center_poses: bool = True
-    """Whether to center the poses."""
+    center_method: Literal["poses", "focus", "none"] = "poses"
+    """The method to use to center the poses."""
     auto_scale_poses: bool = True
     """Whether to automatically scale the poses to fit in +/- 1 bounding box."""
-    train_split_percentage: float = 0.9
-    """The percent of images to use for training. The remaining images are for eval."""
 
 
 @dataclass
-class Nerfstudio(DataParser):
-    """Nerfstudio DatasetParser"""
-
-    config: NerfstudioDataParserConfig
-    downscale_factor: Optional[int] = None
+class Phototourism(DataParser):
+    """Phototourism dataset. This is based on https://github.com/kwea123/nerf_pl/blob/nerfw/datasets/phototourism.py
+    and uses colmap's utils file to read the poses.
+    """
+
+    config: PhototourismDataParserConfig
+
+    def __init__(self, config: PhototourismDataParserConfig):
+        super().__init__(config=config)
+        self.data: Path = config.data
 
+    # pylint: disable=too-many-statements
     def _generate_dataparser_outputs(self, split="train"):
-        # pylint: disable=too-many-statements
-
-        meta = load_from_json(self.config.data / "transforms.json")
         image_filenames = []
         poses = []
-        num_skipped_image_filenames = 0
 
-        for frame in meta["frames"]:
-            filepath = PurePath(frame["file_path"])
-            fname = self._get_fname(filepath)
-            if not fname.exists():
-                num_skipped_image_filenames += 1
-            else:
-                image_filenames.append(fname)
-                poses.append(np.array(frame["transform_matrix"]))
-        if num_skipped_image_filenames >= 0:
-            CONSOLE.log(f"Skipping {num_skipped_image_filenames} files in dataset split {split}.")
-        assert (
-            len(image_filenames) != 0
-        ), """
-        No image files found. 
-        You should check the file_paths in the transforms.json file to make sure they are correct.
-        """
+        with CONSOLE.status(f"[bold green]Reading phototourism images and poses for {split} split...") as _:
+            # TODO(1480) use pycolmap
+            # recon = pycolmap.Reconstruction(self.data / "dense" / "sparse")
+            # cams = recon.cameras
+            # imgs = recon.images
+            cams = read_cameras_binary(self.data / "dense/sparse/cameras.bin")
+            imgs = read_images_binary(self.data / "dense/sparse/images.bin")
+
+        poses = []
+        fxs = []
+        fys = []
+        cxs = []
+        cys = []
+        image_filenames = []
+
+        flip = torch.eye(3)
+        flip[0, 0] = -1.0
+        flip = flip.double()
+
+        for _id, cam in cams.items():
+            img = imgs[_id]
+
+            assert cam.model == "PINHOLE", "Only pinhole (perspective) camera model is supported at the moment"
+
+            pose = torch.cat([torch.tensor(img.qvec2rotmat()), torch.tensor(img.tvec.reshape(3, 1))], dim=1)
+            pose = torch.cat([pose, torch.tensor([[0.0, 0.0, 0.0, 1.0]])], dim=0)
+            poses.append(torch.linalg.inv(pose))
+            fxs.append(torch.tensor(cam.params[0]))
+            fys.append(torch.tensor(cam.params[1]))
+            cxs.append(torch.tensor(cam.params[2]))
+            cys.append(torch.tensor(cam.params[3]))
+
+            image_filenames.append(self.data / "dense/images" / img.name)
+
+        poses = torch.stack(poses).float()
+        poses[..., 1:3] *= -1
+        fxs = torch.stack(fxs).float()
+        fys = torch.stack(fys).float()
+        cxs = torch.stack(cxs).float()
+        cys = torch.stack(cys).float()
 
         # filter image_filenames and poses based on train/eval split percentage
         num_images = len(image_filenames)
-        num_train_images = math.ceil(num_images * self.config.train_split_percentage)
+        num_train_images = math.ceil(num_images * self.config.train_split_fraction)
         num_eval_images = num_images - num_train_images
         i_all = np.arange(num_images)
         i_train = np.linspace(
             0, num_images - 1, num_train_images, dtype=int
         )  # equally spaced training images starting and ending at 0 and num_images-1
         i_eval = np.setdiff1d(i_all, i_train)  # eval images are the remaining images
+        i_all = torch.tensor(i_all)
+        i_train = torch.tensor(i_train, dtype=torch.long)
+        i_eval = torch.tensor(i_eval, dtype=torch.long)
         assert len(i_eval) == num_eval_images
         if split == "train":
             indices = i_train
         elif split in ["val", "test"]:
             indices = i_eval
         else:
             raise ValueError(f"Unknown dataparser split {split}")
 
-        poses = torch.from_numpy(np.array(poses).astype(np.float32))
-        poses = camera_utils.auto_orient_and_center_poses(
-            poses, method=self.config.orientation_method, center_poses=self.config.center_poses
+        poses, transform_matrix = camera_utils.auto_orient_and_center_poses(
+            poses, method=self.config.orientation_method, center_method=self.config.center_method
         )
 
         # Scale poses
         scale_factor = 1.0
         if self.config.auto_scale_poses:
-            scale_factor /= torch.max(torch.abs(poses[:, :3, 3]))
+            scale_factor /= float(torch.max(torch.abs(poses[:, :3, 3])))
+        scale_factor *= self.config.scale_factor
 
-        poses[:, :3, 3] *= scale_factor * self.config.scale_factor
-
-        # Choose image_filenames and poses based on split, but after auto orient and scaling the poses.
-        image_filenames = [image_filenames[i] for i in indices]
-        poses = poses[indices]
+        poses[:, :3, 3] *= scale_factor
 
         # in x,y,z order
         # assumes that the scene is centered at the origin
         aabb_scale = self.config.scene_scale
         scene_box = SceneBox(
             aabb=torch.tensor(
                 [[-aabb_scale, -aabb_scale, -aabb_scale], [aabb_scale, aabb_scale, aabb_scale]], dtype=torch.float32
             )
         )
 
-        if "camera_model" in meta:
-            camera_type = CAMERA_MODEL_TO_TYPE[meta["camera_model"]]
-        else:
-            camera_type = CameraType.PERSPECTIVE
-
-        distortion_params = camera_utils.get_distortion_params(
-            k1=float(meta["k1"]) if "k1" in meta else 0.0,
-            k2=float(meta["k2"]) if "k2" in meta else 0.0,
-            k3=float(meta["k3"]) if "k3" in meta else 0.0,
-            k4=float(meta["k4"]) if "k4" in meta else 0.0,
-            p1=float(meta["p1"]) if "p1" in meta else 0.0,
-            p2=float(meta["p2"]) if "p2" in meta else 0.0,
-        )
-
         cameras = Cameras(
-            fx=float(meta["fl_x"]),
-            fy=float(meta["fl_y"]),
-            cx=float(meta["cx"]),
-            cy=float(meta["cy"]),
-            distortion_params=distortion_params,
-            height=int(meta["h"]),
-            width=int(meta["w"]),
             camera_to_worlds=poses[:, :3, :4],
-            camera_type=camera_type,
+            fx=fxs,
+            fy=fys,
+            cx=cxs,
+            cy=cys,
+            camera_type=CameraType.PERSPECTIVE,
         )
 
-        assert self.downscale_factor is not None
-        cameras.rescale_output_resolution(scaling_factor=1.0 / self.downscale_factor)
+        cameras = cameras[indices]
+        image_filenames = [image_filenames[i] for i in indices]
+
+        assert len(cameras) == len(image_filenames)
 
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             scene_box=scene_box,
+            dataparser_scale=scale_factor,
+            dataparser_transform=transform_matrix,
         )
-        return dataparser_outputs
 
-    def _get_fname(self, filepath: PurePath) -> Path:
-        """Get the filename of the image file."""
-
-        if self.downscale_factor is None:
-            if self.config.downscale_factor is None:
-                test_img = Image.open(self.config.data / filepath)
-                h, w = test_img.size
-                max_res = max(h, w)
-                df = 0
-                while True:
-                    if (max_res / 2 ** (df)) < MAX_AUTO_RESOLUTION:
-                        break
-                    if not (self.config.data / f"images_{2**(df+1)}" / filepath.name).exists():
-                        break
-                    df += 1
-
-                self.downscale_factor = 2**df
-                CONSOLE.log(f"Auto image downscale factor of {self.downscale_factor}")
-            else:
-                self.downscale_factor = self.config.downscale_factor
-
-        if self.downscale_factor > 1:
-            return self.config.data / f"images_{self.downscale_factor}" / filepath.name
-        return self.config.data / filepath
+        return dataparser_outputs
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/dataparsers/record3d_dataparser.py` & `nerfstudio-0.2.0/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,153 +8,170 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Data parser for record3d dataset"""
-from __future__ import annotations
-
+"""Data parser for ScanNet dataset"""
+import math
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
+import cv2
 import numpy as np
 import torch
-from rich.console import Console
-from scipy.spatial.transform import Rotation
 from typing_extensions import Literal
 
 from nerfstudio.cameras import camera_utils
 from nerfstudio.cameras.cameras import Cameras, CameraType
 from nerfstudio.data.dataparsers.base_dataparser import (
     DataParser,
     DataParserConfig,
     DataparserOutputs,
 )
 from nerfstudio.data.scene_box import SceneBox
-from nerfstudio.utils import poses as pose_utils
-from nerfstudio.utils.io import load_from_json
-
-CONSOLE = Console(width=120)
 
 
 @dataclass
-class Record3DDataParserConfig(DataParserConfig):
-    """Record3D dataset config"""
+class ScanNetDataParserConfig(DataParserConfig):
+    """ScanNet dataset config.
+    ScanNet dataset (https://www.scan-net.org/) is a large-scale 3D dataset of indoor scenes.
+    This dataparser assumes that the dense stream was extracted from .sens files.
+    Expected structure of scene directory:
+
+    .. code-block:: text
+
+        root/
+        ├── color/
+        ├── depth/
+        ├── intrinsic/
+        ├── pose/
+    """
 
-    _target: Type = field(default_factory=lambda: Record3D)
+    _target: Type = field(default_factory=lambda: ScanNet)
     """target class to instantiate"""
-    data: Path = Path("data/record3d/bear")
-    """Location of data"""
-    val_skip: int = 8
-    """1/val_skip images to use for validation."""
-    aabb_scale: float = 4.0
-    """Scene scale."""
-    orientation_method: Literal["pca", "up"] = "up"
-    """The method to use for orientation"""
-    max_dataset_size: int = 300
-    """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
-    use all images."""
+    data: Path = Path("data/scannet/scene0423_02")
+    """Path to ScanNet folder with densely extracted scenes."""
+    scale_factor: float = 1.0
+    """How much to scale the camera origins by."""
+    scene_scale: float = 1.0
+    """How much to scale the region of interest by."""
+    center_method: Literal["poses", "focus", "none"] = "poses"
+    """The method to use to center the poses."""
+    auto_scale_poses: bool = True
+    """Whether to automatically scale the poses to fit in +/- 1 bounding box."""
+    train_split_fraction: float = 0.9
+    """The fraction of images to use for training. The remaining images are for eval."""
+    depth_unit_scale_factor: float = 1e-3
+    """Scales the depth values to meters. Default value is 0.001 for a millimeter to meter conversion."""
 
 
 @dataclass
-class Record3D(DataParser):
-    """Record3D Dataset"""
-
-    config: Record3DDataParserConfig
-
-    def _generate_dataparser_outputs(self, split: str = "train") -> DataparserOutputs:
-
-        CONSOLE.print(
-            "[bold red]DEPRECATION WARNING: The Record3D dataparser will be deprecated in future versions. "
-            "Use `ns-data-process record3d` to convert the data into the nerfstudio format instead."
-        )
+class ScanNet(DataParser):
+    """ScanNet DatasetParser"""
 
-        image_dir = self.config.data / "rgb"
+    config: ScanNetDataParserConfig
 
-        if not image_dir.exists():
-            raise ValueError(f"Image directory {image_dir} doesn't exist")
+    def _generate_dataparser_outputs(self, split="train"):
+        image_dir = self.config.data / "color"
+        depth_dir = self.config.data / "depth"
+        pose_dir = self.config.data / "pose"
+
+        img_dir_sorted = list(sorted(image_dir.iterdir(), key=lambda x: int(x.name.split(".")[0])))
+        depth_dir_sorted = list(sorted(depth_dir.iterdir(), key=lambda x: int(x.name.split(".")[0])))
+        pose_dir_sorted = list(sorted(pose_dir.iterdir(), key=lambda x: int(x.name.split(".")[0])))
+
+        first_img = cv2.imread(img_dir_sorted[0].as_posix())
+        h, w, _ = first_img.shape
+
+        image_filenames, depth_filenames, intrinsics, poses = [], [], [], []
+
+        K = np.loadtxt(self.config.data / "intrinsic" / "intrinsic_color.txt")
+        for img, depth, pose in zip(img_dir_sorted, depth_dir_sorted, pose_dir_sorted):
+            pose = np.loadtxt(pose)
+            pose[0:3, 1:3] *= -1
+            pose = pose[np.array([1, 0, 2, 3]), :]
+            pose[2, :] *= -1
+
+            # We cannot accept files directly, as some of the poses are invalid
+            if np.isinf(pose).any():
+                continue
+
+            poses.append(pose)
+            intrinsics.append(K)
+            image_filenames.append(img)
+            depth_filenames.append(depth)
 
-        image_filenames = []
-        for f in image_dir.iterdir():
-            if f.stem.isdigit():  # removes possible duplicate images (for example, 123(3).jpg)
-                image_filenames.append(f)
-
-        image_filenames = sorted(image_filenames, key=lambda fn: int(fn.stem))
-        image_filenames = np.array(image_filenames)
+        # filter image_filenames and poses based on train/eval split percentage
         num_images = len(image_filenames)
+        num_train_images = math.ceil(num_images * self.config.train_split_fraction)
+        num_eval_images = num_images - num_train_images
+        i_all = np.arange(num_images)
+        i_train = np.linspace(
+            0, num_images - 1, num_train_images, dtype=int
+        )  # equally spaced training images starting and ending at 0 and num_images-1
+        i_eval = np.setdiff1d(i_all, i_train)  # eval images are the remaining images
+        assert len(i_eval) == num_eval_images
+        if split == "train":
+            indices = i_train
+        elif split in ["val", "test"]:
+            indices = i_eval
+        else:
+            raise ValueError(f"Unknown dataparser split {split}")
+
+        poses = torch.from_numpy(np.stack(poses).astype(np.float32))
+        intrinsics = torch.from_numpy(np.stack(intrinsics).astype(np.float32))
+
+        poses, transform_matrix = camera_utils.auto_orient_and_center_poses(
+            poses,
+            method="none",
+            center_method=self.config.center_method,
+        )
 
-        metadata_path = self.config.data / "metadata.json"
-        metadata_dict = load_from_json(metadata_path)
-
-        poses_data = np.array(metadata_dict["poses"])
-        # (N, 3, 4)
-        poses = np.concatenate(
-            [Rotation.from_quat(poses_data[:, :4]).as_matrix(), poses_data[:, 4:, None]],
-            axis=-1,
-        ).astype(np.float32)
-
-        if self.config.max_dataset_size != -1 and num_images > self.config.max_dataset_size:
-            # Evenly select max_dataset_size images from dataset, including first
-            # and last indices.
-            idx = np.round(np.linspace(0, num_images - 1, self.config.max_dataset_size)).astype(int)
-            poses = poses[idx]
-            image_filenames = image_filenames[idx]
-            num_images = len(image_filenames)
-
-        idx_test = np.arange(num_images)[:: self.config.val_skip]
-        idx_train = np.array([i for i in np.arange(num_images) if i not in idx_test])
-        idx = idx_train if split == "train" else idx_test
-        if num_images != poses.shape[0]:
-            raise RuntimeError(f"Different number of images ({num_images}), and poses ({poses.shape[0]})")
-
-        image_filenames = image_filenames[idx]
-        poses = poses[idx]
-
-        # convert to Tensors
-        poses = torch.from_numpy(poses[:, :3, :4])
-
-        poses = camera_utils.auto_orient_and_center_poses(
-            pose_utils.to4x4(poses), method=self.config.orientation_method
-        )[:, :3, :4]
-
-        # Centering poses
-        poses[:, :3, 3] = poses[:, :3, 3] - torch.mean(poses[:, :3, 3], dim=0)
-        poses = pose_utils.normalize(poses)
-
-        # Camera intrinsics
-        K = np.array(metadata_dict["K"]).reshape((3, 3)).T
-        focal_length = K[0, 0]
-
-        H = metadata_dict["h"]
-        W = metadata_dict["w"]
-
-        # TODO(akristoffersen): The metadata dict comes with principle points,
-        # but caused errors in image coord indexing. Should update once that is fixed.
-        cx, cy = W / 2, H / 2
-
-        num_cameras = len(image_filenames)
-        num_intrinsics_params = 3
-        intrinsics = torch.ones((num_cameras, num_intrinsics_params), dtype=torch.float32)
-        intrinsics *= torch.tensor([cx, cy, focal_length])
-
-        aabb = torch.tensor([[-1, -1, -1], [1, 1, 1]], dtype=torch.float32) * self.config.aabb_scale
-        scene_box = SceneBox(aabb=aabb)
+        # Scale poses
+        scale_factor = 1.0
+        if self.config.auto_scale_poses:
+            scale_factor /= float(torch.max(torch.abs(poses[:, :3, 3])))
+        scale_factor *= self.config.scale_factor
+
+        poses[:, :3, 3] *= scale_factor
+
+        # Choose image_filenames and poses based on split, but after auto orient and scaling the poses.
+        image_filenames = [image_filenames[i] for i in indices]
+        depth_filenames = [depth_filenames[i] for i in indices] if len(depth_filenames) > 0 else []
+        intrinsics = intrinsics[indices.tolist()]
+        poses = poses[indices.tolist()]
+
+        # in x,y,z order
+        # assumes that the scene is centered at the origin
+        aabb_scale = self.config.scene_scale
+        scene_box = SceneBox(
+            aabb=torch.tensor(
+                [[-aabb_scale, -aabb_scale, -aabb_scale], [aabb_scale, aabb_scale, aabb_scale]], dtype=torch.float32
+            )
+        )
 
         cameras = Cameras(
-            fx=focal_length,
-            fy=focal_length,
-            cx=cx,
-            cy=cy,
-            camera_to_worlds=poses,
+            fx=intrinsics[:, 0, 0],
+            fy=intrinsics[:, 1, 1],
+            cx=intrinsics[:, 0, 2],
+            cy=intrinsics[:, 1, 2],
+            height=h,
+            width=w,
+            camera_to_worlds=poses[:, :3, :4],
             camera_type=CameraType.PERSPECTIVE,
         )
 
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
             scene_box=scene_box,
+            dataparser_scale=scale_factor,
+            dataparser_transform=transform_matrix,
+            metadata={
+                "depth_filenames": depth_filenames if len(depth_filenames) > 0 else None,
+                "depth_unit_scale_factor": self.config.depth_unit_scale_factor,
+            },
         )
-
         return dataparser_outputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datasets/__init__.py` & `nerfstudio-0.2.0/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-0.2.0/nerfstudio/data/datasets/base_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 # limitations under the License.
 
 """
 Dataset.
 """
 from __future__ import annotations
 
-from typing import Dict
+from copy import deepcopy
+from pathlib import Path
+from typing import Dict, List
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from PIL import Image
 from torch.utils.data import Dataset
 from torchtyping import TensorType
@@ -31,64 +33,79 @@
 
 
 class InputDataset(Dataset):
     """Dataset that returns images.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
+        scale_factor: The scaling factor for the dataparser outputs
     """
 
-    def __init__(self, dataparser_outputs: DataparserOutputs):
+    def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
         super().__init__()
-        self.dataparser_outputs = dataparser_outputs
-        self.has_masks = self.dataparser_outputs.mask_filenames is not None
+        self._dataparser_outputs = dataparser_outputs
+        self.has_masks = dataparser_outputs.mask_filenames is not None
+        self.scale_factor = scale_factor
+        self.scene_box = deepcopy(dataparser_outputs.scene_box)
+        self.metadata = deepcopy(dataparser_outputs.metadata)
+        self.cameras = deepcopy(dataparser_outputs.cameras)
+        self.cameras.rescale_output_resolution(scaling_factor=scale_factor)
 
     def __len__(self):
-        return len(self.dataparser_outputs.image_filenames)
+        return len(self._dataparser_outputs.image_filenames)
 
     def get_numpy_image(self, image_idx: int) -> npt.NDArray[np.uint8]:
         """Returns the image of shape (H, W, 3 or 4).
 
         Args:
             image_idx: The image index in the dataset.
         """
-        image_filename = self.dataparser_outputs.image_filenames[image_idx]
+        image_filename = self._dataparser_outputs.image_filenames[image_idx]
         pil_image = Image.open(image_filename)
-        image = np.array(pil_image, dtype="uint8")  # shape is (h, w, 3 or 4)
+        if self.scale_factor != 1.0:
+            width, height = pil_image.size
+            newsize = (int(width * self.scale_factor), int(height * self.scale_factor))
+            pil_image = pil_image.resize(newsize, resample=Image.BILINEAR)
+        image = np.array(pil_image, dtype="uint8")  # shape is (h, w) or (h, w, 3 or 4)
+        if len(image.shape) == 2:
+            image = image[:, :, None].repeat(3, axis=2)
         assert len(image.shape) == 3
         assert image.dtype == np.uint8
         assert image.shape[2] in [3, 4], f"Image shape of {image.shape} is in correct."
         return image
 
     def get_image(self, image_idx: int) -> TensorType["image_height", "image_width", "num_channels"]:
         """Returns a 3 channel image.
 
         Args:
             image_idx: The image index in the dataset.
         """
         image = torch.from_numpy(self.get_numpy_image(image_idx).astype("float32") / 255.0)
-        if self.dataparser_outputs.alpha_color is not None and image.shape[-1] == 4:
+        if self._dataparser_outputs.alpha_color is not None and image.shape[-1] == 4:
             assert image.shape[-1] == 4
-            image = image[:, :, :3] * image[:, :, -1:] + self.dataparser_outputs.alpha_color * (1.0 - image[:, :, -1:])
+            image = image[:, :, :3] * image[:, :, -1:] + self._dataparser_outputs.alpha_color * (1.0 - image[:, :, -1:])
         else:
             image = image[:, :, :3]
         return image
 
     def get_data(self, image_idx: int) -> Dict:
         """Returns the ImageDataset data as a dictionary.
 
         Args:
             image_idx: The image index in the dataset.
         """
         image = self.get_image(image_idx)
         data = {"image_idx": image_idx}
         data["image"] = image
         if self.has_masks:
-            mask_filepath = self.dataparser_outputs.mask_filenames[image_idx]
-            data["mask"] = get_image_mask_tensor_from_path(filepath=mask_filepath)
+            mask_filepath = self._dataparser_outputs.mask_filenames[image_idx]
+            data["mask"] = get_image_mask_tensor_from_path(filepath=mask_filepath, scale_factor=self.scale_factor)
+            assert (
+                data["mask"].shape[:2] == data["image"].shape[:2]
+            ), f"Mask and image have different shapes. Got {data['mask'].shape[:2]} and {data['image'].shape[:2]}"
         metadata = self.get_metadata(data)
         data.update(metadata)
         return data
 
     # pylint: disable=no-self-use
     def get_metadata(self, data: Dict) -> Dict:
         """Method that can be used to process any additional metadata that may be part of the model inputs.
@@ -98,7 +115,16 @@
         """
         del data
         return {}
 
     def __getitem__(self, image_idx: int) -> Dict:
         data = self.get_data(image_idx)
         return data
+
+    @property
+    def image_filenames(self) -> List[Path]:
+        """
+        Returns image filenames for this dataset.
+        The order of filenames is the same as in the Cameras object for easy mapping.
+        """
+
+        return self._dataparser_outputs.image_filenames
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-0.2.0/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,26 +28,24 @@
 class SemanticDataset(InputDataset):
     """Dataset that returns images and semantics and masks.
 
     Args:
         dataparser_outputs: description of where and how to read input images.
     """
 
-    def __init__(self, dataparser_outputs: DataparserOutputs):
-        super().__init__(dataparser_outputs)
-        assert "semantics" in dataparser_outputs.metadata.keys() and isinstance(
-            dataparser_outputs.metadata["semantics"], Semantics
-        )
-        self.semantics = dataparser_outputs.metadata["semantics"]
+    def __init__(self, dataparser_outputs: DataparserOutputs, scale_factor: float = 1.0):
+        super().__init__(dataparser_outputs, scale_factor)
+        assert "semantics" in dataparser_outputs.metadata.keys() and isinstance(self.metadata["semantics"], Semantics)
+        self.semantics = self.metadata["semantics"]
         self.mask_indices = torch.tensor(
             [self.semantics.classes.index(mask_class) for mask_class in self.semantics.mask_classes]
         ).view(1, 1, -1)
 
     def get_metadata(self, data: Dict) -> Dict:
         # handle mask
         filepath = self.semantics.filenames[data["image_idx"]]
         semantic_label, mask = get_semantics_and_mask_tensors_from_path(
-            filepath=filepath, mask_indices=self.mask_indices
+            filepath=filepath, mask_indices=self.mask_indices, scale_factor=self.scale_factor
         )
         if "mask" in data.keys():
             mask = mask & data["mask"]
         return {"mask": mask, "semantics": semantic_label}
```

### Comparing `nerfstudio-0.1.9/nerfstudio/data/utils/__init__.py` & `nerfstudio-0.2.0/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-0.2.0/nerfstudio/data/utils/dataloaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,55 +12,64 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Code for sampling images from a dataset of images.
 """
 
+# for multithreading
+import concurrent.futures
+import multiprocessing
 import random
 from abc import abstractmethod
 from typing import Dict, Optional, Tuple, Union
 
 import torch
 from rich.progress import Console, track
-from torch.utils.data import Dataset, default_collate
+from torch.utils.data import Dataset
 from torch.utils.data.dataloader import DataLoader
 
 from nerfstudio.cameras.cameras import Cameras
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.data.datasets.base_dataset import InputDataset
+from nerfstudio.data.utils.nerfstudio_collate import nerfstudio_collate
 from nerfstudio.utils.misc import get_dict_to_torch
 
 CONSOLE = Console(width=120)
 
 
 class CacheDataloader(DataLoader):
     """Collated image dataset that implements caching of default-pytorch-collatable data.
     Creates batches of the InputDataset return type.
 
     Args:
         dataset: Dataset to sample from.
         num_samples_to_collate: How many images to sample rays for each batch. -1 for all images.
         num_times_to_repeat_images: How often to collate new images. -1 to never pick new images.
         device: Device to perform computation.
+        collate_fn: The function we will use to collate our training data
     """
 
     def __init__(
         self,
         dataset: Dataset,
         num_images_to_sample_from: int = -1,
         num_times_to_repeat_images: int = -1,
         device: Union[torch.device, str] = "cpu",
+        collate_fn=nerfstudio_collate,
         **kwargs,
     ):
         self.dataset = dataset
+        super().__init__(dataset=dataset, **kwargs)  # This will set self.dataset
         self.num_times_to_repeat_images = num_times_to_repeat_images
         self.cache_all_images = (num_images_to_sample_from == -1) or (num_images_to_sample_from >= len(self.dataset))
         self.num_images_to_sample_from = len(self.dataset) if self.cache_all_images else num_images_to_sample_from
         self.device = device
+        self.collate_fn = collate_fn
+        self.num_workers = kwargs.get("num_workers", 0)
 
         self.num_repeated = self.num_times_to_repeat_images  # starting value
         self.first_time = True
 
         self.cached_collated_batch = None
         if self.cache_all_images:
             CONSOLE.print(f"Caching all {len(self.dataset)} images.")
@@ -74,31 +83,43 @@
                 f"Caching {self.num_images_to_sample_from} out of {len(self.dataset)} images, without resampling."
             )
         else:
             CONSOLE.print(
                 f"Caching {self.num_images_to_sample_from} out of {len(self.dataset)} images, "
                 f"resampling every {self.num_times_to_repeat_images} iters."
             )
-        super().__init__(dataset=dataset, **kwargs)
 
     def __getitem__(self, idx):
         return self.dataset.__getitem__(idx)
 
     def _get_batch_list(self):
         """Returns a list of batches from the dataset attribute."""
+
         indices = random.sample(range(len(self.dataset)), k=self.num_images_to_sample_from)
         batch_list = []
-        for idx in track(indices, description="Loading data batch"):
-            batch_list.append(self.dataset.__getitem__(idx))
+        results = []
+
+        num_threads = int(self.num_workers) * 4
+        num_threads = min(num_threads, multiprocessing.cpu_count() - 1)
+        num_threads = max(num_threads, 1)
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=num_threads) as executor:
+            for idx in indices:
+                res = executor.submit(self.dataset.__getitem__, idx)
+                results.append(res)
+
+            for res in track(results, description="Loading data batch", transient=True):
+                batch_list.append(res.result())
+
         return batch_list
 
     def _get_collated_batch(self):
         """Returns a collated batch."""
         batch_list = self._get_batch_list()
-        collated_batch = default_collate(batch_list)
+        collated_batch = self.collate_fn(batch_list)
         collated_batch = get_dict_to_torch(collated_batch, device=self.device, exclude=["image"])
         return collated_batch
 
     def __iter__(self):
         while True:
             if self.cache_all_images:
                 collated_batch = self.cached_collated_batch
@@ -128,15 +149,15 @@
     def __init__(
         self,
         input_dataset: InputDataset,
         device: Union[torch.device, str] = "cpu",
         **kwargs,
     ):
         self.input_dataset = input_dataset
-        self.cameras = input_dataset.dataparser_outputs.cameras.to(device)
+        self.cameras = input_dataset.cameras.to(device)
         self.device = device
         self.kwargs = kwargs
         super().__init__(dataset=input_dataset)
 
     @abstractmethod
     def __iter__(self):
         """Iterates over the dataset"""
@@ -148,38 +169,23 @@
 
     def get_camera(self, image_idx: int = 0) -> Cameras:
         """Get camera for the given image index
 
         Args:
             image_idx: Camera image index
         """
-        distortion_params = None
-        if self.cameras.distortion_params is not None:
-            distortion_params = self.cameras.distortion_params[image_idx]
-
-        camera = Cameras(
-            fx=self.cameras.fx[image_idx : image_idx + 1],
-            fy=self.cameras.fy[image_idx : image_idx + 1],
-            cx=self.cameras.cx[image_idx : image_idx + 1],
-            cy=self.cameras.cy[image_idx : image_idx + 1],
-            height=self.cameras.image_height[image_idx : image_idx + 1],
-            width=self.cameras.image_width[image_idx : image_idx + 1],
-            camera_to_worlds=self.cameras.camera_to_worlds[image_idx : image_idx + 1],
-            distortion_params=distortion_params,
-            camera_type=self.cameras.camera_type[image_idx : image_idx + 1],
-        )
-        return camera
+        return self.cameras[image_idx]
 
     def get_data_from_image_idx(self, image_idx: int) -> Tuple[RayBundle, Dict]:
         """Returns the data for a specific image index.
 
         Args:
             image_idx: Camera image index
         """
-        ray_bundle = self.cameras.generate_rays(camera_indices=image_idx)
+        ray_bundle = self.cameras.generate_rays(camera_indices=image_idx, keep_shape=True)
         batch = self.input_dataset[image_idx]
         batch = get_dict_to_torch(batch, device=self.device, exclude=["image"])
         return ray_bundle, batch
 
 
 class FixedIndicesEvalDataloader(EvalDataloader):
     """Dataloader that returns a fixed set of indices.
```

### Comparing `nerfstudio-0.1.9/nerfstudio/engine/__init__.py` & `nerfstudio-0.2.0/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/engine/callbacks.py` & `nerfstudio-0.2.0/nerfstudio/engine/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Callback code used for training iterations
 """
+from __future__ import annotations
 
 from dataclasses import InitVar, dataclass
 from enum import Enum, auto
 from inspect import signature
 from typing import Callable, Dict, List, Optional, Tuple
 
-from nerfstudio.configs.base_config import TrainerConfig
-
 
 @dataclass
 class TrainingCallbackAttributes:
     """Attributes that can be used to configure training callbacks.
     The callbacks can be specified in the Dataloader or Model implementations.
     Instead of providing access to the entire Trainer object, we only provide these attributes.
     This should be least prone to errors and fairly clean from a user perspective."""
@@ -34,16 +33,14 @@
     # TODO(ethan): type this without circular imports
     optimizers: Optional[InitVar]
     """optimizers for training"""
     grad_scaler: Optional[InitVar]
     """gradient scalers"""
     pipeline: Optional[InitVar]
     """reference to training pipeline"""
-    config: TrainerConfig
-    """the trainer config"""
 
 
 class TrainingCallbackLocation(Enum):
     """Enum for specifying where the training callback should be run."""
 
     BEFORE_TRAIN_ITERATION = auto()
     AFTER_TRAIN_ITERATION = auto()
@@ -51,15 +48,15 @@
 
 class TrainingCallback:
     """Callback class used during training.
     The function 'func' with 'args' and 'kwargs' will be called every 'update_every_num_iters' training iterations,
     including at iteration 0. The function is called after the training iteration.
 
     Args:
-        where_to_run: List of locations for when to run callbak (before/after iteration)
+        where_to_run: List of locations for when to run callback (before/after iteration)
         func: The function that will be called.
         update_every_num_iters: How often to call the function `func`.
         iters: Tuple of iteration steps to perform callback
         args: args for the function 'func'.
         kwargs: kwargs for the function 'func'.
     """
 
@@ -78,28 +75,28 @@
         self.where_to_run = where_to_run
         self.update_every_num_iters = update_every_num_iters
         self.iters = iters
         self.func = func
         self.args = args if args is not None else []
         self.kwargs = kwargs if kwargs is not None else {}
 
-    def run_callback(self, step: int):
+    def run_callback(self, step: int) -> None:
         """Callback to run after training step
 
         Args:
             step: current iteration step
         """
         if self.update_every_num_iters is not None:
             if step % self.update_every_num_iters == 0:
                 self.func(*self.args, **self.kwargs, step=step)
         elif self.iters is not None:
             if step in self.iters:
                 self.func(*self.args, **self.kwargs, step=step)
 
-    def run_callback_at_location(self, step: int, location: TrainingCallbackLocation):
+    def run_callback_at_location(self, step: int, location: TrainingCallbackLocation) -> None:
         """Runs the callback if it's supposed to be run at the given location.
 
         Args:
             step: current iteration step
             location: when to run callback (before/after iteration)
         """
         if location in self.where_to_run:
```

### Comparing `nerfstudio-0.1.9/nerfstudio/engine/optimizers.py` & `nerfstudio-0.2.0/nerfstudio/engine/optimizers.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """
 Optimizers class.
 """
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type
 
 import torch
 from torch.cuda.amp.grad_scaler import GradScaler
 from torch.nn.parameter import Parameter
 
 from nerfstudio.configs import base_config
 from nerfstudio.utils import writer
@@ -30,82 +30,72 @@
 
 # Optimizer related configs
 @dataclass
 class OptimizerConfig(base_config.PrintableConfig):
     """Basic optimizer config with RAdam"""
 
     _target: Type = torch.optim.Adam
+    """The optimizer class to use."""
     lr: float = 0.0005
+    """The learning rate to use."""
     eps: float = 1e-08
+    """The epsilon value to use."""
+    max_norm: Optional[float] = None
+    """The max norm to use for gradient clipping."""
 
     # TODO: somehow make this more generic. i dont like the idea of overriding the setup function
     # but also not sure how to go about passing things into predefined torch objects.
-    def setup(self, params) -> Any:
+    def setup(self, params) -> torch.optim.Optimizer:
         """Returns the instantiated object using the config."""
         kwargs = vars(self).copy()
         kwargs.pop("_target")
+        kwargs.pop("max_norm")
         return self._target(params, **kwargs)
 
 
 @dataclass
 class AdamOptimizerConfig(OptimizerConfig):
     """Basic optimizer config with Adam"""
 
     _target: Type = torch.optim.Adam
     weight_decay: float = 0
+    """The weight decay to use."""
 
 
 @dataclass
 class RAdamOptimizerConfig(OptimizerConfig):
     """Basic optimizer config with RAdam"""
 
     _target: Type = torch.optim.RAdam
-
-
-def setup_optimizers(config: base_config.Config, param_groups: Dict[str, List[Parameter]]) -> "Optimizers":
-    """Helper to set up the optimizers
-
-    Args:
-        config: The trainer configuration object.
-        param_groups: A dictionary of parameter groups to optimize.
-
-    Returns:
-        The optimizers object.
-    """
-    optimizer_config = config.optimizers.copy()
-
-    # Add the camera optimizer if enabled.
-    camera_optimizer_config = config.pipeline.datamanager.camera_optimizer
-    if camera_optimizer_config.mode != "off":
-        assert camera_optimizer_config.param_group not in optimizer_config
-        optimizer_config[camera_optimizer_config.param_group] = {
-            "optimizer": config.pipeline.datamanager.camera_optimizer.optimizer,
-            "scheduler": config.pipeline.datamanager.camera_optimizer.scheduler,
-        }
-    return Optimizers(optimizer_config, param_groups)
+    weight_decay: float = 0
+    """The weight decay to use."""
 
 
 class Optimizers:
     """A set of optimizers.
 
     Args:
         config: The optimizer configuration object.
         param_groups: A dictionary of parameter groups to optimize.
     """
 
-    def __init__(self, config: Dict[str, Any], param_groups: Dict[str, List[Parameter]]):
+    def __init__(self, config: Dict[str, Any], param_groups: Dict[str, List[Parameter]]) -> None:
         self.config = config
         self.optimizers = {}
         self.schedulers = {}
+        self.parameters = {}
         for param_group_name, params in param_groups.items():
             lr_init = config[param_group_name]["optimizer"].lr
             self.optimizers[param_group_name] = config[param_group_name]["optimizer"].setup(params=params)
+            self.parameters[param_group_name] = params
             if config[param_group_name]["scheduler"]:
-                self.schedulers[param_group_name] = config[param_group_name]["scheduler"].setup(
-                    optimizer=self.optimizers[param_group_name], lr_init=lr_init
+                self.schedulers[param_group_name] = (
+                    config[param_group_name]["scheduler"]
+                    .setup()
+                    .get_scheduler(optimizer=self.optimizers[param_group_name], lr_init=lr_init)
                 )
 
     def optimizer_step(self, param_group_name: str) -> None:
         """Fetch and step corresponding optimizer.
 
         Args:
             param_group_name: name of optimizer to step forward
@@ -128,21 +118,28 @@
 
     def optimizer_scaler_step_all(self, grad_scaler: GradScaler) -> None:
         """Take an optimizer step using a grad scaler.
 
         Args:
             grad_scaler: GradScaler to use
         """
-        for _, optimizer in self.optimizers.items():
+        for param_group, optimizer in self.optimizers.items():
+            max_norm = self.config[param_group]["optimizer"].max_norm
+            if max_norm is not None:
+                grad_scaler.unscale_(optimizer)
+                torch.nn.utils.clip_grad_norm_(self.parameters[param_group], max_norm)
             grad_scaler.step(optimizer)
 
-    def optimizer_step_all(self):
+    def optimizer_step_all(self) -> None:
         """Run step for all optimizers."""
-        for _, optimizer in self.optimizers.items():
+        for param_group, optimizer in self.optimizers.items():
             # note that they key is the parameter name
+            max_norm = self.config[param_group]["optimizer"].max_norm
+            if max_norm is not None:
+                torch.nn.utils.clip_grad_norm_(self.parameters[param_group], max_norm)
             optimizer.step()
 
     def scheduler_step_all(self, step: int) -> None:
         """Run step for all schedulers.
 
         Args:
             step: the current step
```

### Comparing `nerfstudio-0.1.9/nerfstudio/engine/trainer.py` & `nerfstudio-0.2.0/nerfstudio/engine/trainer.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,40 +17,80 @@
 """
 from __future__ import annotations
 
 import dataclasses
 import functools
 import os
 import time
-from typing import Dict, List, Tuple
+from dataclasses import dataclass, field
+from pathlib import Path
+from threading import Lock
+from typing import Dict, List, Optional, Tuple, Type, Union
 
 import torch
 from rich.console import Console
 from torch.cuda.amp.grad_scaler import GradScaler
+from typing_extensions import Literal
 
-from nerfstudio.configs import base_config as cfg
+from nerfstudio.configs.experiment_config import ExperimentConfig
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
-from nerfstudio.engine.optimizers import Optimizers, setup_optimizers
+from nerfstudio.engine.optimizers import Optimizers
 from nerfstudio.pipelines.base_pipeline import VanillaPipeline
 from nerfstudio.utils import profiler, writer
 from nerfstudio.utils.decorators import (
     check_eval_enabled,
     check_main_thread,
     check_viewer_enabled,
 )
 from nerfstudio.utils.misc import step_check
 from nerfstudio.utils.writer import EventName, TimeWriter
-from nerfstudio.viewer.server import viewer_utils
+from nerfstudio.viewer.server.viewer_state import ViewerState
 
 CONSOLE = Console(width=120)
 
+TRAIN_INTERATION_OUTPUT = Tuple[  # pylint: disable=invalid-name
+    torch.Tensor, Dict[str, torch.Tensor], Dict[str, torch.Tensor]
+]
+TORCH_DEVICE = Union[torch.device, str]  # pylint: disable=invalid-name
+
+
+@dataclass
+class TrainerConfig(ExperimentConfig):
+    """Configuration for training regimen"""
+
+    _target: Type = field(default_factory=lambda: Trainer)
+    """target class to instantiate"""
+    steps_per_save: int = 1000
+    """Number of steps between saves."""
+    steps_per_eval_batch: int = 500
+    """Number of steps between randomly sampled batches of rays."""
+    steps_per_eval_image: int = 500
+    """Number of steps between single eval images."""
+    steps_per_eval_all_images: int = 25000
+    """Number of steps between eval all images."""
+    max_num_iterations: int = 1000000
+    """Maximum number of iterations to run."""
+    mixed_precision: bool = False
+    """Whether or not to use mixed precision for training."""
+    save_only_latest_checkpoint: bool = True
+    """Whether to only save the latest checkpoint or all checkpoints."""
+    # optional parameters if we want to resume training
+    load_dir: Optional[Path] = None
+    """Optionally specify a pre-trained model directory to load from."""
+    load_step: Optional[int] = None
+    """Optionally specify model step to load from; if none, will find most recent model in load_dir."""
+    load_config: Optional[Path] = None
+    """Path to config YAML file."""
+    log_gradients: bool = False
+    """Optionally log gradients during training"""
+
 
 class Trainer:
     """Trainer class
 
     Args:
         config: The configuration object.
         local_rank: Local rank of the process.
@@ -60,209 +100,265 @@
         config: The configuration object.
         local_rank: Local rank of the process.
         world_size: World size of the process.
         device: The device to run the training on.
         pipeline: The pipeline object.
         optimizers: The optimizers object.
         callbacks: The callbacks object.
+        is_training: Whether the model is training.
     """
 
     pipeline: VanillaPipeline
     optimizers: Optimizers
     callbacks: List[TrainingCallback]
 
-    def __init__(self, config: cfg.Config, local_rank: int = 0, world_size: int = 1):
+    def __init__(self, config: TrainerConfig, local_rank: int = 0, world_size: int = 1) -> None:
+        self.train_lock = Lock()
         self.config = config
         self.local_rank = local_rank
         self.world_size = world_size
-        self.device = "cpu" if world_size == 0 else f"cuda:{local_rank}"
-        self.mixed_precision = self.config.trainer.mixed_precision
+        self.device: TORCH_DEVICE = "cpu" if world_size == 0 else f"cuda:{local_rank}"
+        self.mixed_precision: bool = self.config.mixed_precision
+        self.is_training: bool = True
         if self.device == "cpu":
             self.mixed_precision = False
             CONSOLE.print("Mixed precision is disabled for CPU training.")
-        self._start_step = 0
+        self._start_step: int = 0
         # optimizers
         self.grad_scaler = GradScaler(enabled=self.mixed_precision)
 
-        self.base_dir = config.get_base_dir()
+        self.base_dir: Path = config.get_base_dir()
         # directory to save checkpoints
-        self.checkpoint_dir = config.get_checkpoint_dir()
+        self.checkpoint_dir: Path = config.get_checkpoint_dir()
         CONSOLE.log(f"Saving checkpoints to: {self.checkpoint_dir}")
-        # set up viewer if enabled
-        viewer_log_path = self.base_dir / config.viewer.relative_log_filename
-        self.viewer_state, banner_messages = None, None
-        if self.config.is_viewer_enabled() and local_rank == 0:
-            self.viewer_state, banner_messages = viewer_utils.setup_viewer(config.viewer, log_filename=viewer_log_path)
-        self._check_viewer_warnings()
-        # set up writers/profilers if enabled
-        writer_log_path = self.base_dir / config.logging.relative_log_dir
-        writer.setup_event_writer(config, log_dir=writer_log_path)
-        writer.setup_local_writer(
-            config.logging, max_iter=config.trainer.max_num_iterations, banner_messages=banner_messages
-        )
-        writer.put_config(name="config", config_dict=dataclasses.asdict(config), step=0)
-        profiler.setup_profiler(config.logging)
 
-    def setup(self, test_mode=False):
+        self.viewer_state = None
+
+    def setup(self, test_mode: Literal["test", "val", "inference"] = "val") -> None:
         """Setup the Trainer by calling other setup functions.
 
         Args:
-            test_mode: Whether to setup for testing. Defaults to False.
+            test_mode:
+                'val': loads train/val datasets into memory
+                'test': loads train/test datasets into memory
+                'inference': does not load any dataset into memory
         """
         self.pipeline = self.config.pipeline.setup(
             device=self.device, test_mode=test_mode, world_size=self.world_size, local_rank=self.local_rank
         )
-        self.optimizers = setup_optimizers(self.config, self.pipeline.get_param_groups())
+        self.optimizers = self.setup_optimizers()
+
+        # set up viewer if enabled
+        viewer_log_path = self.base_dir / self.config.viewer.relative_log_filename
+        self.viewer_state, banner_messages = None, None
+        if self.config.is_viewer_enabled() and self.local_rank == 0:
+            datapath = self.config.data
+            if datapath is None:
+                datapath = self.base_dir
+            self.viewer_state = ViewerState(
+                self.config.viewer,
+                log_filename=viewer_log_path,
+                datapath=datapath,
+                pipeline=self.pipeline,
+                trainer=self,
+                train_lock=self.train_lock,
+            )
+            banner_messages = [f"Viewer at: {self.viewer_state.viewer_url}"]
+        self._check_viewer_warnings()
 
         self._load_checkpoint()
 
         self.callbacks = self.pipeline.get_training_callbacks(
             TrainingCallbackAttributes(
                 optimizers=self.optimizers,  # type: ignore
                 grad_scaler=self.grad_scaler,  # type: ignore
                 pipeline=self.pipeline,  # type: ignore
-                config=self.config.trainer,  # type: ignore
             )
         )
 
+        # set up writers/profilers if enabled
+        writer_log_path = self.base_dir / self.config.logging.relative_log_dir
+        writer.setup_event_writer(
+            self.config.is_wandb_enabled(), self.config.is_tensorboard_enabled(), log_dir=writer_log_path
+        )
+        writer.setup_local_writer(
+            self.config.logging, max_iter=self.config.max_num_iterations, banner_messages=banner_messages
+        )
+        writer.put_config(name="config", config_dict=dataclasses.asdict(self.config), step=0)
+        profiler.setup_profiler(self.config.logging)
+
+    def setup_optimizers(self) -> Optimizers:
+        """Helper to set up the optimizers
+
+        Returns:
+            The optimizers object given the trainer config.
+        """
+        optimizer_config = self.config.optimizers.copy()
+        param_groups = self.pipeline.get_param_groups()
+        camera_optimizer_config = self.config.pipeline.datamanager.camera_optimizer
+        if camera_optimizer_config is not None and camera_optimizer_config.mode != "off":
+            assert camera_optimizer_config.param_group not in optimizer_config
+            optimizer_config[camera_optimizer_config.param_group] = {
+                "optimizer": camera_optimizer_config.optimizer,
+                "scheduler": camera_optimizer_config.scheduler,
+            }
+        return Optimizers(optimizer_config, param_groups)
+
     def train(self) -> None:
         """Train the model."""
         assert self.pipeline.datamanager.train_dataset is not None, "Missing DatsetInputs"
 
+        self.pipeline.datamanager.train_dataparser_outputs.save_dataparser_transform(
+            self.base_dir / "dataparser_transforms.json"
+        )
+
         self._init_viewer_state()
         with TimeWriter(writer, EventName.TOTAL_TRAIN_TIME):
-            num_iterations = self.config.trainer.max_num_iterations
+            num_iterations = self.config.max_num_iterations
+            step = 0
             for step in range(self._start_step, self._start_step + num_iterations):
-                with TimeWriter(writer, EventName.ITER_TRAIN_TIME, step=step) as train_t:
-
-                    self.pipeline.train()
-
-                    # training callbacks before the training iteration
-                    for callback in self.callbacks:
-                        callback.run_callback_at_location(
-                            step, location=TrainingCallbackLocation.BEFORE_TRAIN_ITERATION
-                        )
-
-                    # time the forward pass
-                    loss, loss_dict, metrics_dict = self.train_iteration(step)
-
-                    # training callbacks after the training iteration
-                    for callback in self.callbacks:
-                        callback.run_callback_at_location(step, location=TrainingCallbackLocation.AFTER_TRAIN_ITERATION)
+                while not self.is_training:
+                    time.sleep(0.01)
+                with self.train_lock:
+                    with TimeWriter(writer, EventName.ITER_TRAIN_TIME, step=step) as train_t:
+                        self.pipeline.train()
+
+                        # training callbacks before the training iteration
+                        for callback in self.callbacks:
+                            callback.run_callback_at_location(
+                                step, location=TrainingCallbackLocation.BEFORE_TRAIN_ITERATION
+                            )
+
+                        # time the forward pass
+                        loss, loss_dict, metrics_dict = self.train_iteration(step)
+
+                        # training callbacks after the training iteration
+                        for callback in self.callbacks:
+                            callback.run_callback_at_location(
+                                step, location=TrainingCallbackLocation.AFTER_TRAIN_ITERATION
+                            )
 
                 # Skip the first two steps to avoid skewed timings that break the viewer rendering speed estimate.
                 if step > 1:
                     writer.put_time(
                         name=EventName.TRAIN_RAYS_PER_SEC,
-                        duration=self.config.pipeline.datamanager.train_num_rays_per_batch / train_t.duration,
+                        duration=self.pipeline.datamanager.get_train_rays_per_batch() / train_t.duration,
                         step=step,
                         avg_over_steps=True,
                     )
 
                 self._update_viewer_state(step)
 
                 # a batch of train rays
                 if step_check(step, self.config.logging.steps_per_log, run_at_zero=True):
                     writer.put_scalar(name="Train Loss", scalar=loss, step=step)
                     writer.put_dict(name="Train Loss Dict", scalar_dict=loss_dict, step=step)
                     writer.put_dict(name="Train Metrics Dict", scalar_dict=metrics_dict, step=step)
+                    # The actual memory allocated by Pytorch. This is likely less than the amount
+                    # shown in nvidia-smi since some unused memory can be held by the caching
+                    # allocator and some context needs to be created on GPU. See Memory management
+                    # (https://pytorch.org/docs/stable/notes/cuda.html#cuda-memory-management)
+                    # for more details about GPU memory management.
+                    writer.put_scalar(
+                        name="GPU Memory (MB)", scalar=torch.cuda.max_memory_allocated() / (1024**2), step=step
+                    )
 
-                self.eval_iteration(step)
+                # Do not perform evaluation if there are no validation images
+                if self.pipeline.datamanager.eval_dataset:
+                    self.eval_iteration(step)
 
-                if step_check(step, self.config.trainer.steps_per_save):
+                if step_check(step, self.config.steps_per_save):
                     self.save_checkpoint(step)
 
                 writer.write_out_storage()
-            # save checkpoint at the end of training
-            self.save_checkpoint(step)
-            CONSOLE.rule()
-            CONSOLE.print("[bold green]:tada: :tada: :tada: Training Finished :tada: :tada: :tada:", justify="center")
-            CONSOLE.print("Use ctrl+c to quit", justify="center")
-            self._always_render(step)
 
-    @check_main_thread
-    def _always_render(self, step):
-        if self.config.is_viewer_enabled():
+        # save checkpoint at the end of training
+        self.save_checkpoint(step)
+
+        # write out any remaining events (e.g., total train time)
+        writer.write_out_storage()
+
+        CONSOLE.rule()
+        CONSOLE.print("[bold green]:tada: :tada: :tada: Training Finished :tada: :tada: :tada:", justify="center")
+        if not self.config.viewer.quit_on_train_completion:
+            CONSOLE.print("Use ctrl+c to quit", justify="center")
             while True:
-                self.viewer_state.vis["renderingState/isTraining"].write(False)
-                self._update_viewer_state(step)
+                time.sleep(0.01)
 
     @check_main_thread
     def _check_viewer_warnings(self) -> None:
         """Helper to print out any warnings regarding the way the viewer/loggers are enabled"""
-        if self.config.is_viewer_enabled():
-            string = (
-                "[WARNING] Not running eval iterations since only viewer is enabled."
-                " Use `--vis wandb` or `--vis tensorboard` to run with eval instead."
+        if (
+            self.config.is_viewer_enabled()
+            and not self.config.is_tensorboard_enabled()
+            and not self.config.is_wandb_enabled()
+        ):
+            string: str = (
+                "[NOTE] Not running eval iterations since only viewer is enabled.\n"
+                "Use [yellow]--vis {wandb, tensorboard, viewer+wandb, viewer+tensorboard}[/yellow] to run with eval."
             )
-            CONSOLE.print(f"[bold red]{string}")
+            CONSOLE.print(f"{string}")
 
     @check_viewer_enabled
     def _init_viewer_state(self) -> None:
         """Initializes viewer scene with given train dataset"""
         assert self.viewer_state and self.pipeline.datamanager.train_dataset
         self.viewer_state.init_scene(
             dataset=self.pipeline.datamanager.train_dataset,
-            start_train=self.config.viewer.start_train,
+            start_train=True,
         )
-        if not self.config.viewer.start_train:
-            self._always_render(self._start_step)
 
     @check_viewer_enabled
-    def _update_viewer_state(self, step: int):
+    def _update_viewer_state(self, step: int) -> None:
         """Updates the viewer state by rendering out scene with current pipeline
         Returns the time taken to render scene.
 
         Args:
             step: current train step
         """
         assert self.viewer_state is not None
-        with TimeWriter(writer, EventName.ITER_VIS_TIME, step=step) as _:
-            num_rays_per_batch = self.config.pipeline.datamanager.train_num_rays_per_batch
-            try:
-                self.viewer_state.update_scene(self, step, self.pipeline.model, num_rays_per_batch)
-            except RuntimeError:
-                time.sleep(0.03)  # sleep to allow buffer to reset
-                assert self.viewer_state.vis is not None
-                self.viewer_state.vis["renderingState/log_errors"].write(
-                    "Error: GPU out of memory. Reduce resolution to prevent viewer from crashing."
-                )
+        num_rays_per_batch: int = self.pipeline.datamanager.get_train_rays_per_batch()
+        try:
+            self.viewer_state.update_scene(step, num_rays_per_batch)
+        except RuntimeError:
+            time.sleep(0.03)  # sleep to allow buffer to reset
+            CONSOLE.log("Viewer failed. Continuing training.")
 
     @check_viewer_enabled
-    def _update_viewer_rays_per_sec(self, train_t: TimeWriter, vis_t: TimeWriter, step: int):
-        """Performs update on rays/sec calclation for training
+    def _update_viewer_rays_per_sec(self, train_t: TimeWriter, vis_t: TimeWriter, step: int) -> None:
+        """Performs update on rays/sec calculation for training
 
         Args:
             train_t: timer object carrying time to execute total training iteration
             vis_t: timer object carrying time to execute visualization step
             step: current step
         """
-        train_num_rays_per_batch = self.config.pipeline.datamanager.train_num_rays_per_batch
+        train_num_rays_per_batch: int = self.pipeline.datamanager.get_train_rays_per_batch()
         writer.put_time(
             name=EventName.TRAIN_RAYS_PER_SEC,
             duration=train_num_rays_per_batch / (train_t.duration - vis_t.duration),
             step=step,
             avg_over_steps=True,
         )
 
     def _load_checkpoint(self) -> None:
         """Helper function to load pipeline and optimizer from prespecified checkpoint"""
-        load_dir = self.config.trainer.load_dir
+        load_dir: Path = self.config.load_dir
         if load_dir is not None:
-            load_step = self.config.trainer.load_step
+            load_step = self.config.load_step
             if load_step is None:
                 print("Loading latest checkpoint from load_dir")
                 # NOTE: this is specific to the checkpoint name format
                 load_step = sorted(int(x[x.find("-") + 1 : x.find(".")]) for x in os.listdir(load_dir))[-1]
-            load_path = load_dir / f"step-{load_step:09d}.ckpt"
+            load_path: Path = load_dir / f"step-{load_step:09d}.ckpt"
             assert load_path.exists(), f"Checkpoint {load_path} does not exist"
             loaded_state = torch.load(load_path, map_location="cpu")
             self._start_step = loaded_state["step"] + 1
             # load the checkpoints for pipeline, optimizers, and gradient scalar
-            self.pipeline.load_pipeline(loaded_state["pipeline"])
+            self.pipeline.load_pipeline(loaded_state["pipeline"], loaded_state["step"])
             self.optimizers.load_optimizers(loaded_state["optimizers"])
             self.grad_scaler.load_state_dict(loaded_state["scalers"])
             CONSOLE.print(f"done loading checkpoint from {load_path}")
         else:
             CONSOLE.print("No checkpoints to load, training from scratch")
 
     @check_main_thread
@@ -272,81 +368,95 @@
         Args:
             step: number of steps in training for given checkpoint
         """
         # possibly make the checkpoint directory
         if not self.checkpoint_dir.exists():
             self.checkpoint_dir.mkdir(parents=True, exist_ok=True)
         # save the checkpoint
-        ckpt_path = self.checkpoint_dir / f"step-{step:09d}.ckpt"
+        ckpt_path: Path = self.checkpoint_dir / f"step-{step:09d}.ckpt"
         torch.save(
             {
                 "step": step,
                 "pipeline": self.pipeline.module.state_dict()  # type: ignore
                 if hasattr(self.pipeline, "module")
                 else self.pipeline.state_dict(),
                 "optimizers": {k: v.state_dict() for (k, v) in self.optimizers.optimizers.items()},
                 "scalers": self.grad_scaler.state_dict(),
             },
             ckpt_path,
         )
         # possibly delete old checkpoints
-        if self.config.trainer.save_only_latest_checkpoint:
+        if self.config.save_only_latest_checkpoint:
             # delete everything else in the checkpoint folder
             for f in self.checkpoint_dir.glob("*"):
                 if f != ckpt_path:
                     f.unlink()
 
     @profiler.time_function
-    def train_iteration(self, step: int) -> Tuple[torch.Tensor, Dict[str, torch.Tensor], Dict[str, torch.Tensor]]:
+    def train_iteration(self, step: int) -> TRAIN_INTERATION_OUTPUT:
         """Run one iteration with a batch of inputs. Returns dictionary of model losses.
 
         Args:
             step: Current training step.
         """
+
         self.optimizers.zero_grad_all()
-        cpu_or_cuda_str = self.device.split(":")[0]
+        cpu_or_cuda_str: str = self.device.split(":")[0]
+
         with torch.autocast(device_type=cpu_or_cuda_str, enabled=self.mixed_precision):
             _, loss_dict, metrics_dict = self.pipeline.get_train_loss_dict(step=step)
             loss = functools.reduce(torch.add, loss_dict.values())
         self.grad_scaler.scale(loss).backward()  # type: ignore
         self.optimizers.optimizer_scaler_step_all(self.grad_scaler)
+
+        if self.config.log_gradients:
+            total_grad = 0
+            for tag, value in self.pipeline.model.named_parameters():
+                assert tag != "Total"
+                if value.grad is not None:
+                    grad = value.grad.norm()
+                    metrics_dict[f"Gradients/{tag}"] = grad
+                    total_grad += grad
+
+            metrics_dict["Gradients/Total"] = total_grad
+
         self.grad_scaler.update()
         self.optimizers.scheduler_step_all(step)
 
         # Merging loss and metrics dict into a single output.
         return loss, loss_dict, metrics_dict
 
     @check_eval_enabled
     @profiler.time_function
-    def eval_iteration(self, step):
+    def eval_iteration(self, step: int) -> None:
         """Run one iteration with different batch/image/all image evaluations depending on step size.
 
         Args:
             step: Current training step.
         """
         # a batch of eval rays
-        if step_check(step, self.config.trainer.steps_per_eval_batch):
+        if step_check(step, self.config.steps_per_eval_batch):
             _, eval_loss_dict, eval_metrics_dict = self.pipeline.get_eval_loss_dict(step=step)
             eval_loss = functools.reduce(torch.add, eval_loss_dict.values())
             writer.put_scalar(name="Eval Loss", scalar=eval_loss, step=step)
             writer.put_dict(name="Eval Loss Dict", scalar_dict=eval_loss_dict, step=step)
             writer.put_dict(name="Eval Metrics Dict", scalar_dict=eval_metrics_dict, step=step)
 
         # one eval image
-        if step_check(step, self.config.trainer.steps_per_eval_image):
+        if step_check(step, self.config.steps_per_eval_image):
             with TimeWriter(writer, EventName.TEST_RAYS_PER_SEC, write=False) as test_t:
                 metrics_dict, images_dict = self.pipeline.get_eval_image_metrics_and_images(step=step)
             writer.put_time(
                 name=EventName.TEST_RAYS_PER_SEC,
                 duration=metrics_dict["num_rays"] / test_t.duration,
                 step=step,
                 avg_over_steps=True,
             )
             writer.put_dict(name="Eval Images Metrics", scalar_dict=metrics_dict, step=step)
             group = "Eval Images"
             for image_name, image in images_dict.items():
                 writer.put_image(name=group + "/" + image_name, image=image, step=step)
 
         # all eval images
-        if step_check(step, self.config.trainer.steps_per_eval_all_images):
+        if step_check(step, self.config.steps_per_eval_all_images):
             metrics_dict = self.pipeline.get_average_eval_image_metrics(step=step)
             writer.put_dict(name="Eval Images Metrics Dict (all images)", scalar_dict=metrics_dict, step=step)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/__init__.py` & `nerfstudio-0.2.0/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/activations.py` & `nerfstudio-0.2.0/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/base_field_component.py` & `nerfstudio-0.2.0/nerfstudio/field_components/base_field_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class FieldComponent(nn.Module):
     """Field modules that can be combined to store and compute the fields.
 
     Args:
         in_dim: Input dimension to module.
-        out_dim: Ouput dimension to module.
+        out_dim: Output dimension to module.
     """
 
     def __init__(self, in_dim: Optional[int] = None, out_dim: Optional[int] = None) -> None:
         super().__init__()
         self.in_dim = in_dim
         self.out_dim = out_dim
```

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/embedding.py` & `nerfstudio-0.2.0/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/encodings.py` & `nerfstudio-0.2.0/nerfstudio/field_components/encodings.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Encoding functions
 """
 
+import itertools
 from abc import abstractmethod
-from typing import Optional
+from typing import Optional, Sequence
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torch import nn
 from torchtyping import TensorType
 from typing_extensions import Literal
@@ -69,15 +70,15 @@
         return self.in_dim
 
     def forward(self, in_tensor: TensorType["bs":..., "input_dim"]) -> TensorType["bs":..., "output_dim"]:
         return in_tensor
 
 
 class ScalingAndOffset(Encoding):
-    """Simple scaling and offet to input
+    """Simple scaling and offset to input
 
     Args:
         in_dim: Input dimension of tensor
         scaling: Scaling applied to tensor.
         offset: Offset applied to tensor.
     """
 
@@ -93,15 +94,15 @@
         return self.in_dim
 
     def forward(self, in_tensor: TensorType["bs":..., "input_dim"]) -> TensorType["bs":..., "output_dim"]:
         return self.scaling * in_tensor + self.offset
 
 
 class NeRFEncoding(Encoding):
-    """Multi-scale sinousoidal encodings. Support ``integrated positional encodings`` if covariances are provided.
+    """Multi-scale sinusoidal encodings. Support ``integrated positional encodings`` if covariances are provided.
     Each axis is encoded with frequencies ranging from 2^min_freq_exp to 2^max_freq_exp.
 
     Args:
         in_dim: Input dimension of tensor
         num_frequencies: Number of encoded frequencies per axis
         min_freq_exp: Minimum frequency exponent
         max_freq_exp: Maximum frequency exponent
@@ -224,27 +225,28 @@
         num_levels: Number of feature grids.
         min_res: Resolution of smallest feature grid.
         max_res: Resolution of largest feature grid.
         log2_hashmap_size: Size of hash map is 2^log2_hashmap_size.
         features_per_level: Number of features per level.
         hash_init_scale: Value to initialize hash grid.
         implementation: Implementation of hash encoding. Fallback to torch if tcnn not available.
+        interpolation: Interpolation override for tcnn hashgrid. Not supported for torch unless linear.
     """
 
     def __init__(
         self,
         num_levels: int = 16,
         min_res: int = 16,
         max_res: int = 1024,
         log2_hashmap_size: int = 19,
         features_per_level: int = 2,
         hash_init_scale: float = 0.001,
         implementation: Literal["tcnn", "torch"] = "tcnn",
+        interpolation: Optional[Literal["Nearest", "Linear", "Smoothstep"]] = None,
     ) -> None:
-
         super().__init__(in_dim=3)
         self.num_levels = num_levels
         self.features_per_level = features_per_level
         self.log2_hashmap_size = log2_hashmap_size
         self.hash_table_size = 2**log2_hashmap_size
 
         levels = torch.arange(num_levels)
@@ -256,26 +258,35 @@
         self.hash_table *= hash_init_scale
         self.hash_table = nn.Parameter(self.hash_table)
 
         self.tcnn_encoding = None
         if not TCNN_EXISTS and implementation == "tcnn":
             print_tcnn_speed_warning("HashEncoding")
         elif implementation == "tcnn":
+            encoding_config = {
+                "otype": "HashGrid",
+                "n_levels": self.num_levels,
+                "n_features_per_level": self.features_per_level,
+                "log2_hashmap_size": self.log2_hashmap_size,
+                "base_resolution": min_res,
+                "per_level_scale": growth_factor,
+            }
+            if interpolation is not None:
+                encoding_config["interpolation"] = interpolation
+
             self.tcnn_encoding = tcnn.Encoding(
                 n_input_dims=3,
-                encoding_config={
-                    "otype": "HashGrid",
-                    "n_levels": self.num_levels,
-                    "n_features_per_level": self.features_per_level,
-                    "log2_hashmap_size": self.log2_hashmap_size,
-                    "base_resolution": min_res,
-                    "per_level_scale": growth_factor,
-                },
+                encoding_config=encoding_config,
             )
 
+        if not TCNN_EXISTS or self.tcnn_encoding is None:
+            assert (
+                interpolation is None or interpolation == "Linear"
+            ), f"interpolation '{interpolation}' is not supported for torch encoding backend"
+
     def get_out_dim(self) -> int:
         return self.num_levels * self.features_per_level
 
     def hash_fn(self, in_tensor: TensorType["bs":..., "num_levels", 3]) -> TensorType["bs":..., "num_levels"]:
         """Returns hash tensor using method described in Instant-NGP
 
         Args:
@@ -419,14 +430,21 @@
         self.plane_coef = nn.Parameter(init_scale * torch.randn((3, num_components, resolution, resolution)))
         self.line_coef = nn.Parameter(init_scale * torch.randn((3, num_components, resolution, 1)))
 
     def get_out_dim(self) -> int:
         return self.num_components * 3
 
     def forward(self, in_tensor: TensorType["bs":..., "input_dim"]) -> TensorType["bs":..., "output_dim"]:
+        """Compute encoding for each position in in_positions
+
+        Args:
+            in_tensor: position inside bounds in range [-1,1],
+
+        Returns: Encoded position
+        """
         plane_coord = torch.stack([in_tensor[..., [0, 1]], in_tensor[..., [0, 2]], in_tensor[..., [1, 2]]])  # [3,...,2]
         line_coord = torch.stack([in_tensor[..., 2], in_tensor[..., 1], in_tensor[..., 0]])  # [3, ...]
         line_coord = torch.stack([torch.zeros_like(line_coord), line_coord], dim=-1)  # [3, ...., 2]
 
         # Stop gradients from going to sampler
         plane_coord = plane_coord.view(3, -1, 1, 2).detach()
         line_coord = line_coord.view(3, -1, 1, 2).detach()
@@ -437,41 +455,205 @@
         features = plane_features * line_features  # [3, Components, -1, 1]
         features = torch.moveaxis(features.view(3 * self.num_components, *in_tensor.shape[:-1]), 0, -1)
 
         return features  # [..., 3 * Components]
 
     @torch.no_grad()
     def upsample_grid(self, resolution: int) -> None:
-        """Upsamples underyling feature grid
+        """Upsamples underlying feature grid
 
         Args:
             resolution: Target resolution.
         """
         plane_coef = F.interpolate(
             self.plane_coef.data, size=(resolution, resolution), mode="bilinear", align_corners=True
         )
         line_coef = F.interpolate(self.line_coef.data, size=(resolution, 1), mode="bilinear", align_corners=True)
 
-        # TODO(ethan): are these torch.nn.Parameters needed?
         self.plane_coef, self.line_coef = torch.nn.Parameter(plane_coef), torch.nn.Parameter(line_coef)
         self.resolution = resolution
 
 
+class TriplaneEncoding(Encoding):
+    """Learned triplane encoding
+
+    The encoding at [i,j,k] is an n dimensional vector corresponding to the element-wise product of the
+    three n dimensional vectors at plane_coeff[i,j], plane_coeff[i,k], and plane_coeff[j,k].
+
+    This allows for marginally more expressivity than the TensorVMEncoding, and each component is self standing
+    and symmetrical, unlike with VM decomposition where we needed one component with a vector along all the x, y, z
+    directions for symmetry.
+
+    This can be thought of as 3 planes of features perpendicular to the x, y, and z axes, respectively and intersecting
+    at the origin, and the encoding being the element-wise product of the element at the projection of [i, j, k] on
+    these planes.
+
+    The use for this is in representing a tensor decomp of a 4D embedding tensor: (x, y, z, feature_size)
+
+    This will return a tensor of shape (bs:..., num_components)
+
+    Args:
+        resolution: Resolution of grid.
+        num_components: The number of scalar triplanes to use (ie: output feature size)
+        init_scale: The scale of the initial values of the planes
+        product: Whether to use the element-wise product of the planes or the sum
+    """
+
+    plane_coef: TensorType[3, "num_components", "resolution", "resolution"]
+
+    def __init__(
+        self,
+        resolution: int = 32,
+        num_components: int = 64,
+        init_scale: float = 0.1,
+        reduce: Literal["sum", "product"] = "sum",
+    ) -> None:
+        super().__init__(in_dim=3)
+
+        self.resolution = resolution
+        self.num_components = num_components
+        self.init_scale = init_scale
+        self.reduce = reduce
+
+        self.plane_coef = nn.Parameter(
+            self.init_scale * torch.randn((3, self.num_components, self.resolution, self.resolution))
+        )
+
+    def get_out_dim(self) -> int:
+        return self.num_components
+
+    def forward(self, in_tensor: TensorType["bs":..., 3]) -> TensorType["bs":..., "num_components", "featuresize"]:
+        """Sample features from this encoder. Expects in_tensor to be in range [0, resolution]"""
+
+        original_shape = in_tensor.shape
+        in_tensor = in_tensor.reshape(-1, 3)
+
+        plane_coord = torch.stack([in_tensor[..., [0, 1]], in_tensor[..., [0, 2]], in_tensor[..., [1, 2]]], dim=0)
+
+        # Stop gradients from going to sampler
+        plane_coord = plane_coord.detach().view(3, -1, 1, 2)
+        plane_features = F.grid_sample(
+            self.plane_coef, plane_coord, align_corners=True
+        )  # [3, num_components, flattened_bs, 1]
+
+        if self.reduce == "product":
+            plane_features = plane_features.prod(0).squeeze(-1).T  # [flattened_bs, num_components]
+        else:
+            plane_features = plane_features.sum(0).squeeze(-1).T
+
+        return plane_features.reshape(*original_shape[:-1], self.num_components)
+
+    @torch.no_grad()
+    def upsample_grid(self, resolution: int) -> None:
+        """Upsamples underlying feature grid
+
+        Args:
+            resolution: Target resolution.
+        """
+        plane_coef = F.interpolate(
+            self.plane_coef.data, size=(resolution, resolution), mode="bilinear", align_corners=True
+        )
+
+        self.plane_coef = torch.nn.Parameter(plane_coef)
+        self.resolution = resolution
+
+
+class KPlanesEncoding(Encoding):
+    """Learned K-Planes encoding
+
+    A plane encoding supporting both 3D and 4D coordinates. With 3D coordinates this is similar to
+    :class:`TriplaneEncoding`. With 4D coordinates, the encoding at point ``[i,j,k,q]`` is
+    a n-dimensional vector computed as the elementwise product of 6 n-dimensional vectors at
+    ``planes[i,j]``, ``planes[i,k]``, ``planes[i,q]``, ``planes[j,k]``, ``planes[j,q]``,
+    ``planes[k,q]``.
+
+    Unlike :class:`TriplaneEncoding` this class supports different resolution along each axis.
+
+    This will return a tensor of shape (bs:..., num_components)
+
+    Args:
+        resolution: Resolution of the grid. Can be a sequence of 3 or 4 integers.
+        num_components: The number of scalar planes to use (ie: output feature size)
+        init_a: The lower-bound of the uniform distribution used to initialize the spatial planes
+        init_b: The upper-bound of the uniform distribution used to initialize the spatial planes
+        reduce: Whether to use the element-wise product of the planes or the sum
+    """
+
+    def __init__(
+        self,
+        resolution: Sequence[int] = (128, 128, 128),
+        num_components: int = 64,
+        init_a: float = 0.1,
+        init_b: float = 0.5,
+        reduce: Literal["sum", "product"] = "product",
+    ) -> None:
+        super().__init__(in_dim=len(resolution))
+
+        self.resolution = resolution
+        self.num_components = num_components
+        self.reduce = reduce
+        if self.in_dim not in {3, 4}:
+            raise ValueError(
+                f"The dimension of coordinates must be either 3 (static scenes) "
+                f"or 4 (dynamic scenes). Found resolution with {self.in_dim} dimensions."
+            )
+        has_time_planes = self.in_dim == 4
+
+        self.coo_combs = list(itertools.combinations(range(self.in_dim), 2))
+        # Unlike the Triplane encoding, we use a parameter list instead of batching all planes
+        # together to support uneven resolutions (especially useful for time).
+        # Dynamic models (in_dim == 4) will have 6 planes:
+        # (y, x), (z, x), (t, x), (z, y), (t, y), (t, z)
+        # static models (in_dim == 3) will only have the 1st, 2nd and 4th planes.
+        self.plane_coefs = nn.ParameterList()
+        for coo_comb in self.coo_combs:
+            new_plane_coef = nn.Parameter(
+                torch.empty([self.num_components] + [self.resolution[cc] for cc in coo_comb[::-1]])
+            )
+            if has_time_planes and 3 in coo_comb:  # Time planes initialized to 1
+                nn.init.ones_(new_plane_coef)
+            else:
+                nn.init.uniform_(new_plane_coef, a=init_a, b=init_b)
+            self.plane_coefs.append(new_plane_coef)
+
+    def get_out_dim(self) -> int:
+        return self.num_components
+
+    def forward(self, in_tensor: TensorType["bs":..., "input_dim"]) -> TensorType["bs":..., "output_dim"]:
+        """Sample features from this encoder. Expects ``in_tensor`` to be in range [-1, 1]"""
+        original_shape = in_tensor.shape
+
+        output = 1.0 if self.reduce == "product" else 0.0  # identity for corresponding op
+        for ci, coo_comb in enumerate(self.coo_combs):
+            grid = self.plane_coefs[ci].unsqueeze(0)  # [1, feature_dim, reso1, reso2]
+            coords = in_tensor[..., coo_comb].view(1, 1, -1, 2)  # [1, 1, flattened_bs, 2]
+            interp = F.grid_sample(
+                grid, coords, align_corners=True, padding_mode="border"
+            )  # [1, output_dim, 1, flattened_bs]
+            interp = interp.view(self.num_components, -1).T  # [flattened_bs, output_dim]
+            if self.reduce == "product":
+                output = output * interp
+            else:
+                output = output + interp
+
+        return output.reshape(*original_shape[:-1], self.num_components)
+
+
 class SHEncoding(Encoding):
     """Spherical harmonic encoding
 
     Args:
-        levels: Number of spherical hamonic levels to encode.
+        levels: Number of spherical harmonic levels to encode.
     """
 
     def __init__(self, levels: int = 4) -> None:
         super().__init__(in_dim=3)
 
         if levels <= 0 or levels > 4:
-            raise ValueError(f"Spherical harmonic encoding only suports 1 to 4 levels, requested {levels}")
+            raise ValueError(f"Spherical harmonic encoding only supports 1 to 4 levels, requested {levels}")
 
         self.levels = levels
 
     def get_out_dim(self) -> int:
         return self.levels**2
 
     @torch.no_grad()
```

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/field_heads.py` & `nerfstudio-0.2.0/nerfstudio/field_components/field_heads.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,36 @@
 
 """
 Collection of render heads
 """
 from enum import Enum
 from typing import Callable, Optional, Union
 
+import torch
 from torch import nn
 from torchtyping import TensorType
 
 from nerfstudio.field_components.base_field_component import FieldComponent
 
 
 class FieldHeadNames(Enum):
     """Possible field outputs"""
 
     RGB = "rgb"
     SH = "sh"
     DENSITY = "density"
+    NORMALS = "normals"
+    PRED_NORMALS = "pred_normals"
     UNCERTAINTY = "uncertainty"
     TRANSIENT_RGB = "transient_rgb"
     TRANSIENT_DENSITY = "transient_density"
     SEMANTICS = "semantics"
-    SEMANTICS_STUFF = "semantics_stuff"
-    SEMANTICS_THING = "semantics_thing"
+    SDF = "sdf"
+    ALPHA = "alpha"
+    GRADIENT = "gradient"
 
 
 class FieldHead(FieldComponent):
     """Base field output
 
     Args:
         out_dim: output dimension for renderer
@@ -79,15 +83,15 @@
         Args:
             in_tensor: Network input
 
         Returns:
             Render head output
         """
         if not self.net:
-            raise SystemError("in_dim not set. Must be provided to construtor, or set_in_dim() should be called.")
+            raise SystemError("in_dim not set. Must be provided to constructor, or set_in_dim() should be called.")
         out_tensor = self.net(in_tensor)
         if self.activation:
             out_tensor = self.activation(out_tensor)
         return out_tensor
 
 
 class DensityFieldHead(FieldHead):
@@ -167,17 +171,35 @@
     def __init__(self, in_dim: Optional[int] = None, activation: Optional[nn.Module] = nn.Softplus()) -> None:
         super().__init__(
             in_dim=in_dim, out_dim=1, field_head_name=FieldHeadNames.TRANSIENT_DENSITY, activation=activation
         )
 
 
 class SemanticFieldHead(FieldHead):
-    """Semantic stuff output
+    """Semantic output
 
     Args:
         num_classes: Number of semantic classes
         in_dim: input dimension. If not defined in constructor, it must be set later.
         activation: output head activation
     """
 
     def __init__(self, num_classes: int, in_dim: Optional[int] = None) -> None:
         super().__init__(in_dim=in_dim, out_dim=num_classes, field_head_name=FieldHeadNames.SEMANTICS, activation=None)
+
+
+class PredNormalsFieldHead(FieldHead):
+    """Predicted normals output.
+
+    Args:
+        in_dim: input dimension. If not defined in constructor, it must be set later.
+        activation: output head activation
+    """
+
+    def __init__(self, in_dim: Optional[int] = None, activation: Optional[nn.Module] = nn.Tanh()) -> None:
+        super().__init__(in_dim=in_dim, out_dim=3, field_head_name=FieldHeadNames.PRED_NORMALS, activation=activation)
+
+    def forward(self, in_tensor: TensorType["bs":..., "in_dim"]) -> TensorType["bs":..., "out_dim"]:
+        """Needed to normalize the output into valid normals."""
+        out_tensor = super().forward(in_tensor)
+        out_tensor = torch.nn.functional.normalize(out_tensor, dim=-1)
+        return out_tensor
```

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/mlp.py` & `nerfstudio-0.2.0/nerfstudio/field_components/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class MLP(FieldComponent):
     """Multilayer perceptron
 
     Args:
         in_dim: Input layer dimension
         num_layers: Number of network layers
         layer_width: Width of each MLP layer
-        out_dim: Ouput layer dimension. Uses layer_width if None.
+        out_dim: Output layer dimension. Uses layer_width if None.
         activation: intermediate layer activation function.
         out_activation: output activation function.
     """
 
     def __init__(
         self,
         in_dim: int,
```

### Comparing `nerfstudio-0.1.9/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-0.2.0/nerfstudio/field_components/spatial_distortions.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,20 +61,16 @@
 
     def __init__(self, order: Optional[Union[float, int]] = None) -> None:
         super().__init__()
         self.order = order
 
     def forward(self, positions):
         def contract(x):
-            mag = torch.linalg.norm(x, ord=self.order, dim=-1)
-            mask = mag >= 1
-            x_new = x.clone()
-            x_new[mask] = (2 - (1 / mag[mask][..., None])) * (x[mask] / mag[mask][..., None])
-
-            return x_new
+            mag = torch.linalg.norm(x, ord=self.order, dim=-1)[..., None]
+            return torch.where(mag < 1, x, (2 - (1 / mag)) * (x / mag))
 
         if isinstance(positions, Gaussians):
             means = contract(positions.mean.clone())
 
             contract = lambda x: (2 - (1 / torch.linalg.norm(x, ord=self.order, dim=-1, keepdim=True))) * (
                 x / torch.linalg.norm(x, ord=self.order, dim=-1, keepdim=True)
             )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/__init__.py` & `nerfstudio-0.2.0/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/density_fields.py` & `nerfstudio-0.2.0/nerfstudio/fields/density_fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 # limitations under the License.
 
 """
 Proposal network field.
 """
 
 
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 import torch
-from torch.nn.parameter import Parameter
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.spatial_distortions import SpatialDistortion
 from nerfstudio.fields.base_field import Field
@@ -46,31 +45,35 @@
         hidden_dim: dimension of hidden layers
         spatial_distortion: spatial distortion module
         use_linear: whether to skip the MLP and use a single linear layer instead
     """
 
     def __init__(
         self,
-        aabb,
+        aabb: TensorType,
         num_layers: int = 2,
         hidden_dim: int = 64,
         spatial_distortion: Optional[SpatialDistortion] = None,
-        use_linear=False,
-        num_levels=8,
-        max_res=1024,
-        base_res=16,
-        log2_hashmap_size=18,
-        features_per_level=2,
+        use_linear: bool = False,
+        num_levels: int = 8,
+        max_res: int = 1024,
+        base_res: int = 16,
+        log2_hashmap_size: int = 18,
+        features_per_level: int = 2,
     ) -> None:
         super().__init__()
-        self.aabb = Parameter(aabb, requires_grad=False)
+        self.register_buffer("aabb", aabb)
         self.spatial_distortion = spatial_distortion
         self.use_linear = use_linear
         growth_factor = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
 
+        self.register_buffer("max_res", torch.tensor(max_res))
+        self.register_buffer("num_levels", torch.tensor(num_levels))
+        self.register_buffer("log2_hashmap_size", torch.tensor(log2_hashmap_size))
+
         config = {
             "encoding": {
                 "otype": "HashGrid",
                 "n_levels": num_levels,
                 "n_features_per_level": features_per_level,
                 "log2_hashmap_size": log2_hashmap_size,
                 "base_resolution": base_res,
@@ -92,30 +95,34 @@
                 encoding_config=config["encoding"],
                 network_config=config["network"],
             )
         else:
             self.encoding = tcnn.Encoding(n_input_dims=3, encoding_config=config["encoding"])
             self.linear = torch.nn.Linear(self.encoding.n_output_dims, 1)
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, None]:
         if self.spatial_distortion is not None:
             positions = self.spatial_distortion(ray_samples.frustums.get_positions())
             positions = (positions + 2.0) / 4.0
         else:
             positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        # Make sure the tcnn gets inputs between 0 and 1.
+        selector = ((positions > 0.0) & (positions < 1.0)).all(dim=-1)
+        positions = positions * selector[..., None]
         positions_flat = positions.view(-1, 3)
         if not self.use_linear:
             density_before_activation = (
                 self.mlp_base(positions_flat).view(*ray_samples.frustums.shape, -1).to(positions)
             )
         else:
             x = self.encoding(positions_flat).to(positions)
             density_before_activation = self.linear(x).view(*ray_samples.frustums.shape, -1)
 
         # Rectifying the density with an exponential is much more stable than a ReLU or
         # softplus, because it enables high post-activation (float32) density outputs
         # from smaller internal (float16) parameters.
         density = trunc_exp(density_before_activation)
+        density = density * selector[..., None]
         return density, None
 
-    def get_outputs(self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None):
+    def get_outputs(self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None) -> dict:
         return {}
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/instant_ngp_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/instant_ngp_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,105 +13,104 @@
 # limitations under the License.
 
 """
 Instant-NGP field implementations using tiny-cuda-nn, torch, ....
 """
 
 
-from typing import Optional
+from typing import Dict, Optional, Tuple
 
+import numpy as np
 import torch
 from nerfacc import ContractionType, contract
 from torch.nn.parameter import Parameter
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import RaySamples
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.embedding import Embedding
 from nerfstudio.field_components.field_heads import FieldHeadNames
-from nerfstudio.fields.base_field import Field
+from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
 
 try:
     import tinycudann as tcnn
 except ImportError:
     # tinycudann module doesn't exist
     pass
 
 
-def get_normalized_directions(directions: TensorType["bs":..., 3]):
-    """SH encoding must be in the range [0, 1]
-
-    Args:
-        directions: batch of directions
-    """
-    return (directions + 1.0) / 2.0
-
-
 class TCNNInstantNGPField(Field):
     """TCNN implementation of the Instant-NGP field.
 
     Args:
         aabb: parameters of scene aabb bounds
         num_layers: number of hidden layers
         hidden_dim: dimension of hidden layers
         geo_feat_dim: output geo feat dimensions
         num_layers_color: number of hidden layers for color network
         hidden_dim_color: dimension of hidden layers for color network
         use_appearance_embedding: whether to use appearance embedding
-        num_images: number of images, requried if use_appearance_embedding is True
+        num_images: number of images, required if use_appearance_embedding is True
         appearance_embedding_dim: dimension of appearance embedding
         contraction_type: type of contraction
+        num_levels: number of levels of the hashmap for the base mlp
+        log2_hashmap_size: size of the hashmap for the base mlp
+        max_res: maximum resolution of the hashmap for the base mlp
     """
 
     def __init__(
         self,
-        aabb,
+        aabb: TensorType,
         num_layers: int = 2,
         hidden_dim: int = 64,
         geo_feat_dim: int = 15,
         num_layers_color: int = 3,
         hidden_dim_color: int = 64,
-        use_appearance_embedding: bool = False,
+        use_appearance_embedding: Optional[bool] = False,
         num_images: Optional[int] = None,
         appearance_embedding_dim: int = 32,
         contraction_type: ContractionType = ContractionType.UN_BOUNDED_SPHERE,
+        num_levels: int = 16,
+        log2_hashmap_size: int = 19,
+        max_res: int = 2048,
     ) -> None:
         super().__init__()
 
         self.aabb = Parameter(aabb, requires_grad=False)
         self.geo_feat_dim = geo_feat_dim
         self.contraction_type = contraction_type
 
         self.use_appearance_embedding = use_appearance_embedding
         if use_appearance_embedding:
             assert num_images is not None
             self.appearance_embedding_dim = appearance_embedding_dim
             self.appearance_embedding = Embedding(num_images, appearance_embedding_dim)
 
         # TODO: set this properly based on the aabb
-        per_level_scale = 1.4472692012786865
+        base_res: int = 16
+        per_level_scale = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
 
         self.direction_encoding = tcnn.Encoding(
             n_input_dims=3,
             encoding_config={
                 "otype": "SphericalHarmonics",
                 "degree": 4,
             },
         )
 
         self.mlp_base = tcnn.NetworkWithInputEncoding(
             n_input_dims=3,
             n_output_dims=1 + self.geo_feat_dim,
             encoding_config={
                 "otype": "HashGrid",
-                "n_levels": 16,
+                "n_levels": num_levels,
                 "n_features_per_level": 2,
-                "log2_hashmap_size": 19,
-                "base_resolution": 16,
+                "log2_hashmap_size": log2_hashmap_size,
+                "base_resolution": base_res,
                 "per_level_scale": per_level_scale,
             },
             network_config={
                 "otype": "FullyFusedMLP",
                 "activation": "ReLU",
                 "output_activation": "None",
                 "n_neurons": hidden_dim,
@@ -130,30 +129,32 @@
                 "activation": "ReLU",
                 "output_activation": "Sigmoid",
                 "n_neurons": hidden_dim_color,
                 "n_hidden_layers": num_layers_color - 1,
             },
         )
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         positions = ray_samples.frustums.get_positions()
         positions_flat = positions.view(-1, 3)
         positions_flat = contract(x=positions_flat, roi=self.aabb, type=self.contraction_type)
 
         h = self.mlp_base(positions_flat).view(*ray_samples.frustums.shape, -1)
         density_before_activation, base_mlp_out = torch.split(h, [1, self.geo_feat_dim], dim=-1)
 
         # Rectifying the density with an exponential is much more stable than a ReLU or
         # softplus, because it enables high post-activation (float32) density outputs
         # from smaller internal (float16) parameters.
         density = trunc_exp(density_before_activation.to(positions))
         return density, base_mlp_out
 
-    def get_outputs(self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None):
-        directions = get_normalized_directions(ray_samples.frustums.directions)
+    def get_outputs(
+        self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
+    ) -> Dict[FieldHeadNames, TensorType]:
+        directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
         directions_flat = directions.view(-1, 3)
 
         d = self.direction_encoding(directions_flat)
         if density_embedding is None:
             positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
             h = torch.cat([d, positions.view(-1, 3)], dim=-1)
         else:
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/nerfacto_field.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,106 +30,121 @@
 from nerfstudio.field_components.activations import trunc_exp
 from nerfstudio.field_components.embedding import Embedding
 from nerfstudio.field_components.encodings import Encoding, HashEncoding, SHEncoding
 from nerfstudio.field_components.field_heads import (
     DensityFieldHead,
     FieldHead,
     FieldHeadNames,
+    PredNormalsFieldHead,
     RGBFieldHead,
     SemanticFieldHead,
     TransientDensityFieldHead,
     TransientRGBFieldHead,
     UncertaintyFieldHead,
 )
 from nerfstudio.field_components.mlp import MLP
 from nerfstudio.field_components.spatial_distortions import (
     SceneContraction,
     SpatialDistortion,
 )
-from nerfstudio.fields.base_field import Field
+from nerfstudio.fields.base_field import Field, shift_directions_for_tcnn
 
 try:
     import tinycudann as tcnn
 except ImportError:
     # tinycudann module doesn't exist
     pass
 
 
-def get_normalized_directions(directions: TensorType["bs":..., 3]):
-    """SH encoding must be in the range [0, 1]
-
-    Args:
-        directions: batch of directions
-    """
-    return (directions + 1.0) / 2.0
-
-
 class TCNNNerfactoField(Field):
     """Compound Field that uses TCNN
 
     Args:
         aabb: parameters of scene aabb bounds
+        num_images: number of images in the dataset
         num_layers: number of hidden layers
         hidden_dim: dimension of hidden layers
         geo_feat_dim: output geo feat dimensions
+        num_levels: number of levels of the hashmap for the base mlp
+        max_res: maximum resolution of the hashmap for the base mlp
+        log2_hashmap_size: size of the hashmap for the base mlp
         num_layers_color: number of hidden layers for color network
+        num_layers_transient: number of hidden layers for transient network
         hidden_dim_color: dimension of hidden layers for color network
+        hidden_dim_transient: dimension of hidden layers for transient network
         appearance_embedding_dim: dimension of appearance embedding
         transient_embedding_dim: dimension of transient embedding
+        use_transient_embedding: whether to use transient embedding
+        use_semantics: whether to use semantic segmentation
+        num_semantic_classes: number of semantic classes
+        use_pred_normals: whether to use predicted normals
         use_average_appearance_embedding: whether to use average appearance embedding or zeros for inference
         spatial_distortion: spatial distortion to apply to the scene
     """
 
     def __init__(
         self,
-        aabb,
+        aabb: TensorType,
         num_images: int,
         num_layers: int = 2,
         hidden_dim: int = 64,
         geo_feat_dim: int = 15,
+        num_levels: int = 16,
+        max_res: int = 2048,
+        log2_hashmap_size: int = 19,
         num_layers_color: int = 3,
         num_layers_transient: int = 2,
         hidden_dim_color: int = 64,
         hidden_dim_transient: int = 64,
         appearance_embedding_dim: int = 32,
         transient_embedding_dim: int = 16,
         use_transient_embedding: bool = False,
         use_semantics: bool = False,
         num_semantic_classes: int = 100,
+        pass_semantic_gradients: bool = False,
+        use_pred_normals: bool = False,
         use_average_appearance_embedding: bool = False,
-        spatial_distortion: Optional[SpatialDistortion] = None,
+        spatial_distortion: SpatialDistortion = None,
     ) -> None:
         super().__init__()
 
-        self.aabb = Parameter(aabb, requires_grad=False)
+        self.register_buffer("aabb", aabb)
         self.geo_feat_dim = geo_feat_dim
 
+        self.register_buffer("max_res", torch.tensor(max_res))
+        self.register_buffer("num_levels", torch.tensor(num_levels))
+        self.register_buffer("log2_hashmap_size", torch.tensor(log2_hashmap_size))
+
         self.spatial_distortion = spatial_distortion
         self.num_images = num_images
         self.appearance_embedding_dim = appearance_embedding_dim
         self.embedding_appearance = Embedding(self.num_images, self.appearance_embedding_dim)
         self.use_average_appearance_embedding = use_average_appearance_embedding
         self.use_transient_embedding = use_transient_embedding
         self.use_semantics = use_semantics
+        self.use_pred_normals = use_pred_normals
+        self.pass_semantic_gradients = pass_semantic_gradients
 
-        num_levels = 16
-        max_res = 1024
-        base_res = 16
-        log2_hashmap_size = 19
-        features_per_level = 2
+        base_res: int = 16
+        features_per_level: int = 2
         growth_factor = np.exp((np.log(max_res) - np.log(base_res)) / (num_levels - 1))
 
         self.direction_encoding = tcnn.Encoding(
             n_input_dims=3,
             encoding_config={
                 "otype": "SphericalHarmonics",
                 "degree": 4,
             },
         )
 
+        self.position_encoding = tcnn.Encoding(
+            n_input_dims=3,
+            encoding_config={"otype": "Frequency", "n_frequencies": 2},
+        )
+
         self.mlp_base = tcnn.NetworkWithInputEncoding(
             n_input_dims=3,
             n_output_dims=1 + self.geo_feat_dim,
             encoding_config={
                 "otype": "HashGrid",
                 "n_levels": num_levels,
                 "n_features_per_level": features_per_level,
@@ -178,54 +193,81 @@
                     "n_hidden_layers": 1,
                 },
             )
             self.field_head_semantics = SemanticFieldHead(
                 in_dim=self.mlp_semantics.n_output_dims, num_classes=num_semantic_classes
             )
 
+        # predicted normals
+        if self.use_pred_normals:
+            self.mlp_pred_normals = tcnn.Network(
+                n_input_dims=self.geo_feat_dim + self.position_encoding.n_output_dims,
+                n_output_dims=hidden_dim_transient,
+                network_config={
+                    "otype": "FullyFusedMLP",
+                    "activation": "ReLU",
+                    "output_activation": "None",
+                    "n_neurons": 64,
+                    "n_hidden_layers": 2,
+                },
+            )
+            self.field_head_pred_normals = PredNormalsFieldHead(in_dim=self.mlp_pred_normals.n_output_dims)
+
         self.mlp_head = tcnn.Network(
             n_input_dims=self.direction_encoding.n_output_dims + self.geo_feat_dim + self.appearance_embedding_dim,
             n_output_dims=3,
             network_config={
                 "otype": "FullyFusedMLP",
                 "activation": "ReLU",
                 "output_activation": "Sigmoid",
                 "n_neurons": hidden_dim_color,
                 "n_hidden_layers": num_layers_color - 1,
             },
         )
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         """Computes and returns the densities."""
         if self.spatial_distortion is not None:
             positions = ray_samples.frustums.get_positions()
             positions = self.spatial_distortion(positions)
             positions = (positions + 2.0) / 4.0
         else:
             positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        # Make sure the tcnn gets inputs between 0 and 1.
+        selector = ((positions > 0.0) & (positions < 1.0)).all(dim=-1)
+        positions = positions * selector[..., None]
+        self._sample_locations = positions
+        if not self._sample_locations.requires_grad:
+            self._sample_locations.requires_grad = True
         positions_flat = positions.view(-1, 3)
         h = self.mlp_base(positions_flat).view(*ray_samples.frustums.shape, -1)
         density_before_activation, base_mlp_out = torch.split(h, [1, self.geo_feat_dim], dim=-1)
+        self._density_before_activation = density_before_activation
 
         # Rectifying the density with an exponential is much more stable than a ReLU or
         # softplus, because it enables high post-activation (float32) density outputs
         # from smaller internal (float16) parameters.
         density = trunc_exp(density_before_activation.to(positions))
+        density = density * selector[..., None]
         return density, base_mlp_out
 
-    def get_outputs(self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None):
+    def get_outputs(
+        self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
+    ) -> Dict[FieldHeadNames, TensorType]:
         assert density_embedding is not None
         outputs = {}
         if ray_samples.camera_indices is None:
             raise AttributeError("Camera indices are not provided.")
         camera_indices = ray_samples.camera_indices.squeeze()
-        directions = get_normalized_directions(ray_samples.frustums.directions)
+        directions = shift_directions_for_tcnn(ray_samples.frustums.directions)
         directions_flat = directions.view(-1, 3)
         d = self.direction_encoding(directions_flat)
 
+        outputs_shape = ray_samples.frustums.directions.shape[:-1]
+
         # appearance
         if self.training:
             embedded_appearance = self.embedding_appearance(camera_indices)
         else:
             if self.use_average_appearance_embedding:
                 embedded_appearance = torch.ones(
                     (*directions.shape[:-1], self.appearance_embedding_dim), device=directions.device
@@ -241,54 +283,60 @@
             transient_input = torch.cat(
                 [
                     density_embedding.view(-1, self.geo_feat_dim),
                     embedded_transient.view(-1, self.transient_embedding_dim),
                 ],
                 dim=-1,
             )
-            x = self.mlp_transient(transient_input).view(*ray_samples.frustums.directions.shape[:-1], -1).to(directions)
+            x = self.mlp_transient(transient_input).view(*outputs_shape, -1).to(directions)
             outputs[FieldHeadNames.UNCERTAINTY] = self.field_head_transient_uncertainty(x)
             outputs[FieldHeadNames.TRANSIENT_RGB] = self.field_head_transient_rgb(x)
             outputs[FieldHeadNames.TRANSIENT_DENSITY] = self.field_head_transient_density(x)
 
         # semantics
         if self.use_semantics:
-            density_embedding_copy = density_embedding.clone().detach()
-            semantics_input = torch.cat(
-                [
-                    density_embedding_copy.view(-1, self.geo_feat_dim),
-                ],
-                dim=-1,
-            )
-            # print(semantics_input)
-            x = self.mlp_semantics(semantics_input).view(*ray_samples.frustums.directions.shape[:-1], -1).to(directions)
+            semantics_input = density_embedding.view(-1, self.geo_feat_dim)
+            if not self.pass_semantic_gradients:
+                semantics_input = semantics_input.detach()
+
+            x = self.mlp_semantics(semantics_input).view(*outputs_shape, -1).to(directions)
             outputs[FieldHeadNames.SEMANTICS] = self.field_head_semantics(x)
 
+        # predicted normals
+        if self.use_pred_normals:
+            positions = ray_samples.frustums.get_positions()
+
+            positions_flat = self.position_encoding(positions.view(-1, 3))
+            pred_normals_inp = torch.cat([positions_flat, density_embedding.view(-1, self.geo_feat_dim)], dim=-1)
+
+            x = self.mlp_pred_normals(pred_normals_inp).view(*outputs_shape, -1).to(directions)
+            outputs[FieldHeadNames.PRED_NORMALS] = self.field_head_pred_normals(x)
+
         h = torch.cat(
             [
                 d,
                 density_embedding.view(-1, self.geo_feat_dim),
                 embedded_appearance.view(-1, self.appearance_embedding_dim),
             ],
             dim=-1,
         )
-        rgb = self.mlp_head(h).view(*ray_samples.frustums.directions.shape[:-1], -1).to(directions)
+        rgb = self.mlp_head(h).view(*outputs_shape, -1).to(directions)
         outputs.update({FieldHeadNames.RGB: rgb})
 
         return outputs
 
 
 class TorchNerfactoField(Field):
     """
     PyTorch implementation of the compound field.
     """
 
     def __init__(
         self,
-        aabb,
+        aabb: TensorType,
         num_images: int,
         position_encoding: Encoding = HashEncoding(),
         direction_encoding: Encoding = SHEncoding(),
         base_mlp_num_layers: int = 3,
         base_mlp_layer_width: int = 64,
         head_mlp_num_layers: int = 2,
         head_mlp_layer_width: int = 32,
@@ -323,37 +371,38 @@
         )
 
         self.field_output_density = DensityFieldHead(in_dim=self.mlp_base.get_out_dim())
         self.field_heads = nn.ModuleList(field_heads)
         for field_head in self.field_heads:
             field_head.set_in_dim(self.mlp_head.get_out_dim())  # type: ignore
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         if self.spatial_distortion is not None:
             positions = ray_samples.frustums.get_positions()
             positions = self.spatial_distortion(positions)
         else:
             positions = ray_samples.frustums.get_positions()
         encoded_xyz = self.position_encoding(positions)
         base_mlp_out = self.mlp_base(encoded_xyz)
         density = self.field_output_density(base_mlp_out)
         return density, base_mlp_out
 
     def get_outputs(
         self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
     ) -> Dict[FieldHeadNames, TensorType]:
+        outputs_shape = ray_samples.frustums.directions.shape[:-1]
 
         if ray_samples.camera_indices is None:
             raise AttributeError("Camera indices are not provided.")
         camera_indices = ray_samples.camera_indices.squeeze()
         if self.training:
             embedded_appearance = self.embedding_appearance(camera_indices)
         else:
             embedded_appearance = torch.zeros(
-                (*ray_samples.frustums.directions.shape[:-1], self.appearance_embedding_dim),
+                (*outputs_shape, self.appearance_embedding_dim),
                 device=ray_samples.frustums.directions.device,
             )
 
         outputs = {}
         for field_head in self.field_heads:
             encoded_dir = self.direction_encoding(ray_samples.frustums.directions)
             mlp_out = self.mlp_head(
@@ -366,8 +415,8 @@
                     dim=-1,  # type:ignore
                 )
             )
             outputs[field_head.field_head_name] = field_head(mlp_out)
         return outputs
 
 
-field_implementation_to_class = {"tcnn": TCNNNerfactoField, "torch": TorchNerfactoField}
+field_implementation_to_class: Dict[str, Field] = {"tcnn": TCNNNerfactoField, "torch": TorchNerfactoField}
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/nerfw_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/nerfw_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Args:
         num_images: How many images exist in the dataset.
         position_encoding: Position encoder.
         direction_encoding: Direction encoder.
         base_mlp_num_layers: Number of layers for base MLP.
         base_mlp_layer_width: Width of base MLP layers.
-        head_mlp_num_layers: Number of layer for ourput head MLP.
+        head_mlp_num_layers: Number of layer for output head MLP.
         head_mlp_layer_width: Width of output head MLP layers.
         appearance_embedding_dim:: Dimension of appearance embedding.
         transient_embedding_dim:: Dimension of transient embedding.
         skip_connections: Where to add skip connection in base MLP.
     """
 
     def __init__(
@@ -105,15 +105,15 @@
         self.field_head_density = DensityFieldHead(in_dim=self.mlp_base.get_out_dim())
         self.field_head_rgb = RGBFieldHead(in_dim=self.mlp_head.get_out_dim())
 
         self.field_head_transient_uncertainty = UncertaintyFieldHead(in_dim=self.mlp_transient.get_out_dim())
         self.field_head_transient_rgb = TransientRGBFieldHead(in_dim=self.mlp_transient.get_out_dim())
         self.field_head_transient_density = TransientDensityFieldHead(in_dim=self.mlp_transient.get_out_dim())
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         """Computes and returns the densities."""
         encoded_xyz = self.position_encoding(ray_samples.frustums.get_positions())
         encoded_xyz = self.position_encoding(ray_samples.frustums.get_positions())
         base_mlp_out = self.mlp_base(encoded_xyz)
         density = self.field_head_density(base_mlp_out)
         return density, base_mlp_out
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/semantic_nerf_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     Args:
         num_semantic_classes: Number of distinct semantic classes.
         position_encoding: Position encoder.
         direction_encoding: Direction encoder.
         base_mlp_num_layers: Number of layers for base MLP.
         base_mlp_layer_width: Width of base MLP layers.
-        head_mlp_num_layers: Number of layer for ourput head MLP.
+        head_mlp_num_layers: Number of layer for output head MLP.
         head_mlp_layer_width: Width of output head MLP layers.
         skip_connections: Where to add skip connection in base MLP.
     """
 
     def __init__(
         self,
         num_semantic_classes: int,
@@ -84,15 +84,15 @@
         )
         self.field_head_density = DensityFieldHead(in_dim=self.mlp_base.get_out_dim())
         self.field_head_rgb = RGBFieldHead(in_dim=self.mlp_head.get_out_dim())
         self.field_head_semantic = SemanticFieldHead(
             in_dim=self.mlp_semantic.get_out_dim(), num_classes=self.num_semantic_classes
         )
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         encoded_xyz = self.position_encoding(ray_samples.frustums.get_positions())
         base_mlp_out = self.mlp_base(encoded_xyz)
         density = self.field_head_density(base_mlp_out)
         return density, base_mlp_out
 
     def get_outputs(
         self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/tensorf_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/tensorf_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """TensoRF Field"""
 
 
-from typing import Optional
+from typing import Dict, Optional
 
 import torch
 from torch import nn
 from torch.nn.parameter import Parameter
 from torchtyping import TensorType
 
 from nerfstudio.cameras.rays import RaySamples
@@ -31,15 +31,15 @@
 
 
 class TensoRFField(Field):
     """TensoRF Field"""
 
     def __init__(
         self,
-        aabb,
+        aabb: TensorType,
         # the aabb bounding box of the dataset
         feature_encoding: Encoding = Identity(in_dim=3),
         # the encoding method used for appearance encoding outputs
         direction_encoding: Encoding = Identity(in_dim=3),
         # the encoding method used for ray direction
         density_encoding: Encoding = Identity(in_dim=3),
         # the tensor encoding method used for scene density
@@ -79,25 +79,27 @@
                 in_features=self.color_encoding.get_out_dim(), out_features=3 * self.sh.get_out_dim(), bias=False
             )
         else:
             self.B = nn.Linear(in_features=self.color_encoding.get_out_dim(), out_features=appearance_dim, bias=False)
 
         self.field_output_rgb = RGBFieldHead(in_dim=self.mlp_head.get_out_dim(), activation=nn.Sigmoid())
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> TensorType:
         positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        positions = positions * 2 - 1
         density = self.density_encoding(positions)
         density_enc = torch.sum(density, dim=-1)[:, :, None]
         relu = torch.nn.ReLU()
         density_enc = relu(density_enc)
         return density_enc
 
     def get_outputs(self, ray_samples: RaySamples, density_embedding: Optional[TensorType] = None) -> TensorType:
         d = ray_samples.frustums.directions
         positions = SceneBox.get_normalized_positions(ray_samples.frustums.get_positions(), self.aabb)
+        positions = positions * 2 - 1
         rgb_features = self.color_encoding(positions)
         rgb_features = self.B(rgb_features)
 
         d_encoded = self.direction_encoding(d)
         rgb_features_encoded = self.feature_encoding(rgb_features)
 
         if self.use_sh:
@@ -107,16 +109,22 @@
         else:
             out = self.mlp_head(torch.cat([rgb_features, d, rgb_features_encoded, d_encoded], dim=-1))  # type: ignore
             rgb = self.field_output_rgb(out)
 
         return rgb
 
     def forward(
-        self, ray_samples: RaySamples, mask: Optional[TensorType] = None, bg_color: Optional[TensorType] = None
-    ):
+        self,
+        ray_samples: RaySamples,
+        compute_normals: bool = False,
+        mask: Optional[TensorType] = None,
+        bg_color: Optional[TensorType] = None,
+    ) -> Dict[FieldHeadNames, TensorType]:
+        if compute_normals is True:
+            raise ValueError("Surface normals are not currently supported with TensoRF")
         if mask is not None and bg_color is not None:
             base_density = torch.zeros(ray_samples.shape)[:, :, None].to(mask.device)
             base_rgb = bg_color.repeat(ray_samples[:, :, None].shape)
             if mask.any():
                 input_rays = ray_samples[mask, :]
                 density = self.get_density(input_rays)
                 rgb = self.get_outputs(input_rays, None)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-0.2.0/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """NeRF Field
 
     Args:
         position_encoding: Position encoder.
         direction_encoding: Direction encoder.
         base_mlp_num_layers: Number of layers for base MLP.
         base_mlp_layer_width: Width of base MLP layers.
-        head_mlp_num_layers: Number of layer for ourput head MLP.
+        head_mlp_num_layers: Number of layer for output head MLP.
         head_mlp_layer_width: Width of output head MLP layers.
         skip_connections: Where to add skip connection in base MLP.
         use_integrated_encoding: Used integrated samples as encoding input.
         spatial_distortion: Spatial distortion.
     """
 
     def __init__(
@@ -54,15 +54,15 @@
         position_encoding: Encoding = Identity(in_dim=3),
         direction_encoding: Encoding = Identity(in_dim=3),
         base_mlp_num_layers: int = 8,
         base_mlp_layer_width: int = 256,
         head_mlp_num_layers: int = 2,
         head_mlp_layer_width: int = 128,
         skip_connections: Tuple[int] = (4,),
-        field_heads: Tuple[FieldHead] = (RGBFieldHead(),),
+        field_heads: Optional[Tuple[FieldHead]] = (RGBFieldHead(),),
         use_integrated_encoding: bool = False,
         spatial_distortion: Optional[SpatialDistortion] = None,
     ) -> None:
         super().__init__()
         self.position_encoding = position_encoding
         self.direction_encoding = direction_encoding
         self.use_integrated_encoding = use_integrated_encoding
@@ -84,15 +84,15 @@
         )
 
         self.field_output_density = DensityFieldHead(in_dim=self.mlp_base.get_out_dim())
         self.field_heads = nn.ModuleList(field_heads)
         for field_head in self.field_heads:
             field_head.set_in_dim(self.mlp_head.get_out_dim())  # type: ignore
 
-    def get_density(self, ray_samples: RaySamples):
+    def get_density(self, ray_samples: RaySamples) -> Tuple[TensorType, TensorType]:
         if self.use_integrated_encoding:
             gaussian_samples = ray_samples.frustums.get_gaussian_blob()
             if self.spatial_distortion is not None:
                 gaussian_samples = self.spatial_distortion(gaussian_samples)
             encoded_xyz = self.position_encoding(gaussian_samples.mean, covs=gaussian_samples.cov)
         else:
             positions = ray_samples.frustums.get_positions()
```

### Comparing `nerfstudio-0.1.9/nerfstudio/model_components/__init__.py` & `nerfstudio-0.2.0/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/model_components/ray_generators.py` & `nerfstudio-0.2.0/nerfstudio/model_components/ray_generators.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,35 +25,35 @@
 
 class RayGenerator(nn.Module):
     """torch.nn Module for generating rays.
     This class is the interface between the scene's cameras/camera optimizer and the ray sampler.
 
     Args:
         cameras: Camera objects containing camera info.
-        pose_optimizer: pose optimization module, for optimizing noisy camera intrisics/extrinsics.
+        pose_optimizer: pose optimization module, for optimizing noisy camera intrinsics/extrinsics.
     """
 
     def __init__(self, cameras: Cameras, pose_optimizer: CameraOptimizer) -> None:
         super().__init__()
         self.cameras = cameras
         self.pose_optimizer = pose_optimizer
-        self.image_coords = nn.Parameter(cameras.get_image_coords(), requires_grad=False)
+        self.register_buffer("image_coords", cameras.get_image_coords(), persistent=False)
 
     def forward(self, ray_indices: TensorType["num_rays", 3]) -> RayBundle:
         """Index into the cameras to generate the rays.
 
         Args:
-            ray_indices: Contains camera, row, and col indicies for target rays.
+            ray_indices: Contains camera, row, and col indices for target rays.
         """
         c = ray_indices[:, 0]  # camera indices
         y = ray_indices[:, 1]  # row indices
         x = ray_indices[:, 2]  # col indices
         coords = self.image_coords[y, x]
 
         camera_opt_to_camera = self.pose_optimizer(c)
 
         ray_bundle = self.cameras.generate_rays(
-            camera_indices=c,
+            camera_indices=c.unsqueeze(-1),
             coords=coords,
             camera_opt_to_camera=camera_opt_to_camera,
         )
         return ray_bundle
```

### Comparing `nerfstudio-0.1.9/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-0.2.0/nerfstudio/model_components/ray_samplers.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Collection of sampling strategies
 """
 
 from abc import abstractmethod
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import nerfacc
 import torch
 from nerfacc import OccupancyGrid
 from torch import nn
 from torchtyping import TensorType
 
@@ -54,15 +54,15 @@
 class SpacedSampler(Sampler):
     """Sample points according to a function.
 
     Args:
         num_samples: Number of samples per ray
         spacing_fn: Function that dictates sample spacing (ie `lambda x : x` is uniform).
         spacing_fn_inv: The inverse of spacing_fn.
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
         single_jitter: Use a same random jitter for all samples along a ray. Defaults to False
     """
 
     def __init__(
         self,
         spacing_fn: Callable,
         spacing_fn_inv: Callable,
@@ -77,15 +77,15 @@
         self.spacing_fn_inv = spacing_fn_inv
 
     def generate_ray_samples(
         self,
         ray_bundle: Optional[RayBundle] = None,
         num_samples: Optional[int] = None,
     ) -> RaySamples:
-        """Generates position samples accoring to spacing function.
+        """Generates position samples according to spacing function.
 
         Args:
             ray_bundle: Rays to generate samples for
             num_samples: Number of samples per ray
 
         Returns:
             Positions and deltas for samples along a ray
@@ -127,15 +127,15 @@
 
 
 class UniformSampler(SpacedSampler):
     """Sample uniformly along a ray
 
     Args:
         num_samples: Number of samples per ray
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
         single_jitter: Use a same random jitter for all samples along a ray. Defaults to False
     """
 
     def __init__(
         self,
         num_samples: Optional[int] = None,
         train_stratified=True,
@@ -151,15 +151,15 @@
 
 
 class LinearDisparitySampler(SpacedSampler):
     """Sample linearly in disparity along a ray
 
     Args:
         num_samples: Number of samples per ray
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
         single_jitter: Use a same random jitter for all samples along a ray. Defaults to False
     """
 
     def __init__(
         self,
         num_samples: Optional[int] = None,
         train_stratified=True,
@@ -175,15 +175,15 @@
 
 
 class SqrtSampler(SpacedSampler):
     """Square root sampler along a ray
 
     Args:
         num_samples: Number of samples per ray
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
     """
 
     def __init__(
         self,
         num_samples: Optional[int] = None,
         train_stratified=True,
         single_jitter=False,
@@ -198,15 +198,15 @@
 
 
 class LogSampler(SpacedSampler):
     """Log sampler along a ray
 
     Args:
         num_samples: Number of samples per ray
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
     """
 
     def __init__(
         self,
         num_samples: Optional[int] = None,
         train_stratified=True,
         single_jitter=False,
@@ -223,15 +223,15 @@
 class UniformLinDispPiecewiseSampler(SpacedSampler):
     """Piecewise sampler along a ray that allocates the first half of the samples uniformly and the second half
     using linearly in disparity spacing.
 
 
     Args:
         num_samples: Number of samples per ray
-        train_stratified: Use stratified sampling during training. Defults to True
+        train_stratified: Use stratified sampling during training. Defaults to True
         single_jitter: Use a same random jitter for all samples along a ray. Defaults to False
     """
 
     def __init__(
         self,
         num_samples: Optional[int] = None,
         train_stratified=True,
@@ -389,15 +389,14 @@
 
         super().__init__()
         self.scene_aabb = scene_aabb
         self.density_fn = density_fn
         self.occupancy_grid = occupancy_grid
         if self.scene_aabb is not None:
             self.scene_aabb = self.scene_aabb.to("cuda").flatten()
-        print(self.scene_aabb)
 
     def get_sigma_fn(self, origins, directions) -> Optional[Callable]:
         """Returns a function that returns the density of a point.
 
         Args:
             origins: Origins of rays
             directions: Directions of rays
@@ -427,60 +426,70 @@
     def forward(
         self,
         ray_bundle: RayBundle,
         render_step_size: float,
         near_plane: float = 0.0,
         far_plane: Optional[float] = None,
         cone_angle: float = 0.0,
-    ) -> Tuple[RaySamples, TensorType["total_samples", 3], TensorType["total_samples", 2]]:
+    ) -> Tuple[RaySamples, TensorType["total_samples",]]:
         """Generate ray samples in a bounding box.
 
         Args:
             ray_bundle: Rays to generate samples for
             render_step_size: Minimum step size to use for rendering
             near_plane: Near plane for raymarching
             far_plane: Far plane for raymarching
             cone_angle: Cone angle for raymarching, set to 0 for uniform marching.
 
         Returns:
             a tuple of (ray_samples, packed_info, ray_indices)
             The ray_samples are packed, only storing the valid samples.
-            The packed_info contains all the information to recover packed samples into unpacked mode for rendering.
             The ray_indices contains the indices of the rays that each sample belongs to.
         """
 
         rays_o = ray_bundle.origins.contiguous()
         rays_d = ray_bundle.directions.contiguous()
+
+        if ray_bundle.nears is not None and ray_bundle.fars is not None:
+            t_min = ray_bundle.nears.contiguous().reshape(-1)
+            t_max = ray_bundle.fars.contiguous().reshape(-1)
+
+        else:
+            t_min = None
+            t_max = None
+
         if ray_bundle.camera_indices is not None:
             camera_indices = ray_bundle.camera_indices.contiguous()
         else:
             camera_indices = None
 
-        packed_info, starts, ends = nerfacc.ray_marching(
+        ray_indices, starts, ends = nerfacc.ray_marching(
             rays_o=rays_o,
             rays_d=rays_d,
+            t_min=t_min,
+            t_max=t_max,
             scene_aabb=self.scene_aabb,
             grid=self.occupancy_grid,
-            sigma_fn=self.get_sigma_fn(rays_o, rays_d),
+            # this is a workaround - using density causes crash and damage quality. should be fixed
+            sigma_fn=None,  # self.get_sigma_fn(rays_o, rays_d),
             render_step_size=render_step_size,
             near_plane=near_plane,
             far_plane=far_plane,
             stratified=self.training,
             cone_angle=cone_angle,
             alpha_thre=1e-2,
         )
         num_samples = starts.shape[0]
         if num_samples == 0:
             # create a single fake sample and update packed_info accordingly
             # this says the last ray in packed_info has 1 sample, which starts and ends at 1
-            packed_info[-1, 1] = 1
+            ray_indices = torch.zeros((1,), dtype=torch.long, device=rays_o.device)
             starts = torch.ones((1, 1), dtype=starts.dtype, device=rays_o.device)
             ends = torch.ones((1, 1), dtype=ends.dtype, device=rays_o.device)
 
-        ray_indices = nerfacc.unpack_info(packed_info)
         origins = rays_o[ray_indices]
         dirs = rays_d[ray_indices]
         if camera_indices is not None:
             camera_indices = camera_indices[ray_indices]
 
         zeros = torch.zeros_like(origins[:, :1])
         ray_samples = RaySamples(
@@ -489,38 +498,53 @@
                 directions=dirs,
                 starts=starts,
                 ends=ends,
                 pixel_area=zeros,
             ),
             camera_indices=camera_indices,
         )
-        return ray_samples, packed_info, ray_indices
+        if ray_bundle.times is not None:
+            ray_samples.times = ray_bundle.times[ray_indices]
+        return ray_samples, ray_indices
 
 
 class ProposalNetworkSampler(Sampler):
-    """Sampler that uses a proposal network to generate samples."""
+    """Sampler that uses a proposal network to generate samples.
+
+    Args:
+        num_proposal_samples_per_ray: Number of samples to generate per ray for each proposal step.
+        num_nerf_samples_per_ray: Number of samples to generate per ray for the NERF model.
+        num_proposal_network_iterations: Number of proposal network iterations to run.
+        single_jitter: Use a same random jitter for all samples along a ray.
+        update_sched: A function that takes the iteration number of steps between updates.
+        initial_sampler: Sampler to use for the first iteration. Uses UniformLinDispPiecewise if not set.
+    """
 
     def __init__(
         self,
         num_proposal_samples_per_ray: Tuple[int] = (64,),
         num_nerf_samples_per_ray: int = 32,
         num_proposal_network_iterations: int = 2,
         single_jitter: bool = False,
         update_sched: Callable = lambda x: 1,
+        initial_sampler: Optional[Sampler] = None,
     ) -> None:
         super().__init__()
         self.num_proposal_samples_per_ray = num_proposal_samples_per_ray
         self.num_nerf_samples_per_ray = num_nerf_samples_per_ray
         self.num_proposal_network_iterations = num_proposal_network_iterations
         self.update_sched = update_sched
         if self.num_proposal_network_iterations < 1:
             raise ValueError("num_proposal_network_iterations must be >= 1")
 
         # samplers
-        self.initial_sampler = UniformLinDispPiecewiseSampler(single_jitter=single_jitter)
+        if initial_sampler is None:
+            self.initial_sampler = UniformLinDispPiecewiseSampler(single_jitter=single_jitter)
+        else:
+            self.initial_sampler = initial_sampler
         self.pdf_sampler = PDFSampler(include_original=False, single_jitter=single_jitter)
 
         self._anneal = 1.0
         self._steps_since_update = 0
         self._step = 0
 
     def set_anneal(self, anneal: float) -> None:
@@ -570,7 +594,175 @@
                 weights_list.append(weights)  # (num_rays, num_samples)
                 ray_samples_list.append(ray_samples)
         if updated:
             self._steps_since_update = 0
 
         assert ray_samples is not None
         return ray_samples, weights_list, ray_samples_list
+
+
+class NeuSSampler(Sampler):
+    """NeuS sampler that uses a sdf network to generate samples with fixed variance value in each iterations."""
+
+    def __init__(
+        self,
+        num_samples: int = 64,
+        num_samples_importance: int = 64,
+        num_samples_outside: int = 32,
+        num_upsample_steps: int = 4,
+        base_variance: float = 64,
+        single_jitter: bool = True,
+    ) -> None:
+        super().__init__()
+        self.num_samples = num_samples
+        self.num_samples_importance = num_samples_importance
+        self.num_samples_outside = num_samples_outside
+        self.num_upsample_steps = num_upsample_steps
+        self.base_variance = base_variance
+        self.single_jitter = single_jitter
+
+        # samplers
+        self.uniform_sampler = UniformSampler(single_jitter=single_jitter)
+        self.pdf_sampler = PDFSampler(
+            include_original=False,
+            single_jitter=single_jitter,
+            histogram_padding=1e-5,
+        )
+        self.outside_sampler = LinearDisparitySampler()
+
+    def generate_ray_samples(
+        self,
+        ray_bundle: Optional[RayBundle] = None,
+        sdf_fn: Optional[Callable] = None,
+        ray_samples: Optional[RaySamples] = None,
+    ) -> Union[Tuple[RaySamples, torch.Tensor], RaySamples]:
+        assert ray_bundle is not None
+        assert sdf_fn is not None
+
+        # Start with uniform sampling
+        if ray_samples is None:
+            ray_samples = self.uniform_sampler(ray_bundle, num_samples=self.num_samples)
+        assert ray_samples is not None
+
+        total_iters = 0
+        sorted_index = None
+        new_samples = ray_samples
+
+        base_variance = self.base_variance
+
+        while total_iters < self.num_upsample_steps:
+
+            with torch.no_grad():
+                new_sdf = sdf_fn(new_samples)
+
+            # merge sdf predictions
+            if sorted_index is not None:
+                sdf_merge = torch.cat([sdf.squeeze(-1), new_sdf.squeeze(-1)], -1)
+                sdf = torch.gather(sdf_merge, 1, sorted_index).unsqueeze(-1)
+            else:
+                sdf = new_sdf
+
+            # compute with fix variances
+            alphas = self.rendering_sdf_with_fixed_inv_s(
+                ray_samples, sdf.reshape(ray_samples.shape), inv_s=base_variance * 2**total_iters
+            )
+
+            weights = ray_samples.get_weights_and_transmittance_from_alphas(alphas[..., None], weights_only=True)
+            weights = torch.cat((weights, torch.zeros_like(weights[:, :1])), dim=1)
+
+            new_samples = self.pdf_sampler(
+                ray_bundle,
+                ray_samples,
+                weights,
+                num_samples=self.num_samples_importance // self.num_upsample_steps,
+            )
+
+            ray_samples, sorted_index = self.merge_ray_samples(ray_bundle, ray_samples, new_samples)
+
+            total_iters += 1
+
+        return ray_samples
+
+    @staticmethod
+    def rendering_sdf_with_fixed_inv_s(
+        ray_samples: RaySamples, sdf: TensorType["num_samples", -1], inv_s: int
+    ) -> TensorType["num_samples", -1]:
+        """
+        rendering given a fixed inv_s as NeuS
+
+        Args:
+            ray_samples: samples along ray
+            sdf: sdf values along ray
+            inv_s: fixed variance value
+        Returns:
+            alpha value
+        """
+        batch_size = ray_samples.shape[0]
+        prev_sdf, next_sdf = sdf[:, :-1], sdf[:, 1:]
+        assert ray_samples.deltas is not None
+        deltas = ray_samples.deltas[:, :-1, 0]
+        mid_sdf = (prev_sdf + next_sdf) * 0.5
+        cos_val = (next_sdf - prev_sdf) / (deltas + 1e-5)
+
+        # ----------------------------------------------------------------------------------------------------------
+        # Use min value of [ cos, prev_cos ]
+        # Though it makes the sampling (not rendering) a little bit biased, this strategy can make the sampling more
+        # robust when meeting situations like below:
+        #
+        # SDF
+        # ^
+        # |\          -----x----...
+        # | \        /
+        # |  x      x
+        # |---\----/-------------> 0 level
+        # |    \  /
+        # |     \/
+        # |
+        # ----------------------------------------------------------------------------------------------------------
+        prev_cos_val = torch.cat([torch.zeros([batch_size, 1], device=sdf.device), cos_val[:, :-1]], dim=-1)
+        cos_val = torch.stack([prev_cos_val, cos_val], dim=-1)
+        cos_val, _ = torch.min(cos_val, dim=-1, keepdim=False)
+        cos_val = cos_val.clip(-1e3, 0.0)
+
+        dist = deltas
+        prev_esti_sdf = mid_sdf - cos_val * dist * 0.5
+        next_esti_sdf = mid_sdf + cos_val * dist * 0.5
+        prev_cdf = torch.sigmoid(prev_esti_sdf * inv_s)
+        next_cdf = torch.sigmoid(next_esti_sdf * inv_s)
+        alpha = (prev_cdf - next_cdf + 1e-5) / (prev_cdf + 1e-5)
+
+        return alpha
+
+    @staticmethod
+    def merge_ray_samples(ray_bundle: RayBundle, ray_samples_1: RaySamples, ray_samples_2: RaySamples):
+        """Merge two set of ray samples and return sorted index which can be used to merge sdf values
+        Args:
+            ray_samples_1 : ray_samples to merge
+            ray_samples_2 : ray_samples to merge
+        """
+
+        assert ray_samples_1.spacing_starts is not None and ray_samples_2.spacing_starts is not None
+        assert ray_samples_1.spacing_ends is not None and ray_samples_2.spacing_ends is not None
+        assert ray_samples_1.spacing_to_euclidean_fn is not None
+        starts_1 = ray_samples_1.spacing_starts[..., 0]
+        starts_2 = ray_samples_2.spacing_starts[..., 0]
+
+        ends = torch.maximum(ray_samples_1.spacing_ends[..., -1:, 0], ray_samples_2.spacing_ends[..., -1:, 0])
+
+        bins, sorted_index = torch.sort(torch.cat([starts_1, starts_2], -1), -1)
+
+        bins = torch.cat([bins, ends], dim=-1)
+
+        # Stop gradients
+        bins = bins.detach()
+
+        euclidean_bins = ray_samples_1.spacing_to_euclidean_fn(bins)
+
+        ray_samples = ray_bundle.get_ray_samples(
+            bin_starts=euclidean_bins[..., :-1, None],
+            bin_ends=euclidean_bins[..., 1:, None],
+            spacing_starts=bins[..., :-1, None],
+            spacing_ends=bins[..., 1:, None],
+            spacing_to_euclidean_fn=ray_samples_1.spacing_to_euclidean_fn,
+        )
+
+        return ray_samples, sorted_index
```

### Comparing `nerfstudio-0.1.9/nerfstudio/model_components/renderers.py` & `nerfstudio-0.2.0/nerfstudio/model_components/renderers.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,44 +22,60 @@
     field_outputs = field(ray_sampler)
     weights = ray_sampler.get_weights(field_outputs[FieldHeadNames.DENSITY])
 
     rgb_renderer = RGBRenderer()
     rgb = rgb_renderer(rgb=field_outputs[FieldHeadNames.RGB], weights=weights)
 
 """
+import contextlib
 import math
-from typing import Optional, Union
+from typing import Generator, Optional, Union
 
 import nerfacc
 import torch
 from torch import nn
 from torchtyping import TensorType
 from typing_extensions import Literal
 
 from nerfstudio.cameras.rays import RaySamples
-from nerfstudio.utils.math import components_from_spherical_harmonics
+from nerfstudio.utils import colors
+from nerfstudio.utils.math import components_from_spherical_harmonics, safe_normalize
+
+BACKGROUND_COLOR_OVERRIDE: Optional[TensorType[3]] = None
+
+
+@contextlib.contextmanager
+def background_color_override_context(mode: TensorType[3]) -> Generator[None, None, None]:
+    """Context manager for setting background mode."""
+    global BACKGROUND_COLOR_OVERRIDE  # pylint: disable=global-statement
+    old_background_color = BACKGROUND_COLOR_OVERRIDE
+    try:
+        BACKGROUND_COLOR_OVERRIDE = mode
+        yield
+    finally:
+        BACKGROUND_COLOR_OVERRIDE = old_background_color
 
 
 class RGBRenderer(nn.Module):
-    """Standard volumetic rendering.
+    """Standard volumetric rendering.
 
     Args:
         background_color: Background color as RGB. Uses random colors if None.
     """
 
     def __init__(self, background_color: Union[Literal["random", "last_sample"], TensorType[3]] = "random") -> None:
         super().__init__()
         self.background_color = background_color
 
     @classmethod
     def combine_rgb(
         cls,
         rgb: TensorType["bs":..., "num_samples", 3],
         weights: TensorType["bs":..., "num_samples", 1],
-        background_color: Union[Literal["random", "last_sample"], TensorType[3]] = "random",
+        background_color: Union[Literal["random", "white", "black", "last_sample"], TensorType[3]] = "random",
         ray_indices: Optional[TensorType["num_samples"]] = None,
         num_rays: Optional[int] = None,
     ) -> TensorType["bs":..., 3]:
         """Composite samples along ray and render color image
 
         Args:
             rgb: RGB for each sample
@@ -77,18 +93,22 @@
                 raise NotImplementedError("Background color 'last_sample' not implemented for packed samples.")
             comp_rgb = nerfacc.accumulate_along_rays(weights, ray_indices, rgb, num_rays)
             accumulated_weight = nerfacc.accumulate_along_rays(weights, ray_indices, None, num_rays)
         else:
             comp_rgb = torch.sum(weights * rgb, dim=-2)
             accumulated_weight = torch.sum(weights, dim=-2)
 
+        if BACKGROUND_COLOR_OVERRIDE is not None:
+            background_color = BACKGROUND_COLOR_OVERRIDE
         if background_color == "last_sample":
             background_color = rgb[..., -1, :]
         if background_color == "random":
             background_color = torch.rand_like(comp_rgb).to(rgb.device)
+        if isinstance(background_color, str) and background_color in colors.COLORS_DICT:
+            background_color = colors.COLORS_DICT[background_color].to(rgb.device)
 
         assert isinstance(background_color, torch.Tensor)
         comp_rgb = comp_rgb + background_color.to(weights.device) * (1.0 - accumulated_weight)
 
         return comp_rgb
 
     def forward(
@@ -106,14 +126,16 @@
             ray_indices: Ray index for each sample, used when samples are packed.
             num_rays: Number of rays, used when samples are packed.
 
         Returns:
             Outputs of rgb values.
         """
 
+        if not self.training:
+            rgb = torch.nan_to_num(rgb)
         rgb = self.combine_rgb(
             rgb, weights, background_color=self.background_color, ray_indices=ray_indices, num_rays=num_rays
         )
         if not self.training:
             torch.clamp_(rgb, min=0.0, max=1.0)
         return rgb
 
@@ -140,34 +162,38 @@
         sh: TensorType[..., "num_samples", "coeffs"],
         directions: TensorType[..., "num_samples", 3],
         weights: TensorType[..., "num_samples", 1],
     ) -> TensorType[..., 3]:
         """Composite samples along ray and render color image
 
         Args:
-            sh: Spherical hamonics coefficients for each sample
+            sh: Spherical harmonics coefficients for each sample
             directions: Sample direction
             weights: Weights for each sample
 
         Returns:
             Outputs of rgb values.
         """
 
         sh = sh.view(*sh.shape[:-1], 3, sh.shape[-1] // 3)
 
         levels = int(math.sqrt(sh.shape[-1]))
         components = components_from_spherical_harmonics(levels=levels, directions=directions)
 
         rgb = sh * components[..., None, :]  # [..., num_samples, 3, sh_components]
-        rgb = torch.sum(sh, dim=-1) + 0.5  # [..., num_samples, 3]
+        rgb = torch.sum(rgb, dim=-1)  # [..., num_samples, 3]
 
         if self.activation is not None:
-            self.activation(rgb)
+            rgb = self.activation(rgb)
 
+        if not self.training:
+            rgb = torch.nan_to_num(rgb)
         rgb = RGBRenderer.combine_rgb(rgb, weights, background_color=self.background_color)
+        if not self.training:
+            torch.clamp_(rgb, min=0.0, max=1.0)
 
         return rgb
 
 
 class AccumulationRenderer(nn.Module):
     """Accumulated value along a ray."""
 
@@ -286,10 +312,33 @@
 
     @classmethod
     def forward(
         cls,
         semantics: TensorType["bs":..., "num_samples", "num_classes"],
         weights: TensorType["bs":..., "num_samples", 1],
     ) -> TensorType["bs":..., "num_classes"]:
-        """_summary_"""
+        """Calculate semantics along the ray."""
         sem = torch.sum(weights * semantics, dim=-2)
         return sem
+
+
+class NormalsRenderer(nn.Module):
+    """Calculate normals along the ray."""
+
+    @classmethod
+    def forward(
+        cls,
+        normals: TensorType["bs":..., "num_samples", 3],
+        weights: TensorType["bs":..., "num_samples", 1],
+        normalize: bool = True,
+    ) -> TensorType["bs":..., 3]:
+        """Calculate normals along the ray.
+
+        Args:
+            normals: Normals for each sample.
+            weights: Weights of each sample.
+            normalize: Normalize normals.
+        """
+        n = torch.sum(weights * normals, dim=-2)
+        if normalize:
+            n = safe_normalize(n)
+        return n
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/__init__.py` & `nerfstudio-0.2.0/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/models/base_model.py` & `nerfstudio-0.2.0/nerfstudio/models/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,17 +70,19 @@
         scene_box: SceneBox,
         num_train_data: int,
         **kwargs,
     ) -> None:
         super().__init__()
         self.config = config
         self.scene_box = scene_box
+        self.render_aabb = None  # the box that we want to render - should be a subset of scene_box
         self.num_train_data = num_train_data
         self.kwargs = kwargs
         self.collider = None
+
         self.populate_modules()  # populate the modules
         self.callbacks = None
         # to keep track of which device the nn.Module is on
         self.device_indicator_param = nn.Parameter(torch.empty(0))
 
     @property
     def device(self):
@@ -95,14 +97,15 @@
 
     def populate_modules(self):
         """Set the necessary modules to get the network working."""
         # default instantiates optional modules that are common among many networks
         # NOTE: call `super().populate_modules()` in subclasses
 
         if self.config.enable_collider:
+            assert self.config.collider_params is not None
             self.collider = NearFarCollider(
                 near_plane=self.config.collider_params["near_plane"], far_plane=self.config.collider_params["far_plane"]
             )
 
     @abstractmethod
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         """Obtain the parameter groups for the optimizers
@@ -205,16 +208,14 @@
 
         Args:
             loaded_state: dictionary of pre-trained model states
         """
         state = {key.replace("module.", ""): value for key, value in loaded_state["model"].items()}
         self.load_state_dict(state)  # type: ignore
 
+    def update_to_step(self, step: int) -> None:
+        """Called when loading a model from a checkpoint. Sets any model parameters that change over
+        training to the correct value, based on the training step of the checkpoint.
 
-@dataclass
-class VanillaModelConfig(ModelConfig):
-    """Vanilla Model Config"""
-
-    num_coarse_samples: int = 64
-    """Number of samples in coarse field evaluation"""
-    num_importance_samples: int = 128
-    """Number of samples in fine field evaluation"""
+        Args:
+            step: training step of the loaded checkpoint
+        """
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/instant_ngp.py` & `nerfstudio-0.2.0/nerfstudio/models/instant_ngp.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import nerfacc
 import torch
 from nerfacc import ContractionType
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
+from typing_extensions import Literal
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
@@ -41,15 +42,15 @@
 from nerfstudio.model_components.ray_samplers import VolumetricSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
 )
 from nerfstudio.models.base_model import Model, ModelConfig
-from nerfstudio.utils import colormaps, colors
+from nerfstudio.utils import colormaps
 
 
 @dataclass
 class InstantNGPModelConfig(ModelConfig):
     """Instant NGP Model Config"""
 
     _target: Type = field(
@@ -60,28 +61,32 @@
     """Whether to create a scene collider to filter rays."""
     collider_params: Optional[Dict[str, float]] = None
     """Instant NGP doesn't use a collider."""
     max_num_samples_per_ray: int = 24
     """Number of samples in field evaluation."""
     grid_resolution: int = 128
     """Resolution of the grid used for the field."""
+    max_res: int = 2048
+    """Maximum resolution of the hashmap for the base mlp."""
+    log2_hashmap_size: int = 19
+    """Size of the hashmap for the base mlp"""
     contraction_type: ContractionType = ContractionType.UN_BOUNDED_SPHERE
-    """Resolution of the grid used for the field."""
+    """Contraction type used for spatial deformation of the field."""
     cone_angle: float = 0.004
     """Should be set to 0.0 for blender scenes but 1./256 for real scenes."""
     render_step_size: float = 0.01
     """Minimum step size for rendering."""
     near_plane: float = 0.05
     """How far along ray to start sampling."""
     far_plane: float = 1e3
     """How far along ray to stop sampling."""
     use_appearance_embedding: bool = False
     """Whether to use an appearance embedding."""
-    randomize_background: bool = True
-    """Whether to randomize the background color."""
+    background_color: Literal["random", "black", "white"] = "random"
+    """The color that is given to untrained areas."""
 
 
 class NGPModel(Model):
     """Instant NGP model
 
     Args:
         config: instant NGP configuration to instantiate model
@@ -98,14 +103,16 @@
         super().populate_modules()
 
         self.field = TCNNInstantNGPField(
             aabb=self.scene_box.aabb,
             contraction_type=self.config.contraction_type,
             use_appearance_embedding=self.config.use_appearance_embedding,
             num_images=self.num_train_data,
+            log2_hashmap_size=self.config.log2_hashmap_size,
+            max_res=self.config.max_res,
         )
 
         self.scene_aabb = Parameter(self.scene_box.aabb.flatten(), requires_grad=False)
 
         # Occupancy Grid
         self.occupancy_grid = nerfacc.OccupancyGrid(
             roi_aabb=self.scene_aabb,
@@ -118,26 +125,25 @@
         self.sampler = VolumetricSampler(
             scene_aabb=vol_sampler_aabb,
             occupancy_grid=self.occupancy_grid,
             density_fn=self.field.density_fn,
         )
 
         # renderers
-        background_color = "random" if self.config.randomize_background else colors.WHITE
-        self.renderer_rgb = RGBRenderer(background_color=background_color)
+        self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
         self.renderer_accumulation = AccumulationRenderer()
         self.renderer_depth = DepthRenderer(method="expected")
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         def update_occupancy_grid(step: int):
             # TODO: needs to get access to the sampler, on how the step size is determinated at each x. See
             # https://github.com/KAIR-BAIR/nerfacc/blob/127223b11401125a9fce5ce269bb0546ee4de6e8/examples/train_ngp_nerf.py#L190-L213
@@ -162,25 +168,26 @@
         return param_groups
 
     def get_outputs(self, ray_bundle: RayBundle):
         assert self.field is not None
         num_rays = len(ray_bundle)
 
         with torch.no_grad():
-            ray_samples, packed_info, ray_indices = self.sampler(
+            ray_samples, ray_indices = self.sampler(
                 ray_bundle=ray_bundle,
                 near_plane=self.config.near_plane,
                 far_plane=self.config.far_plane,
                 render_step_size=self.config.render_step_size,
                 cone_angle=self.config.cone_angle,
             )
 
         field_outputs = self.field(ray_samples)
 
         # accumulation
+        packed_info = nerfacc.pack_info(ray_indices, num_rays)
         weights = nerfacc.render_weight_from_density(
             packed_info=packed_info,
             sigmas=field_outputs[FieldHeadNames.DENSITY],
             t_starts=ray_samples.frustums.starts,
             t_ends=ray_samples.frustums.ends,
         )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/mipnerf.py` & `nerfstudio-0.2.0/nerfstudio/models/mipnerf.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
         if self.field is None:
             raise ValueError("populate_fields() must be called before get_param_groups")
         param_groups["fields"] = list(self.field.parameters())
         return param_groups
@@ -169,16 +169,16 @@
         combined_acc = torch.cat([acc_coarse, acc_fine], dim=1)
         combined_depth = torch.cat([depth_coarse, depth_fine], dim=1)
 
         # Switch images from [H, W, C] to [1, C, H, W] for metrics computations
         image = torch.moveaxis(image, -1, 0)[None, ...]
         rgb_coarse = torch.moveaxis(rgb_coarse, -1, 0)[None, ...]
         rgb_fine = torch.moveaxis(rgb_fine, -1, 0)[None, ...]
-        rgb_coarse = torch.clip(rgb_coarse, min=-1, max=1)
-        rgb_fine = torch.clip(rgb_fine, min=-1, max=1)
+        rgb_coarse = torch.clip(rgb_coarse, min=0, max=1)
+        rgb_fine = torch.clip(rgb_fine, min=0, max=1)
 
         coarse_psnr = self.psnr(image, rgb_coarse)
         fine_psnr = self.psnr(image, rgb_fine)
         fine_ssim = self.ssim(image, rgb_fine)
         fine_lpips = self.lpips(image, rgb_fine)
 
         metrics_dict = {
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/nerfacto.py` & `nerfstudio-0.2.0/nerfstudio/models/nerfacto.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,70 +35,103 @@
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
 from nerfstudio.field_components.field_heads import FieldHeadNames
 from nerfstudio.field_components.spatial_distortions import SceneContraction
 from nerfstudio.fields.density_fields import HashMLPDensityField
 from nerfstudio.fields.nerfacto_field import TCNNNerfactoField
-from nerfstudio.model_components.losses import MSELoss, distortion_loss, interlevel_loss
-from nerfstudio.model_components.ray_samplers import ProposalNetworkSampler
+from nerfstudio.model_components.losses import (
+    MSELoss,
+    distortion_loss,
+    interlevel_loss,
+    orientation_loss,
+    pred_normal_loss,
+)
+from nerfstudio.model_components.ray_samplers import (
+    ProposalNetworkSampler,
+    UniformSampler,
+)
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
+    NormalsRenderer,
     RGBRenderer,
 )
 from nerfstudio.model_components.scene_colliders import NearFarCollider
+from nerfstudio.model_components.shaders import NormalsShader
 from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils import colormaps
 
 
 @dataclass
 class NerfactoModelConfig(ModelConfig):
     """Nerfacto Model Config"""
 
     _target: Type = field(default_factory=lambda: NerfactoModel)
     near_plane: float = 0.05
     """How far along the ray to start sampling."""
     far_plane: float = 1000.0
     """How far along the ray to stop sampling."""
-    background_color: Literal["background", "last_sample"] = "last_sample"
+    background_color: Literal["random", "last_sample", "black", "white"] = "last_sample"
     """Whether to randomize the background color."""
-    num_proposal_samples_per_ray: Tuple[int] = (256, 96)
-    """Number of samples per ray for the proposal network."""
+    hidden_dim: int = 64
+    """Dimension of hidden layers"""
+    hidden_dim_color: int = 64
+    """Dimension of hidden layers for color network"""
+    hidden_dim_transient: int = 64
+    """Dimension of hidden layers for transient network"""
+    num_levels: int = 16
+    """Number of levels of the hashmap for the base mlp."""
+    max_res: int = 2048
+    """Maximum resolution of the hashmap for the base mlp."""
+    log2_hashmap_size: int = 19
+    """Size of the hashmap for the base mlp"""
+    num_proposal_samples_per_ray: Tuple[int, ...] = (256, 96)
+    """Number of samples per ray for each proposal network."""
     num_nerf_samples_per_ray: int = 48
     """Number of samples per ray for the nerf network."""
     proposal_update_every: int = 5
     """Sample every n steps after the warmup"""
     proposal_warmup: int = 5000
     """Scales n from 1 to proposal_update_every over this many steps"""
     num_proposal_iterations: int = 2
     """Number of proposal network iterations."""
     use_same_proposal_network: bool = False
     """Use the same proposal network. Otherwise use different ones."""
     proposal_net_args_list: List[Dict] = field(
         default_factory=lambda: [
-            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 64},
-            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256},
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 128, "use_linear": False},
+            {"hidden_dim": 16, "log2_hashmap_size": 17, "num_levels": 5, "max_res": 256, "use_linear": False},
         ]
     )
     """Arguments for the proposal density fields."""
+    proposal_initial_sampler: Literal["piecewise", "uniform"] = "piecewise"
+    """Initial sampler for the proposal network. Piecewise is preferred for unbounded scenes."""
     interlevel_loss_mult: float = 1.0
     """Proposal loss multiplier."""
     distortion_loss_mult: float = 0.002
     """Distortion loss multiplier."""
+    orientation_loss_mult: float = 0.0001
+    """Orientation loss multiplier on computed normals."""
+    pred_normal_loss_mult: float = 0.001
+    """Predicted normal loss multiplier."""
     use_proposal_weight_anneal: bool = True
     """Whether to use proposal weight annealing."""
     use_average_appearance_embedding: bool = True
     """Whether to use average appearance embedding or zeros for inference."""
     proposal_weights_anneal_slope: float = 10.0
     """Slope of the annealing function for the proposal weights."""
     proposal_weights_anneal_max_num_iters: int = 1000
     """Max num iterations for the annealing function."""
     use_single_jitter: bool = True
     """Whether use single jitter or not for the proposal networks."""
+    predict_normals: bool = False
+    """Whether to predict normals or not."""
+    disable_scene_contraction: bool = False
+    """Whether to disable scene contraction or not."""
 
 
 class NerfactoModel(Model):
     """Nerfacto model
 
     Args:
         config: Nerfacto configuration to instantiate model
@@ -106,21 +139,31 @@
 
     config: NerfactoModelConfig
 
     def populate_modules(self):
         """Set the fields and modules."""
         super().populate_modules()
 
-        scene_contraction = SceneContraction(order=float("inf"))
+        if self.config.disable_scene_contraction:
+            scene_contraction = None
+        else:
+            scene_contraction = SceneContraction(order=float("inf"))
 
         # Fields
         self.field = TCNNNerfactoField(
             self.scene_box.aabb,
+            hidden_dim=self.config.hidden_dim,
+            num_levels=self.config.num_levels,
+            max_res=self.config.max_res,
+            log2_hashmap_size=self.config.log2_hashmap_size,
+            hidden_dim_color=self.config.hidden_dim_color,
+            hidden_dim_transient=self.config.hidden_dim_transient,
             spatial_distortion=scene_contraction,
             num_images=self.num_train_data,
+            use_pred_normals=self.config.predict_normals,
             use_average_appearance_embedding=self.config.use_average_appearance_embedding,
         )
 
         self.density_fns = []
         num_prop_nets = self.config.num_proposal_iterations
         # Build the proposal network(s)
         self.proposal_networks = torch.nn.ModuleList()
@@ -143,37 +186,48 @@
 
         # Samplers
         update_schedule = lambda step: np.clip(
             np.interp(step, [0, self.config.proposal_warmup], [0, self.config.proposal_update_every]),
             1,
             self.config.proposal_update_every,
         )
+
+        # Change proposal network initial sampler if uniform
+        initial_sampler = None  # None is for piecewise as default (see ProposalNetworkSampler)
+        if self.config.proposal_initial_sampler == "uniform":
+            initial_sampler = UniformSampler(single_jitter=self.config.use_single_jitter)
+
         self.proposal_sampler = ProposalNetworkSampler(
             num_nerf_samples_per_ray=self.config.num_nerf_samples_per_ray,
             num_proposal_samples_per_ray=self.config.num_proposal_samples_per_ray,
             num_proposal_network_iterations=self.config.num_proposal_iterations,
             single_jitter=self.config.use_single_jitter,
             update_sched=update_schedule,
+            initial_sampler=initial_sampler,
         )
 
         # Collider
         self.collider = NearFarCollider(near_plane=self.config.near_plane, far_plane=self.config.far_plane)
 
         # renderers
         self.renderer_rgb = RGBRenderer(background_color=self.config.background_color)
         self.renderer_accumulation = AccumulationRenderer()
         self.renderer_depth = DepthRenderer()
+        self.renderer_normals = NormalsRenderer()
+
+        # shaders
+        self.normals_shader = NormalsShader()
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
         param_groups["proposal_networks"] = list(self.proposal_networks.parameters())
         param_groups["fields"] = list(self.field.parameters())
         return param_groups
 
@@ -206,30 +260,50 @@
                     func=self.proposal_sampler.step_cb,
                 )
             )
         return callbacks
 
     def get_outputs(self, ray_bundle: RayBundle):
         ray_samples, weights_list, ray_samples_list = self.proposal_sampler(ray_bundle, density_fns=self.density_fns)
-        field_outputs = self.field(ray_samples)
+        field_outputs = self.field(ray_samples, compute_normals=self.config.predict_normals)
         weights = ray_samples.get_weights(field_outputs[FieldHeadNames.DENSITY])
         weights_list.append(weights)
         ray_samples_list.append(ray_samples)
 
         rgb = self.renderer_rgb(rgb=field_outputs[FieldHeadNames.RGB], weights=weights)
         depth = self.renderer_depth(weights=weights, ray_samples=ray_samples)
         accumulation = self.renderer_accumulation(weights=weights)
 
-        outputs = {"rgb": rgb, "accumulation": accumulation, "depth": depth}
-
+        outputs = {
+            "rgb": rgb,
+            "accumulation": accumulation,
+            "depth": depth,
+        }
+
+        if self.config.predict_normals:
+            normals = self.renderer_normals(normals=field_outputs[FieldHeadNames.NORMALS], weights=weights)
+            pred_normals = self.renderer_normals(field_outputs[FieldHeadNames.PRED_NORMALS], weights=weights)
+            outputs["normals"] = self.normals_shader(normals)
+            outputs["pred_normals"] = self.normals_shader(pred_normals)
         # These use a lot of GPU memory, so we avoid storing them for eval.
         if self.training:
             outputs["weights_list"] = weights_list
             outputs["ray_samples_list"] = ray_samples_list
 
+        if self.training and self.config.predict_normals:
+            outputs["rendered_orientation_loss"] = orientation_loss(
+                weights.detach(), field_outputs[FieldHeadNames.NORMALS], ray_bundle.directions
+            )
+
+            outputs["rendered_pred_normal_loss"] = pred_normal_loss(
+                weights.detach(),
+                field_outputs[FieldHeadNames.NORMALS].detach(),
+                field_outputs[FieldHeadNames.PRED_NORMALS],
+            )
+
         for i in range(self.config.num_proposal_iterations):
             outputs[f"prop_depth_{i}"] = self.renderer_depth(weights=weights_list[i], ray_samples=ray_samples_list[i])
 
         return outputs
 
     def get_metrics_dict(self, outputs, batch):
         metrics_dict = {}
@@ -245,20 +319,29 @@
         loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
         if self.training:
             loss_dict["interlevel_loss"] = self.config.interlevel_loss_mult * interlevel_loss(
                 outputs["weights_list"], outputs["ray_samples_list"]
             )
             assert metrics_dict is not None and "distortion" in metrics_dict
             loss_dict["distortion_loss"] = self.config.distortion_loss_mult * metrics_dict["distortion"]
+            if self.config.predict_normals:
+                # orientation loss for computed normals
+                loss_dict["orientation_loss"] = self.config.orientation_loss_mult * torch.mean(
+                    outputs["rendered_orientation_loss"]
+                )
+
+                # ground truth supervision for normals
+                loss_dict["pred_normal_loss"] = self.config.pred_normal_loss_mult * torch.mean(
+                    outputs["rendered_pred_normal_loss"]
+                )
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
-
         image = batch["image"].to(self.device)
         rgb = outputs["rgb"]
         acc = colormaps.apply_colormap(outputs["accumulation"])
         depth = colormaps.apply_depth_colormap(
             outputs["depth"],
             accumulation=outputs["accumulation"],
         )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-0.2.0/nerfstudio/models/semantic_nerfw.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 @dataclass
 class SemanticNerfWModelConfig(NerfactoModelConfig):
     """Nerfacto Model Config"""
 
     _target: Type = field(default_factory=lambda: SemanticNerfWModel)
     use_transient_embedding: bool = False
     """Whether to use transient embedding."""
+    semantic_loss_weight: float = 1.0
+    pass_semantic_gradients: bool = False
 
 
 class SemanticNerfWModel(Model):
     """Nerfacto model
 
     Args:
         config: Nerfacto configuration to instantiate model
@@ -72,33 +74,38 @@
 
     config: SemanticNerfWModelConfig
 
     def __init__(self, config: SemanticNerfWModelConfig, metadata: Dict, **kwargs) -> None:
         assert "semantics" in metadata.keys() and isinstance(metadata["semantics"], Semantics)
         self.semantics = metadata["semantics"]
         super().__init__(config=config, **kwargs)
+        self.colormap = self.semantics.colors.clone().detach().to(self.device)
 
     def populate_modules(self):
         """Set the fields and modules."""
         super().populate_modules()
 
         scene_contraction = SceneContraction(order=float("inf"))
 
         if self.config.use_transient_embedding:
             raise ValueError("Transient embedding is not fully working for semantic nerf-w.")
 
         # Fields
         self.field = TCNNNerfactoField(
             self.scene_box.aabb,
+            num_levels=self.config.num_levels,
+            max_res=self.config.max_res,
+            log2_hashmap_size=self.config.log2_hashmap_size,
             spatial_distortion=scene_contraction,
             num_images=self.num_train_data,
             use_average_appearance_embedding=self.config.use_average_appearance_embedding,
             use_transient_embedding=self.config.use_transient_embedding,
             use_semantics=True,
             num_semantic_classes=len(self.semantics.classes),
+            pass_semantic_gradients=self.config.pass_semantic_gradients,
         )
 
         # Build the proposal network(s)
         self.proposal_networks = torch.nn.ModuleList()
         if self.config.use_same_proposal_network:
             network = HashMLPDensityField(self.scene_box.aabb, spatial_distortion=scene_contraction)
             self.proposal_networks.append(network)
@@ -130,15 +137,15 @@
         # losses
         self.rgb_loss = MSELoss()
         self.cross_entropy_loss = torch.nn.CrossEntropyLoss(reduction="mean")
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
         param_groups["proposal_networks"] = list(self.proposal_networks.parameters())
         param_groups["fields"] = list(self.field.parameters())
         return param_groups
 
@@ -200,21 +207,24 @@
         if self.training and self.config.use_transient_embedding:
             weights_transient = ray_samples.get_weights(field_outputs[FieldHeadNames.TRANSIENT_DENSITY])
             uncertainty = self.renderer_uncertainty(field_outputs[FieldHeadNames.UNCERTAINTY], weights_transient)
             outputs["uncertainty"] = uncertainty + 0.03  # NOTE(ethan): this is the uncertainty min
             outputs["density_transient"] = field_outputs[FieldHeadNames.TRANSIENT_DENSITY]
 
         # semantics
+        semantic_weights = weights_static
+        if not self.config.pass_semantic_gradients:
+            semantic_weights = semantic_weights.detach()
         outputs["semantics"] = self.renderer_semantics(
-            field_outputs[FieldHeadNames.SEMANTICS], weights=weights_static.detach()
+            field_outputs[FieldHeadNames.SEMANTICS], weights=semantic_weights
         )
 
         # semantics colormaps
         semantic_labels = torch.argmax(torch.nn.functional.softmax(outputs["semantics"], dim=-1), dim=-1)
-        outputs["semantics_colormap"] = self.semantics.colors[semantic_labels]
+        outputs["semantics_colormap"] = self.colormap.to(self.device)[semantic_labels]
 
         return outputs
 
     def get_metrics_dict(self, outputs, batch):
         metrics_dict = {}
         image = batch["image"].to(self.device)
         metrics_dict["psnr"] = self.psnr(outputs["rgb"], image)
@@ -236,15 +246,17 @@
             loss_dict["uncertainty_loss"] = 3 + torch.log(betas).mean()
             loss_dict["density_loss"] = 0.01 * outputs["density_transient"].mean()
             loss_dict["rgb_loss"] = (((image - outputs["rgb"]) ** 2).sum(-1) / (betas[..., 0] ** 2)).mean()
         else:
             loss_dict["rgb_loss"] = self.rgb_loss(image, outputs["rgb"])
 
         # semantic loss
-        loss_dict["semantics_loss"] = self.cross_entropy_loss(outputs["semantics"], batch["semantics"][..., 0].long())
+        loss_dict["semantics_loss"] = self.config.semantic_loss_weight * self.cross_entropy_loss(
+            outputs["semantics"], batch["semantics"][..., 0].long()
+        )
         return loss_dict
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
 
         image = batch["image"].to(self.device)
@@ -280,13 +292,13 @@
                 outputs[key],
                 accumulation=outputs["accumulation"],
             )
             images_dict[key] = prop_depth_i
 
         # semantics
         semantic_labels = torch.argmax(torch.nn.functional.softmax(outputs["semantics"], dim=-1), dim=-1)
-        images_dict["semantics_colormap"] = self.semantics.colors[semantic_labels]
+        images_dict["semantics_colormap"] = self.colormap.to(self.device)[semantic_labels]
 
         # valid mask
         images_dict["mask"] = batch["mask"].repeat(1, 1, 3)
 
         return metrics_dict, images_dict
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/tensorf.py` & `nerfstudio-0.2.0/nerfstudio/models/tensorf.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,68 +23,79 @@
 
 import numpy as np
 import torch
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
+from typing_extensions import Literal
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.configs.config_utils import to_immutable_dict
 from nerfstudio.engine.callbacks import (
     TrainingCallback,
     TrainingCallbackAttributes,
     TrainingCallbackLocation,
 )
-from nerfstudio.field_components.encodings import NeRFEncoding, TensorVMEncoding
+from nerfstudio.field_components.encodings import (
+    NeRFEncoding,
+    TensorCPEncoding,
+    TensorVMEncoding,
+    TriplaneEncoding,
+)
 from nerfstudio.field_components.field_heads import FieldHeadNames
 from nerfstudio.fields.tensorf_field import TensoRFField
 from nerfstudio.model_components.losses import MSELoss
 from nerfstudio.model_components.ray_samplers import PDFSampler, UniformSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
 )
 from nerfstudio.model_components.scene_colliders import AABBBoxCollider
-from nerfstudio.models.base_model import Model, VanillaModelConfig
+from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils import colormaps, colors, misc
 
 
 @dataclass
-class TensoRFModelConfig(VanillaModelConfig):
+class TensoRFModelConfig(ModelConfig):
     """TensoRF model config"""
 
     _target: Type = field(default_factory=lambda: TensoRFModel)
     """target class to instantiate"""
     init_resolution: int = 128
     """initial render resolution"""
     final_resolution: int = 300
     """final render resolution"""
     upsampling_iters: Tuple[int, ...] = (2000, 3000, 4000, 5500, 7000)
     """specifies a list of iteration step numbers to perform upsampling"""
     loss_coefficients: Dict[str, float] = to_immutable_dict({"rgb_loss": 1.0})
     """Loss specific weights."""
-    num_samples: int = 256
+    num_samples: int = 50
     """Number of samples in field evaluation"""
+    num_uniform_samples: int = 200
+    """Number of samples in density evaluation"""
     num_den_components: int = 16
     """Number of components in density encoding"""
     num_color_components: int = 48
     """Number of components in color encoding"""
     appearance_dim: int = 27
     """Number of channels for color encoding"""
+    tensorf_encoding: Literal["triplane", "vm", "cp"] = "vm"
 
 
 class TensoRFModel(Model):
     """TensoRF Model
 
     Args:
         config: TensoRF configuration to instantiate model
     """
 
+    config: TensoRFModelConfig
+
     def __init__(
         self,
         config: TensoRFModelConfig,
         **kwargs,
     ) -> None:
         self.init_resolution = config.init_resolution
         self.upsampling_iters = config.upsampling_iters
@@ -105,61 +116,99 @@
             .tolist()[1:]
         )
         super().__init__(config=config, **kwargs)
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
-
         # the callback that we want to run every X iterations after the training iteration
         def reinitialize_optimizer(
             self, training_callback_attributes: TrainingCallbackAttributes, step: int  # pylint: disable=unused-argument
         ):
-            resolution = self.upsampling_steps.pop(0)
+            index = self.upsampling_iters.index(step)
+            resolution = self.upsampling_steps[index]
 
             # upsample the position and direction grids
             self.field.density_encoding.upsample_grid(resolution)
             self.field.color_encoding.upsample_grid(resolution)
 
             # reinitialize the encodings optimizer
             optimizers_config = training_callback_attributes.optimizers.config
             enc = training_callback_attributes.pipeline.get_param_groups()["encodings"]
             lr_init = optimizers_config["encodings"]["optimizer"].lr
 
             training_callback_attributes.optimizers.optimizers["encodings"] = optimizers_config["encodings"][
                 "optimizer"
             ].setup(params=enc)
             if optimizers_config["encodings"]["scheduler"]:
-                training_callback_attributes.optimizers.schedulers["encodings"] = optimizers_config["encodings"][
-                    "scheduler"
-                ].setup(optimizer=training_callback_attributes.optimizers.optimizers["encodings"], lr_init=lr_init)
+                training_callback_attributes.optimizers.schedulers["encodings"] = (
+                    optimizers_config["encodings"]["scheduler"]
+                    .setup()
+                    .get_scheduler(
+                        optimizer=training_callback_attributes.optimizers.optimizers["encodings"], lr_init=lr_init
+                    )
+                )
 
         callbacks = [
             TrainingCallback(
                 where_to_run=[TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
                 iters=self.upsampling_iters,
                 func=reinitialize_optimizer,
                 args=[self, training_callback_attributes],
             )
         ]
         return callbacks
 
+    def update_to_step(self, step: int) -> None:
+        if step < self.upsampling_iters[0]:
+            return
+
+        new_iters = list(self.upsampling_iters) + [step + 1]
+        new_iters.sort()
+
+        index = new_iters.index(step + 1)
+        new_grid_resolution = self.upsampling_steps[index - 1]
+
+        self.field.density_encoding.upsample_grid(new_grid_resolution)  # type: ignore
+        self.field.color_encoding.upsample_grid(new_grid_resolution)  # type: ignore
+
     def populate_modules(self):
         """Set the fields and modules"""
         super().populate_modules()
 
         # setting up fields
-        density_encoding = TensorVMEncoding(
-            resolution=self.init_resolution,
-            num_components=self.num_den_components,
-        )
-        color_encoding = TensorVMEncoding(
-            resolution=self.init_resolution,
-            num_components=self.num_color_components,
-        )
+        if self.config.tensorf_encoding == "vm":
+            density_encoding = TensorVMEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
+            )
+            color_encoding = TensorVMEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        elif self.config.tensorf_encoding == "cp":
+            density_encoding = TensorCPEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
+            )
+            color_encoding = TensorCPEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        elif self.config.tensorf_encoding == "triplane":
+            density_encoding = TriplaneEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_den_components,
+            )
+            color_encoding = TriplaneEncoding(
+                resolution=self.init_resolution,
+                num_components=self.num_color_components,
+            )
+        else:
+            raise ValueError(f"Encoding {self.config.tensorf_encoding} not supported")
 
         feature_encoding = NeRFEncoding(in_dim=self.appearance_dim, num_frequencies=2, min_freq_exp=0, max_freq_exp=2)
         direction_encoding = NeRFEncoding(in_dim=3, num_frequencies=2, min_freq_exp=0, max_freq_exp=2)
 
         self.field = TensoRFField(
             self.scene_box.aabb,
             feature_encoding=feature_encoding,
@@ -169,29 +218,29 @@
             appearance_dim=self.appearance_dim,
             head_mlp_num_layers=2,
             head_mlp_layer_width=128,
             use_sh=False,
         )
 
         # samplers
-        self.sampler_uniform = UniformSampler(num_samples=self.config.num_samples, single_jitter=True)
-        self.sampler_pdf = PDFSampler(num_samples=self.config.num_samples // 2, single_jitter=True)
+        self.sampler_uniform = UniformSampler(num_samples=self.config.num_uniform_samples, single_jitter=True)
+        self.sampler_pdf = PDFSampler(num_samples=self.config.num_samples, single_jitter=True, include_original=False)
 
         # renderers
         self.renderer_rgb = RGBRenderer(background_color=colors.WHITE)
         self.renderer_accumulation = AccumulationRenderer()
         self.renderer_depth = DepthRenderer()
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
 
         # colliders
         if self.config.enable_collider:
             self.collider = AABBBoxCollider(scene_box=self.scene_box)
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
@@ -215,15 +264,17 @@
         coarse_accumulation = self.renderer_accumulation(weights)
         acc_mask = torch.where(coarse_accumulation < 0.0001, False, True).reshape(-1)
 
         # pdf sampling
         ray_samples_pdf = self.sampler_pdf(ray_bundle, ray_samples_uniform, weights)
 
         # fine field:
-        field_outputs_fine = self.field.forward(ray_samples_pdf, acc_mask, colors.WHITE.to(weights.device))
+        field_outputs_fine = self.field.forward(
+            ray_samples_pdf, mask=acc_mask, bg_color=colors.WHITE.to(weights.device)
+        )
 
         weights_fine = ray_samples_pdf.get_weights(field_outputs_fine[FieldHeadNames.DENSITY])
 
         accumulation = self.renderer_accumulation(weights_fine)
         depth = self.renderer_depth(weights_fine, ray_samples_pdf)
 
         rgb = self.renderer_rgb(
@@ -250,14 +301,15 @@
 
     def get_image_metrics_and_images(
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
         image = batch["image"].to(outputs["rgb"].device)
         rgb = outputs["rgb"]
         acc = colormaps.apply_colormap(outputs["accumulation"])
+        assert self.config.collider_params is not None
         depth = colormaps.apply_depth_colormap(
             outputs["depth"],
             accumulation=outputs["accumulation"],
             near_plane=self.config.collider_params["near_plane"],
             far_plane=self.config.collider_params["far_plane"],
         )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-0.2.0/nerfstudio/models/vanilla_nerf.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,51 +14,71 @@
 
 """
 Implementation of vanilla nerf.
 """
 
 from __future__ import annotations
 
-from typing import Dict, List, Tuple
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Tuple, Type
 
 import torch
 from torch.nn import Parameter
 from torchmetrics import PeakSignalNoiseRatio
 from torchmetrics.functional import structural_similarity_index_measure
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
 from nerfstudio.cameras.rays import RayBundle
+from nerfstudio.configs.config_utils import to_immutable_dict
 from nerfstudio.field_components.encodings import NeRFEncoding
 from nerfstudio.field_components.field_heads import FieldHeadNames
+from nerfstudio.field_components.temporal_distortions import TemporalDistortionKind
 from nerfstudio.fields.vanilla_nerf_field import NeRFField
 from nerfstudio.model_components.losses import MSELoss
 from nerfstudio.model_components.ray_samplers import PDFSampler, UniformSampler
 from nerfstudio.model_components.renderers import (
     AccumulationRenderer,
     DepthRenderer,
     RGBRenderer,
 )
 from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils import colormaps, colors, misc
 
 
+@dataclass
+class VanillaModelConfig(ModelConfig):
+    """Vanilla Model Config"""
+
+    _target: Type = field(default_factory=lambda: NeRFModel)
+    num_coarse_samples: int = 64
+    """Number of samples in coarse field evaluation"""
+    num_importance_samples: int = 128
+    """Number of samples in fine field evaluation"""
+
+    enable_temporal_distortion: bool = False
+    """Specifies whether or not to include ray warping based on time."""
+    temporal_distortion_params: Dict[str, Any] = to_immutable_dict({"kind": TemporalDistortionKind.DNERF})
+    """Parameters to instantiate temporal distortion with"""
+
+
 class NeRFModel(Model):
     """Vanilla NeRF model
 
     Args:
         config: Basic NeRF configuration to instantiate model
     """
 
     def __init__(
         self,
-        config: ModelConfig,
+        config: VanillaModelConfig,
         **kwargs,
     ) -> None:
         self.field_coarse = None
         self.field_fine = None
+        self.temporal_distortion = None
 
         super().__init__(
             config=config,
             **kwargs,
         )
 
     def populate_modules(self):
@@ -69,16 +89,23 @@
         position_encoding = NeRFEncoding(
             in_dim=3, num_frequencies=10, min_freq_exp=0.0, max_freq_exp=8.0, include_input=True
         )
         direction_encoding = NeRFEncoding(
             in_dim=3, num_frequencies=4, min_freq_exp=0.0, max_freq_exp=4.0, include_input=True
         )
 
-        self.field_coarse = NeRFField(position_encoding=position_encoding, direction_encoding=direction_encoding)
-        self.field_fine = NeRFField(position_encoding=position_encoding, direction_encoding=direction_encoding)
+        self.field_coarse = NeRFField(
+            position_encoding=position_encoding,
+            direction_encoding=direction_encoding,
+        )
+
+        self.field_fine = NeRFField(
+            position_encoding=position_encoding,
+            direction_encoding=direction_encoding,
+        )
 
         # samplers
         self.sampler_uniform = UniformSampler(num_samples=self.config.num_coarse_samples)
         self.sampler_pdf = PDFSampler(num_samples=self.config.num_importance_samples)
 
         # renderers
         self.renderer_rgb = RGBRenderer(background_color=colors.WHITE)
@@ -87,43 +114,56 @@
 
         # losses
         self.rgb_loss = MSELoss()
 
         # metrics
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = structural_similarity_index_measure
-        self.lpips = LearnedPerceptualImagePatchSimilarity()
+        self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
+
+        if getattr(self.config, "enable_temporal_distortion", False):
+            params = self.config.temporal_distortion_params
+            kind = params.pop("kind")
+            self.temporal_distortion = kind.to_temporal_distortion(params)
 
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         param_groups = {}
         if self.field_coarse is None or self.field_fine is None:
             raise ValueError("populate_fields() must be called before get_param_groups")
         param_groups["fields"] = list(self.field_coarse.parameters()) + list(self.field_fine.parameters())
+        if self.temporal_distortion is not None:
+            param_groups["temporal_distortion"] = list(self.temporal_distortion.parameters())
         return param_groups
 
     def get_outputs(self, ray_bundle: RayBundle):
 
         if self.field_coarse is None or self.field_fine is None:
             raise ValueError("populate_fields() must be called before get_outputs")
 
         # uniform sampling
         ray_samples_uniform = self.sampler_uniform(ray_bundle)
+        if self.temporal_distortion is not None:
+            offsets = self.temporal_distortion(ray_samples_uniform.frustums.get_positions(), ray_samples_uniform.times)
+            ray_samples_uniform.frustums.set_offsets(offsets)
 
         # coarse field:
         field_outputs_coarse = self.field_coarse.forward(ray_samples_uniform)
         weights_coarse = ray_samples_uniform.get_weights(field_outputs_coarse[FieldHeadNames.DENSITY])
         rgb_coarse = self.renderer_rgb(
             rgb=field_outputs_coarse[FieldHeadNames.RGB],
             weights=weights_coarse,
         )
         accumulation_coarse = self.renderer_accumulation(weights_coarse)
         depth_coarse = self.renderer_depth(weights_coarse, ray_samples_uniform)
 
         # pdf sampling
         ray_samples_pdf = self.sampler_pdf(ray_bundle, ray_samples_uniform, weights_coarse)
+        if self.temporal_distortion is not None:
+            offsets = self.temporal_distortion(ray_samples_pdf.frustums.get_positions(), ray_samples_pdf.times)
+            ray_samples_pdf.frustums.set_offsets(offsets)
 
         # fine field:
         field_outputs_fine = self.field_fine.forward(ray_samples_pdf)
         weights_fine = ray_samples_pdf.get_weights(field_outputs_fine[FieldHeadNames.DENSITY])
         rgb_fine = self.renderer_rgb(
             rgb=field_outputs_fine[FieldHeadNames.RGB],
             weights=weights_fine,
@@ -157,14 +197,15 @@
         self, outputs: Dict[str, torch.Tensor], batch: Dict[str, torch.Tensor]
     ) -> Tuple[Dict[str, float], Dict[str, torch.Tensor]]:
         image = batch["image"].to(outputs["rgb_coarse"].device)
         rgb_coarse = outputs["rgb_coarse"]
         rgb_fine = outputs["rgb_fine"]
         acc_coarse = colormaps.apply_colormap(outputs["accumulation_coarse"])
         acc_fine = colormaps.apply_colormap(outputs["accumulation_fine"])
+        assert self.config.collider_params is not None
         depth_coarse = colormaps.apply_depth_colormap(
             outputs["depth_coarse"],
             accumulation=outputs["accumulation_coarse"],
             near_plane=self.config.collider_params["near_plane"],
             far_plane=self.config.collider_params["far_plane"],
         )
         depth_fine = colormaps.apply_depth_colormap(
```

### Comparing `nerfstudio-0.1.9/nerfstudio/pipelines/__init__.py` & `nerfstudio-0.2.0/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-0.2.0/nerfstudio/pipelines/base_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 """
 from __future__ import annotations
 
 import typing
 from abc import abstractmethod
 from dataclasses import dataclass, field
 from time import time
-from typing import Any, Dict, List, Optional, Type, Union, cast
+from typing import Any, Dict, List, Mapping, Optional, Type, Union, cast
 
 import torch
 import torch.distributed as dist
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
     TextColumn,
     TimeElapsedColumn,
 )
 from torch import nn
 from torch.nn import Parameter
 from torch.nn.parallel import DistributedDataParallel as DDP
+from typing_extensions import Literal
 
 from nerfstudio.configs import base_config as cfg
 from nerfstudio.data.datamanagers.base_datamanager import (
     DataManager,
+    DataManagerConfig,
     VanillaDataManager,
     VanillaDataManagerConfig,
 )
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes
 from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils import profiler
 
@@ -73,38 +75,61 @@
     Hopefully this provides a higher level interface for the trainer to use, and
     simplifying the model classes, which each may have different forward() methods
     and so on.
 
     Args:
         config: configuration to instantiate pipeline
         device: location to place model and data
-        test_mode: if True, loads test datset. if False, loads train/eval datasets
+        test_mode:
+            'train': loads train/eval datasets into memory
+            'test': loads train/test dataset into memory
+            'inference': does not load any dataset into memory
         world_size: total number of machines available
         local_rank: rank of current machine
 
     Attributes:
         datamanager: The data manager that will be used
         model: The model that will be used
     """
 
     # pylint: disable=abstract-method
 
     datamanager: DataManager
     _model: Model
+    world_size: int
 
     @property
     def model(self):
         """Returns the unwrapped model if in ddp"""
         return module_wrapper(self._model)
 
     @property
     def device(self):
         """Returns the device that the model is on."""
         return self.model.device
 
+    def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True):
+        is_ddp_model_state = True
+        model_state = {}
+        for key, value in state_dict.items():
+            if key.startswith("_model."):
+                # remove the "_model." prefix from key
+                model_state[key[len("_model.") :]] = value
+                # make sure that the "module." prefix comes from DDP,
+                # rather than an attribute of the model named "module"
+                if not key.startswith("_model.module."):
+                    is_ddp_model_state = False
+        # remove "module." prefix added by DDP
+        if is_ddp_model_state:
+            model_state = {key[len("module.") :]: value for key, value in model_state.items()}
+
+        pipeline_state = {key: value for key, value in state_dict.items() if not key.startswith("_model.")}
+        self.model.load_state_dict(model_state, strict=strict)
+        super().load_state_dict(pipeline_state, strict=False)
+
     @profiler.time_function
     def get_train_loss_dict(self, step: int):
         """This function gets your training loss dict. This will be responsible for
         getting the next batch of data from the DataManager and interfacing with the
         Model class, feeding the data to the model's forward function.
 
         Args:
@@ -150,19 +175,20 @@
         """
 
     @abstractmethod
     @profiler.time_function
     def get_average_eval_image_metrics(self, step: Optional[int] = None):
         """Iterate over all the images in the eval dataset and get the average."""
 
-    def load_pipeline(self, loaded_state: Dict[str, Any]) -> None:
+    def load_pipeline(self, loaded_state: Dict[str, Any], step: int) -> None:
         """Load the checkpoint from the given path
 
         Args:
             loaded_state: pre-trained model state dict
+            step: training step of the loaded checkpoint
         """
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         """Returns the training callbacks from both the Dataloader and the Model."""
 
@@ -176,55 +202,60 @@
 
 @dataclass
 class VanillaPipelineConfig(cfg.InstantiateConfig):
     """Configuration for pipeline instantiation"""
 
     _target: Type = field(default_factory=lambda: VanillaPipeline)
     """target class to instantiate"""
-    datamanager: VanillaDataManagerConfig = VanillaDataManagerConfig()
+    datamanager: DataManagerConfig = VanillaDataManagerConfig()
     """specifies the datamanager config"""
     model: ModelConfig = ModelConfig()
     """specifies the model config"""
 
 
 class VanillaPipeline(Pipeline):
     """The pipeline class for the vanilla nerf setup of multiple cameras for one or a few scenes.
 
+    Args:
         config: configuration to instantiate pipeline
         device: location to place model and data
-        test_mode: if True, loads test datset. if False, loads train/eval datasets
+        test_mode:
+            'val': loads train/val datasets into memory
+            'test': loads train/test dataset into memory
+            'inference': does not load any dataset into memory
         world_size: total number of machines available
         local_rank: rank of current machine
 
     Attributes:
         datamanager: The data manager that will be used
         model: The model that will be used
     """
 
     def __init__(
         self,
         config: VanillaPipelineConfig,
         device: str,
-        test_mode: bool = False,
+        test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
     ):
         super().__init__()
         self.config = config
+        self.test_mode = test_mode
         self.datamanager: VanillaDataManager = config.datamanager.setup(
             device=device, test_mode=test_mode, world_size=world_size, local_rank=local_rank
         )
         self.datamanager.to(device)
         # TODO(ethan): get rid of scene_bounds from the model
         assert self.datamanager.train_dataset is not None, "Missing input dataset"
 
         self._model = config.model.setup(
-            scene_box=self.datamanager.train_dataset.dataparser_outputs.scene_box,
+            scene_box=self.datamanager.train_dataset.scene_box,
             num_train_data=len(self.datamanager.train_dataset),
-            metadata=self.datamanager.train_dataset.dataparser_outputs.metadata,
+            metadata=self.datamanager.train_dataset.metadata,
         )
         self.model.to(device)
 
         self.world_size = world_size
         if world_size > 1:
             self._model = typing.cast(Model, DDP(self._model, device_ids=[local_rank], find_unused_parameters=True))
             dist.barrier(device_ids=[local_rank])
@@ -243,23 +274,24 @@
         Args:
             step: current iteration step to update sampler if using DDP (distributed)
         """
         ray_bundle, batch = self.datamanager.next_train(step)
         model_outputs = self.model(ray_bundle)
         metrics_dict = self.model.get_metrics_dict(model_outputs, batch)
 
-        camera_opt_param_group = self.config.datamanager.camera_optimizer.param_group
-        if camera_opt_param_group in self.datamanager.get_param_groups():
-            # Report the camera optimization metrics
-            metrics_dict["camera_opt_translation"] = (
-                self.datamanager.get_param_groups()[camera_opt_param_group][0].data[:, :3].norm()
-            )
-            metrics_dict["camera_opt_rotation"] = (
-                self.datamanager.get_param_groups()[camera_opt_param_group][0].data[:, 3:].norm()
-            )
+        if self.config.datamanager.camera_optimizer is not None:
+            camera_opt_param_group = self.config.datamanager.camera_optimizer.param_group
+            if camera_opt_param_group in self.datamanager.get_param_groups():
+                # Report the camera optimization metrics
+                metrics_dict["camera_opt_translation"] = (
+                    self.datamanager.get_param_groups()[camera_opt_param_group][0].data[:, :3].norm()
+                )
+                metrics_dict["camera_opt_rotation"] = (
+                    self.datamanager.get_param_groups()[camera_opt_param_group][0].data[:, 3:].norm()
+                )
 
         loss_dict = self.model.get_loss_dict(model_outputs, batch, metrics_dict)
 
         return model_outputs, loss_dict, metrics_dict
 
     def forward(self):
         """Blank forward method
@@ -326,36 +358,40 @@
                 inner_start = time()
                 height, width = camera_ray_bundle.shape
                 num_rays = height * width
                 outputs = self.model.get_outputs_for_camera_ray_bundle(camera_ray_bundle)
                 metrics_dict, _ = self.model.get_image_metrics_and_images(outputs, batch)
                 assert "num_rays_per_sec" not in metrics_dict
                 metrics_dict["num_rays_per_sec"] = num_rays / (time() - inner_start)
-                fps_str = f"fps_at_{height}x{width}"
+                fps_str = "fps"
                 assert fps_str not in metrics_dict
                 metrics_dict[fps_str] = metrics_dict["num_rays_per_sec"] / (height * width)
                 metrics_dict_list.append(metrics_dict)
                 progress.advance(task)
         # average the metrics list
         metrics_dict = {}
         for key in metrics_dict_list[0].keys():
             metrics_dict[key] = float(
                 torch.mean(torch.tensor([metrics_dict[key] for metrics_dict in metrics_dict_list]))
             )
         self.train()
         return metrics_dict
 
-    def load_pipeline(self, loaded_state: Dict[str, Any]) -> None:
+    def load_pipeline(self, loaded_state: Dict[str, Any], step: int) -> None:
         """Load the checkpoint from the given path
 
         Args:
             loaded_state: pre-trained model state dict
+            step: training step of the loaded checkpoint
         """
-        state = {key.replace("module.", ""): value for key, value in loaded_state.items()}
-        self.load_state_dict(state)  # type: ignore
+        state = {
+            (key[len("module.") :] if key.startswith("module.") else key): value for key, value in loaded_state.items()
+        }
+        self.model.update_to_step(step)
+        self.load_state_dict(state, strict=True)
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         """Returns the training callbacks from both the Dataloader and the Model."""
         datamanager_callbacks = self.datamanager.get_training_callbacks(training_callback_attributes)
         model_callbacks = self.model.get_training_callbacks(training_callback_attributes)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-0.2.0/nerfstudio/pipelines/dynamic_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 A pipeline that dynamically chooses the number of rays to sample.
 """
 
 from dataclasses import dataclass, field
 from typing import Type
 
 import torch
+from typing_extensions import Literal
 
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager
 from nerfstudio.pipelines.base_pipeline import VanillaPipeline, VanillaPipelineConfig
 
 
 @dataclass
 class DynamicBatchPipelineConfig(VanillaPipelineConfig):
@@ -45,30 +46,32 @@
     datamanager: VanillaDataManager
     dynamic_num_rays_per_batch: int
 
     def __init__(
         self,
         config: DynamicBatchPipelineConfig,
         device: str,
-        test_mode: bool = False,
+        test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
     ):
         super().__init__(config, device, test_mode, world_size, local_rank)
         assert isinstance(
             self.datamanager, VanillaDataManager
         ), "DynamicBatchPipeline only works with VanillaDataManager."
 
         self.dynamic_num_rays_per_batch = self.config.target_num_samples // self.config.max_num_samples_per_ray
         self._update_pixel_samplers()
 
     def _update_pixel_samplers(self):
         """Update the pixel samplers for train and eval with the dynamic number of rays per batch."""
-        self.datamanager.train_pixel_sampler.set_num_rays_per_batch(self.dynamic_num_rays_per_batch)
-        self.datamanager.eval_pixel_sampler.set_num_rays_per_batch(self.dynamic_num_rays_per_batch)
+        if self.datamanager.train_pixel_sampler is not None:
+            self.datamanager.train_pixel_sampler.set_num_rays_per_batch(self.dynamic_num_rays_per_batch)
+        if self.datamanager.eval_pixel_sampler is not None:
+            self.datamanager.eval_pixel_sampler.set_num_rays_per_batch(self.dynamic_num_rays_per_batch)
 
     def _update_dynamic_num_rays_per_batch(self, num_samples_per_batch: int):
         """Updates the dynamic number of rays per batch variable,
         based on the total number of samples in the last batch of rays."""
         self.dynamic_num_rays_per_batch = int(
             self.dynamic_num_rays_per_batch * (self.config.target_num_samples / num_samples_per_batch)
         )
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/__init__.py` & `nerfstudio-0.2.0/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/colormaps.py` & `nerfstudio-0.2.0/nerfstudio/utils/colormaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,20 @@
     """Convert single channel to a color image.
 
     Args:
         image: Single channel image.
         cmap: Colormap for image.
 
     Returns:
-        TensorType: Colored image
+        TensorType: Colored image with colors in [0, 1]
     """
 
     colormap = cm.get_cmap(cmap)
     colormap = torch.tensor(colormap.colors).to(image.device)  # type: ignore
+    image = torch.nan_to_num(image, 0)
     image_long = (image * 255).long()
     image_long_min = torch.min(image_long)
     image_long_max = torch.max(image_long)
     assert image_long_min >= 0, f"the min value is {image_long_min}"
     assert image_long_max <= 255, f"the max value is {image_long_max}"
     return colormap[image_long[..., 0]]
 
@@ -57,15 +58,15 @@
         depth: Depth image.
         accumulation: Ray accumulation used for masking vis.
         near_plane: Closest depth to consider. If None, use min image value.
         far_plane: Furthest depth to consider. If None, use max image value.
         cmap: Colormap to apply.
 
     Returns:
-        Colored depth image
+        Colored depth image with colors in [0, 1]
     """
 
     near_plane = near_plane or float(torch.min(depth))
     far_plane = far_plane or float(torch.max(depth))
 
     depth = (depth - near_plane) / (far_plane - near_plane + 1e-10)
     depth = torch.clip(depth, 0, 1)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/colors.py` & `nerfstudio-0.2.0/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/comms.py` & `nerfstudio-0.2.0/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/decorators.py` & `nerfstudio-0.2.0/nerfstudio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/eval_utils.py` & `nerfstudio-0.2.0/nerfstudio/utils/eval_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,28 +21,31 @@
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 import torch
 import yaml
 from rich.console import Console
+from typing_extensions import Literal
 
-from nerfstudio.configs import base_config as cfg
+from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.pipelines.base_pipeline import Pipeline
 
 CONSOLE = Console(width=120)
 
 
-def eval_load_checkpoint(config: cfg.TrainerConfig, pipeline: Pipeline) -> Path:
+def eval_load_checkpoint(config: TrainerConfig, pipeline: Pipeline) -> Tuple[Path, int]:
     ## TODO: ideally eventually want to get this to be the same as whatever is used to load train checkpoint too
     """Helper function to load checkpointed pipeline
 
     Args:
         config (DictConfig): Configuration of pipeline to load
         pipeline (Pipeline): Pipeline instance of which to load weights
+    Returns:
+        A tuple of the path to the loaded checkpoint and the step at which it was saved.
     """
     assert config.load_dir is not None
     if config.load_step is None:
         CONSOLE.print("Loading latest checkpoint from load_dir")
         # NOTE: this is specific to the checkpoint name format
         if not os.path.exists(config.load_dir):
             CONSOLE.rule("Error", style="red")
@@ -54,43 +57,53 @@
             sys.exit(1)
         load_step = sorted(int(x[x.find("-") + 1 : x.find(".")]) for x in os.listdir(config.load_dir))[-1]
     else:
         load_step = config.load_step
     load_path = config.load_dir / f"step-{load_step:09d}.ckpt"
     assert load_path.exists(), f"Checkpoint {load_path} does not exist"
     loaded_state = torch.load(load_path, map_location="cpu")
-    pipeline.load_pipeline(loaded_state["pipeline"])
+    pipeline.load_pipeline(loaded_state["pipeline"], loaded_state["step"])
     CONSOLE.print(f":white_check_mark: Done loading checkpoint from {load_path}")
-    return load_path
+    return load_path, load_step
 
 
-def eval_setup(config_path: Path, eval_num_rays_per_chunk: Optional[int] = None) -> Tuple[cfg.Config, Pipeline, Path]:
+def eval_setup(
+    config_path: Path,
+    eval_num_rays_per_chunk: Optional[int] = None,
+    test_mode: Literal["test", "val", "inference"] = "test",
+) -> Tuple[TrainerConfig, Pipeline, Path, int]:
     """Shared setup for loading a saved pipeline for evaluation.
 
     Args:
         config_path: Path to config YAML file.
+        eval_num_rays_per_chunk: Number of rays per forward pass
+        test_mode:
+            'val': loads train/val datasets into memory
+            'test': loads train/test dataset into memory
+            'inference': does not load any dataset into memory
+
 
     Returns:
-        Loaded config, pipeline module, and corresponding checkpoint.
+        Loaded config, pipeline module, corresponding checkpoint, and step
     """
     # load save config
     config = yaml.load(config_path.read_text(), Loader=yaml.Loader)
-    assert isinstance(config, cfg.Config)
+    assert isinstance(config, TrainerConfig)
 
     if eval_num_rays_per_chunk:
         config.pipeline.model.eval_num_rays_per_chunk = eval_num_rays_per_chunk
 
     # load checkpoints from wherever they were saved
     # TODO: expose the ability to choose an arbitrary checkpoint
-    config.trainer.load_dir = config.get_checkpoint_dir()
+    config.load_dir = config.get_checkpoint_dir()
     config.pipeline.datamanager.eval_image_indices = None
 
     # setup pipeline (which includes the DataManager)
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    pipeline = config.pipeline.setup(device=device, test_mode=True)
+    pipeline = config.pipeline.setup(device=device, test_mode=test_mode)
     assert isinstance(pipeline, Pipeline)
     pipeline.eval()
 
     # load checkpointed information
-    checkpoint_path = eval_load_checkpoint(config.trainer, pipeline)
+    checkpoint_path, step = eval_load_checkpoint(config, pipeline)
 
-    return config, pipeline, checkpoint_path
+    return config, pipeline, checkpoint_path, step
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/install_checks.py` & `nerfstudio-0.2.0/nerfstudio/utils/install_checks.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,18 +24,25 @@
 
 def check_ffmpeg_installed():
     """Checks if ffmpeg is installed."""
     ffmpeg_path = shutil.which("ffmpeg")
     if ffmpeg_path is None:
         CONSOLE.print("[bold red]Could not find ffmpeg. Please install ffmpeg.")
         print("See https://ffmpeg.org/download.html for installation instructions.")
-        print("ffmpeg is only necessary if using videos as input.")
         sys.exit(1)
 
 
 def check_colmap_installed():
     """Checks if colmap is installed."""
     colmap_path = shutil.which("colmap")
     if colmap_path is None:
         CONSOLE.print("[bold red]Could not find COLMAP. Please install COLMAP.")
         print("See https://colmap.github.io/install.html for installation instructions.")
         sys.exit(1)
+
+
+def check_curl_installed():
+    """Checks if curl is installed."""
+    curl_path = shutil.which("curl")
+    if curl_path is None:
+        CONSOLE.print("[bold red]Could not find [yellow]curl[red], Please install [yellow]curl")
+        sys.exit(1)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/io.py` & `nerfstudio-0.2.0/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/misc.py` & `nerfstudio-0.2.0/nerfstudio/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Miscellaneous helper code.
 """
 
+
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import torch
 
 
 def get_dict_to_torch(stuff: Any, device: Union[torch.device, str] = "cpu", exclude: Optional[List[str]] = None):
     """Set everything in the dict to the specified torch device.
@@ -143,7 +144,14 @@
         new_val (float): new value to update the average with
         step (int): current step number
 
     Returns:
         float: new updated average
     """
     return (step * prev_avg + new_val) / (step + 1)
+
+
+def strtobool(val) -> bool:
+    """Cheap replacement for `distutils.util.strtobool()` which is deprecated
+    FMI https://stackoverflow.com/a/715468
+    """
+    return val.lower() in ("yes", "y", "true", "t", "on", "1")
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/plotly_utils.py` & `nerfstudio-0.2.0/nerfstudio/utils/plotly_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             "opacity": opacity,
             "color": color,
         }
     )
 
 
 def get_cube(
-    side_length: float,
+    side_length: Union[float, torch.Tensor],
     center: TensorType[3] = None,
     color: str = "black",
     opacity: float = 1.0,
 ) -> go.Mesh3d:  # type: ignore
     """Returns a cube object for plotting with plotly.
 
     Args:
@@ -224,17 +224,25 @@
 
     x = np.array([-1.0, -1.0, 1.0, 1.0, -1.0, -1.0, 1.0, 1.0])
     y = np.array([-1.0, 1.0, 1.0, -1.0, -1.0, 1.0, 1.0, -1.0])
     z = np.array([-1.0, -1.0, -1.0, -1.0, 1.0, 1.0, 1.0, 1.0])
 
     pts = np.stack((x, y, z), axis=0)
 
-    pts *= side_length / 2.0
+    if isinstance(side_length, float):
+        pts *= side_length / 2.0
+    else:
+        pts[0] *= side_length[0].item() / 2.0
+        pts[1] *= side_length[1].item() / 2.0
+        pts[2] *= side_length[2].item() / 2.0
+
     if center is not None:
-        pts += center
+        pts[0] = np.add(pts[0], center[0])
+        pts[1] = np.add(pts[1], center[1])
+        pts[2] = np.add(pts[2], center[2])
 
     return go.Mesh3d(
         {
             "x": pts[0],
             "y": pts[1],
             "z": pts[2],
             "alphahull": 0,
@@ -254,15 +262,15 @@
     name: str = "ellipse",
 ) -> go.Mesh3d:  # type: ignore
     """Get a plotly ellipsoid for a Gaussian.
 
     Args:
         mean: mean of the Gaussian.
         cov: covariance of the Gaussian.
-        n_std: Standard devation to visualize. Defaults to 2 (95% confidence).
+        n_std: Standard deviation to visualize. Defaults to 2 (95% confidence).
         color: Color of the ellipsoid. Defaults to None.
         opacity: Opacity of the ellipsoid. Defaults to 0.5.
         resolution: Resolution of the ellipsoid. Defaults to 20.
         name: Name of the ellipsoid. Defaults to "ellipse".
 
     Returns:
         ellipsoid object.
@@ -425,15 +433,15 @@
     frustum: Frustums, opacity: float = 1.0, color: str = "forestgreen", size: float = 5
 ) -> go.Scatter3d:  # type: ignore
     """Get a set plotly points for frustums centers.
 
     Args:
         frustum: Frustums to visualize.
         opacity: Opacity of the points. Defaults to 0.3.
-        color: Color of the poinst. Defaults to "forestgreen".
+        color: Color of the points. Defaults to "forestgreen".
         size: Size of points. Defaults to 10.
 
     Returns:
         Plotly points
     """
 
     frustum = frustum.flatten()
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/poses.py` & `nerfstudio-0.2.0/nerfstudio/utils/poses.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 def multiply(pose_a: TensorType[..., 3, 4], pose_b: TensorType[..., 3, 4]) -> TensorType[..., 3, 4]:
     """Multiply two pose matrices, A @ B.
 
     Args:
         pose_a: Left pose matrix, usually a transformation applied to the right.
-        pose_b: Right pose matrix, usually a camera pose that will be tranformed by pose_a.
+        pose_b: Right pose matrix, usually a camera pose that will be transformed by pose_a.
 
     Returns:
         Camera pose matrix where pose_a was applied to pose_b.
     """
     R1, t1 = pose_a[..., :3, :3], pose_a[..., :3, 3:]
     R2, t2 = pose_b[..., :3, :3], pose_b[..., :3, 3:]
     R = R1.matmul(R2)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/printing.py` & `nerfstudio-0.2.0/nerfstudio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/profiler.py` & `nerfstudio-0.2.0/nerfstudio/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/rich_utils.py` & `nerfstudio-0.2.0/nerfstudio/utils/rich_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,59 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Additional rich ui components"""
 
-from rich.progress import ProgressColumn
+from contextlib import nullcontext
+from typing import Optional
+
+from rich.console import Console
+from rich.progress import (
+    BarColumn,
+    Progress,
+    ProgressColumn,
+    TaskProgressColumn,
+    TextColumn,
+    TimeRemainingColumn,
+)
 from rich.text import Text
 
+CONSOLE = Console(width=120)
+
 
 class ItersPerSecColumn(ProgressColumn):
     """Renders the iterations per second for a progress bar."""
 
     def __init__(self, suffix="it/s") -> None:
         super().__init__()
         self.suffix = suffix
 
     def render(self, task: "Task") -> Text:
         """Show data transfer speed."""
         speed = task.finished_speed or task.speed
         if speed is None:
             return Text("?", style="progress.data.speed")
         return Text(f"{speed:.2f} {self.suffix}", style="progress.data.speed")
+
+
+def status(msg: str, spinner: str = "bouncingBall", verbose: bool = False):
+    """A context manager that does nothing is verbose is True. Otherwise it hides logs under a message.
+
+    Args:
+        msg: The message to log.
+        spinner: The spinner to use.
+        verbose: If True, print all logs, else hide them.
+    """
+    if verbose:
+        return nullcontext()
+    return CONSOLE.status(msg, spinner=spinner)
+
+
+def get_progress(description: str, suffix: Optional[str] = None):
+    """Helper function to return a rich Progress object."""
+    progress_list = [TextColumn(description), BarColumn(), TaskProgressColumn(show_speed=True)]
+    progress_list += [ItersPerSecColumn(suffix=suffix)] if suffix else []
+    progress_list += [TimeRemainingColumn(elapsed_when_finished=True, compact=True)]
+    progress = Progress(*progress_list)
+    return progress
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-0.2.0/nerfstudio/utils/tensor_dataclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 class TensorDataclass:
     """@dataclass of tensors with the same size batch. Allows indexing and standard tensor ops.
     Fields that are not Tensors will not be batched unless they are also a TensorDataclass.
     Any fields that are dictionaries will have their Tensors or TensorDataclasses batched, and
     dictionaries will have their tensors or TensorDataclasses considered in the initial broadcast.
+    Tensor fields must have at least 1 dimension, meaning that you must convert a field like torch.Tensor(1)
+    to torch.Tensor([1])
 
     Example:
 
     .. code-block:: python
 
         @dataclass
         class TestTensorDataclass(TensorDataclass):
@@ -52,20 +54,32 @@
 
         test[..., 0].shape  # [2, 3]
         test[:, 0, :].shape  # [2, 4]
     """
 
     _shape: tuple
 
+    # A mapping from field-name (str): n (int)
+    # Any field OR any key in a dictionary field with this name (field-name) and a corresponding
+    # torch.Tensor will be assumed to have n dimensions after the batch dims. These n final dimensions
+    # will remain the same shape when doing reshapes, broadcasting, etc on the tensordataclass
+    _field_custom_dimensions: Dict[str, int] = {}
+
     def __post_init__(self) -> None:
         """Finishes setting up the TensorDataclass
 
         This will 1) find the broadcasted shape and 2) broadcast all fields to this shape 3)
         set _shape to be the broadcasted shape.
         """
+        if self._field_custom_dimensions is not None:
+            for k, v in self._field_custom_dimensions.items():
+                assert (
+                    isinstance(v, int) and v > 1
+                ), f"Custom dimensions must be an integer greater than 1, since 1 is the default, received {k}: {v}"
+
         if not dataclasses.is_dataclass(self):
             raise TypeError("TensorDataclass must be a dataclass")
 
         batch_shapes = self._get_dict_batch_shapes(
             {f.name: self.__getattribute__(f.name) for f in dataclasses.fields(self)}
         )
         if len(batch_shapes) == 0:
@@ -86,17 +100,21 @@
         Args:
             dict_: The dictionary to get the batch shapes of.
 
         Returns:
             The batch shapes of all tensors in the dictionary.
         """
         batch_shapes = []
-        for v in dict_.values():
+        for k, v in dict_.items():
             if isinstance(v, torch.Tensor):
-                batch_shapes.append(v.shape[:-1])
+                if isinstance(self._field_custom_dimensions, dict) and k in self._field_custom_dimensions:
+                    # pylint: disable=unsubscriptable-object
+                    batch_shapes.append(v.shape[: -self._field_custom_dimensions[k]])
+                else:
+                    batch_shapes.append(v.shape[:-1])
             elif isinstance(v, TensorDataclass):
                 batch_shapes.append(v.shape)
             elif isinstance(v, Dict):
                 batch_shapes.extend(self._get_dict_batch_shapes(v))
         return batch_shapes
 
     def _broadcast_dict_fields(self, dict_: Dict, batch_shape) -> Dict:
@@ -107,34 +125,52 @@
 
         Returns:
             The broadcasted dictionary.
         """
         new_dict = {}
         for k, v in dict_.items():
             if isinstance(v, torch.Tensor):
-                new_dict[k] = v.broadcast_to((*batch_shape, v.shape[-1]))
+                # If custom dimension key, then we need to
+                if isinstance(self._field_custom_dimensions, dict) and k in self._field_custom_dimensions:
+                    # pylint: disable=unsubscriptable-object
+                    new_dict[k] = v.broadcast_to(
+                        (
+                            *batch_shape,
+                            *v.shape[-self._field_custom_dimensions[k] :],
+                        )
+                    )
+                else:
+                    new_dict[k] = v.broadcast_to((*batch_shape, v.shape[-1]))
             elif isinstance(v, TensorDataclass):
                 new_dict[k] = v.broadcast_to(batch_shape)
             elif isinstance(v, Dict):
                 new_dict[k] = self._broadcast_dict_fields(v, batch_shape)
         return new_dict
 
     def __getitem__(self: TensorDataclassT, indices) -> TensorDataclassT:
-        if isinstance(indices, torch.Tensor):
+        if isinstance(indices, (torch.Tensor)):
             return self._apply_fn_to_fields(lambda x: x[indices])
-        if isinstance(indices, (int, slice)):
+        if isinstance(indices, (int, slice, type(Ellipsis))):
             indices = (indices,)
+        assert isinstance(indices, tuple)
         tensor_fn = lambda x: x[indices + (slice(None),)]
         dataclass_fn = lambda x: x[indices]
-        return self._apply_fn_to_fields(tensor_fn, dataclass_fn)
+
+        def custom_tensor_dims_fn(k, v):
+            custom_dims = self._field_custom_dimensions[k]  # pylint: disable=unsubscriptable-object
+            return v[indices + ((slice(None),) * custom_dims)]
+
+        return self._apply_fn_to_fields(tensor_fn, dataclass_fn, custom_tensor_dims_fn=custom_tensor_dims_fn)
 
     def __setitem__(self, indices, value) -> NoReturn:
         raise RuntimeError("Index assignment is not supported for TensorDataclass")
 
     def __len__(self) -> int:
+        if len(self._shape) == 0:
+            raise TypeError("len() of a 0-d tensor")
         return self.shape[0]
 
     def __bool__(self) -> bool:
         if len(self) == 0:
             raise ValueError(
                 f"The truth value of {self.__class__.__name__} when `len(x) == 0` "
                 "is ambiguous. Use `len(x)` or `x is not None`."
@@ -169,15 +205,20 @@
         Returns:
             A new TensorDataclass with the same data but with a new shape.
         """
         if isinstance(shape, int):
             shape = (shape,)
         tensor_fn = lambda x: x.reshape((*shape, x.shape[-1]))
         dataclass_fn = lambda x: x.reshape(shape)
-        return self._apply_fn_to_fields(tensor_fn, dataclass_fn)
+
+        def custom_tensor_dims_fn(k, v):
+            custom_dims = self._field_custom_dimensions[k]  # pylint: disable=unsubscriptable-object
+            return v.reshape((*shape, *v.shape[-custom_dims:]))
+
+        return self._apply_fn_to_fields(tensor_fn, dataclass_fn, custom_tensor_dims_fn=custom_tensor_dims_fn)
 
     def flatten(self: TensorDataclassT) -> TensorDataclassT:
         """Returns a new TensorDataclass with flattened batch dimensions
 
         Returns:
             TensorDataclass: A new TensorDataclass with the same data but with a new shape.
         """
@@ -191,29 +232,39 @@
 
         Args:
             shape: The new shape of the tensor dataclass.
 
         Returns:
             A new TensorDataclass with the same data but with a new shape.
         """
-        return self._apply_fn_to_fields(lambda x: x.broadcast_to((*shape, x.shape[-1])))
+
+        def custom_tensor_dims_fn(k, v):
+            custom_dims = self._field_custom_dimensions[k]  # pylint: disable=unsubscriptable-object
+            return v.broadcast_to((*shape, *v.shape[-custom_dims:]))
+
+        return self._apply_fn_to_fields(
+            lambda x: x.broadcast_to((*shape, x.shape[-1])), custom_tensor_dims_fn=custom_tensor_dims_fn
+        )
 
     def to(self: TensorDataclassT, device) -> TensorDataclassT:
         """Returns a new TensorDataclass with the same data but on the specified device.
 
         Args:
             device: The device to place the tensor dataclass.
 
         Returns:
             A new TensorDataclass with the same data but on the specified device.
         """
         return self._apply_fn_to_fields(lambda x: x.to(device))
 
     def _apply_fn_to_fields(
-        self: TensorDataclassT, fn: Callable, dataclass_fn: Optional[Callable] = None
+        self: TensorDataclassT,
+        fn: Callable,
+        dataclass_fn: Optional[Callable] = None,
+        custom_tensor_dims_fn: Optional[Callable] = None,
     ) -> TensorDataclassT:
         """Applies a function to all fields of the tensor dataclass.
 
         TODO: Someone needs to make a high level design choice for whether not not we want this
         to apply the function to any fields in arbitray superclasses. This is an edge case until we
         upgrade to python 3.10 and dataclasses can actually be subclassed with vanilla python and no
         janking, but if people try to jank some subclasses that are grandchildren of TensorDataclass
@@ -227,20 +278,29 @@
             dataclass_fn: The function to apply to TensorDataclass fields.
 
         Returns:
             A new TensorDataclass with the same data but with a new shape.
         """
 
         new_fields = self._apply_fn_to_dict(
-            {f.name: self.__getattribute__(f.name) for f in dataclasses.fields(self)}, fn, dataclass_fn
+            {f.name: self.__getattribute__(f.name) for f in dataclasses.fields(self)},
+            fn,
+            dataclass_fn,
+            custom_tensor_dims_fn,
         )
 
         return dataclasses.replace(self, **new_fields)
 
-    def _apply_fn_to_dict(self, dict_: Dict, fn: Callable, dataclass_fn: Optional[Callable] = None) -> Dict:
+    def _apply_fn_to_dict(
+        self,
+        dict_: Dict,
+        fn: Callable,
+        dataclass_fn: Optional[Callable] = None,
+        custom_tensor_dims_fn: Optional[Callable] = None,
+    ) -> Dict:
         """A helper function for _apply_fn_to_fields, applying a function to all fields of dict_
 
         Args:
             dict_: The dictionary to apply the function to.
             fn: The function to apply to tensor fields.
             dataclass_fn: The function to apply to TensorDataclass fields.
 
@@ -250,14 +310,22 @@
         field_names = dict_.keys()
         new_dict = {}
         for f in field_names:
             v = dict_[f]
             if v is not None:
                 if isinstance(v, TensorDataclass) and dataclass_fn is not None:
                     new_dict[f] = dataclass_fn(v)
+                # This is the case when we have a custom dimensions tensor
+                elif (
+                    isinstance(v, torch.Tensor)
+                    and isinstance(self._field_custom_dimensions, dict)
+                    and f in self._field_custom_dimensions
+                    and custom_tensor_dims_fn is not None
+                ):
+                    new_dict[f] = custom_tensor_dims_fn(f, v)
                 elif isinstance(v, (torch.Tensor, TensorDataclass)):
                     new_dict[f] = fn(v)
                 elif isinstance(v, Dict):
                     new_dict[f] = self._apply_fn_to_dict(v, fn, dataclass_fn)
                 else:
                     new_dict[f] = deepcopy(v)
```

### Comparing `nerfstudio-0.1.9/nerfstudio/utils/writer.py` & `nerfstudio-0.2.0/nerfstudio/utils/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 Generic Writer class
 """
 from __future__ import annotations
 
 import enum
+import os
 from abc import abstractmethod
 from pathlib import Path
 from time import time
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 import wandb
@@ -42,15 +43,14 @@
 
 class EventName(enum.Enum):
     """Names of possible events that can be logged via Local Writer for convenience.
     see config/logging/default_logging.yaml"""
 
     ITER_TRAIN_TIME = "Train Iter (time)"
     TOTAL_TRAIN_TIME = "Train Total (time)"
-    ITER_VIS_TIME = "Viewer Rendering (time)"
     ETA = "ETA (time)"
     TRAIN_RAYS_PER_SEC = "Train Rays / Sec"
     TEST_RAYS_PER_SEC = "Test Rays / Sec"
     VIS_RAYS_PER_SEC = "Vis Rays / Sec"
     CURR_TEST_PSNR = "Test PSNR"
 
 
@@ -184,36 +184,36 @@
     GLOBAL_BUFFER["max_iter"] = max_iter
     GLOBAL_BUFFER["max_buffer_size"] = config.max_buffer_size
     GLOBAL_BUFFER["steps_per_log"] = config.steps_per_log
     GLOBAL_BUFFER["events"] = {}
 
 
 @check_main_thread
-def setup_event_writer(config: cfg.Config, log_dir: Path) -> None:
+def setup_event_writer(is_wandb_enabled: bool, is_tensorboard_enabled: bool, log_dir: Path) -> None:
     """Initialization of all event writers specified in config
 
     Args:
         config: configuration to instantiate loggers
         max_iter: maximum number of train iterations
         banner_messages: list of messages to always display at bottom of screen
     """
     using_event_writer = False
-    if config.is_wandb_enabled():
+    if is_wandb_enabled:
         curr_writer = WandbWriter(log_dir=log_dir)
         EVENT_WRITERS.append(curr_writer)
         using_event_writer = True
-    if config.is_tensorboard_enabled():
+    if is_tensorboard_enabled:
         curr_writer = TensorboardWriter(log_dir=log_dir)
         EVENT_WRITERS.append(curr_writer)
         using_event_writer = True
     if using_event_writer:
         string = f"logging events to: {log_dir}"
     else:
-        string = "disabled tensorboard/wandb event writers"
-    CONSOLE.print(f"[bold red]{string}")
+        string = "Disabled tensorboard/wandb event writers"
+    CONSOLE.print(f"[bold yellow]{string}")
 
 
 class Writer:
     """Writer class"""
 
     @abstractmethod
     def write_image(self, name: str, image: TensorType["H", "W", "C"], step: int) -> None:
@@ -279,15 +279,20 @@
 
 
 @decorate_all([check_main_thread])
 class WandbWriter(Writer):
     """WandDB Writer Class"""
 
     def __init__(self, log_dir: Path):
-        wandb.init(project="nerfstudio-project", dir=str(log_dir), reinit=True)
+        wandb.init(
+            project=os.environ.get("WANDB_PROJECT", "nerfstudio-project"),
+            dir=os.environ.get("WANDB_DIR", str(log_dir)),
+            name=os.environ.get("WANDB_NAME", log_dir.name),
+            reinit=True,
+        )
 
     def write_image(self, name: str, image: TensorType["H", "W", "C"], step: int) -> None:
         image = torch.permute(image, (2, 0, 1))
         wandb.log({name: wandb.Image(image)}, step=step)
 
     def write_scalar(self, name: str, scalar: Union[float, torch.Tensor], step: int) -> None:
         wandb.log({name: scalar}, step=step)
@@ -357,15 +362,15 @@
 
 @decorate_all([check_main_thread])
 class LocalWriter:
     """Local Writer Class
     TODO: migrate to prettyprint
 
     Args:
-        config: configuration to instatiate class
+        config: configuration to instantiate class
         banner_messages: list of messages to always display at bottom of screen
     """
 
     def __init__(self, config: cfg.LocalWriterConfig, banner_messages: Optional[List[str]] = None):
         self.config = config
         self.stats_to_track = [name.value for name in config.stats_to_track]
         self.keys = set()
@@ -378,20 +383,20 @@
 
     def write_stats_log(self, step: int) -> None:
         """Function to write out scalars to terminal
 
         Args:
             step: current train step
         """
-        valid_step = step > 0 and step % GLOBAL_BUFFER["steps_per_log"] == 0
+        valid_step = step % GLOBAL_BUFFER["steps_per_log"] == 0
         if valid_step:
             if not self.has_printed and self.config.max_log_size:
                 CONSOLE.log(
                     f"Printing max of {self.config.max_log_size} lines. "
-                    "Set flag  `--logging.local-writer.max-log-size=0` "
+                    "Set flag [yellow]--logging.local-writer.max-log-size=0[/yellow] "
                     "to disable line wrapping."
                 )
             latest_map, new_key = self._consolidate_events()
             self._update_header(latest_map, new_key)
             self._print_stats(latest_map)
 
     def write_config(self, name: str, config_dict: Dict[str, Any], step: int):
@@ -426,18 +431,16 @@
             mssg = f"{'Step (% Done)':<20}"
             for name, _ in latest_map.items():
                 if name in self.stats_to_track:
                     mssg += f"{name:<20} "
             self.past_mssgs[0] = mssg
             self.past_mssgs[1] = "-" * len(mssg)
             if full_log_cond or not self.has_printed:
-                print("testeing testing!")
                 print(mssg)
                 print("-" * len(mssg))
-                # self.has_printed = True
 
     def _print_stats(self, latest_map, padding=" "):
         """helper to print out the stats in a readable format
 
         Args:
             latest_map: the most recent dictionary of stats that have been recorded
             padding: type of characters to print to pad open space
```

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/__init__.py` & `nerfstudio-0.2.0/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/app/package.json` & `nerfstudio-0.2.0/nerfstudio/viewer/app/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9597665847665847%*

 * *Differences: {"'dependencies'": "{'await-lock': '^2.2.2', 'lodash': '^4.17.21', 'msgpackr': '^1.8.5'}",*

 * * "'devDependencies'": "{'typescript': '^5.0.3'}",*

 * * "'version'": "'23-04-10-0'"}*

```diff
@@ -20,23 +20,26 @@
         "@mui/material": "^5.10.3",
         "@mui/system": "^5.10.6",
         "@mui/x-date-pickers": "^5.0.0",
         "@reduxjs/toolkit": "^1.8.3",
         "@testing-library/jest-dom": "^5.16.4",
         "@testing-library/react": "^13.3.0",
         "@testing-library/user-event": "^14.2.0",
+        "await-lock": "^2.2.2",
         "camera-controls": "^1.37.2",
         "classnames": "^2.3.1",
         "dat.gui": "^0.7.9",
         "dayjs": "^1.11.5",
         "eslint-config-prettier": "^8.5.0",
         "eslint-plugin-unused-imports": "^2.0.0",
         "leva": "^0.9.29",
+        "lodash": "^4.17.21",
         "meshline": "^2.0.4",
         "msgpack-lite": "^0.1.26",
+        "msgpackr": "^1.8.5",
         "prop-types": "^15.8.1",
         "re-resizable": "^6.9.9",
         "react": "^18.1.0",
         "react-dom": "^18.1.0",
         "react-icons": "^4.4.0",
         "react-pro-sidebar": "^0.7.1",
         "react-redux": "^8.0.2",
@@ -55,15 +58,15 @@
         "eslint-config-airbnb": "19.0.4",
         "eslint-plugin-import": "^2.25.3",
         "eslint-plugin-jsx-a11y": "^6.5.1",
         "eslint-plugin-react": "^7.28.0",
         "eslint-plugin-react-hooks": "^4.3.0",
         "prettier": "2.7.1",
         "react-scripts": "^5.0.1",
-        "typescript": "^4.7.3",
+        "typescript": "^5.0.3",
         "wait-on": "^6.0.1"
     },
     "eslintConfig": {
         "extends": "react-app"
     },
     "homepage": ".",
     "license": "ISC",
@@ -78,9 +81,9 @@
         "eject": "react-scripts eject",
         "electron": "electron .",
         "lint": "eslint --ext .js,.jsx .",
         "lint:fix": "eslint --fix --ext .js,.jsx .",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "22-11-10-0"
+    "version": "23-04-10-0"
 }
```

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/app/run_deploy.py` & `nerfstudio-0.2.0/nerfstudio/viewer/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/app/src/themes/leva_theme.json` & `nerfstudio-0.2.0/nerfstudio/viewer/app/src/themes/leva_theme.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967532467532468%*

 * *Differences: {"'colors'": "{'highlight3': '#EEEEEE'}"}*

```diff
@@ -13,15 +13,15 @@
         "accent3": "#ffd65c",
         "disabled": "#595959",
         "elevation1": "#292d39",
         "elevation2": "#222831",
         "elevation3": "#393E46",
         "highlight1": "#d1d4db",
         "highlight2": "#EEEEEE",
-        "highlight3": "#222831",
+        "highlight3": "#EEEEEE",
         "vivid1": "#ffcc00"
     },
     "fontSizes": {
         "root": "11px"
     },
     "fontWeights": {
         "button": "normal",
```

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/server/__init__.py` & `nerfstudio-0.2.0/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/server/path.py` & `nerfstudio-0.2.0/nerfstudio/viewer/server/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     __slots__ = ["entries"]
 
     def __init__(self, entries: Tuple = tuple()):
         self.entries = entries
 
     def append(self, other: str) -> "Path":
-        """Methodthat appends a new component and returns new Path
+        """Method that appends a new component and returns new Path
 
         Args:
             other: _description_
         """
         new_path = self.entries
         for element in other.split("/"):
             if len(element) == 0:
```

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/server/state/node.py` & `nerfstudio-0.2.0/nerfstudio/viewer/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/server/state/state_node.py` & `nerfstudio-0.2.0/nerfstudio/viewer/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/nerfstudio/viewer/server/utils.py` & `nerfstudio-0.2.0/nerfstudio/viewer/server/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Generic utility functions
 """
 
-import sys
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple
 
 import numpy as np
 import torch
-import zmq
-from aiortc import RTCPeerConnection
-from aiortc.rtcrtpsender import RTCRtpSender
+
+from nerfstudio.viewer.viser.messages import CameraMessage
 
 
 def get_chunks(
     lst: List[float], num_chunks: Optional[int] = None, size_of_chunk: Optional[int] = None
 ) -> List[List[float]]:
-    """Returns list of n elements, constaining a sublist.
+    """Returns list of n elements, containing a sublist.
 
     Args:
         lst: List to be chunked up
         num_chunks: number of chunks to split list into
         size_of_chunk: size of each chunk
     """
     if num_chunks:
@@ -50,39 +48,54 @@
 def three_js_perspective_camera_focal_length(fov: float, image_height: int):
     """Returns the focal length of a three.js perspective camera.
 
     Args:
         fov: the field of view of the camera in degrees.
         image_height: the height of the image in pixels.
     """
+    if fov is None:
+        print("Warning: fov is None, using default value")
+        return 50
     pp_h = image_height / 2.0
     focal_length = pp_h / np.tan(fov * (np.pi / 180.0) / 2.0)
     return focal_length
 
 
 def get_intrinsics_matrix_and_camera_to_world_h(
-    camera_object: Dict[str, Any], image_height: int
+    camera_message: CameraMessage, image_height: int, image_width: Optional[int] = None
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     """Returns the camera intrinsics matrix and the camera to world homogeneous matrix.
 
     Args:
         camera_object: a Camera object.
         image_size: the size of the image (height, width)
     """
     # intrinsics
-    fov = camera_object["fov"]
-    aspect = camera_object["aspect"]
-    image_width = aspect * image_height
+    fov = camera_message.fov
+    aspect = camera_message.aspect
+    if image_width is None:
+        image_width = aspect * image_height
     pp_w = image_width / 2.0
     pp_h = image_height / 2.0
-    focal_length = three_js_perspective_camera_focal_length(fov, image_height)
-    intrinsics_matrix = torch.tensor([[focal_length, 0, pp_w], [0, focal_length, pp_h], [0, 0, 1]]).float()
+    if (camera_message.camera_type == "perspective") | (camera_message.camera_type == "fisheye"):
+        focal_length = three_js_perspective_camera_focal_length(fov, image_height)
+        intrinsics_matrix = torch.tensor([[focal_length, 0, pp_w], [0, focal_length, pp_h], [0, 0, 1]]).float()
+    elif camera_message.camera_type == "equirectangular":
+        render_aspect = camera_message.render_aspect
+        if aspect < render_aspect:
+            intrinsics_matrix = torch.tensor(
+                [[pp_w, 0, pp_w], [0, image_width / render_aspect, pp_h], [0, 0, 1]]
+            ).float()
+        else:
+            intrinsics_matrix = torch.tensor(
+                [[image_height * render_aspect / 2, 0, pp_w], [0, pp_h * 2, pp_h], [0, 0, 1]]
+            ).float()
 
     # extrinsics
-    camera_to_world_h = torch.tensor(get_chunks(camera_object["matrix"], size_of_chunk=4)).T.float()
+    camera_to_world_h = torch.tensor(get_chunks(camera_message.matrix, size_of_chunk=4)).T.float()
     camera_to_world_h = torch.stack(
         [
             camera_to_world_h[0, :],
             camera_to_world_h[2, :],
             camera_to_world_h[1, :],
             camera_to_world_h[3, :],
         ],
@@ -100,29 +113,13 @@
         default_port: the default port
         max_attempts: max number of attempts to try connection. Defaults to MAX_ATTEMPTS.
     """
     for i in range(max_attempts):
         port = default_port + i
         try:
             return func(port, **kwargs), port
-        except (OSError, zmq.error.ZMQError):
-            print(f"Port: {port:d} in use, trying another...", file=sys.stderr)
         except Exception as e:
             print(type(e))
             raise
     raise (
         Exception(f"Could not find an available port in the range: [{default_port:d}, {max_attempts + default_port:d})")
     )
-
-
-def force_codec(pc: RTCPeerConnection, sender: RTCRtpSender, forced_codec: str) -> None:
-    """Sets the codec preferences on a connection between sender and reciever
-
-    Args:
-        pc: peer connection point
-        sender: sender that will send to connection point
-        forced_codec: codec to set
-    """
-    kind = forced_codec.split("/")[0]
-    codecs = RTCRtpSender.getCapabilities(kind).codecs
-    transceiver = next(t for t in pc.getTransceivers() if t.sender == sender)
-    transceiver.setCodecPreferences([codec for codec in codecs if codec.mimeType == forced_codec])
```

### Comparing `nerfstudio-0.1.9/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nerfstudio
-Version: 0.1.9
-Summary: All-in-one repository for state-of-the-art NeRFs
-License: Apache 2.0
-Project-URL: Documentation, https://docs.nerf.studio
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 <p align="center">
     <!-- community badges -->
     <a href="https://discord.gg/uMbNqcraFc"><img src="https://img.shields.io/badge/Join-Discord-blue.svg"/></a>
     <!-- doc badges -->
     <a href='https://plenoptix-nerfstudio.readthedocs-hosted.com/en/latest/?badge=latest'>
         <img src='https://readthedocs.com/projects/plenoptix-nerfstudio/badge/?version=latest' alt='Documentation Status' />
     </a>
@@ -83,122 +69,165 @@
 The quickstart will help you get started with the default vanilla NeRF trained on the classic Blender Lego scene.
 For more complex changes (e.g., running with your own data/setting up a new NeRF graph, please refer to our [references](#learn-more).
 
 ## 1. Installation: Setup the environment
 
 ### Prerequisites
 
-CUDA must be installed on the system. This library has been tested with version 11.3. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
+You must have an NVIDIA video card with CUDA installed on the system. This library has been tested with version 11.3 of CUDA. You can find more information about installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/index.html)
 
 ### Create environment
 
 Nerfstudio requires `python >= 3.7`. We recommend using conda to manage dependencies. Make sure to install [Conda](https://docs.conda.io/en/latest/miniconda.html) before proceeding.
 
 ```bash
 conda create --name nerfstudio -y python=3.8
 conda activate nerfstudio
 python -m pip install --upgrade pip
 ```
 
 ### Dependencies
 
-Install pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+Install pytorch with CUDA (this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn](https://github.com/NVlabs/tiny-cuda-nn)
+
+For CUDA 11.3:
 
 ```bash
 pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/whl/torch_stable.html
-pip install git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
+```
+
+For CUDA 11.7:
+
+```bash
+pip install torch==1.13.1 torchvision functorch --extra-index-url https://download.pytorch.org/whl/cu117
+pip install ninja git+https://github.com/NVlabs/tiny-cuda-nn/#subdirectory=bindings/torch
 ```
 
+See [Dependencies](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md#dependencies)
+in the Installation documentation for more.
+
 ### Installing nerfstudio
 
 Easy option:
 
 ```bash
 pip install nerfstudio
 ```
 
-If you want the latest and greatest:
+**OR** if you want the latest and greatest:
 
 ```bash
 git clone https://github.com/nerfstudio-project/nerfstudio.git
 cd nerfstudio
 pip install --upgrade pip setuptools
 pip install -e .
 ```
 
-## 2. Setting up the data
+**OR** if you want to skip all installation steps and directly start using nerfstudio, use the docker image:
+
+See [Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/installation.md) - **Use docker image**.
 
-Download the original NeRF Blender dataset. We support the major datasets and allow users to create their own dataset, described in detail [here](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html).
+## 2. Training your first model!
+
+The following will train a _nerfacto_ model, our recommended model for real world scenes.
 
 ```bash
-ns-download-data --dataset=blender
-ns-download-data --dataset=nerfstudio --capture=poster
+# Download some test data:
+ns-download-data nerfstudio --capture-name=poster
+# Train model
+ns-train nerfacto --data data/nerfstudio/poster
 ```
 
-### 2.x Using custom data
+If everything works, you should see training progress like the following:
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766069-cadfd34f-8833-4156-88b7-ad406d688fc0.png">
+</p>
+
+Navigating to the link at the end of the terminal will load the webviewer. If you are running on a remote machine, you will need to port forward the websocket port (defaults to 7007).
+
+<p align="center">
+    <img width="800" alt="image" src="https://user-images.githubusercontent.com/3310961/202766653-586a0daa-466b-4140-a136-6b02f2ce2c54.png">
+</p>
 
-If you have custom data in the form of a video or folder of images, we've provided some [COLMAP](https://colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to help you process your data so it is compatible with nerfstudio.
+### Resume from checkpoint / visualize existing run
 
-After installing both software, you can process your data via:
+It is possible to load a pretrained model by running
 
 ```bash
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir {PROCESSED_DATA_DIR}
-# Or if you're on a system without an attached display (i.e. colab):
-ns-process-data {video,images,insta360,record3d} --data {DATA_PATH}  --output-dir {PROCESSED_DATA_DIR} --no-gpu
+ns-train nerfacto --data data/nerfstudio/poster --load-dir {outputs/.../nerfstudio_models}
 ```
 
-## 3. Training a model
+This will automatically start training. If you do not want it to train, add `--viewer.start-train False` to your training command.
 
-To run with all the defaults, e.g., vanilla NeRF method with the Blender Lego image
+## 3. Exporting Results
 
-```bash
-# To see what models are available.
-ns-train --help
+Once you have a NeRF model you can either render out a video or export a point cloud.
 
-# To see what model-specific cli arguments are available.
-ns-train nerfacto --help
+### Render Video
 
-# Run with nerfacto model.
-ns-train nerfacto
+First we must create a path for the camera to follow. This can be done in the viewer under the "RENDER" tab. Orient your 3D view to the location where you wish the video to start, then press "ADD CAMERA". This will set the first camera key frame. Continue to new viewpoints adding additional cameras to create the camera path. We provide other parameters to further refine your camera path. Once satisfied, press "RENDER" which will display a modal that contains the command needed to render the video. Kill the training job (or create a new terminal if you have lots of compute) and run the command to generate the video.
 
-# We provide support for other models. E.g., to run instant-ngp.
-ns-train instant-ngp
+Other video export options are available, learn more by running
 
-# To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR}
+```bash
+ns-render --help
 ```
 
-### 3.x Training a model with the viewer
+### Generate Point Cloud
 
-You can visualize training in real-time using our web-based viewer.
+While NeRF models are not designed to generate point clouds, it is still possible. Navigate to the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option is selected, everything in the yellow square will be exported into a point cloud. Modify the settings as desired then run the command at the bottom of the panel in your command line.
 
-Make sure to forward a port for the websocket to localhost. The default port is 7007, which you should expose to localhost:7007.
+Alternatively you can use the CLI without the viewer. Learn about the export options by running
 
 ```bash
-# with the default port
-ns-train nerfacto --vis viewer
+ns-export pointcloud --help
+```
+
+## 4. Using Custom Data
+
+Using an existing dataset is great, but likely you want to use your own data! We support various methods for using your own data. Before it can be used in nerfstudio, the camera location and orientations must be determined and then converted into our format using `ns-process-data`. We rely on external tools for this, instructions and information can be found in the documentation.
+
+| Data                                                                                                 | Capture Device | Requirements                                                      | `ns-process-data` Speed |
+| ---------------------------------------------------------------------------------------------------- | -------------- | ----------------------------------------------------------------- | ----------------------- |
+| 📷 [Images](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)      | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📹 [Video](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video)       | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 🌎 [360 Data](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#360_data)            | Any            | [COLMAP](https://colmap.github.io/install.html)                   | 🐢                      |
+| 📱 [Polycam](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#polycam-capture)      | IOS with LiDAR | [Polycam App](https://poly.cam/)                                  | 🐇                      |
+| 📱 [KIRI Engine](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#kiri-capture)     | IOS or Android | [KIRI Engine App](https://www.kiriengine.com/)                    | 🐇                      |
+| 📱 [Record3D](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture)    | IOS with LiDAR | [Record3D app](https://record3d.app/)                             | 🐇                      |
+| 🖥 [Metashape](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#metashape)           | Any            | [Metashape](https://www.agisoft.com/)                             | 🐇                      |
+| 🖥 [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html#realitycapture) | Any            | [RealityCapture](https://www.capturingreality.com/realitycapture) | 🐇                      |
+| 🛠 [Custom](https://docs.nerf.studio/en/latest/quickstart/data_conventions.html)                      | Any            | Camera Poses                                                      | 🐇                      |
 
-# with a specified websocket port
-ns-train nerfacto --vis viewer --viewer.websocket-port=7008
+## 5. Advanced Options
 
-# port forward if running on remote
-ssh -L localhost:7008:localhost:7008 {REMOTE HOST}
+### Training models other than nerfacto
+
+We provide other models than nerfacto, for example if you want to train the original nerf model, use the following command
+
+```bash
+ns-train vanilla-nerf --data DATA_PATH
 ```
 
-For more details on how to interact with the visualizer, please visit our viewer [walk-through](https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html).
+For a full list of included models run `ns-train --help`.
 
-## 4. Rendering a trajectory during inference
+### Modify Configuration
 
-After your model has trained, you can headlessly render out a video of the scene with a pre-defined trajectory.
+Each model contains many parameters that can be changed, too many to list here. Use the `--help` command to see the full list of configuration options.
 
 ```bash
-# assuming previously ran `ns-train nerfacto`
-ns-render --load-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --traj=spiral --output-path=renders/output.mp4
+ns-train nerfacto --help
 ```
 
+### Tensorboard / WandB
+
+We support three different methods to track training progress, using the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights and Biases](https://wandb.ai/site). You can specify which visualizer to use by appending `--vis {viewer, tensorboard, wandb}` to the training command. Note that only one may be used at a time. Additionally the viewer only works for methods that are fast (ie. nerfacto, instant-ngp), for slower methods like NeRF, use the other loggers.
+
 # Learn More
 
 And that's it for getting started with the basics of nerfstudio.
 
 If you're interested in learning more on how to create your own pipelines, develop with the viewer, run benchmarks, and more, please check out some of the quicklinks below or visit our [documentation](https://docs.nerf.studio/en/latest/) directly.
 
 | Section                                                                                            | Description                                                                                        |
@@ -215,30 +244,29 @@
 | 💻 **For Developers**                                                                              |
 | [Creating pipelines](https://docs.nerf.studio/en/latest/developer_guides/pipelines/index.html)     | Learn how to easily build new neural rendering pipelines by using and/or implementing new modules. |
 | [Creating datasets](https://docs.nerf.studio/en/latest/quickstart/custom_dataset.html)             | Have a new dataset? Learn how to run it with nerfstudio.                                           |
 | [Contributing](https://docs.nerf.studio/en/latest/reference/contributing.html)                     | Walk-through for how you can start contributing now.                                               |
 | 💖 **Community**                                                                                   |
 | [Discord](https://discord.gg/uMbNqcraFc)                                                           | Join our community to discuss more. We would love to hear from you!                                |
 | [Twitter](https://twitter.com/nerfstudioteam)                                                      | Follow us on Twitter @nerfstudioteam to see cool updates and announcements                         |
-| [TikTok](#)                                                                                        | Coming soon! Follow us on TikTok to see some of our fan favorite results                           |
 
 # Supported Features
 
-We provide the following support structures to make life easier for getting started with NeRFs. For a full description, please refer to our [features page](#).
+We provide the following support structures to make life easier for getting started with NeRFs.
 
 **If you are looking for a feature that is not currently supported, please do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/uMbNqcraFc)!**
 
 - :mag_right: Web-based visualizer that allows you to:
   - Visualize training in real-time + interact with the scene
   - Create and render out scenes with custom camera trajectories
   - View different output types
   - And more!
 - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb), code profiling, and other built-in debugging tools
 - :chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender dataset
-- :iphone: Full pipeline support (w/ Colmap or Record3D) for going from a video on your phone to a full 3D render.
+- :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for going from a video on your phone to a full 3D render.
 
 # Built On
 
 <a href="https://github.com/brentyi/tyro">
     <img alt="tyro logo" src="https://brentyi.github.io/tyro/_static/logo-light.svg" width="150px" />
 </a>
 
@@ -250,24 +278,26 @@
 </a>
 
 - Library for accelerating NeRF renders
 - Developed by [Ruilong Li](https://www.liruilong.cn/)
 
 # Citation
 
+You can find a paper writeup of the framework on [arXiv](https://arxiv.org/abs/2302.04264).
+
 If you use this library or find the documentation useful for your research, please consider citing:
 
 ```
-@misc{nerfstudio,
-      title={Nerfstudio: A Framework for Neural Radiance Field Development},
-      author={Matthew Tancik*, Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi,
-              Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi,
-              Abhik Ahuja, David McAllister, Angjoo Kanazawa},
-      year={2022},
-      url={https://github.com/nerfstudio-project/nerfstudio},
+@article{nerfstudio,
+    author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne and Li, Ruilong and Yi,
+            Brent and Kerr, Justin and Wang, Terrance and Kristoffersen, Alexander and Austin,
+            Jake and Salahi, Kamyar and Ahuja, Abhik and McAllister, David and Kanazawa, Angjoo},
+    title = {Nerfstudio: A Modular Framework for Neural Radiance Field Development},
+    journal = {arXiv preprint arXiv:2302.04264},
+    year = {2023},
 }
 ```
 
 # Contributors
 
 <a href="https://github.com/nerfstudio-project/nerfstudio/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=nerfstudio-project/nerfstudio" />
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 0.1.9 Summary: All-in-one
-repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
-Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
-Alpha Classifier: Programming Language :: Python Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-docs License-File: LICENSE
  [https://img.shields.io/badge/Join-Discord-blue.svg]  [Documentation_Status]
         [PyPI_version]  [Test_Status] [Viewer_build_Status]  [License]
                                  [nerfstudio]
 
                    A collaboration friendly studio for NeRFs
                        [documentation] [viewer] [colab]
 [https://user-images.githubusercontent.com/3310961/194017985-ade69503-9d68-
@@ -31,71 +25,124 @@
 contributing.html)!** Please do not hesitate to reach out to the nerfstudio
 team with any questions via [Discord](https://discord.gg/uMbNqcraFc). We hope
 nerfstudio enables you to build faster :hammer: learn together :books: and
 contribute to our NeRF community :sparkling_heart:. # Quickstart The quickstart
 will help you get started with the default vanilla NeRF trained on the classic
 Blender Lego scene. For more complex changes (e.g., running with your own data/
 setting up a new NeRF graph, please refer to our [references](#learn-more). ##
-1. Installation: Setup the environment ### Prerequisites CUDA must be installed
-on the system. This library has been tested with version 11.3. You can find
-more information about installing CUDA [here](https://docs.nvidia.com/cuda/
-cuda-quick-start-guide/index.html) ### Create environment Nerfstudio requires
-`python >= 3.7`. We recommend using conda to manage dependencies. Make sure to
-install [Conda](https://docs.conda.io/en/latest/miniconda.html) before
-proceeding. ```bash conda create --name nerfstudio -y python=3.8 conda activate
-nerfstudio python -m pip install --upgrade pip ``` ### Dependencies Install
-pytorch with CUDA (this repo has been tested with CUDA 11.3) and [tiny-cuda-nn]
-(https://github.com/NVlabs/tiny-cuda-nn) ```bash pip install
+1. Installation: Setup the environment ### Prerequisites You must have an
+NVIDIA video card with CUDA installed on the system. This library has been
+tested with version 11.3 of CUDA. You can find more information about
+installing CUDA [here](https://docs.nvidia.com/cuda/cuda-quick-start-guide/
+index.html) ### Create environment Nerfstudio requires `python >= 3.7`. We
+recommend using conda to manage dependencies. Make sure to install [Conda]
+(https://docs.conda.io/en/latest/miniconda.html) before proceeding. ```bash
+conda create --name nerfstudio -y python=3.8 conda activate nerfstudio python -
+m pip install --upgrade pip ``` ### Dependencies Install pytorch with CUDA
+(this repo has been tested with CUDA 11.3 and CUDA 11.7) and [tiny-cuda-nn]
+(https://github.com/NVlabs/tiny-cuda-nn) For CUDA 11.3: ```bash pip install
 torch==1.12.1+cu113 torchvision==0.13.1+cu113 -f https://download.pytorch.org/
-whl/torch_stable.html pip install git+https://github.com/NVlabs/tiny-cuda-nn/
-#subdirectory=bindings/torch ``` ### Installing nerfstudio Easy option: ```bash
-pip install nerfstudio ``` If you want the latest and greatest: ```bash git
-clone https://github.com/nerfstudio-project/nerfstudio.git cd nerfstudio pip
-install --upgrade pip setuptools pip install -e . ``` ## 2. Setting up the data
-Download the original NeRF Blender dataset. We support the major datasets and
-allow users to create their own dataset, described in detail [here](https://
-docs.nerf.studio/en/latest/quickstart/custom_dataset.html). ```bash ns-
-download-data --dataset=blender ns-download-data --dataset=nerfstudio --
-capture=poster ``` ### 2.x Using custom data If you have custom data in the
-form of a video or folder of images, we've provided some [COLMAP](https://
-colmap.github.io/) and [FFmpeg](https://ffmpeg.org/download.html) scripts to
-help you process your data so it is compatible with nerfstudio. After
-installing both software, you can process your data via: ```bash ns-process-
-data {video,images,insta360,record3d} --data {DATA_PATH} --output-dir
-{PROCESSED_DATA_DIR} # Or if you're on a system without an attached display
-(i.e. colab): ns-process-data {video,images,insta360,record3d} --data
-{DATA_PATH} --output-dir {PROCESSED_DATA_DIR} --no-gpu ``` ## 3. Training a
-model To run with all the defaults, e.g., vanilla NeRF method with the Blender
-Lego image ```bash # To see what models are available. ns-train --help # To see
-what model-specific cli arguments are available. ns-train nerfacto --help # Run
-with nerfacto model. ns-train nerfacto # We provide support for other models.
-E.g., to run instant-ngp. ns-train instant-ngp # To train on your custom data.
-ns-train nerfacto --data {PROCESSED_DATA_DIR} ``` ### 3.x Training a model with
-the viewer You can visualize training in real-time using our web-based viewer.
-Make sure to forward a port for the websocket to localhost. The default port is
-7007, which you should expose to localhost:7007. ```bash # with the default
-port ns-train nerfacto --vis viewer # with a specified websocket port ns-train
-nerfacto --vis viewer --viewer.websocket-port=7008 # port forward if running on
-remote ssh -L localhost:7008:localhost:7008 {REMOTE HOST} ``` For more details
-on how to interact with the visualizer, please visit our viewer [walk-through]
-(https://docs.nerf.studio/en/latest/quickstart/viewer_quickstart.html). ## 4.
-Rendering a trajectory during inference After your model has trained, you can
-headlessly render out a video of the scene with a pre-defined trajectory.
-```bash # assuming previously ran `ns-train nerfacto` ns-render --load-
-config=outputs/data-nerfstudio-poster/nerfacto/{TIMESTAMP}/config.yml --
-traj=spiral --output-path=renders/output.mp4 ``` # Learn More And that's it for
-getting started with the basics of nerfstudio. If you're interested in learning
-more on how to create your own pipelines, develop with the viewer, run
-benchmarks, and more, please check out some of the quicklinks below or visit
-our [documentation](https://docs.nerf.studio/en/latest/) directly. | Section |
-Description | | ---------------------------------------------------------------
------------------------------------ | -----------------------------------------
---------------------------------------------------------- | | [Documentation]
-(https://docs.nerf.studio/en/latest/) | Full API documentation and tutorials |
-| [Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
+whl/torch_stable.html pip install ninja git+https://github.com/NVlabs/tiny-
+cuda-nn/#subdirectory=bindings/torch ``` For CUDA 11.7: ```bash pip install
+torch==1.13.1 torchvision functorch --extra-index-url https://
+download.pytorch.org/whl/cu117 pip install ninja git+https://github.com/NVlabs/
+tiny-cuda-nn/#subdirectory=bindings/torch ``` See [Dependencies](https://
+github.com/nerfstudio-project/nerfstudio/blob/main/docs/quickstart/
+installation.md#dependencies) in the Installation documentation for more. ###
+Installing nerfstudio Easy option: ```bash pip install nerfstudio ``` **OR** if
+you want the latest and greatest: ```bash git clone https://github.com/
+nerfstudio-project/nerfstudio.git cd nerfstudio pip install --upgrade pip
+setuptools pip install -e . ``` **OR** if you want to skip all installation
+steps and directly start using nerfstudio, use the docker image: See
+[Installation](https://github.com/nerfstudio-project/nerfstudio/blob/main/docs/
+quickstart/installation.md) - **Use docker image**. ## 2. Training your first
+model! The following will train a _nerfacto_ model, our recommended model for
+real world scenes. ```bash # Download some test data: ns-download-data
+nerfstudio --capture-name=poster # Train model ns-train nerfacto --data data/
+nerfstudio/poster ``` If everything works, you should see training progress
+like the following:
+                                    [image]
+Navigating to the link at the end of the terminal will load the webviewer. If
+you are running on a remote machine, you will need to port forward the
+websocket port (defaults to 7007).
+                                    [image]
+### Resume from checkpoint / visualize existing run It is possible to load a
+pretrained model by running ```bash ns-train nerfacto --data data/nerfstudio/
+poster --load-dir {outputs/.../nerfstudio_models} ``` This will automatically
+start training. If you do not want it to train, add `--viewer.start-train
+False` to your training command. ## 3. Exporting Results Once you have a NeRF
+model you can either render out a video or export a point cloud. ### Render
+Video First we must create a path for the camera to follow. This can be done in
+the viewer under the "RENDER" tab. Orient your 3D view to the location where
+you wish the video to start, then press "ADD CAMERA". This will set the first
+camera key frame. Continue to new viewpoints adding additional cameras to
+create the camera path. We provide other parameters to further refine your
+camera path. Once satisfied, press "RENDER" which will display a modal that
+contains the command needed to render the video. Kill the training job (or
+create a new terminal if you have lots of compute) and run the command to
+generate the video. Other video export options are available, learn more by
+running ```bash ns-render --help ``` ### Generate Point Cloud While NeRF models
+are not designed to generate point clouds, it is still possible. Navigate to
+the "EXPORT" tab in the 3D viewer and select "POINT CLOUD". If the crop option
+is selected, everything in the yellow square will be exported into a point
+cloud. Modify the settings as desired then run the command at the bottom of the
+panel in your command line. Alternatively you can use the CLI without the
+viewer. Learn about the export options by running ```bash ns-export pointcloud
+--help ``` ## 4. Using Custom Data Using an existing dataset is great, but
+likely you want to use your own data! We support various methods for using your
+own data. Before it can be used in nerfstudio, the camera location and
+orientations must be determined and then converted into our format using `ns-
+process-data`. We rely on external tools for this, instructions and information
+can be found in the documentation. | Data | Capture Device | Requirements |
+`ns-process-data` Speed | | ---------------------------------------------------
+------------------------------------------------- | -------------- | ----------
+------------------------------------------------------- | ---------------------
+-- | | ð· [Images](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#images-and-video) | Any | [COLMAP](https://
+colmap.github.io/install.html) | ð¢ | | ð¹ [Video](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#images-and-video) |
+Any | [COLMAP](https://colmap.github.io/install.html) | ð¢ | | ð [360
+Data](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#360_data) | Any | [COLMAP](https://colmap.github.io/
+install.html) | ð¢ | | ð± [Polycam](https://docs.nerf.studio/en/latest/
+quickstart/custom_dataset.html#polycam-capture) | IOS with LiDAR | [Polycam
+App](https://poly.cam/) | ð | | ð± [KIRI Engine](https://docs.nerf.studio/
+en/latest/quickstart/custom_dataset.html#kiri-capture) | IOS or Android | [KIRI
+Engine App](https://www.kiriengine.com/) | ð | | ð± [Record3D](https://
+docs.nerf.studio/en/latest/quickstart/custom_dataset.html#record3d-capture) |
+IOS with LiDAR | [Record3D app](https://record3d.app/) | ð | | ð¥
+[Metashape](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#metashape) | Any | [Metashape](https://www.agisoft.com/) |
+ð | | ð¥ [RealityCapture](https://docs.nerf.studio/en/latest/quickstart/
+custom_dataset.html#realitycapture) | Any | [RealityCapture](https://
+www.capturingreality.com/realitycapture) | ð | | ð  [Custom](https://
+docs.nerf.studio/en/latest/quickstart/data_conventions.html) | Any | Camera
+Poses | ð | ## 5. Advanced Options ### Training models other than nerfacto
+We provide other models than nerfacto, for example if you want to train the
+original nerf model, use the following command ```bash ns-train vanilla-nerf --
+data DATA_PATH ``` For a full list of included models run `ns-train --help`.
+### Modify Configuration Each model contains many parameters that can be
+changed, too many to list here. Use the `--help` command to see the full list
+of configuration options. ```bash ns-train nerfacto --help ``` ### Tensorboard
+/ WandB We support three different methods to track training progress, using
+the viewer, [tensorboard](https://www.tensorflow.org/tensorboard), and [Weights
+and Biases](https://wandb.ai/site). You can specify which visualizer to use by
+appending `--vis {viewer, tensorboard, wandb}` to the training command. Note
+that only one may be used at a time. Additionally the viewer only works for
+methods that are fast (ie. nerfacto, instant-ngp), for slower methods like
+NeRF, use the other loggers. # Learn More And that's it for getting started
+with the basics of nerfstudio. If you're interested in learning more on how to
+create your own pipelines, develop with the viewer, run benchmarks, and more,
+please check out some of the quicklinks below or visit our [documentation]
+(https://docs.nerf.studio/en/latest/) directly. | Section | Description | | ---
+-------------------------------------------------------------------------------
+---------------- | ------------------------------------------------------------
+-------------------------------------- | | [Documentation](https://
+docs.nerf.studio/en/latest/) | Full API documentation and tutorials | |
+[Viewer](https://viewer.nerf.studio/) | Home page for our web viewer | | ð
 **Educational** | | [Model Descriptions](https://docs.nerf.studio/en/latest/
 nerfology/methods/index.html) | Description of all the models supported by
 nerfstudio and explanations of component parts. | | [Component Descriptions]
 (https://docs.nerf.studio/en/latest/nerfology/model_components/index.html) |
 Interactive notebooks that explain notable/commonly used modules in various
 models. | | ð **Tutorials** | | [Getting Started](https://docs.nerf.studio/
 en/latest/quickstart/installation.html) | A more in-depth guide on how to get
@@ -109,31 +156,31 @@
 implementing new modules. | | [Creating datasets](https://docs.nerf.studio/en/
 latest/quickstart/custom_dataset.html) | Have a new dataset? Learn how to run
 it with nerfstudio. | | [Contributing](https://docs.nerf.studio/en/latest/
 reference/contributing.html) | Walk-through for how you can start contributing
 now. | | ð **Community** | | [Discord](https://discord.gg/uMbNqcraFc) | Join
 our community to discuss more. We would love to hear from you! | | [Twitter]
 (https://twitter.com/nerfstudioteam) | Follow us on Twitter @nerfstudioteam to
-see cool updates and announcements | | [TikTok](#) | Coming soon! Follow us on
-TikTok to see some of our fan favorite results | # Supported Features We
-provide the following support structures to make life easier for getting
-started with NeRFs. For a full description, please refer to our [features page]
-(#). **If you are looking for a feature that is not currently supported, please
-do not hesitate to contact the Nerfstudio Team on [Discord](https://discord.gg/
-uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you to: -
-Visualize training in real-time + interact with the scene - Create and render
-out scenes with custom camera trajectories - View different output types - And
-more! - :pencil2: Support for multiple logging interfaces (Tensorboard, Wandb),
-code profiling, and other built-in debugging tools - :chart_with_upwards_trend:
-Easy-to-use benchmarking scripts on the Blender dataset - :iphone: Full
-pipeline support (w/ Colmap or Record3D) for going from a video on your phone
-to a full 3D render. # Built On [tyro_logo] - Easy-to-use config system -
-Developed by [Brent Yi](https://brentyi.com/) [tyro_logo] - Library for
-accelerating NeRF renders - Developed by [Ruilong Li](https://www.liruilong.cn/
-) # Citation If you use this library or find the documentation useful for your
-research, please consider citing: ``` @misc{nerfstudio, title={Nerfstudio: A
-Framework for Neural Radiance Field Development}, author={Matthew Tancik*,
-Ethan Weber*, Evonne Ng*, Ruilong Li, Brent Yi, Terrance Wang, Alexander
-Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister,
-Angjoo Kanazawa}, year={2022}, url={https://github.com/nerfstudio-project/
-nerfstudio}, } ``` # Contributors [https://contrib.rocks/image?repo=nerfstudio-
-project/nerfstudio]
+see cool updates and announcements | # Supported Features We provide the
+following support structures to make life easier for getting started with
+NeRFs. **If you are looking for a feature that is not currently supported,
+please do not hesitate to contact the Nerfstudio Team on [Discord](https://
+discord.gg/uMbNqcraFc)!** - :mag_right: Web-based visualizer that allows you
+to: - Visualize training in real-time + interact with the scene - Create and
+render out scenes with custom camera trajectories - View different output types
+- And more! - :pencil2: Support for multiple logging interfaces (Tensorboard,
+Wandb), code profiling, and other built-in debugging tools - :
+chart_with_upwards_trend: Easy-to-use benchmarking scripts on the Blender
+dataset - :iphone: Full pipeline support (w/ Colmap, Polycam, or Record3D) for
+going from a video on your phone to a full 3D render. # Built On [tyro_logo] -
+Easy-to-use config system - Developed by [Brent Yi](https://brentyi.com/) [tyro
+logo] - Library for accelerating NeRF renders - Developed by [Ruilong Li]
+(https://www.liruilong.cn/) # Citation You can find a paper writeup of the
+framework on [arXiv](https://arxiv.org/abs/2302.04264). If you use this library
+or find the documentation useful for your research, please consider citing: ```
+@article{nerfstudio, author = {Tancik, Matthew and Weber, Ethan and Ng, Evonne
+and Li, Ruilong and Yi, Brent and Kerr, Justin and Wang, Terrance and
+Kristoffersen, Alexander and Austin, Jake and Salahi, Kamyar and Ahuja, Abhik
+and McAllister, David and Kanazawa, Angjoo}, title = {Nerfstudio: A Modular
+Framework for Neural Radiance Field Development}, journal = {arXiv preprint
+arXiv:2302.04264}, year = {2023}, } ``` # Contributors [https://contrib.rocks/
+image?repo=nerfstudio-project/nerfstudio]
```

### Comparing `nerfstudio-0.1.9/nerfstudio.egg-info/requires.txt` & `nerfstudio-0.2.0/nerfstudio.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-aiohttp==3.8.1
-aiortc==1.3.2
 appdirs>=1.4
-av==9.2.0
+av>=9.2.0
+cryptography>=38
 tyro>=0.3.31
-gdown==4.5.1
-ninja==1.10.2.3
-functorch==0.2.1
+gdown>=4.6.0
+ninja>=1.10
+functorch>=0.2.1
 h5py>=2.9.0
-imageio==2.21.1
+imageio>=2.21.1
 ipywidgets>=7.6
-jupyterlab==3.3.4
-matplotlib==3.5.3
-mediapy==1.1.0
-msgpack==1.0.4
-msgpack_numpy==0.4.8
-nerfacc==0.2.1
+jupyterlab>=3.3.4
+matplotlib>=3.5.3
+mediapy>=1.1.0
+msgpack>=1.0.4
+msgpack_numpy>=0.4.8
+nerfacc==0.3.5
 open3d>=0.16.0
 opencv-python==4.6.0.66
-plotly==5.7.0
-protobuf==3.20.0
-pyngrok==5.1.0
-python-socketio==5.7.1
+Pillow>=9.3.0
+plotly>=5.7.0
+protobuf!=3.20.0,<=3.20.3
+pyequilib>=0.5.6
+pymeshlab>=2022.2.post2
+pyngrok>=5.1.0
+python-socketio>=5.7.1
+pyquaternion>=0.9.9
 requests
-rich==12.5.1
+rich>=12.5.1
+scikit-image>=0.19.3
 tensorboard==2.9.0
-torch==1.12.1
+torch<2.0.0,>=1.12.1
 torchmetrics[image]>=0.9.3
 torchtyping>=0.1.4
 torchvision>=0.13.0
-u-msgpack-python>=2.4.1
+viser>=0.0.5
+nuscenes-devkit>=1.1.1
 wandb>=0.13.3
+xatlas
+trimesh>=3.20.2
+
+[:python_version < "3.10"]
+importlib-metadata>=6.0.0
 
 [dev]
 black[jupyter]==22.3.0
 pylint==2.13.4
 pytest==7.1.2
 pytest-xdist==2.5.0
-typeguard>=2.13.3
+typeguard==2.13.3
 
 [docs]
-furo==2022.4.7
+furo==2022.09.29
+ipython==8.6.0
 readthedocs-sphinx-search==0.1.2
 myst-nb==0.16.0
+nbconvert==7.2.5
 nbformat==5.5.0
-sphinx==4.5.0
+sphinx==5.2.1
 sphinxemoji==0.2.0
 sphinx-argparse==0.3.1
 sphinx-copybutton==0.5.0
 sphinx-design==0.2.0
 sphinxext-opengraph==0.6.3
+
+[gen]
+diffusers==0.9.0
+transformers==4.24.0
```

### Comparing `nerfstudio-0.1.9/pyproject.toml` & `nerfstudio-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,96 +1,118 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "0.1.9"
+version = "0.2.0"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.7.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "aiohttp==3.8.1",
-    "aiortc==1.3.2",
     "appdirs>=1.4",
-    "av==9.2.0",
+    "av>=9.2.0",
+    "cryptography>=38",
     "tyro>=0.3.31",
-    "gdown==4.5.1",
-    "ninja==1.10.2.3",
-    "functorch==0.2.1",
+    "gdown>=4.6.0",
+    "ninja>=1.10",
+    "functorch>=0.2.1",
     "h5py>=2.9.0",
-    "imageio==2.21.1",
+    "imageio>=2.21.1",
+    'importlib-metadata>=6.0.0; python_version < "3.10"',
     "ipywidgets>=7.6",
-    "jupyterlab==3.3.4",
-    "matplotlib==3.5.3",
-    "mediapy==1.1.0",
-    "msgpack==1.0.4",
-    "msgpack_numpy==0.4.8",
-    "nerfacc==0.2.1",
+    "jupyterlab>=3.3.4",
+    "matplotlib>=3.5.3",
+    "mediapy>=1.1.0",
+    "msgpack>=1.0.4",
+    "msgpack_numpy>=0.4.8",
+    "nerfacc==0.3.5",
     "open3d>=0.16.0",
     "opencv-python==4.6.0.66",
-    "plotly==5.7.0",
-    "protobuf==3.20.0",
-    "pyngrok==5.1.0",
-    "python-socketio==5.7.1",
+    "Pillow>=9.3.0",
+    "plotly>=5.7.0",
+    "protobuf<=3.20.3,!=3.20.0",
+    # TODO(1480) enable when pycolmap windows wheels are available
+    # "pycolmap==0.3.0",
+    "pyequilib>=0.5.6",
+    "pymeshlab>=2022.2.post2",
+    "pyngrok>=5.1.0",
+    "python-socketio>=5.7.1",
+    "pyquaternion>=0.9.9",
     "requests",
-    "rich==12.5.1",
+    "rich>=12.5.1",
+    "scikit-image>=0.19.3",
     "tensorboard==2.9.0",
-    "torch==1.12.1",
+    "torch>=1.12.1,<2.0.0",
     "torchmetrics[image]>=0.9.3",
     "torchtyping>=0.1.4",
     "torchvision>=0.13.0",
-    "u-msgpack-python>=2.4.1",
-    "wandb>=0.13.3"
+    "viser>=0.0.5",
+    "nuscenes-devkit>=1.1.1",
+    "wandb>=0.13.3",
+    "xatlas",
+    "trimesh>=3.20.2"
 ]
 
 [project.urls]
 "Documentation" = "https://docs.nerf.studio"
 
 
 [project.optional-dependencies]
+
+# Generative related dependencies
+gen = [
+    "diffusers==0.9.0",
+    "transformers==4.24.0",
+]
+
+
 # Development packages
 dev = [
     "black[jupyter]==22.3.0",
     "pylint==2.13.4",
     "pytest==7.1.2",
     "pytest-xdist==2.5.0",
-    "typeguard>=2.13.3",
+    "typeguard==2.13.3",
 ]
 
 # Documentation related packages
 docs = [
-    "furo==2022.4.7",
+    "furo==2022.09.29",
+    # Specifying ipython for https://github.com/ipython/ipython/issues/13845
+    "ipython==8.6.0",
     "readthedocs-sphinx-search==0.1.2",
     "myst-nb==0.16.0",
+    "nbconvert==7.2.5",
     "nbformat==5.5.0",
-    "sphinx==4.5.0",
+    "sphinx==5.2.1",
     "sphinxemoji==0.2.0",
     "sphinx-argparse==0.3.1",
     "sphinx-copybutton==0.5.0",
     "sphinx-design==0.2.0",
     "sphinxext-opengraph==0.6.3"
 ]
 
 [project.scripts]
 # Note, add entrypoint name to scripts/completions/install.py to include CLI completion
 ns-install-cli = "scripts.completions.install:entrypoint"
 ns-process-data = "scripts.process_data:entrypoint"
 ns-download-data = "scripts.downloads.download_data:entrypoint"
 ns-train = "scripts.train:entrypoint"
+ns-viewer = "scripts.viewer.run_viewer:entrypoint"
 ns-eval = "scripts.eval:entrypoint"
 ns-render = "scripts.render:entrypoint"
 ns-export = "scripts.exporter:entrypoint"
 ns-dev-test = "scripts.github.run_actions:entrypoint"
-ns-bridge-server = "nerfstudio.viewer.server.server:entrypoint"
+ns-dev-sync-viser-message-defs = "scripts.viewer.sync_viser_message_defs:entrypoint"
 
 [options]
 # equivalent to using --extra-index-url with pip, which is needed for specifying the CUDA version torch and torchvision
 dependency_links = [
     "https://download.pytorch.org/whl/cu113"
 ]
 
@@ -133,17 +155,16 @@
 
 # pyright
 [tool.pyright]
 include = ["nerfstudio"]
 exclude = ["**/node_modules",
     "**/__pycache__",
 ]
-ignore = ["nerfstudio/viewer"]
 defineConstant = { DEBUG = true }
 
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportPrivateImportUsage = false
 reportUndefinedVariable = false
 
-pythonVersion = "3.8"
+pythonVersion = "3.7"
 pythonPlatform = "Linux"
```

### Comparing `nerfstudio-0.1.9/scripts/completions/setup.zsh` & `nerfstudio-0.2.0/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/scripts/docs/add_nb_tags.py` & `nerfstudio-0.2.0/scripts/docs/add_nb_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 CONSOLE = Console(width=120)
 
 
 def main(check: bool = False):
     """Add tags to notebooks based on cell comments.
 
-    In notebook cells, you can add  the folling tags to the notebook by adding a comment:
+    In notebook cells, you can add the following tags to the notebook by adding a comment:
     "# HIDDEN" - This cell will be hidden from the notebook.
     "# OUTPUT_ONLY" - This cell will only show the output.
     "# COLLAPSED" - Hide the code and include a button to show the code.
 
     Args:
         check: check will not modify the notebooks.
     """
```

### Comparing `nerfstudio-0.1.9/scripts/docs/build_docs.py` & `nerfstudio-0.2.0/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/scripts/eval.py` & `nerfstudio-0.2.0/scripts/eval.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # Path to config YAML file.
     load_config: Path
     # Name of the output file.
     output_path: Path = Path("output.json")
 
     def main(self) -> None:
         """Main function."""
-        config, pipeline, checkpoint_path = eval_setup(self.load_config)
+        config, pipeline, checkpoint_path, _ = eval_setup(self.load_config)
         assert self.output_path.suffix == ".json"
         metrics_dict = pipeline.get_average_eval_image_metrics()
         self.output_path.parent.mkdir(parents=True, exist_ok=True)
         # Get the output and define the names to save to
         benchmark_info = {
             "experiment_name": config.experiment_name,
             "method_name": config.method_name,
```

### Comparing `nerfstudio-0.1.9/scripts/github/run_actions.py` & `nerfstudio-0.2.0/scripts/github/run_actions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-0.1.9/scripts/process_data.py` & `nerfstudio-0.2.0/scripts/process_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,637 +1,38 @@
 #!/usr/bin/env python
 """Processes a video or image sequence to a nerfstudio compatible dataset."""
 
-import json
+
 import shutil
-import subprocess
 import sys
-from contextlib import nullcontext
+import zipfile
 from dataclasses import dataclass
-from enum import Enum
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
-import appdirs
 import numpy as np
-import requests
 import tyro
 from rich.console import Console
-from rich.progress import track
-from scipy.spatial.transform import Rotation
 from typing_extensions import Annotated, Literal
 
-from nerfstudio.utils import colmap_utils, install_checks, io
+from nerfstudio.process_data import (
+    colmap_utils,
+    equirect_utils,
+    hloc_utils,
+    metashape_utils,
+    polycam_utils,
+    process_data_utils,
+    realitycapture_utils,
+    record3d_utils,
+)
+from nerfstudio.process_data.process_data_utils import CAMERA_MODELS
+from nerfstudio.utils import install_checks
 
 CONSOLE = Console(width=120)
-
-
-class CameraModel(Enum):
-    """Enum for camera types."""
-
-    OPENCV = "OPENCV"
-    OPENCV_FISHEYE = "OPENCV_FISHEYE"
-
-
-CAMERA_MODELS = {
-    "perspective": CameraModel.OPENCV,
-    "fisheye": CameraModel.OPENCV_FISHEYE,
-}
-
-
-def status(msg: str, spinner: str = "bouncingBall", verbose: bool = False):
-    """A context manager that does nothing is verbose is True. Otherwise it hides logs under a message.
-
-    Args:
-        msg: The message to log.
-        spinner: The spinner to use.
-        verbose: If True, print all logs, else hide them.
-    """
-    if verbose:
-        return nullcontext()
-    return CONSOLE.status(msg, spinner=spinner)
-
-
-def get_colmap_version(colmap_cmd: str, default_version=3.8) -> float:
-    """Returns the version of COLMAP.
-    This code assumes that colmap returns a version string of the form
-    "COLMAP 3.8 ..." which may not be true for all versions of COLMAP.
-
-    Args:
-        default_version: Default version to return if COLMAP version can't be determined.
-    Returns:
-        The version of COLMAP.
-    """
-    output = run_command(colmap_cmd, verbose=False)
-    assert output is not None
-    for line in output.split("\n"):
-        if line.startswith("COLMAP"):
-            return float(line.split(" ")[1])
-    CONSOLE.print(f"[bold red]Could not find COLMAP version. Using default {default_version}")
-    return default_version
-
-
-def get_vocab_tree() -> Path:
-    """Return path to vocab tree. Downloads vocab tree if it doesn't exist.
-
-    Returns:
-        The path to the vocab tree.
-    """
-    vocab_tree_filename = Path(appdirs.user_data_dir("nerfstudio")) / "vocab_tree.fbow"
-
-    if not vocab_tree_filename.exists():
-        r = requests.get("https://demuc.de/colmap/vocab_tree_flickr100K_words32K.bin", stream=True)
-        vocab_tree_filename.parent.mkdir(parents=True, exist_ok=True)
-        with open(vocab_tree_filename, "wb") as f:
-            total_length = r.headers.get("content-length")
-            assert total_length is not None
-            for chunk in track(
-                r.iter_content(chunk_size=1024),
-                total=int(total_length) / 1024 + 1,
-                description="Downloading vocab tree...",
-            ):
-                if chunk:
-                    f.write(chunk)
-                    f.flush()
-    return vocab_tree_filename
-
-
-def run_command(cmd: str, verbose=False) -> Optional[str]:
-    """Runs a command and returns the output.
-
-    Args:
-        cmd: Command to run.
-        verbose: If True, logs the output of the command.
-    Returns:
-        The output of the command if return_output is True, otherwise None.
-    """
-    out = subprocess.run(cmd, capture_output=not verbose, shell=True, check=False)
-    if out.returncode != 0:
-        CONSOLE.rule("[bold red] :skull: :skull: :skull: ERROR :skull: :skull: :skull: ", style="red")
-        CONSOLE.print(f"[bold red]Error running command: {cmd}")
-        CONSOLE.rule(style="red")
-        CONSOLE.print(out.stderr.decode("utf-8"))
-        sys.exit(1)
-    if out.stdout is not None:
-        return out.stdout.decode("utf-8")
-    return out
-
-
-def get_num_frames_in_video(video: Path) -> int:
-    """Returns the number of frames in a video.
-
-    Args:
-        video: Path to a video.
-
-    Returns:
-        The number of frames in a video.
-    """
-    cmd = f"ffprobe -v error -select_streams v:0 -count_packets \
-            -show_entries stream=nb_read_packets -of csv=p=0 {video}"
-    output = run_command(cmd)
-    assert output is not None
-    output = output.strip(" ,\t\n\r")
-    return int(output)
-
-
-def convert_video_to_images(
-    video_path: Path, image_dir: Path, num_frames_target: int, verbose: bool = False
-) -> Tuple[List[str], int]:
-    """Converts a video into a sequence of images.
-
-    Args:
-        video_path: Path to the video.
-        output_dir: Path to the output directory.
-        num_frames_target: Number of frames to extract.
-        verbose: If True, logs the output of the command.
-    Returns:
-        A tuple containing summary of the conversion and the number of extracted frames.
-    """
-
-    with status(msg="Converting video to images...", spinner="bouncingBall", verbose=verbose):
-        # delete existing images in folder
-        for img in image_dir.glob("*.png"):
-            if verbose:
-                CONSOLE.log(f"Deleting {img}")
-            img.unlink()
-
-        num_frames = get_num_frames_in_video(video_path)
-        if num_frames == 0:
-            CONSOLE.print(f"[bold red]Error: Video has no frames: {video_path}")
-            sys.exit(1)
-        print("Number of frames in video:", num_frames)
-
-        out_filename = image_dir / "frame_%05d.png"
-        ffmpeg_cmd = f"ffmpeg -i {video_path}"
-        spacing = num_frames // num_frames_target
-
-        if spacing > 1:
-            ffmpeg_cmd += f" -vf thumbnail={spacing},setpts=N/TB -r 1"
-        else:
-            CONSOLE.print("[bold red]Can't satify requested number of frames. Extracting all frames.")
-
-        ffmpeg_cmd += f" {out_filename}"
-
-        run_command(ffmpeg_cmd, verbose=verbose)
-
-    num_final_frames = len(list(image_dir.glob("*.png")))
-    summary_log = []
-    summary_log.append(f"Starting with {num_frames} video frames")
-    summary_log.append(f"We extracted {num_final_frames} images")
-    CONSOLE.log("[bold green]:tada: Done converting video to images.")
-
-    return summary_log, num_final_frames
-
-
-def convert_insta360_to_images(
-    video_front: Path,
-    video_back: Path,
-    image_dir: Path,
-    num_frames_target: int,
-    crop_percentage: float = 0.7,
-    verbose: bool = False,
-) -> Tuple[List[str], int]:
-    """Converts a video into a sequence of images.
-
-    Args:
-        video_front: Path to the front video.
-        video_back: Path to the back video.
-        output_dir: Path to the output directory.
-        num_frames_target: Number of frames to extract.
-        verbose: If True, logs the output of the command.
-    Returns:
-        A tuple containing summary of the conversion and the number of extracted frames.
-    """
-
-    with status(msg="Converting video to images...", spinner="bouncingBall", verbose=verbose):
-        # delete existing images in folder
-        for img in image_dir.glob("*.png"):
-            if verbose:
-                CONSOLE.log(f"Deleting {img}")
-            img.unlink()
-
-        num_frames_front = get_num_frames_in_video(video_front)
-        num_frames_back = get_num_frames_in_video(video_back)
-        if num_frames_front == 0:
-            CONSOLE.print(f"[bold red]Error: Video has no frames: {video_front}")
-            sys.exit(1)
-        if num_frames_back == 0:
-            CONSOLE.print(f"[bold red]Error: Video has no frames: {video_front}")
-            sys.exit(1)
-
-        spacing = num_frames_front // (num_frames_target // 2)
-        vf_cmds = []
-        if spacing > 1:
-            vf_cmds = [f"thumbnail={spacing}", "setpts=N/TB"]
-        else:
-            CONSOLE.print("[bold red]Can't satify requested number of frames. Extracting all frames.")
-
-        vf_cmds.append(f"crop=iw*{crop_percentage}:ih*{crop_percentage}")
-
-        front_vf_cmds = vf_cmds + ["transpose=2"]
-        back_vf_cmds = vf_cmds + ["transpose=1"]
-
-        front_ffmpeg_cmd = f"ffmpeg -i {video_front} -vf {','.join(front_vf_cmds)} -r 1 {image_dir / 'frame_%05d.png'}"
-        back_ffmpeg_cmd = (
-            f"ffmpeg -i {video_back} -vf {','.join(back_vf_cmds)} -r 1 {image_dir / 'back_frame_%05d.png'}"
-        )
-
-        run_command(front_ffmpeg_cmd, verbose=verbose)
-        run_command(back_ffmpeg_cmd, verbose=verbose)
-
-        num_extracted_front_frames = len(list(image_dir.glob("frame*.png")))
-        for i, img in enumerate(image_dir.glob("back_frame_*.png")):
-            img.rename(image_dir / f"frame_{i+1+num_extracted_front_frames:05d}.png")
-
-    num_final_frames = len(list(image_dir.glob("*.png")))
-    summary_log = []
-    summary_log.append(f"Starting with {num_frames_front + num_frames_back} video frames")
-    summary_log.append(f"We extracted {num_final_frames} images")
-    CONSOLE.log("[bold green]:tada: Done converting insta360 to images.")
-
-    return summary_log, num_final_frames
-
-
-def copy_images_list(image_paths: List[Path], image_dir: Path, verbose) -> List[Path]:
-    """Copy all images in a list of Paths. Useful for filtering from a directory.
-    Args:
-        image_paths: List of Paths of images to copy to a new directory.
-        image_dir: Path to the output directory.
-        verbose: If True, print extra logging.
-    Returns:
-        A list of the copied image Paths.
-    """
-
-    # Remove original directory only if we provide a proper image folder path
-    if image_dir.is_dir() and len(image_paths):
-        shutil.rmtree(image_dir, ignore_errors=True)
-        image_dir.mkdir(exist_ok=True, parents=True)
-
-    copied_image_paths = []
-
-    # Images should be 1-indexed for the rest of the pipeline.
-    for idx, image_path in enumerate(image_paths):
-        if verbose:
-            CONSOLE.log(f"Copying image {idx + 1} of {len(image_paths)}...")
-        copied_image_path = image_dir / f"frame_{idx + 1:05d}{image_path.suffix}"
-        shutil.copy(image_path, copied_image_path)
-        copied_image_paths.append(copied_image_path)
-
-    num_frames = len(image_paths)
-
-    if num_frames == 0:
-        CONSOLE.log("[bold red]:skull: No usable images in the data folder.")
-    else:
-        CONSOLE.log("[bold green]:tada: Done copying images.")
-
-    return copied_image_paths
-
-
-def copy_images(data: Path, image_dir: Path, verbose) -> int:
-    """Copy images from a directory to a new directory.
-
-    Args:
-        data: Path to the directory of images.
-        image_dir: Path to the output directory.
-        verbose: If True, print extra logging.
-    Returns:
-        The number of images copied.
-    """
-    with status(msg="[bold yellow]Copying images...", spinner="bouncingBall", verbose=verbose):
-        allowed_exts = [".jpg", ".jpeg", ".png", ".tif", ".tiff"]
-        image_paths = sorted([p for p in data.glob("[!.]*") if p.suffix.lower() in allowed_exts])
-
-        num_frames = len(copy_images_list(image_paths, image_dir, verbose))
-
-    return num_frames
-
-
-def downscale_images(image_dir: Path, num_downscales: int, verbose: bool = False) -> str:
-    """Downscales the images in the directory. Uses FFMPEG.
-
-    Assumes images are named frame_00001.png, frame_00002.png, etc.
-
-    Args:
-        image_dir: Path to the directory containing the images.
-        num_downscales: Number of times to downscale the images. Downscales by 2 each time.
-        verbose: If True, logs the output of the command.
-
-    Returns:
-        Summary of downscaling.
-    """
-
-    if num_downscales == 0:
-        return "No downscaling performed."
-
-    with status(msg="[bold yellow]Downscaling images...", spinner="growVertical", verbose=verbose):
-        downscale_factors = [2**i for i in range(num_downscales + 1)[1:]]
-        for downscale_factor in downscale_factors:
-            assert downscale_factor > 1
-            assert isinstance(downscale_factor, int)
-            downscale_dir = image_dir.parent / f"images_{downscale_factor}"
-            downscale_dir.mkdir(parents=True, exist_ok=True)
-            file_type = image_dir.glob("frame_*").__next__().suffix
-            filename = f"frame_%05d{file_type}"
-            ffmpeg_cmd = [
-                f"ffmpeg -i {image_dir / filename} ",
-                f"-q:v 2 -vf scale=iw/{downscale_factor}:ih/{downscale_factor} ",
-                f"{downscale_dir / filename}",
-            ]
-            ffmpeg_cmd = " ".join(ffmpeg_cmd)
-            run_command(ffmpeg_cmd, verbose=verbose)
-
-    CONSOLE.log("[bold green]:tada: Done downscaling images.")
-    downscale_text = [f"[bold blue]{2**(i+1)}x[/bold blue]" for i in range(num_downscales)]
-    downscale_text = ", ".join(downscale_text[:-1]) + " and " + downscale_text[-1]
-    return f"We downsampled the images by {downscale_text}"
-
-
-def run_colmap(
-    image_dir: Path,
-    colmap_dir: Path,
-    camera_model: CameraModel,
-    gpu: bool = True,
-    verbose: bool = False,
-    matching_method: Literal["vocab_tree", "exhaustive", "sequential"] = "vocab_tree",
-    colmap_cmd: str = "colmap",
-) -> None:
-    """Runs COLMAP on the images.
-
-    Args:
-        image_dir: Path to the directory containing the images.
-        colmap_dir: Path to the output directory.
-        camera_model: Camera model to use.
-        gpu: If True, use GPU.
-        verbose: If True, logs the output of the command.
-    """
-
-    colmap_version = get_colmap_version(colmap_cmd)
-
-    colmap_database_path = colmap_dir / "database.db"
-    if colmap_database_path.exists():
-        # Can't use missing_ok argument because of Python 3.7 compatibility.
-        colmap_database_path.unlink()
-
-    # Feature extraction
-    feature_extractor_cmd = [
-        f"{colmap_cmd} feature_extractor",
-        f"--database_path {colmap_dir / 'database.db'}",
-        f"--image_path {image_dir}",
-        "--ImageReader.single_camera 1",
-        f"--ImageReader.camera_model {camera_model.value}",
-        f"--SiftExtraction.use_gpu {int(gpu)}",
-    ]
-    feature_extractor_cmd = " ".join(feature_extractor_cmd)
-    with status(msg="[bold yellow]Running COLMAP feature extractor...", spinner="moon", verbose=verbose):
-        run_command(feature_extractor_cmd, verbose=verbose)
-
-    CONSOLE.log("[bold green]:tada: Done extracting COLMAP features.")
-
-    # Feature matching
-    feature_matcher_cmd = [
-        f"{colmap_cmd} {matching_method}_matcher",
-        f"--database_path {colmap_dir / 'database.db'}",
-        f"--SiftMatching.use_gpu {int(gpu)}",
-    ]
-    if matching_method == "vocab_tree":
-        vocab_tree_filename = get_vocab_tree()
-        feature_matcher_cmd.append(f"--VocabTreeMatching.vocab_tree_path {vocab_tree_filename}")
-    feature_matcher_cmd = " ".join(feature_matcher_cmd)
-    with status(msg="[bold yellow]Running COLMAP feature matcher...", spinner="runner", verbose=verbose):
-        run_command(feature_matcher_cmd, verbose=verbose)
-    CONSOLE.log("[bold green]:tada: Done matching COLMAP features.")
-
-    # Bundle adjustment
-    sparse_dir = colmap_dir / "sparse"
-    sparse_dir.mkdir(parents=True, exist_ok=True)
-    mapper_cmd = [
-        f"{colmap_cmd} mapper",
-        f"--database_path {colmap_dir / 'database.db'}",
-        f"--image_path {image_dir}",
-        f"--output_path {sparse_dir}",
-    ]
-    if colmap_version >= 3.7:
-        mapper_cmd.append("--Mapper.ba_global_function_tolerance 1e-6")
-
-    mapper_cmd = " ".join(mapper_cmd)
-
-    with status(
-        msg="[bold yellow]Running COLMAP bundle adjustment... (This may take a while)",
-        spinner="circle",
-        verbose=verbose,
-    ):
-        run_command(mapper_cmd, verbose=verbose)
-    CONSOLE.log("[bold green]:tada: Done COLMAP bundle adjustment.")
-    with status(msg="[bold yellow]Refine intrinsics...", spinner="dqpb", verbose=verbose):
-        bundle_adjuster_cmd = [
-            f"{colmap_cmd} bundle_adjuster",
-            f"--input_path {sparse_dir}/0",
-            f"--output_path {sparse_dir}/0",
-            "--BundleAdjustment.refine_principal_point 1",
-        ]
-        run_command(" ".join(bundle_adjuster_cmd), verbose=verbose)
-    CONSOLE.log("[bold green]:tada: Done refining intrinsics.")
-
-
-def colmap_to_json(cameras_path: Path, images_path: Path, output_dir: Path, camera_model: CameraModel) -> int:
-    """Converts COLMAP's cameras.bin and images.bin to a JSON file.
-
-    Args:
-        cameras_path: Path to the cameras.bin file.
-        images_path: Path to the images.bin file.
-        output_dir: Path to the output directory.
-        camera_model: Camera model used.
-
-    Returns:
-        The number of registered images.
-    """
-
-    cameras = colmap_utils.read_cameras_binary(cameras_path)
-    images = colmap_utils.read_images_binary(images_path)
-
-    # Only supports one camera
-    camera_params = cameras[1].params
-
-    frames = []
-    for _, im_data in images.items():
-        rotation = colmap_utils.qvec2rotmat(im_data.qvec)
-        translation = im_data.tvec.reshape(3, 1)
-        w2c = np.concatenate([rotation, translation], 1)
-        w2c = np.concatenate([w2c, np.array([[0, 0, 0, 1]])], 0)
-        c2w = np.linalg.inv(w2c)
-        # Convert from COLMAP's camera coordinate system to ours
-        c2w[0:3, 1:3] *= -1
-        c2w = c2w[np.array([1, 0, 2, 3]), :]
-        c2w[2, :] *= -1
-
-        name = Path(f"./images/{im_data.name}")
-
-        frame = {
-            "file_path": name.as_posix(),
-            "transform_matrix": c2w.tolist(),
-        }
-        frames.append(frame)
-
-    out = {
-        "fl_x": float(camera_params[0]),
-        "fl_y": float(camera_params[1]),
-        "cx": float(camera_params[2]),
-        "cy": float(camera_params[3]),
-        "w": cameras[1].width,
-        "h": cameras[1].height,
-        "camera_model": camera_model.value,
-    }
-
-    if camera_model == CameraModel.OPENCV:
-        out.update(
-            {
-                "k1": float(camera_params[4]),
-                "k2": float(camera_params[5]),
-                "p1": float(camera_params[6]),
-                "p2": float(camera_params[7]),
-            }
-        )
-    if camera_model == CameraModel.OPENCV_FISHEYE:
-        out.update(
-            {
-                "k1": float(camera_params[4]),
-                "k2": float(camera_params[5]),
-                "k3": float(camera_params[6]),
-                "k4": float(camera_params[7]),
-            }
-        )
-
-    out["frames"] = frames
-
-    with open(output_dir / "transforms.json", "w", encoding="utf-8") as f:
-        json.dump(out, f, indent=4)
-
-    return len(frames)
-
-
-def record3d_to_json(images_paths: List[Path], metadata_path: Path, output_dir: Path, indices: np.ndarray) -> int:
-    """Converts Record3D's metadata and image paths to a JSON file.
-
-    Args:
-        images_paths: list if image paths.
-        metadata_path: Path to the Record3D metadata JSON file.
-        output_dir: Path to the output directory.
-        indices: Indices to sample the metadata_path. Should be the same length as images_paths.
-
-    Returns:
-        The number of registered images.
-    """
-
-    assert len(images_paths) == len(indices)
-
-    metadata_dict = io.load_from_json(metadata_path)
-
-    poses_data = np.array(metadata_dict["poses"])  # (N, 3, 4)
-    camera_to_worlds = np.concatenate(
-        [Rotation.from_quat(poses_data[:, :4]).as_matrix(), poses_data[:, 4:, None]],
-        axis=-1,
-    ).astype(np.float32)
-    camera_to_worlds = camera_to_worlds[indices]
-
-    homogeneous_coord = np.zeros_like(camera_to_worlds[..., :1, :])
-    homogeneous_coord[..., :, 3] = 1
-    camera_to_worlds = np.concatenate([camera_to_worlds, homogeneous_coord], -2)
-
-    frames = []
-    for i, im_path in enumerate(images_paths):
-        c2w = camera_to_worlds[i]
-        frame = {
-            "file_path": im_path.as_posix(),
-            "transform_matrix": c2w.tolist(),
-        }
-        frames.append(frame)
-
-    # Camera intrinsics
-    K = np.array(metadata_dict["K"]).reshape((3, 3)).T
-    focal_length = K[0, 0]
-
-    H = metadata_dict["h"]
-    W = metadata_dict["w"]
-
-    # TODO(akristoffersen): The metadata dict comes with principle points,
-    # but caused errors in image coord indexing. Should update once that is fixed.
-    cx, cy = W / 2, H / 2
-
-    out = {
-        "fl_x": focal_length,
-        "fl_y": focal_length,
-        "cx": cx,
-        "cy": cy,
-        "w": W,
-        "h": H,
-        "camera_model": CAMERA_MODELS["perspective"].name,
-    }
-
-    out["frames"] = frames
-
-    with open(output_dir / "transforms.json", "w", encoding="utf-8") as f:
-        json.dump(out, f, indent=4)
-
-    return len(frames)
-
-
-def get_insta360_filenames(data: Path) -> Tuple[Path, Path]:
-    """Returns the filenames of the Insta360 videos from a single video file.
-
-    Example input name: VID_20220212_070353_00_003.insv
-
-    Args:
-        data: Path to a Insta360 file.
-
-    Returns:
-        The filenames of the Insta360 videios.
-    """
-    if data.suffix != ".insv":
-        raise ValueError("The input file must be an .insv file.")
-    file_parts = data.stem.split("_")
-
-    stem_back = f"VID_{file_parts[1]}_{file_parts[2]}_00_{file_parts[4]}.insv"
-    stem_front = f"VID_{file_parts[1]}_{file_parts[2]}_10_{file_parts[4]}.insv"
-
-    filename_back = data.parent / stem_back
-    filename_front = data.parent / stem_front
-
-    if not filename_back.exists():
-        raise FileNotFoundError(f"Could not find {filename_back}")
-    if not filename_front.exists():
-        raise FileNotFoundError(f"Could not find {filename_front}")
-
-    return filename_back, filename_front
-
-
-def get_matching_summary(num_intial_frames: int, num_matched_frames: int) -> str:
-    """Returns a summary of the matching results.
-
-    Args:
-        num_intial_frames: The number of initial frames.
-        num_matched_frames: The number of matched frames.
-
-    Returns:
-        A summary of the matching results.
-    """
-    match_ratio = num_matched_frames / num_intial_frames
-    if match_ratio == 1:
-        return "[bold green]COLAMP found poses for all images, CONGRATS!"
-    if match_ratio < 0.4:
-        result = f"[bold red]COLMAP only found poses for {num_matched_frames / num_intial_frames * 100:.2f}%"
-        result += " of the images. This is low.\nThis can be caused by a variety of reasons,"
-        result += " such poor scene coverage, blurry images, or large exposure changes."
-        return result
-    if match_ratio < 0.8:
-        result = f"[bold yellow]COLMAP only found poses for {num_matched_frames / num_intial_frames * 100:.2f}%"
-        result += " of the images.\nThis isn't great, but may be ok."
-        result += "\nMissing poses can be caused by a variety of reasons, such poor scene coverage, blurry images,"
-        result += " or large exposure changes."
-        return result
-    return f"[bold green]COLMAP found poses for {num_matched_frames / num_intial_frames * 100:.2f}% of the images."
+DEFAULT_COLMAP_PATH = Path("colmap/sparse/0")
 
 
 @dataclass
 class ProcessImages:
     """Process images into a nerfstudio dataset.
 
     This script does the following:
@@ -640,84 +41,211 @@
     2. Calculates the camera poses for each image using `COLMAP <https://colmap.github.io/>`_.
     """
 
     data: Path
     """Path the data, either a video file or a directory of images."""
     output_dir: Path
     """Path to the output directory."""
-    camera_type: Literal["perspective", "fisheye"] = "perspective"
+    camera_type: Literal["perspective", "fisheye", "equirectangular"] = "perspective"
     """Camera model to use."""
     matching_method: Literal["exhaustive", "sequential", "vocab_tree"] = "vocab_tree"
     """Feature matching method to use. Vocab tree is recommended for a balance of speed and
         accuracy. Exhaustive is slower but more accurate. Sequential is faster but should only be used for videos."""
+    sfm_tool: Literal["any", "colmap", "hloc"] = "any"
+    """Structure from motion tool to use. Colmap will use sift features, hloc can use many modern methods
+       such as superpoint features and superglue matcher"""
+    refine_pixsfm: bool = False
+    """If True, runs refinement using Pixel Perfect SFM. Only works with hloc sfm_tool"""
+    feature_type: Literal[
+        "any",
+        "sift",
+        "superpoint",
+        "superpoint_aachen",
+        "superpoint_max",
+        "superpoint_inloc",
+        "r2d2",
+        "d2net-ss",
+        "sosnet",
+        "disk",
+    ] = "any"
+    """Type of feature to use."""
+    matcher_type: Literal[
+        "any", "NN", "superglue", "superglue-fast", "NN-superpoint", "NN-ratio", "NN-mutual", "adalam"
+    ] = "any"
+    """Matching algorithm."""
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
     skip_colmap: bool = False
     """If True, skips COLMAP and generates transforms.json if possible."""
+    skip_image_processing: bool = False
+    """If True, skips copying and downscaling of images and only runs COLMAP if possible and enabled"""
+    colmap_model_path: Path = DEFAULT_COLMAP_PATH
+    """Optionally sets the path of the colmap model. Used only when --skip-colmap is set to True.
+       The path is relative to the output directory.
+    """
     colmap_cmd: str = "colmap"
     """How to call the COLMAP executable."""
+    images_per_equirect: Literal[8, 14] = 8
+    """Number of samples per image to take from each equirectangular image.
+       Used only when camera-type is equirectangular.
+    """
+    crop_factor: Tuple[float, float, float, float] = (0.0, 0.0, 0.0, 0.0)
+    """Portion of the image to crop. All values should be in [0,1]. (top, bottom, left, right)"""
     gpu: bool = True
     """If True, use GPU."""
+    use_sfm_depth: bool = False
+    """If True, export and use depth maps induced from SfM points."""
+    include_depth_debug: bool = False
+    """If --use-sfm-depth and this flag is True, also export debug images showing SfM overlaid upon input images."""
     verbose: bool = False
     """If True, print extra logging."""
 
-    def main(self) -> None:
+    def main(self) -> None:  # pylint: disable=R0915
         """Process images into a nerfstudio dataset."""
+        # pylint: disable=too-many-statements
+        require_cameras_exist = False
+        colmap_model_path = self.output_dir / Path(self.colmap_model_path)
+        if self.colmap_model_path != DEFAULT_COLMAP_PATH:
+            if not self.skip_colmap:
+                CONSOLE.log("[bold red]The --colmap-model-path can only be used when --skip-colmap is not set.")
+                sys.exit(1)
+            elif not (self.output_dir / self.colmap_model_path).exists():
+                CONSOLE.log(
+                    f"[bold red]The colmap-model-path {self.output_dir / self.colmap_model_path} does not exist."
+                )
+                sys.exit(1)
+            require_cameras_exist = True
+
         install_checks.check_ffmpeg_installed()
         install_checks.check_colmap_installed()
 
+        image_rename_map: Optional[Dict[str, str]] = None
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
+        # Generate planar projections if equirectangular
+        if self.camera_type == "equirectangular":
+            pers_size = equirect_utils.compute_resolution_from_equirect(self.data, self.images_per_equirect)
+            CONSOLE.log(f"Generating {self.images_per_equirect} {pers_size} sized images per equirectangular image")
+            self.data = equirect_utils.generate_planar_projections_from_equirectangular(
+                self.data, pers_size, self.images_per_equirect, crop_factor=self.crop_factor
+            )
+
         summary_log = []
 
-        # Copy images to output directory
-        num_frames = copy_images(self.data, image_dir=image_dir, verbose=self.verbose)
-        summary_log.append(f"Starting with {num_frames} images")
+        # Copy and downscale images
+        if not self.skip_image_processing:
+            # Copy images to output directory
+            image_rename_map_paths = process_data_utils.copy_images(
+                self.data, image_dir=image_dir, crop_factor=self.crop_factor, verbose=self.verbose
+            )
+            image_rename_map = dict((a.name, b.name) for a, b in image_rename_map_paths.items())
+            num_frames = len(image_rename_map)
+            summary_log.append(f"Starting with {num_frames} images")
 
-        # Downscale images
-        summary_log.append(downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+            # Downscale images
+            summary_log.append(
+                process_data_utils.downscale_images(image_dir, self.num_downscales, verbose=self.verbose)
+            )
+        else:
+            num_frames = len(process_data_utils.list_images(self.data))
+            if num_frames == 0:
+                CONSOLE.log("[bold red]:skull: No usable images in the data folder.")
+                sys.exit(1)
+            summary_log.append(f"Starting with {num_frames} images")
 
         # Run COLMAP
         colmap_dir = self.output_dir / "colmap"
         if not self.skip_colmap:
             colmap_dir.mkdir(parents=True, exist_ok=True)
+            colmap_model_path = colmap_dir / "sparse" / "0"
+            require_cameras_exist = True
 
-            run_colmap(
-                image_dir=image_dir,
-                colmap_dir=colmap_dir,
-                camera_model=CAMERA_MODELS[self.camera_type],
-                gpu=self.gpu,
+            self._run_colmap(image_dir, colmap_dir)
+
+            # Colmap uses renamed images
+            image_rename_map = None
+
+        # Export depth maps
+        if self.use_sfm_depth:
+            depth_dir = self.output_dir / "depth"
+            depth_dir.mkdir(parents=True, exist_ok=True)
+            image_id_to_depth_path = colmap_utils.create_sfm_depth(
+                recon_dir=colmap_dir / "sparse" / "0",
+                output_dir=depth_dir,
+                include_depth_debug=self.include_depth_debug,
+                input_images_dir=image_dir,
                 verbose=self.verbose,
-                matching_method=self.matching_method,
-                colmap_cmd=self.colmap_cmd,
             )
+            summary_log.append(
+                process_data_utils.downscale_images(
+                    depth_dir, self.num_downscales, folder_name="depths", nearest_neighbor=True, verbose=self.verbose
+                )
+            )
+        else:
+            image_id_to_depth_path = None
 
         # Save transforms.json
-        if (colmap_dir / "sparse" / "0" / "cameras.bin").exists():
+        if (colmap_model_path / "cameras.bin").exists():
             with CONSOLE.status("[bold yellow]Saving results to transforms.json", spinner="balloon"):
-                num_matched_frames = colmap_to_json(
-                    cameras_path=colmap_dir / "sparse" / "0" / "cameras.bin",
-                    images_path=colmap_dir / "sparse" / "0" / "images.bin",
+                num_matched_frames = colmap_utils.colmap_to_json(
+                    recon_dir=colmap_model_path,
                     output_dir=self.output_dir,
-                    camera_model=CAMERA_MODELS[self.camera_type],
+                    image_id_to_depth_path=image_id_to_depth_path,
+                    image_rename_map=image_rename_map,
                 )
                 summary_log.append(f"Colmap matched {num_matched_frames} images")
-            summary_log.append(get_matching_summary(num_frames, num_matched_frames))
+            summary_log.append(colmap_utils.get_matching_summary(num_frames, num_matched_frames))
+        elif require_cameras_exist:
+            CONSOLE.log(f"[bold red]Could not find existing COLMAP results ({colmap_model_path / 'cameras.bin'}).")
+            sys.exit(1)
         else:
             CONSOLE.log("[bold yellow]Warning: could not find existing COLMAP results. Not generating transforms.json")
 
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
             CONSOLE.print(summary, justify="center")
         CONSOLE.rule()
 
+    def _run_colmap(self, image_dir, colmap_dir):
+        (sfm_tool, feature_type, matcher_type) = process_data_utils.find_tool_feature_matcher_combination(
+            self.sfm_tool, self.feature_type, self.matcher_type
+        )
+        # check that sfm_tool is hloc if using refine_pixsfm
+        if self.refine_pixsfm:
+            assert sfm_tool == "hloc", "refine_pixsfm only works with sfm_tool hloc"
+
+        if sfm_tool == "colmap":
+            colmap_utils.run_colmap(
+                image_dir=image_dir,
+                colmap_dir=colmap_dir,
+                camera_model=CAMERA_MODELS[self.camera_type],
+                gpu=self.gpu,
+                verbose=self.verbose,
+                matching_method=self.matching_method,
+                colmap_cmd=self.colmap_cmd,
+            )
+        elif sfm_tool == "hloc":
+            hloc_utils.run_hloc(
+                image_dir=image_dir,
+                colmap_dir=colmap_dir,
+                camera_model=CAMERA_MODELS[self.camera_type],
+                verbose=self.verbose,
+                matching_method=self.matching_method,
+                feature_type=feature_type,
+                matcher_type=matcher_type,
+                refine_pixsfm=self.refine_pixsfm,
+            )
+        else:
+            CONSOLE.log("[bold red]Invalid combination of sfm_tool, feature_type, and matcher_type, exiting")
+            sys.exit(1)
+
 
 @dataclass
 class ProcessVideo:
     """Process videos into a nerfstudio dataset.
 
     This script does the following:
 
@@ -728,257 +256,580 @@
 
     data: Path
     """Path the data, either a video file or a directory of images."""
     output_dir: Path
     """Path to the output directory."""
     num_frames_target: int = 300
     """Target number of frames to use for the dataset, results may not be exact."""
-    camera_type: Literal["perspective", "fisheye"] = "perspective"
+    camera_type: Literal["perspective", "fisheye", "equirectangular"] = "perspective"
     """Camera model to use."""
     matching_method: Literal["exhaustive", "sequential", "vocab_tree"] = "vocab_tree"
     """Feature matching method to use. Vocab tree is recommended for a balance of speed and
         accuracy. Exhaustive is slower but more accurate. Sequential is faster but should only be used for videos."""
+    sfm_tool: Literal["any", "colmap", "hloc"] = "any"
+    """Structure from motion tool to use. Colmap will use sift features, hloc can use many modern methods
+       such as superpoint features and superglue matcher"""
+    refine_pixsfm: bool = False
+    """If True, runs refinement using Pixel Perfect SFM. Only has an effect if sfm_tool is hloc"""
+    feature_type: Literal[
+        "any",
+        "sift",
+        "superpoint",
+        "superpoint_aachen",
+        "superpoint_max",
+        "superpoint_inloc",
+        "r2d2",
+        "d2net-ss",
+        "sosnet",
+        "disk",
+    ] = "any"
+    """Type of feature to use."""
+    matcher_type: Literal[
+        "any", "NN", "superglue", "superglue-fast", "NN-superpoint", "NN-ratio", "NN-mutual", "adalam"
+    ] = "any"
+    """Matching algorithm."""
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
     skip_colmap: bool = False
     """If True, skips COLMAP and generates transforms.json if possible."""
     colmap_cmd: str = "colmap"
     """How to call the COLMAP executable."""
+    images_per_equirect: Literal[8, 14] = 8
+    """Number of samples per image to take from each equirectangular image.
+       Used only when camera-type is equirectangular.
+    """
+    percent_radius_crop: float = 1.0
+    """Create circle crop mask. The radius is the percent of the image diagonal."""
+    crop_factor: Tuple[float, float, float, float] = (0.0, 0.0, 0.0, 0.0)
+    """Portion of the image to crop. All values should be in [0,1]. (top, bottom, left, right)"""
+    use_sfm_depth: bool = False
+    """If True, export and use depth maps induced from SfM points."""
+    include_depth_debug: bool = False
+    """If --use-sfm-depth and this flag is True, also export debug images showing SfM overlaid upon input images."""
     gpu: bool = True
     """If True, use GPU."""
     verbose: bool = False
     """If True, print extra logging."""
 
-    def main(self) -> None:
+    def main(self) -> None:  # pylint: disable=R0915
         """Process video into a nerfstudio dataset."""
         install_checks.check_ffmpeg_installed()
         install_checks.check_colmap_installed()
 
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
+        summary_log = []
         # Convert video to images
-        summary_log, num_extracted_frames = convert_video_to_images(
-            self.data, image_dir=image_dir, num_frames_target=self.num_frames_target, verbose=self.verbose
+        if self.camera_type == "equirectangular":
+            # create temp images folder to store the equirect and perspective images
+            temp_image_dir = self.output_dir / "temp_images"
+            temp_image_dir.mkdir(parents=True, exist_ok=True)
+            summary_log, num_extracted_frames = process_data_utils.convert_video_to_images(
+                self.data,
+                image_dir=temp_image_dir,
+                num_frames_target=self.num_frames_target,
+                crop_factor=(0.0, 0.0, 0.0, 0.0),
+                verbose=self.verbose,
+            )
+        else:
+            summary_log, num_extracted_frames = process_data_utils.convert_video_to_images(
+                self.data,
+                image_dir=image_dir,
+                num_frames_target=self.num_frames_target,
+                crop_factor=self.crop_factor,
+                verbose=self.verbose,
+            )
+
+        # Generate planar projections if equirectangular
+        if self.camera_type == "equirectangular":
+            perspective_image_size = equirect_utils.compute_resolution_from_equirect(
+                self.output_dir / "temp_images", self.images_per_equirect
+            )
+            image_dir = equirect_utils.generate_planar_projections_from_equirectangular(
+                self.output_dir / "temp_images",
+                perspective_image_size,
+                self.images_per_equirect,
+                crop_factor=self.crop_factor,
+            )
+
+            # copy the perspective images to the image directory
+            process_data_utils.copy_images(
+                self.output_dir / "temp_images" / "planar_projections",
+                image_dir=self.output_dir / "images",
+                verbose=False,
+            )
+            image_dir = self.output_dir / "images"
+
+            # remove the temp_images folder
+            shutil.rmtree(self.output_dir / "temp_images", ignore_errors=True)
+
+        # # Create mask
+        mask_path = process_data_utils.save_mask(
+            image_dir=image_dir,
+            num_downscales=self.num_downscales,
+            crop_factor=(0.0, 0.0, 0.0, 0.0),
+            percent_radius=self.percent_radius_crop,
         )
+        if mask_path is not None:
+            summary_log.append(f"Saved mask to {mask_path}")
 
-        # Downscale images
-        summary_log.append(downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+        # # Downscale images
+        summary_log.append(process_data_utils.downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
 
         # Run Colmap
         colmap_dir = self.output_dir / "colmap"
         if not self.skip_colmap:
             colmap_dir.mkdir(parents=True, exist_ok=True)
 
-            run_colmap(
-                image_dir=image_dir,
-                colmap_dir=colmap_dir,
-                camera_model=CAMERA_MODELS[self.camera_type],
-                gpu=self.gpu,
+            (sfm_tool, feature_type, matcher_type) = process_data_utils.find_tool_feature_matcher_combination(
+                self.sfm_tool, self.feature_type, self.matcher_type
+            )
+
+            if sfm_tool == "colmap":
+                colmap_utils.run_colmap(
+                    image_dir=image_dir,
+                    colmap_dir=colmap_dir,
+                    camera_model=CAMERA_MODELS[self.camera_type],
+                    camera_mask_path=mask_path,
+                    gpu=self.gpu,
+                    verbose=self.verbose,
+                    matching_method=self.matching_method,
+                    colmap_cmd=self.colmap_cmd,
+                )
+            elif sfm_tool == "hloc":
+                if mask_path is not None:
+                    CONSOLE.log(
+                        "[bold red]Cannot use a mask with hloc. Please remove the cropping options and try again."
+                    )
+                    sys.exit(1)
+                hloc_utils.run_hloc(
+                    image_dir=image_dir,
+                    colmap_dir=colmap_dir,
+                    camera_model=CAMERA_MODELS[self.camera_type],
+                    verbose=self.verbose,
+                    matching_method=self.matching_method,
+                    feature_type=feature_type,
+                    matcher_type=matcher_type,
+                    refine_pixsfm=self.refine_pixsfm,
+                )
+            else:
+                CONSOLE.log("[bold red]Invalid combination of sfm_tool, feature_type, and matcher_type, exiting")
+                sys.exit(1)
+
+        # Export depth maps
+        if self.use_sfm_depth:
+            depth_dir = self.output_dir / "depth"
+            depth_dir.mkdir(parents=True, exist_ok=True)
+            image_id_to_depth_path = colmap_utils.create_sfm_depth(
+                recon_dir=colmap_dir / "sparse" / "0",
+                output_dir=depth_dir,
+                include_depth_debug=self.include_depth_debug,
+                input_images_dir=image_dir,
                 verbose=self.verbose,
-                matching_method=self.matching_method,
-                colmap_cmd=self.colmap_cmd,
             )
+            summary_log.append(
+                process_data_utils.downscale_images(
+                    depth_dir, self.num_downscales, folder_name="depths", nearest_neighbor=True, verbose=self.verbose
+                )
+            )
+        else:
+            image_id_to_depth_path = None
 
         # Save transforms.json
         if (colmap_dir / "sparse" / "0" / "cameras.bin").exists():
             with CONSOLE.status("[bold yellow]Saving results to transforms.json", spinner="balloon"):
-                num_matched_frames = colmap_to_json(
-                    cameras_path=colmap_dir / "sparse" / "0" / "cameras.bin",
-                    images_path=colmap_dir / "sparse" / "0" / "images.bin",
+                num_matched_frames = colmap_utils.colmap_to_json(
+                    recon_dir=colmap_dir / "sparse" / "0",
                     output_dir=self.output_dir,
-                    camera_model=CAMERA_MODELS[self.camera_type],
+                    image_id_to_depth_path=image_id_to_depth_path,
+                    camera_mask_path=mask_path,
+                    image_rename_map=None,
                 )
                 summary_log.append(f"Colmap matched {num_matched_frames} images")
-            summary_log.append(get_matching_summary(num_extracted_frames, num_matched_frames))
+            summary_log.append(colmap_utils.get_matching_summary(num_extracted_frames, num_matched_frames))
         else:
             CONSOLE.log("[bold yellow]Warning: could not find existing COLMAP results. Not generating transforms.json")
 
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
             CONSOLE.print(summary, justify="center")
         CONSOLE.rule()
 
 
 @dataclass
-class ProcessInsta360:
-    """Process Insta360 videos into a nerfstudio dataset. Currently this uses a center crop of the raw data
-    so data at the extreme edges of the video will be lost.
-
-    Expects data from a 2 camera Insta360, single or >2 camera models will not work.
-    (tested with Insta360 One X2)
+class ProcessRecord3D:
+    """Process Record3D data into a nerfstudio dataset.
 
     This script does the following:
 
-    1. Converts the videos into images.
-    2. Scales images to a specified size.
-    3. Calculates the camera poses for each image using `COLMAP <https://colmap.github.io/>`_.
+    1. Scales images to a specified size.
+    2. Converts Record3D poses into the nerfstudio format.
     """
 
     data: Path
-    """Path the data, It should be one of the 3 .insv files saved with each capture (Any work)."""
+    """Path to the record3D data."""
     output_dir: Path
     """Path to the output directory."""
-    num_frames_target: int = 400
-    """Target number of frames to use for the dataset, results may not be exact."""
-    matching_method: Literal["exhaustive", "sequential", "vocab_tree"] = "vocab_tree"
-    """Feature matching method to use. Vocab tree is recommended for a balance of speed and
-        accuracy. Exhaustive is slower but more accurate. Sequential is faster but should only be used for videos."""
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
-    skip_colmap: bool = False
-    """If True, skips COLMAP and generates transforms.json if possible."""
-    colmap_cmd: str = "colmap"
-    """How to call the COLMAP executable."""
-    gpu: bool = True
-    """If True, use GPU."""
+    max_dataset_size: int = 300
+    """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
+    use all images."""
+
     verbose: bool = False
     """If True, print extra logging."""
 
     def main(self) -> None:
-        """Process video into a nerfstudio dataset."""
-        install_checks.check_ffmpeg_installed()
-        install_checks.check_colmap_installed()
+        """Process images into a nerfstudio dataset."""
 
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
-        filename_back, filename_front = get_insta360_filenames(self.data)
+        summary_log = []
 
-        # Convert video to images
-        summary_log, num_extracted_frames = convert_insta360_to_images(
-            video_front=filename_front,
-            video_back=filename_back,
-            image_dir=image_dir,
-            num_frames_target=self.num_frames_target,
-            verbose=self.verbose,
+        record3d_image_dir = self.data / "rgb"
+
+        if not record3d_image_dir.exists():
+            raise ValueError(f"Image directory {record3d_image_dir} doesn't exist")
+
+        record3d_image_filenames = []
+        for f in record3d_image_dir.iterdir():
+            if f.stem.isdigit():  # removes possible duplicate images (for example, 123(3).jpg)
+                if f.suffix.lower() in [".jpg", ".jpeg", ".png", ".tif", ".tiff"]:
+                    record3d_image_filenames.append(f)
+
+        record3d_image_filenames = sorted(record3d_image_filenames, key=lambda fn: int(fn.stem))
+        num_images = len(record3d_image_filenames)
+        idx = np.arange(num_images)
+        if self.max_dataset_size != -1 and num_images > self.max_dataset_size:
+            idx = np.round(np.linspace(0, num_images - 1, self.max_dataset_size)).astype(int)
+
+        record3d_image_filenames = list(np.array(record3d_image_filenames)[idx])
+        # Copy images to output directory
+        copied_image_paths = process_data_utils.copy_images_list(
+            record3d_image_filenames, image_dir=image_dir, verbose=self.verbose
         )
+        num_frames = len(copied_image_paths)
+
+        copied_image_paths = [Path("images/" + copied_image_path.name) for copied_image_path in copied_image_paths]
+        summary_log.append(f"Used {num_frames} images out of {num_images} total")
+        if self.max_dataset_size > 0:
+            summary_log.append(
+                "To change the size of the dataset add the argument [yellow]--max_dataset_size[/yellow] to "
+                f"larger than the current value ({self.max_dataset_size}), or -1 to use all images."
+            )
 
         # Downscale images
-        summary_log.append(downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+        summary_log.append(process_data_utils.downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
 
-        # Run Colmap
-        colmap_dir = self.output_dir / "colmap"
-        if not self.skip_colmap:
-            colmap_dir.mkdir(parents=True, exist_ok=True)
+        metadata_path = self.data / "metadata.json"
+        record3d_utils.record3d_to_json(copied_image_paths, metadata_path, self.output_dir, indices=idx)
+        CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
-            run_colmap(
-                image_dir=image_dir,
-                colmap_dir=colmap_dir,
-                camera_model=CAMERA_MODELS["fisheye"],
-                gpu=self.gpu,
+        for summary in summary_log:
+            CONSOLE.print(summary, justify="center")
+        CONSOLE.rule()
+
+
+@dataclass
+class ProcessPolycam:
+    """Process Polycam data into a nerfstudio dataset.
+
+    To capture data, use the Polycam app on an iPhone or iPad with LiDAR. The capture must be in LiDAR or ROOM mode.
+    Developer mode must be enabled in the app settings, this will enable a raw data export option in the export menus.
+    The exported data folder is used as the input to this script.
+
+    This script does the following:
+
+    1. Scales images to a specified size.
+    2. Converts Polycam poses into the nerfstudio format.
+    """
+
+    data: Path
+    """Path the polycam export data folder. Can be .zip file or folder."""
+    output_dir: Path
+    """Path to the output directory."""
+    num_downscales: int = 3
+    """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
+        will downscale the images by 2x, 4x, and 8x."""
+    use_uncorrected_images: bool = False
+    """If True, use the raw images from the polycam export. If False, use the corrected images."""
+    max_dataset_size: int = 600
+    """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
+    use all images."""
+    min_blur_score: float = 25
+    """Minimum blur score to use an image. If the blur score is below this value, the image will be skipped."""
+    crop_border_pixels: int = 15
+    """Number of pixels to crop from each border of the image. Useful as borders may be black due to undistortion."""
+    use_depth: bool = False
+    """If True, processes the generated depth maps from Polycam"""
+    verbose: bool = False
+    """If True, print extra logging."""
+
+    def main(self) -> None:
+        """Process images into a nerfstudio dataset."""
+
+        self.output_dir.mkdir(parents=True, exist_ok=True)
+        image_dir = self.output_dir / "images"
+        image_dir.mkdir(parents=True, exist_ok=True)
+
+        summary_log = []
+
+        if self.data.suffix == ".zip":
+            with zipfile.ZipFile(self.data, "r") as zip_ref:
+                zip_ref.extractall(self.output_dir)
+                extracted_folder = zip_ref.namelist()[0].split("/")[0]
+            self.data = self.output_dir / extracted_folder
+
+        if (self.data / "keyframes" / "corrected_images").exists() and not self.use_uncorrected_images:
+            polycam_image_dir = self.data / "keyframes" / "corrected_images"
+            polycam_cameras_dir = self.data / "keyframes" / "corrected_cameras"
+        else:
+            polycam_image_dir = self.data / "keyframes" / "images"
+            polycam_cameras_dir = self.data / "keyframes" / "cameras"
+            if not self.use_uncorrected_images:
+                CONSOLE.print("[bold yellow]Corrected images not found, using raw images.")
+
+        if not polycam_image_dir.exists():
+            raise ValueError(f"Image directory {polycam_image_dir} doesn't exist")
+
+        if not (self.data / "keyframes" / "depth").exists():
+            depth_dir = self.data / "keyframes" / "depth"
+            raise ValueError(f"Depth map directory {depth_dir} doesn't exist")
+
+        (image_processing_log, polycam_image_filenames) = polycam_utils.process_images(
+            polycam_image_dir,
+            image_dir,
+            crop_border_pixels=self.crop_border_pixels,
+            max_dataset_size=self.max_dataset_size,
+            num_downscales=self.num_downscales,
+            verbose=self.verbose,
+        )
+
+        summary_log.extend(image_processing_log)
+
+        polycam_depth_filenames = []
+        if self.use_depth:
+            polycam_depth_image_dir = self.data / "keyframes" / "depth"
+            depth_dir = self.output_dir / "depth"
+            depth_dir.mkdir(parents=True, exist_ok=True)
+            (depth_processing_log, polycam_depth_filenames) = polycam_utils.process_depth_maps(
+                polycam_depth_image_dir,
+                depth_dir,
+                num_processed_images=len(polycam_image_filenames),
+                crop_border_pixels=self.crop_border_pixels,
+                max_dataset_size=self.max_dataset_size,
+                num_downscales=self.num_downscales,
                 verbose=self.verbose,
-                matching_method=self.matching_method,
-                colmap_cmd=self.colmap_cmd,
             )
+            summary_log.extend(depth_processing_log)
 
-        # Save transforms.json
-        if (colmap_dir / "sparse" / "0" / "cameras.bin").exists():
-            with CONSOLE.status("[bold yellow]Saving results to transforms.json", spinner="balloon"):
-                num_matched_frames = colmap_to_json(
-                    cameras_path=colmap_dir / "sparse" / "0" / "cameras.bin",
-                    images_path=colmap_dir / "sparse" / "0" / "images.bin",
-                    output_dir=self.output_dir,
-                    camera_model=CAMERA_MODELS["fisheye"],
-                )
-                summary_log.append(f"Colmap matched {num_matched_frames} images")
-            summary_log.append(get_matching_summary(num_extracted_frames, num_matched_frames))
-        else:
-            CONSOLE.log("[bold yellow]Warning: could not find existing COLMAP results. Not generating transforms.json")
+        summary_log.extend(
+            polycam_utils.polycam_to_json(
+                image_filenames=polycam_image_filenames,
+                depth_filenames=polycam_depth_filenames,
+                cameras_dir=polycam_cameras_dir,
+                output_dir=self.output_dir,
+                min_blur_score=self.min_blur_score,
+                crop_border_pixels=self.crop_border_pixels,
+            )
+        )
 
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
             CONSOLE.print(summary, justify="center")
         CONSOLE.rule()
 
 
 @dataclass
-class ProcessRecord3D:
-    """Process Record3D data into a nerfstudio dataset.
+class ProcessMetashape:
+    """Process Metashape data into a nerfstudio dataset.
+
+    This script assumes that cameras have been aligned using Metashape. After alignment, it is necessary to export the
+    camera poses as a `.xml` file. This option can be found under `File > Export > Export Cameras`.
 
     This script does the following:
 
     1. Scales images to a specified size.
-    2. Converts Record3D poses into the nerfacto format.
+    2. Converts Metashape poses into the nerfstudio format.
     """
 
     data: Path
-    """Path the data, either a video file or a directory of images."""
+    """Path to a folder of images."""
+    xml: Path
+    """Path to the Metashape xml file."""
     output_dir: Path
     """Path to the output directory."""
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
-    max_dataset_size: int = 300
+    max_dataset_size: int = 600
     """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
     use all images."""
-
     verbose: bool = False
     """If True, print extra logging."""
 
     def main(self) -> None:
         """Process images into a nerfstudio dataset."""
 
+        if self.xml.suffix != ".xml":
+            raise ValueError(f"XML file {self.xml} must have a .xml extension")
+        if not self.xml.exists:
+            raise ValueError(f"XML file {self.xml} doesn't exist")
+
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
         summary_log = []
 
-        record3d_image_dir = self.data / "rgb"
+        # Copy images to output directory
+        image_filenames, num_orig_images = process_data_utils.get_image_filenames(self.data, self.max_dataset_size)
+        copied_image_paths = process_data_utils.copy_images_list(
+            image_filenames,
+            image_dir=image_dir,
+            verbose=self.verbose,
+        )
+        num_frames = len(copied_image_paths)
 
-        if not record3d_image_dir.exists():
-            raise ValueError(f"Image directory {image_dir} doesn't exist")
+        copied_image_paths = [Path("images/" + copied_image_path.name) for copied_image_path in copied_image_paths]
+        original_names = [image_path.stem for image_path in image_filenames]
+        image_filename_map = dict(zip(original_names, copied_image_paths))
 
-        record3d_image_filenames = []
-        for f in record3d_image_dir.iterdir():
-            if f.stem.isdigit():  # removes possible duplicate images (for example, 123(3).jpg)
-                record3d_image_filenames.append(f)
+        if self.max_dataset_size > 0 and num_frames != num_orig_images:
+            summary_log.append(f"Started with {num_frames} images out of {num_orig_images} total")
+            summary_log.append(
+                "To change the size of the dataset add the argument [yellow]--max_dataset_size[/yellow] to "
+                f"larger than the current value ({self.max_dataset_size}), or -1 to use all images."
+            )
+        else:
+            summary_log.append(f"Started with {num_frames} images")
 
-        record3d_image_filenames = sorted(record3d_image_filenames, key=lambda fn: int(fn.stem))
-        num_images = len(record3d_image_filenames)
-        idx = np.arange(num_images)
-        if self.max_dataset_size != -1 and num_images > self.max_dataset_size:
-            idx = np.round(np.linspace(0, num_images - 1, self.max_dataset_size)).astype(int)
+        # Downscale images
+        summary_log.append(process_data_utils.downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+
+        # Save json
+        if num_frames == 0:
+            CONSOLE.print("[bold red]No images found, exiting")
+            sys.exit(1)
+        summary_log.extend(
+            metashape_utils.metashape_to_json(
+                image_filename_map=image_filename_map,
+                xml_filename=self.xml,
+                output_dir=self.output_dir,
+                verbose=self.verbose,
+            )
+        )
+
+        CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
+
+        for summary in summary_log:
+            CONSOLE.print(summary, justify="center")
+        CONSOLE.rule()
+
+
+@dataclass
+class ProcessRealityCapture:
+    """Process RealityCapture data into a nerfstudio dataset.
+
+    This script assumes that cameras have been aligned using RealityCapture. After alignment, it is necessary to
+    export the camera poses as a `.csv` file using the `Internal/External camera parameters` option.
+
+    This script does the following:
+
+    1. Scales images to a specified size.
+    2. Converts RealityCapture poses into the nerfstudio format.
+    """
+
+    data: Path
+    """Path to a folder of images."""
+    csv: Path
+    """Path to the RealityCapture cameras CSV file."""
+    output_dir: Path
+    """Path to the output directory."""
+    num_downscales: int = 3
+    """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
+        will downscale the images by 2x, 4x, and 8x."""
+    max_dataset_size: int = 600
+    """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
+    use all images."""
+    verbose: bool = False
+    """If True, print extra logging."""
+
+    def main(self) -> None:
+        """Process images into a nerfstudio dataset."""
+
+        if self.csv.suffix != ".csv":
+            raise ValueError(f"CSV file {self.csv} must have a .csv extension")
+        if not self.csv.exists:
+            raise ValueError(f"CSV file {self.csv} doesn't exist")
+
+        self.output_dir.mkdir(parents=True, exist_ok=True)
+        image_dir = self.output_dir / "images"
+        image_dir.mkdir(parents=True, exist_ok=True)
+
+        summary_log = []
 
-        record3d_image_filenames = list(np.array(record3d_image_filenames)[idx])
         # Copy images to output directory
-        copied_image_paths = copy_images_list(record3d_image_filenames, image_dir=image_dir, verbose=self.verbose)
+        image_filenames, num_orig_images = process_data_utils.get_image_filenames(self.data, self.max_dataset_size)
+        copied_image_paths = process_data_utils.copy_images_list(
+            image_filenames,
+            image_dir=image_dir,
+            verbose=self.verbose,
+        )
         num_frames = len(copied_image_paths)
 
         copied_image_paths = [Path("images/" + copied_image_path.name) for copied_image_path in copied_image_paths]
-        summary_log.append(f"Used {num_frames} images out of {num_images} total")
-        if self.max_dataset_size > 0:
+        original_names = [image_path.stem for image_path in image_filenames]
+        image_filename_map = dict(zip(original_names, copied_image_paths))
+
+        if self.max_dataset_size > 0 and num_frames != num_orig_images:
+            summary_log.append(f"Started with {num_frames} images out of {num_orig_images} total")
             summary_log.append(
-                "To change the size of the dataset add the argument --max_dataset_size to larger than the "
-                f"current value ({self.max_dataset_size}), or -1 to use all images."
+                "To change the size of the dataset add the argument [yellow]--max_dataset_size[/yellow] to "
+                f"larger than the current value ({self.max_dataset_size}), or -1 to use all images."
             )
+        else:
+            summary_log.append(f"Started with {num_frames} images")
 
         # Downscale images
-        summary_log.append(downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+        summary_log.append(process_data_utils.downscale_images(image_dir, self.num_downscales, verbose=self.verbose))
+
+        # Save json
+        if num_frames == 0:
+            CONSOLE.print("[bold red]No images found, exiting")
+            sys.exit(1)
+        summary_log.extend(
+            realitycapture_utils.realitycapture_to_json(
+                image_filename_map=image_filename_map,
+                csv_filename=self.csv,
+                output_dir=self.output_dir,
+            )
+        )
 
-        metadata_path = self.data / "metadata.json"
-        record3d_to_json(copied_image_paths, metadata_path, self.output_dir, indices=idx)
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
             CONSOLE.print(summary, justify="center")
         CONSOLE.rule()
 
 
 Commands = Union[
     Annotated[ProcessImages, tyro.conf.subcommand(name="images")],
     Annotated[ProcessVideo, tyro.conf.subcommand(name="video")],
-    Annotated[ProcessInsta360, tyro.conf.subcommand(name="insta360")],
+    Annotated[ProcessPolycam, tyro.conf.subcommand(name="polycam")],
+    Annotated[ProcessMetashape, tyro.conf.subcommand(name="metashape")],
+    Annotated[ProcessRealityCapture, tyro.conf.subcommand(name="realitycapture")],
     Annotated[ProcessRecord3D, tyro.conf.subcommand(name="record3d")],
 ]
 
 
 def entrypoint():
     """Entrypoint for use with pyproject scripts."""
     tyro.extras.set_accent_color("bright_yellow")
```

### Comparing `nerfstudio-0.1.9/scripts/train.py` & `nerfstudio-0.2.0/scripts/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 import torch
 import torch.distributed as dist
 import torch.multiprocessing as mp
 import tyro
 import yaml
 from rich.console import Console
 
-from nerfstudio.configs import base_config as cfg
 from nerfstudio.configs.config_utils import convert_markup_to_ansi
 from nerfstudio.configs.method_configs import AnnotatedBaseConfigUnion
-from nerfstudio.engine.trainer import Trainer
+from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.utils import comms, profiler
 
 CONSOLE = Console(width=120)
 DEFAULT_TIMEOUT = timedelta(minutes=30)
 
 # speedup for when input size to model doesn't change (much)
 torch.backends.cudnn.benchmark = True  # type: ignore
@@ -70,51 +69,51 @@
 def _set_random_seed(seed) -> None:
     """Set randomness seed in torch and numpy"""
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
 
 
-def train_loop(local_rank: int, world_size: int, config: cfg.Config, global_rank: int = 0):
+def train_loop(local_rank: int, world_size: int, config: TrainerConfig, global_rank: int = 0):
     """Main training function that sets up and runs the trainer per process
 
     Args:
         local_rank: current rank of process
         world_size: total number of gpus available
         config: config file specifying training regimen
     """
     _set_random_seed(config.machine.seed + global_rank)
-    trainer = Trainer(config, local_rank, world_size)
+    trainer = config.setup(local_rank=local_rank, world_size=world_size)
     trainer.setup()
     trainer.train()
 
 
 def _distributed_worker(
     local_rank: int,
     main_func: Callable,
     world_size: int,
     num_gpus_per_machine: int,
     machine_rank: int,
     dist_url: str,
-    config: cfg.Config,
+    config: TrainerConfig,
     timeout: timedelta = DEFAULT_TIMEOUT,
 ) -> Any:
     """Spawned distributed worker that handles the initialization of process group and handles the
        training process on multiple processes.
 
     Args:
         local_rank: Current rank of process.
         main_func: Function that will be called by the distributed workers.
         world_size: Total number of gpus available.
         num_gpus_per_machine: Number of GPUs per machine.
         machine_rank: Rank of this machine.
         dist_url: URL to connect to for distributed jobs, including protocol
             E.g., "tcp://127.0.0.1:8686".
             It can be set to "auto" to automatically select a free port on localhost.
-        config: Config specifying training regimen.
+        config: TrainerConfig specifying training regimen.
         timeout: Timeout of the distributed workers.
 
     Raises:
         e: Exception in initializing the process group
 
     Returns:
         Any: TODO: determine the return type
@@ -146,26 +145,26 @@
 
 def launch(
     main_func: Callable,
     num_gpus_per_machine: int,
     num_machines: int = 1,
     machine_rank: int = 0,
     dist_url: str = "auto",
-    config: Optional[cfg.Config] = None,
+    config: Optional[TrainerConfig] = None,
     timeout: timedelta = DEFAULT_TIMEOUT,
 ) -> None:
-    """Function that spawns muliple processes to call on main_func
+    """Function that spawns multiple processes to call on main_func
 
     Args:
         main_func (Callable): function that will be called by the distributed workers
         num_gpus_per_machine (int): number of GPUs per machine
         num_machines (int, optional): total number of machines
         machine_rank (int, optional): rank of this machine.
         dist_url (str, optional): url to connect to for distributed jobs.
-        config (Config, optional): config file specifying training regimen.
+        config (TrainerConfig, optional): config file specifying training regimen.
         timeout (timedelta, optional): timeout of the distributed workers.
     """
     assert config is not None
     world_size = num_machines * num_gpus_per_machine
     if world_size <= 1:
         # world_size=0 uses one CPU in one process.
         # world_size=1 uses one GPU in one process.
@@ -211,25 +210,25 @@
                     process.terminate()
                 process.join()
                 CONSOLE.log(f"Process {i} finished.")
         finally:
             profiler.flush_profiler(config.logging)
 
 
-def main(config: cfg.Config) -> None:
+def main(config: TrainerConfig) -> None:
     """Main function."""
 
     config.set_timestamp()
     if config.data:
-        CONSOLE.log("Using --data alias for --data.pipeline.datamanager.dataparser.data")
-        config.pipeline.datamanager.dataparser.data = config.data
+        CONSOLE.log("Using --data alias for --data.pipeline.datamanager.data")
+        config.pipeline.datamanager.data = config.data
 
-    if config.trainer.load_config:
-        CONSOLE.log(f"Loading pre-set config from: {config.trainer.load_config}")
-        config = yaml.load(config.trainer.load_config.read_text(), Loader=yaml.Loader)
+    if config.load_config:
+        CONSOLE.log(f"Loading pre-set config from: {config.load_config}")
+        config = yaml.load(config.load_config.read_text(), Loader=yaml.Loader)
 
     # print and save config
     config.print_to_terminal()
     config.save_config()
 
     launch(
         main_func=train_loop,
```

