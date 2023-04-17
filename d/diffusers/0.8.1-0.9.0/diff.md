# Comparing `tmp/diffusers-0.8.1.tar.gz` & `tmp/diffusers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusers-0.8.1.tar", last modified: Thu Nov 24 00:00:06 2022, max compression
+gzip compressed data, was "diffusers-0.9.0.tar", last modified: Fri Nov 25 16:49:02 2022, max compression
```

## Comparing `diffusers-0.8.1.tar` & `diffusers-0.9.0.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.670988 diffusers-0.8.1/
--rw-rw-r--   0 anton     (1000) anton     (1000)    11357 2022-11-20 22:38:47.000000 diffusers-0.8.1/LICENSE
--rw-rw-r--   0 anton     (1000) anton     (1000)       67 2022-11-20 22:38:47.000000 diffusers-0.8.1/MANIFEST.in
--rw-rw-r--   0 anton     (1000) anton     (1000)    29177 2022-11-24 00:00:06.670988 diffusers-0.8.1/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)    28133 2022-11-21 11:33:32.000000 diffusers-0.8.1/README.md
--rw-rw-r--   0 anton     (1000) anton     (1000)       57 2022-11-20 22:38:47.000000 diffusers-0.8.1/pyproject.toml
--rw-rw-r--   0 anton     (1000) anton     (1000)      440 2022-11-24 00:00:06.670988 diffusers-0.8.1/setup.cfg
--rw-rw-r--   0 anton     (1000) anton     (1000)     9703 2022-11-23 23:11:37.000000 diffusers-0.8.1/setup.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/diffusers/
--rw-rw-r--   0 anton     (1000) anton     (1000)     3796 2022-11-23 23:12:03.000000 diffusers-0.8.1/src/diffusers/__init__.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/diffusers/commands/
--rw-rw-r--   0 anton     (1000) anton     (1000)      920 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/commands/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     1200 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/commands/diffusers_cli.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     2384 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/commands/env.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    27156 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/configuration_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     1756 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/dependency_versions_check.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     1056 2022-11-23 17:27:43.000000 diffusers-0.8.1/src/diffusers/dependency_versions_table.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    18265 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/dynamic_modules_utils.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/diffusers/experimental/
--rw-rw-r--   0 anton     (1000) anton     (1000)       38 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/experimental/__init__.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/diffusers/experimental/rl/
--rw-rw-r--   0 anton     (1000) anton     (1000)       57 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/experimental/rl/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4966 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/experimental/rl/value_guided_sampling.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     9381 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/hub_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4599 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/modeling_flax_pytorch_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    25838 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/modeling_flax_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    32084 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/modeling_utils.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/models/
--rw-rw-r--   0 anton     (1000) anton     (1000)     1046 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    36988 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/models/attention.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     9802 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/attention_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6530 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/embeddings.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     3392 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/embeddings_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    24780 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/resnet.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4021 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/resnet_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    10283 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/unet_1d.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    24857 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/unet_1d_blocks.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11619 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/models/unet_2d.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    59474 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/models/unet_2d_blocks.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12836 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/unet_2d_blocks_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    15913 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/models/unet_2d_condition.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12669 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/models/unet_2d_condition_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    22505 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/vae.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    31047 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/models/vae_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     8282 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/onnx_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11363 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/optimization.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    23215 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipeline_flax_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    34366 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipeline_utils.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/
--rw-rw-r--   0 anton     (1000) anton     (1000)     1860 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/__init__.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)     1347 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4673 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    26662 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    29058 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/dance_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)       76 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/dance_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5172 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/ddim/
--rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/ddim/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5713 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/ddim/pipeline_ddim.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/ddpm/
--rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/ddpm/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5572 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/ddpm/pipeline_ddpm.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)      258 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    30929 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     7288 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion_uncond/
--rw-rw-r--   0 anton     (1000) anton     (1000)       73 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion_uncond/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4801 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/pndm/
--rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/pndm/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4049 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/pndm/pipeline_pndm.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/repaint/
--rw-rw-r--   0 anton     (1000) anton     (1000)       46 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/repaint/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5897 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/repaint/pipeline_repaint.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/score_sde_ve/
--rw-rw-r--   0 anton     (1000) anton     (1000)       69 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/score_sde_ve/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4286 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)     3394 2022-11-23 23:56:10.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    33227 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    17160 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    15071 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    23224 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    24270 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    23012 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    26285 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    22015 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    29995 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    35568 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    30864 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5555 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/safety_checker.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4485 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/
--rw-rw-r--   0 anton     (1000) anton     (1000)     2503 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    35442 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5049 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.666988 diffusers-0.8.1/src/diffusers/pipelines/stochastic_karras_ve/
--rw-rw-r--   0 anton     (1000) anton     (1000)       75 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/stochastic_karras_ve/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     5604 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.670988 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)      883 2022-11-23 23:56:10.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    44014 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    24032 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    30894 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    23270 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    25156 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.670988 diffusers-0.8.1/src/diffusers/pipelines/vq_diffusion/
--rw-rw-r--   0 anton     (1000) anton     (1000)      226 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/vq_diffusion/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    16151 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.670988 diffusers-0.8.1/src/diffusers/schedulers/
--rw-rw-r--   0 anton     (1000) anton     (1000)     2362 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    15953 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddim.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12944 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddim_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    15101 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddpm.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    13114 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddpm_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    24358 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_dpmsolver_multistep.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    26847 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11797 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12009 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_euler_discrete.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6153 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_ipndm.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     9760 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_karras_ve.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     9600 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_karras_ve_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    11555 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_lms_discrete.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     8890 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_lms_discrete_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    18543 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_pndm.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    22654 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_pndm_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    13652 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_repaint.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12125 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_sde_ve.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12087 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_sde_ve_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     3317 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_sde_vp.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6845 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     7416 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_utils_flax.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    23768 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/schedulers/scheduling_vq_diffusion.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4110 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/training_utils.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.670988 diffusers-0.8.1/src/diffusers/utils/
--rw-rw-r--   0 anton     (1000) anton     (1000)     2428 2022-11-23 23:33:39.000000 diffusers-0.8.1/src/diffusers/utils/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     2069 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/deprecation_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)      584 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/dummy_flax_and_transformers_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     4587 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/dummy_flax_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    12101 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/dummy_pt_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)      553 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_scipy_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     2555 2022-11-21 11:33:32.000000 diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     6845 2022-11-23 23:10:37.000000 diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_transformers_objects.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    13381 2022-11-23 23:56:10.000000 diffusers-0.8.1/src/diffusers/utils/import_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     9413 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/logging.py
--rw-rw-r--   0 anton     (1000) anton     (1000)     1484 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/model_card_template.md
--rw-rw-r--   0 anton     (1000) anton     (1000)     3656 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/outputs.py
--rw-rw-r--   0 anton     (1000) anton     (1000)      665 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/pil_utils.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    13255 2022-11-20 22:38:47.000000 diffusers-0.8.1/src/diffusers/utils/testing_utils.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-24 00:00:06.662988 diffusers-0.8.1/src/diffusers.egg-info/
--rw-rw-r--   0 anton     (1000) anton     (1000)    29177 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)     6550 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/SOURCES.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)        1 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/dependency_links.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       72 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/entry_points.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)      795 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/requires.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       10 2022-11-24 00:00:06.000000 diffusers-0.8.1/src/diffusers.egg-info/top_level.txt
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.723243 diffusers-0.9.0/
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11357 2022-11-25 16:48:51.000000 diffusers-0.9.0/LICENSE
+-rw-rw-r--   0 anton     (1000) anton     (1000)       67 2022-11-25 16:48:51.000000 diffusers-0.9.0/MANIFEST.in
+-rw-rw-r--   0 anton     (1000) anton     (1000)    29177 2022-11-25 16:49:02.723243 diffusers-0.9.0/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)    28133 2022-11-25 16:48:51.000000 diffusers-0.9.0/README.md
+-rw-rw-r--   0 anton     (1000) anton     (1000)       57 2022-11-25 16:48:51.000000 diffusers-0.9.0/pyproject.toml
+-rw-rw-r--   0 anton     (1000) anton     (1000)      440 2022-11-25 16:49:02.723243 diffusers-0.9.0/setup.cfg
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9703 2022-11-25 16:48:51.000000 diffusers-0.9.0/setup.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.711243 diffusers-0.9.0/src/
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3836 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/__init__.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/commands/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      920 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/commands/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1200 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/commands/diffusers_cli.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2384 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/commands/env.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    27747 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/configuration_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1756 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/dependency_versions_check.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1056 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/dependency_versions_table.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    18265 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/dynamic_modules_utils.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/experimental/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       38 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/experimental/__init__.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/experimental/rl/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       57 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/experimental/rl/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5035 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/experimental/rl/value_guided_sampling.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9381 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/hub_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4599 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/modeling_flax_pytorch_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    25838 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/modeling_flax_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    32212 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/modeling_utils.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/models/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1046 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    38426 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/attention.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9802 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/attention_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     6530 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/embeddings.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3392 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/embeddings_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24780 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/resnet.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4021 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/resnet_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    10283 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_1d.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24857 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_1d_blocks.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11619 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_2d.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    60670 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_2d_blocks.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12836 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_2d_blocks_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    17399 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_2d_condition.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12669 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/unet_2d_condition_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    22505 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/vae.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    31047 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/models/vae_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     8282 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/onnx_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11363 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/optimization.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    23215 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipeline_flax_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    35455 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipeline_utils.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers/pipelines/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1900 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/__init__.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1347 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4673 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    29828 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    31860 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/dance_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       76 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/dance_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5172 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/ddim/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/ddim/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5713 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/ddim/pipeline_ddim.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/ddpm/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/ddpm/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5541 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/ddpm/pipeline_ddpm.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      258 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    31318 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     7288 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       73 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4801 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/pndm/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       55 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/pndm/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4049 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/pndm/pipeline_pndm.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/repaint/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       46 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/repaint/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5897 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/repaint/pipeline_repaint.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/score_sde_ve/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       69 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/score_sde_ve/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4286 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3476 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    35945 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    19542 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    16410 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    23799 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24866 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    25300 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    29451 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24981 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    32797 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    38796 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    33727 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    27122 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5555 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4485 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2503 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    38101 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5049 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/
+-rw-rw-r--   0 anton     (1000) anton     (1000)       75 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     5604 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      883 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    46826 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24527 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    31742 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    24004 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    25932 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.719243 diffusers-0.9.0/src/diffusers/pipelines/vq_diffusion/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      226 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/vq_diffusion/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    16151 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.723243 diffusers-0.9.0/src/diffusers/schedulers/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2362 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    17395 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddim.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    14410 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddim_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    15948 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddpm.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    13935 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddpm_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    25871 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    28393 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11797 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12494 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_euler_discrete.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     6153 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_ipndm.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9760 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_karras_ve.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9600 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    11555 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     8890 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    18543 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_pndm.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    22654 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_pndm_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    13652 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_repaint.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12125 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_ve.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12087 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_ve_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3317 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_vp.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     6845 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     7416 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_utils_flax.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    23768 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/schedulers/scheduling_vq_diffusion.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4110 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/training_utils.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.723243 diffusers-0.9.0/src/diffusers/utils/
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2428 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2064 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/deprecation_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)      584 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     4587 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_flax_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    12101 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_pt_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)      553 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     2555 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     7293 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_objects.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    13381 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/import_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     9413 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/logging.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)     1484 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/model_card_template.md
+-rw-rw-r--   0 anton     (1000) anton     (1000)     3656 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/outputs.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)      665 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/pil_utils.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    13255 2022-11-25 16:48:51.000000 diffusers-0.9.0/src/diffusers/utils/testing_utils.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-11-25 16:49:02.715243 diffusers-0.9.0/src/diffusers.egg-info/
+-rw-rw-r--   0 anton     (1000) anton     (1000)    29177 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)     6628 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/SOURCES.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)        1 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/dependency_links.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       72 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/entry_points.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)      795 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/requires.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       10 2022-11-25 16:49:02.000000 diffusers-0.9.0/src/diffusers.egg-info/top_level.txt
```

### Comparing `diffusers-0.8.1/LICENSE` & `diffusers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/PKG-INFO` & `diffusers-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusers
-Version: 0.8.1
+Version: 0.9.0
 Summary: Diffusers
 Home-page: https://github.com/huggingface/diffusers
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diffusers Version: 0.8.1 Summary: Diffusers Home-
+Metadata-Version: 2.1 Name: diffusers Version: 0.9.0 Summary: Diffusers Home-
 page: https://github.com/huggingface/diffusers Author: The HuggingFace team
 Author-email: patrick@huggingface.co License: Apache Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `diffusers-0.8.1/README.md` & `diffusers-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/setup.py` & `diffusers-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     deps["regex"],
     deps["requests"],
     deps["Pillow"],
 ]
 
 setup(
     name="diffusers",
-    version="0.8.1",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.9.0",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Diffusers",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `diffusers-0.8.1/src/diffusers/__init__.py` & `diffusers-0.9.0/src/diffusers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     is_scipy_available,
     is_torch_available,
     is_transformers_available,
     is_unidecode_available,
 )
 
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 from .configuration_utils import ConfigMixin
 from .onnx_utils import OnnxRuntimeModel
 from .utils import logging
 
 
 if is_torch_available():
@@ -71,14 +71,15 @@
         LDMTextToImagePipeline,
         StableDiffusionImageVariationPipeline,
         StableDiffusionImg2ImgPipeline,
         StableDiffusionInpaintPipeline,
         StableDiffusionInpaintPipelineLegacy,
         StableDiffusionPipeline,
         StableDiffusionPipelineSafe,
+        StableDiffusionUpscalePipeline,
         VersatileDiffusionDualGuidedPipeline,
         VersatileDiffusionImageVariationPipeline,
         VersatileDiffusionPipeline,
         VersatileDiffusionTextToImagePipeline,
         VQDiffusionPipeline,
     )
 else:
```

### Comparing `diffusers-0.8.1/src/diffusers/commands/__init__.py` & `diffusers-0.9.0/src/diffusers/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/commands/diffusers_cli.py` & `diffusers-0.9.0/src/diffusers/commands/diffusers_cli.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/commands/env.py` & `diffusers-0.9.0/src/diffusers/commands/env.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/configuration_utils.py` & `diffusers-0.9.0/src/diffusers/configuration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,29 @@
         - [`~ConfigMixin.from_config`]
         - [`~ConfigMixin.save_config`]
 
     Class attributes:
         - **config_name** (`str`) -- A filename under which the config should stored when calling
           [`~ConfigMixin.save_config`] (should be overridden by parent class).
         - **ignore_for_config** (`List[str]`) -- A list of attributes that should not be saved in the config (should be
-          overridden by parent class).
-        - **has_compatibles** (`bool`) -- Whether the class has compatible classes (should be overridden by parent
-          class).
+          overridden by subclass).
+        - **has_compatibles** (`bool`) -- Whether the class has compatible classes (should be overridden by subclass).
+        - **_deprecated_kwargs** (`List[str]`) -- Keyword arguments that are deprecated. Note that the init function
+          should only have a `kwargs` argument if at least one argument is deprecated (should be overridden by
+          subclass).
     """
     config_name = None
     ignore_for_config = []
     has_compatibles = False
 
+    _deprecated_kwargs = []
+
     def register_to_config(self, **kwargs):
         if self.config_name is None:
             raise NotImplementedError(f"Make sure that {self.__class__} has defined a class name `config_name`")
-        kwargs["_class_name"] = self.__class__.__name__
-        kwargs["_diffusers_version"] = __version__
-
         # Special case for `kwargs` used in deprecation warning added to schedulers
         # TODO: remove this when we remove the deprecation warning, and the `kwargs` argument,
         # or solve in a more general way.
         kwargs.pop("kwargs", None)
         for key, value in kwargs.items():
             try:
                 setattr(self, key, value)
@@ -194,14 +195,19 @@
 
         init_dict, unused_kwargs, hidden_dict = cls.extract_init_dict(config, **kwargs)
 
         # Allow dtype to be specified on initialization
         if "dtype" in unused_kwargs:
             init_dict["dtype"] = unused_kwargs.pop("dtype")
 
+        # add possible deprecated kwargs
+        for deprecated_kwarg in cls._deprecated_kwargs:
+            if deprecated_kwarg in unused_kwargs:
+                init_dict[deprecated_kwarg] = unused_kwargs.pop(deprecated_kwarg)
+
         # Return model and optionally state and/or unused_kwargs
         model = cls(**init_dict)
 
         # make sure to also save config parameters that might be used for compatible classes
         model.register_to_config(**hidden_dict)
 
         # add hidden kwargs of compatible classes to unused_kwargs
@@ -458,15 +464,15 @@
                 f"{expected_keys - passed_keys} was not found in config. Values will be initialized to default values."
             )
 
         # 6. Define unused keyword arguments
         unused_kwargs = {**config_dict, **kwargs}
 
         # 7. Define "hidden" config parameters that were saved for compatible classes
-        hidden_config_dict = {k: v for k, v in original_dict.items() if k not in init_dict and not k.startswith("_")}
+        hidden_config_dict = {k: v for k, v in original_dict.items() if k not in init_dict}
 
         return init_dict, unused_kwargs, hidden_config_dict
 
     @classmethod
     def _dict_from_json_file(cls, json_file: Union[str, os.PathLike]):
         with open(json_file, "r", encoding="utf-8") as reader:
             text = reader.read()
@@ -489,14 +495,17 @@
         """
         Serializes this instance to a JSON string.
 
         Returns:
             `str`: String containing all the attributes that make up this configuration instance in JSON format.
         """
         config_dict = self._internal_dict if hasattr(self, "_internal_dict") else {}
+        config_dict["_class_name"] = self.__class__.__name__
+        config_dict["_diffusers_version"] = __version__
+
         return json.dumps(config_dict, indent=2, sort_keys=True) + "\n"
 
     def to_json_file(self, json_file_path: Union[str, os.PathLike]):
         """
         Save this instance to a JSON file.
 
         Args:
@@ -516,15 +525,15 @@
     Warning: Once decorated, all private arguments (beginning with an underscore) are trashed and not sent to the init!
     """
 
     @functools.wraps(init)
     def inner_init(self, *args, **kwargs):
         # Ignore private kwargs in the init.
         init_kwargs = {k: v for k, v in kwargs.items() if not k.startswith("_")}
-        init(self, *args, **init_kwargs)
+        config_init_kwargs = {k: v for k, v in kwargs.items() if k.startswith("_")}
         if not isinstance(self, ConfigMixin):
             raise RuntimeError(
                 f"`@register_for_config` was applied to {self.__class__.__name__} init method, but this class does "
                 "not inherit from `ConfigMixin`."
             )
 
         ignore = getattr(self, "ignore_for_config", [])
@@ -541,15 +550,17 @@
         new_kwargs.update(
             {
                 k: init_kwargs.get(k, default)
                 for k, default in parameters.items()
                 if k not in ignore and k not in new_kwargs
             }
         )
+        new_kwargs = {**config_init_kwargs, **new_kwargs}
         getattr(self, "register_to_config")(**new_kwargs)
+        init(self, *args, **init_kwargs)
 
     return inner_init
 
 
 def flax_register_to_config(cls):
     original_init = cls.__init__
 
@@ -558,15 +569,15 @@
         if not isinstance(self, ConfigMixin):
             raise RuntimeError(
                 f"`@register_for_config` was applied to {self.__class__.__name__} init method, but this class does "
                 "not inherit from `ConfigMixin`."
             )
 
         # Ignore private kwargs in the init. Retrieve all passed attributes
-        init_kwargs = {k: v for k, v in kwargs.items() if not k.startswith("_")}
+        init_kwargs = {k: v for k, v in kwargs.items()}
 
         # Retrieve default values
         fields = dataclasses.fields(self)
         default_kwargs = {}
         for field in fields:
             # ignore flax specific attributes
             if field.name in self._flax_internal_args:
```

### Comparing `diffusers-0.8.1/src/diffusers/dependency_versions_check.py` & `diffusers-0.9.0/src/diffusers/dependency_versions_check.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/dependency_versions_table.py` & `diffusers-0.9.0/src/diffusers/dependency_versions_table.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/dynamic_modules_utils.py` & `diffusers-0.9.0/src/diffusers/dynamic_modules_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/experimental/rl/value_guided_sampling.py` & `diffusers-0.9.0/src/diffusers/experimental/rl/value_guided_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                     model_std = torch.exp(0.5 * posterior_variance)
                     grad = model_std * grad
                 grad[timesteps < 2] = 0
                 x = x.detach()
                 x = x + scale * grad
                 x = self.reset_x0(x, conditions, self.action_dim)
             prev_x = self.unet(x.permute(0, 2, 1), timesteps).sample.permute(0, 2, 1)
+            # TODO: set prediction_type when instantiating the model
             x = self.scheduler.step(prev_x, i, x, predict_epsilon=False)["prev_sample"]
 
             # apply conditions to the trajectory
             x = self.reset_x0(x, conditions, self.action_dim)
             x = self.to_torch(x)
         return x, y
```

### Comparing `diffusers-0.8.1/src/diffusers/hub_utils.py` & `diffusers-0.9.0/src/diffusers/hub_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/modeling_flax_pytorch_utils.py` & `diffusers-0.9.0/src/diffusers/modeling_flax_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/modeling_flax_utils.py` & `diffusers-0.9.0/src/diffusers/modeling_flax_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/modeling_utils.py` & `diffusers-0.9.0/src/diffusers/modeling_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,28 +444,29 @@
                 )
 
             # restore default dtype
 
         if low_cpu_mem_usage:
             # Instantiate model with empty weights
             with accelerate.init_empty_weights():
-                model, unused_kwargs = cls.from_config(
+                config, unused_kwargs = cls.load_config(
                     config_path,
                     cache_dir=cache_dir,
                     return_unused_kwargs=True,
                     force_download=force_download,
                     resume_download=resume_download,
                     proxies=proxies,
                     local_files_only=local_files_only,
                     use_auth_token=use_auth_token,
                     revision=revision,
                     subfolder=subfolder,
                     device_map=device_map,
                     **kwargs,
                 )
+                model = cls.from_config(config, **unused_kwargs)
 
             # if device_map is Non,e load the state dict on move the params from meta device to the cpu
             if device_map is None:
                 param_device = "cpu"
                 state_dict = load_state_dict(model_file)
                 # move the parms from meta device to cpu
                 for param_name, param in state_dict.items():
@@ -478,28 +479,29 @@
             loading_info = {
                 "missing_keys": [],
                 "unexpected_keys": [],
                 "mismatched_keys": [],
                 "error_msgs": [],
             }
         else:
-            model, unused_kwargs = cls.from_config(
+            config, unused_kwargs = cls.load_config(
                 config_path,
                 cache_dir=cache_dir,
                 return_unused_kwargs=True,
                 force_download=force_download,
                 resume_download=resume_download,
                 proxies=proxies,
                 local_files_only=local_files_only,
                 use_auth_token=use_auth_token,
                 revision=revision,
                 subfolder=subfolder,
                 device_map=device_map,
                 **kwargs,
             )
+            model = cls.from_config(config, **unused_kwargs)
 
             state_dict = load_state_dict(model_file)
             model, missing_keys, unexpected_keys, mismatched_keys, error_msgs = cls._load_pretrained_model(
                 model,
                 state_dict,
                 model_file,
                 pretrained_model_name_or_path,
```

### Comparing `diffusers-0.8.1/src/diffusers/models/__init__.py` & `diffusers-0.9.0/src/diffusers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/attention.py` & `diffusers-0.9.0/src/diffusers/models/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,19 @@
         norm_num_groups: int = 32,
         cross_attention_dim: Optional[int] = None,
         attention_bias: bool = False,
         sample_size: Optional[int] = None,
         num_vector_embeds: Optional[int] = None,
         activation_fn: str = "geglu",
         num_embeds_ada_norm: Optional[int] = None,
+        use_linear_projection: bool = False,
+        only_cross_attention: bool = False,
     ):
         super().__init__()
+        self.use_linear_projection = use_linear_projection
         self.num_attention_heads = num_attention_heads
         self.attention_head_dim = attention_head_dim
         inner_dim = num_attention_heads * attention_head_dim
 
         # 1. Transformer2DModel can process both standard continous images of shape `(batch_size, num_channels, width, height)` as well as quantized image embeddings of shape `(batch_size, num_image_vectors)`
         # Define whether input is continuous or discrete depending on configuration
         self.is_input_continuous = in_channels is not None
@@ -122,15 +125,18 @@
             )
 
         # 2. Define input layers
         if self.is_input_continuous:
             self.in_channels = in_channels
 
             self.norm = torch.nn.GroupNorm(num_groups=norm_num_groups, num_channels=in_channels, eps=1e-6, affine=True)
-            self.proj_in = nn.Conv2d(in_channels, inner_dim, kernel_size=1, stride=1, padding=0)
+            if use_linear_projection:
+                self.proj_in = nn.Linear(in_channels, inner_dim)
+            else:
+                self.proj_in = nn.Conv2d(in_channels, inner_dim, kernel_size=1, stride=1, padding=0)
         elif self.is_input_vectorized:
             assert sample_size is not None, "Transformer2DModel over discrete input must provide sample_size"
             assert num_vector_embeds is not None, "Transformer2DModel over discrete input must provide num_embed"
 
             self.height = sample_size
             self.width = sample_size
             self.num_vector_embeds = num_vector_embeds
@@ -148,22 +154,26 @@
                     num_attention_heads,
                     attention_head_dim,
                     dropout=dropout,
                     cross_attention_dim=cross_attention_dim,
                     activation_fn=activation_fn,
                     num_embeds_ada_norm=num_embeds_ada_norm,
                     attention_bias=attention_bias,
+                    only_cross_attention=only_cross_attention,
                 )
                 for d in range(num_layers)
             ]
         )
 
         # 4. Define output layers
         if self.is_input_continuous:
-            self.proj_out = nn.Conv2d(inner_dim, in_channels, kernel_size=1, stride=1, padding=0)
+            if use_linear_projection:
+                self.proj_out = nn.Linear(in_channels, inner_dim)
+            else:
+                self.proj_out = nn.Conv2d(inner_dim, in_channels, kernel_size=1, stride=1, padding=0)
         elif self.is_input_vectorized:
             self.norm_out = nn.LayerNorm(inner_dim)
             self.out = nn.Linear(inner_dim, self.num_vector_embeds - 1)
 
     def _set_attention_slice(self, slice_size):
         for block in self.transformer_blocks:
             block._set_attention_slice(slice_size)
@@ -187,29 +197,44 @@
             if `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample
             tensor.
         """
         # 1. Input
         if self.is_input_continuous:
             batch, channel, height, weight = hidden_states.shape
             residual = hidden_states
+
             hidden_states = self.norm(hidden_states)
-            hidden_states = self.proj_in(hidden_states)
-            inner_dim = hidden_states.shape[1]
-            hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(batch, height * weight, inner_dim)
+            if not self.use_linear_projection:
+                hidden_states = self.proj_in(hidden_states)
+                inner_dim = hidden_states.shape[1]
+                hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(batch, height * weight, inner_dim)
+            else:
+                inner_dim = hidden_states.shape[1]
+                hidden_states = hidden_states.permute(0, 2, 3, 1).reshape(batch, height * weight, inner_dim)
+                hidden_states = self.proj_in(hidden_states)
         elif self.is_input_vectorized:
             hidden_states = self.latent_image_embedding(hidden_states)
 
         # 2. Blocks
         for block in self.transformer_blocks:
             hidden_states = block(hidden_states, context=encoder_hidden_states, timestep=timestep)
 
         # 3. Output
         if self.is_input_continuous:
-            hidden_states = hidden_states.reshape(batch, height, weight, inner_dim).permute(0, 3, 1, 2)
-            hidden_states = self.proj_out(hidden_states)
+            if not self.use_linear_projection:
+                hidden_states = (
+                    hidden_states.reshape(batch, height, weight, inner_dim).permute(0, 3, 1, 2).contiguous()
+                )
+                hidden_states = self.proj_out(hidden_states)
+            else:
+                hidden_states = self.proj_out(hidden_states)
+                hidden_states = (
+                    hidden_states.reshape(batch, height, weight, inner_dim).permute(0, 3, 1, 2).contiguous()
+                )
+
             output = hidden_states + residual
         elif self.is_input_vectorized:
             hidden_states = self.norm_out(hidden_states)
             logits = self.out(hidden_states)
             # (batch, self.num_vector_embeds - 1, self.num_latent_pixels)
             logits = logits.permute(0, 2, 1)
 
@@ -364,22 +389,25 @@
         num_attention_heads: int,
         attention_head_dim: int,
         dropout=0.0,
         cross_attention_dim: Optional[int] = None,
         activation_fn: str = "geglu",
         num_embeds_ada_norm: Optional[int] = None,
         attention_bias: bool = False,
+        only_cross_attention: bool = False,
     ):
         super().__init__()
+        self.only_cross_attention = only_cross_attention
         self.attn1 = CrossAttention(
             query_dim=dim,
             heads=num_attention_heads,
             dim_head=attention_head_dim,
             dropout=dropout,
             bias=attention_bias,
+            cross_attention_dim=cross_attention_dim if only_cross_attention else None,
         )  # is a self-attention
         self.ff = FeedForward(dim, dropout=dropout, activation_fn=activation_fn)
         self.attn2 = CrossAttention(
             query_dim=dim,
             cross_attention_dim=cross_attention_dim,
             heads=num_attention_heads,
             dim_head=attention_head_dim,
@@ -438,15 +466,19 @@
             self.attn2._use_memory_efficient_attention_xformers = use_memory_efficient_attention_xformers
 
     def forward(self, hidden_states, context=None, timestep=None):
         # 1. Self-Attention
         norm_hidden_states = (
             self.norm1(hidden_states, timestep) if self.use_ada_layer_norm else self.norm1(hidden_states)
         )
-        hidden_states = self.attn1(norm_hidden_states) + hidden_states
+
+        if self.only_cross_attention:
+            hidden_states = self.attn1(norm_hidden_states, context) + hidden_states
+        else:
+            hidden_states = self.attn1(norm_hidden_states) + hidden_states
 
         # 2. Cross-Attention
         norm_hidden_states = (
             self.norm2(hidden_states, timestep) if self.use_ada_layer_norm else self.norm2(hidden_states)
         )
         hidden_states = self.attn2(norm_hidden_states, context=context) + hidden_states
```

### Comparing `diffusers-0.8.1/src/diffusers/models/attention_flax.py` & `diffusers-0.9.0/src/diffusers/models/attention_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/embeddings.py` & `diffusers-0.9.0/src/diffusers/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/embeddings_flax.py` & `diffusers-0.9.0/src/diffusers/models/embeddings_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/resnet.py` & `diffusers-0.9.0/src/diffusers/models/resnet.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/resnet_flax.py` & `diffusers-0.9.0/src/diffusers/models/resnet_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_1d.py` & `diffusers-0.9.0/src/diffusers/models/unet_1d.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_1d_blocks.py` & `diffusers-0.9.0/src/diffusers/models/unet_1d_blocks.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_2d.py` & `diffusers-0.9.0/src/diffusers/models/unet_2d.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_2d_blocks.py` & `diffusers-0.9.0/src/diffusers/models/unet_2d_blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
     downsample_padding=None,
     dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     down_block_type = down_block_type[7:] if down_block_type.startswith("UNetRes") else down_block_type
     if down_block_type == "DownBlock2D":
         return DownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -72,14 +74,16 @@
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             downsample_padding=downsample_padding,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
             dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     elif down_block_type == "SkipDownBlock2D":
         return SkipDownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             temb_channels=temb_channels,
@@ -136,14 +140,16 @@
     add_upsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
     dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     up_block_type = up_block_type[7:] if up_block_type.startswith("UNetRes") else up_block_type
     if up_block_type == "UpBlock2D":
         return UpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -166,14 +172,16 @@
             add_upsample=add_upsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
             dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     elif up_block_type == "AttnUpBlock2D":
         return AttnUpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             prev_output_channel=prev_output_channel,
@@ -242,15 +250,14 @@
         resnet_time_scale_shift: str = "default",
         resnet_act_fn: str = "swish",
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
-        **kwargs,
     ):
         super().__init__()
 
         self.attention_type = attention_type
         resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
         # there is always at least one resnet
@@ -323,15 +330,15 @@
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
         cross_attention_dim=1280,
         dual_cross_attention=False,
-        **kwargs,
+        use_linear_projection=False,
     ):
         super().__init__()
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
         resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
@@ -358,14 +365,15 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         in_channels // attn_num_head_channels,
                         in_channels=in_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         in_channels // attn_num_head_channels,
@@ -390,23 +398,25 @@
                 )
             )
 
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
         for attn in self.attentions:
@@ -519,14 +529,16 @@
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         downsample_padding=1,
         add_downsample=True,
         dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -552,14 +564,16 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
                         in_channels=out_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
@@ -582,23 +596,25 @@
             )
         else:
             self.downsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
         for attn in self.attentions:
@@ -1116,14 +1132,16 @@
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         add_upsample=True,
         dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -1151,14 +1169,16 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
                         in_channels=out_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
@@ -1175,23 +1195,25 @@
             self.upsamplers = nn.ModuleList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
         self.gradient_checkpointing = False
```

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_2d_blocks_flax.py` & `diffusers-0.9.0/src/diffusers/models/unet_2d_blocks_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_2d_condition.py` & `diffusers-0.9.0/src/diffusers/models/unet_2d_condition.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     Parameters:
         sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
             Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 4): The number of channels in the input sample.
         out_channels (`int`, *optional*, defaults to 4): The number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
-        flip_sin_to_cos (`bool`, *optional*, defaults to `True`):
+        flip_sin_to_cos (`bool`, *optional*, defaults to `False`):
             Whether to flip the sin to cos in the time embedding.
         freq_shift (`int`, *optional*, defaults to 0): The frequency shift to apply to the time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to `("CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "DownBlock2D")`):
             The tuple of downsample blocks to use.
         up_block_types (`Tuple[str]`, *optional*, defaults to `("UpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D",)`):
             The tuple of upsample blocks to use.
         block_out_channels (`Tuple[int]`, *optional*, defaults to `(320, 640, 1280, 1280)`):
@@ -94,24 +94,27 @@
         down_block_types: Tuple[str] = (
             "CrossAttnDownBlock2D",
             "CrossAttnDownBlock2D",
             "CrossAttnDownBlock2D",
             "DownBlock2D",
         ),
         up_block_types: Tuple[str] = ("UpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D"),
+        only_cross_attention: Union[bool, Tuple[bool]] = False,
         block_out_channels: Tuple[int] = (320, 640, 1280, 1280),
         layers_per_block: int = 2,
         downsample_padding: int = 1,
         mid_block_scale_factor: float = 1,
         act_fn: str = "silu",
         norm_num_groups: int = 32,
         norm_eps: float = 1e-5,
         cross_attention_dim: int = 1280,
-        attention_head_dim: int = 8,
+        attention_head_dim: Union[int, Tuple[int]] = 8,
         dual_cross_attention: bool = False,
+        use_linear_projection: bool = False,
+        num_class_embeds: Optional[int] = None,
     ):
         super().__init__()
 
         self.sample_size = sample_size
         time_embed_dim = block_out_channels[0] * 4
 
         # input
@@ -119,18 +122,28 @@
 
         # time
         self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos, freq_shift)
         timestep_input_dim = block_out_channels[0]
 
         self.time_embedding = TimestepEmbedding(timestep_input_dim, time_embed_dim)
 
+        # class embedding
+        if num_class_embeds is not None:
+            self.class_embedding = nn.Embedding(num_class_embeds, time_embed_dim)
+
         self.down_blocks = nn.ModuleList([])
         self.mid_block = None
         self.up_blocks = nn.ModuleList([])
 
+        if isinstance(only_cross_attention, bool):
+            only_cross_attention = [only_cross_attention] * len(down_block_types)
+
+        if isinstance(attention_head_dim, int):
+            attention_head_dim = (attention_head_dim,) * len(down_block_types)
+
         # down
         output_channel = block_out_channels[0]
         for i, down_block_type in enumerate(down_block_types):
             input_channel = output_channel
             output_channel = block_out_channels[i]
             is_final_block = i == len(block_out_channels) - 1
 
@@ -141,39 +154,44 @@
                 out_channels=output_channel,
                 temb_channels=time_embed_dim,
                 add_downsample=not is_final_block,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=attention_head_dim[i],
                 downsample_padding=downsample_padding,
                 dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.down_blocks.append(down_block)
 
         # mid
         self.mid_block = UNetMidBlock2DCrossAttn(
             in_channels=block_out_channels[-1],
             temb_channels=time_embed_dim,
             resnet_eps=norm_eps,
             resnet_act_fn=act_fn,
             output_scale_factor=mid_block_scale_factor,
             resnet_time_scale_shift="default",
             cross_attention_dim=cross_attention_dim,
-            attn_num_head_channels=attention_head_dim,
+            attn_num_head_channels=attention_head_dim[-1],
             resnet_groups=norm_num_groups,
             dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
         )
 
         # count how many layers upsample the images
         self.num_upsamplers = 0
 
         # up
         reversed_block_out_channels = list(reversed(block_out_channels))
+        reversed_attention_head_dim = list(reversed(attention_head_dim))
+        only_cross_attention = list(reversed(only_cross_attention))
         output_channel = reversed_block_out_channels[0]
         for i, up_block_type in enumerate(up_block_types):
             is_final_block = i == len(block_out_channels) - 1
 
             prev_output_channel = output_channel
             output_channel = reversed_block_out_channels[i]
             input_channel = reversed_block_out_channels[min(i + 1, len(block_out_channels) - 1)]
@@ -193,35 +211,39 @@
                 prev_output_channel=prev_output_channel,
                 temb_channels=time_embed_dim,
                 add_upsample=add_upsample,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=reversed_attention_head_dim[i],
                 dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
         self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0], num_groups=norm_num_groups, eps=norm_eps)
         self.conv_act = nn.SiLU()
         self.conv_out = nn.Conv2d(block_out_channels[0], out_channels, kernel_size=3, padding=1)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.config.attention_head_dim % slice_size != 0:
+        head_dims = self.config.attention_head_dim
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.config.attention_head_dim:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for block in self.down_blocks:
             if hasattr(block, "attentions") and block.attentions is not None:
                 block.set_attention_slice(slice_size)
 
         self.mid_block.set_attention_slice(slice_size)
@@ -246,22 +268,22 @@
             module.gradient_checkpointing = value
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: Union[torch.Tensor, float, int],
         encoder_hidden_states: torch.Tensor,
+        class_labels: Optional[torch.Tensor] = None,
         return_dict: bool = True,
     ) -> Union[UNet2DConditionOutput, Tuple]:
         r"""
         Args:
             sample (`torch.FloatTensor`): (batch, channel, height, width) noisy inputs tensor
             timestep (`torch.FloatTensor` or `float` or `int`): (batch) timesteps
-            encoder_hidden_states (`torch.FloatTensor`):
-                (batch_size, sequence_length, hidden_size) encoder hidden states
+            encoder_hidden_states (`torch.FloatTensor`): (batch, channel, height, width) encoder hidden states
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`models.unet_2d_condition.UNet2DConditionOutput`] instead of a plain tuple.
 
         Returns:
             [`~models.unet_2d_condition.UNet2DConditionOutput`] or `tuple`:
             [`~models.unet_2d_condition.UNet2DConditionOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
@@ -299,14 +321,20 @@
 
         # timesteps does not contain any weights and will always return f32 tensors
         # but time_embedding might actually be running in fp16. so we need to cast here.
         # there might be better ways to encapsulate this.
         t_emb = t_emb.to(dtype=self.dtype)
         emb = self.time_embedding(t_emb)
 
+        if self.config.num_class_embeds is not None:
+            if class_labels is None:
+                raise ValueError("class_labels should be provided when num_class_embeds > 0")
+            class_emb = self.class_embedding(class_labels).to(dtype=self.dtype)
+            emb = emb + class_emb
+
         # 2. pre-process
         sample = self.conv_in(sample)
 
         # 3. down
         down_block_res_samples = (sample,)
         for downsample_block in self.down_blocks:
             if hasattr(downsample_block, "attentions") and downsample_block.attentions is not None:
```

### Comparing `diffusers-0.8.1/src/diffusers/models/unet_2d_condition_flax.py` & `diffusers-0.9.0/src/diffusers/models/unet_2d_condition_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/vae.py` & `diffusers-0.9.0/src/diffusers/models/vae.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/models/vae_flax.py` & `diffusers-0.9.0/src/diffusers/models/vae_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/onnx_utils.py` & `diffusers-0.9.0/src/diffusers/onnx_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/optimization.py` & `diffusers-0.9.0/src/diffusers/optimization.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipeline_flax_utils.py` & `diffusers-0.9.0/src/diffusers/pipeline_flax_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipeline_utils.py` & `diffusers-0.9.0/src/diffusers/pipeline_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,18 +125,21 @@
     and handles methods for loading, downloading and saving models as well as a few methods common to all pipelines to:
 
         - move all PyTorch modules to the device of your choice
         - enabling/disabling the progress bar for the denoising iteration
 
     Class attributes:
 
-        - **config_name** ([`str`]) -- name of the config file that will store the class and module names of all
+        - **config_name** (`str`) -- name of the config file that will store the class and module names of all
           components of the diffusion pipeline.
+        - **_optional_components** (List[`str`]) -- list of all components that are optional so they don't have to be
+          passed for the pipeline to function (should be overridden by subclasses).
     """
     config_name = "model_index.json"
+    _optional_components = []
 
     def register_modules(self, **kwargs):
         # import it here to avoid circular import
         from diffusers import pipelines
 
         for name, module in kwargs.items():
             # retrieve library
@@ -180,20 +183,27 @@
         self.save_config(save_directory)
 
         model_index_dict = dict(self.config)
         model_index_dict.pop("_class_name")
         model_index_dict.pop("_diffusers_version")
         model_index_dict.pop("_module", None)
 
+        expected_modules, optional_kwargs = self._get_signature_keys(self)
+
+        def is_saveable_module(name, value):
+            if name not in expected_modules:
+                return False
+            if name in self._optional_components and value[0] is None:
+                return False
+            return True
+
+        model_index_dict = {k: v for k, v in model_index_dict.items() if is_saveable_module(k, v)}
+
         for pipeline_component_name in model_index_dict.keys():
             sub_model = getattr(self, pipeline_component_name)
-            if sub_model is None:
-                # edge case for saving a pipeline with safety_checker=None
-                continue
-
             model_cls = sub_model.__class__
 
             save_method_name = None
             # search for the model's base class in LOADABLE_CLASSES
             for library_name, library_classes in LOADABLE_CLASSES.items():
                 library = importlib.import_module(library_name)
                 for base_class, save_load_methods in library_classes.items():
@@ -519,46 +529,55 @@
                 " the {StableDiffusionInpaintPipelineLegacy} class and will likely remove it in version 1.0.0."
             )
             deprecate("StableDiffusionInpaintPipelineLegacy", "1.0.0", deprecation_message, standard_warn=False)
 
         # some modules can be passed directly to the init
         # in this case they are already instantiated in `kwargs`
         # extract them here
-        expected_modules = set(inspect.signature(pipeline_class.__init__).parameters.keys()) - set(["self"])
+        expected_modules, optional_kwargs = cls._get_signature_keys(pipeline_class)
         passed_class_obj = {k: kwargs.pop(k) for k in expected_modules if k in kwargs}
+        passed_pipe_kwargs = {k: kwargs.pop(k) for k in optional_kwargs if k in kwargs}
 
         init_dict, unused_kwargs, _ = pipeline_class.extract_init_dict(config_dict, **kwargs)
 
-        if len(unused_kwargs) > 0:
-            logger.warning(f"Keyword arguments {unused_kwargs} not recognized.")
+        # define init kwargs
+        init_kwargs = {k: init_dict.pop(k) for k in optional_kwargs if k in init_dict}
+        init_kwargs = {**init_kwargs, **passed_pipe_kwargs}
+
+        # remove `null` components
+        def load_module(name, value):
+            if value[0] is None:
+                return False
+            if name in passed_class_obj and passed_class_obj[name] is None:
+                return False
+            return True
 
-        init_kwargs = {}
+        init_dict = {k: v for k, v in init_dict.items() if load_module(k, v)}
+
+        if len(unused_kwargs) > 0:
+            logger.warning(
+                f"Keyword arguments {unused_kwargs} are not expected by {pipeline_class.__name__} and will be ignored."
+            )
 
         # import it here to avoid circular import
         from diffusers import pipelines
 
         # 3. Load each module in the pipeline
         for name, (library_name, class_name) in init_dict.items():
-            if class_name is None:
-                # edge case for when the pipeline was saved with safety_checker=None
-                init_kwargs[name] = None
-                continue
-
             # 3.1 - now that JAX/Flax is an official framework of the library, we might load from Flax names
             if class_name.startswith("Flax"):
                 class_name = class_name[4:]
 
             is_pipeline_module = hasattr(pipelines, library_name)
             loaded_sub_model = None
-            sub_model_should_be_defined = True
 
             # if the model is in a pipeline module, then we load it from the pipeline
             if name in passed_class_obj:
                 # 1. check that passed_class_obj has correct parent class
-                if not is_pipeline_module and passed_class_obj[name] is not None:
+                if not is_pipeline_module:
                     library = importlib.import_module(library_name)
                     class_obj = getattr(library, class_name)
                     importable_classes = LOADABLE_CLASSES[library_name]
                     class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
                     expected_class_obj = None
                     for class_name, class_candidate in class_candidates.items():
@@ -566,20 +585,14 @@
                             expected_class_obj = class_candidate
 
                     if not issubclass(passed_class_obj[name].__class__, expected_class_obj):
                         raise ValueError(
                             f"{passed_class_obj[name]} is of type: {type(passed_class_obj[name])}, but should be"
                             f" {expected_class_obj}"
                         )
-                elif passed_class_obj[name] is None:
-                    logger.warning(
-                        f"You have passed `None` for {name} to disable its functionality in {pipeline_class}. Note"
-                        f" that this might lead to problems when using {pipeline_class} and is not recommended."
-                    )
-                    sub_model_should_be_defined = False
                 else:
                     logger.warning(
                         f"You have passed a non-standard module {passed_class_obj[name]}. We cannot verify whether it"
                         " has the correct type"
                     )
 
                 # set passed class object
@@ -593,15 +606,15 @@
                 # else we just import it from the library.
                 library = importlib.import_module(library_name)
 
                 class_obj = getattr(library, class_name)
                 importable_classes = LOADABLE_CLASSES[library_name]
                 class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
-            if loaded_sub_model is None and sub_model_should_be_defined:
+            if loaded_sub_model is None:
                 load_method_name = None
                 for class_name, class_candidate in class_candidates.items():
                     if class_candidate is not None and issubclass(class_obj, class_candidate):
                         load_method_name = importable_classes[class_name][1]
 
                 if load_method_name is None:
                     none_module = class_obj.__module__
@@ -647,27 +660,37 @@
                     # else load from the root directory
                     loaded_sub_model = load_method(cached_folder, **loading_kwargs)
 
             init_kwargs[name] = loaded_sub_model  # UNet(...), # DiffusionSchedule(...)
 
         # 4. Potentially add passed objects if expected
         missing_modules = set(expected_modules) - set(init_kwargs.keys())
-        if len(missing_modules) > 0 and missing_modules <= set(passed_class_obj.keys()):
+        passed_modules = list(passed_class_obj.keys())
+        optional_modules = pipeline_class._optional_components
+        if len(missing_modules) > 0 and missing_modules <= set(passed_modules + optional_modules):
             for module in missing_modules:
-                init_kwargs[module] = passed_class_obj[module]
+                init_kwargs[module] = passed_class_obj.get(module, None)
         elif len(missing_modules) > 0:
-            passed_modules = set(list(init_kwargs.keys()) + list(passed_class_obj.keys()))
+            passed_modules = set(list(init_kwargs.keys()) + list(passed_class_obj.keys())) - optional_kwargs
             raise ValueError(
                 f"Pipeline {pipeline_class} expected {expected_modules}, but only {passed_modules} were passed."
             )
 
         # 5. Instantiate the pipeline
         model = pipeline_class(**init_kwargs)
         return model
 
+    @staticmethod
+    def _get_signature_keys(obj):
+        parameters = inspect.signature(obj.__init__).parameters
+        required_parameters = {k: v for k, v in parameters.items() if v.default == inspect._empty}
+        optional_parameters = set({k for k, v in parameters.items() if v.default != inspect._empty})
+        expected_modules = set(required_parameters.keys()) - set(["self"])
+        return expected_modules, optional_parameters
+
     @property
     def components(self) -> Dict[str, Any]:
         r"""
 
         The `self.components` property can be useful to run different pipelines with the same weights and
         configurations to not have to re-allocate memory.
 
@@ -684,16 +707,18 @@
         >>> img2img = StableDiffusionImg2ImgPipeline(**text2img.components)
         >>> inpaint = StableDiffusionInpaintPipeline(**text2img.components)
         ```
 
         Returns:
             A dictionaly containing all the modules needed to initialize the pipeline.
         """
-        components = {k: getattr(self, k) for k in self.config.keys() if not k.startswith("_")}
-        expected_modules = set(inspect.signature(self.__init__).parameters.keys()) - set(["self"])
+        expected_modules, optional_parameters = self._get_signature_keys(self)
+        components = {
+            k: getattr(self, k) for k in self.config.keys() if not k.startswith("_") and k not in optional_parameters
+        }
 
         if set(components.keys()) != expected_modules:
             raise ValueError(
                 f"{self} has been incorrectly initialized or {self.__class__} is incorrectly implemented. Expected"
                 f" {expected_modules} to be defined, but {components} are defined."
             )
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/__init__.py` & `diffusers-0.9.0/src/diffusers/pipelines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     from .stable_diffusion import (
         CycleDiffusionPipeline,
         StableDiffusionImageVariationPipeline,
         StableDiffusionImg2ImgPipeline,
         StableDiffusionInpaintPipeline,
         StableDiffusionInpaintPipelineLegacy,
         StableDiffusionPipeline,
+        StableDiffusionUpscalePipeline,
     )
     from .stable_diffusion_safe import StableDiffusionPipelineSafe
     from .versatile_diffusion import (
         VersatileDiffusionDualGuidedPipeline,
         VersatileDiffusionImageVariationPipeline,
         VersatileDiffusionPipeline,
         VersatileDiffusionTextToImagePipeline,
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/__init__.py` & `diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py` & `diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import torch
 
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, XLMRobertaTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -63,14 +64,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: RobertaSeriesModelWithTransformation,
         tokenizer: XLMRobertaTokenizer,
         unet: UNet2DConditionModel,
@@ -80,14 +82,15 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -110,33 +113,62 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Alt Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -162,17 +194,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
@@ -188,18 +225,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     @property
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
         """
@@ -366,15 +408,15 @@
         ):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -386,16 +428,16 @@
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -407,17 +449,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -455,14 +497,17 @@
         Returns:
             [`~pipelines.stable_diffusion.AltDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.AltDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(prompt, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(prompt, str) else len(prompt)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py` & `diffusers-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, XLMRobertaTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -76,14 +77,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: RobertaSeriesModelWithTransformation,
         tokenizer: XLMRobertaTokenizer,
         unet: UNet2DConditionModel,
@@ -93,14 +95,15 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -123,33 +126,62 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Alt Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
@@ -157,17 +189,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
@@ -183,18 +220,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     @property
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
         """
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/ddim/pipeline_ddim.py` & `diffusers-0.9.0/src/diffusers/pipelines/ddim/pipeline_ddim.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/ddpm/pipeline_ddpm.py` & `diffusers-0.9.0/src/diffusers/pipelines/ddpm/pipeline_ddpm.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,22 +66,22 @@
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
         message = (
-            "Please make sure to instantiate your scheduler with `predict_epsilon` instead. E.g. `scheduler ="
-            " DDPMScheduler.from_pretrained(<model_id>, predict_epsilon=True)`."
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
         )
         predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
 
         if predict_epsilon is not None:
             new_config = dict(self.scheduler.config)
-            new_config["predict_epsilon"] = predict_epsilon
+            new_config["prediction_type"] = "epsilon" if predict_epsilon else "sample"
             self.scheduler._internal_dict = FrozenDict(new_config)
 
         if generator is not None and generator.device.type != self.device.type and self.device.type != "mps":
             message = (
                 f"The `generator` device is `{generator.device}` and does not match the pipeline "
                 f"device `{self.device}`, so the `generator` will be ignored. "
                 f'Please use `torch.Generator(device="{self.device}")` instead.'
@@ -110,17 +110,15 @@
         self.scheduler.set_timesteps(num_inference_steps)
 
         for t in self.progress_bar(self.scheduler.timesteps):
             # 1. predict noise model_output
             model_output = self.unet(image, t).sample
 
             # 2. compute previous image: x_t -> x_t-1
-            image = self.scheduler.step(
-                model_output, t, image, generator=generator, predict_epsilon=predict_epsilon
-            ).prev_sample
+            image = self.scheduler.step(model_output, t, image, generator=generator).prev_sample
 
         image = (image / 2 + 0.5).clamp(0, 1)
         image = image.cpu().permute(0, 2, 3, 1).numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,36 +56,37 @@
         bert: PreTrainedModel,
         tokenizer: PreTrainedTokenizer,
         unet: Union[UNet2DModel, UNet2DConditionModel],
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
     ):
         super().__init__()
         self.register_modules(vqvae=vqvae, bert=bert, tokenizer=tokenizer, unet=unet, scheduler=scheduler)
+        self.vae_scale_factor = 2 ** (len(self.vqvae.config.block_out_channels) - 1)
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: Optional[int] = 256,
-        width: Optional[int] = 256,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: Optional[int] = 50,
         guidance_scale: Optional[float] = 1.0,
         eta: Optional[float] = 0.0,
         generator: Optional[torch.Generator] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[Tuple, ImagePipelineOutput]:
         r"""
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 256):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 256):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 1.0):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -102,14 +103,17 @@
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         if isinstance(prompt, str):
             batch_size = 1
         elif isinstance(prompt, list):
             batch_size = len(prompt)
         else:
             raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py` & `diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py` & `diffusers-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/pndm/pipeline_pndm.py` & `diffusers-0.9.0/src/diffusers/pipelines/pndm/pipeline_pndm.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/repaint/pipeline_repaint.py` & `diffusers-0.9.0/src/diffusers/pipelines/repaint/pipeline_repaint.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py` & `diffusers-0.9.0/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/__init__.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 if is_transformers_available() and is_torch_available():
     from .pipeline_cycle_diffusion import CycleDiffusionPipeline
     from .pipeline_stable_diffusion import StableDiffusionPipeline
     from .pipeline_stable_diffusion_img2img import StableDiffusionImg2ImgPipeline
     from .pipeline_stable_diffusion_inpaint import StableDiffusionInpaintPipeline
     from .pipeline_stable_diffusion_inpaint_legacy import StableDiffusionInpaintPipelineLegacy
+    from .pipeline_stable_diffusion_upscale import StableDiffusionUpscalePipeline
     from .safety_checker import StableDiffusionSafetyChecker
 
 if is_transformers_available() and is_torch_available() and is_transformers_version(">=", "4.25.0.dev0"):
     from .pipeline_stable_diffusion_image_variation import StableDiffusionImageVariationPipeline
 else:
     from ...utils.dummy_torch_and_transformers_objects import StableDiffusionImageVariationPipeline
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import DDIMScheduler
 from ...utils import PIL_INTERPOLATION, deprecate, logging
@@ -128,24 +129,26 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/CompVis/stable-diffusion-v1-4) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
         scheduler: DDIMScheduler,
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -155,33 +158,60 @@
                 " file"
             )
             deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["steps_offset"] = 1
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -190,17 +220,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -218,18 +253,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     @property
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._execution_device
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 import numpy as np
 
 import jax
 import jax.numpy as jnp
 from flax.core.frozen_dict import FrozenDict
 from flax.jax_utils import unreplicate
 from flax.training.common_utils import shard
+from packaging import version
 from PIL import Image
 from transformers import CLIPFeatureExtractor, CLIPTokenizer, FlaxCLIPTextModel
 
 from ...models import FlaxAutoencoderKL, FlaxUNet2DConditionModel
 from ...pipeline_flax_utils import FlaxDiffusionPipeline
 from ...schedulers import (
     FlaxDDIMScheduler,
     FlaxDPMSolverMultistepScheduler,
     FlaxLMSDiscreteScheduler,
     FlaxPNDMScheduler,
 )
-from ...utils import logging
+from ...utils import deprecate, logging
 from . import FlaxStableDiffusionPipelineOutput
 from .safety_checker_flax import FlaxStableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
@@ -93,23 +94,45 @@
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
     def prepare_inputs(self, prompt: Union[str, List[str]]):
         if not isinstance(prompt, (str, list)):
             raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
 
         text_input = self.tokenizer(
             prompt,
@@ -156,21 +179,25 @@
 
     def _generate(
         self,
         prompt_ids: jnp.array,
         params: Union[Dict, FrozenDict],
         prng_seed: jax.random.PRNGKey,
         num_inference_steps: int = 50,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         guidance_scale: float = 7.5,
         latents: Optional[jnp.array] = None,
         debug: bool = False,
         neg_prompt_ids: jnp.array = None,
     ):
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
+
         if height % 8 != 0 or width % 8 != 0:
             raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
 
         # get prompt text embeddings
         text_embeddings = self.text_encoder(prompt_ids, params=params["text_encoder"])[0]
 
         # TODO: currently it is assumed `do_classifier_free_guidance = guidance_scale > 1.0`
@@ -184,15 +211,20 @@
                 [""] * batch_size, padding="max_length", max_length=max_length, return_tensors="np"
             ).input_ids
         else:
             uncond_input = neg_prompt_ids
         uncond_embeddings = self.text_encoder(uncond_input, params=params["text_encoder"])[0]
         context = jnp.concatenate([uncond_embeddings, text_embeddings])
 
-        latents_shape = (batch_size, self.unet.in_channels, height // 8, width // 8)
+        latents_shape = (
+            batch_size,
+            self.unet.in_channels,
+            height // self.vae_scale_factor,
+            width // self.vae_scale_factor,
+        )
         if latents is None:
             latents = jax.random.normal(prng_seed, shape=latents_shape, dtype=jnp.float32)
         else:
             if latents.shape != latents_shape:
                 raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
 
         def loop_body(step, args):
@@ -245,33 +277,33 @@
 
     def __call__(
         self,
         prompt_ids: jnp.array,
         params: Union[Dict, FrozenDict],
         prng_seed: jax.random.PRNGKey,
         num_inference_steps: int = 50,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         guidance_scale: float = 7.5,
         latents: jnp.array = None,
         return_dict: bool = True,
         jit: bool = False,
         debug: bool = False,
         neg_prompt_ids: jnp.array = None,
         **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -298,14 +330,18 @@
         Returns:
             [`~pipelines.stable_diffusion.FlaxStableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.FlaxStableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a
             `tuple. When returning a tuple, the first element is a list with the generated images, and the second
             element is a list of `bool`s denoting whether the corresponding generated image likely represents
             "not-safe-for-work" (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
+
         if jit:
             images = _p_generate(
                 self,
                 prompt_ids,
                 params,
                 prng_seed,
                 num_inference_steps,
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,24 +37,27 @@
     text_encoder: OnnxRuntimeModel
     tokenizer: CLIPTokenizer
     unet: OnnxRuntimeModel
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
     safety_checker: OnnxRuntimeModel
     feature_extractor: CLIPFeatureExtractor
 
+    _optional_components = ["safety_checker", "feature_extractor"]
+
     def __init__(
         self,
         vae_encoder: OnnxRuntimeModel,
         vae_decoder: OnnxRuntimeModel,
         text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: OnnxRuntimeModel,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         safety_checker: OnnxRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -77,24 +80,41 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
+        if safety_checker is None and requires_safety_checker:
+            logger.warning(
+                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
+                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
+                " results in services or applications open to the public. Both the diffusers team and Hugging Face"
+                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
+                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
+                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
+            )
+
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
             prompt (`str` or `list(int)`):
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,24 +73,27 @@
     text_encoder: OnnxRuntimeModel
     tokenizer: CLIPTokenizer
     unet: OnnxRuntimeModel
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
     safety_checker: OnnxRuntimeModel
     feature_extractor: CLIPFeatureExtractor
 
+    _optional_components = ["safety_checker", "feature_extractor"]
+
     def __init__(
         self,
         vae_encoder: OnnxRuntimeModel,
         vae_decoder: OnnxRuntimeModel,
         text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: OnnxRuntimeModel,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         safety_checker: OnnxRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -113,34 +116,41 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
     def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,24 +86,27 @@
     text_encoder: OnnxRuntimeModel
     tokenizer: CLIPTokenizer
     unet: OnnxRuntimeModel
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
     safety_checker: OnnxRuntimeModel
     feature_extractor: CLIPFeatureExtractor
 
+    _optional_components = ["safety_checker", "feature_extractor"]
+
     def __init__(
         self,
         vae_encoder: OnnxRuntimeModel,
         vae_decoder: OnnxRuntimeModel,
         text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: OnnxRuntimeModel,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         safety_checker: OnnxRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
         logger.info("`OnnxStableDiffusionInpaintPipeline` is experimental and will very likely change in the future.")
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
@@ -127,34 +130,41 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
     def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
@@ -232,16 +242,16 @@
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
         image: PIL.Image.Image,
         mask_image: PIL.Image.Image,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = 512,
+        width: Optional[int] = 512,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[np.random.RandomState] = None,
         latents: Optional[np.ndarray] = None,
@@ -308,14 +318,15 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+
         if isinstance(prompt, str):
             batch_size = 1
         elif isinstance(prompt, list):
             batch_size = len(prompt)
         else:
             raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...onnx_utils import OnnxRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
 from ...utils import deprecate, logging
@@ -23,19 +24,19 @@
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
     image = image.resize((w, h), resample=PIL.Image.LANCZOS)
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     return 2.0 * image - 1.0
 
 
-def preprocess_mask(mask):
+def preprocess_mask(mask, scale_factor=8):
     mask = mask.convert("L")
     w, h = mask.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    mask = mask.resize((w // 8, h // 8), resample=PIL.Image.NEAREST)
+    mask = mask.resize((w // scale_factor, h // scale_factor), resample=PIL.Image.NEAREST)
     mask = np.array(mask).astype(np.float32) / 255.0
     mask = np.tile(mask, (4, 1, 1))
     mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
     mask = 1 - mask  # repaint white, keep black
     return mask
 
 
@@ -82,14 +83,15 @@
         vae_decoder: OnnxRuntimeModel,
         text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: OnnxRuntimeModel,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         safety_checker: OnnxRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -112,34 +114,63 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
     def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
         Encodes the prompt into text encoder hidden states.
 
         Args:
@@ -337,15 +368,15 @@
 
         # Expand init_latents for batch_size and num_images_per_prompt
         init_latents = np.concatenate([init_latents] * num_images_per_prompt, axis=0)
         init_latents_orig = init_latents
 
         # preprocess mask
         if not isinstance(mask_image, np.ndarray):
-            mask_image = preprocess_mask(mask_image)
+            mask_image = preprocess_mask(mask_image, self.vae_scale_factor)
         mask_image = mask_image.astype(latents_dtype)
         mask = np.concatenate([mask_image] * num_images_per_prompt, axis=0)
 
         # check sizes
         if not mask.shape == init_latents.shape:
             raise ValueError("The mask and init_image should be the same size!")
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import torch
 
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -62,14 +63,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
@@ -79,14 +81,15 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -109,33 +112,62 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -161,17 +193,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
@@ -187,18 +224,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     @property
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
         """
@@ -365,15 +407,15 @@
         ):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -385,16 +427,16 @@
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -406,17 +448,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -454,14 +496,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(prompt, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(prompt, str) else len(prompt)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 import inspect
 from typing import Callable, List, Optional, Union
 
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPVisionModelWithProjection
 
+from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
     DPMSolverMultistepScheduler,
     EulerAncestralDiscreteScheduler,
     EulerDiscreteScheduler,
     LMSDiscreteScheduler,
     PNDMScheduler,
 )
-from ...utils import logging
+from ...utils import deprecate, logging
 from . import StableDiffusionPipelineOutput
 from .safety_checker import StableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
@@ -59,14 +61,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         image_encoder: CLIPVisionModelWithProjection,
         unet: UNet2DConditionModel,
         scheduler: Union[
@@ -75,35 +78,65 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warn(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             image_encoder=image_encoder,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
@@ -132,17 +165,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -268,15 +306,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -288,16 +326,16 @@
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @torch.no_grad()
     def __call__(
         self,
         image: Union[PIL.Image.Image, List[PIL.Image.Image], torch.FloatTensor],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
@@ -311,17 +349,17 @@
 
         Args:
             image (`PIL.Image.Image` or `List[PIL.Image.Image]` or `torch.FloatTensor`):
                 The image or images to guide the image generation. If you provide a tensor, it needs to comply with the
                 configuration of
                 [this](https://huggingface.co/lambdalabs/sd-image-variations-diffusers/blob/main/feature_extractor/preprocessor_config.json)
                 `CLIPFeatureExtractor`
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -356,14 +394,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(image, height, width, callback_steps)
 
         # 2. Define call parameters
         if isinstance(image, PIL.Image.Image):
             batch_size = 1
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -74,14 +75,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.__init__
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
@@ -92,14 +94,15 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -122,33 +125,62 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -157,17 +189,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -185,18 +222,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     @property
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._execution_device
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
 from ...utils import deprecate, logging
@@ -146,24 +147,26 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -187,33 +190,62 @@
                 " `scheduler/scheduler_config.json` file"
             )
             deprecate("skip_prk_steps not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["skip_prk_steps"] = True
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -222,17 +254,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -250,18 +287,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -455,15 +497,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -477,15 +519,17 @@
 
     def prepare_mask_latents(
         self, mask, masked_image, batch_size, height, width, dtype, device, generator, do_classifier_free_guidance
     ):
         # resize the mask to latents shape as we concatenate the mask to the latents
         # we do that before converting to dtype to avoid breaking in case we're using cpu_offload
         # and half precision
-        mask = torch.nn.functional.interpolate(mask, size=(height // 8, width // 8))
+        mask = torch.nn.functional.interpolate(
+            mask, size=(height // self.vae_scale_factor, width // self.vae_scale_factor)
+        )
         mask = mask.to(device=device, dtype=dtype)
 
         masked_image = masked_image.to(device=device, dtype=dtype)
 
         # encode the mask image into latents space so we can concatenate it to the latents
         masked_image_latents = self.vae.encode(masked_image).latent_dist.sample(generator=generator)
         masked_image_latents = 0.18215 * masked_image_latents
@@ -505,16 +549,16 @@
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
         image: Union[torch.FloatTensor, PIL.Image.Image],
         mask_image: Union[torch.FloatTensor, PIL.Image.Image],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -534,17 +578,17 @@
                 `Image`, or tensor representing an image batch which will be inpainted, *i.e.* parts of the image will
                 be masked out with `mask_image` and repainted according to `prompt`.
             mask_image (`PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
                 repainted, while black pixels will be preserved. If `mask_image` is a PIL image, it will be converted
                 to a single channel (luminance) before use. If it's a tensor, it should contain one color channel (L)
                 instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -582,14 +626,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs
         self.check_inputs(prompt, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(prompt, str) else len(prompt)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from diffusers.utils import is_accelerate_available
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -47,19 +48,19 @@
     image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     image = torch.from_numpy(image)
     return 2.0 * image - 1.0
 
 
-def preprocess_mask(mask):
+def preprocess_mask(mask, scale_factor=8):
     mask = mask.convert("L")
     w, h = mask.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    mask = mask.resize((w // 8, h // 8), resample=PIL_INTERPOLATION["nearest"])
+    mask = mask.resize((w // scale_factor, h // scale_factor), resample=PIL_INTERPOLATION["nearest"])
     mask = np.array(mask).astype(np.float32) / 255.0
     mask = np.tile(mask, (4, 1, 1))
     mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
     mask = 1 - mask  # repaint white, keep black
     mask = torch.from_numpy(mask)
     return mask
 
@@ -87,14 +88,15 @@
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.__init__
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
@@ -105,14 +107,15 @@
             LMSDiscreteScheduler,
             EulerDiscreteScheduler,
             EulerAncestralDiscreteScheduler,
             DPMSolverMultistepScheduler,
         ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -135,33 +138,62 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -170,17 +202,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -198,18 +235,23 @@
         if is_accelerate_available():
             from accelerate import cpu_offload
         else:
             raise ImportError("Please install accelerate via `pip install accelerate`")
 
         device = torch.device(f"cuda:{gpu_id}")
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
+        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae]:
             if cpu_offloaded_model is not None:
                 cpu_offload(cpu_offloaded_model, device)
 
+        if self.safety_checker is not None:
+            # TODO(Patrick) - there is currently a bug with cpu offload of nn.Parameter in accelerate
+            # fix by only offloading self.safety_checker for now
+            cpu_offload(self.safety_checker.vision_model, device)
+
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -528,15 +570,15 @@
         )
 
         # 4. Preprocess image and mask
         if not isinstance(init_image, torch.FloatTensor):
             init_image = preprocess_image(init_image)
 
         if not isinstance(mask_image, torch.FloatTensor):
-            mask_image = preprocess_mask(mask_image)
+            mask_image = preprocess_mask(mask_image, self.vae_scale_factor)
 
         # 5. set timesteps
         self.scheduler.set_timesteps(num_inference_steps, device=device)
         timesteps = self.get_timesteps(num_inference_steps, strength, device)
         latent_timestep = timesteps[:1].repeat(batch_size * num_images_per_prompt)
 
         # 6. Prepare latent variables
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/safety_checker.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/__init__.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import warnings
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
+from packaging import version
 from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import (
     DDIMScheduler,
@@ -52,14 +53,16 @@
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
 
+    _optional_components = ["safety_checker", "feature_extractor"]
+
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
         scheduler: Union[
@@ -68,14 +71,15 @@
             EulerAncestralDiscreteScheduler,
             EulerDiscreteScheduler,
             LMSDiscreteScheduler,
             PNDMScheduler,
         ],
         safety_checker: SafeStableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
         safety_concept: Optional[str] = (
             "an image showing hate, harassment, violence, suffering, humiliation, harm, suicide, sexual, nudity,"
             " bodily fluids, blood, obscene gestures, illegal activity, drug use, theft, vandalism, weapons, child"
             " abuse, brutality, cruelty"
         )
@@ -103,34 +107,63 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
 
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_diffusers_version") and version.parse(
+            version.parse(unet.config._diffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
+
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self._safety_text_concept = safety_concept
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
     @property
     def safety_concept(self):
         r"""
         Getter method for the safety concept used with SLD
 
         Returns:
@@ -429,15 +462,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -491,16 +524,16 @@
                 noise_guidance = noise_guidance - noise_guidance_safety
         return noise_guidance, safety_momentum
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -517,17 +550,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -585,14 +618,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(prompt, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(prompt, str) else len(prompt)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py` & `diffusers-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py` & `diffusers-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/__init__.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     add_downsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
     downsample_padding=None,
-    dual_cross_attention=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     down_block_type = down_block_type[7:] if down_block_type.startswith("UNetRes") else down_block_type
     if down_block_type == "DownBlockFlat":
         return DownBlockFlat(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -54,14 +56,17 @@
             add_downsample=add_downsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             downsample_padding=downsample_padding,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
+            dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     raise ValueError(f"{down_block_type} is not supported.")
 
 
 def get_up_block(
     up_block_type,
     num_layers,
@@ -71,15 +76,17 @@
     temb_channels,
     add_upsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
-    dual_cross_attention=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     up_block_type = up_block_type[7:] if up_block_type.startswith("UNetRes") else up_block_type
     if up_block_type == "UpBlockFlat":
         return UpBlockFlat(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -101,14 +108,17 @@
             temb_channels=temb_channels,
             add_upsample=add_upsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
+            dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     raise ValueError(f"{up_block_type} is not supported.")
 
 
 # Copied from diffusers.models.unet_2d_condition.UNet2DConditionModel with UNet2DConditionModel->UNetFlatConditionModel, nn.Conv2d->LinearMultiDim, Block2D->BlockFlat
 class UNetFlatConditionModel(ModelMixin, ConfigMixin):
     r"""
@@ -120,15 +130,15 @@
 
     Parameters:
         sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
             Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 4): The number of channels in the input sample.
         out_channels (`int`, *optional*, defaults to 4): The number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
-        flip_sin_to_cos (`bool`, *optional*, defaults to `True`):
+        flip_sin_to_cos (`bool`, *optional*, defaults to `False`):
             Whether to flip the sin to cos in the time embedding.
         freq_shift (`int`, *optional*, defaults to 0): The frequency shift to apply to the time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to `("CrossAttnDownBlockFlat", "CrossAttnDownBlockFlat", "CrossAttnDownBlockFlat", "DownBlockFlat")`):
             The tuple of downsample blocks to use.
         up_block_types (`Tuple[str]`, *optional*, defaults to `("UpBlockFlat", "CrossAttnUpBlockFlat", "CrossAttnUpBlockFlat", "CrossAttnUpBlockFlat",)`):
             The tuple of upsample blocks to use.
         block_out_channels (`Tuple[int]`, *optional*, defaults to `(320, 640, 1280, 1280)`):
@@ -162,24 +172,27 @@
         ),
         up_block_types: Tuple[str] = (
             "UpBlockFlat",
             "CrossAttnUpBlockFlat",
             "CrossAttnUpBlockFlat",
             "CrossAttnUpBlockFlat",
         ),
+        only_cross_attention: Union[bool, Tuple[bool]] = False,
         block_out_channels: Tuple[int] = (320, 640, 1280, 1280),
         layers_per_block: int = 2,
         downsample_padding: int = 1,
         mid_block_scale_factor: float = 1,
         act_fn: str = "silu",
         norm_num_groups: int = 32,
         norm_eps: float = 1e-5,
         cross_attention_dim: int = 1280,
-        attention_head_dim: int = 8,
+        attention_head_dim: Union[int, Tuple[int]] = 8,
         dual_cross_attention: bool = False,
+        use_linear_projection: bool = False,
+        num_class_embeds: Optional[int] = None,
     ):
         super().__init__()
 
         self.sample_size = sample_size
         time_embed_dim = block_out_channels[0] * 4
 
         # input
@@ -187,18 +200,28 @@
 
         # time
         self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos, freq_shift)
         timestep_input_dim = block_out_channels[0]
 
         self.time_embedding = TimestepEmbedding(timestep_input_dim, time_embed_dim)
 
+        # class embedding
+        if num_class_embeds is not None:
+            self.class_embedding = nn.Embedding(num_class_embeds, time_embed_dim)
+
         self.down_blocks = nn.ModuleList([])
         self.mid_block = None
         self.up_blocks = nn.ModuleList([])
 
+        if isinstance(only_cross_attention, bool):
+            only_cross_attention = [only_cross_attention] * len(down_block_types)
+
+        if isinstance(attention_head_dim, int):
+            attention_head_dim = (attention_head_dim,) * len(down_block_types)
+
         # down
         output_channel = block_out_channels[0]
         for i, down_block_type in enumerate(down_block_types):
             input_channel = output_channel
             output_channel = block_out_channels[i]
             is_final_block = i == len(block_out_channels) - 1
 
@@ -209,39 +232,44 @@
                 out_channels=output_channel,
                 temb_channels=time_embed_dim,
                 add_downsample=not is_final_block,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=attention_head_dim[i],
                 downsample_padding=downsample_padding,
                 dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.down_blocks.append(down_block)
 
         # mid
         self.mid_block = UNetMidBlockFlatCrossAttn(
             in_channels=block_out_channels[-1],
             temb_channels=time_embed_dim,
             resnet_eps=norm_eps,
             resnet_act_fn=act_fn,
             output_scale_factor=mid_block_scale_factor,
             resnet_time_scale_shift="default",
             cross_attention_dim=cross_attention_dim,
-            attn_num_head_channels=attention_head_dim,
+            attn_num_head_channels=attention_head_dim[-1],
             resnet_groups=norm_num_groups,
             dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
         )
 
         # count how many layers upsample the images
         self.num_upsamplers = 0
 
         # up
         reversed_block_out_channels = list(reversed(block_out_channels))
+        reversed_attention_head_dim = list(reversed(attention_head_dim))
+        only_cross_attention = list(reversed(only_cross_attention))
         output_channel = reversed_block_out_channels[0]
         for i, up_block_type in enumerate(up_block_types):
             is_final_block = i == len(block_out_channels) - 1
 
             prev_output_channel = output_channel
             output_channel = reversed_block_out_channels[i]
             input_channel = reversed_block_out_channels[min(i + 1, len(block_out_channels) - 1)]
@@ -261,35 +289,39 @@
                 prev_output_channel=prev_output_channel,
                 temb_channels=time_embed_dim,
                 add_upsample=add_upsample,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=reversed_attention_head_dim[i],
                 dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
         self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0], num_groups=norm_num_groups, eps=norm_eps)
         self.conv_act = nn.SiLU()
         self.conv_out = LinearMultiDim(block_out_channels[0], out_channels, kernel_size=3, padding=1)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.config.attention_head_dim % slice_size != 0:
+        head_dims = self.config.attention_head_dim
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.config.attention_head_dim:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for block in self.down_blocks:
             if hasattr(block, "attentions") and block.attentions is not None:
                 block.set_attention_slice(slice_size)
 
         self.mid_block.set_attention_slice(slice_size)
@@ -314,22 +346,22 @@
             module.gradient_checkpointing = value
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: Union[torch.Tensor, float, int],
         encoder_hidden_states: torch.Tensor,
+        class_labels: Optional[torch.Tensor] = None,
         return_dict: bool = True,
     ) -> Union[UNet2DConditionOutput, Tuple]:
         r"""
         Args:
             sample (`torch.FloatTensor`): (batch, channel, height, width) noisy inputs tensor
             timestep (`torch.FloatTensor` or `float` or `int`): (batch) timesteps
-            encoder_hidden_states (`torch.FloatTensor`):
-                (batch_size, sequence_length, hidden_size) encoder hidden states
+            encoder_hidden_states (`torch.FloatTensor`): (batch, channel, height, width) encoder hidden states
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`models.unet_2d_condition.UNet2DConditionOutput`] instead of a plain tuple.
 
         Returns:
             [`~models.unet_2d_condition.UNet2DConditionOutput`] or `tuple`:
             [`~models.unet_2d_condition.UNet2DConditionOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
@@ -367,14 +399,20 @@
 
         # timesteps does not contain any weights and will always return f32 tensors
         # but time_embedding might actually be running in fp16. so we need to cast here.
         # there might be better ways to encapsulate this.
         t_emb = t_emb.to(dtype=self.dtype)
         emb = self.time_embedding(t_emb)
 
+        if self.config.num_class_embeds is not None:
+            if class_labels is None:
+                raise ValueError("class_labels should be provided when num_class_embeds > 0")
+            class_emb = self.class_embedding(class_labels).to(dtype=self.dtype)
+            emb = emb + class_emb
+
         # 2. pre-process
         sample = self.conv_in(sample)
 
         # 3. down
         down_block_res_samples = (sample,)
         for downsample_block in self.down_blocks:
             if hasattr(downsample_block, "attentions") and downsample_block.attentions is not None:
@@ -636,14 +674,16 @@
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         downsample_padding=1,
         add_downsample=True,
         dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -669,14 +709,16 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
                         in_channels=out_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
@@ -699,23 +741,25 @@
             )
         else:
             self.downsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
         for attn in self.attentions:
@@ -847,14 +891,16 @@
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         add_upsample=True,
         dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -882,14 +928,16 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
                         in_channels=out_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         out_channels // attn_num_head_channels,
@@ -906,23 +954,25 @@
             self.upsamplers = nn.ModuleList([LinearMultiDim(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
         self.gradient_checkpointing = False
 
@@ -984,15 +1034,15 @@
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
         cross_attention_dim=1280,
         dual_cross_attention=False,
-        **kwargs,
+        use_linear_projection=False,
     ):
         super().__init__()
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
         resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
@@ -1019,14 +1069,15 @@
                     Transformer2DModel(
                         attn_num_head_channels,
                         in_channels // attn_num_head_channels,
                         in_channels=in_channels,
                         num_layers=1,
                         cross_attention_dim=cross_attention_dim,
                         norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
                     )
                 )
             else:
                 attentions.append(
                     DualTransformer2DModel(
                         attn_num_head_channels,
                         in_channels // attn_num_head_channels,
@@ -1051,23 +1102,25 @@
                 )
             )
 
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
         for attn in self.attentions:
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             text_encoder=text_encoder,
             image_encoder=image_encoder,
             image_unet=image_unet,
             text_unet=text_unet,
             vae=vae,
             scheduler=scheduler,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
@@ -107,16 +108,16 @@
         # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
     @torch.no_grad()
     def image_variation(
         self,
         image: Union[torch.FloatTensor, PIL.Image.Image],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -127,17 +128,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             image (`PIL.Image.Image`, `List[PIL.Image.Image]` or `torch.Tensor`):
                 The image prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -189,15 +190,15 @@
 
         >>> pipe = VersatileDiffusionPipeline.from_pretrained(
         ...     "shi-labs/versatile-diffusion", torch_dtype=torch.float16
         ... )
         >>> pipe = pipe.to("cuda")
 
         >>> generator = torch.Generator(device="cuda").manual_seed(0)
-        >>> image = pipe(image, generator=generator).images[0]
+        >>> image = pipe.image_variation(image, generator=generator).images[0]
         >>> image.save("./car_variation.png")
         ```
 
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
@@ -223,16 +224,16 @@
             callback_steps=callback_steps,
         )
 
     @torch.no_grad()
     def text_to_image(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -243,17 +244,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -337,16 +338,16 @@
 
     @torch.no_grad()
     def dual_guided(
         self,
         prompt: Union[PIL.Image.Image, List[PIL.Image.Image]],
         image: Union[str, List[str]],
         text_to_image_strength: float = 0.5,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
@@ -356,17 +357,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     text_encoder: CLIPTextModelWithProjection
     image_encoder: CLIPVisionModelWithProjection
     image_unet: UNet2DConditionModel
     text_unet: UNetFlatConditionModel
     vae: AutoencoderKL
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
 
+    _optional_components = ["text_unet"]
+
     def __init__(
         self,
         tokenizer: CLIPTokenizer,
         image_feature_extractor: CLIPFeatureExtractor,
         text_encoder: CLIPTextModelWithProjection,
         image_encoder: CLIPVisionModelWithProjection,
         image_unet: UNet2DConditionModel,
@@ -83,14 +85,15 @@
             text_encoder=text_encoder,
             image_encoder=image_encoder,
             image_unet=image_unet,
             text_unet=text_unet,
             vae=vae,
             scheduler=scheduler,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
         if self.text_unet is not None and (
             "dual_cross_attention" not in self.image_unet.config or not self.image_unet.config.dual_cross_attention
         ):
             # if loading from a universal checkpoint rather than a saved dual-guided pipeline
             self._convert_to_dual_attention()
 
@@ -138,14 +141,16 @@
         """
         for name, module in self.image_unet.named_modules():
             if isinstance(module, DualTransformer2DModel):
                 parent_name, index = name.rsplit(".", 1)
                 index = int(index)
                 self.image_unet.get_submodule(parent_name)[index] = module.transformers[0]
 
+        self.image_unet.register_to_config(dual_cross_attention=False)
+
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention with unet->image_unet
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -173,17 +178,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.image_unet.config.attention_head_dim // 2
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
+
         self.image_unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -415,15 +425,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -450,16 +460,16 @@
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[PIL.Image.Image, List[PIL.Image.Image]],
         image: Union[str, List[str]],
         text_to_image_strength: float = 0.5,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
@@ -470,17 +480,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -547,14 +557,17 @@
         ```
 
         Returns:
             [`~pipelines.stable_diffusion.ImagePipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.ImagePipelineOutput`] if `return_dict` is True, otherwise a `tuple. When
             returning a tuple, the first element is a list with the generated images.
         """
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(prompt, image, height, width, callback_steps)
 
         # 2. Define call parameters
         prompt = [prompt] if not isinstance(prompt, list) else prompt
         image = [image] if not isinstance(image, list) else image
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.register_modules(
             image_feature_extractor=image_feature_extractor,
             image_encoder=image_encoder,
             image_unet=image_unet,
             vae=vae,
             scheduler=scheduler,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention with unet->image_unet
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
@@ -103,17 +104,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.image_unet.config.attention_head_dim // 2
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
+
         self.image_unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -273,15 +279,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -293,16 +299,16 @@
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @torch.no_grad()
     def __call__(
         self,
         image: Union[PIL.Image.Image, List[PIL.Image.Image], torch.Tensor],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -314,17 +320,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             image (`PIL.Image.Image`, `List[PIL.Image.Image]` or `torch.Tensor`):
                 The image prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -387,14 +393,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(image, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(image, PIL.Image.Image) else len(image)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py` & `diffusers-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     image_feature_extractor: CLIPFeatureExtractor
     text_encoder: CLIPTextModelWithProjection
     image_unet: UNet2DConditionModel
     text_unet: UNetFlatConditionModel
     vae: AutoencoderKL
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
 
+    _optional_components = ["text_unet"]
+
     def __init__(
         self,
         tokenizer: CLIPTokenizer,
         text_encoder: CLIPTextModelWithProjection,
         image_unet: UNet2DConditionModel,
         text_unet: UNetFlatConditionModel,
         vae: AutoencoderKL,
@@ -71,14 +73,15 @@
             tokenizer=tokenizer,
             text_encoder=text_encoder,
             image_unet=image_unet,
             text_unet=text_unet,
             vae=vae,
             scheduler=scheduler,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
         if self.text_unet is not None:
             self._swap_unet_attention_blocks()
 
     def _swap_unet_attention_blocks(self):
         """
         Swap the `Transformer2DModel` blocks between the image and text UNets
@@ -126,17 +129,22 @@
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.image_unet.config.attention_head_dim // 2
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
+
         self.image_unet.set_attention_slice(slice_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
@@ -333,15 +341,15 @@
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
     def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
-        shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
         if latents is None:
             if device.type == "mps":
                 # randn does not work reproducibly on mps
                 latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
             else:
                 latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
         else:
@@ -353,16 +361,16 @@
         latents = latents * self.scheduler.init_noise_sigma
         return latents
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
@@ -374,17 +382,17 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -439,14 +447,17 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
 
         # 1. Check inputs. Raise error if not correct
         self.check_inputs(prompt, height, width, callback_steps)
 
         # 2. Define call parameters
         batch_size = 1 if isinstance(prompt, str) else len(prompt)
         device = self._execution_device
```

### Comparing `diffusers-0.8.1/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py` & `diffusers-0.9.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/__init__.py` & `diffusers-0.9.0/src/diffusers/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddim.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddim.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, deprecate
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
 # Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->DDIM
 class DDIMSchedulerOutput(BaseOutput):
     """
@@ -102,31 +102,45 @@
             each diffusion step uses the value of alphas product at that step and at the previous one. For the final
             step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
             otherwise it uses the value of alpha at step 0.
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the samples. One of `epsilon`, `sample`.
+            `v-prediction` is not supported for this scheduler.
 
     """
 
     _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[np.ndarray] = None,
         clip_sample: bool = True,
         set_alpha_to_one: bool = True,
         steps_offset: int = 0,
+        prediction_type: str = "epsilon",
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDIMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
+
         if trained_betas is not None:
             self.betas = torch.from_numpy(trained_betas)
         elif beta_schedule == "linear":
             self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = (
@@ -254,15 +268,27 @@
         alpha_prod_t = self.alphas_cumprod[timestep]
         alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
 
         beta_prod_t = 1 - alpha_prod_t
 
         # 3. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+        elif self.config.prediction_type == "sample":
+            pred_original_sample = model_output
+        elif self.config.prediction_type == "v_prediction":
+            pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
+            # predict V
+            model_output = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                " `v_prediction`"
+            )
 
         # 4. Clip "predicted x_0"
         if self.config.clip_sample:
             pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
 
         # 5. compute variance: "sigma_t(η)" -> see formula (16)
         # σ_t = sqrt((1 − α_t−1)/(1 − α_t)) * sqrt(1 − α_t/α_t−1)
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddim_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddpm_flax.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# Copyright 2022 Stanford University Team and The HuggingFace Team. All rights reserved.
+# Copyright 2022 UC Berkeley Team and The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# DISCLAIMER: This code is strongly influenced by https://github.com/pesser/pytorch_diffusion
-# and https://github.com/hojonathanho/diffusion
+# DISCLAIMER: This file is strongly influenced by https://github.com/ermongroup/ddim
 
 import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import flax
 import jax.numpy as jnp
+from jax import random
 
-from ..configuration_utils import ConfigMixin, register_to_config
+from ..configuration_utils import ConfigMixin, FrozenDict, register_to_config
+from ..utils import deprecate
 from .scheduling_utils_flax import (
     _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
     FlaxSchedulerMixin,
     FlaxSchedulerOutput,
     broadcast_to_shape_from_left,
 )
 
@@ -57,241 +58,260 @@
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
     return jnp.array(betas, dtype=jnp.float32)
 
 
 @flax.struct.dataclass
-class DDIMSchedulerState:
+class DDPMSchedulerState:
     # setable values
     timesteps: jnp.ndarray
-    alphas_cumprod: jnp.ndarray
     num_inference_steps: Optional[int] = None
 
     @classmethod
-    def create(cls, num_train_timesteps: int, alphas_cumprod: jnp.ndarray):
-        return cls(timesteps=jnp.arange(0, num_train_timesteps)[::-1], alphas_cumprod=alphas_cumprod)
+    def create(cls, num_train_timesteps: int):
+        return cls(timesteps=jnp.arange(0, num_train_timesteps)[::-1])
 
 
 @dataclass
-class FlaxDDIMSchedulerOutput(FlaxSchedulerOutput):
-    state: DDIMSchedulerState
+class FlaxDDPMSchedulerOutput(FlaxSchedulerOutput):
+    state: DDPMSchedulerState
 
 
-class FlaxDDIMScheduler(FlaxSchedulerMixin, ConfigMixin):
+class FlaxDDPMScheduler(FlaxSchedulerMixin, ConfigMixin):
     """
-    Denoising diffusion implicit models is a scheduler that extends the denoising procedure introduced in denoising
-    diffusion probabilistic models (DDPMs) with non-Markovian guidance.
+    Denoising diffusion probabilistic models (DDPMs) explores the connections between denoising score matching and
+    Langevin dynamics sampling.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
     [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
     [`~SchedulerMixin.from_pretrained`] functions.
 
-    For more details, see the original paper: https://arxiv.org/abs/2010.02502
+    For more details, see the original paper: https://arxiv.org/abs/2006.11239
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
-        trained_betas (`jnp.ndarray`, optional):
+        trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
+        variance_type (`str`):
+            options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
+            `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
-        set_alpha_to_one (`bool`, default `True`):
-            each diffusion step uses the value of alphas product at that step and at the previous one. For the final
-            step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
-            otherwise it uses the value of alpha at step 0.
-        steps_offset (`int`, default `0`):
-            an offset added to the inference steps. You can use a combination of `offset=1` and
-            `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
-            stable diffusion.
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the samples. One of `epsilon`, `sample`.
+            `v-prediction` is not supported for this scheduler.
     """
 
     _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
 
     @property
     def has_state(self):
         return True
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        set_alpha_to_one: bool = True,
-        steps_offset: int = 0,
+        trained_betas: Optional[jnp.ndarray] = None,
+        variance_type: str = "fixed_small",
+        clip_sample: bool = True,
+        prediction_type: str = "epsilon",
+        **kwargs,
     ):
-        if beta_schedule == "linear":
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " FlaxDDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
+
+        if trained_betas is not None:
+            self.betas = jnp.asarray(trained_betas)
+        elif beta_schedule == "linear":
             self.betas = jnp.linspace(beta_start, beta_end, num_train_timesteps, dtype=jnp.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = jnp.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=jnp.float32) ** 2
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
         else:
             raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
-
-        # HACK for now - clean up later (PVP)
-        self._alphas_cumprod = jnp.cumprod(self.alphas, axis=0)
-
-        # At every step in ddim, we are looking into the previous alphas_cumprod
-        # For the final step, there is no previous alphas_cumprod because we are already at 0
-        # `set_alpha_to_one` decides whether we set this parameter simply to one or
-        # whether we use the final alpha of the "non-previous" one.
-        self.final_alpha_cumprod = jnp.array(1.0) if set_alpha_to_one else float(self._alphas_cumprod[0])
-
-        # standard deviation of the initial noise distribution
-        self.init_noise_sigma = 1.0
-
-    def scale_model_input(
-        self, state: DDIMSchedulerState, sample: jnp.ndarray, timestep: Optional[int] = None
-    ) -> jnp.ndarray:
-        """
-        Args:
-            state (`PNDMSchedulerState`): the `FlaxPNDMScheduler` state data class instance.
-            sample (`jnp.ndarray`): input sample
-            timestep (`int`, optional): current timestep
-
-        Returns:
-            `jnp.ndarray`: scaled input sample
-        """
-        return sample
+        self.alphas_cumprod = jnp.cumprod(self.alphas, axis=0)
+        self.one = jnp.array(1.0)
 
     def create_state(self):
-        return DDIMSchedulerState.create(
-            num_train_timesteps=self.config.num_train_timesteps, alphas_cumprod=self._alphas_cumprod
-        )
-
-    def _get_variance(self, timestep, prev_timestep, alphas_cumprod):
-        alpha_prod_t = alphas_cumprod[timestep]
-        alpha_prod_t_prev = jnp.where(prev_timestep >= 0, alphas_cumprod[prev_timestep], self.final_alpha_cumprod)
-        beta_prod_t = 1 - alpha_prod_t
-        beta_prod_t_prev = 1 - alpha_prod_t_prev
-
-        variance = (beta_prod_t_prev / beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
-
-        return variance
+        return DDPMSchedulerState.create(num_train_timesteps=self.config.num_train_timesteps)
 
     def set_timesteps(
-        self, state: DDIMSchedulerState, num_inference_steps: int, shape: Tuple = ()
-    ) -> DDIMSchedulerState:
+        self, state: DDPMSchedulerState, num_inference_steps: int, shape: Tuple = ()
+    ) -> DDPMSchedulerState:
         """
         Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             state (`DDIMSchedulerState`):
-                the `FlaxDDIMScheduler` state data class instance.
+                the `FlaxDDPMScheduler` state data class instance.
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
         """
-        offset = self.config.steps_offset
+        num_inference_steps = min(self.config.num_train_timesteps, num_inference_steps)
+        timesteps = jnp.arange(
+            0, self.config.num_train_timesteps, self.config.num_train_timesteps // num_inference_steps
+        )[::-1]
+        return state.replace(num_inference_steps=num_inference_steps, timesteps=timesteps)
 
-        step_ratio = self.config.num_train_timesteps // num_inference_steps
-        # creates integer timesteps by multiplying by ratio
-        # casting to int to avoid issues when num_inference_step is power of 3
-        timesteps = (jnp.arange(0, num_inference_steps) * step_ratio).round()[::-1]
-        timesteps = timesteps + offset
+    def _get_variance(self, t, predicted_variance=None, variance_type=None):
+        alpha_prod_t = self.alphas_cumprod[t]
+        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
+
+        # For t > 0, compute predicted variance βt (see formula (6) and (7) from https://arxiv.org/pdf/2006.11239.pdf)
+        # and sample from it to get previous sample
+        # x_{t-1} ~ N(pred_prev_sample, variance) == add variance to pred_sample
+        variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
+
+        if variance_type is None:
+            variance_type = self.config.variance_type
+
+        # hacks - were probably added for training stability
+        if variance_type == "fixed_small":
+            variance = jnp.clip(variance, a_min=1e-20)
+        # for rl-diffuser https://arxiv.org/abs/2205.09991
+        elif variance_type == "fixed_small_log":
+            variance = jnp.log(jnp.clip(variance, a_min=1e-20))
+        elif variance_type == "fixed_large":
+            variance = self.betas[t]
+        elif variance_type == "fixed_large_log":
+            # Glide max_log
+            variance = jnp.log(self.betas[t])
+        elif variance_type == "learned":
+            return predicted_variance
+        elif variance_type == "learned_range":
+            min_log = variance
+            max_log = self.betas[t]
+            frac = (predicted_variance + 1) / 2
+            variance = frac * max_log + (1 - frac) * min_log
 
-        return state.replace(num_inference_steps=num_inference_steps, timesteps=timesteps)
+        return variance
 
     def step(
         self,
-        state: DDIMSchedulerState,
+        state: DDPMSchedulerState,
         model_output: jnp.ndarray,
         timestep: int,
         sample: jnp.ndarray,
+        key: random.KeyArray,
         return_dict: bool = True,
-    ) -> Union[FlaxDDIMSchedulerOutput, Tuple]:
+        **kwargs,
+    ) -> Union[FlaxDDPMSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
-            state (`DDIMSchedulerState`): the `FlaxDDIMScheduler` state data class instance.
+            state (`DDPMSchedulerState`): the `FlaxDDPMScheduler` state data class instance.
             model_output (`jnp.ndarray`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`jnp.ndarray`):
                 current instance of sample being created by diffusion process.
-            return_dict (`bool`): option for returning tuple rather than FlaxDDIMSchedulerOutput class
+            key (`random.KeyArray`): a PRNG key.
+            return_dict (`bool`): option for returning tuple rather than FlaxDDPMSchedulerOutput class
 
         Returns:
-            [`FlaxDDIMSchedulerOutput`] or `tuple`: [`FlaxDDIMSchedulerOutput`] if `return_dict` is True, otherwise a
+            [`FlaxDDPMSchedulerOutput`] or `tuple`: [`FlaxDDPMSchedulerOutput`] if `return_dict` is True, otherwise a
             `tuple`. When returning a tuple, the first element is the sample tensor.
 
         """
-        if state.num_inference_steps is None:
-            raise ValueError(
-                "Number of inference steps is 'None', you need to run 'set_timesteps' after creating the scheduler"
-            )
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " FlaxDDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            new_config = dict(self.config)
+            new_config["prediction_type"] = "epsilon" if predict_epsilon else "sample"
+            self._internal_dict = FrozenDict(new_config)
 
-        # See formulas (12) and (16) of DDIM paper https://arxiv.org/pdf/2010.02502.pdf
-        # Ideally, read DDIM paper in-detail understanding
+        t = timestep
 
-        # Notation (<variable name> -> <name in paper>
-        # - pred_noise_t -> e_theta(x_t, t)
-        # - pred_original_sample -> f_theta(x_t, t) or x_0
-        # - std_dev_t -> sigma_t
-        # - eta -> η
-        # - pred_sample_direction -> "direction pointing to x_t"
-        # - pred_prev_sample -> "x_t-1"
-
-        # TODO(Patrick) - eta is always 0.0 for now, allow to be set in step function
-        eta = 0.0
-
-        # 1. get previous step value (=t-1)
-        prev_timestep = timestep - self.config.num_train_timesteps // state.num_inference_steps
-
-        alphas_cumprod = state.alphas_cumprod
-
-        # 2. compute alphas, betas
-        alpha_prod_t = alphas_cumprod[timestep]
-        alpha_prod_t_prev = jnp.where(prev_timestep >= 0, alphas_cumprod[prev_timestep], self.final_alpha_cumprod)
+        if model_output.shape[1] == sample.shape[1] * 2 and self.config.variance_type in ["learned", "learned_range"]:
+            model_output, predicted_variance = jnp.split(model_output, sample.shape[1], axis=1)
+        else:
+            predicted_variance = None
 
+        # 1. compute alphas, betas
+        alpha_prod_t = self.alphas_cumprod[t]
+        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
         beta_prod_t = 1 - alpha_prod_t
+        beta_prod_t_prev = 1 - alpha_prod_t_prev
 
-        # 3. compute predicted original sample from predicted noise also called
-        # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
-
-        # 4. compute variance: "sigma_t(η)" -> see formula (16)
-        # σ_t = sqrt((1 − α_t−1)/(1 − α_t)) * sqrt(1 − α_t/α_t−1)
-        variance = self._get_variance(timestep, prev_timestep, alphas_cumprod)
-        std_dev_t = eta * variance ** (0.5)
+        # 2. compute predicted original sample from predicted noise also called
+        # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+        elif self.config.prediction_type == "sample":
+            pred_original_sample = model_output
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample` "
+                " for the FlaxDDPMScheduler."
+            )
 
-        # 5. compute "direction pointing to x_t" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * model_output
+        # 3. Clip "predicted x_0"
+        if self.config.clip_sample:
+            pred_original_sample = jnp.clip(pred_original_sample, -1, 1)
+
+        # 4. Compute coefficients for pred_original_sample x_0 and current sample x_t
+        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
+        pred_original_sample_coeff = (alpha_prod_t_prev ** (0.5) * self.betas[t]) / beta_prod_t
+        current_sample_coeff = self.alphas[t] ** (0.5) * beta_prod_t_prev / beta_prod_t
+
+        # 5. Compute predicted previous sample µ_t
+        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
+        pred_prev_sample = pred_original_sample_coeff * pred_original_sample + current_sample_coeff * sample
+
+        # 6. Add noise
+        variance = 0
+        if t > 0:
+            key = random.split(key, num=1)
+            noise = random.normal(key=key, shape=model_output.shape)
+            variance = (self._get_variance(t, predicted_variance=predicted_variance) ** 0.5) * noise
 
-        # 6. compute x_t without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        prev_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
+        pred_prev_sample = pred_prev_sample + variance
 
         if not return_dict:
-            return (prev_sample, state)
+            return (pred_prev_sample, state)
 
-        return FlaxDDIMSchedulerOutput(prev_sample=prev_sample, state=state)
+        return FlaxDDPMSchedulerOutput(prev_sample=pred_prev_sample, state=state)
 
     def add_noise(
         self,
         original_samples: jnp.ndarray,
         noise: jnp.ndarray,
         timesteps: jnp.ndarray,
     ) -> jnp.ndarray:
         sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
         sqrt_alpha_prod = sqrt_alpha_prod.flatten()
         sqrt_alpha_prod = broadcast_to_shape_from_left(sqrt_alpha_prod, original_samples.shape)
 
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.0
+        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
         sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
         sqrt_one_minus_alpha_prod = broadcast_to_shape_from_left(sqrt_one_minus_alpha_prod, original_samples.shape)
 
         noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
         return noisy_samples
 
     def __len__(self):
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddpm.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_ddpm.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,33 +95,43 @@
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         variance_type (`str`):
             options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
             `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
-        predict_epsilon (`bool`):
-            optional flag to use when the model predicts the noise (epsilon), or the samples instead of the noise.
-
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the samples. One of `epsilon`, `sample`.
+            `v-prediction` is not supported for this scheduler.
     """
 
     _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[np.ndarray] = None,
         variance_type: str = "fixed_small",
         clip_sample: bool = True,
-        predict_epsilon: bool = True,
+        prediction_type: str = "epsilon",
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
+
         if trained_betas is not None:
             self.betas = torch.from_numpy(trained_betas)
         elif beta_schedule == "linear":
             self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = (
@@ -237,21 +247,21 @@
         Returns:
             [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
         """
         message = (
-            "Please make sure to instantiate your scheduler with `predict_epsilon` instead. E.g. `scheduler ="
-            " DDPMScheduler.from_pretrained(<model_id>, predict_epsilon=True)`."
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
         )
         predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
-        if predict_epsilon is not None and predict_epsilon != self.config.predict_epsilon:
+        if predict_epsilon is not None:
             new_config = dict(self.config)
-            new_config["predict_epsilon"] = predict_epsilon
+            new_config["prediction_type"] = "epsilon" if predict_epsilon else "sample"
             self._internal_dict = FrozenDict(new_config)
 
         t = timestep
 
         if model_output.shape[1] == sample.shape[1] * 2 and self.variance_type in ["learned", "learned_range"]:
             model_output, predicted_variance = torch.split(model_output, sample.shape[1], dim=1)
         else:
@@ -261,18 +271,23 @@
         alpha_prod_t = self.alphas_cumprod[t]
         alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
         beta_prod_t = 1 - alpha_prod_t
         beta_prod_t_prev = 1 - alpha_prod_t_prev
 
         # 2. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        if self.config.predict_epsilon:
+        if self.config.prediction_type == "epsilon":
             pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
-        else:
+        elif self.config.prediction_type == "sample":
             pred_original_sample = model_output
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample` "
+                " for the DDPMScheduler."
+            )
 
         # 3. Clip "predicted x_0"
         if self.config.clip_sample:
             pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
 
         # 4. Compute coefficients for pred_original_sample x_0 and current sample x_t
         # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_ddpm_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_repaint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,304 +1,322 @@
-# Copyright 2022 UC Berkeley Team and The HuggingFace Team. All rights reserved.
+# Copyright 2022 ETH Zurich Computer Vision Lab and The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# DISCLAIMER: This file is strongly influenced by https://github.com/ermongroup/ddim
-
 import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
-import flax
-import jax.numpy as jnp
-from jax import random
-
-from ..configuration_utils import ConfigMixin, FrozenDict, register_to_config
-from ..utils import deprecate
-from .scheduling_utils_flax import (
-    _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
-    FlaxSchedulerMixin,
-    FlaxSchedulerOutput,
-    broadcast_to_shape_from_left,
-)
+import numpy as np
+import torch
+
+from ..configuration_utils import ConfigMixin, register_to_config
+from ..utils import BaseOutput
+from .scheduling_utils import SchedulerMixin
+
+
+@dataclass
+class RePaintSchedulerOutput(BaseOutput):
+    """
+    Output class for the scheduler's step function output.
+
+    Args:
+        prev_sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
+            Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
+            denoising loop.
+        pred_original_sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
+            The predicted denoised sample (x_{0}) based on the model output from
+             the current timestep. `pred_original_sample` can be used to preview progress or for guidance.
+    """
+
+    prev_sample: torch.FloatTensor
+    pred_original_sample: torch.FloatTensor
 
 
-def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999) -> jnp.ndarray:
+def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
     Contains a function alpha_bar that takes an argument t and transforms it to the cumulative product of (1-beta) up
     to that part of the diffusion process.
 
 
     Args:
         num_diffusion_timesteps (`int`): the number of betas to produce.
         max_beta (`float`): the maximum beta to use; use values lower than 1 to
                      prevent singularities.
 
     Returns:
-        betas (`jnp.ndarray`): the betas used by the scheduler to step the model outputs
+        betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
     """
 
     def alpha_bar(time_step):
         return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
 
     betas = []
     for i in range(num_diffusion_timesteps):
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
-    return jnp.array(betas, dtype=jnp.float32)
-
-
-@flax.struct.dataclass
-class DDPMSchedulerState:
-    # setable values
-    timesteps: jnp.ndarray
-    num_inference_steps: Optional[int] = None
-
-    @classmethod
-    def create(cls, num_train_timesteps: int):
-        return cls(timesteps=jnp.arange(0, num_train_timesteps)[::-1])
+    return torch.tensor(betas, dtype=torch.float32)
 
 
-@dataclass
-class FlaxDDPMSchedulerOutput(FlaxSchedulerOutput):
-    state: DDPMSchedulerState
-
-
-class FlaxDDPMScheduler(FlaxSchedulerMixin, ConfigMixin):
+class RePaintScheduler(SchedulerMixin, ConfigMixin):
     """
-    Denoising diffusion probabilistic models (DDPMs) explores the connections between denoising score matching and
-    Langevin dynamics sampling.
+    RePaint is a schedule for DDPM inpainting inside a given mask.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
     [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
     [`~SchedulerMixin.from_pretrained`] functions.
 
-    For more details, see the original paper: https://arxiv.org/abs/2006.11239
+    For more details, see the original paper: https://arxiv.org/pdf/2201.09865.pdf
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
+        eta (`float`):
+            The weight of noise for added noise in a diffusion step. Its value is between 0.0 and 1.0 -0.0 is DDIM and
+            1.0 is DDPM scheduler respectively.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         variance_type (`str`):
             options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
             `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
-        predict_epsilon (`bool`):
-            optional flag to use when the model predicts the noise (epsilon), or the samples instead of the noise.
 
     """
 
-    _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
-
-    @property
-    def has_state(self):
-        return True
-
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[jnp.ndarray] = None,
-        variance_type: str = "fixed_small",
+        eta: float = 0.0,
+        trained_betas: Optional[np.ndarray] = None,
         clip_sample: bool = True,
-        predict_epsilon: bool = True,
     ):
         if trained_betas is not None:
-            self.betas = jnp.asarray(trained_betas)
+            self.betas = torch.from_numpy(trained_betas)
         elif beta_schedule == "linear":
-            self.betas = jnp.linspace(beta_start, beta_end, num_train_timesteps, dtype=jnp.float32)
+            self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = jnp.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=jnp.float32) ** 2
+            self.betas = (
+                torch.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=torch.float32) ** 2
+            )
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
+        elif beta_schedule == "sigmoid":
+            # GeoDiff sigmoid schedule
+            betas = torch.linspace(-6, 6, num_train_timesteps)
+            self.betas = torch.sigmoid(betas) * (beta_end - beta_start) + beta_start
         else:
             raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
-        self.alphas_cumprod = jnp.cumprod(self.alphas, axis=0)
-        self.one = jnp.array(1.0)
+        self.alphas_cumprod = torch.cumprod(self.alphas, dim=0)
+        self.one = torch.tensor(1.0)
 
-    def create_state(self):
-        return DDPMSchedulerState.create(num_train_timesteps=self.config.num_train_timesteps)
+        self.final_alpha_cumprod = torch.tensor(1.0)
 
-    def set_timesteps(
-        self, state: DDPMSchedulerState, num_inference_steps: int, shape: Tuple = ()
-    ) -> DDPMSchedulerState:
+        # standard deviation of the initial noise distribution
+        self.init_noise_sigma = 1.0
+
+        # setable values
+        self.num_inference_steps = None
+        self.timesteps = torch.from_numpy(np.arange(0, num_train_timesteps)[::-1].copy())
+
+        self.eta = eta
+
+    def scale_model_input(self, sample: torch.FloatTensor, timestep: Optional[int] = None) -> torch.FloatTensor:
         """
-        Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
+        Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
+        current timestep.
 
         Args:
-            state (`DDIMSchedulerState`):
-                the `FlaxDDPMScheduler` state data class instance.
-            num_inference_steps (`int`):
-                the number of diffusion steps used when generating samples with a pre-trained model.
+            sample (`torch.FloatTensor`): input sample
+            timestep (`int`, optional): current timestep
+
+        Returns:
+            `torch.FloatTensor`: scaled input sample
         """
+        return sample
+
+    def set_timesteps(
+        self,
+        num_inference_steps: int,
+        jump_length: int = 10,
+        jump_n_sample: int = 10,
+        device: Union[str, torch.device] = None,
+    ):
         num_inference_steps = min(self.config.num_train_timesteps, num_inference_steps)
-        timesteps = jnp.arange(
-            0, self.config.num_train_timesteps, self.config.num_train_timesteps // num_inference_steps
-        )[::-1]
-        return state.replace(num_inference_steps=num_inference_steps, timesteps=timesteps)
+        self.num_inference_steps = num_inference_steps
+
+        timesteps = []
+
+        jumps = {}
+        for j in range(0, num_inference_steps - jump_length, jump_length):
+            jumps[j] = jump_n_sample - 1
+
+        t = num_inference_steps
+        while t >= 1:
+            t = t - 1
+            timesteps.append(t)
+
+            if jumps.get(t, 0) > 0:
+                jumps[t] = jumps[t] - 1
+                for _ in range(jump_length):
+                    t = t + 1
+                    timesteps.append(t)
+
+        timesteps = np.array(timesteps) * (self.config.num_train_timesteps // self.num_inference_steps)
+        self.timesteps = torch.from_numpy(timesteps).to(device)
+
+    def _get_variance(self, t):
+        prev_timestep = t - self.config.num_train_timesteps // self.num_inference_steps
 
-    def _get_variance(self, t, predicted_variance=None, variance_type=None):
         alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        beta_prod_t = 1 - alpha_prod_t
+        beta_prod_t_prev = 1 - alpha_prod_t_prev
 
-        # For t > 0, compute predicted variance βt (see formula (6) and (7) from https://arxiv.org/pdf/2006.11239.pdf)
-        # and sample from it to get previous sample
-        # x_{t-1} ~ N(pred_prev_sample, variance) == add variance to pred_sample
-        variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
-
-        if variance_type is None:
-            variance_type = self.config.variance_type
-
-        # hacks - were probably added for training stability
-        if variance_type == "fixed_small":
-            variance = jnp.clip(variance, a_min=1e-20)
-        # for rl-diffuser https://arxiv.org/abs/2205.09991
-        elif variance_type == "fixed_small_log":
-            variance = jnp.log(jnp.clip(variance, a_min=1e-20))
-        elif variance_type == "fixed_large":
-            variance = self.betas[t]
-        elif variance_type == "fixed_large_log":
-            # Glide max_log
-            variance = jnp.log(self.betas[t])
-        elif variance_type == "learned":
-            return predicted_variance
-        elif variance_type == "learned_range":
-            min_log = variance
-            max_log = self.betas[t]
-            frac = (predicted_variance + 1) / 2
-            variance = frac * max_log + (1 - frac) * min_log
+        # For t > 0, compute predicted variance βt (see formula (6) and (7) from
+        # https://arxiv.org/pdf/2006.11239.pdf) and sample from it to get
+        # previous sample x_{t-1} ~ N(pred_prev_sample, variance) == add
+        # variance to pred_sample
+        # Is equivalent to formula (16) in https://arxiv.org/pdf/2010.02502.pdf
+        # without eta.
+        # variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
+        variance = (beta_prod_t_prev / beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
 
         return variance
 
     def step(
         self,
-        state: DDPMSchedulerState,
-        model_output: jnp.ndarray,
+        model_output: torch.FloatTensor,
         timestep: int,
-        sample: jnp.ndarray,
-        key: random.KeyArray,
-        predict_epsilon: bool = True,
+        sample: torch.FloatTensor,
+        original_image: torch.FloatTensor,
+        mask: torch.FloatTensor,
+        generator: Optional[torch.Generator] = None,
         return_dict: bool = True,
-        **kwargs,
-    ) -> Union[FlaxDDPMSchedulerOutput, Tuple]:
+    ) -> Union[RePaintSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
-            state (`DDPMSchedulerState`): the `FlaxDDPMScheduler` state data class instance.
-            model_output (`jnp.ndarray`): direct output from learned diffusion model.
+            model_output (`torch.FloatTensor`): direct output from learned
+                diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
-            sample (`jnp.ndarray`):
+            sample (`torch.FloatTensor`):
                 current instance of sample being created by diffusion process.
-            key (`random.KeyArray`): a PRNG key.
-            return_dict (`bool`): option for returning tuple rather than FlaxDDPMSchedulerOutput class
+            original_image (`torch.FloatTensor`):
+                the original image to inpaint on.
+            mask (`torch.FloatTensor`):
+                the mask where 0.0 values define which part of the original image to inpaint (change).
+            generator (`torch.Generator`, *optional*): random number generator.
+            return_dict (`bool`): option for returning tuple rather than
+                DDPMSchedulerOutput class
 
         Returns:
-            [`FlaxDDPMSchedulerOutput`] or `tuple`: [`FlaxDDPMSchedulerOutput`] if `return_dict` is True, otherwise a
-            `tuple`. When returning a tuple, the first element is the sample tensor.
+            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] or `tuple`:
+            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            returning a tuple, the first element is the sample tensor.
 
         """
-        message = (
-            "Please make sure to instantiate your scheduler with `predict_epsilon` instead. E.g. `scheduler ="
-            " DDPMScheduler.from_pretrained(<model_id>, predict_epsilon=True)`."
-        )
-        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
-        if predict_epsilon is not None and predict_epsilon != self.config.predict_epsilon:
-            new_config = dict(self.config)
-            new_config["predict_epsilon"] = predict_epsilon
-            self._internal_dict = FrozenDict(new_config)
-
         t = timestep
-
-        if model_output.shape[1] == sample.shape[1] * 2 and self.config.variance_type in ["learned", "learned_range"]:
-            model_output, predicted_variance = jnp.split(model_output, sample.shape[1], axis=1)
-        else:
-            predicted_variance = None
+        prev_timestep = timestep - self.config.num_train_timesteps // self.num_inference_steps
 
         # 1. compute alphas, betas
         alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
         beta_prod_t = 1 - alpha_prod_t
-        beta_prod_t_prev = 1 - alpha_prod_t_prev
 
         # 2. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        if self.config.predict_epsilon:
-            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
-        else:
-            pred_original_sample = model_output
+        pred_original_sample = (sample - beta_prod_t**0.5 * model_output) / alpha_prod_t**0.5
 
         # 3. Clip "predicted x_0"
         if self.config.clip_sample:
-            pred_original_sample = jnp.clip(pred_original_sample, -1, 1)
+            pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
 
-        # 4. Compute coefficients for pred_original_sample x_0 and current sample x_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_original_sample_coeff = (alpha_prod_t_prev ** (0.5) * self.betas[t]) / beta_prod_t
-        current_sample_coeff = self.alphas[t] ** (0.5) * beta_prod_t_prev / beta_prod_t
-
-        # 5. Compute predicted previous sample µ_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_prev_sample = pred_original_sample_coeff * pred_original_sample + current_sample_coeff * sample
+        # We choose to follow RePaint Algorithm 1 to get x_{t-1}, however we
+        # substitute formula (7) in the algorithm coming from DDPM paper
+        # (formula (4) Algorithm 2 - Sampling) with formula (12) from DDIM paper.
+        # DDIM schedule gives the same results as DDPM with eta = 1.0
+        # Noise is being reused in 7. and 8., but no impact on quality has
+        # been observed.
+
+        # 5. Add noise
+        noise = torch.randn(
+            model_output.shape, dtype=model_output.dtype, generator=generator, device=model_output.device
+        )
+        std_dev_t = self.eta * self._get_variance(timestep) ** 0.5
 
-        # 6. Add noise
         variance = 0
-        if t > 0:
-            key = random.split(key, num=1)
-            noise = random.normal(key=key, shape=model_output.shape)
-            variance = (self._get_variance(t, predicted_variance=predicted_variance) ** 0.5) * noise
+        if t > 0 and self.eta > 0:
+            variance = std_dev_t * noise
+
+        # 6. compute "direction pointing to x_t" of formula (12)
+        # from https://arxiv.org/pdf/2010.02502.pdf
+        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** 0.5 * model_output
+
+        # 7. compute x_{t-1} of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
+        prev_unknown_part = alpha_prod_t_prev**0.5 * pred_original_sample + pred_sample_direction + variance
 
-        pred_prev_sample = pred_prev_sample + variance
+        # 8. Algorithm 1 Line 5 https://arxiv.org/pdf/2201.09865.pdf
+        prev_known_part = (alpha_prod_t**0.5) * original_image + ((1 - alpha_prod_t) ** 0.5) * noise
+
+        # 9. Algorithm 1 Line 8 https://arxiv.org/pdf/2201.09865.pdf
+        pred_prev_sample = mask * prev_known_part + (1.0 - mask) * prev_unknown_part
 
         if not return_dict:
-            return (pred_prev_sample, state)
+            return (
+                pred_prev_sample,
+                pred_original_sample,
+            )
+
+        return RePaintSchedulerOutput(prev_sample=pred_prev_sample, pred_original_sample=pred_original_sample)
+
+    def undo_step(self, sample, timestep, generator=None):
+        n = self.config.num_train_timesteps // self.num_inference_steps
 
-        return FlaxDDPMSchedulerOutput(prev_sample=pred_prev_sample, state=state)
+        for i in range(n):
+            beta = self.betas[timestep + i]
+            noise = torch.randn(sample.shape, generator=generator, device=sample.device)
+
+            # 10. Algorithm 1 Line 10 https://arxiv.org/pdf/2201.09865.pdf
+            sample = (1 - beta) ** 0.5 * sample + beta**0.5 * noise
+
+        return sample
 
     def add_noise(
         self,
-        original_samples: jnp.ndarray,
-        noise: jnp.ndarray,
-        timesteps: jnp.ndarray,
-    ) -> jnp.ndarray:
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
-        sqrt_alpha_prod = sqrt_alpha_prod.flatten()
-        sqrt_alpha_prod = broadcast_to_shape_from_left(sqrt_alpha_prod, original_samples.shape)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        sqrt_one_minus_alpha_prod = broadcast_to_shape_from_left(sqrt_one_minus_alpha_prod, original_samples.shape)
-
-        noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
-        return noisy_samples
+        original_samples: torch.FloatTensor,
+        noise: torch.FloatTensor,
+        timesteps: torch.IntTensor,
+    ) -> torch.FloatTensor:
+        raise NotImplementedError("Use `DDPMScheduler.add_noise()` to train for sampling with RePaint.")
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_dpmsolver_multistep.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import math
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, deprecate
 from .scheduling_utils import SchedulerMixin, SchedulerOutput
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
@@ -83,18 +83,17 @@
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         solver_order (`int`, default `2`):
             the order of DPM-Solver; can be `1` or `2` or `3`. We recommend to use `solver_order=2` for guided
             sampling, and `solver_order=3` for unconditional sampling.
-        predict_epsilon (`bool`, default `True`):
-            we currently support both the noise prediction model and the data prediction model. If the model predicts
-            the noise / epsilon, set `predict_epsilon` to `True`. If the model predicts the data / x0 directly, set
-            `predict_epsilon` to `False`.
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the data / `x0`. One of `epsilon`, `sample`,
+            or `v-prediction`.
         thresholding (`bool`, default `False`):
             whether to use the "dynamic thresholding" method (introduced by Imagen, https://arxiv.org/abs/2205.11487).
             For pixel-space diffusion models, you can set both `algorithm_type=dpmsolver++` and `thresholding=True` to
             use the dynamic thresholding. Note that the thresholding method is unsuitable for latent-space diffusion
             models (such as stable-diffusion).
         dynamic_thresholding_ratio (`float`, default `0.995`):
             the ratio for the dynamic thresholding method. Default is `0.995`, the same as Imagen
@@ -114,32 +113,42 @@
         lower_order_final (`bool`, default `True`):
             whether to use lower-order solvers in the final steps. Only valid for < 15 inference steps. We empirically
             find this trick can stabilize the sampling of DPM-Solver for steps < 15, especially for steps <= 10.
 
     """
 
     _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[np.ndarray] = None,
         solver_order: int = 2,
-        predict_epsilon: bool = True,
+        prediction_type: str = "epsilon",
         thresholding: bool = False,
         dynamic_thresholding_ratio: float = 0.995,
         sample_max_value: float = 1.0,
         algorithm_type: str = "dpmsolver++",
         solver_type: str = "midpoint",
         lower_order_final: bool = True,
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DPMSolverMultistepScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
+
         if trained_betas is not None:
             self.betas = torch.from_numpy(trained_betas)
         elif beta_schedule == "linear":
             self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = (
@@ -199,15 +208,15 @@
 
     def convert_model_output(
         self, model_output: torch.FloatTensor, timestep: int, sample: torch.FloatTensor
     ) -> torch.FloatTensor:
         """
         Convert the model output to the corresponding type that the algorithm (DPM-Solver / DPM-Solver++) needs.
 
-        DPM-Solver is designed to discretize an integral of the noise prediciton model, and DPM-Solver++ is designed to
+        DPM-Solver is designed to discretize an integral of the noise prediction model, and DPM-Solver++ is designed to
         discretize an integral of the data prediction model. So we need to first convert the model output to the
         corresponding type to match the algorithm.
 
         Note that the algorithm type and the model type is decoupled. That is to say, we can use either DPM-Solver or
         DPM-Solver++ for both noise prediction model and data prediction model.
 
         Args:
@@ -217,38 +226,56 @@
                 current instance of sample being created by diffusion process.
 
         Returns:
             `torch.FloatTensor`: the converted model output.
         """
         # DPM-Solver++ needs to solve an integral of the data prediction model.
         if self.config.algorithm_type == "dpmsolver++":
-            if self.config.predict_epsilon:
+            if self.config.prediction_type == "epsilon":
                 alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 x0_pred = (sample - sigma_t * model_output) / alpha_t
-            else:
+            elif self.config.prediction_type == "sample":
                 x0_pred = model_output
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                x0_pred = alpha_t * sample - sigma_t * model_output
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                    " `v_prediction` for the DPMSolverMultistepScheduler."
+                )
+
             if self.config.thresholding:
                 # Dynamic thresholding in https://arxiv.org/abs/2205.11487
                 dynamic_max_val = torch.quantile(
                     torch.abs(x0_pred).reshape((x0_pred.shape[0], -1)), self.config.dynamic_thresholding_ratio, dim=1
                 )
                 dynamic_max_val = torch.maximum(
                     dynamic_max_val,
                     self.config.sample_max_value * torch.ones_like(dynamic_max_val).to(dynamic_max_val.device),
                 )[(...,) + (None,) * (x0_pred.ndim - 1)]
                 x0_pred = torch.clamp(x0_pred, -dynamic_max_val, dynamic_max_val) / dynamic_max_val
             return x0_pred
         # DPM-Solver needs to solve an integral of the noise prediction model.
         elif self.config.algorithm_type == "dpmsolver":
-            if self.config.predict_epsilon:
+            if self.config.prediction_type == "epsilon":
                 return model_output
-            else:
+            elif self.config.prediction_type == "sample":
                 alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 epsilon = (sample - alpha_t * model_output) / sigma_t
                 return epsilon
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                epsilon = alpha_t * model_output + sigma_t * sample
+                return epsilon
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                    " `v_prediction` for the DPMSolverMultistepScheduler."
+                )
 
     def dpm_solver_first_order_update(
         self,
         model_output: torch.FloatTensor,
         timestep: int,
         prev_timestep: int,
         sample: torch.FloatTensor,
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import List, Optional, Tuple, Union
 
 import flax
 import jax
 import jax.numpy as jnp
 
 from ..configuration_utils import ConfigMixin, register_to_config
+from ..utils import deprecate
 from .scheduling_utils_flax import (
     _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
     FlaxSchedulerMixin,
     FlaxSchedulerOutput,
     broadcast_to_shape_from_left,
 )
 
@@ -114,18 +115,17 @@
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         solver_order (`int`, default `2`):
             the order of DPM-Solver; can be `1` or `2` or `3`. We recommend to use `solver_order=2` for guided
             sampling, and `solver_order=3` for unconditional sampling.
-        predict_epsilon (`bool`, default `True`):
-            we currently support both the noise prediction model and the data prediction model. If the model predicts
-            the noise / epsilon, set `predict_epsilon` to `True`. If the model predicts the data / x0 directly, set
-            `predict_epsilon` to `False`.
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the data / `x0`. One of `epsilon`, `sample`,
+            or `v-prediction`.
         thresholding (`bool`, default `False`):
             whether to use the "dynamic thresholding" method (introduced by Imagen, https://arxiv.org/abs/2205.11487).
             For pixel-space diffusion models, you can set both `algorithm_type=dpmsolver++` and `thresholding=True` to
             use the dynamic thresholding. Note that the thresholding method is unsuitable for latent-space diffusion
             models (such as stable-diffusion).
         dynamic_thresholding_ratio (`float`, default `0.995`):
             the ratio for the dynamic thresholding method. Default is `0.995`, the same as Imagen
@@ -145,36 +145,46 @@
         lower_order_final (`bool`, default `True`):
             whether to use lower-order solvers in the final steps. Only valid for < 15 inference steps. We empirically
             find this trick can stabilize the sampling of DPM-Solver for steps < 15, especially for steps <= 10.
 
     """
 
     _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
 
     @property
     def has_state(self):
         return True
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[jnp.ndarray] = None,
         solver_order: int = 2,
-        predict_epsilon: bool = True,
+        prediction_type: str = "epsilon",
         thresholding: bool = False,
         dynamic_thresholding_ratio: float = 0.995,
         sample_max_value: float = 1.0,
         algorithm_type: str = "dpmsolver++",
         solver_type: str = "midpoint",
         lower_order_final: bool = True,
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " FlaxDPMSolverMultistepScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
+
         if trained_betas is not None:
             self.betas = jnp.asarray(trained_betas)
         elif beta_schedule == "linear":
             self.betas = jnp.linspace(beta_start, beta_end, num_train_timesteps, dtype=jnp.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = jnp.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=jnp.float32) ** 2
@@ -238,15 +248,15 @@
         model_output: jnp.ndarray,
         timestep: int,
         sample: jnp.ndarray,
     ) -> jnp.ndarray:
         """
         Convert the model output to the corresponding type that the algorithm (DPM-Solver / DPM-Solver++) needs.
 
-        DPM-Solver is designed to discretize an integral of the noise prediciton model, and DPM-Solver++ is designed to
+        DPM-Solver is designed to discretize an integral of the noise prediction model, and DPM-Solver++ is designed to
         discretize an integral of the data prediction model. So we need to first convert the model output to the
         corresponding type to match the algorithm.
 
         Note that the algorithm type and the model type is decoupled. That is to say, we can use either DPM-Solver or
         DPM-Solver++ for both noise prediction model and data prediction model.
 
         Args:
@@ -256,37 +266,55 @@
                 current instance of sample being created by diffusion process.
 
         Returns:
             `jnp.ndarray`: the converted model output.
         """
         # DPM-Solver++ needs to solve an integral of the data prediction model.
         if self.config.algorithm_type == "dpmsolver++":
-            if self.config.predict_epsilon:
+            if self.config.prediction_type == "epsilon":
                 alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 x0_pred = (sample - sigma_t * model_output) / alpha_t
-            else:
+            elif self.config.prediction_type == "sample":
                 x0_pred = model_output
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                x0_pred = alpha_t * sample - sigma_t * model_output
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, "
+                    " or `v_prediction` for the FlaxDPMSolverMultistepScheduler."
+                )
+
             if self.config.thresholding:
                 # Dynamic thresholding in https://arxiv.org/abs/2205.11487
                 dynamic_max_val = jnp.percentile(
                     jnp.abs(x0_pred), self.config.dynamic_thresholding_ratio, axis=tuple(range(1, x0_pred.ndim))
                 )
                 dynamic_max_val = jnp.maximum(
                     dynamic_max_val, self.config.sample_max_value * jnp.ones_like(dynamic_max_val)
                 )
                 x0_pred = jnp.clip(x0_pred, -dynamic_max_val, dynamic_max_val) / dynamic_max_val
             return x0_pred
         # DPM-Solver needs to solve an integral of the noise prediction model.
         elif self.config.algorithm_type == "dpmsolver":
-            if self.config.predict_epsilon:
+            if self.config.prediction_type == "epsilon":
                 return model_output
-            else:
+            elif self.config.prediction_type == "sample":
                 alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 epsilon = (sample - alpha_t * model_output) / sigma_t
                 return epsilon
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                epsilon = alpha_t * model_output + sigma_t * sample
+                return epsilon
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, "
+                    " or `v_prediction` for the FlaxDPMSolverMultistepScheduler."
+                )
 
     def dpm_solver_first_order_update(
         self, model_output: jnp.ndarray, timestep: int, prev_timestep: int, sample: jnp.ndarray
     ) -> jnp.ndarray:
         """
         One step for the first-order DPM-Solver (equivalent to DDIM).
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_euler_discrete.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_euler_discrete.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[np.ndarray] = None,
+        prediction_type: str = "epsilon",
     ):
         if trained_betas is not None:
             self.betas = torch.from_numpy(trained_betas)
         elif beta_schedule == "linear":
             self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
@@ -225,15 +226,23 @@
         eps = noise * s_noise
         sigma_hat = sigma * (gamma + 1)
 
         if gamma > 0:
             sample = sample + eps * (sigma_hat**2 - sigma**2) ** 0.5
 
         # 1. compute predicted original sample (x_0) from sigma-scaled predicted noise
-        pred_original_sample = sample - sigma_hat * model_output
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = sample - sigma_hat * model_output
+        elif self.config.prediction_type == "v_prediction":
+            # * c_out + input * c_skip
+            pred_original_sample = model_output * (-sigma / (sigma**2 + 1) ** 0.5) + (sample / (sigma**2 + 1))
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, or `v_prediction`"
+            )
 
         # 2. Convert to an ODE derivative
         derivative = (sample - pred_original_sample) / sigma_hat
 
         dt = self.sigmas[step_index + 1] - sigma_hat
 
         prev_sample = sample + derivative * dt
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_ipndm.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_ipndm.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_karras_ve.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_karras_ve.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_karras_ve_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_lms_discrete.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_lms_discrete_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_pndm.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_pndm.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_pndm_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_pndm_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_repaint.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_ve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,92 @@
-# Copyright 2022 ETH Zurich Computer Vision Lab and The HuggingFace Team. All rights reserved.
+# Copyright 2022 Google Brain and The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# DISCLAIMER: This file is strongly influenced by https://github.com/yang-song/score_sde_pytorch
+
 import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
-import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..utils import BaseOutput
-from .scheduling_utils import SchedulerMixin
+from .scheduling_utils import SchedulerMixin, SchedulerOutput
 
 
 @dataclass
-class RePaintSchedulerOutput(BaseOutput):
+class SdeVeOutput(BaseOutput):
     """
-    Output class for the scheduler's step function output.
+    Output class for the ScoreSdeVeScheduler's step function output.
 
     Args:
         prev_sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
             denoising loop.
-        pred_original_sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
-            The predicted denoised sample (x_{0}) based on the model output from
-             the current timestep. `pred_original_sample` can be used to preview progress or for guidance.
+        prev_sample_mean (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
+            Mean averaged `prev_sample`. Same as `prev_sample`, only mean-averaged over previous timesteps.
     """
 
     prev_sample: torch.FloatTensor
-    pred_original_sample: torch.FloatTensor
-
-
-def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
-    """
-    Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
-    (1-beta) over time from t = [0,1].
+    prev_sample_mean: torch.FloatTensor
 
-    Contains a function alpha_bar that takes an argument t and transforms it to the cumulative product of (1-beta) up
-    to that part of the diffusion process.
-
-
-    Args:
-        num_diffusion_timesteps (`int`): the number of betas to produce.
-        max_beta (`float`): the maximum beta to use; use values lower than 1 to
-                     prevent singularities.
 
-    Returns:
-        betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
+class ScoreSdeVeScheduler(SchedulerMixin, ConfigMixin):
     """
+    The variance exploding stochastic differential equation (SDE) scheduler.
 
-    def alpha_bar(time_step):
-        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
-
-    betas = []
-    for i in range(num_diffusion_timesteps):
-        t1 = i / num_diffusion_timesteps
-        t2 = (i + 1) / num_diffusion_timesteps
-        betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
-    return torch.tensor(betas, dtype=torch.float32)
-
-
-class RePaintScheduler(SchedulerMixin, ConfigMixin):
-    """
-    RePaint is a schedule for DDPM inpainting inside a given mask.
+    For more information, see the original paper: https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
     [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
     [`~SchedulerMixin.from_pretrained`] functions.
 
-    For more details, see the original paper: https://arxiv.org/pdf/2201.09865.pdf
-
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
-        beta_start (`float`): the starting `beta` value of inference.
-        beta_end (`float`): the final `beta` value.
-        beta_schedule (`str`):
-            the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
-            `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
-        eta (`float`):
-            The weight of noise for added noise in a diffusion step. Its value is between 0.0 and 1.0 -0.0 is DDIM and
-            1.0 is DDPM scheduler respectively.
-        trained_betas (`np.ndarray`, optional):
-            option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
-        variance_type (`str`):
-            options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
-            `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
-        clip_sample (`bool`, default `True`):
-            option to clip predicted sample between -1 and 1 for numerical stability.
-
+        snr (`float`):
+            coefficient weighting the step from the model_output sample (from the network) to the random noise.
+        sigma_min (`float`):
+                initial noise scale for sigma sequence in sampling procedure. The minimum sigma should mirror the
+                distribution of the data.
+        sigma_max (`float`): maximum value used for the range of continuous timesteps passed into the model.
+        sampling_eps (`float`): the end value of sampling, where timesteps decrease progressively from 1 to
+        epsilon.
+        correct_steps (`int`): number of correction steps performed on a produced sample.
     """
 
     @register_to_config
     def __init__(
         self,
-        num_train_timesteps: int = 1000,
-        beta_start: float = 0.0001,
-        beta_end: float = 0.02,
-        beta_schedule: str = "linear",
-        eta: float = 0.0,
-        trained_betas: Optional[np.ndarray] = None,
-        clip_sample: bool = True,
+        num_train_timesteps: int = 2000,
+        snr: float = 0.15,
+        sigma_min: float = 0.01,
+        sigma_max: float = 1348.0,
+        sampling_eps: float = 1e-5,
+        correct_steps: int = 1,
     ):
-        if trained_betas is not None:
-            self.betas = torch.from_numpy(trained_betas)
-        elif beta_schedule == "linear":
-            self.betas = torch.linspace(beta_start, beta_end, num_train_timesteps, dtype=torch.float32)
-        elif beta_schedule == "scaled_linear":
-            # this schedule is very specific to the latent diffusion model.
-            self.betas = (
-                torch.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype=torch.float32) ** 2
-            )
-        elif beta_schedule == "squaredcos_cap_v2":
-            # Glide cosine schedule
-            self.betas = betas_for_alpha_bar(num_train_timesteps)
-        elif beta_schedule == "sigmoid":
-            # GeoDiff sigmoid schedule
-            betas = torch.linspace(-6, 6, num_train_timesteps)
-            self.betas = torch.sigmoid(betas) * (beta_end - beta_start) + beta_start
-        else:
-            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
-
-        self.alphas = 1.0 - self.betas
-        self.alphas_cumprod = torch.cumprod(self.alphas, dim=0)
-        self.one = torch.tensor(1.0)
-
-        self.final_alpha_cumprod = torch.tensor(1.0)
-
         # standard deviation of the initial noise distribution
-        self.init_noise_sigma = 1.0
+        self.init_noise_sigma = sigma_max
 
         # setable values
-        self.num_inference_steps = None
-        self.timesteps = torch.from_numpy(np.arange(0, num_train_timesteps)[::-1].copy())
+        self.timesteps = None
 
-        self.eta = eta
+        self.set_sigmas(num_train_timesteps, sigma_min, sigma_max, sampling_eps)
 
     def scale_model_input(self, sample: torch.FloatTensor, timestep: Optional[int] = None) -> torch.FloatTensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
@@ -158,165 +95,170 @@
 
         Returns:
             `torch.FloatTensor`: scaled input sample
         """
         return sample
 
     def set_timesteps(
-        self,
-        num_inference_steps: int,
-        jump_length: int = 10,
-        jump_n_sample: int = 10,
-        device: Union[str, torch.device] = None,
+        self, num_inference_steps: int, sampling_eps: float = None, device: Union[str, torch.device] = None
+    ):
+        """
+        Sets the continuous timesteps used for the diffusion chain. Supporting function to be run before inference.
+
+        Args:
+            num_inference_steps (`int`):
+                the number of diffusion steps used when generating samples with a pre-trained model.
+            sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
+
+        """
+        sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
+
+        self.timesteps = torch.linspace(1, sampling_eps, num_inference_steps, device=device)
+
+    def set_sigmas(
+        self, num_inference_steps: int, sigma_min: float = None, sigma_max: float = None, sampling_eps: float = None
     ):
-        num_inference_steps = min(self.config.num_train_timesteps, num_inference_steps)
-        self.num_inference_steps = num_inference_steps
+        """
+        Sets the noise scales used for the diffusion chain. Supporting function to be run before inference.
 
-        timesteps = []
+        The sigmas control the weight of the `drift` and `diffusion` components of sample update.
 
-        jumps = {}
-        for j in range(0, num_inference_steps - jump_length, jump_length):
-            jumps[j] = jump_n_sample - 1
-
-        t = num_inference_steps
-        while t >= 1:
-            t = t - 1
-            timesteps.append(t)
-
-            if jumps.get(t, 0) > 0:
-                jumps[t] = jumps[t] - 1
-                for _ in range(jump_length):
-                    t = t + 1
-                    timesteps.append(t)
-
-        timesteps = np.array(timesteps) * (self.config.num_train_timesteps // self.num_inference_steps)
-        self.timesteps = torch.from_numpy(timesteps).to(device)
-
-    def _get_variance(self, t):
-        prev_timestep = t - self.config.num_train_timesteps // self.num_inference_steps
-
-        alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
-        beta_prod_t = 1 - alpha_prod_t
-        beta_prod_t_prev = 1 - alpha_prod_t_prev
-
-        # For t > 0, compute predicted variance βt (see formula (6) and (7) from
-        # https://arxiv.org/pdf/2006.11239.pdf) and sample from it to get
-        # previous sample x_{t-1} ~ N(pred_prev_sample, variance) == add
-        # variance to pred_sample
-        # Is equivalent to formula (16) in https://arxiv.org/pdf/2010.02502.pdf
-        # without eta.
-        # variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
-        variance = (beta_prod_t_prev / beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
+        Args:
+            num_inference_steps (`int`):
+                the number of diffusion steps used when generating samples with a pre-trained model.
+            sigma_min (`float`, optional):
+                initial noise scale value (overrides value given at Scheduler instantiation).
+            sigma_max (`float`, optional): final noise scale value (overrides value given at Scheduler instantiation).
+            sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
 
-        return variance
+        """
+        sigma_min = sigma_min if sigma_min is not None else self.config.sigma_min
+        sigma_max = sigma_max if sigma_max is not None else self.config.sigma_max
+        sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
+        if self.timesteps is None:
+            self.set_timesteps(num_inference_steps, sampling_eps)
+
+        self.sigmas = sigma_min * (sigma_max / sigma_min) ** (self.timesteps / sampling_eps)
+        self.discrete_sigmas = torch.exp(torch.linspace(math.log(sigma_min), math.log(sigma_max), num_inference_steps))
+        self.sigmas = torch.tensor([sigma_min * (sigma_max / sigma_min) ** t for t in self.timesteps])
+
+    def get_adjacent_sigma(self, timesteps, t):
+        return torch.where(
+            timesteps == 0,
+            torch.zeros_like(t.to(timesteps.device)),
+            self.discrete_sigmas[timesteps - 1].to(timesteps.device),
+        )
 
-    def step(
+    def step_pred(
         self,
         model_output: torch.FloatTensor,
         timestep: int,
         sample: torch.FloatTensor,
-        original_image: torch.FloatTensor,
-        mask: torch.FloatTensor,
         generator: Optional[torch.Generator] = None,
         return_dict: bool = True,
-    ) -> Union[RePaintSchedulerOutput, Tuple]:
+    ) -> Union[SdeVeOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
-            model_output (`torch.FloatTensor`): direct output from learned
-                diffusion model.
+            model_output (`torch.FloatTensor`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`torch.FloatTensor`):
                 current instance of sample being created by diffusion process.
-            original_image (`torch.FloatTensor`):
-                the original image to inpaint on.
-            mask (`torch.FloatTensor`):
-                the mask where 0.0 values define which part of the original image to inpaint (change).
-            generator (`torch.Generator`, *optional*): random number generator.
-            return_dict (`bool`): option for returning tuple rather than
-                DDPMSchedulerOutput class
+            generator: random number generator.
+            return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
 
         Returns:
-            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] or `tuple`:
-            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
-            returning a tuple, the first element is the sample tensor.
+            [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
+            `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
 
         """
-        t = timestep
-        prev_timestep = timestep - self.config.num_train_timesteps // self.num_inference_steps
+        if self.timesteps is None:
+            raise ValueError(
+                "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
+            )
 
-        # 1. compute alphas, betas
-        alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
-        beta_prod_t = 1 - alpha_prod_t
-
-        # 2. compute predicted original sample from predicted noise also called
-        # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_original_sample = (sample - beta_prod_t**0.5 * model_output) / alpha_prod_t**0.5
-
-        # 3. Clip "predicted x_0"
-        if self.config.clip_sample:
-            pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
-
-        # We choose to follow RePaint Algorithm 1 to get x_{t-1}, however we
-        # substitute formula (7) in the algorithm coming from DDPM paper
-        # (formula (4) Algorithm 2 - Sampling) with formula (12) from DDIM paper.
-        # DDIM schedule gives the same results as DDPM with eta = 1.0
-        # Noise is being reused in 7. and 8., but no impact on quality has
-        # been observed.
-
-        # 5. Add noise
-        noise = torch.randn(
-            model_output.shape, dtype=model_output.dtype, generator=generator, device=model_output.device
-        )
-        std_dev_t = self.eta * self._get_variance(timestep) ** 0.5
+        timestep = timestep * torch.ones(
+            sample.shape[0], device=sample.device
+        )  # torch.repeat_interleave(timestep, sample.shape[0])
+        timesteps = (timestep * (len(self.timesteps) - 1)).long()
+
+        # mps requires indices to be in the same device, so we use cpu as is the default with cuda
+        timesteps = timesteps.to(self.discrete_sigmas.device)
+
+        sigma = self.discrete_sigmas[timesteps].to(sample.device)
+        adjacent_sigma = self.get_adjacent_sigma(timesteps, timestep).to(sample.device)
+        drift = torch.zeros_like(sample)
+        diffusion = (sigma**2 - adjacent_sigma**2) ** 0.5
+
+        # equation 6 in the paper: the model_output modeled by the network is grad_x log pt(x)
+        # also equation 47 shows the analog from SDE models to ancestral sampling methods
+        diffusion = diffusion.flatten()
+        while len(diffusion.shape) < len(sample.shape):
+            diffusion = diffusion.unsqueeze(-1)
+        drift = drift - diffusion**2 * model_output
+
+        #  equation 6: sample noise for the diffusion term of
+        noise = torch.randn(sample.shape, layout=sample.layout, generator=generator).to(sample.device)
+        prev_sample_mean = sample - drift  # subtract because `dt` is a small negative timestep
+        # TODO is the variable diffusion the correct scaling term for the noise?
+        prev_sample = prev_sample_mean + diffusion * noise  # add impact of diffusion field g
 
-        variance = 0
-        if t > 0 and self.eta > 0:
-            variance = std_dev_t * noise
+        if not return_dict:
+            return (prev_sample, prev_sample_mean)
 
-        # 6. compute "direction pointing to x_t" of formula (12)
-        # from https://arxiv.org/pdf/2010.02502.pdf
-        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** 0.5 * model_output
+        return SdeVeOutput(prev_sample=prev_sample, prev_sample_mean=prev_sample_mean)
 
-        # 7. compute x_{t-1} of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        prev_unknown_part = alpha_prod_t_prev**0.5 * pred_original_sample + pred_sample_direction + variance
+    def step_correct(
+        self,
+        model_output: torch.FloatTensor,
+        sample: torch.FloatTensor,
+        generator: Optional[torch.Generator] = None,
+        return_dict: bool = True,
+    ) -> Union[SchedulerOutput, Tuple]:
+        """
+        Correct the predicted sample based on the output model_output of the network. This is often run repeatedly
+        after making the prediction for the previous timestep.
 
-        # 8. Algorithm 1 Line 5 https://arxiv.org/pdf/2201.09865.pdf
-        prev_known_part = (alpha_prod_t**0.5) * original_image + ((1 - alpha_prod_t) ** 0.5) * noise
+        Args:
+            model_output (`torch.FloatTensor`): direct output from learned diffusion model.
+            sample (`torch.FloatTensor`):
+                current instance of sample being created by diffusion process.
+            generator: random number generator.
+            return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
 
-        # 9. Algorithm 1 Line 8 https://arxiv.org/pdf/2201.09865.pdf
-        pred_prev_sample = mask * prev_known_part + (1.0 - mask) * prev_unknown_part
+        Returns:
+            [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
+            `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
 
-        if not return_dict:
-            return (
-                pred_prev_sample,
-                pred_original_sample,
+        """
+        if self.timesteps is None:
+            raise ValueError(
+                "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
-        return RePaintSchedulerOutput(prev_sample=pred_prev_sample, pred_original_sample=pred_original_sample)
+        # For small batch sizes, the paper "suggest replacing norm(z) with sqrt(d), where d is the dim. of z"
+        # sample noise for correction
+        noise = torch.randn(sample.shape, layout=sample.layout, generator=generator).to(sample.device)
+
+        # compute step size from the model_output, the noise, and the snr
+        grad_norm = torch.norm(model_output.reshape(model_output.shape[0], -1), dim=-1).mean()
+        noise_norm = torch.norm(noise.reshape(noise.shape[0], -1), dim=-1).mean()
+        step_size = (self.config.snr * noise_norm / grad_norm) ** 2 * 2
+        step_size = step_size * torch.ones(sample.shape[0]).to(sample.device)
+        # self.repeat_scalar(step_size, sample.shape[0])
+
+        # compute corrected sample: model_output term and noise term
+        step_size = step_size.flatten()
+        while len(step_size.shape) < len(sample.shape):
+            step_size = step_size.unsqueeze(-1)
+        prev_sample_mean = sample + step_size * model_output
+        prev_sample = prev_sample_mean + ((step_size * 2) ** 0.5) * noise
 
-    def undo_step(self, sample, timestep, generator=None):
-        n = self.config.num_train_timesteps // self.num_inference_steps
-
-        for i in range(n):
-            beta = self.betas[timestep + i]
-            noise = torch.randn(sample.shape, generator=generator, device=sample.device)
-
-            # 10. Algorithm 1 Line 10 https://arxiv.org/pdf/2201.09865.pdf
-            sample = (1 - beta) ** 0.5 * sample + beta**0.5 * noise
-
-        return sample
+        if not return_dict:
+            return (prev_sample,)
 
-    def add_noise(
-        self,
-        original_samples: torch.FloatTensor,
-        noise: torch.FloatTensor,
-        timesteps: torch.IntTensor,
-    ) -> torch.FloatTensor:
-        raise NotImplementedError("Use `DDPMScheduler.add_noise()` to train for sampling with RePaint.")
+        return SchedulerOutput(prev_sample=prev_sample)
 
     def __len__(self):
         return self.config.num_train_timesteps
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_sde_ve.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_ve_flax.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,43 +10,57 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # DISCLAIMER: This file is strongly influenced by https://github.com/yang-song/score_sde_pytorch
 
-import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
-import torch
+import flax
+import jax.numpy as jnp
+from jax import random
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput
-from .scheduling_utils import SchedulerMixin, SchedulerOutput
+from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
+
+
+@flax.struct.dataclass
+class ScoreSdeVeSchedulerState:
+    # setable values
+    timesteps: Optional[jnp.ndarray] = None
+    discrete_sigmas: Optional[jnp.ndarray] = None
+    sigmas: Optional[jnp.ndarray] = None
+
+    @classmethod
+    def create(cls):
+        return cls()
 
 
 @dataclass
-class SdeVeOutput(BaseOutput):
+class FlaxSdeVeOutput(FlaxSchedulerOutput):
     """
     Output class for the ScoreSdeVeScheduler's step function output.
 
     Args:
-        prev_sample (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
+        state (`ScoreSdeVeSchedulerState`):
+        prev_sample (`jnp.ndarray` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
             denoising loop.
-        prev_sample_mean (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)` for images):
+        prev_sample_mean (`jnp.ndarray` of shape `(batch_size, num_channels, height, width)` for images):
             Mean averaged `prev_sample`. Same as `prev_sample`, only mean-averaged over previous timesteps.
     """
 
-    prev_sample: torch.FloatTensor
-    prev_sample_mean: torch.FloatTensor
+    state: ScoreSdeVeSchedulerState
+    prev_sample: jnp.ndarray
+    prev_sample_mean: Optional[jnp.ndarray] = None
 
 
-class ScoreSdeVeScheduler(SchedulerMixin, ConfigMixin):
+class FlaxScoreSdeVeScheduler(FlaxSchedulerMixin, ConfigMixin):
     """
     The variance exploding stochastic differential equation (SDE) scheduler.
 
     For more information, see the original paper: https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
@@ -62,203 +76,201 @@
                 distribution of the data.
         sigma_max (`float`): maximum value used for the range of continuous timesteps passed into the model.
         sampling_eps (`float`): the end value of sampling, where timesteps decrease progressively from 1 to
         epsilon.
         correct_steps (`int`): number of correction steps performed on a produced sample.
     """
 
+    @property
+    def has_state(self):
+        return True
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 2000,
         snr: float = 0.15,
         sigma_min: float = 0.01,
         sigma_max: float = 1348.0,
         sampling_eps: float = 1e-5,
         correct_steps: int = 1,
     ):
-        # standard deviation of the initial noise distribution
-        self.init_noise_sigma = sigma_max
+        pass
 
-        # setable values
-        self.timesteps = None
-
-        self.set_sigmas(num_train_timesteps, sigma_min, sigma_max, sampling_eps)
-
-    def scale_model_input(self, sample: torch.FloatTensor, timestep: Optional[int] = None) -> torch.FloatTensor:
-        """
-        Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
-        current timestep.
-
-        Args:
-            sample (`torch.FloatTensor`): input sample
-            timestep (`int`, optional): current timestep
-
-        Returns:
-            `torch.FloatTensor`: scaled input sample
-        """
-        return sample
+    def create_state(self):
+        state = ScoreSdeVeSchedulerState.create()
+        return self.set_sigmas(
+            state,
+            self.config.num_train_timesteps,
+            self.config.sigma_min,
+            self.config.sigma_max,
+            self.config.sampling_eps,
+        )
 
     def set_timesteps(
-        self, num_inference_steps: int, sampling_eps: float = None, device: Union[str, torch.device] = None
-    ):
+        self, state: ScoreSdeVeSchedulerState, num_inference_steps: int, shape: Tuple = (), sampling_eps: float = None
+    ) -> ScoreSdeVeSchedulerState:
         """
         Sets the continuous timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
             sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
 
         """
         sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
 
-        self.timesteps = torch.linspace(1, sampling_eps, num_inference_steps, device=device)
+        timesteps = jnp.linspace(1, sampling_eps, num_inference_steps)
+        return state.replace(timesteps=timesteps)
 
     def set_sigmas(
-        self, num_inference_steps: int, sigma_min: float = None, sigma_max: float = None, sampling_eps: float = None
-    ):
+        self,
+        state: ScoreSdeVeSchedulerState,
+        num_inference_steps: int,
+        sigma_min: float = None,
+        sigma_max: float = None,
+        sampling_eps: float = None,
+    ) -> ScoreSdeVeSchedulerState:
         """
         Sets the noise scales used for the diffusion chain. Supporting function to be run before inference.
 
         The sigmas control the weight of the `drift` and `diffusion` components of sample update.
 
         Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
             sigma_min (`float`, optional):
                 initial noise scale value (overrides value given at Scheduler instantiation).
             sigma_max (`float`, optional): final noise scale value (overrides value given at Scheduler instantiation).
             sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
-
         """
         sigma_min = sigma_min if sigma_min is not None else self.config.sigma_min
         sigma_max = sigma_max if sigma_max is not None else self.config.sigma_max
         sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
-        if self.timesteps is None:
-            self.set_timesteps(num_inference_steps, sampling_eps)
+        if state.timesteps is None:
+            state = self.set_timesteps(state, num_inference_steps, sampling_eps)
 
-        self.sigmas = sigma_min * (sigma_max / sigma_min) ** (self.timesteps / sampling_eps)
-        self.discrete_sigmas = torch.exp(torch.linspace(math.log(sigma_min), math.log(sigma_max), num_inference_steps))
-        self.sigmas = torch.tensor([sigma_min * (sigma_max / sigma_min) ** t for t in self.timesteps])
-
-    def get_adjacent_sigma(self, timesteps, t):
-        return torch.where(
-            timesteps == 0,
-            torch.zeros_like(t.to(timesteps.device)),
-            self.discrete_sigmas[timesteps - 1].to(timesteps.device),
-        )
+        discrete_sigmas = jnp.exp(jnp.linspace(jnp.log(sigma_min), jnp.log(sigma_max), num_inference_steps))
+        sigmas = jnp.array([sigma_min * (sigma_max / sigma_min) ** t for t in state.timesteps])
+
+        return state.replace(discrete_sigmas=discrete_sigmas, sigmas=sigmas)
+
+    def get_adjacent_sigma(self, state, timesteps, t):
+        return jnp.where(timesteps == 0, jnp.zeros_like(t), state.discrete_sigmas[timesteps - 1])
 
     def step_pred(
         self,
-        model_output: torch.FloatTensor,
+        state: ScoreSdeVeSchedulerState,
+        model_output: jnp.ndarray,
         timestep: int,
-        sample: torch.FloatTensor,
-        generator: Optional[torch.Generator] = None,
+        sample: jnp.ndarray,
+        key: random.KeyArray,
         return_dict: bool = True,
-    ) -> Union[SdeVeOutput, Tuple]:
+    ) -> Union[FlaxSdeVeOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
-            model_output (`torch.FloatTensor`): direct output from learned diffusion model.
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            model_output (`jnp.ndarray`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
-            sample (`torch.FloatTensor`):
+            sample (`jnp.ndarray`):
                 current instance of sample being created by diffusion process.
             generator: random number generator.
-            return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
+            return_dict (`bool`): option for returning tuple rather than FlaxSdeVeOutput class
 
         Returns:
-            [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
-            `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
+            [`FlaxSdeVeOutput`] or `tuple`: [`FlaxSdeVeOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            returning a tuple, the first element is the sample tensor.
 
         """
-        if self.timesteps is None:
+        if state.timesteps is None:
             raise ValueError(
-                "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
+                "`state.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
-        timestep = timestep * torch.ones(
-            sample.shape[0], device=sample.device
-        )  # torch.repeat_interleave(timestep, sample.shape[0])
-        timesteps = (timestep * (len(self.timesteps) - 1)).long()
-
-        # mps requires indices to be in the same device, so we use cpu as is the default with cuda
-        timesteps = timesteps.to(self.discrete_sigmas.device)
-
-        sigma = self.discrete_sigmas[timesteps].to(sample.device)
-        adjacent_sigma = self.get_adjacent_sigma(timesteps, timestep).to(sample.device)
-        drift = torch.zeros_like(sample)
+        timestep = timestep * jnp.ones(
+            sample.shape[0],
+        )
+        timesteps = (timestep * (len(state.timesteps) - 1)).long()
+
+        sigma = state.discrete_sigmas[timesteps]
+        adjacent_sigma = self.get_adjacent_sigma(state, timesteps, timestep)
+        drift = jnp.zeros_like(sample)
         diffusion = (sigma**2 - adjacent_sigma**2) ** 0.5
 
         # equation 6 in the paper: the model_output modeled by the network is grad_x log pt(x)
         # also equation 47 shows the analog from SDE models to ancestral sampling methods
         diffusion = diffusion.flatten()
-        while len(diffusion.shape) < len(sample.shape):
-            diffusion = diffusion.unsqueeze(-1)
+        diffusion = broadcast_to_shape_from_left(diffusion, sample.shape)
         drift = drift - diffusion**2 * model_output
 
         #  equation 6: sample noise for the diffusion term of
-        noise = torch.randn(sample.shape, layout=sample.layout, generator=generator).to(sample.device)
+        key = random.split(key, num=1)
+        noise = random.normal(key=key, shape=sample.shape)
         prev_sample_mean = sample - drift  # subtract because `dt` is a small negative timestep
         # TODO is the variable diffusion the correct scaling term for the noise?
         prev_sample = prev_sample_mean + diffusion * noise  # add impact of diffusion field g
 
         if not return_dict:
-            return (prev_sample, prev_sample_mean)
+            return (prev_sample, prev_sample_mean, state)
 
-        return SdeVeOutput(prev_sample=prev_sample, prev_sample_mean=prev_sample_mean)
+        return FlaxSdeVeOutput(prev_sample=prev_sample, prev_sample_mean=prev_sample_mean, state=state)
 
     def step_correct(
         self,
-        model_output: torch.FloatTensor,
-        sample: torch.FloatTensor,
-        generator: Optional[torch.Generator] = None,
+        state: ScoreSdeVeSchedulerState,
+        model_output: jnp.ndarray,
+        sample: jnp.ndarray,
+        key: random.KeyArray,
         return_dict: bool = True,
-    ) -> Union[SchedulerOutput, Tuple]:
+    ) -> Union[FlaxSdeVeOutput, Tuple]:
         """
         Correct the predicted sample based on the output model_output of the network. This is often run repeatedly
         after making the prediction for the previous timestep.
 
         Args:
-            model_output (`torch.FloatTensor`): direct output from learned diffusion model.
-            sample (`torch.FloatTensor`):
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            model_output (`jnp.ndarray`): direct output from learned diffusion model.
+            sample (`jnp.ndarray`):
                 current instance of sample being created by diffusion process.
             generator: random number generator.
-            return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
+            return_dict (`bool`): option for returning tuple rather than FlaxSdeVeOutput class
 
         Returns:
-            [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
-            `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
+            [`FlaxSdeVeOutput`] or `tuple`: [`FlaxSdeVeOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            returning a tuple, the first element is the sample tensor.
 
         """
-        if self.timesteps is None:
+        if state.timesteps is None:
             raise ValueError(
-                "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
+                "`state.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
         # For small batch sizes, the paper "suggest replacing norm(z) with sqrt(d), where d is the dim. of z"
         # sample noise for correction
-        noise = torch.randn(sample.shape, layout=sample.layout, generator=generator).to(sample.device)
+        key = random.split(key, num=1)
+        noise = random.normal(key=key, shape=sample.shape)
 
         # compute step size from the model_output, the noise, and the snr
-        grad_norm = torch.norm(model_output.reshape(model_output.shape[0], -1), dim=-1).mean()
-        noise_norm = torch.norm(noise.reshape(noise.shape[0], -1), dim=-1).mean()
+        grad_norm = jnp.linalg.norm(model_output)
+        noise_norm = jnp.linalg.norm(noise)
         step_size = (self.config.snr * noise_norm / grad_norm) ** 2 * 2
-        step_size = step_size * torch.ones(sample.shape[0]).to(sample.device)
-        # self.repeat_scalar(step_size, sample.shape[0])
+        step_size = step_size * jnp.ones(sample.shape[0])
 
         # compute corrected sample: model_output term and noise term
         step_size = step_size.flatten()
-        while len(step_size.shape) < len(sample.shape):
-            step_size = step_size.unsqueeze(-1)
+        step_size = broadcast_to_shape_from_left(step_size, sample.shape)
         prev_sample_mean = sample + step_size * model_output
         prev_sample = prev_sample_mean + ((step_size * 2) ** 0.5) * noise
 
         if not return_dict:
-            return (prev_sample,)
+            return (prev_sample, state)
 
-        return SchedulerOutput(prev_sample=prev_sample)
+        return FlaxSdeVeOutput(prev_sample=prev_sample, state=state)
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_sde_vp.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_sde_vp.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_utils.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_utils_flax.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_utils_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/schedulers/scheduling_vq_diffusion.py` & `diffusers-0.9.0/src/diffusers/schedulers/scheduling_vq_diffusion.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/training_utils.py` & `diffusers-0.9.0/src/diffusers/training_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/__init__.py` & `diffusers-0.9.0/src/diffusers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/deprecation_utils.py` & `diffusers-0.9.0/src/diffusers/utils/deprecation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             values += (getattr(deprecated_kwargs, attribute),)
             warning = f"The `{attribute}` attribute is deprecated and will be removed in version {version_name}."
         elif deprecated_kwargs is None:
             warning = f"`{attribute}` is deprecated and will be removed in version {version_name}."
 
         if warning is not None:
             warning = warning + " " if standard_warn else ""
-            warnings.warn(warning + message, DeprecationWarning)
+            warnings.warn(warning + message, FutureWarning)
 
     if isinstance(deprecated_kwargs, dict) and len(deprecated_kwargs) > 0:
         call_frame = inspect.getouterframes(inspect.currentframe())[1]
         filename = call_frame.filename
         line_number = call_frame.lineno
         function = call_frame.function
         key, value = next(iter(deprecated_kwargs.items()))
```

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_flax_and_transformers_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_flax_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_pt_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_scipy_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/dummy_torch_and_transformers_objects.py` & `diffusers-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,29 @@
         requires_backends(cls, ["torch", "transformers"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch", "transformers"])
 
 
+class StableDiffusionUpscalePipeline(metaclass=DummyObject):
+    _backends = ["torch", "transformers"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["torch", "transformers"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["torch", "transformers"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["torch", "transformers"])
+
+
 class VersatileDiffusionDualGuidedPipeline(metaclass=DummyObject):
     _backends = ["torch", "transformers"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch", "transformers"])
 
     @classmethod
```

### Comparing `diffusers-0.8.1/src/diffusers/utils/import_utils.py` & `diffusers-0.9.0/src/diffusers/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/logging.py` & `diffusers-0.9.0/src/diffusers/utils/logging.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/model_card_template.md` & `diffusers-0.9.0/src/diffusers/utils/model_card_template.md`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/outputs.py` & `diffusers-0.9.0/src/diffusers/utils/outputs.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/pil_utils.py` & `diffusers-0.9.0/src/diffusers/utils/pil_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers/utils/testing_utils.py` & `diffusers-0.9.0/src/diffusers/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-0.8.1/src/diffusers.egg-info/PKG-INFO` & `diffusers-0.9.0/src/diffusers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusers
-Version: 0.8.1
+Version: 0.9.0
 Summary: Diffusers
 Home-page: https://github.com/huggingface/diffusers
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diffusers Version: 0.8.1 Summary: Diffusers Home-
+Metadata-Version: 2.1 Name: diffusers Version: 0.9.0 Summary: Diffusers Home-
 page: https://github.com/huggingface/diffusers Author: The HuggingFace team
 Author-email: patrick@huggingface.co License: Apache Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `diffusers-0.8.1/src/diffusers.egg-info/SOURCES.txt` & `diffusers-0.9.0/src/diffusers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
 src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
+src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
 src/diffusers/pipelines/stable_diffusion/safety_checker.py
 src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
 src/diffusers/pipelines/stable_diffusion_safe/__init__.py
 src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
 src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py
 src/diffusers/pipelines/stochastic_karras_ve/__init__.py
 src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
```

### Comparing `diffusers-0.8.1/src/diffusers.egg-info/requires.txt` & `diffusers-0.9.0/src/diffusers.egg-info/requires.txt`

 * *Files identical despite different names*

