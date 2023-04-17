# Comparing `tmp/tfimm-0.2.8.tar.gz` & `tmp/tfimm-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfimm-0.2.8.tar", max compression
+gzip compressed data, was "tfimm-0.2.9.tar", max compression
```

## Comparing `tfimm-0.2.8.tar` & `tfimm-0.2.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     2062 2022-09-05 12:02:42.440267 tfimm-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0    11343 2022-09-05 12:02:42.440267 tfimm-0.2.8/LICENSE
--rw-r--r--   0        0        0     9841 2022-09-05 12:02:42.440267 tfimm-0.2.8/README.md
--rw-r--r--   0        0        0     2170 2022-09-05 12:02:42.444268 tfimm-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      375 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/__init__.py
--rw-r--r--   0        0        0      515 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/__init__.py
--rw-r--r--   0        0        0    17933 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/cait.py
--rw-r--r--   0        0        0     5624 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/convmixer.py
--rw-r--r--   0        0        0    20048 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/convnext.py
--rw-r--r--   0        0        0    47399 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/efficientnet.py
--rw-r--r--   0        0        0    18220 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/efficientnet_blocks.py
--rw-r--r--   0        0        0    10499 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/efficientnet_builder.py
--rw-r--r--   0        0        0    22036 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/mlp_mixer.py
--rw-r--r--   0        0        0    17359 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/pit.py
--rw-r--r--   0        0        0    14314 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/poolformer.py
--rw-r--r--   0        0        0    15597 2022-09-05 12:02:42.444268 tfimm-0.2.8/tfimm/architectures/pvt.py
--rw-r--r--   0        0        0    16564 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/pvt_v2.py
--rw-r--r--   0        0        0    50410 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/resnet.py
--rw-r--r--   0        0        0    18334 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/resnetv2.py
--rw-r--r--   0        0        0    22144 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/swin.py
--rw-r--r--   0        0        0      281 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/timm/__init__.py
--rw-r--r--   0        0        0    16047 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/timm/poolformer.py
--rw-r--r--   0        0        0    13215 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/timm/pvt.py
--rw-r--r--   0        0        0    17241 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/timm/pvt_v2.py
--rw-r--r--   0        0        0    33495 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/vit.py
--rw-r--r--   0        0        0     6341 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/architectures/vit_hybrid.py
--rw-r--r--   0        0        0      593 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/__init__.py
--rw-r--r--   0        0        0     4596 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/attention.py
--rw-r--r--   0        0        0     2145 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/blurpool.py
--rw-r--r--   0        0        0     2208 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/classifier.py
--rw-r--r--   0        0        0     6830 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/conv.py
--rw-r--r--   0        0        0     1322 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/drop.py
--rw-r--r--   0        0        0     2176 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/factory.py
--rw-r--r--   0        0        0     1144 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/initializers.py
--rw-r--r--   0        0        0     6131 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/norm.py
--rw-r--r--   0        0        0    13728 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/layers/transformers.py
--rw-r--r--   0        0        0      446 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/__init__.py
--rw-r--r--   0        0        0      158 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/config.py
--rw-r--r--   0        0        0     1541 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/embedding_model.py
--rw-r--r--   0        0        0    10146 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/factory.py
--rw-r--r--   0        0        0     6126 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/registry.py
--rw-r--r--   0        0        0     3069 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/models/serialization.py
--rw-r--r--   0        0        0     6253 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/README.md
--rw-r--r--   0        0        0     1246 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/__init__.py
--rw-r--r--   0        0        0    14804 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/config.py
--rw-r--r--   0        0        0       56 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/datasets/__init__.py
--rw-r--r--   0        0        0     2138 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/datasets/tfds.py
--rw-r--r--   0        0        0     2448 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/examples/cifar10.py
--rw-r--r--   0        0        0     1557 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/examples/config.yaml
--rw-r--r--   0        0        0     1515 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/interface.py
--rw-r--r--   0        0        0     5350 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/model.py
--rw-r--r--   0        0        0     6269 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/optimizers/optimizer.py
--rw-r--r--   0        0        0     3228 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/optimizers/schedules.py
--rw-r--r--   0        0        0      166 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/problems/__init__.py
--rw-r--r--   0        0        0    10016 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/problems/classification.py
--rw-r--r--   0        0        0     7356 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/problems/distillation.py
--rw-r--r--   0        0        0     1622 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/registry.py
--rw-r--r--   0        0        0      276 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/run_local.py
--rw-r--r--   0        0        0     2273 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/timekeeping.py
--rw-r--r--   0        0        0     3450 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/train.py
--rw-r--r--   0        0        0    10857 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/trainer.py
--rw-r--r--   0        0        0     5431 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/train/utils.py
--rw-r--r--   0        0        0      322 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/__init__.py
--rw-r--r--   0        0        0     2678 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/cache.py
--rw-r--r--   0        0        0      310 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/constants.py
--rw-r--r--   0        0        0      731 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/etc.py
--rw-r--r--   0        0        0     1855 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/flops.py
--rw-r--r--   0        0        0     6856 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/profile.py
--rw-r--r--   0        0        0     9490 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/utils/timm.py
--rw-r--r--   0        0        0       22 2022-09-05 12:02:42.448268 tfimm-0.2.8/tfimm/version.py
--rw-r--r--   0        0        0    11308 2022-09-05 12:03:31.691116 tfimm-0.2.8/setup.py
--rw-r--r--   0        0        0    11473 2022-09-05 12:03:31.692281 tfimm-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2124 2022-10-28 09:33:14.937411 tfimm-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0    11343 2022-10-28 09:33:14.937411 tfimm-0.2.9/LICENSE
+-rw-r--r--   0        0        0     9841 2022-10-28 09:33:14.937411 tfimm-0.2.9/README.md
+-rw-r--r--   0        0        0     2170 2022-10-28 09:33:14.941411 tfimm-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      375 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/__init__.py
+-rw-r--r--   0        0        0      515 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/__init__.py
+-rw-r--r--   0        0        0    17933 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/cait.py
+-rw-r--r--   0        0        0     5624 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/convmixer.py
+-rw-r--r--   0        0        0    20048 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/convnext.py
+-rw-r--r--   0        0        0    47399 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/efficientnet.py
+-rw-r--r--   0        0        0    18220 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/efficientnet_blocks.py
+-rw-r--r--   0        0        0    10499 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/efficientnet_builder.py
+-rw-r--r--   0        0        0    22036 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/mlp_mixer.py
+-rw-r--r--   0        0        0    17359 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/pit.py
+-rw-r--r--   0        0        0    14314 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/poolformer.py
+-rw-r--r--   0        0        0    15597 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/pvt.py
+-rw-r--r--   0        0        0    16564 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/pvt_v2.py
+-rw-r--r--   0        0        0    50410 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/resnet.py
+-rw-r--r--   0        0        0    18334 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/resnetv2.py
+-rw-r--r--   0        0        0    22144 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/swin.py
+-rw-r--r--   0        0        0      281 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/timm/__init__.py
+-rw-r--r--   0        0        0    16047 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/timm/poolformer.py
+-rw-r--r--   0        0        0    13215 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/timm/pvt.py
+-rw-r--r--   0        0        0    17241 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/timm/pvt_v2.py
+-rw-r--r--   0        0        0    34122 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/vit.py
+-rw-r--r--   0        0        0     6341 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/architectures/vit_hybrid.py
+-rw-r--r--   0        0        0      593 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/layers/__init__.py
+-rw-r--r--   0        0        0     4596 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/layers/attention.py
+-rw-r--r--   0        0        0     2145 2022-10-28 09:33:14.941411 tfimm-0.2.9/tfimm/layers/blurpool.py
+-rw-r--r--   0        0        0     2208 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/classifier.py
+-rw-r--r--   0        0        0     6830 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/conv.py
+-rw-r--r--   0        0        0     1322 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/drop.py
+-rw-r--r--   0        0        0     2176 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/factory.py
+-rw-r--r--   0        0        0     1144 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/initializers.py
+-rw-r--r--   0        0        0     6131 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/norm.py
+-rw-r--r--   0        0        0    13728 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/layers/transformers.py
+-rw-r--r--   0        0        0      446 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/__init__.py
+-rw-r--r--   0        0        0      158 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/config.py
+-rw-r--r--   0        0        0     1541 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/embedding_model.py
+-rw-r--r--   0        0        0    10146 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/factory.py
+-rw-r--r--   0        0        0     6126 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/registry.py
+-rw-r--r--   0        0        0     3069 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/models/serialization.py
+-rw-r--r--   0        0        0     6253 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/README.md
+-rw-r--r--   0        0        0     1246 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/__init__.py
+-rw-r--r--   0        0        0    14804 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/config.py
+-rw-r--r--   0        0        0       56 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/datasets/__init__.py
+-rw-r--r--   0        0        0     2138 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/datasets/tfds.py
+-rw-r--r--   0        0        0     2448 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/examples/cifar10.py
+-rw-r--r--   0        0        0     1557 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/examples/config.yaml
+-rw-r--r--   0        0        0     1515 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/interface.py
+-rw-r--r--   0        0        0     5350 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/model.py
+-rw-r--r--   0        0        0     6269 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/optimizers/optimizer.py
+-rw-r--r--   0        0        0     3228 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/optimizers/schedules.py
+-rw-r--r--   0        0        0      166 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/problems/__init__.py
+-rw-r--r--   0        0        0    10016 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/problems/classification.py
+-rw-r--r--   0        0        0     7356 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/problems/distillation.py
+-rw-r--r--   0        0        0     1622 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/registry.py
+-rw-r--r--   0        0        0      276 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/run_local.py
+-rw-r--r--   0        0        0     2273 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/timekeeping.py
+-rw-r--r--   0        0        0     3450 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/train.py
+-rw-r--r--   0        0        0    10857 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/trainer.py
+-rw-r--r--   0        0        0     5431 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/train/utils.py
+-rw-r--r--   0        0        0      322 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/__init__.py
+-rw-r--r--   0        0        0     2678 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/cache.py
+-rw-r--r--   0        0        0      310 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/constants.py
+-rw-r--r--   0        0        0      731 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/etc.py
+-rw-r--r--   0        0        0     1855 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/flops.py
+-rw-r--r--   0        0        0     6856 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/profile.py
+-rw-r--r--   0        0        0     9490 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/utils/timm.py
+-rw-r--r--   0        0        0       22 2022-10-28 09:33:14.945412 tfimm-0.2.9/tfimm/version.py
+-rw-r--r--   0        0        0    11308 2022-10-28 09:33:51.355487 tfimm-0.2.9/setup.py
+-rw-r--r--   0        0        0    11473 2022-10-28 09:33:51.356685 tfimm-0.2.9/PKG-INFO
```

### Comparing `tfimm-0.2.8/CHANGELOG.md` & `tfimm-0.2.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change Log
 
+## v0.2.9 - 22-10-28
+
+- Exposed attention map in ViT models.
+
 ## v0.2.8 - 2022-09-05
 
 - `tfimm` now supports python 3.10.
 
 ## v0.2.7 - 2022-06-14
 
 - Added EfficinentNet and MobileNet-V2 models.
```

### Comparing `tfimm-0.2.8/LICENSE` & `tfimm-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/README.md` & `tfimm-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/pyproject.toml` & `tfimm-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tfimm"
-version = "0.2.8"
+version = "0.2.9"
 description = "TensorFlow port of PyTorch Image Models (timm) - image models with pretrained weights"
 authors = ["Martins Bruveris <martins.bruveris@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/martinsbruveris/tensorflow-image-models"
 repository = "https://github.com/martinsbruveris/tensorflow-image-models"
 keywords = ["tensorfow", "pretrained models", "visual transformer"]
```

### Comparing `tfimm-0.2.8/tfimm/architectures/__init__.py` & `tfimm-0.2.9/tfimm/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/cait.py` & `tfimm-0.2.9/tfimm/architectures/cait.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/convmixer.py` & `tfimm-0.2.9/tfimm/architectures/convmixer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/convnext.py` & `tfimm-0.2.9/tfimm/architectures/convnext.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/efficientnet.py` & `tfimm-0.2.9/tfimm/architectures/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/efficientnet_blocks.py` & `tfimm-0.2.9/tfimm/architectures/efficientnet_blocks.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/efficientnet_builder.py` & `tfimm-0.2.9/tfimm/architectures/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/mlp_mixer.py` & `tfimm-0.2.9/tfimm/architectures/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/pit.py` & `tfimm-0.2.9/tfimm/architectures/pit.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/poolformer.py` & `tfimm-0.2.9/tfimm/architectures/poolformer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/pvt.py` & `tfimm-0.2.9/tfimm/architectures/pvt.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/pvt_v2.py` & `tfimm-0.2.9/tfimm/architectures/pvt_v2.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/resnet.py` & `tfimm-0.2.9/tfimm/architectures/resnet.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/resnetv2.py` & `tfimm-0.2.9/tfimm/architectures/resnetv2.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/swin.py` & `tfimm-0.2.9/tfimm/architectures/swin.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/timm/poolformer.py` & `tfimm-0.2.9/tfimm/architectures/timm/poolformer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/timm/pvt.py` & `tfimm-0.2.9/tfimm/architectures/timm/pvt.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/timm/pvt_v2.py` & `tfimm-0.2.9/tfimm/architectures/timm/pvt_v2.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/architectures/vit.py` & `tfimm-0.2.9/tfimm/architectures/vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 TensorFlow implementation of the Visual Transformer
 
 Based on timm/models/visual_transformer.py by Ross Wightman.
 Based on transformers/models/vit by HuggingFace
 
 Copyright 2021 Martins Bruveris
 """
+from collections import OrderedDict
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Union
 
 import tensorflow as tf
 
 from tfimm.layers import (
     MLP,
@@ -141,34 +142,37 @@
         self.qkv = tf.keras.layers.Dense(
             units=3 * embed_dim, use_bias=qkv_bias, name="qkv"
         )
         self.attn_drop = tf.keras.layers.Dropout(rate=attn_drop_rate)
         self.proj = tf.keras.layers.Dense(units=embed_dim, name="proj")
         self.proj_drop = tf.keras.layers.Dropout(rate=drop_rate)
 
-    def call(self, x, training=False):
+    def call(self, x, training=False, return_features=False):
+        features = OrderedDict()
+
         # B (batch size), N (sequence length), D (embedding dimension),
         # H (number of heads)
         batch_size, seq_length = tf.unstack(tf.shape(x)[:2])
         qkv = self.qkv(x)  # (B, N, 3*D)
         qkv = tf.reshape(qkv, (batch_size, seq_length, 3, self.nb_heads, -1))
         qkv = tf.transpose(qkv, (2, 0, 3, 1, 4))  # (3, B, H, N, D/H)
         q, k, v = qkv[0], qkv[1], qkv[2]
 
         attn = self.scale * tf.linalg.matmul(q, k, transpose_b=True)  # (B, H, N, N)
         attn = tf.nn.softmax(attn, axis=-1)  # (B, H, N, N)
         attn = self.attn_drop(attn, training=training)
+        features["attn"] = attn
 
         x = tf.linalg.matmul(attn, v)  # (B, H, N, D/H)
         x = tf.transpose(x, (0, 2, 1, 3))  # (B, N, H, D/H)
         x = tf.reshape(x, (batch_size, seq_length, -1))  # (B, N, D)
 
         x = self.proj(x)
         x = self.proj_drop(x, training=training)
-        return x
+        return (x, features) if return_features else x
 
 
 class ViTBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         embed_dim: int,
         nb_heads: int,
@@ -208,27 +212,31 @@
             hidden_dim=int(embed_dim * mlp_ratio),
             embed_dim=embed_dim,
             drop_rate=drop_rate,
             act_layer=act_layer,
             name="mlp",
         )
 
-    def call(self, x, training=False):
+    def call(self, x, training=False, return_features=False):
+        features = OrderedDict()
         shortcut = x
         x = self.norm1(x, training=training)
-        x = self.attn(x, training=training)
+        x = self.attn(x, training=training, return_features=return_features)
+        if return_features:
+            x, mha_features = x
+            features["attn"] = mha_features["attn"]
         x = self.drop_path(x, training=training)
         x = x + shortcut
 
         shortcut = x
         x = self.norm2(x, training=training)
         x = self.mlp(x, training=training)
         x = self.drop_path(x, training=training)
         x = x + shortcut
-        return x
+        return (x, features) if return_features else x
 
 
 class HybridEmbeddings(tf.keras.layers.Layer):
     """
     CNN feature map embedding
 
     Extract feature map from CNN, flatten, project to embedding dim.
@@ -393,30 +401,30 @@
 
     @property
     def dummy_inputs(self) -> tf.Tensor:
         return tf.zeros((1, *self.cfg.input_size, self.cfg.in_channels))
 
     @property
     def feature_names(self) -> List[str]:
-        return (
-            ["patch_embedding"]
-            + [f"block_{j}" for j in range(self.cfg.nb_blocks)]
-            + ["features_all", "features", "logits"]
-        )
+        """
+        Names of features, returned when calling ``call`` with ``return_features=True``.
+        """
+        _, features = self(self.dummy_inputs, return_features=True)
+        return list(features.keys())
 
     def transform_pos_embed(self, target_cfg: ViTConfig):
         return interpolate_pos_embeddings(
             pos_embed=self.pos_embed,
             src_grid_size=self.cfg.grid_size,
             tgt_grid_size=target_cfg.grid_size,
             nb_tokens=self.cfg.nb_tokens,
         )
 
     def forward_features(self, x, training=False, return_features=False):
-        features = {}
+        features = OrderedDict()
         batch_size = tf.shape(x)[0]
 
         x, grid_size = self.patch_embed(x, return_shape=True)
         cls_token = tf.repeat(self.cls_token, repeats=batch_size, axis=0)
         if not self.cfg.distilled:
             x = tf.concat((cls_token, x), axis=1)
         else:
@@ -432,15 +440,18 @@
                 nb_tokens=self.cfg.nb_tokens,
             )
             x = x + pos_embed
         x = self.pos_drop(x, training=training)
         features["patch_embedding"] = x
 
         for j, block in enumerate(self.blocks):
-            x = block(x, training=training)
+            x = block(x, training=training, return_features=return_features)
+            if return_features:
+                x, block_features = x
+                features[f"block_{j}/attn"] = block_features["attn"]
             features[f"block_{j}"] = x
         x = self.norm(x, training=training)
         features["features_all"] = x
 
         if self.cfg.distilled:
             # Here we diverge from timm and return both outputs as one tensor. That way
             # all models always have one output by default
```

### Comparing `tfimm-0.2.8/tfimm/architectures/vit_hybrid.py` & `tfimm-0.2.9/tfimm/architectures/vit_hybrid.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/__init__.py` & `tfimm-0.2.9/tfimm/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/attention.py` & `tfimm-0.2.9/tfimm/layers/attention.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/blurpool.py` & `tfimm-0.2.9/tfimm/layers/blurpool.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/classifier.py` & `tfimm-0.2.9/tfimm/layers/classifier.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/conv.py` & `tfimm-0.2.9/tfimm/layers/conv.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/drop.py` & `tfimm-0.2.9/tfimm/layers/drop.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/factory.py` & `tfimm-0.2.9/tfimm/layers/factory.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/initializers.py` & `tfimm-0.2.9/tfimm/layers/initializers.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/norm.py` & `tfimm-0.2.9/tfimm/layers/norm.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/layers/transformers.py` & `tfimm-0.2.9/tfimm/layers/transformers.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/models/embedding_model.py` & `tfimm-0.2.9/tfimm/models/embedding_model.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/models/factory.py` & `tfimm-0.2.9/tfimm/models/factory.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/models/registry.py` & `tfimm-0.2.9/tfimm/models/registry.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/models/serialization.py` & `tfimm-0.2.9/tfimm/models/serialization.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/README.md` & `tfimm-0.2.9/tfimm/train/README.md`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/__init__.py` & `tfimm-0.2.9/tfimm/train/__init__.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/config.py` & `tfimm-0.2.9/tfimm/train/config.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/datasets/tfds.py` & `tfimm-0.2.9/tfimm/train/datasets/tfds.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/examples/cifar10.py` & `tfimm-0.2.9/tfimm/train/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/examples/config.yaml` & `tfimm-0.2.9/tfimm/train/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/interface.py` & `tfimm-0.2.9/tfimm/train/interface.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/model.py` & `tfimm-0.2.9/tfimm/train/model.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/optimizers/optimizer.py` & `tfimm-0.2.9/tfimm/train/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/optimizers/schedules.py` & `tfimm-0.2.9/tfimm/train/optimizers/schedules.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/problems/classification.py` & `tfimm-0.2.9/tfimm/train/problems/classification.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/problems/distillation.py` & `tfimm-0.2.9/tfimm/train/problems/distillation.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/registry.py` & `tfimm-0.2.9/tfimm/train/registry.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/timekeeping.py` & `tfimm-0.2.9/tfimm/train/timekeeping.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/train.py` & `tfimm-0.2.9/tfimm/train/train.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/trainer.py` & `tfimm-0.2.9/tfimm/train/trainer.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/train/utils.py` & `tfimm-0.2.9/tfimm/train/utils.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/utils/cache.py` & `tfimm-0.2.9/tfimm/utils/cache.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/utils/etc.py` & `tfimm-0.2.9/tfimm/utils/etc.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/utils/flops.py` & `tfimm-0.2.9/tfimm/utils/flops.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/utils/profile.py` & `tfimm-0.2.9/tfimm/utils/profile.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/tfimm/utils/timm.py` & `tfimm-0.2.9/tfimm/utils/timm.py`

 * *Files identical despite different names*

### Comparing `tfimm-0.2.8/setup.py` & `tfimm-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 extras_require = \
 {'docs': ['sphinx', 'sphinx-rtd-theme'],
  'timm': ['pyyaml'],
  'timm:python_version < "3.10"': ['timm']}
 
 setup_kwargs = {
     'name': 'tfimm',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'TensorFlow port of PyTorch Image Models (timm) - image models with pretrained weights',
     'long_description': '# TensorFlow Image Models\n\n![Test Status](https://github.com/martinsbruveris/tensorflow-image-models/actions/workflows/tests.yml/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/tfimm/badge/?version=latest)](https://tfimm.readthedocs.io/en/latest/?badge=latest)\n[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)](https://join.slack.com/t/tfimm/shared_invite/zt-13dnaf3qo-5JJaCBFIQhugeBXBT3NK8A)\n\n- [Introduction](#introduction)\n- [Usage](#usage)\n- [Models](#models)\n- [Profiling](#profiling)\n- [License](#license)\n- [Contact](#contact)\n\n## Introduction\n\nTensorFlow Image Models (`tfimm`) is a collection of image models with pretrained\nweights, obtained by porting architectures from \n[timm](https://github.com/rwightman/pytorch-image-models) to TensorFlow. The hope is\nthat the number of available architectures will grow over time. For now, it contains\nvision transformers (ViT, DeiT, CaiT, PVT and Swin Transformers), MLP-Mixer models \n(MLP-Mixer, ResMLP, gMLP, PoolFormer and ConvMixer), various ResNet flavours (ResNet,\nResNeXt, ECA-ResNet, SE-ResNet), the EfficientNet family (including AdvProp, \nNoisyStudent, Edge-TPU, V2 and Lite versions), MobileNet-V2, as well as the recent \nConvNeXt.\n\nThis work would not have been possible wihout Ross Wightman\'s `timm` library and the\nwork on PyTorch/TensorFlow interoperability in HuggingFace\'s `transformer` repository.\nI tried to make sure all source material is acknowledged. Please let me know if I have\nmissed something.\n\n## Usage\n\n### Installation \n\nThe package can be installed via `pip`,\n\n```shell\npip install tfimm\n```\n\nTo load pretrained weights, `timm` needs to be installed separately.\n\n### Creating models\n\nTo load pretrained models use\n\n```python\nimport tfimm\n\nmodel = tfimm.create_model("vit_tiny_patch16_224", pretrained="timm")\n```\n\nWe can list available models with pretrained weights via\n\n```python\nimport tfimm\n\nprint(tfimm.list_models(pretrained="timm"))\n```\n\nMost models are pretrained on ImageNet or ImageNet-21k. If we want to use them for other\ntasks we need to change the number of classes in the classifier or remove the \nclassifier altogether. We can do this by setting the `nb_classes` parameter in \n`create_model`. If `nb_classes=0`, the model will have no classification layer. If\n`nb_classes` is set to a value different from the default model config, the \nclassification layer will be randomly initialized, while all other weights will be\ncopied from the pretrained model.\n\nThe preprocessing function for each model can be created via\n```python\nimport tensorflow as tf\nimport tfimm\n\npreprocess = tfimm.create_preprocessing("vit_tiny_patch16_224", dtype="float32")\nimg = tf.ones((1, 224, 224, 3), dtype="uint8")\nimg_preprocessed = preprocess(img)\n```\n\n### Saving and loading models\n\nAll models are subclassed from `tf.keras.Model` (they are _not_ functional models).\nThey can still be saved and loaded using the `SavedModel` format.\n\n```\n>>> import tesnorflow as tf\n>>> import tfimm\n>>> model = tfimm.create_model("vit_tiny_patch16_224")\n>>> type(model)\n<class \'tfimm.architectures.vit.ViT\'>\n>>> model.save("/tmp/my_model")\n>>> loaded_model = tf.keras.models.load_model("/tmp/my_model")\n>>> type(loaded_model)\n<class \'tfimm.architectures.vit.ViT\'>\n```\n\nFor this to work, the `tfimm` library needs to be imported before the model is loaded,\nsince during the import process, `tfimm` is registering custom models with Keras.\nOtherwise, we obtain the following output\n\n```\n>>> import tensorflow as tf\n>>> loaded_model = tf.keras.models.load_model("/tmp/my_model")\n>>> type(loaded_model)\n<class \'keras.saving.saved_model.load.Custom>ViT\'>\n```\n\n## Models\n\nThe following architectures are currently available:\n\n- CaiT (vision transformer) \n  [\\[github\\]](https://github.com/facebookresearch/deit/blob/main/README_cait.md)\n  - Going deeper with Image Transformers \n    [\\[arXiv:2103.17239\\]](https://arxiv.org/abs/2103.17239)\n- DeiT (vision transformer) \n  [\\[github\\]](https://github.com/facebookresearch/deit)\n  - Training data-efficient image transformers & distillation through attention. \n    [\\[arXiv:2012.12877\\]](https://arxiv.org/abs/2012.12877) \n- ViT (vision transformer) \n  [\\[github\\]](https://github.com/google-research/vision_transformer)\n  - An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale.\n    [\\[arXiv:2010.11929\\]](https://arxiv.org/abs/2010.11929)\n  - How to train your ViT? Data, Augmentation, and Regularization in Vision \n    Transformers. [\\[arXiv:2106.10270\\]](https://arxiv.org/abs/2106.10270)\n  - Includes models trained with the SAM optimizer: Sharpness-Aware Minimization for \n    Efficiently Improving Generalization. \n    [\\[arXiv:2010.01412\\]](https://arxiv.org/abs/2010.01412)\n  - Includes models from: ImageNet-21K Pretraining for the Masses\n    [\\[arXiv:2104.10972\\]](https://arxiv.org/abs/2104.10972) \n    [\\[github\\]](https://github.com/Alibaba-MIIL/ImageNet21K)\n- Swin Transformer \n  [\\[github\\]](https://github.com/microsoft/Swin-Transformer)\n  - Swin Transformer: Hierarchical Vision Transformer using Shifted Windows. \n    [\\[arXiv:2103.14030\\]](https://arxiv.org/abs/2103.14030)\n  - Tensorflow code adapted from \n    [Swin-Transformer-TF](https://github.com/rishigami/Swin-Transformer-TF)\n- MLP-Mixer and friends\n  - MLP-Mixer: An all-MLP Architecture for Vision \n    [\\[arXiv:2105.01601\\]](https://arxiv.org/abs/2105.01601)\n  - ResMLP: Feedforward networks for image classification... \n    [\\[arXiv:2105.03404\\]](https://arxiv.org/abs/2105.03404)\n  - Pay Attention to MLPs (gMLP)\n    [\\[arXiv:2105.08050\\]](https://arxiv.org/abs/2105.08050)\n- ConvMixer \n  [\\[github\\]](https://github.com/tmp-iclr/convmixer)\n  - Patches Are All You Need? \n    [\\[ICLR 2022 submission\\]](https://openreview.net/forum?id=TVHS5Y4dNvM)\n- EfficientNet family\n  - EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks\n    [\\[arXiv:1905.11946\\]](https://arxiv.org/abs/1905.11946)\n  - Adversarial Examples Improve Image Recognition\n    [\\[arXiv:1911.09665\\]](https://arxiv.org/abs/1911.09665)\n  - Self-training with Noisy Student improves ImageNet classification\n    [\\[arXiv:1911.04252\\]](https://arxiv.org/abs/1911.04252)\n  - EfficientNet-EdgeTPU\n    [\\[Blog\\]](https://ai.googleblog.com/2019/08/efficientnet-edgetpu-creating.html)\n  - EfficientNet-Lite\n    [\\[Blog\\]](https://blog.tensorflow.org/2020/03/higher-accuracy-on-vision-models-with-efficientnet-lite.html)\n  - EfficientNetV2: Smaller Models and Faster Training\n    [\\[arXiv:2104.00298\\]](https://arxiv.org/abs/2104.00298)\n- MobileNet-V2\n  - MobileNetV2: Inverted Residuals and Linear Bottlenecks\n    [\\[arXiv:1801.04381\\]](https://arxiv.org/abs/1801.04381)\n- Pyramid Vision Transformer \n  [\\[github\\]](https://github.com/whai362/PVT)\n  - Pyramid Vision Transformer: A Versatile Backbone for Dense Prediction without\n    Convolutions. [\\[arXiv:2102.12122\\]](https://arxiv.org/abs/2102.12122)\n  - PVTv2: Improved Baselines with Pyramid Vision Transformer \n    [\\[arXiv:2106.13797\\]](https://arxiv.org/abs/2106.13797)\n- ConvNeXt\n  [\\[github\\]](https://github.com/facebookresearch/ConvNeXt)\n  - A ConvNet for the 2020s. [\\[arXiv:2201.03545\\]](https://arxiv.org/abs/2201.03545)\n- PoolFormer\n  [\\[github\\]](https://github.com/sail-sg/poolformer)\n  - PoolFormer: MetaFormer is Actually What You Need for Vision.\n    [\\[arXiv:2111.11418\\]](https://arxiv.org/abs/2111.11418)\n- Pooling-based Vision Transformers (PiT)\n  - Rethinking Spatial Dimensions of Vision Transformers.\n    [\\[arXiv:2103.16302\\]](https://arxiv.org/abs/2103.16302)\n- ResNet, ResNeXt, ECA-ResNet, SE-ResNet and friends\n  - Deep Residual Learning for Image Recognition. \n    [\\[arXiv:1512.03385\\]](https://arxiv.org/abs/1512.03385)\n  - Exploring the Limits of Weakly Supervised Pretraining. \n    [\\[arXiv:1805.00932\\]](https://arxiv.org/abs/1805.00932)\n  - Billion-scale Semi-Supervised Learning for Image Classification. \n    [\\[arXiv:1905.00546\\]](https://arxiv.org/abs/1905.00546)\n  - ECA-Net: Efficient Channel Attention for Deep Convolutional Neural Networks. \n    [\\[arXiv1910.03151\\]](https://arxiv.org/abs/1910.03151)\n  - Revisiting ResNets. [\\[arXiv:2103.07579\\]](https://arxiv.org/abs/2103.07579)\n  - Making Convolutional Networks Shift-Invariant Again. (anti-aliasing layer)\n    [\\[arXiv:1904.11486\\]](https://arxiv.org/abs/1904.11486)\n  - Squeeze-and-Excitation Networks. \n    [\\[arXiv:1709.01507\\]](https://arxiv.org/abs/1709.01507)\n  - Big Transfer (BiT): General Visual Representation Learning\n    [\\[arXiv:1912.11370\\]](https://arxiv.org/abs/1912.11370)\n  - Knowledge distillation: A good teacher is patient and consistent\n    [\\[arXiv:2106:05237\\]](https://arxiv.org/abs/2106.05237)\n\n## Profiling\n\nTo understand how big each of the models is, I have done some profiling to measure\n- maximum batch size that fits in GPU memory and\n- throughput in images/second\nfor both inference and backpropagation on K80 and V100 GPUs. For V100, measurements \nwere done for both `float32` and mixed precision.\n\nThe results can be found in the `results/profiling_{k80, v100}.csv` files.\n\nFor backpropagation, we use as loss the mean of model outputs\n\n```python\ndef backprop():\n    with tf.GradientTape() as tape:\n        output = model(x, training=True)\n        loss = tf.reduce_mean(output)\n        grads = tape.gradient(loss, model.trainable_variables)\n    optimizer.apply_gradients(zip(grads, model.trainable_variables))\n```\n\n## License\n\nThis repository is released under the Apache 2.0 license as found in the \n[LICENSE](LICENSE) file.\n\n## Contact\n\nAll things related to `tfimm` can be discussed via \n[Slack](https://join.slack.com/t/tfimm/shared_invite/zt-13dnaf3qo-5JJaCBFIQhugeBXBT3NK8A).',
     'author': 'Martins Bruveris',
     'author_email': 'martins.bruveris@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/martinsbruveris/tensorflow-image-models',
```

### Comparing `tfimm-0.2.8/PKG-INFO` & `tfimm-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfimm
-Version: 0.2.8
+Version: 0.2.9
 Summary: TensorFlow port of PyTorch Image Models (timm) - image models with pretrained weights
 Home-page: https://github.com/martinsbruveris/tensorflow-image-models
 License: Apache-2.0
 Keywords: tensorfow,pretrained models,visual transformer
 Author: Martins Bruveris
 Author-email: martins.bruveris@gmail.com
 Requires-Python: >=3.7,<3.11
```

