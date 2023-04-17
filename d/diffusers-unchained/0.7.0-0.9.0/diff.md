# Comparing `tmp/diffusers-unchained-0.7.0.tar.gz` & `tmp/diffusers-unchained-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusers-unchained-0.7.0.tar", last modified: Fri Nov  4 00:36:31 2022, max compression
+gzip compressed data, was "diffusers-unchained-0.9.0.tar", last modified: Fri Dec  2 19:21:14 2022, max compression
```

## Comparing `diffusers-unchained-0.7.0.tar` & `diffusers-unchained-0.9.0.tar`

### file list

```diff
@@ -1,133 +1,161 @@
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.999174 diffusers-unchained-0.7.0/
--rw-r--r--   0 ghunk      (501) staff       (20)    11357 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/LICENSE
--rw-r--r--   0 ghunk      (501) staff       (20)       67 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/MANIFEST.in
--rw-r--r--   0 ghunk      (501) staff       (20)    28827 2022-11-04 00:36:30.999355 diffusers-unchained-0.7.0/PKG-INFO
--rw-r--r--   0 ghunk      (501) staff       (20)    27759 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/README.md
--rw-r--r--   0 ghunk      (501) staff       (20)       57 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/pyproject.toml
--rw-r--r--   0 ghunk      (501) staff       (20)      440 2022-11-04 00:36:30.999829 diffusers-unchained-0.7.0/setup.cfg
--rw-r--r--   0 ghunk      (501) staff       (20)     9673 2022-11-03 23:52:34.000000 diffusers-unchained-0.7.0/setup.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.969170 diffusers-unchained-0.7.0/src/
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.974408 diffusers-unchained-0.7.0/src/diffusers/
--rw-r--r--   0 ghunk      (501) staff       (20)     3799 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/__init__.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.975171 diffusers-unchained-0.7.0/src/diffusers/commands/
--rw-r--r--   0 ghunk      (501) staff       (20)      920 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/commands/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1200 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/commands/diffusers_cli.py
--rw-r--r--   0 ghunk      (501) staff       (20)     2384 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/commands/env.py
--rw-r--r--   0 ghunk      (501) staff       (20)    23721 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/configuration_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1756 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/dependency_versions_check.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1006 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/dependency_versions_table.py
--rw-r--r--   0 ghunk      (501) staff       (20)    18265 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/dynamic_modules_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)     9381 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/hub_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4599 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/modeling_flax_pytorch_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)    25838 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/modeling_flax_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)    31109 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/modeling_utils.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.978758 diffusers-unchained-0.7.0/src/diffusers/models/
--rw-r--r--   0 ghunk      (501) staff       (20)     1046 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)    28799 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/attention.py
--rw-r--r--   0 ghunk      (501) staff       (20)     9802 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/attention_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)     6297 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/embeddings.py
--rw-r--r--   0 ghunk      (501) staff       (20)     3348 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/embeddings_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    20922 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/resnet.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4021 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/resnet_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)     6980 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_1d.py
--rw-r--r--   0 ghunk      (501) staff       (20)    14802 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_1d_blocks.py
--rw-r--r--   0 ghunk      (501) staff       (20)    11429 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_2d.py
--rw-r--r--   0 ghunk      (501) staff       (20)    57549 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_blocks.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12836 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_blocks_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    15594 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_condition.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12644 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_condition_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22505 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/vae.py
--rw-r--r--   0 ghunk      (501) staff       (20)    31047 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/models/vae_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)     7474 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/onnx_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)    11363 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/optimization.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22794 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipeline_flax_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)    33164 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipeline_utils.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.978952 diffusers-unchained-0.7.0/src/diffusers/pipelines/
--rw-r--r--   0 ghunk      (501) staff       (20)     1298 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/__init__.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.979500 diffusers-unchained-0.7.0/src/diffusers/pipelines/dance_diffusion/
--rw-r--r--   0 ghunk      (501) staff       (20)       76 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/dance_diffusion/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     5173 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.979931 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddim/
--rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddim/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     5069 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddim/pipeline_ddim.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.980222 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddpm/
--rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddpm/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4073 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/ddpm/pipeline_ddpm.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.980690 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion/
--rw-r--r--   0 ghunk      (501) staff       (20)      176 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)    30321 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.981038 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion_uncond/
--rw-r--r--   0 ghunk      (501) staff       (20)       73 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion_uncond/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4193 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.981532 diffusers-unchained-0.7.0/src/diffusers/pipelines/pndm/
--rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/pndm/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4050 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/pndm/pipeline_pndm.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.981902 diffusers-unchained-0.7.0/src/diffusers/pipelines/repaint/
--rw-r--r--   0 ghunk      (501) staff       (20)       46 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/repaint/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     5897 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/repaint/pipeline_repaint.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.982186 diffusers-unchained-0.7.0/src/diffusers/pipelines/score_sde_ve/
--rw-r--r--   0 ghunk      (501) staff       (20)       69 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/score_sde_ve/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     3702 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.984860 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/
--rw-r--r--   0 ghunk      (501) staff       (20)     2861 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)    15719 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12769 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
--rw-r--r--   0 ghunk      (501) staff       (20)    20930 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22278 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22188 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22800 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-r--r--   0 ghunk      (501) staff       (20)    24831 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22661 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4632 2022-11-03 23:55:22.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/safety_checker.py
--rw-r--r--   0 ghunk      (501) staff       (20)     3878 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.985208 diffusers-unchained-0.7.0/src/diffusers/pipelines/stochastic_karras_ve/
--rw-r--r--   0 ghunk      (501) staff       (20)       75 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stochastic_karras_ve/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     5020 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.985535 diffusers-unchained-0.7.0/src/diffusers/pipelines/vq_diffusion/
--rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/vq_diffusion/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)    11942 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.995828 diffusers-unchained-0.7.0/src/diffusers/schedulers/
--rw-r--r--   0 ghunk      (501) staff       (20)     2201 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)    15014 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddim.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12795 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddim_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    13999 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddpm.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12373 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddpm_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12291 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12503 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_euler_discrete.py
--rw-r--r--   0 ghunk      (501) staff       (20)     6143 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ipndm.py
--rw-r--r--   0 ghunk      (501) staff       (20)     9750 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_karras_ve.py
--rw-r--r--   0 ghunk      (501) staff       (20)     9590 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12683 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_lms_discrete.py
--rw-r--r--   0 ghunk      (501) staff       (20)     8741 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    18600 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_pndm.py
--rw-r--r--   0 ghunk      (501) staff       (20)    22505 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_pndm_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    13642 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_repaint.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12115 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_sde_ve.py
--rw-r--r--   0 ghunk      (501) staff       (20)    12077 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_sde_ve_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)     3307 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_sde_vp.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1294 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1530 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_utils_flax.py
--rw-r--r--   0 ghunk      (501) staff       (20)    23758 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_vq_diffusion.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4110 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/training_utils.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.998261 diffusers-unchained-0.7.0/src/diffusers/utils/
--rw-r--r--   0 ghunk      (501) staff       (20)     2052 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/__init__.py
--rw-r--r--   0 ghunk      (501) staff       (20)     2069 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/deprecation_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)      584 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)     4206 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_flax_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)    11713 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_pt_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)    13006 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_accelerate_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)      553 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)     2065 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)     2811 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_transformers_objects.py
--rw-r--r--   0 ghunk      (501) staff       (20)    10580 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/import_utils.py
--rw-r--r--   0 ghunk      (501) staff       (20)     9413 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/logging.py
--rw-r--r--   0 ghunk      (501) staff       (20)     1484 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/model_card_template.md
--rw-r--r--   0 ghunk      (501) staff       (20)     3656 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/outputs.py
--rw-r--r--   0 ghunk      (501) staff       (20)    13255 2022-11-03 23:48:47.000000 diffusers-unchained-0.7.0/src/diffusers/utils/testing_utils.py
-drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-11-04 00:36:30.999056 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/
--rw-r--r--   0 ghunk      (501) staff       (20)    28827 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/PKG-INFO
--rw-r--r--   0 ghunk      (501) staff       (20)     5124 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/SOURCES.txt
--rw-r--r--   0 ghunk      (501) staff       (20)        1 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/dependency_links.txt
--rw-r--r--   0 ghunk      (501) staff       (20)       72 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/entry_points.txt
--rw-r--r--   0 ghunk      (501) staff       (20)      738 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/requires.txt
--rw-r--r--   0 ghunk      (501) staff       (20)       10 2022-11-04 00:36:30.000000 diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/top_level.txt
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.608362 diffusers-unchained-0.9.0/
+-rw-r--r--   0 ghunk      (501) staff       (20)    11357 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/LICENSE
+-rw-r--r--   0 ghunk      (501) staff       (20)       67 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/MANIFEST.in
+-rw-r--r--   0 ghunk      (501) staff       (20)    29204 2022-12-02 19:21:14.608532 diffusers-unchained-0.9.0/PKG-INFO
+-rw-r--r--   0 ghunk      (501) staff       (20)    28133 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/README.md
+-rw-r--r--   0 ghunk      (501) staff       (20)       57 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/pyproject.toml
+-rw-r--r--   0 ghunk      (501) staff       (20)      440 2022-12-02 19:21:14.608940 diffusers-unchained-0.9.0/setup.cfg
+-rw-r--r--   0 ghunk      (501) staff       (20)     9730 2022-12-02 19:07:03.000000 diffusers-unchained-0.9.0/setup.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.559808 diffusers-unchained-0.9.0/src/
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.571441 diffusers-unchained-0.9.0/src/diffusers/
+-rw-r--r--   0 ghunk      (501) staff       (20)     3836 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/__init__.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.573650 diffusers-unchained-0.9.0/src/diffusers/commands/
+-rw-r--r--   0 ghunk      (501) staff       (20)      920 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/commands/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     1200 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/commands/diffusers_cli.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     2384 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/commands/env.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    27747 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/configuration_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     1756 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/dependency_versions_check.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     1056 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/dependency_versions_table.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    18265 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/dynamic_modules_utils.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.573844 diffusers-unchained-0.9.0/src/diffusers/experimental/
+-rw-r--r--   0 ghunk      (501) staff       (20)       38 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/experimental/__init__.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.574290 diffusers-unchained-0.9.0/src/diffusers/experimental/rl/
+-rw-r--r--   0 ghunk      (501) staff       (20)       57 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/experimental/rl/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5035 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/experimental/rl/value_guided_sampling.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     9381 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/hub_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4599 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/modeling_flax_pytorch_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    25838 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/modeling_flax_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    32212 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/modeling_utils.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.579482 diffusers-unchained-0.9.0/src/diffusers/models/
+-rw-r--r--   0 ghunk      (501) staff       (20)     1046 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    38426 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/attention.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     9802 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/attention_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     6530 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/embeddings.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     3392 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/embeddings_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24780 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/resnet.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4021 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/resnet_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    10283 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_1d.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24857 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_1d_blocks.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    11619 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_2d.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    60670 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_blocks.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12836 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_blocks_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    17399 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_condition.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12669 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_condition_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    22505 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/vae.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    31047 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/models/vae_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     8282 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/onnx_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    11363 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/optimization.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    23215 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipeline_flax_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    35455 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipeline_utils.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.579850 diffusers-unchained-0.9.0/src/diffusers/pipelines/
+-rw-r--r--   0 ghunk      (501) staff       (20)     1900 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/__init__.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.582712 diffusers-unchained-0.9.0/src/diffusers/pipelines/alt_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)     1347 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/alt_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4673 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    29828 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    31860 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.583366 diffusers-unchained-0.9.0/src/diffusers/pipelines/dance_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)       76 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/dance_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5172 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.583952 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddim/
+-rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddim/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5713 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddim/pipeline_ddim.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.584669 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddpm/
+-rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddpm/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5541 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/ddpm/pipeline_ddpm.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.585439 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)      258 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    31318 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     7288 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.585942 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/
+-rw-r--r--   0 ghunk      (501) staff       (20)       73 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4801 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.586550 diffusers-unchained-0.9.0/src/diffusers/pipelines/pndm/
+-rw-r--r--   0 ghunk      (501) staff       (20)       55 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/pndm/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4049 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/pndm/pipeline_pndm.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.587108 diffusers-unchained-0.9.0/src/diffusers/pipelines/repaint/
+-rw-r--r--   0 ghunk      (501) staff       (20)       46 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/repaint/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5897 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/repaint/pipeline_repaint.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.587581 diffusers-unchained-0.9.0/src/diffusers/pipelines/score_sde_ve/
+-rw-r--r--   0 ghunk      (501) staff       (20)       69 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/score_sde_ve/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4286 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.594011 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)     3476 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    35945 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    19542 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    16410 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    23799 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24866 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    25300 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    29451 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24981 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    32797 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    38796 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    33727 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    27122 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5239 2022-12-02 19:13:22.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4485 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.594939 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/
+-rw-r--r--   0 ghunk      (501) staff       (20)     2503 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    38101 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5049 2022-12-02 19:10:46.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.595595 diffusers-unchained-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/
+-rw-r--r--   0 ghunk      (501) staff       (20)       75 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     5604 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.597854 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)      883 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    46826 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24527 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    31742 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    24004 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    25932 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.599055 diffusers-unchained-0.9.0/src/diffusers/pipelines/vq_diffusion/
+-rw-r--r--   0 ghunk      (501) staff       (20)      226 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/vq_diffusion/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    16151 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.604454 diffusers-unchained-0.9.0/src/diffusers/schedulers/
+-rw-r--r--   0 ghunk      (501) staff       (20)     2362 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    17395 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddim.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    14410 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddim_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    15948 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddpm.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    13935 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddpm_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    25871 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    28393 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    11797 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12494 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_euler_discrete.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     6153 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ipndm.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     9760 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_karras_ve.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     9600 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    11555 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     8890 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    18543 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_pndm.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    22654 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_pndm_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    13652 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_repaint.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12125 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_ve.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12087 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_ve_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     3317 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_vp.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     6845 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     7416 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_utils_flax.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    23768 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_vq_diffusion.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4110 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/training_utils.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.607397 diffusers-unchained-0.9.0/src/diffusers/utils/
+-rw-r--r--   0 ghunk      (501) staff       (20)     2428 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/__init__.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     2064 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/deprecation_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)      584 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     4587 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_flax_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    12101 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_pt_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)      553 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     2555 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     7293 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_objects.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    13381 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/import_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     9413 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/logging.py
+-rw-r--r--   0 ghunk      (501) staff       (20)     1484 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/model_card_template.md
+-rw-r--r--   0 ghunk      (501) staff       (20)     3656 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/outputs.py
+-rw-r--r--   0 ghunk      (501) staff       (20)      665 2022-12-02 19:02:02.000000 diffusers-unchained-0.9.0/src/diffusers/utils/pil_utils.py
+-rw-r--r--   0 ghunk      (501) staff       (20)    13255 2022-11-03 23:48:47.000000 diffusers-unchained-0.9.0/src/diffusers/utils/testing_utils.py
+drwxr-xr-x   0 ghunk      (501) staff       (20)        0 2022-12-02 19:21:14.608244 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/
+-rw-r--r--   0 ghunk      (501) staff       (20)    29204 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/PKG-INFO
+-rw-r--r--   0 ghunk      (501) staff       (20)     6688 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/SOURCES.txt
+-rw-r--r--   0 ghunk      (501) staff       (20)        1 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/dependency_links.txt
+-rw-r--r--   0 ghunk      (501) staff       (20)       72 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/entry_points.txt
+-rw-r--r--   0 ghunk      (501) staff       (20)      795 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/requires.txt
+-rw-r--r--   0 ghunk      (501) staff       (20)       10 2022-12-02 19:21:14.000000 diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/top_level.txt
```

### Comparing `diffusers-unchained-0.7.0/LICENSE` & `diffusers-unchained-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/PKG-INFO` & `diffusers-unchained-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: diffusers-unchained
-Version: 0.7.0
+Version: 0.9.0
 Summary: Diffusers
-Home-page: https://github.com/ghunkins/diffusers-unchained
+Home-page: https://github.com/huggingface/diffusers-unchained
 Author: The HuggingFace Team ft. Mage Team
 Author-email: greg@mage.space
 License: Apache
 Keywords: deep learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -179,23 +179,15 @@
 
 If you wish to use a different scheduler (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate
 it before the pipeline and pass it to `from_pretrained`.
     
 ```python
 from diffusers import LMSDiscreteScheduler
 
-lms = LMSDiscreteScheduler.from_config("CompVis/stable-diffusion-v1-4", subfolder="scheduler")
-
-pipe = StableDiffusionPipeline.from_pretrained(
-    "runwayml/stable-diffusion-v1-5", 
-    revision="fp16", 
-    torch_dtype=torch.float16,
-    scheduler=lms,
-)
-pipe = pipe.to("cuda")
+pipe.scheduler = LMSDiscreteScheduler.from_config(pipe.scheduler.config)
 
 prompt = "a photo of an astronaut riding a horse on mars"
 image = pipe(prompt).images[0]  
     
 image.save("astronaut_rides_horse.png")
 ```
 
@@ -373,22 +365,23 @@
 
 Fine-tuning techniques make it possible to adapt Stable Diffusion to your own dataset, or add new subjects to it. These are some of the techniques supported in `diffusers`:
 
 Textual Inversion is a technique for capturing novel concepts from a small number of example images in a way that can later be used to control text-to-image pipelines. It does so by learning new 'words' in the embedding space of the pipeline's text encoder. These special words can then be used within text prompts to achieve very fine-grained control of the resulting images. 
 
 - Textual Inversion. Capture novel concepts from a small set of sample images, and associate them with new "words" in the embedding space of the text encoder. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation](https://huggingface.co/docs/diffusers/training/text_inversion) to try for yourself.
 
-- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and training recommendations.
+- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training example](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for additional details and training recommendations.
 
 - Full Stable Diffusion fine-tuning. If you have a more sizable dataset with a specific look or style, you can fine-tune Stable Diffusion so that it outputs images following those examples. This was the approach taken to create [a Pokémon Stable Diffusion model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at [our text-to-image fine-tuning example](https://github.com/huggingface/diffusers/tree/main/examples/text_to_image) and go from there.
 
 
 ## Stable Diffusion Community Pipelines
 
-The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! Take a look and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipelines).
+The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. 
+Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! [Take a look](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline).
 
 ## Other Examples
 
 There are many ways to try running Diffusers! Here we outline code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and interactive web-tools.
 
 ### Running Code
 
@@ -429,18 +422,22 @@
 
 # save image
 image.save("ddpm_generated_image.png")
 ```
 - [Unconditional Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256)
 - [Unconditional Diffusion with continuous scheduler](https://huggingface.co/google/ncsnpp-ffhq-1024)
 
-**Other Notebooks**:
+**Other Image Notebooks**:
 * [image-to-image generation with Stable Diffusion](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 * [tweak images via repeated Stable Diffusion seeds](https://colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 
+**Diffusers for Other Modalities**:
+* [Molecule conformation generation](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/geodiff_molecule_conformation.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+* [Model-based reinforcement learning](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+
 ### Web Demos
 If you just want to play around with some web demos, you can try out the following 🚀 Spaces:
 | Model                          	| Hugging Face Spaces                                                                                                                                               	|
 |--------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
 | Text-to-Image Latent Diffusion 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/text2img-latent-diffusion) 	|
 | Faces generator                	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion)    	|
 | DDPM with different schedulers 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/fusing/celeba-diffusion)           	|
@@ -455,15 +452,15 @@
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-429a-affe-096e8199ad5b.png" width="800"/>
     <br>
     <em> Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
     
 **Schedulers**: Algorithm class for both **inference** and **training**.
-The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training.
+The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training. Also known as **Samplers**.
 *Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-4cda-b3e8-432d9dc7ad38.png" width="800"/>
     <br>
     <em> Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: diffusers-unchained Version: 0.7.0 Summary:
-Diffusers Home-page: https://github.com/ghunkins/diffusers-unchained Author:
+Metadata-Version: 2.1 Name: diffusers-unchained Version: 0.9.0 Summary:
+Diffusers Home-page: https://github.com/huggingface/diffusers-unchained Author:
 The HuggingFace Team ft. Mage Team Author-email: greg@mage.space License:
 Apache Keywords: deep learning Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -115,34 +115,31 @@
 following snippet should result in less than 4GB VRAM. ```python pipe =
 StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="fp16", torch_dtype=torch.float16, ) pipe = pipe.to("cuda") prompt =
 "a photo of an astronaut riding a horse on mars" pipe.enable_attention_slicing
 () image = pipe(prompt).images[0] ``` If you wish to use a different scheduler
 (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate it before the pipeline and
 pass it to `from_pretrained`. ```python from diffusers import
-LMSDiscreteScheduler lms = LMSDiscreteScheduler.from_config("CompVis/stable-
-diffusion-v1-4", subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
-revision="fp16", torch_dtype=torch.float16, scheduler=lms, ) pipe = pipe.to
-("cuda") prompt = "a photo of an astronaut riding a horse on mars" image = pipe
-(prompt).images[0] image.save("astronaut_rides_horse.png") ``` If you want to
-run Stable Diffusion on CPU or you want to have maximum precision on GPU,
-please run the model in the default *full-precision* setting: ```python # make
-sure you're logged in with `huggingface-cli login` from diffusers import
-StableDiffusionPipeline pipe = StableDiffusionPipeline.from_pretrained
-("runwayml/stable-diffusion-v1-5") # disable the following line if you run on
-CPU pipe = pipe.to("cuda") prompt = "a photo of an astronaut riding a horse on
+LMSDiscreteScheduler pipe.scheduler = LMSDiscreteScheduler.from_config
+(pipe.scheduler.config) prompt = "a photo of an astronaut riding a horse on
 mars" image = pipe(prompt).images[0] image.save("astronaut_rides_horse.png")
-``` ### JAX/Flax Diffusers offers a JAX / Flax implementation of Stable
-Diffusion for very fast inference. JAX shines specially on TPU hardware because
-each TPU server has 8 accelerators working in parallel, but it runs great on
-GPUs too. Running the pipeline with the default PNDMScheduler: ```python import
-jax import numpy as np from flax.jax_utils import replicate from
-flax.training.common_utils import shard from diffusers import
-FlaxStableDiffusionPipeline pipeline, params =
+``` If you want to run Stable Diffusion on CPU or you want to have maximum
+precision on GPU, please run the model in the default *full-precision* setting:
+```python # make sure you're logged in with `huggingface-cli login` from
+diffusers import StableDiffusionPipeline pipe =
+StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5") #
+disable the following line if you run on CPU pipe = pipe.to("cuda") prompt = "a
+photo of an astronaut riding a horse on mars" image = pipe(prompt).images[0]
+image.save("astronaut_rides_horse.png") ``` ### JAX/Flax Diffusers offers a JAX
+/ Flax implementation of Stable Diffusion for very fast inference. JAX shines
+specially on TPU hardware because each TPU server has 8 accelerators working in
+parallel, but it runs great on GPUs too. Running the pipeline with the default
+PNDMScheduler: ```python import jax import numpy as np from flax.jax_utils
+import replicate from flax.training.common_utils import shard from diffusers
+import FlaxStableDiffusionPipeline pipeline, params =
 FlaxStableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="flax", dtype=jax.numpy.bfloat16 ) prompt = "a photo of an astronaut
 riding a horse on mars" prng_seed = jax.random.PRNGKey(0) num_inference_steps =
 50 num_samples = jax.device_count() prompt = num_samples * [prompt] prompt_ids
 = pipeline.prepare_inputs(prompt) # shard inputs and rng params = replicate
 (params) prng_seed = jax.random.split(prng_seed, jax.device_count()) prompt_ids
 = shard(prompt_ids) images = pipeline(prompt_ids, params, prng_seed,
@@ -233,36 +230,36 @@
 images, and associate them with new "words" in the embedding space of the text
 encoder. Please, refer to [our training examples](https://github.com/
 huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation]
 (https://huggingface.co/docs/diffusers/training/text_inversion) to try for
 yourself. - Dreambooth. Another technique to capture new concepts in Stable
 Diffusion. This method fine-tunes the UNet (and, optionally, also the text
 encoder) of the pipeline to achieve impressive results. Please, refer to [our
-training examples](https://github.com/huggingface/diffusers/tree/main/examples/
-dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/
-Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and
-training recommendations. - Full Stable Diffusion fine-tuning. If you have a
-more sizable dataset with a specific look or style, you can fine-tune Stable
-Diffusion so that it outputs images following those examples. This was the
-approach taken to create [a PokÃ©mon Stable Diffusion model](https://
-huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney /
-Lambda Labs), [a Japanese specific version of Stable Diffusion](https://
-huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://
-github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at
-[our text-to-image fine-tuning example](https://github.com/huggingface/
-diffusers/tree/main/examples/text_to_image) and go from there. ## Stable
-Diffusion Community Pipelines The release of Stable Diffusion as an open source
-model has fostered a lot of interesting ideas and experimentation. Our
+training example](https://github.com/huggingface/diffusers/tree/main/examples/
+dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for
+additional details and training recommendations. - Full Stable Diffusion fine-
+tuning. If you have a more sizable dataset with a specific look or style, you
+can fine-tune Stable Diffusion so that it outputs images following those
+examples. This was the approach taken to create [a PokÃ©mon Stable Diffusion
+model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by
+Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable
+Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by
+[Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others.
+You can start at [our text-to-image fine-tuning example](https://github.com/
+huggingface/diffusers/tree/main/examples/text_to_image) and go from there. ##
+Stable Diffusion Community Pipelines The release of Stable Diffusion as an open
+source model has fostered a lot of interesting ideas and experimentation. Our
 [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/
 examples/community) contains many ideas worth exploring, like interpolating to
 create animated videos, using CLIP Guidance for additional prompt fidelity,
-term weighting, and much more! Take a look and [contribute your own](https://
-huggingface.co/docs/diffusers/using-diffusers/custom_pipelines). ## Other
-Examples There are many ways to try running Diffusers! Here we outline code-
-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
+term weighting, and much more! [Take a look](https://huggingface.co/docs/
+diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own]
+(https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline). ##
+Other Examples There are many ways to try running Diffusers! Here we outline
+code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
 interactive web-tools. ### Running Code If you want to run the code yourself
 ð», you can try out: - [Text-to-Image Latent Diffusion](https://
 huggingface.co/CompVis/ldm-text2im-large-256) ```python # !pip install
 diffusers["torch"] transformers from diffusers import DiffusionPipeline device
 = "cuda" model_id = "CompVis/ldm-text2im-large-256" # load model and scheduler
 ldm = DiffusionPipeline.from_pretrained(model_id) ldm = ldm.to(device) # run
 pipeline in inference (sample random noise and denoise) prompt = "A painting of
@@ -274,51 +271,59 @@
 ddpm-celebahq-256" device = "cuda" # load model and scheduler ddpm =
 DDPMPipeline.from_pretrained(model_id) # you can replace DDPMPipeline with
 DDIMPipeline or PNDMPipeline for faster inference ddpm.to(device) # run
 pipeline in inference (sample random noise and denoise) image = ddpm().images
 [0] # save image image.save("ddpm_generated_image.png") ``` - [Unconditional
 Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256) -
 [Unconditional Diffusion with continuous scheduler](https://huggingface.co/
-google/ncsnpp-ffhq-1024) **Other Notebooks**: * [image-to-image generation with
-Stable Diffusion](https://colab.research.google.com/github/huggingface/
-notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg), * [tweak
-images via repeated Stable Diffusion seeds](https://colab.research.google.com/
-github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-
-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg), ### Web Demos If you just want to play around with some web demos,
-you can try out the following ð Spaces: | Model | Hugging Face Spaces | |---
------------------------------ |------------------------------------------------
+google/ncsnpp-ffhq-1024) **Other Image Notebooks**: * [image-to-image
+generation with Stable Diffusion](https://colab.research.google.com/github/
+huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb)
+![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg), *
+[tweak images via repeated Stable Diffusion seeds](https://
+colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/
+notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), **Diffusers for Other
+Modalities**: * [Molecule conformation generation](https://
+colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/
+geodiff_molecule_conformation.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), * [Model-based reinforcement
+learning](https://colab.research.google.com/github/huggingface/notebooks/blob/
+main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg), ### Web Demos If
+you just want to play around with some web demos, you can try out the following
+ð Spaces: | Model | Hugging Face Spaces | |-------------------------------
+- |----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------- | | Text-to-Image Latent Diffusion | [!
-[Hugging Face Spaces](https://img.shields.io/badge/
+-------- | | Text-to-Image Latent Diffusion | [![Hugging Face Spaces](https://
+img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://
+huggingface.co/spaces/CompVis/text2img-latent-diffusion) | | Faces generator |
+[![Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-CompVis/text2img-latent-diffusion) | | Faces generator | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion) | | DDPM
-with different schedulers | [![Hugging Face Spaces](https://img.shields.io/
-badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/
-spaces/fusing/celeba-diffusion) | | Conditional generation from sketch | [!
+CompVis/celeba-latent-diffusion) | | DDPM with different schedulers | [!
 [Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-huggingface/diffuse-the-rest) | | Composable diffusion | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/Shuang59/Composable-Diffusion) | ##
-Definitions **Models**: Neural network that models $p_\theta(\mathbf{x}_{t-
-1}|\mathbf{x}_t)$ (see image below) and is trained end-to-end to *denoise* a
-noisy input to an image. *Examples*: UNet, Conditioned UNet, 3D UNet,
-Transformer UNet
+fusing/celeba-diffusion) | | Conditional generation from sketch | [![Hugging
+Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
+blue)](https://huggingface.co/spaces/huggingface/diffuse-the-rest) | |
+Composable diffusion | [![Hugging Face Spaces](https://img.shields.io/badge/
+%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
+Shuang59/Composable-Diffusion) | ## Definitions **Models**: Neural network that
+models $p_\theta(\mathbf{x}_{t-1}|\mathbf{x}_t)$ (see image below) and is
+trained end-to-end to *denoise* a noisy input to an image. *Examples*: UNet,
+Conditioned UNet, 3D UNet, Transformer UNet
  [https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-
                          429a-affe-096e8199ad5b.png]
           Figure from DDPM paper (https://arxiv.org/abs/2006.11239).
 **Schedulers**: Algorithm class for both **inference** and **training**. The
 class provides functionality to compute previous image according to alpha, beta
-schedule as well as predict noise for training. *Examples*: [DDPM](https://
-arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM]
-(https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
+schedule as well as predict noise for training. Also known as **Samplers**.
+*Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/
+abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://
+arxiv.org/abs/2204.13902)
  [https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-
                          4cda-b3e8-432d9dc7ad38.png]
  Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/
                                abs/2006.11239).
 **Diffusion Pipeline**: End-to-end pipeline that includes multiple diffusion
 models, possible text encoders, ... *Examples*: Glide, Latent-Diffusion,
 Imagen, DALL-E 2
```

### Comparing `diffusers-unchained-0.7.0/README.md` & `diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: diffusers-unchained
+Version: 0.9.0
+Summary: Diffusers
+Home-page: https://github.com/huggingface/diffusers-unchained
+Author: The HuggingFace Team ft. Mage Team
+Author-email: greg@mage.space
+License: Apache
+Keywords: deep learning
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: quality
+Provides-Extra: docs
+Provides-Extra: training
+Provides-Extra: test
+Provides-Extra: torch
+Provides-Extra: flax
+Provides-Extra: dev
+License-File: LICENSE
+
 <p align="center">
     <br>
     <img src="https://github.com/huggingface/diffusers/raw/main/docs/source/imgs/diffusers_library.jpg" width="400"/>
     <br>
 <p>
 <p align="center">
     <a href="https://github.com/huggingface/diffusers/blob/main/LICENSE">
@@ -148,23 +179,15 @@
 
 If you wish to use a different scheduler (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate
 it before the pipeline and pass it to `from_pretrained`.
     
 ```python
 from diffusers import LMSDiscreteScheduler
 
-lms = LMSDiscreteScheduler.from_config("CompVis/stable-diffusion-v1-4", subfolder="scheduler")
-
-pipe = StableDiffusionPipeline.from_pretrained(
-    "runwayml/stable-diffusion-v1-5", 
-    revision="fp16", 
-    torch_dtype=torch.float16,
-    scheduler=lms,
-)
-pipe = pipe.to("cuda")
+pipe.scheduler = LMSDiscreteScheduler.from_config(pipe.scheduler.config)
 
 prompt = "a photo of an astronaut riding a horse on mars"
 image = pipe(prompt).images[0]  
     
 image.save("astronaut_rides_horse.png")
 ```
 
@@ -342,22 +365,23 @@
 
 Fine-tuning techniques make it possible to adapt Stable Diffusion to your own dataset, or add new subjects to it. These are some of the techniques supported in `diffusers`:
 
 Textual Inversion is a technique for capturing novel concepts from a small number of example images in a way that can later be used to control text-to-image pipelines. It does so by learning new 'words' in the embedding space of the pipeline's text encoder. These special words can then be used within text prompts to achieve very fine-grained control of the resulting images. 
 
 - Textual Inversion. Capture novel concepts from a small set of sample images, and associate them with new "words" in the embedding space of the text encoder. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation](https://huggingface.co/docs/diffusers/training/text_inversion) to try for yourself.
 
-- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and training recommendations.
+- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training example](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for additional details and training recommendations.
 
 - Full Stable Diffusion fine-tuning. If you have a more sizable dataset with a specific look or style, you can fine-tune Stable Diffusion so that it outputs images following those examples. This was the approach taken to create [a Pokémon Stable Diffusion model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at [our text-to-image fine-tuning example](https://github.com/huggingface/diffusers/tree/main/examples/text_to_image) and go from there.
 
 
 ## Stable Diffusion Community Pipelines
 
-The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! Take a look and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipelines).
+The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. 
+Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! [Take a look](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline).
 
 ## Other Examples
 
 There are many ways to try running Diffusers! Here we outline code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and interactive web-tools.
 
 ### Running Code
 
@@ -398,18 +422,22 @@
 
 # save image
 image.save("ddpm_generated_image.png")
 ```
 - [Unconditional Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256)
 - [Unconditional Diffusion with continuous scheduler](https://huggingface.co/google/ncsnpp-ffhq-1024)
 
-**Other Notebooks**:
+**Other Image Notebooks**:
 * [image-to-image generation with Stable Diffusion](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 * [tweak images via repeated Stable Diffusion seeds](https://colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 
+**Diffusers for Other Modalities**:
+* [Molecule conformation generation](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/geodiff_molecule_conformation.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+* [Model-based reinforcement learning](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+
 ### Web Demos
 If you just want to play around with some web demos, you can try out the following 🚀 Spaces:
 | Model                          	| Hugging Face Spaces                                                                                                                                               	|
 |--------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
 | Text-to-Image Latent Diffusion 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/text2img-latent-diffusion) 	|
 | Faces generator                	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion)    	|
 | DDPM with different schedulers 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/fusing/celeba-diffusion)           	|
@@ -424,15 +452,15 @@
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-429a-affe-096e8199ad5b.png" width="800"/>
     <br>
     <em> Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
     
 **Schedulers**: Algorithm class for both **inference** and **training**.
-The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training.
+The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training. Also known as **Samplers**.
 *Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-4cda-b3e8-432d9dc7ad38.png" width="800"/>
     <br>
     <em> Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
```

#### html2text {}

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1 Name: diffusers-unchained Version: 0.9.0 Summary:
+Diffusers Home-page: https://github.com/huggingface/diffusers-unchained Author:
+The HuggingFace Team ft. Mage Team Author-email: greg@mage.space License:
+Apache Keywords: deep learning Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Education Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
+Provides-Extra: quality Provides-Extra: docs Provides-Extra: training Provides-
+Extra: test Provides-Extra: torch Provides-Extra: flax Provides-Extra: dev
+License-File: LICENSE
 
      [https://github.com/huggingface/diffusers/raw/main/docs/source/imgs/
                             diffusers_library.jpg]
                [GitHub] [GitHub_release] [Contributor_Covenant]
 ð¤ Diffusers provides pretrained diffusion models across multiple modalities,
 such as vision and audio, and serves as a modular toolbox for inference and
 training of diffusion models. More precisely, ð¤ Diffusers offers: - State-
@@ -100,34 +115,31 @@
 following snippet should result in less than 4GB VRAM. ```python pipe =
 StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="fp16", torch_dtype=torch.float16, ) pipe = pipe.to("cuda") prompt =
 "a photo of an astronaut riding a horse on mars" pipe.enable_attention_slicing
 () image = pipe(prompt).images[0] ``` If you wish to use a different scheduler
 (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate it before the pipeline and
 pass it to `from_pretrained`. ```python from diffusers import
-LMSDiscreteScheduler lms = LMSDiscreteScheduler.from_config("CompVis/stable-
-diffusion-v1-4", subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
-revision="fp16", torch_dtype=torch.float16, scheduler=lms, ) pipe = pipe.to
-("cuda") prompt = "a photo of an astronaut riding a horse on mars" image = pipe
-(prompt).images[0] image.save("astronaut_rides_horse.png") ``` If you want to
-run Stable Diffusion on CPU or you want to have maximum precision on GPU,
-please run the model in the default *full-precision* setting: ```python # make
-sure you're logged in with `huggingface-cli login` from diffusers import
-StableDiffusionPipeline pipe = StableDiffusionPipeline.from_pretrained
-("runwayml/stable-diffusion-v1-5") # disable the following line if you run on
-CPU pipe = pipe.to("cuda") prompt = "a photo of an astronaut riding a horse on
+LMSDiscreteScheduler pipe.scheduler = LMSDiscreteScheduler.from_config
+(pipe.scheduler.config) prompt = "a photo of an astronaut riding a horse on
 mars" image = pipe(prompt).images[0] image.save("astronaut_rides_horse.png")
-``` ### JAX/Flax Diffusers offers a JAX / Flax implementation of Stable
-Diffusion for very fast inference. JAX shines specially on TPU hardware because
-each TPU server has 8 accelerators working in parallel, but it runs great on
-GPUs too. Running the pipeline with the default PNDMScheduler: ```python import
-jax import numpy as np from flax.jax_utils import replicate from
-flax.training.common_utils import shard from diffusers import
-FlaxStableDiffusionPipeline pipeline, params =
+``` If you want to run Stable Diffusion on CPU or you want to have maximum
+precision on GPU, please run the model in the default *full-precision* setting:
+```python # make sure you're logged in with `huggingface-cli login` from
+diffusers import StableDiffusionPipeline pipe =
+StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5") #
+disable the following line if you run on CPU pipe = pipe.to("cuda") prompt = "a
+photo of an astronaut riding a horse on mars" image = pipe(prompt).images[0]
+image.save("astronaut_rides_horse.png") ``` ### JAX/Flax Diffusers offers a JAX
+/ Flax implementation of Stable Diffusion for very fast inference. JAX shines
+specially on TPU hardware because each TPU server has 8 accelerators working in
+parallel, but it runs great on GPUs too. Running the pipeline with the default
+PNDMScheduler: ```python import jax import numpy as np from flax.jax_utils
+import replicate from flax.training.common_utils import shard from diffusers
+import FlaxStableDiffusionPipeline pipeline, params =
 FlaxStableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="flax", dtype=jax.numpy.bfloat16 ) prompt = "a photo of an astronaut
 riding a horse on mars" prng_seed = jax.random.PRNGKey(0) num_inference_steps =
 50 num_samples = jax.device_count() prompt = num_samples * [prompt] prompt_ids
 = pipeline.prepare_inputs(prompt) # shard inputs and rng params = replicate
 (params) prng_seed = jax.random.split(prng_seed, jax.device_count()) prompt_ids
 = shard(prompt_ids) images = pipeline(prompt_ids, params, prng_seed,
@@ -218,36 +230,36 @@
 images, and associate them with new "words" in the embedding space of the text
 encoder. Please, refer to [our training examples](https://github.com/
 huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation]
 (https://huggingface.co/docs/diffusers/training/text_inversion) to try for
 yourself. - Dreambooth. Another technique to capture new concepts in Stable
 Diffusion. This method fine-tunes the UNet (and, optionally, also the text
 encoder) of the pipeline to achieve impressive results. Please, refer to [our
-training examples](https://github.com/huggingface/diffusers/tree/main/examples/
-dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/
-Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and
-training recommendations. - Full Stable Diffusion fine-tuning. If you have a
-more sizable dataset with a specific look or style, you can fine-tune Stable
-Diffusion so that it outputs images following those examples. This was the
-approach taken to create [a PokÃ©mon Stable Diffusion model](https://
-huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney /
-Lambda Labs), [a Japanese specific version of Stable Diffusion](https://
-huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://
-github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at
-[our text-to-image fine-tuning example](https://github.com/huggingface/
-diffusers/tree/main/examples/text_to_image) and go from there. ## Stable
-Diffusion Community Pipelines The release of Stable Diffusion as an open source
-model has fostered a lot of interesting ideas and experimentation. Our
+training example](https://github.com/huggingface/diffusers/tree/main/examples/
+dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for
+additional details and training recommendations. - Full Stable Diffusion fine-
+tuning. If you have a more sizable dataset with a specific look or style, you
+can fine-tune Stable Diffusion so that it outputs images following those
+examples. This was the approach taken to create [a PokÃ©mon Stable Diffusion
+model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by
+Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable
+Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by
+[Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others.
+You can start at [our text-to-image fine-tuning example](https://github.com/
+huggingface/diffusers/tree/main/examples/text_to_image) and go from there. ##
+Stable Diffusion Community Pipelines The release of Stable Diffusion as an open
+source model has fostered a lot of interesting ideas and experimentation. Our
 [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/
 examples/community) contains many ideas worth exploring, like interpolating to
 create animated videos, using CLIP Guidance for additional prompt fidelity,
-term weighting, and much more! Take a look and [contribute your own](https://
-huggingface.co/docs/diffusers/using-diffusers/custom_pipelines). ## Other
-Examples There are many ways to try running Diffusers! Here we outline code-
-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
+term weighting, and much more! [Take a look](https://huggingface.co/docs/
+diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own]
+(https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline). ##
+Other Examples There are many ways to try running Diffusers! Here we outline
+code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
 interactive web-tools. ### Running Code If you want to run the code yourself
 ð», you can try out: - [Text-to-Image Latent Diffusion](https://
 huggingface.co/CompVis/ldm-text2im-large-256) ```python # !pip install
 diffusers["torch"] transformers from diffusers import DiffusionPipeline device
 = "cuda" model_id = "CompVis/ldm-text2im-large-256" # load model and scheduler
 ldm = DiffusionPipeline.from_pretrained(model_id) ldm = ldm.to(device) # run
 pipeline in inference (sample random noise and denoise) prompt = "A painting of
@@ -259,51 +271,59 @@
 ddpm-celebahq-256" device = "cuda" # load model and scheduler ddpm =
 DDPMPipeline.from_pretrained(model_id) # you can replace DDPMPipeline with
 DDIMPipeline or PNDMPipeline for faster inference ddpm.to(device) # run
 pipeline in inference (sample random noise and denoise) image = ddpm().images
 [0] # save image image.save("ddpm_generated_image.png") ``` - [Unconditional
 Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256) -
 [Unconditional Diffusion with continuous scheduler](https://huggingface.co/
-google/ncsnpp-ffhq-1024) **Other Notebooks**: * [image-to-image generation with
-Stable Diffusion](https://colab.research.google.com/github/huggingface/
-notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg), * [tweak
-images via repeated Stable Diffusion seeds](https://colab.research.google.com/
-github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-
-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg), ### Web Demos If you just want to play around with some web demos,
-you can try out the following ð Spaces: | Model | Hugging Face Spaces | |---
------------------------------ |------------------------------------------------
+google/ncsnpp-ffhq-1024) **Other Image Notebooks**: * [image-to-image
+generation with Stable Diffusion](https://colab.research.google.com/github/
+huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb)
+![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg), *
+[tweak images via repeated Stable Diffusion seeds](https://
+colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/
+notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), **Diffusers for Other
+Modalities**: * [Molecule conformation generation](https://
+colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/
+geodiff_molecule_conformation.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), * [Model-based reinforcement
+learning](https://colab.research.google.com/github/huggingface/notebooks/blob/
+main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg), ### Web Demos If
+you just want to play around with some web demos, you can try out the following
+ð Spaces: | Model | Hugging Face Spaces | |-------------------------------
+- |----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------- | | Text-to-Image Latent Diffusion | [!
-[Hugging Face Spaces](https://img.shields.io/badge/
+-------- | | Text-to-Image Latent Diffusion | [![Hugging Face Spaces](https://
+img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://
+huggingface.co/spaces/CompVis/text2img-latent-diffusion) | | Faces generator |
+[![Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-CompVis/text2img-latent-diffusion) | | Faces generator | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion) | | DDPM
-with different schedulers | [![Hugging Face Spaces](https://img.shields.io/
-badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/
-spaces/fusing/celeba-diffusion) | | Conditional generation from sketch | [!
+CompVis/celeba-latent-diffusion) | | DDPM with different schedulers | [!
 [Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-huggingface/diffuse-the-rest) | | Composable diffusion | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/Shuang59/Composable-Diffusion) | ##
-Definitions **Models**: Neural network that models $p_\theta(\mathbf{x}_{t-
-1}|\mathbf{x}_t)$ (see image below) and is trained end-to-end to *denoise* a
-noisy input to an image. *Examples*: UNet, Conditioned UNet, 3D UNet,
-Transformer UNet
+fusing/celeba-diffusion) | | Conditional generation from sketch | [![Hugging
+Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
+blue)](https://huggingface.co/spaces/huggingface/diffuse-the-rest) | |
+Composable diffusion | [![Hugging Face Spaces](https://img.shields.io/badge/
+%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
+Shuang59/Composable-Diffusion) | ## Definitions **Models**: Neural network that
+models $p_\theta(\mathbf{x}_{t-1}|\mathbf{x}_t)$ (see image below) and is
+trained end-to-end to *denoise* a noisy input to an image. *Examples*: UNet,
+Conditioned UNet, 3D UNet, Transformer UNet
  [https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-
                          429a-affe-096e8199ad5b.png]
           Figure from DDPM paper (https://arxiv.org/abs/2006.11239).
 **Schedulers**: Algorithm class for both **inference** and **training**. The
 class provides functionality to compute previous image according to alpha, beta
-schedule as well as predict noise for training. *Examples*: [DDPM](https://
-arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM]
-(https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
+schedule as well as predict noise for training. Also known as **Samplers**.
+*Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/
+abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://
+arxiv.org/abs/2204.13902)
  [https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-
                          4cda-b3e8-432d9dc7ad38.png]
  Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/
                                abs/2006.11239).
 **Diffusion Pipeline**: End-to-end pipeline that includes multiple diffusion
 models, possible text encoders, ... *Examples*: Glide, Latent-Diffusion,
 Imagen, DALL-E 2
```

### Comparing `diffusers-unchained-0.7.0/setup.py` & `diffusers-unchained-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 from setuptools import find_packages, setup
 
 
 # IMPORTANT:
 # 1. all dependencies should be listed here with their version requirements if any
 # 2. once modified, run: `make deps_table_update` to update src/diffusers/dependency_versions_table.py
 _deps = [
-    "Pillow<10.0",  # keep the PIL.Image.Resampling deprecation away
+    "Pillow",  # keep the PIL.Image.Resampling deprecation away
     "accelerate>=0.11.0",
     "black==22.8",
     "datasets",
     "filelock",
     "flake8>=3.8.3",
     "flax>=0.4.1",
     "hf-doc-builder>=0.3.0",
@@ -93,14 +93,15 @@
     "jaxlib>=0.1.65",
     "modelcards>=0.1.4",
     "numpy",
     "parameterized",
     "pytest",
     "pytest-timeout",
     "pytest-xdist",
+    "sentencepiece>=0.1.91,!=0.1.92",
     "scipy",
     "regex!=2019.12.17",
     "requests",
     "tensorboard",
     "torch>=1.4",
     "torchvision",
     "transformers>=4.21.0",
@@ -179,14 +180,15 @@
 extras["training"] = deps_list("accelerate", "datasets", "tensorboard", "modelcards")
 extras["test"] = deps_list(
     "datasets",
     "parameterized",
     "pytest",
     "pytest-timeout",
     "pytest-xdist",
+    "sentencepiece",
     "scipy",
     "torchvision",
     "transformers"
 )
 extras["torch"] = deps_list("torch", "accelerate")
 
 if os.name == "nt":  # windows
@@ -206,23 +208,23 @@
     deps["regex"],
     deps["requests"],
     deps["Pillow"],
 ]
 
 setup(
     name="diffusers-unchained",
-    version="0.7.0",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.9.0",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Diffusers",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace Team ft. Mage Team",
     author_email="greg@mage.space",
-    url="https://github.com/ghunkins/diffusers-unchained",
+    url="https://github.com/huggingface/diffusers-unchained",
     package_dir={"": "src"},
     packages=find_packages("src"),
     include_package_data=True,
     python_requires=">=3.7.0",
     install_requires=install_requires,
     extras_require=extras,
     entry_points={"console_scripts": ["diffusers-cli=diffusers.commands.diffusers_cli:main"]},
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/commands/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/commands/diffusers_cli.py` & `diffusers-unchained-0.9.0/src/diffusers/commands/diffusers_cli.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/commands/env.py` & `diffusers-unchained-0.9.0/src/diffusers/commands/env.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/configuration_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/configuration_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,48 +25,80 @@
 from typing import Any, Dict, Tuple, Union
 
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError, RepositoryNotFoundError, RevisionNotFoundError
 from requests import HTTPError
 
 from . import __version__
-from .utils import DIFFUSERS_CACHE, HUGGINGFACE_CO_RESOLVE_ENDPOINT, logging
+from .utils import DIFFUSERS_CACHE, HUGGINGFACE_CO_RESOLVE_ENDPOINT, DummyObject, deprecate, logging
 
 
 logger = logging.get_logger(__name__)
 
 _re_configuration_file = re.compile(r"config\.(.*)\.json")
 
 
+class FrozenDict(OrderedDict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        for key, value in self.items():
+            setattr(self, key, value)
+
+        self.__frozen = True
+
+    def __delitem__(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance.")
+
+    def setdefault(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance.")
+
+    def pop(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
+
+    def update(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``update`` on a {self.__class__.__name__} instance.")
+
+    def __setattr__(self, name, value):
+        if hasattr(self, "__frozen") and self.__frozen:
+            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
+        super().__setattr__(name, value)
+
+    def __setitem__(self, name, value):
+        if hasattr(self, "__frozen") and self.__frozen:
+            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
+        super().__setitem__(name, value)
+
+
 class ConfigMixin:
     r"""
     Base class for all configuration classes. Stores all configuration parameters under `self.config` Also handles all
     methods for loading/downloading/saving classes inheriting from [`ConfigMixin`] with
         - [`~ConfigMixin.from_config`]
         - [`~ConfigMixin.save_config`]
 
     Class attributes:
         - **config_name** (`str`) -- A filename under which the config should stored when calling
           [`~ConfigMixin.save_config`] (should be overridden by parent class).
         - **ignore_for_config** (`List[str]`) -- A list of attributes that should not be saved in the config (should be
-          overridden by parent class).
-        - **_compatible_classes** (`List[str]`) -- A list of classes that are compatible with the parent class, so that
-          `from_config` can be used from a class different than the one used to save the config (should be overridden
-          by parent class).
+          overridden by subclass).
+        - **has_compatibles** (`bool`) -- Whether the class has compatible classes (should be overridden by subclass).
+        - **_deprecated_kwargs** (`List[str]`) -- Keyword arguments that are deprecated. Note that the init function
+          should only have a `kwargs` argument if at least one argument is deprecated (should be overridden by
+          subclass).
     """
     config_name = None
     ignore_for_config = []
-    _compatible_classes = []
+    has_compatibles = False
+
+    _deprecated_kwargs = []
 
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
@@ -97,37 +129,127 @@
 
         os.makedirs(save_directory, exist_ok=True)
 
         # If we save using the predefined names, we can load using `from_config`
         output_config_file = os.path.join(save_directory, self.config_name)
 
         self.to_json_file(output_config_file)
-        logger.info(f"ConfigMixinuration saved in {output_config_file}")
+        logger.info(f"Configuration saved in {output_config_file}")
+
+    @classmethod
+    def from_config(cls, config: Union[FrozenDict, Dict[str, Any]] = None, return_unused_kwargs=False, **kwargs):
+        r"""
+        Instantiate a Python class from a config dictionary
+
+        Parameters:
+            config (`Dict[str, Any]`):
+                A config dictionary from which the Python class will be instantiated. Make sure to only load
+                configuration files of compatible classes.
+            return_unused_kwargs (`bool`, *optional*, defaults to `False`):
+                Whether kwargs that are not consumed by the Python class should be returned or not.
+
+            kwargs (remaining dictionary of keyword arguments, *optional*):
+                Can be used to update the configuration object (after it being loaded) and initiate the Python class.
+                `**kwargs` will be directly passed to the underlying scheduler/model's `__init__` method and eventually
+                overwrite same named arguments of `config`.
+
+        Examples:
+
+        ```python
+        >>> from diffusers import DDPMScheduler, DDIMScheduler, PNDMScheduler
+
+        >>> # Download scheduler from huggingface.co and cache.
+        >>> scheduler = DDPMScheduler.from_pretrained("google/ddpm-cifar10-32")
+
+        >>> # Instantiate DDIM scheduler class with same config as DDPM
+        >>> scheduler = DDIMScheduler.from_config(scheduler.config)
+
+        >>> # Instantiate PNDM scheduler class with same config as DDPM
+        >>> scheduler = PNDMScheduler.from_config(scheduler.config)
+        ```
+        """
+        # <===== TO BE REMOVED WITH DEPRECATION
+        # TODO(Patrick) - make sure to remove the following lines when config=="model_path" is deprecated
+        if "pretrained_model_name_or_path" in kwargs:
+            config = kwargs.pop("pretrained_model_name_or_path")
+
+        if config is None:
+            raise ValueError("Please make sure to provide a config as the first positional argument.")
+        # ======>
+
+        if not isinstance(config, dict):
+            deprecation_message = "It is deprecated to pass a pretrained model name or path to `from_config`."
+            if "Scheduler" in cls.__name__:
+                deprecation_message += (
+                    f"If you were trying to load a scheduler, please use {cls}.from_pretrained(...) instead."
+                    " Otherwise, please make sure to pass a configuration dictionary instead. This functionality will"
+                    " be removed in v1.0.0."
+                )
+            elif "Model" in cls.__name__:
+                deprecation_message += (
+                    f"If you were trying to load a model, please use {cls}.load_config(...) followed by"
+                    f" {cls}.from_config(...) instead. Otherwise, please make sure to pass a configuration dictionary"
+                    " instead. This functionality will be removed in v1.0.0."
+                )
+            deprecate("config-passed-as-path", "1.0.0", deprecation_message, standard_warn=False)
+            config, kwargs = cls.load_config(pretrained_model_name_or_path=config, return_unused_kwargs=True, **kwargs)
+
+        init_dict, unused_kwargs, hidden_dict = cls.extract_init_dict(config, **kwargs)
+
+        # Allow dtype to be specified on initialization
+        if "dtype" in unused_kwargs:
+            init_dict["dtype"] = unused_kwargs.pop("dtype")
+
+        # add possible deprecated kwargs
+        for deprecated_kwarg in cls._deprecated_kwargs:
+            if deprecated_kwarg in unused_kwargs:
+                init_dict[deprecated_kwarg] = unused_kwargs.pop(deprecated_kwarg)
+
+        # Return model and optionally state and/or unused_kwargs
+        model = cls(**init_dict)
+
+        # make sure to also save config parameters that might be used for compatible classes
+        model.register_to_config(**hidden_dict)
+
+        # add hidden kwargs of compatible classes to unused_kwargs
+        unused_kwargs = {**unused_kwargs, **hidden_dict}
+
+        if return_unused_kwargs:
+            return (model, unused_kwargs)
+        else:
+            return model
 
     @classmethod
-    def from_config(cls, pretrained_model_name_or_path: Union[str, os.PathLike], return_unused_kwargs=False, **kwargs):
+    def get_config_dict(cls, *args, **kwargs):
+        deprecation_message = (
+            f" The function get_config_dict is deprecated. Please use {cls}.load_config instead. This function will be"
+            " removed in version v1.0.0"
+        )
+        deprecate("get_config_dict", "1.0.0", deprecation_message, standard_warn=False)
+        return cls.load_config(*args, **kwargs)
+
+    @classmethod
+    def load_config(
+        cls, pretrained_model_name_or_path: Union[str, os.PathLike], return_unused_kwargs=False, **kwargs
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         r"""
-        Instantiate a Python class from a pre-defined JSON-file.
+        Instantiate a Python class from a config dictionary
 
         Parameters:
             pretrained_model_name_or_path (`str` or `os.PathLike`, *optional*):
                 Can be either:
 
                     - A string, the *model id* of a model repo on huggingface.co. Valid model ids should have an
                       organization name, like `google/ddpm-celebahq-256`.
                     - A path to a *directory* containing model weights saved using [`~ConfigMixin.save_config`], e.g.,
                       `./my_model_directory/`.
 
             cache_dir (`Union[str, os.PathLike]`, *optional*):
                 Path to a directory in which a downloaded pretrained model configuration should be cached if the
                 standard cache should not be used.
-            ignore_mismatched_sizes (`bool`, *optional*, defaults to `False`):
-                Whether or not to raise an error if some of the weights from the checkpoint do not have the same size
-                as the weights of the model (if for instance, you are instantiating a model with 10 labels from a
-                checkpoint with 3 labels).
             force_download (`bool`, *optional*, defaults to `False`):
                 Whether or not to force the (re-)download of the model weights and configuration files, overriding the
                 cached versions if they exist.
             resume_download (`bool`, *optional*, defaults to `False`):
                 Whether or not to delete incompletely received files. Will attempt to resume the download if such a
                 file exists.
             proxies (`Dict[str, str]`, *optional*):
@@ -157,41 +279,15 @@
 
         <Tip>
 
         Activate the special ["offline-mode"](https://huggingface.co/transformers/installation.html#offline-mode) to
         use this method in a firewalled environment.
 
         </Tip>
-
         """
-        config_dict = cls.get_config_dict(pretrained_model_name_or_path=pretrained_model_name_or_path, **kwargs)
-        init_dict, unused_kwargs = cls.extract_init_dict(config_dict, **kwargs)
-
-        # Allow dtype to be specified on initialization
-        if "dtype" in unused_kwargs:
-            init_dict["dtype"] = unused_kwargs.pop("dtype")
-
-        # Return model and optionally state and/or unused_kwargs
-        model = cls(**init_dict)
-        return_tuple = (model,)
-
-        # Flax schedulers have a state, so return it.
-        if cls.__name__.startswith("Flax") and hasattr(model, "create_state") and getattr(model, "has_state", False):
-            state = model.create_state()
-            return_tuple += (state,)
-
-        if return_unused_kwargs:
-            return return_tuple + (unused_kwargs,)
-        else:
-            return return_tuple if len(return_tuple) > 1 else model
-
-    @classmethod
-    def get_config_dict(
-        cls, pretrained_model_name_or_path: Union[str, os.PathLike], **kwargs
-    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         cache_dir = kwargs.pop("cache_dir", DIFFUSERS_CACHE)
         force_download = kwargs.pop("force_download", False)
         resume_download = kwargs.pop("resume_download", False)
         proxies = kwargs.pop("proxies", None)
         use_auth_token = kwargs.pop("use_auth_token", None)
         local_files_only = kwargs.pop("local_files_only", False)
         revision = kwargs.pop("revision", None)
@@ -279,22 +375,28 @@
 
         try:
             # Load config dict
             config_dict = cls._dict_from_json_file(config_file)
         except (json.JSONDecodeError, UnicodeDecodeError):
             raise EnvironmentError(f"It looks like the config file at '{config_file}' is not a valid JSON file.")
 
+        if return_unused_kwargs:
+            return config_dict, kwargs
+
         return config_dict
 
     @staticmethod
     def _get_init_keys(cls):
         return set(dict(inspect.signature(cls.__init__).parameters).keys())
 
     @classmethod
     def extract_init_dict(cls, config_dict, **kwargs):
+        # 0. Copy origin config dict
+        original_dict = {k: v for k, v in config_dict.items()}
+
         # 1. Retrieve expected config attributes from __init__ signature
         expected_keys = cls._get_init_keys(cls)
         expected_keys.remove("self")
         # remove general kwargs if present in dict
         if "kwargs" in expected_keys:
             expected_keys.remove("kwargs")
         # remove flax internal keys
@@ -306,18 +408,19 @@
         # remove keys to be ignored
         if len(cls.ignore_for_config) > 0:
             expected_keys = expected_keys - set(cls.ignore_for_config)
 
         # load diffusers library to import compatible and original scheduler
         diffusers_library = importlib.import_module(__name__.split(".")[0])
 
-        # remove attributes from compatible classes that orig cannot expect
-        compatible_classes = [getattr(diffusers_library, c, None) for c in cls._compatible_classes]
-        # filter out None potentially undefined dummy classes
-        compatible_classes = [c for c in compatible_classes if c is not None]
+        if cls.has_compatibles:
+            compatible_classes = [c for c in cls._get_compatibles() if not isinstance(c, DummyObject)]
+        else:
+            compatible_classes = []
+
         expected_keys_comp_cls = set()
         for c in compatible_classes:
             expected_keys_c = cls._get_init_keys(c)
             expected_keys_comp_cls = expected_keys_comp_cls.union(expected_keys_c)
         expected_keys_comp_cls = expected_keys_comp_cls - cls._get_init_keys(cls)
         config_dict = {k: v for k, v in config_dict.items() if k not in expected_keys_comp_cls}
 
@@ -330,14 +433,19 @@
 
         # remove private attributes
         config_dict = {k: v for k, v in config_dict.items() if not k.startswith("_")}
 
         # 3. Create keyword arguments that will be passed to __init__ from expected keyword arguments
         init_dict = {}
         for key in expected_keys:
+            # if config param is passed to kwarg and is present in config dict
+            # it should overwrite existing config dict key
+            if key in kwargs and key in config_dict:
+                config_dict[key] = kwargs.pop(key)
+
             if key in kwargs:
                 # overwrite key
                 init_dict[key] = kwargs.pop(key)
             elif key in config_dict:
                 # use value from config dict
                 init_dict[key] = config_dict.pop(key)
 
@@ -355,97 +463,77 @@
             logger.info(
                 f"{expected_keys - passed_keys} was not found in config. Values will be initialized to default values."
             )
 
         # 6. Define unused keyword arguments
         unused_kwargs = {**config_dict, **kwargs}
 
-        return init_dict, unused_kwargs
+        # 7. Define "hidden" config parameters that were saved for compatible classes
+        hidden_config_dict = {k: v for k, v in original_dict.items() if k not in init_dict}
+
+        return init_dict, unused_kwargs, hidden_config_dict
 
     @classmethod
     def _dict_from_json_file(cls, json_file: Union[str, os.PathLike]):
         with open(json_file, "r", encoding="utf-8") as reader:
             text = reader.read()
         return json.loads(text)
 
     def __repr__(self):
         return f"{self.__class__.__name__} {self.to_json_string()}"
 
     @property
     def config(self) -> Dict[str, Any]:
+        """
+        Returns the config of the class as a frozen dictionary
+
+        Returns:
+            `Dict[str, Any]`: Config of the class.
+        """
         return self._internal_dict
 
     def to_json_string(self) -> str:
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
             json_file_path (`str` or `os.PathLike`):
                 Path to the JSON file in which this configuration instance's parameters will be saved.
         """
         with open(json_file_path, "w", encoding="utf-8") as writer:
             writer.write(self.to_json_string())
 
 
-class FrozenDict(OrderedDict):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        for key, value in self.items():
-            setattr(self, key, value)
-
-        self.__frozen = True
-
-    def __delitem__(self, *args, **kwargs):
-        raise Exception(f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance.")
-
-    def setdefault(self, *args, **kwargs):
-        raise Exception(f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance.")
-
-    def pop(self, *args, **kwargs):
-        raise Exception(f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
-
-    def update(self, *args, **kwargs):
-        raise Exception(f"You cannot use ``update`` on a {self.__class__.__name__} instance.")
-
-    def __setattr__(self, name, value):
-        if hasattr(self, "__frozen") and self.__frozen:
-            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
-        super().__setattr__(name, value)
-
-    def __setitem__(self, name, value):
-        if hasattr(self, "__frozen") and self.__frozen:
-            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
-        super().__setitem__(name, value)
-
-
 def register_to_config(init):
     r"""
     Decorator to apply on the init of classes inheriting from [`ConfigMixin`] so that all the arguments are
     automatically sent to `self.register_for_config`. To ignore a specific argument accepted by the init but that
     shouldn't be registered in the config, use the `ignore_for_config` class variable
 
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
@@ -462,15 +550,17 @@
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
 
@@ -479,15 +569,15 @@
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/dependency_versions_check.py` & `diffusers-unchained-0.9.0/src/diffusers/dependency_versions_check.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/dependency_versions_table.py` & `diffusers-unchained-0.9.0/src/diffusers/dependency_versions_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # THIS FILE HAS BEEN AUTOGENERATED. To update:
 # 1. modify the `_deps` dict in setup.py
 # 2. run `make deps_table_update``
 deps = {
-    "Pillow": "Pillow<10.0",
+    "Pillow": "Pillow",
     "accelerate": "accelerate>=0.11.0",
     "black": "black==22.8",
     "datasets": "datasets",
     "filelock": "filelock",
     "flake8": "flake8>=3.8.3",
     "flax": "flax>=0.4.1",
     "hf-doc-builder": "hf-doc-builder>=0.3.0",
@@ -17,14 +17,15 @@
     "jaxlib": "jaxlib>=0.1.65",
     "modelcards": "modelcards>=0.1.4",
     "numpy": "numpy",
     "parameterized": "parameterized",
     "pytest": "pytest",
     "pytest-timeout": "pytest-timeout",
     "pytest-xdist": "pytest-xdist",
+    "sentencepiece": "sentencepiece>=0.1.91,!=0.1.92",
     "scipy": "scipy",
     "regex": "regex!=2019.12.17",
     "requests": "requests",
     "tensorboard": "tensorboard",
     "torch": "torch>=1.4",
     "torchvision": "torchvision",
     "transformers": "transformers>=4.21.0",
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/dynamic_modules_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/dynamic_modules_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/hub_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/hub_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/modeling_flax_pytorch_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/modeling_flax_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/modeling_flax_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/modeling_flax_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/modeling_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/modeling_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,45 @@
 import os
 from functools import partial
 from typing import Callable, List, Optional, Tuple, Union
 
 import torch
 from torch import Tensor, device
 
-import accelerate
-from accelerate.utils import set_module_tensor_to_device
-from accelerate.utils.versions import is_torch_version
 from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError, RepositoryNotFoundError, RevisionNotFoundError
 from requests import HTTPError
 
 from . import __version__
-from .utils import CONFIG_NAME, DIFFUSERS_CACHE, HUGGINGFACE_CO_RESOLVE_ENDPOINT, WEIGHTS_NAME, logging
+from .utils import (
+    CONFIG_NAME,
+    DIFFUSERS_CACHE,
+    HUGGINGFACE_CO_RESOLVE_ENDPOINT,
+    WEIGHTS_NAME,
+    is_accelerate_available,
+    is_torch_version,
+    logging,
+)
 
 
 logger = logging.get_logger(__name__)
 
 
 if is_torch_version(">=", "1.9.0"):
     _LOW_CPU_MEM_USAGE_DEFAULT = True
 else:
     _LOW_CPU_MEM_USAGE_DEFAULT = False
 
 
+if is_accelerate_available():
+    import accelerate
+    from accelerate.utils import set_module_tensor_to_device
+    from accelerate.utils.versions import is_torch_version
+
+
 def get_parameter_device(parameter: torch.nn.Module):
     try:
         return next(parameter.parameters()).device
     except StopIteration:
         # For torch.nn.DataParallel compatibility in PyTorch 1.5
 
         def find_tensor_attributes(module: torch.nn.Module) -> List[Tuple[str, Tensor]]:
@@ -315,14 +326,29 @@
         use_auth_token = kwargs.pop("use_auth_token", None)
         revision = kwargs.pop("revision", None)
         torch_dtype = kwargs.pop("torch_dtype", None)
         subfolder = kwargs.pop("subfolder", None)
         device_map = kwargs.pop("device_map", None)
         low_cpu_mem_usage = kwargs.pop("low_cpu_mem_usage", _LOW_CPU_MEM_USAGE_DEFAULT)
 
+        if low_cpu_mem_usage and not is_accelerate_available():
+            low_cpu_mem_usage = False
+            logger.warning(
+                "Cannot initialize model with low cpu memory usage because `accelerate` was not found in the"
+                " environment. Defaulting to `low_cpu_mem_usage=False`. It is strongly recommended to install"
+                " `accelerate` for faster and less memory-intense model loading. You can do so with: \n```\npip"
+                " install accelerate\n```\n."
+            )
+
+        if device_map is not None and not is_accelerate_available():
+            raise NotImplementedError(
+                "Loading and dispatching requires `accelerate`. Please make sure to install accelerate or set"
+                " `device_map=None`. You can install accelerate with `pip install accelerate`."
+            )
+
         # Check if we can handle device_map and dispatching the weights
         if device_map is not None and not is_torch_version(">=", "1.9.0"):
             raise NotImplementedError(
                 "Loading and dispatching requires torch >= 1.9.0. Please either update your PyTorch version or set"
                 " `device_map=None`."
             )
 
@@ -418,28 +444,29 @@
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
@@ -452,28 +479,29 @@
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/attention.py` & `diffusers-unchained-0.9.0/src/diffusers/models/attention.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
+import warnings
 from dataclasses import dataclass
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
@@ -94,16 +95,19 @@
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
@@ -121,15 +125,18 @@
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
@@ -147,22 +154,26 @@
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
@@ -186,29 +197,44 @@
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
 
@@ -280,30 +306,60 @@
         hidden_states = hidden_states.view(batch, channel, height * width).transpose(1, 2)
 
         # proj to q, k, v
         query_proj = self.query(hidden_states)
         key_proj = self.key(hidden_states)
         value_proj = self.value(hidden_states)
 
-        # transpose
-        query_states = self.transpose_for_scores(query_proj)
-        key_states = self.transpose_for_scores(key_proj)
-        value_states = self.transpose_for_scores(value_proj)
+        scale = 1 / math.sqrt(self.channels / self.num_heads)
 
         # get scores
-        scale = 1 / math.sqrt(math.sqrt(self.channels / self.num_heads))
-        attention_scores = torch.matmul(query_states * scale, key_states.transpose(-1, -2) * scale)  # TODO: use baddmm
+        if self.num_heads > 1:
+            query_states = self.transpose_for_scores(query_proj)
+            key_states = self.transpose_for_scores(key_proj)
+            value_states = self.transpose_for_scores(value_proj)
+
+            # TODO: is there a way to perform batched matmul (e.g. baddbmm) on 4D tensors?
+            #       or reformulate this into a 3D problem?
+            # TODO: measure whether on MPS device it would be faster to do this matmul via einsum
+            #       as some matmuls can be 1.94x slower than an equivalent einsum on MPS
+            #       https://gist.github.com/Birch-san/cba16789ec27bb20996a4b4831b13ce0
+            attention_scores = torch.matmul(query_states, key_states.transpose(-1, -2)) * scale
+        else:
+            query_states, key_states, value_states = query_proj, key_proj, value_proj
+
+            attention_scores = torch.baddbmm(
+                torch.empty(
+                    query_states.shape[0],
+                    query_states.shape[1],
+                    key_states.shape[1],
+                    dtype=query_states.dtype,
+                    device=query_states.device,
+                ),
+                query_states,
+                key_states.transpose(-1, -2),
+                beta=0,
+                alpha=scale,
+            )
+
         attention_probs = torch.softmax(attention_scores.float(), dim=-1).type(attention_scores.dtype)
 
         # compute attention output
-        hidden_states = torch.matmul(attention_probs, value_states)
-
-        hidden_states = hidden_states.permute(0, 2, 1, 3).contiguous()
-        new_hidden_states_shape = hidden_states.size()[:-2] + (self.channels,)
-        hidden_states = hidden_states.view(new_hidden_states_shape)
+        if self.num_heads > 1:
+            # TODO: is there a way to perform batched matmul (e.g. bmm) on 4D tensors?
+            #       or reformulate this into a 3D problem?
+            # TODO: measure whether on MPS device it would be faster to do this matmul via einsum
+            #       as some matmuls can be 1.94x slower than an equivalent einsum on MPS
+            #       https://gist.github.com/Birch-san/cba16789ec27bb20996a4b4831b13ce0
+            hidden_states = torch.matmul(attention_probs, value_states)
+            hidden_states = hidden_states.permute(0, 2, 1, 3).contiguous()
+            new_hidden_states_shape = hidden_states.size()[:-2] + (self.channels,)
+            hidden_states = hidden_states.view(new_hidden_states_shape)
+        else:
+            hidden_states = torch.bmm(attention_probs, value_states)
 
         # compute next hidden_states
         hidden_states = self.proj_attn(hidden_states)
         hidden_states = hidden_states.transpose(-1, -2).reshape(batch, channel, height, width)
 
         # res connect and rescale
         hidden_states = (hidden_states + residual) / self.rescale_output_factor
@@ -333,22 +389,25 @@
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
@@ -362,14 +421,24 @@
             self.norm1 = AdaLayerNorm(dim, num_embeds_ada_norm)
             self.norm2 = AdaLayerNorm(dim, num_embeds_ada_norm)
         else:
             self.norm1 = nn.LayerNorm(dim)
             self.norm2 = nn.LayerNorm(dim)
         self.norm3 = nn.LayerNorm(dim)
 
+        # if xformers is installed try to use memory_efficient_attention by default
+        if is_xformers_available():
+            try:
+                self._set_use_memory_efficient_attention_xformers(True)
+            except Exception as e:
+                warnings.warn(
+                    "Could not enable memory efficient attention. Make sure xformers is installed"
+                    f" correctly and a GPU is available: {e}"
+                )
+
     def _set_attention_slice(self, slice_size):
         self.attn1._slice_size = slice_size
         self.attn2._slice_size = slice_size
 
     def _set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
         if not is_xformers_available():
             print("Here is how to install it")
@@ -397,15 +466,19 @@
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
 
@@ -488,77 +561,74 @@
         value = self.reshape_heads_to_batch_dim(value)
 
         # TODO(PVP) - mask is currently never used. Remember to re-implement when used
 
         # attention, what we cannot get enough of
         if self._use_memory_efficient_attention_xformers:
             hidden_states = self._memory_efficient_attention_xformers(query, key, value)
+            # Some versions of xformers return output in fp32, cast it back to the dtype of the input
+            hidden_states = hidden_states.to(query.dtype)
         else:
             if self._slice_size is None or query.shape[0] // self._slice_size == 1:
                 hidden_states = self._attention(query, key, value)
             else:
                 hidden_states = self._sliced_attention(query, key, value, sequence_length, dim)
 
         # linear proj
         hidden_states = self.to_out[0](hidden_states)
         # dropout
         hidden_states = self.to_out[1](hidden_states)
         return hidden_states
 
     def _attention(self, query, key, value):
-        # TODO: use baddbmm for better performance
-        if query.device.type == "mps":
-            # Better performance on mps (~20-25%)
-            attention_scores = torch.einsum("b i d, b j d -> b i j", query, key) * self.scale
-        else:
-            attention_scores = torch.matmul(query, key.transpose(-1, -2)) * self.scale
+        attention_scores = torch.baddbmm(
+            torch.empty(query.shape[0], query.shape[1], key.shape[1], dtype=query.dtype, device=query.device),
+            query,
+            key.transpose(-1, -2),
+            beta=0,
+            alpha=self.scale,
+        )
         attention_probs = attention_scores.softmax(dim=-1)
         # compute attention output
 
-        if query.device.type == "mps":
-            hidden_states = torch.einsum("b i j, b j d -> b i d", attention_probs, value)
-        else:
-            hidden_states = torch.matmul(attention_probs, value)
+        hidden_states = torch.bmm(attention_probs, value)
 
         # reshape hidden_states
         hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
         return hidden_states
 
     def _sliced_attention(self, query, key, value, sequence_length, dim):
         batch_size_attention = query.shape[0]
         hidden_states = torch.zeros(
             (batch_size_attention, sequence_length, dim // self.heads), device=query.device, dtype=query.dtype
         )
         slice_size = self._slice_size if self._slice_size is not None else hidden_states.shape[0]
         for i in range(hidden_states.shape[0] // slice_size):
             start_idx = i * slice_size
             end_idx = (i + 1) * slice_size
-            if query.device.type == "mps":
-                # Better performance on mps (~20-25%)
-                attn_slice = (
-                    torch.einsum("b i d, b j d -> b i j", query[start_idx:end_idx], key[start_idx:end_idx])
-                    * self.scale
-                )
-            else:
-                attn_slice = (
-                    torch.matmul(query[start_idx:end_idx], key[start_idx:end_idx].transpose(1, 2)) * self.scale
-                )  # TODO: use baddbmm for better performance
+            attn_slice = torch.baddbmm(
+                torch.empty(slice_size, query.shape[1], key.shape[1], dtype=query.dtype, device=query.device),
+                query[start_idx:end_idx],
+                key[start_idx:end_idx].transpose(-1, -2),
+                beta=0,
+                alpha=self.scale,
+            )
             attn_slice = attn_slice.softmax(dim=-1)
-            if query.device.type == "mps":
-                attn_slice = torch.einsum("b i j, b j d -> b i d", attn_slice, value[start_idx:end_idx])
-            else:
-                attn_slice = torch.matmul(attn_slice, value[start_idx:end_idx])
+            attn_slice = torch.bmm(attn_slice, value[start_idx:end_idx])
 
             hidden_states[start_idx:end_idx] = attn_slice
 
         # reshape hidden_states
         hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
         return hidden_states
 
     def _memory_efficient_attention_xformers(self, query, key, value):
+        query = query.contiguous()
+        key = key.contiguous()
+        value = value.contiguous()
         hidden_states = xformers.ops.memory_efficient_attention(query, key, value, attn_bias=None)
         hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
         return hidden_states
 
 
 class FeedForward(nn.Module):
     r"""
@@ -657,7 +727,133 @@
         self.norm = nn.LayerNorm(embedding_dim, elementwise_affine=False)
 
     def forward(self, x, timestep):
         emb = self.linear(self.silu(self.emb(timestep)))
         scale, shift = torch.chunk(emb, 2)
         x = self.norm(x) * (1 + scale) + shift
         return x
+
+
+class DualTransformer2DModel(nn.Module):
+    """
+    Dual transformer wrapper that combines two `Transformer2DModel`s for mixed inference.
+
+    Parameters:
+        num_attention_heads (`int`, *optional*, defaults to 16): The number of heads to use for multi-head attention.
+        attention_head_dim (`int`, *optional*, defaults to 88): The number of channels in each head.
+        in_channels (`int`, *optional*):
+            Pass if the input is continuous. The number of channels in the input and output.
+        num_layers (`int`, *optional*, defaults to 1): The number of layers of Transformer blocks to use.
+        dropout (`float`, *optional*, defaults to 0.1): The dropout probability to use.
+        cross_attention_dim (`int`, *optional*): The number of context dimensions to use.
+        sample_size (`int`, *optional*): Pass if the input is discrete. The width of the latent images.
+            Note that this is fixed at training time as it is used for learning a number of position embeddings. See
+            `ImagePositionalEmbeddings`.
+        num_vector_embeds (`int`, *optional*):
+            Pass if the input is discrete. The number of classes of the vector embeddings of the latent pixels.
+            Includes the class for the masked latent pixel.
+        activation_fn (`str`, *optional*, defaults to `"geglu"`): Activation function to be used in feed-forward.
+        num_embeds_ada_norm ( `int`, *optional*): Pass if at least one of the norm_layers is `AdaLayerNorm`.
+            The number of diffusion steps used during training. Note that this is fixed at training time as it is used
+            to learn a number of embeddings that are added to the hidden states. During inference, you can denoise for
+            up to but not more than steps than `num_embeds_ada_norm`.
+        attention_bias (`bool`, *optional*):
+            Configure if the TransformerBlocks' attention should contain a bias parameter.
+    """
+
+    def __init__(
+        self,
+        num_attention_heads: int = 16,
+        attention_head_dim: int = 88,
+        in_channels: Optional[int] = None,
+        num_layers: int = 1,
+        dropout: float = 0.0,
+        norm_num_groups: int = 32,
+        cross_attention_dim: Optional[int] = None,
+        attention_bias: bool = False,
+        sample_size: Optional[int] = None,
+        num_vector_embeds: Optional[int] = None,
+        activation_fn: str = "geglu",
+        num_embeds_ada_norm: Optional[int] = None,
+    ):
+        super().__init__()
+        self.transformers = nn.ModuleList(
+            [
+                Transformer2DModel(
+                    num_attention_heads=num_attention_heads,
+                    attention_head_dim=attention_head_dim,
+                    in_channels=in_channels,
+                    num_layers=num_layers,
+                    dropout=dropout,
+                    norm_num_groups=norm_num_groups,
+                    cross_attention_dim=cross_attention_dim,
+                    attention_bias=attention_bias,
+                    sample_size=sample_size,
+                    num_vector_embeds=num_vector_embeds,
+                    activation_fn=activation_fn,
+                    num_embeds_ada_norm=num_embeds_ada_norm,
+                )
+                for _ in range(2)
+            ]
+        )
+
+        # Variables that can be set by a pipeline:
+
+        # The ratio of transformer1 to transformer2's output states to be combined during inference
+        self.mix_ratio = 0.5
+
+        # The shape of `encoder_hidden_states` is expected to be
+        # `(batch_size, condition_lengths[0]+condition_lengths[1], num_features)`
+        self.condition_lengths = [77, 257]
+
+        # Which transformer to use to encode which condition.
+        # E.g. `(1, 0)` means that we'll use `transformers[1](conditions[0])` and `transformers[0](conditions[1])`
+        self.transformer_index_for_condition = [1, 0]
+
+    def forward(self, hidden_states, encoder_hidden_states, timestep=None, return_dict: bool = True):
+        """
+        Args:
+            hidden_states ( When discrete, `torch.LongTensor` of shape `(batch size, num latent pixels)`.
+                When continuous, `torch.FloatTensor` of shape `(batch size, channel, height, width)`): Input
+                hidden_states
+            encoder_hidden_states ( `torch.LongTensor` of shape `(batch size, context dim)`, *optional*):
+                Conditional embeddings for cross attention layer. If not given, cross-attention defaults to
+                self-attention.
+            timestep ( `torch.long`, *optional*):
+                Optional timestep to be applied as an embedding in AdaLayerNorm's. Used to indicate denoising step.
+            return_dict (`bool`, *optional*, defaults to `True`):
+                Whether or not to return a [`models.unet_2d_condition.UNet2DConditionOutput`] instead of a plain tuple.
+
+        Returns:
+            [`~models.attention.Transformer2DModelOutput`] or `tuple`: [`~models.attention.Transformer2DModelOutput`]
+            if `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample
+            tensor.
+        """
+        input_states = hidden_states
+
+        encoded_states = []
+        tokens_start = 0
+        for i in range(2):
+            # for each of the two transformers, pass the corresponding condition tokens
+            condition_state = encoder_hidden_states[:, tokens_start : tokens_start + self.condition_lengths[i]]
+            transformer_index = self.transformer_index_for_condition[i]
+            encoded_state = self.transformers[transformer_index](input_states, condition_state, timestep, return_dict)[
+                0
+            ]
+            encoded_states.append(encoded_state - input_states)
+            tokens_start += self.condition_lengths[i]
+
+        output_states = encoded_states[0] * self.mix_ratio + encoded_states[1] * (1 - self.mix_ratio)
+        output_states = output_states + input_states
+
+        if not return_dict:
+            return (output_states,)
+
+        return Transformer2DModelOutput(sample=output_states)
+
+    def _set_attention_slice(self, slice_size):
+        for transformer in self.transformers:
+            transformer._set_attention_slice(slice_size)
+
+    def _set_use_memory_efficient_attention_xformers(self, use_memory_efficient_attention_xformers: bool):
+        for transformer in self.transformers:
+            transformer._set_use_memory_efficient_attention_xformers(use_memory_efficient_attention_xformers)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/attention_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/attention_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/embeddings.py` & `diffusers-unchained-0.9.0/src/diffusers/models/embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,22 +58,29 @@
     # zero pad
     if embedding_dim % 2 == 1:
         emb = torch.nn.functional.pad(emb, (0, 1, 0, 0))
     return emb
 
 
 class TimestepEmbedding(nn.Module):
-    def __init__(self, channel: int, time_embed_dim: int, act_fn: str = "silu"):
+    def __init__(self, in_channels: int, time_embed_dim: int, act_fn: str = "silu", out_dim: int = None):
         super().__init__()
 
-        self.linear_1 = nn.Linear(channel, time_embed_dim)
+        self.linear_1 = nn.Linear(in_channels, time_embed_dim)
         self.act = None
         if act_fn == "silu":
             self.act = nn.SiLU()
-        self.linear_2 = nn.Linear(time_embed_dim, time_embed_dim)
+        elif act_fn == "mish":
+            self.act = nn.Mish()
+
+        if out_dim is not None:
+            time_embed_dim_out = out_dim
+        else:
+            time_embed_dim_out = time_embed_dim
+        self.linear_2 = nn.Linear(time_embed_dim, time_embed_dim_out)
 
     def forward(self, sample):
         sample = self.linear_1(sample)
 
         if self.act is not None:
             sample = self.act(sample)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/embeddings_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/embeddings_flax.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,8 +84,10 @@
                 Time step embedding dimension
     """
     dim: int = 32
     freq_shift: float = 1
 
     @nn.compact
     def __call__(self, timesteps):
-        return get_sinusoidal_embeddings(timesteps, embedding_dim=self.dim, freq_shift=self.freq_shift)
+        return get_sinusoidal_embeddings(
+            timesteps, embedding_dim=self.dim, freq_shift=self.freq_shift, flip_sin_to_cos=True
+        )
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/resnet.py` & `diffusers-unchained-0.9.0/src/diffusers/models/resnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,92 @@
 from functools import partial
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
+class Upsample1D(nn.Module):
+    """
+    An upsampling layer with an optional convolution.
+
+    Parameters:
+            channels: channels in the inputs and outputs.
+            use_conv: a bool determining if a convolution is applied.
+            use_conv_transpose:
+            out_channels:
+    """
+
+    def __init__(self, channels, use_conv=False, use_conv_transpose=False, out_channels=None, name="conv"):
+        super().__init__()
+        self.channels = channels
+        self.out_channels = out_channels or channels
+        self.use_conv = use_conv
+        self.use_conv_transpose = use_conv_transpose
+        self.name = name
+
+        self.conv = None
+        if use_conv_transpose:
+            self.conv = nn.ConvTranspose1d(channels, self.out_channels, 4, 2, 1)
+        elif use_conv:
+            self.conv = nn.Conv1d(self.channels, self.out_channels, 3, padding=1)
+
+    def forward(self, x):
+        assert x.shape[1] == self.channels
+        if self.use_conv_transpose:
+            return self.conv(x)
+
+        x = F.interpolate(x, scale_factor=2.0, mode="nearest")
+
+        if self.use_conv:
+            x = self.conv(x)
+
+        return x
+
+
+class Downsample1D(nn.Module):
+    """
+    A downsampling layer with an optional convolution.
+
+    Parameters:
+        channels: channels in the inputs and outputs.
+        use_conv: a bool determining if a convolution is applied.
+        out_channels:
+        padding:
+    """
+
+    def __init__(self, channels, use_conv=False, out_channels=None, padding=1, name="conv"):
+        super().__init__()
+        self.channels = channels
+        self.out_channels = out_channels or channels
+        self.use_conv = use_conv
+        self.padding = padding
+        stride = 2
+        self.name = name
+
+        if use_conv:
+            self.conv = nn.Conv1d(self.channels, self.out_channels, 3, stride=stride, padding=padding)
+        else:
+            assert self.channels == self.out_channels
+            self.conv = nn.AvgPool1d(kernel_size=stride, stride=stride)
+
+    def forward(self, x):
+        assert x.shape[1] == self.channels
+        return self.conv(x)
+
+
 class Upsample2D(nn.Module):
     """
     An upsampling layer with an optional convolution.
 
     Parameters:
         channels: channels in the inputs and outputs.
         use_conv: a bool determining if a convolution is applied.
-        dims: determines if the signal is 1D, 2D, or 3D. If 3D, then upsampling occurs in the inner-two dimensions.
+        use_conv_transpose:
+        out_channels:
     """
 
     def __init__(self, channels, use_conv=False, use_conv_transpose=False, out_channels=None, name="conv"):
         super().__init__()
         self.channels = channels
         self.out_channels = out_channels or channels
         self.use_conv = use_conv
@@ -76,15 +146,16 @@
 class Downsample2D(nn.Module):
     """
     A downsampling layer with an optional convolution.
 
     Parameters:
         channels: channels in the inputs and outputs.
         use_conv: a bool determining if a convolution is applied.
-        dims: determines if the signal is 1D, 2D, or 3D. If 3D, then downsampling occurs in the inner-two dimensions.
+        out_channels:
+        padding:
     """
 
     def __init__(self, channels, use_conv=False, out_channels=None, padding=1, name="conv"):
         super().__init__()
         self.channels = channels
         self.out_channels = out_channels or channels
         self.use_conv = use_conv
@@ -411,14 +482,77 @@
 
 
 class Mish(torch.nn.Module):
     def forward(self, hidden_states):
         return hidden_states * torch.tanh(torch.nn.functional.softplus(hidden_states))
 
 
+# unet_rl.py
+def rearrange_dims(tensor):
+    if len(tensor.shape) == 2:
+        return tensor[:, :, None]
+    if len(tensor.shape) == 3:
+        return tensor[:, :, None, :]
+    elif len(tensor.shape) == 4:
+        return tensor[:, :, 0, :]
+    else:
+        raise ValueError(f"`len(tensor)`: {len(tensor)} has to be 2, 3 or 4.")
+
+
+class Conv1dBlock(nn.Module):
+    """
+    Conv1d --> GroupNorm --> Mish
+    """
+
+    def __init__(self, inp_channels, out_channels, kernel_size, n_groups=8):
+        super().__init__()
+
+        self.conv1d = nn.Conv1d(inp_channels, out_channels, kernel_size, padding=kernel_size // 2)
+        self.group_norm = nn.GroupNorm(n_groups, out_channels)
+        self.mish = nn.Mish()
+
+    def forward(self, x):
+        x = self.conv1d(x)
+        x = rearrange_dims(x)
+        x = self.group_norm(x)
+        x = rearrange_dims(x)
+        x = self.mish(x)
+        return x
+
+
+# unet_rl.py
+class ResidualTemporalBlock1D(nn.Module):
+    def __init__(self, inp_channels, out_channels, embed_dim, kernel_size=5):
+        super().__init__()
+        self.conv_in = Conv1dBlock(inp_channels, out_channels, kernel_size)
+        self.conv_out = Conv1dBlock(out_channels, out_channels, kernel_size)
+
+        self.time_emb_act = nn.Mish()
+        self.time_emb = nn.Linear(embed_dim, out_channels)
+
+        self.residual_conv = (
+            nn.Conv1d(inp_channels, out_channels, 1) if inp_channels != out_channels else nn.Identity()
+        )
+
+    def forward(self, x, t):
+        """
+        Args:
+            x : [ batch_size x inp_channels x horizon ]
+            t : [ batch_size x embed_dim ]
+
+        returns:
+            out : [ batch_size x out_channels x horizon ]
+        """
+        t = self.time_emb_act(t)
+        t = self.time_emb(t)
+        out = self.conv_in(x) + rearrange_dims(t)
+        out = self.conv_out(out)
+        return out + self.residual_conv(x)
+
+
 def upsample_2d(hidden_states, kernel=None, factor=2, gain=1):
     r"""Upsample2D a batch of 2D images with the given filter.
     Accepts a batch of 2D images of the shape `[N, C, H, W]` or `[N, H, W, C]` and upsamples each image with the given
     filter. The filter is normalized so that if the input pixels are constant, they will be scaled by the specified
     `gain`. Pixels outside the image are assumed to be zero, and the filter is padded with zeros so that its shape is
     a: multiple of the upsampling factor.
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/resnet_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/resnet_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_1d.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_1d.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,32 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..modeling_utils import ModelMixin
 from ..utils import BaseOutput
 from .embeddings import GaussianFourierProjection, TimestepEmbedding, Timesteps
-from .unet_1d_blocks import get_down_block, get_mid_block, get_up_block
+from .unet_1d_blocks import get_down_block, get_mid_block, get_out_block, get_up_block
 
 
 @dataclass
 class UNet1DOutput(BaseOutput):
     """
     Args:
         sample (`torch.FloatTensor` of shape `(batch_size, num_channels, sample_size)`):
@@ -26,63 +40,81 @@
     r"""
     UNet1DModel is a 1D UNet model that takes in a noisy sample and a timestep and returns sample shaped output.
 
     This model inherits from [`ModelMixin`]. Check the superclass documentation for the generic methods the library
     implements for all the model (such as downloading or saving, etc.)
 
     Parameters:
-        sample_size (`int`, *optionl*): Default length of sample. Should be adaptable at runtime.
+        sample_size (`int`, *optional*): Default length of sample. Should be adaptable at runtime.
         in_channels (`int`, *optional*, defaults to 2): Number of channels in the input sample.
         out_channels (`int`, *optional*, defaults to 2): Number of channels in the output.
         time_embedding_type (`str`, *optional*, defaults to `"fourier"`): Type of time embedding to use.
-        freq_shift (`int`, *optional*, defaults to 0): Frequency shift for fourier time embedding.
+        freq_shift (`float`, *optional*, defaults to 0.0): Frequency shift for fourier time embedding.
         flip_sin_to_cos (`bool`, *optional*, defaults to :
             obj:`False`): Whether to flip sin to cos for fourier time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("DownBlock1D", "DownBlock1DNoSkip", "AttnDownBlock1D")`): Tuple of downsample block types.
         up_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("UpBlock1D", "UpBlock1DNoSkip", "AttnUpBlock1D")`): Tuple of upsample block types.
         block_out_channels (`Tuple[int]`, *optional*, defaults to :
             obj:`(32, 32, 64)`): Tuple of block output channels.
+        mid_block_type (`str`, *optional*, defaults to "UNetMidBlock1D"): block type for middle of UNet.
+        out_block_type (`str`, *optional*, defaults to `None`): optional output processing of UNet.
+        act_fn (`str`, *optional*, defaults to None): optional activitation function in UNet blocks.
+        norm_num_groups (`int`, *optional*, defaults to 8): group norm member count in UNet blocks.
+        layers_per_block (`int`, *optional*, defaults to 1): added number of layers in a UNet block.
+        downsample_each_block (`int`, *optional*, defaults to False:
+            experimental feature for using a UNet without upsampling.
     """
 
     @register_to_config
     def __init__(
         self,
         sample_size: int = 65536,
         sample_rate: Optional[int] = None,
         in_channels: int = 2,
         out_channels: int = 2,
         extra_in_channels: int = 0,
         time_embedding_type: str = "fourier",
-        freq_shift: int = 0,
         flip_sin_to_cos: bool = True,
         use_timestep_embedding: bool = False,
+        freq_shift: float = 0.0,
         down_block_types: Tuple[str] = ("DownBlock1DNoSkip", "DownBlock1D", "AttnDownBlock1D"),
-        mid_block_type: str = "UNetMidBlock1D",
         up_block_types: Tuple[str] = ("AttnUpBlock1D", "UpBlock1D", "UpBlock1DNoSkip"),
+        mid_block_type: Tuple[str] = "UNetMidBlock1D",
+        out_block_type: str = None,
         block_out_channels: Tuple[int] = (32, 32, 64),
+        act_fn: str = None,
+        norm_num_groups: int = 8,
+        layers_per_block: int = 1,
+        downsample_each_block: bool = False,
     ):
         super().__init__()
-
         self.sample_size = sample_size
 
         # time
         if time_embedding_type == "fourier":
             self.time_proj = GaussianFourierProjection(
                 embedding_size=8, set_W_to_weight=False, log=False, flip_sin_to_cos=flip_sin_to_cos
             )
             timestep_input_dim = 2 * block_out_channels[0]
         elif time_embedding_type == "positional":
-            self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos, freq_shift)
+            self.time_proj = Timesteps(
+                block_out_channels[0], flip_sin_to_cos=flip_sin_to_cos, downscale_freq_shift=freq_shift
+            )
             timestep_input_dim = block_out_channels[0]
 
         if use_timestep_embedding:
             time_embed_dim = block_out_channels[0] * 4
-            self.time_embedding = TimestepEmbedding(timestep_input_dim, time_embed_dim)
+            self.time_mlp = TimestepEmbedding(
+                in_channels=timestep_input_dim,
+                time_embed_dim=time_embed_dim,
+                act_fn=act_fn,
+                out_dim=block_out_channels[0],
+            )
 
         self.down_blocks = nn.ModuleList([])
         self.mid_block = None
         self.up_blocks = nn.ModuleList([])
         self.out_block = None
 
         # down
@@ -90,46 +122,74 @@
         for i, down_block_type in enumerate(down_block_types):
             input_channel = output_channel
             output_channel = block_out_channels[i]
 
             if i == 0:
                 input_channel += extra_in_channels
 
+            is_final_block = i == len(block_out_channels) - 1
+
             down_block = get_down_block(
                 down_block_type,
+                num_layers=layers_per_block,
                 in_channels=input_channel,
                 out_channels=output_channel,
+                temb_channels=block_out_channels[0],
+                add_downsample=not is_final_block or downsample_each_block,
             )
             self.down_blocks.append(down_block)
 
         # mid
         self.mid_block = get_mid_block(
-            mid_block_type=mid_block_type,
-            mid_channels=block_out_channels[-1],
+            mid_block_type,
             in_channels=block_out_channels[-1],
-            out_channels=None,
+            mid_channels=block_out_channels[-1],
+            out_channels=block_out_channels[-1],
+            embed_dim=block_out_channels[0],
+            num_layers=layers_per_block,
+            add_downsample=downsample_each_block,
         )
 
         # up
         reversed_block_out_channels = list(reversed(block_out_channels))
         output_channel = reversed_block_out_channels[0]
+        if out_block_type is None:
+            final_upsample_channels = out_channels
+        else:
+            final_upsample_channels = block_out_channels[0]
+
         for i, up_block_type in enumerate(up_block_types):
             prev_output_channel = output_channel
-            output_channel = reversed_block_out_channels[i + 1] if i < len(up_block_types) - 1 else out_channels
+            output_channel = (
+                reversed_block_out_channels[i + 1] if i < len(up_block_types) - 1 else final_upsample_channels
+            )
+
+            is_final_block = i == len(block_out_channels) - 1
 
             up_block = get_up_block(
                 up_block_type,
+                num_layers=layers_per_block,
                 in_channels=prev_output_channel,
                 out_channels=output_channel,
+                temb_channels=block_out_channels[0],
+                add_upsample=not is_final_block,
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
-        # TODO(PVP, Nathan) placeholder for RL application to be merged shortly
-        # Totally fine to add another layer with a if statement - no need for nn.Identity here
+        # out
+        num_groups_out = norm_num_groups if norm_num_groups is not None else min(block_out_channels[0] // 4, 32)
+        self.out_block = get_out_block(
+            out_block_type=out_block_type,
+            num_groups_out=num_groups_out,
+            embed_dim=block_out_channels[0],
+            out_channels=out_channels,
+            act_fn=act_fn,
+            fc_dim=block_out_channels[-1] // 4,
+        )
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: Union[torch.Tensor, float, int],
         return_dict: bool = True,
     ) -> Union[UNet1DOutput, Tuple]:
@@ -140,33 +200,46 @@
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~models.unet_1d.UNet1DOutput`] instead of a plain tuple.
 
         Returns:
             [`~models.unet_1d.UNet1DOutput`] or `tuple`: [`~models.unet_1d.UNet1DOutput`] if `return_dict` is True,
             otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
         """
-        # 1. time
-        if len(timestep.shape) == 0:
-            timestep = timestep[None]
 
-        timestep_embed = self.time_proj(timestep)[..., None]
-        timestep_embed = timestep_embed.repeat([1, 1, sample.shape[2]]).to(sample.dtype)
+        # 1. time
+        timesteps = timestep
+        if not torch.is_tensor(timesteps):
+            timesteps = torch.tensor([timesteps], dtype=torch.long, device=sample.device)
+        elif torch.is_tensor(timesteps) and len(timesteps.shape) == 0:
+            timesteps = timesteps[None].to(sample.device)
+
+        timestep_embed = self.time_proj(timesteps)
+        if self.config.use_timestep_embedding:
+            timestep_embed = self.time_mlp(timestep_embed)
+        else:
+            timestep_embed = timestep_embed[..., None]
+            timestep_embed = timestep_embed.repeat([1, 1, sample.shape[2]]).to(sample.dtype)
 
         # 2. down
         down_block_res_samples = ()
         for downsample_block in self.down_blocks:
             sample, res_samples = downsample_block(hidden_states=sample, temb=timestep_embed)
             down_block_res_samples += res_samples
 
         # 3. mid
-        sample = self.mid_block(sample)
+        if self.mid_block:
+            sample = self.mid_block(sample, timestep_embed)
 
         # 4. up
         for i, upsample_block in enumerate(self.up_blocks):
             res_samples = down_block_res_samples[-1:]
             down_block_res_samples = down_block_res_samples[:-1]
-            sample = upsample_block(sample, res_samples)
+            sample = upsample_block(sample, res_hidden_states_tuple=res_samples, temb=timestep_embed)
+
+        # 5. post-process
+        if self.out_block:
+            sample = self.out_block(sample, timestep_embed)
 
         if not return_dict:
             return (sample,)
 
         return UNet1DOutput(sample=sample)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_2d.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,23 +39,23 @@
     r"""
     UNet2DModel is a 2D UNet model that takes in a noisy sample and a timestep and returns sample shaped output.
 
     This model inherits from [`ModelMixin`]. Check the superclass documentation for the generic methods the library
     implements for all the model (such as downloading or saving, etc.)
 
     Parameters:
-        sample_size (`torch.FloatTensor` of shape `(batch_size, num_channels, height, width)`, *optional*):
-            Input sample size.
+        sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
+            Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 3): Number of channels in the input image.
         out_channels (`int`, *optional*, defaults to 3): Number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
         time_embedding_type (`str`, *optional*, defaults to `"positional"`): Type of time embedding to use.
         freq_shift (`int`, *optional*, defaults to 0): Frequency shift for fourier time embedding.
         flip_sin_to_cos (`bool`, *optional*, defaults to :
-            obj:`False`): Whether to flip sin to cos for fourier time embedding.
+            obj:`True`): Whether to flip sin to cos for fourier time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("DownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D")`): Tuple of downsample block
             types.
         up_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("AttnUpBlock2D", "AttnUpBlock2D", "AttnUpBlock2D", "UpBlock2D")`): Tuple of upsample block types.
         block_out_channels (`Tuple[int]`, *optional*, defaults to :
             obj:`(224, 448, 672, 896)`): Tuple of block output channels.
@@ -67,15 +67,15 @@
         norm_num_groups (`int`, *optional*, defaults to `32`): The number of groups for the normalization.
         norm_eps (`float`, *optional*, defaults to `1e-5`): The epsilon for the normalization.
     """
 
     @register_to_config
     def __init__(
         self,
-        sample_size: Optional[int] = None,
+        sample_size: Optional[Union[int, Tuple[int, int]]] = None,
         in_channels: int = 3,
         out_channels: int = 3,
         center_input_sample: bool = False,
         time_embedding_type: str = "positional",
         freq_shift: int = 0,
         flip_sin_to_cos: bool = True,
         down_block_types: Tuple[str] = ("DownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D"),
@@ -171,15 +171,15 @@
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
         num_groups_out = norm_num_groups if norm_num_groups is not None else min(block_out_channels[0] // 4, 32)
         self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0], num_groups=num_groups_out, eps=norm_eps)
         self.conv_act = nn.SiLU()
-        self.conv_out = nn.Conv2d(block_out_channels[0], out_channels, 3, padding=1)
+        self.conv_out = nn.Conv2d(block_out_channels[0], out_channels, kernel_size=3, padding=1)
 
     def forward(
         self,
         sample: torch.FloatTensor,
         timestep: Union[torch.Tensor, float, int],
         return_dict: bool = True,
     ) -> Union[UNet2DOutput, Tuple]:
@@ -205,14 +205,19 @@
         elif torch.is_tensor(timesteps) and len(timesteps.shape) == 0:
             timesteps = timesteps[None].to(sample.device)
 
         # broadcast to batch dimension in a way that's compatible with ONNX/Core ML
         timesteps = timesteps * torch.ones(sample.shape[0], dtype=timesteps.dtype, device=timesteps.device)
 
         t_emb = self.time_proj(timesteps)
+
+        # timesteps does not contain any weights and will always return f32 tensors
+        # but time_embedding might actually be running in fp16. so we need to cast here.
+        # there might be better ways to encapsulate this.
+        t_emb = t_emb.to(dtype=self.dtype)
         emb = self.time_embedding(t_emb)
 
         # 2. pre-process
         skip_sample = sample
         sample = self.conv_in(sample)
 
         # 3. down
@@ -238,17 +243,15 @@
 
             if hasattr(upsample_block, "skip_conv"):
                 sample, skip_sample = upsample_block(sample, res_samples, emb, skip_sample)
             else:
                 sample = upsample_block(sample, res_samples, emb)
 
         # 6. post-process
-        # make sure hidden states is in float32
-        # when running in half-precision
-        sample = self.conv_norm_out(sample.float()).type(sample.dtype)
+        sample = self.conv_norm_out(sample)
         sample = self.conv_act(sample)
         sample = self.conv_out(sample)
 
         if skip_sample is not None:
             sample += skip_sample
 
         if self.config.time_embedding_type == "fourier":
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_blocks.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
 import torch
 from torch import nn
 
-from .attention import AttentionBlock, Transformer2DModel
+from .attention import AttentionBlock, DualTransformer2DModel, Transformer2DModel
 from .resnet import Downsample2D, FirDownsample2D, FirUpsample2D, ResnetBlock2D, Upsample2D
 
 
 def get_down_block(
     down_block_type,
     num_layers,
     in_channels,
@@ -28,14 +28,17 @@
     add_downsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
     downsample_padding=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     down_block_type = down_block_type[7:] if down_block_type.startswith("UNetRes") else down_block_type
     if down_block_type == "DownBlock2D":
         return DownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -70,14 +73,17 @@
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
     elif down_block_type == "SkipDownBlock2D":
         return SkipDownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             temb_channels=temb_channels,
@@ -133,14 +139,17 @@
     temb_channels,
     add_upsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
     up_block_type = up_block_type[7:] if up_block_type.startswith("UNetRes") else up_block_type
     if up_block_type == "UpBlock2D":
         return UpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
@@ -162,14 +171,17 @@
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
     elif up_block_type == "AttnUpBlock2D":
         return AttnUpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             prev_output_channel=prev_output_channel,
@@ -238,15 +250,14 @@
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
@@ -318,15 +329,16 @@
         resnet_act_fn: str = "swish",
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
         cross_attention_dim=1280,
-        **kwargs,
+        dual_cross_attention=False,
+        use_linear_projection=False,
     ):
         super().__init__()
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
         resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
@@ -344,24 +356,37 @@
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
             )
         ]
         attentions = []
 
         for _ in range(num_layers):
-            attentions.append(
-                Transformer2DModel(
-                    attn_num_head_channels,
-                    in_channels // attn_num_head_channels,
-                    in_channels=in_channels,
-                    num_layers=1,
-                    cross_attention_dim=cross_attention_dim,
-                    norm_num_groups=resnet_groups,
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        in_channels // attn_num_head_channels,
+                        in_channels=in_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        in_channels // attn_num_head_channels,
+                        in_channels=in_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                    )
                 )
-            )
             resnets.append(
                 ResnetBlock2D(
                     in_channels=in_channels,
                     out_channels=in_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
@@ -373,23 +398,25 @@
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
@@ -458,15 +485,15 @@
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
         if add_downsample:
             self.downsamplers = nn.ModuleList(
                 [
                     Downsample2D(
-                        in_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
                     )
                 ]
             )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states, temb=None):
@@ -501,14 +528,17 @@
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         downsample_padding=1,
         add_downsample=True,
+        dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -525,50 +555,66 @@
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
                 )
             )
-            attentions.append(
-                Transformer2DModel(
-                    attn_num_head_channels,
-                    out_channels // attn_num_head_channels,
-                    in_channels=out_channels,
-                    num_layers=1,
-                    cross_attention_dim=cross_attention_dim,
-                    norm_num_groups=resnet_groups,
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                    )
                 )
-            )
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
         if add_downsample:
             self.downsamplers = nn.ModuleList(
                 [
                     Downsample2D(
-                        in_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
                     )
                 ]
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
@@ -647,15 +693,15 @@
 
         self.resnets = nn.ModuleList(resnets)
 
         if add_downsample:
             self.downsamplers = nn.ModuleList(
                 [
                     Downsample2D(
-                        in_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
                     )
                 ]
             )
         else:
             self.downsamplers = None
 
         self.gradient_checkpointing = False
@@ -725,15 +771,15 @@
 
         self.resnets = nn.ModuleList(resnets)
 
         if add_downsample:
             self.downsamplers = nn.ModuleList(
                 [
                     Downsample2D(
-                        in_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
                     )
                 ]
             )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states):
@@ -797,15 +843,15 @@
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
         if add_downsample:
             self.downsamplers = nn.ModuleList(
                 [
                     Downsample2D(
-                        in_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
                     )
                 ]
             )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states):
@@ -882,15 +928,15 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 down=True,
                 kernel="fir",
             )
-            self.downsamplers = nn.ModuleList([FirDownsample2D(in_channels, out_channels=out_channels)])
+            self.downsamplers = nn.ModuleList([FirDownsample2D(out_channels, out_channels=out_channels)])
             self.skip_conv = nn.Conv2d(3, out_channels, kernel_size=(1, 1), stride=(1, 1))
         else:
             self.resnet_down = None
             self.downsamplers = None
             self.skip_conv = None
 
     def forward(self, hidden_states, temb=None, skip_sample=None):
@@ -962,15 +1008,15 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 down=True,
                 kernel="fir",
             )
-            self.downsamplers = nn.ModuleList([FirDownsample2D(in_channels, out_channels=out_channels)])
+            self.downsamplers = nn.ModuleList([FirDownsample2D(out_channels, out_channels=out_channels)])
             self.skip_conv = nn.Conv2d(3, out_channels, kernel_size=(1, 1), stride=(1, 1))
         else:
             self.resnet_down = None
             self.downsamplers = None
             self.skip_conv = None
 
     def forward(self, hidden_states, temb=None, skip_sample=None):
@@ -1085,14 +1131,17 @@
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         add_upsample=True,
+        dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -1111,44 +1160,60 @@
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
                 )
             )
-            attentions.append(
-                Transformer2DModel(
-                    attn_num_head_channels,
-                    out_channels // attn_num_head_channels,
-                    in_channels=out_channels,
-                    num_layers=1,
-                    cross_attention_dim=cross_attention_dim,
-                    norm_num_groups=resnet_groups,
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                    )
                 )
-            )
         self.attentions = nn.ModuleList(attentions)
         self.resnets = nn.ModuleList(resnets)
 
         if add_upsample:
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_blocks_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_blocks_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_condition.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_condition.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     UNet2DConditionModel is a conditional 2D UNet model that takes in a noisy sample, conditional state, and a timestep
     and returns sample shaped output.
 
     This model inherits from [`ModelMixin`]. Check the superclass documentation for the generic methods the library
     implements for all the models (such as downloading or saving, etc.)
 
     Parameters:
-        sample_size (`int`, *optional*): The size of the input sample.
+        sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
+            Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 4): The number of channels in the input sample.
         out_channels (`int`, *optional*, defaults to 4): The number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
         flip_sin_to_cos (`bool`, *optional*, defaults to `False`):
             Whether to flip the sin to cos in the time embedding.
         freq_shift (`int`, *optional*, defaults to 0): The frequency shift to apply to the time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to `("CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "DownBlock2D")`):
@@ -93,23 +94,27 @@
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
+        dual_cross_attention: bool = False,
+        use_linear_projection: bool = False,
+        num_class_embeds: Optional[int] = None,
     ):
         super().__init__()
 
         self.sample_size = sample_size
         time_embed_dim = block_out_channels[0] * 4
 
         # input
@@ -117,18 +122,28 @@
 
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
 
@@ -139,37 +154,44 @@
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
+                dual_cross_attention=dual_cross_attention,
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
+            dual_cross_attention=dual_cross_attention,
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
@@ -189,34 +211,39 @@
                 prev_output_channel=prev_output_channel,
                 temb_channels=time_embed_dim,
                 add_upsample=add_upsample,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=reversed_attention_head_dim[i],
+                dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
         self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0], num_groups=norm_num_groups, eps=norm_eps)
         self.conv_act = nn.SiLU()
-        self.conv_out = nn.Conv2d(block_out_channels[0], out_channels, 3, padding=1)
+        self.conv_out = nn.Conv2d(block_out_channels[0], out_channels, kernel_size=3, padding=1)
 
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
@@ -241,14 +268,15 @@
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
             encoder_hidden_states (`torch.FloatTensor`): (batch, channel, height, width) encoder hidden states
@@ -293,14 +321,20 @@
 
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/unet_2d_condition_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/unet_2d_condition_flax.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,17 @@
         timesteps,
         encoder_hidden_states,
         return_dict: bool = True,
         train: bool = False,
     ) -> Union[FlaxUNet2DConditionOutput, Tuple]:
         r"""
         Args:
-            sample (`jnp.ndarray`): (channel, height, width) noisy inputs tensor
+            sample (`jnp.ndarray`): (batch, channel, height, width) noisy inputs tensor
             timestep (`jnp.ndarray` or `float` or `int`): timesteps
-            encoder_hidden_states (`jnp.ndarray`): (channel, height, width) encoder hidden states
+            encoder_hidden_states (`jnp.ndarray`): (batch_size, sequence_length, hidden_size) encoder hidden states
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`models.unet_2d_condition_flax.FlaxUNet2DConditionOutput`] instead of a
                 plain tuple.
             train (`bool`, *optional*, defaults to `False`):
                 Use deterministic functions and disable dropout when not training.
 
         Returns:
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/vae.py` & `diffusers-unchained-0.9.0/src/diffusers/models/vae.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/models/vae_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/models/vae_flax.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/onnx_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/onnx_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,30 +20,45 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 
 from huggingface_hub import hf_hub_download
 
-from .utils import ONNX_WEIGHTS_NAME, is_onnx_available, logging
+from .utils import ONNX_EXTERNAL_WEIGHTS_NAME, ONNX_WEIGHTS_NAME, is_onnx_available, logging
 
 
 if is_onnx_available():
     import onnxruntime as ort
 
 
 logger = logging.get_logger(__name__)
 
+ORT_TO_NP_TYPE = {
+    "tensor(bool)": np.bool_,
+    "tensor(int8)": np.int8,
+    "tensor(uint8)": np.uint8,
+    "tensor(int16)": np.int16,
+    "tensor(uint16)": np.uint16,
+    "tensor(int32)": np.int32,
+    "tensor(uint32)": np.uint32,
+    "tensor(int64)": np.int64,
+    "tensor(uint64)": np.uint64,
+    "tensor(float16)": np.float16,
+    "tensor(float)": np.float32,
+    "tensor(double)": np.float64,
+}
+
 
 class OnnxRuntimeModel:
     def __init__(self, model=None, **kwargs):
         logger.info("`diffusers.OnnxRuntimeModel` is experimental and might change in the future.")
         self.model = model
         self.model_save_dir = kwargs.get("model_save_dir", None)
-        self.latest_model_name = kwargs.get("latest_model_name", "model.onnx")
+        self.latest_model_name = kwargs.get("latest_model_name", ONNX_WEIGHTS_NAME)
 
     def __call__(self, **kwargs):
         inputs = {k: np.array(v) for k, v in kwargs.items()}
         return self.model.run(None, inputs)
 
     @staticmethod
     def load_model(path: Union[str, Path], provider=None, sess_options=None):
@@ -80,14 +95,23 @@
         src_path = self.model_save_dir.joinpath(self.latest_model_name)
         dst_path = Path(save_directory).joinpath(model_file_name)
         try:
             shutil.copyfile(src_path, dst_path)
         except shutil.SameFileError:
             pass
 
+        # copy external weights (for models >2GB)
+        src_path = self.model_save_dir.joinpath(ONNX_EXTERNAL_WEIGHTS_NAME)
+        if src_path.exists():
+            dst_path = Path(save_directory).joinpath(ONNX_EXTERNAL_WEIGHTS_NAME)
+            try:
+                shutil.copyfile(src_path, dst_path)
+            except shutil.SameFileError:
+                pass
+
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         **kwargs,
     ):
         """
         Save a model to a directory, so that it can be re-loaded using the [`~OnnxModel.from_pretrained`] class
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/optimization.py` & `diffusers-unchained-0.9.0/src/diffusers/optimization.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipeline_flax_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/pipeline_flax_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,22 +43,24 @@
 
 logger = logging.get_logger(__name__)
 
 
 LOADABLE_CLASSES = {
     "diffusers": {
         "FlaxModelMixin": ["save_pretrained", "from_pretrained"],
-        "FlaxSchedulerMixin": ["save_config", "from_config"],
+        "FlaxSchedulerMixin": ["save_pretrained", "from_pretrained"],
         "FlaxDiffusionPipeline": ["save_pretrained", "from_pretrained"],
     },
     "transformers": {
         "PreTrainedTokenizer": ["save_pretrained", "from_pretrained"],
         "PreTrainedTokenizerFast": ["save_pretrained", "from_pretrained"],
         "FlaxPreTrainedModel": ["save_pretrained", "from_pretrained"],
         "FeatureExtractionMixin": ["save_pretrained", "from_pretrained"],
+        "ProcessorMixin": ["save_pretrained", "from_pretrained"],
+        "ImageProcessingMixin": ["save_pretrained", "from_pretrained"],
     },
 }
 
 ALL_IMPORTABLE_CLASSES = {}
 for library in LOADABLE_CLASSES:
     ALL_IMPORTABLE_CLASSES.update(LOADABLE_CLASSES[library])
 
@@ -168,16 +170,16 @@
             model_cls = sub_model.__class__
 
             save_method_name = None
             # search for the model's base class in LOADABLE_CLASSES
             for library_name, library_classes in LOADABLE_CLASSES.items():
                 library = importlib.import_module(library_name)
                 for base_class, save_load_methods in library_classes.items():
-                    class_candidate = getattr(library, base_class)
-                    if issubclass(model_cls, class_candidate):
+                    class_candidate = getattr(library, base_class, None)
+                    if class_candidate is not None and issubclass(model_cls, class_candidate):
                         # if we found a suitable base class in LOADABLE_CLASSES then grab its save method
                         save_method_name = save_load_methods[0]
                         break
                 if save_method_name is not None:
                     break
 
             save_method = getattr(sub_model, save_method_name)
@@ -262,41 +264,50 @@
 
         Examples:
 
         ```py
         >>> from diffusers import FlaxDiffusionPipeline
 
         >>> # Download pipeline from huggingface.co and cache.
-        >>> pipeline = FlaxDiffusionPipeline.from_pretrained("CompVis/ldm-text2im-large-256")
-
-        >>> # Download pipeline that requires an authorization token
-        >>> # For more information on access tokens, please refer to this section
-        >>> # of the documentation](https://huggingface.co/docs/hub/security-tokens)
-        >>> pipeline = FlaxDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
-
-        >>> # Download pipeline, but overwrite scheduler
-        >>> from diffusers import LMSDiscreteScheduler
-
-        >>> scheduler = LMSDiscreteScheduler.from_config("runwayml/stable-diffusion-v1-5", subfolder="scheduler")
-        >>> pipeline = FlaxDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5", scheduler=scheduler)
+        >>> # Requires to be logged in to Hugging Face hub,
+        >>> # see more in [the documentation](https://huggingface.co/docs/hub/security-tokens)
+        >>> pipeline, params = FlaxDiffusionPipeline.from_pretrained(
+        ...     "runwayml/stable-diffusion-v1-5",
+        ...     revision="bf16",
+        ...     dtype=jnp.bfloat16,
+        ... )
+
+        >>> # Download pipeline, but use a different scheduler
+        >>> from diffusers import FlaxDPMSolverMultistepScheduler
+
+        >>> model_id = "runwayml/stable-diffusion-v1-5"
+        >>> sched, sched_state = FlaxDPMSolverMultistepScheduler.from_pretrained(
+        ...     model_id,
+        ...     subfolder="scheduler",
+        ... )
+
+        >>> dpm_pipe, dpm_params = FlaxStableDiffusionPipeline.from_pretrained(
+        ...     model_id, revision="bf16", dtype=jnp.bfloat16, scheduler=dpmpp
+        ... )
+        >>> dpm_params["scheduler"] = dpmpp_state
         ```
         """
         cache_dir = kwargs.pop("cache_dir", DIFFUSERS_CACHE)
         resume_download = kwargs.pop("resume_download", False)
         proxies = kwargs.pop("proxies", None)
         local_files_only = kwargs.pop("local_files_only", False)
         use_auth_token = kwargs.pop("use_auth_token", None)
         revision = kwargs.pop("revision", None)
         from_pt = kwargs.pop("from_pt", False)
         dtype = kwargs.pop("dtype", None)
 
         # 1. Download the checkpoints and configs
         # use snapshot download here to get it working from from_pretrained
         if not os.path.isdir(pretrained_model_name_or_path):
-            config_dict = cls.get_config_dict(
+            config_dict = cls.load_config(
                 pretrained_model_name_or_path,
                 cache_dir=cache_dir,
                 resume_download=resume_download,
                 proxies=proxies,
                 local_files_only=local_files_only,
                 use_auth_token=use_auth_token,
                 revision=revision,
@@ -334,15 +345,15 @@
                 allow_patterns=allow_patterns,
                 ignore_patterns=ignore_patterns,
                 user_agent=user_agent,
             )
         else:
             cached_folder = pretrained_model_name_or_path
 
-        config_dict = cls.get_config_dict(cached_folder)
+        config_dict = cls.load_config(cached_folder)
 
         # 2. Load the pipeline class, if using custom module then load it from the hub
         # if we load from explicit class, let's use it
         if cls != FlaxDiffusionPipeline:
             pipeline_class = cls
         else:
             diffusers_module = importlib.import_module(cls.__module__.split(".")[0])
@@ -355,15 +366,15 @@
 
         # some modules can be passed directly to the init
         # in this case they are already instantiated in `kwargs`
         # extract them here
         expected_modules = set(inspect.signature(pipeline_class.__init__).parameters.keys())
         passed_class_obj = {k: kwargs.pop(k) for k in expected_modules if k in kwargs}
 
-        init_dict, _ = pipeline_class.extract_init_dict(config_dict, **kwargs)
+        init_dict, _, _ = pipeline_class.extract_init_dict(config_dict, **kwargs)
 
         init_kwargs = {}
 
         # inference_params
         params = {}
 
         # import it here to avoid circular import
@@ -383,34 +394,34 @@
             # if the model is in a pipeline module, then we load it from the pipeline
             if name in passed_class_obj:
                 # 1. check that passed_class_obj has correct parent class
                 if not is_pipeline_module:
                     library = importlib.import_module(library_name)
                     class_obj = getattr(library, class_name)
                     importable_classes = LOADABLE_CLASSES[library_name]
-                    class_candidates = {c: getattr(library, c) for c in importable_classes.keys()}
+                    class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
                     expected_class_obj = None
                     for class_name, class_candidate in class_candidates.items():
-                        if issubclass(class_obj, class_candidate):
+                        if class_candidate is not None and issubclass(class_obj, class_candidate):
                             expected_class_obj = class_candidate
 
                     if not issubclass(passed_class_obj[name].__class__, expected_class_obj):
                         raise ValueError(
                             f"{passed_class_obj[name]} is of type: {type(passed_class_obj[name])}, but should be"
                             f" {expected_class_obj}"
                         )
                 elif passed_class_obj[name] is None:
-                    logger.warn(
+                    logger.warning(
                         f"You have passed `None` for {name} to disable its functionality in {pipeline_class}. Note"
                         f" that this might lead to problems when using {pipeline_class} and is not recommended."
                     )
                     sub_model_should_be_defined = False
                 else:
-                    logger.warn(
+                    logger.warning(
                         f"You have passed a non-standard module {passed_class_obj[name]}. We cannot verify whether it"
                         " has the correct type"
                     )
 
                 # set passed class object
                 loaded_sub_model = passed_class_obj[name]
             elif is_pipeline_module:
@@ -421,20 +432,20 @@
                 class_candidates = {c: class_obj for c in importable_classes.keys()}
             else:
                 # else we just import it from the library.
                 library = importlib.import_module(library_name)
                 class_obj = import_flax_or_no_model(library, class_name)
 
                 importable_classes = LOADABLE_CLASSES[library_name]
-                class_candidates = {c: getattr(library, c) for c in importable_classes.keys()}
+                class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
             if loaded_sub_model is None and sub_model_should_be_defined:
                 load_method_name = None
                 for class_name, class_candidate in class_candidates.items():
-                    if issubclass(class_obj, class_candidate):
+                    if class_candidate is not None and issubclass(class_obj, class_candidate):
                         load_method_name = importable_classes[class_name][1]
 
                 load_method = getattr(class_obj, load_method_name)
 
                 # check if the module is in a subdirectory
                 if os.path.isdir(os.path.join(cached_folder, name)):
                     loadable_folder = os.path.join(cached_folder, name)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipeline_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/pipeline_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 import inspect
 import os
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import torch
 
 import diffusers
 import PIL
-from accelerate.utils.versions import is_torch_version
 from huggingface_hub import snapshot_download
 from packaging import version
 from PIL import Image
 from tqdm.auto import tqdm
 
 from .configuration_utils import ConfigMixin
 from .dynamic_modules_utils import get_class_from_dynamic_module
@@ -39,44 +39,52 @@
 from .utils import (
     CONFIG_NAME,
     DIFFUSERS_CACHE,
     ONNX_WEIGHTS_NAME,
     WEIGHTS_NAME,
     BaseOutput,
     deprecate,
+    is_accelerate_available,
+    is_torch_version,
     is_transformers_available,
     logging,
 )
 
 
 if is_transformers_available():
     import transformers
     from transformers import PreTrainedModel
 
 
 INDEX_FILE = "diffusion_pytorch_model.bin"
 CUSTOM_PIPELINE_FILE_NAME = "pipeline.py"
 DUMMY_MODULES_FOLDER = "diffusers.utils"
+TRANSFORMERS_DUMMY_MODULES_FOLDER = "transformers.utils"
 
 
 logger = logging.get_logger(__name__)
 
 
 LOADABLE_CLASSES = {
     "diffusers": {
         "ModelMixin": ["save_pretrained", "from_pretrained"],
-        "SchedulerMixin": ["save_config", "from_config"],
+        "SchedulerMixin": ["save_pretrained", "from_pretrained"],
         "DiffusionPipeline": ["save_pretrained", "from_pretrained"],
         "OnnxRuntimeModel": ["save_pretrained", "from_pretrained"],
     },
     "transformers": {
         "PreTrainedTokenizer": ["save_pretrained", "from_pretrained"],
         "PreTrainedTokenizerFast": ["save_pretrained", "from_pretrained"],
         "PreTrainedModel": ["save_pretrained", "from_pretrained"],
         "FeatureExtractionMixin": ["save_pretrained", "from_pretrained"],
+        "ProcessorMixin": ["save_pretrained", "from_pretrained"],
+        "ImageProcessingMixin": ["save_pretrained", "from_pretrained"],
+    },
+    "onnxruntime.training": {
+        "ORTModule": ["save_pretrained", "from_pretrained"],
     },
 }
 
 ALL_IMPORTABLE_CLASSES = {}
 for library in LOADABLE_CLASSES:
     ALL_IMPORTABLE_CLASSES.update(LOADABLE_CLASSES[library])
 
@@ -117,18 +125,21 @@
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
@@ -172,69 +183,74 @@
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
-                    class_candidate = getattr(library, base_class)
-                    if issubclass(model_cls, class_candidate):
+                    class_candidate = getattr(library, base_class, None)
+                    if class_candidate is not None and issubclass(model_cls, class_candidate):
                         # if we found a suitable base class in LOADABLE_CLASSES then grab its save method
                         save_method_name = save_load_methods[0]
                         break
                 if save_method_name is not None:
                     break
 
             save_method = getattr(sub_model, save_method_name)
             save_method(os.path.join(save_directory, pipeline_component_name))
 
     def to(self, torch_device: Optional[Union[str, torch.device]] = None):
         if torch_device is None:
             return self
 
-        module_names, _ = self.extract_init_dict(dict(self.config))
+        module_names, _, _ = self.extract_init_dict(dict(self.config))
         for name in module_names.keys():
             module = getattr(self, name)
             if isinstance(module, torch.nn.Module):
-                if module.dtype == torch.float16 and str(torch_device) in ["cpu", "mps"]:
+                if module.dtype == torch.float16 and str(torch_device) in ["cpu"]:
                     logger.warning(
-                        "Pipelines loaded with `torch_dtype=torch.float16` cannot run with `cpu` or `mps` device. It"
-                        " is not recommended to move them to `cpu` or `mps` as running them will fail. Please make"
-                        " sure to use a `cuda` device to run the pipeline in inference. due to the lack of support for"
-                        " `float16` operations on those devices in PyTorch. Please remove the"
-                        " `torch_dtype=torch.float16` argument, or use a `cuda` device to run inference."
+                        "Pipelines loaded with `torch_dtype=torch.float16` cannot run with `cpu` device. It"
+                        " is not recommended to move them to `cpu` as running them will fail. Please make"
+                        " sure to use an accelerator to run the pipeline in inference, due to the lack of"
+                        " support for`float16` operations on this device in PyTorch. Please, remove the"
+                        " `torch_dtype=torch.float16` argument, or use another device for inference."
                     )
                 module.to(torch_device)
         return self
 
     @property
     def device(self) -> torch.device:
         r"""
         Returns:
             `torch.device`: The torch device on which the pipeline is located.
         """
-        module_names, _ = self.extract_init_dict(dict(self.config))
+        module_names, _, _ = self.extract_init_dict(dict(self.config))
         for name in module_names.keys():
             module = getattr(self, name)
             if isinstance(module, torch.nn.Module):
-                if module.device == torch.device("meta"):
-                    return torch.device("cpu")
                 return module.device
         return torch.device("cpu")
 
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path: Optional[Union[str, os.PathLike]], **kwargs):
         r"""
         Instantiate a PyTorch diffusion pipeline from pre-trained pipeline weights.
@@ -298,16 +314,16 @@
 
                          It is required that the directory has a file, called `pipeline.py` that defines the custom
                          pipeline.
 
                         </Tip>
 
                 For more information on how to load and create custom pipelines, please have a look at [Loading and
-                Creating Custom
-                Pipelines](https://huggingface.co/docs/diffusers/main/en/using-diffusers/custom_pipelines)
+                Adding Custom
+                Pipelines](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipeline_overview)
 
             torch_dtype (`str` or `torch.dtype`, *optional*):
             force_download (`bool`, *optional*, defaults to `False`):
                 Whether or not to force the (re-)download of the model weights and configuration files, overriding the
                 cached versions if they exist.
             resume_download (`bool`, *optional*, defaults to `False`):
                 Whether or not to delete incompletely received files. Will attempt to resume the download if such a
@@ -372,19 +388,19 @@
         >>> pipeline = DiffusionPipeline.from_pretrained("CompVis/ldm-text2im-large-256")
 
         >>> # Download pipeline that requires an authorization token
         >>> # For more information on access tokens, please refer to this section
         >>> # of the documentation](https://huggingface.co/docs/hub/security-tokens)
         >>> pipeline = DiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 
-        >>> # Download pipeline, but overwrite scheduler
+        >>> # Use a different scheduler
         >>> from diffusers import LMSDiscreteScheduler
 
-        >>> scheduler = LMSDiscreteScheduler.from_config("runwayml/stable-diffusion-v1-5", subfolder="scheduler")
-        >>> pipeline = DiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5", scheduler=scheduler)
+        >>> scheduler = LMSDiscreteScheduler.from_config(pipeline.scheduler.config)
+        >>> pipeline.scheduler = scheduler
         ```
         """
         cache_dir = kwargs.pop("cache_dir", DIFFUSERS_CACHE)
         resume_download = kwargs.pop("resume_download", False)
         force_download = kwargs.pop("force_download", False)
         proxies = kwargs.pop("proxies", None)
         local_files_only = kwargs.pop("local_files_only", False)
@@ -393,14 +409,23 @@
         torch_dtype = kwargs.pop("torch_dtype", None)
         custom_pipeline = kwargs.pop("custom_pipeline", None)
         provider = kwargs.pop("provider", None)
         sess_options = kwargs.pop("sess_options", None)
         device_map = kwargs.pop("device_map", None)
         low_cpu_mem_usage = kwargs.pop("low_cpu_mem_usage", _LOW_CPU_MEM_USAGE_DEFAULT)
 
+        if low_cpu_mem_usage and not is_accelerate_available():
+            low_cpu_mem_usage = False
+            logger.warning(
+                "Cannot initialize model with low cpu memory usage because `accelerate` was not found in the"
+                " environment. Defaulting to `low_cpu_mem_usage=False`. It is strongly recommended to install"
+                " `accelerate` for faster and less memory-intense model loading. You can do so with: \n```\npip"
+                " install accelerate\n```\n."
+            )
+
         if device_map is not None and not is_torch_version(">=", "1.9.0"):
             raise NotImplementedError(
                 "Loading and dispatching requires torch >= 1.9.0. Please either update your PyTorch version or set"
                 " `device_map=None`."
             )
 
         if low_cpu_mem_usage is True and not is_torch_version(">=", "1.9.0"):
@@ -414,15 +439,15 @@
                 f"You cannot set `low_cpu_mem_usage` to False while using device_map={device_map} for loading and"
                 " dispatching. Please make sure to set `low_cpu_mem_usage=True`."
             )
 
         # 1. Download the checkpoints and configs
         # use snapshot download here to get it working from from_pretrained
         if not os.path.isdir(pretrained_model_name_or_path):
-            config_dict = cls.get_config_dict(
+            config_dict = cls.load_config(
                 pretrained_model_name_or_path,
                 cache_dir=cache_dir,
                 resume_download=resume_download,
                 force_download=force_download,
                 proxies=proxies,
                 local_files_only=local_files_only,
                 use_auth_token=use_auth_token,
@@ -460,21 +485,29 @@
                 allow_patterns=allow_patterns,
                 ignore_patterns=ignore_patterns,
                 user_agent=user_agent,
             )
         else:
             cached_folder = pretrained_model_name_or_path
 
-        config_dict = cls.get_config_dict(cached_folder)
+        config_dict = cls.load_config(cached_folder)
 
         # 2. Load the pipeline class, if using custom module then load it from the hub
         # if we load from explicit class, let's use it
         if custom_pipeline is not None:
+            if custom_pipeline.endswith(".py"):
+                path = Path(custom_pipeline)
+                # decompose into folder & file
+                file_name = path.name
+                custom_pipeline = path.parent.absolute()
+            else:
+                file_name = CUSTOM_PIPELINE_FILE_NAME
+
             pipeline_class = get_class_from_dynamic_module(
-                custom_pipeline, module_file=CUSTOM_PIPELINE_FILE_NAME, cache_dir=custom_pipeline
+                custom_pipeline, module_file=file_name, cache_dir=custom_pipeline
             )
         elif cls != DiffusionPipeline:
             pipeline_class = cls
         else:
             diffusers_module = importlib.import_module(cls.__module__.split(".")[0])
             pipeline_class = getattr(diffusers_module, config_dict["_class_name"])
 
@@ -496,96 +529,103 @@
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
 
-        init_dict, unused_kwargs = pipeline_class.extract_init_dict(config_dict, **kwargs)
+        init_dict, unused_kwargs, _ = pipeline_class.extract_init_dict(config_dict, **kwargs)
 
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
                 if not is_pipeline_module:
                     library = importlib.import_module(library_name)
                     class_obj = getattr(library, class_name)
                     importable_classes = LOADABLE_CLASSES[library_name]
-                    class_candidates = {c: getattr(library, c) for c in importable_classes.keys()}
+                    class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
                     expected_class_obj = None
                     for class_name, class_candidate in class_candidates.items():
-                        if issubclass(class_obj, class_candidate):
+                        if class_candidate is not None and issubclass(class_obj, class_candidate):
                             expected_class_obj = class_candidate
 
                     if not issubclass(passed_class_obj[name].__class__, expected_class_obj):
                         raise ValueError(
                             f"{passed_class_obj[name]} is of type: {type(passed_class_obj[name])}, but should be"
                             f" {expected_class_obj}"
                         )
-                elif passed_class_obj[name] is None:
-                    logger.warn(
-                        f"You have passed `None` for {name} to disable its functionality in {pipeline_class}. Note"
-                        f" that this might lead to problems when using {pipeline_class} and is not recommended."
-                    )
-                    sub_model_should_be_defined = False
                 else:
-                    logger.warn(
+                    logger.warning(
                         f"You have passed a non-standard module {passed_class_obj[name]}. We cannot verify whether it"
                         " has the correct type"
                     )
 
                 # set passed class object
                 loaded_sub_model = passed_class_obj[name]
             elif is_pipeline_module:
                 pipeline_module = getattr(pipelines, library_name)
                 class_obj = getattr(pipeline_module, class_name)
                 importable_classes = ALL_IMPORTABLE_CLASSES
                 class_candidates = {c: class_obj for c in importable_classes.keys()}
             else:
                 # else we just import it from the library.
                 library = importlib.import_module(library_name)
+
                 class_obj = getattr(library, class_name)
                 importable_classes = LOADABLE_CLASSES[library_name]
-                class_candidates = {c: getattr(library, c) for c in importable_classes.keys()}
+                class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
-            if loaded_sub_model is None and sub_model_should_be_defined:
+            if loaded_sub_model is None:
                 load_method_name = None
                 for class_name, class_candidate in class_candidates.items():
-                    if issubclass(class_obj, class_candidate):
+                    if class_candidate is not None and issubclass(class_obj, class_candidate):
                         load_method_name = importable_classes[class_name][1]
 
                 if load_method_name is None:
                     none_module = class_obj.__module__
-                    if none_module.startswith(DUMMY_MODULES_FOLDER) and "dummy" in none_module:
+                    is_dummy_path = none_module.startswith(DUMMY_MODULES_FOLDER) or none_module.startswith(
+                        TRANSFORMERS_DUMMY_MODULES_FOLDER
+                    )
+                    if is_dummy_path and "dummy" in none_module:
                         # call class_obj for nice error message of missing requirements
                         class_obj()
 
                     raise ValueError(
                         f"The component {class_obj} of {pipeline_class} cannot be loaded as it does not seem to have"
                         f" any of the loading methods defined in {ALL_IMPORTABLE_CLASSES}."
                     )
@@ -620,27 +660,37 @@
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
 
@@ -649,24 +699,26 @@
         ```py
         >>> from diffusers import (
         ...     StableDiffusionPipeline,
         ...     StableDiffusionImg2ImgPipeline,
         ...     StableDiffusionInpaintPipeline,
         ... )
 
-        >>> img2text = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
-        >>> img2img = StableDiffusionImg2ImgPipeline(**img2text.components)
-        >>> inpaint = StableDiffusionInpaintPipeline(**img2text.components)
+        >>> text2img = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+        >>> img2img = StableDiffusionImg2ImgPipeline(**text2img.components)
+        >>> inpaint = StableDiffusionInpaintPipeline(**text2img.components)
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 from ..utils import is_flax_available, is_onnx_available, is_torch_available, is_transformers_available
 
 
 if is_torch_available():
     from .dance_diffusion import DanceDiffusionPipeline
     from .ddim import DDIMPipeline
     from .ddpm import DDPMPipeline
+    from .latent_diffusion import LDMSuperResolutionPipeline
     from .latent_diffusion_uncond import LDMPipeline
     from .pndm import PNDMPipeline
     from .repaint import RePaintPipeline
     from .score_sde_ve import ScoreSdeVePipeline
     from .stochastic_karras_ve import KarrasVePipeline
 else:
     from ..utils.dummy_pt_objects import *  # noqa F403
 
 if is_torch_available() and is_transformers_available():
+    from .alt_diffusion import AltDiffusionImg2ImgPipeline, AltDiffusionPipeline
     from .latent_diffusion import LDMTextToImagePipeline
     from .stable_diffusion import (
+        CycleDiffusionPipeline,
+        StableDiffusionImageVariationPipeline,
         StableDiffusionImg2ImgPipeline,
         StableDiffusionInpaintPipeline,
         StableDiffusionInpaintPipelineLegacy,
         StableDiffusionPipeline,
+        StableDiffusionUpscalePipeline,
+    )
+    from .stable_diffusion_safe import StableDiffusionPipelineSafe
+    from .versatile_diffusion import (
+        VersatileDiffusionDualGuidedPipeline,
+        VersatileDiffusionImageVariationPipeline,
+        VersatileDiffusionPipeline,
+        VersatileDiffusionTextToImagePipeline,
     )
     from .vq_diffusion import VQDiffusionPipeline
 
 if is_transformers_available() and is_onnx_available():
     from .stable_diffusion import (
         OnnxStableDiffusionImg2ImgPipeline,
         OnnxStableDiffusionInpaintPipeline,
+        OnnxStableDiffusionInpaintPipelineLegacy,
         OnnxStableDiffusionPipeline,
         StableDiffusionOnnxPipeline,
     )
 
 if is_transformers_available() and is_flax_available():
     from .stable_diffusion import FlaxStableDiffusionPipeline
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
 
 from typing import Optional, Tuple, Union
 
 import torch
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/ddim/pipeline_ddim.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/ddim/pipeline_ddim.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
-import inspect
 from typing import Optional, Tuple, Union
 
 import torch
 
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...utils import deprecate
 
 
 class DDIMPipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
@@ -72,40 +71,53 @@
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
 
+        if generator is not None and generator.device.type != self.device.type and self.device.type != "mps":
+            message = (
+                f"The `generator` device is `{generator.device}` and does not match the pipeline "
+                f"device `{self.device}`, so the `generator` will be ignored. "
+                f'Please use `generator=torch.Generator(device="{self.device}")` instead.'
+            )
+            deprecate(
+                "generator.device == 'cpu'",
+                "0.11.0",
+                message,
+            )
+            generator = None
+
         # Sample gaussian noise to begin loop
-        image = torch.randn(
-            (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
-            generator=generator,
-        )
-        image = image.to(self.device)
+        if isinstance(self.unet.sample_size, int):
+            image_shape = (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size)
+        else:
+            image_shape = (batch_size, self.unet.in_channels, *self.unet.sample_size)
+
+        if self.device.type == "mps":
+            # randn does not work reproducibly on mps
+            image = torch.randn(image_shape, generator=generator)
+            image = image.to(self.device)
+        else:
+            image = torch.randn(image_shape, generator=generator, device=self.device)
 
         # set step values
         self.scheduler.set_timesteps(num_inference_steps)
 
-        # Ignore use_clipped_model_output if the scheduler doesn't accept this argument
-        accepts_use_clipped_model_output = "use_clipped_model_output" in set(
-            inspect.signature(self.scheduler.step).parameters.keys()
-        )
-        extra_kwargs = {}
-        if accepts_use_clipped_model_output:
-            extra_kwargs["use_clipped_model_output"] = use_clipped_model_output
-
         for t in self.progress_bar(self.scheduler.timesteps):
             # 1. predict noise model_output
             model_output = self.unet(image, t).sample
 
             # 2. predict previous mean of image x_t-1 and add variance depending on eta
             # eta corresponds to η in paper and should be between [0, 1]
             # do x_t -> x_t-1
-            image = self.scheduler.step(model_output, t, image, eta, **extra_kwargs).prev_sample
+            image = self.scheduler.step(
+                model_output, t, image, eta=eta, use_clipped_model_output=use_clipped_model_output, generator=generator
+            ).prev_sample
 
         image = (image / 2 + 0.5).clamp(0, 1)
         image = image.cpu().permute(0, 2, 3, 1).numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/ddpm/pipeline_ddpm.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/pndm/pipeline_pndm.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,92 +6,88 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
 
 from typing import Optional, Tuple, Union
 
 import torch
 
+from ...models import UNet2DModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...schedulers import PNDMScheduler
 
 
-class DDPMPipeline(DiffusionPipeline):
+class PNDMPipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Parameters:
-        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image.
+        unet (`UNet2DModel`): U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image. Can be one of
-            [`DDPMScheduler`], or [`DDIMScheduler`].
+            The `PNDMScheduler` to be used in combination with `unet` to denoise the encoded image.
     """
 
-    def __init__(self, unet, scheduler):
+    unet: UNet2DModel
+    scheduler: PNDMScheduler
+
+    def __init__(self, unet: UNet2DModel, scheduler: PNDMScheduler):
         super().__init__()
         self.register_modules(unet=unet, scheduler=scheduler)
 
     @torch.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
+        num_inference_steps: int = 50,
         generator: Optional[torch.Generator] = None,
-        num_inference_steps: int = 1000,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
-        predict_epsilon: bool = True,
         **kwargs,
     ) -> Union[ImagePipelineOutput, Tuple]:
         r"""
         Args:
-            batch_size (`int`, *optional*, defaults to 1):
-                The number of images to generate.
-            generator (`torch.Generator`, *optional*):
-                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
-                deterministic.
-            num_inference_steps (`int`, *optional*, defaults to 1000):
+            batch_size (`int`, `optional`, defaults to 1): The number of images to generate.
+            num_inference_steps (`int`, `optional`, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
+            generator (`torch.Generator`, `optional`): A [torch
+                generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
+                deterministic.
+            output_type (`str`, `optional`, defaults to `"pil"`): The output format of the generate image. Choose
+                between [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, `optional`, defaults to `True`): Whether or not to return a
+                [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
+        # For more information on the sampling method you can take a look at Algorithm 2 of
+        # the official paper: https://arxiv.org/pdf/2202.09778.pdf
 
         # Sample gaussian noise to begin loop
         image = torch.randn(
             (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
             generator=generator,
         )
         image = image.to(self.device)
 
-        # set step values
         self.scheduler.set_timesteps(num_inference_steps)
-
         for t in self.progress_bar(self.scheduler.timesteps):
-            # 1. predict noise model_output
             model_output = self.unet(image, t).sample
 
-            # 2. compute previous image: x_t -> x_t-1
-            image = self.scheduler.step(
-                model_output, t, image, generator=generator, predict_epsilon=predict_epsilon
-            ).prev_sample
+            image = self.scheduler.step(model_output, t, image).prev_sample
 
         image = (image / 2 + 0.5).clamp(0, 1)
         image = image.cpu().permute(0, 2, 3, 1).numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.utils.checkpoint
 
@@ -28,50 +42,51 @@
         bert ([`LDMBertModel`]):
             Text-encoder model based on [BERT](https://huggingface.co/docs/transformers/model_doc/bert) architecture.
         tokenizer (`transformers.BertTokenizer`):
             Tokenizer of class
             [BertTokenizer](https://huggingface.co/docs/transformers/model_doc/bert#transformers.BertTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
     """
 
     def __init__(
         self,
         vqvae: Union[VQModel, AutoencoderKL],
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
@@ -88,14 +103,17 @@
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,101 @@
-import inspect
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Optional, Tuple, Union
 
 import torch
 
-from ...models import UNet2DModel, VQModel
+from ...models import UNet2DModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
-from ...schedulers import DDIMScheduler
+from ...schedulers import ScoreSdeVeScheduler
 
 
-class LDMPipeline(DiffusionPipeline):
+class ScoreSdeVePipeline(DiffusionPipeline):
     r"""
+    Parameters:
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
-
-    Parameters:
-        vqvae ([`VQModel`]):
-            Vector-quantized (VQ) Model to encode and decode images to and from latent representations.
-        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image latents.
-        scheduler ([`SchedulerMixin`]):
-            [`DDIMScheduler`] is to be used in combination with `unet` to denoise the encoded image latens.
+        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image. scheduler ([`SchedulerMixin`]):
+            The [`ScoreSdeVeScheduler`] scheduler to be used in combination with `unet` to denoise the encoded image.
     """
+    unet: UNet2DModel
+    scheduler: ScoreSdeVeScheduler
 
-    def __init__(self, vqvae: VQModel, unet: UNet2DModel, scheduler: DDIMScheduler):
+    def __init__(self, unet: UNet2DModel, scheduler: DiffusionPipeline):
         super().__init__()
-        self.register_modules(vqvae=vqvae, unet=unet, scheduler=scheduler)
+        self.register_modules(unet=unet, scheduler=scheduler)
 
     @torch.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
+        num_inference_steps: int = 2000,
         generator: Optional[torch.Generator] = None,
-        eta: float = 0.0,
-        num_inference_steps: int = 50,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
-    ) -> Union[Tuple, ImagePipelineOutput]:
+    ) -> Union[ImagePipelineOutput, Tuple]:
         r"""
         Args:
             batch_size (`int`, *optional*, defaults to 1):
-                Number of images to generate.
+                The number of images to generate.
             generator (`torch.Generator`, *optional*):
                 A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
                 deterministic.
-            num_inference_steps (`int`, *optional*, defaults to 50):
-                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
 
-        latents = torch.randn(
-            (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
-            generator=generator,
-        )
-        latents = latents.to(self.device)
+        img_size = self.unet.config.sample_size
+        shape = (batch_size, 3, img_size, img_size)
+
+        model = self.unet
 
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        sample = torch.randn(*shape, generator=generator) * self.scheduler.init_noise_sigma
+        sample = sample.to(self.device)
 
         self.scheduler.set_timesteps(num_inference_steps)
+        self.scheduler.set_sigmas(num_inference_steps)
+
+        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
+            sigma_t = self.scheduler.sigmas[i] * torch.ones(shape[0], device=self.device)
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+            # correction step
+            for _ in range(self.scheduler.config.correct_steps):
+                model_output = self.unet(sample, sigma_t).sample
+                sample = self.scheduler.step_correct(model_output, sample, generator=generator).prev_sample
 
-        extra_kwargs = {}
-        if accepts_eta:
-            extra_kwargs["eta"] = eta
-
-        for t in self.progress_bar(self.scheduler.timesteps):
-            latent_model_input = self.scheduler.scale_model_input(latents, t)
-            # predict the noise residual
-            noise_prediction = self.unet(latent_model_input, t).sample
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_prediction, t, latents, **extra_kwargs).prev_sample
+            # prediction step
+            model_output = model(sample, sigma_t).sample
+            output = self.scheduler.step_pred(model_output, t, sample, generator=generator)
 
-        # decode the image latents with the VAE
-        image = self.vqvae.decode(latents).sample
+            sample, sample_mean = output.prev_sample, output.prev_sample_mean
 
-        image = (image / 2 + 0.5).clamp(0, 1)
-        image = image.cpu().permute(0, 2, 3, 1).numpy()
+        sample = sample_mean.clamp(0, 1)
+        sample = sample.cpu().permute(0, 2, 3, 1).numpy()
         if output_type == "pil":
-            image = self.numpy_to_pil(image)
+            sample = self.numpy_to_pil(sample)
 
         if not return_dict:
-            return (image,)
+            return (sample,)
 
-        return ImagePipelineOutput(images=image)
+        return ImagePipelineOutput(images=sample)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/pndm/pipeline_pndm.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,89 +6,103 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
-
+import inspect
 from typing import Optional, Tuple, Union
 
 import torch
 
-from ...models import UNet2DModel
+from ...models import UNet2DModel, VQModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
-from ...schedulers import PNDMScheduler
+from ...schedulers import DDIMScheduler
 
 
-class PNDMPipeline(DiffusionPipeline):
+class LDMPipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Parameters:
-        unet (`UNet2DModel`): U-Net architecture to denoise the encoded image latents.
+        vqvae ([`VQModel`]):
+            Vector-quantized (VQ) Model to encode and decode images to and from latent representations.
+        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            The `PNDMScheduler` to be used in combination with `unet` to denoise the encoded image.
+            [`DDIMScheduler`] is to be used in combination with `unet` to denoise the encoded image latents.
     """
 
-    unet: UNet2DModel
-    scheduler: PNDMScheduler
-
-    def __init__(self, unet: UNet2DModel, scheduler: PNDMScheduler):
+    def __init__(self, vqvae: VQModel, unet: UNet2DModel, scheduler: DDIMScheduler):
         super().__init__()
-        self.register_modules(unet=unet, scheduler=scheduler)
+        self.register_modules(vqvae=vqvae, unet=unet, scheduler=scheduler)
 
     @torch.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
-        num_inference_steps: int = 50,
         generator: Optional[torch.Generator] = None,
+        eta: float = 0.0,
+        num_inference_steps: int = 50,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
-    ) -> Union[ImagePipelineOutput, Tuple]:
+    ) -> Union[Tuple, ImagePipelineOutput]:
         r"""
         Args:
-            batch_size (`int`, `optional`, defaults to 1): The number of images to generate.
-            num_inference_steps (`int`, `optional`, defaults to 50):
+            batch_size (`int`, *optional*, defaults to 1):
+                Number of images to generate.
+            generator (`torch.Generator`, *optional*):
+                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
+                deterministic.
+            num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
-            generator (`torch.Generator`, `optional`): A [torch
-                generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
-                deterministic.
-            output_type (`str`, `optional`, defaults to `"pil"`): The output format of the generate image. Choose
-                between [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, `optional`, defaults to `True`): Whether or not to return a
-                [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
+            output_type (`str`, *optional*, defaults to `"pil"`):
+                The output format of the generate image. Choose between
+                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, *optional*, defaults to `True`):
+                Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        # For more information on the sampling method you can take a look at Algorithm 2 of
-        # the official paper: https://arxiv.org/pdf/2202.09778.pdf
 
-        # Sample gaussian noise to begin loop
-        image = torch.randn(
+        latents = torch.randn(
             (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
             generator=generator,
         )
-        image = image.to(self.device)
+        latents = latents.to(self.device)
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
 
         self.scheduler.set_timesteps(num_inference_steps)
+
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+
+        extra_kwargs = {}
+        if accepts_eta:
+            extra_kwargs["eta"] = eta
+
         for t in self.progress_bar(self.scheduler.timesteps):
-            model_output = self.unet(image, t).sample
+            latent_model_input = self.scheduler.scale_model_input(latents, t)
+            # predict the noise residual
+            noise_prediction = self.unet(latent_model_input, t).sample
+            # compute the previous noisy sample x_t -> x_t-1
+            latents = self.scheduler.step(noise_prediction, t, latents, **extra_kwargs).prev_sample
 
-            image = self.scheduler.step(model_output, t, image).prev_sample
+        # decode the image latents with the VAE
+        image = self.vqvae.decode(latents).sample
 
         image = (image / 2 + 0.5).clamp(0, 1)
         image = image.cpu().permute(0, 2, 3, 1).numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/repaint/pipeline_repaint.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/repaint/pipeline_repaint.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 from typing import List, Optional, Union
 
 import numpy as np
 
 import PIL
 from PIL import Image
 
-from ...utils import BaseOutput, is_flax_available, is_onnx_available, is_torch_available, is_transformers_available
+from ...utils import (
+    BaseOutput,
+    is_flax_available,
+    is_onnx_available,
+    is_torch_available,
+    is_transformers_available,
+    is_transformers_version,
+)
 
 
 @dataclass
 class StableDiffusionPipelineOutput(BaseOutput):
     """
     Output class for Stable Diffusion pipelines.
 
@@ -24,24 +31,32 @@
     """
 
     images: Union[List[PIL.Image.Image], np.ndarray]
     nsfw_content_detected: Optional[List[bool]]
 
 
 if is_transformers_available() and is_torch_available():
+    from .pipeline_cycle_diffusion import CycleDiffusionPipeline
     from .pipeline_stable_diffusion import StableDiffusionPipeline
     from .pipeline_stable_diffusion_img2img import StableDiffusionImg2ImgPipeline
     from .pipeline_stable_diffusion_inpaint import StableDiffusionInpaintPipeline
     from .pipeline_stable_diffusion_inpaint_legacy import StableDiffusionInpaintPipelineLegacy
+    from .pipeline_stable_diffusion_upscale import StableDiffusionUpscalePipeline
     from .safety_checker import StableDiffusionSafetyChecker
 
+if is_transformers_available() and is_torch_available() and is_transformers_version(">=", "4.25.0.dev0"):
+    from .pipeline_stable_diffusion_image_variation import StableDiffusionImageVariationPipeline
+else:
+    from ...utils.dummy_torch_and_transformers_objects import StableDiffusionImageVariationPipeline
+
 if is_transformers_available() and is_onnx_available():
     from .pipeline_onnx_stable_diffusion import OnnxStableDiffusionPipeline, StableDiffusionOnnxPipeline
     from .pipeline_onnx_stable_diffusion_img2img import OnnxStableDiffusionImg2ImgPipeline
     from .pipeline_onnx_stable_diffusion_inpaint import OnnxStableDiffusionInpaintPipeline
+    from .pipeline_onnx_stable_diffusion_inpaint_legacy import OnnxStableDiffusionInpaintPipelineLegacy
 
 if is_transformers_available() and is_flax_available():
     import flax
 
     @flax.struct.dataclass
     class FlaxStableDiffusionPipelineOutput(BaseOutput):
         """
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,45 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import warnings
 from functools import partial
 from typing import Dict, List, Optional, Union
 
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
-from ...schedulers import FlaxDDIMScheduler, FlaxLMSDiscreteScheduler, FlaxPNDMScheduler
-from ...utils import logging
+from ...schedulers import (
+    FlaxDDIMScheduler,
+    FlaxDPMSolverMultistepScheduler,
+    FlaxLMSDiscreteScheduler,
+    FlaxPNDMScheduler,
+)
+from ...utils import deprecate, logging
 from . import FlaxStableDiffusionPipelineOutput
 from .safety_checker_flax import FlaxStableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
@@ -38,56 +58,81 @@
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.FlaxCLIPTextModel),
             specifically the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`FlaxUNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`FlaxDDIMScheduler`], [`FlaxLMSDiscreteScheduler`], or [`FlaxPNDMScheduler`].
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`FlaxDDIMScheduler`], [`FlaxLMSDiscreteScheduler`], [`FlaxPNDMScheduler`], or
+            [`FlaxDPMSolverMultistepScheduler`].
         safety_checker ([`FlaxStableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
 
     def __init__(
         self,
         vae: FlaxAutoencoderKL,
         text_encoder: FlaxCLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: FlaxUNet2DConditionModel,
-        scheduler: Union[FlaxDDIMScheduler, FlaxPNDMScheduler, FlaxLMSDiscreteScheduler],
+        scheduler: Union[
+            FlaxDDIMScheduler, FlaxPNDMScheduler, FlaxLMSDiscreteScheduler, FlaxDPMSolverMultistepScheduler
+        ],
         safety_checker: FlaxStableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
         dtype: jnp.dtype = jnp.float32,
     ):
         super().__init__()
         self.dtype = dtype
 
         if safety_checker is None:
-            logger.warn(
+            logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
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
@@ -134,38 +179,52 @@
 
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
+        neg_prompt_ids: jnp.array = None,
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
         # implement this conditional `do_classifier_free_guidance = guidance_scale > 1.0`
         batch_size = prompt_ids.shape[0]
 
         max_length = prompt_ids.shape[-1]
-        uncond_input = self.tokenizer(
-            [""] * batch_size, padding="max_length", max_length=max_length, return_tensors="np"
-        )
-        uncond_embeddings = self.text_encoder(uncond_input.input_ids, params=params["text_encoder"])[0]
+
+        if neg_prompt_ids is None:
+            uncond_input = self.tokenizer(
+                [""] * batch_size, padding="max_length", max_length=max_length, return_tensors="np"
+            ).input_ids
+        else:
+            uncond_input = neg_prompt_ids
+        uncond_embeddings = self.text_encoder(uncond_input, params=params["text_encoder"])[0]
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
@@ -218,32 +277,33 @@
 
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
+        neg_prompt_ids: jnp.array = None,
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
@@ -270,21 +330,44 @@
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
-                self, prompt_ids, params, prng_seed, num_inference_steps, height, width, guidance_scale, latents, debug
+                self,
+                prompt_ids,
+                params,
+                prng_seed,
+                num_inference_steps,
+                height,
+                width,
+                guidance_scale,
+                latents,
+                debug,
+                neg_prompt_ids,
             )
         else:
             images = self._generate(
-                prompt_ids, params, prng_seed, num_inference_steps, height, width, guidance_scale, latents, debug
+                prompt_ids,
+                params,
+                prng_seed,
+                num_inference_steps,
+                height,
+                width,
+                guidance_scale,
+                latents,
+                debug,
+                neg_prompt_ids,
             )
 
         if self.safety_checker is not None:
             safety_params = params["safety_checker"]
             images_uint8_casted = (images * 255).round().astype("uint8")
             num_devices, batch_size = images.shape[:2]
 
@@ -307,18 +390,37 @@
 
         return FlaxStableDiffusionPipelineOutput(images=images, nsfw_content_detected=has_nsfw_concept)
 
 
 # TODO: maybe use a config dict instead of so many static argnums
 @partial(jax.pmap, static_broadcasted_argnums=(0, 4, 5, 6, 7, 9))
 def _p_generate(
-    pipe, prompt_ids, params, prng_seed, num_inference_steps, height, width, guidance_scale, latents, debug
+    pipe,
+    prompt_ids,
+    params,
+    prng_seed,
+    num_inference_steps,
+    height,
+    width,
+    guidance_scale,
+    latents,
+    debug,
+    neg_prompt_ids,
 ):
     return pipe._generate(
-        prompt_ids, params, prng_seed, num_inference_steps, height, width, guidance_scale, latents, debug
+        prompt_ids,
+        params,
+        prng_seed,
+        num_inference_steps,
+        height,
+        width,
+        guidance_scale,
+        latents,
+        debug,
+        neg_prompt_ids,
     )
 
 
 @partial(jax.pmap, static_broadcasted_argnums=(0,))
 def _p_get_has_nsfw_concepts(pipe, features, params):
     return pipe._get_has_nsfw_concepts(features, params)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_ve_flax.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,280 +1,276 @@
-import inspect
-from typing import Callable, List, Optional, Union
+# Copyright 2022 Google Brain and The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+# DISCLAIMER: This file is strongly influenced by https://github.com/yang-song/score_sde_pytorch
+
+from dataclasses import dataclass
+from typing import Optional, Tuple, Union
+
+import flax
+import jax.numpy as jnp
+from jax import random
+
+from ..configuration_utils import ConfigMixin, register_to_config
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
+
+
+@dataclass
+class FlaxSdeVeOutput(FlaxSchedulerOutput):
+    """
+    Output class for the ScoreSdeVeScheduler's step function output.
+
+    Args:
+        state (`ScoreSdeVeSchedulerState`):
+        prev_sample (`jnp.ndarray` of shape `(batch_size, num_channels, height, width)` for images):
+            Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
+            denoising loop.
+        prev_sample_mean (`jnp.ndarray` of shape `(batch_size, num_channels, height, width)` for images):
+            Mean averaged `prev_sample`. Same as `prev_sample`, only mean-averaged over previous timesteps.
+    """
+
+    state: ScoreSdeVeSchedulerState
+    prev_sample: jnp.ndarray
+    prev_sample_mean: Optional[jnp.ndarray] = None
+
+
+class FlaxScoreSdeVeScheduler(FlaxSchedulerMixin, ConfigMixin):
+    """
+    The variance exploding stochastic differential equation (SDE) scheduler.
+
+    For more information, see the original paper: https://arxiv.org/abs/2011.13456
+
+    [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
+    function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
+
+    Args:
+        num_train_timesteps (`int`): number of diffusion steps used to train the model.
+        snr (`float`):
+            coefficient weighting the step from the model_output sample (from the network) to the random noise.
+        sigma_min (`float`):
+                initial noise scale for sigma sequence in sampling procedure. The minimum sigma should mirror the
+                distribution of the data.
+        sigma_max (`float`): maximum value used for the range of continuous timesteps passed into the model.
+        sampling_eps (`float`): the end value of sampling, where timesteps decrease progressively from 1 to
+        epsilon.
+        correct_steps (`int`): number of correction steps performed on a produced sample.
+    """
+
+    @property
+    def has_state(self):
+        return True
 
-import numpy as np
-
-from transformers import CLIPFeatureExtractor, CLIPTokenizer
-
-from ...configuration_utils import FrozenDict
-from ...onnx_utils import OnnxRuntimeModel
-from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
+    @register_to_config
+    def __init__(
+        self,
+        num_train_timesteps: int = 2000,
+        snr: float = 0.15,
+        sigma_min: float = 0.01,
+        sigma_max: float = 1348.0,
+        sampling_eps: float = 1e-5,
+        correct_steps: int = 1,
+    ):
+        pass
 
+    def create_state(self):
+        state = ScoreSdeVeSchedulerState.create()
+        return self.set_sigmas(
+            state,
+            self.config.num_train_timesteps,
+            self.config.sigma_min,
+            self.config.sigma_max,
+            self.config.sampling_eps,
+        )
 
-logger = logging.get_logger(__name__)
+    def set_timesteps(
+        self, state: ScoreSdeVeSchedulerState, num_inference_steps: int, shape: Tuple = (), sampling_eps: float = None
+    ) -> ScoreSdeVeSchedulerState:
+        """
+        Sets the continuous timesteps used for the diffusion chain. Supporting function to be run before inference.
+
+        Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            num_inference_steps (`int`):
+                the number of diffusion steps used when generating samples with a pre-trained model.
+            sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
 
+        """
+        sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
 
-class OnnxStableDiffusionPipeline(DiffusionPipeline):
-    vae_decoder: OnnxRuntimeModel
-    text_encoder: OnnxRuntimeModel
-    tokenizer: CLIPTokenizer
-    unet: OnnxRuntimeModel
-    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
-    safety_checker: OnnxRuntimeModel
-    feature_extractor: CLIPFeatureExtractor
+        timesteps = jnp.linspace(1, sampling_eps, num_inference_steps)
+        return state.replace(timesteps=timesteps)
 
-    def __init__(
+    def set_sigmas(
         self,
-        vae_encoder: OnnxRuntimeModel,
-        vae_decoder: OnnxRuntimeModel,
-        text_encoder: OnnxRuntimeModel,
-        tokenizer: CLIPTokenizer,
-        unet: OnnxRuntimeModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
-        safety_checker: OnnxRuntimeModel,
-        feature_extractor: CLIPFeatureExtractor,
-    ):
-        super().__init__()
+        state: ScoreSdeVeSchedulerState,
+        num_inference_steps: int,
+        sigma_min: float = None,
+        sigma_max: float = None,
+        sampling_eps: float = None,
+    ) -> ScoreSdeVeSchedulerState:
+        """
+        Sets the noise scales used for the diffusion chain. Supporting function to be run before inference.
+
+        The sigmas control the weight of the `drift` and `diffusion` components of sample update.
+
+        Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            num_inference_steps (`int`):
+                the number of diffusion steps used when generating samples with a pre-trained model.
+            sigma_min (`float`, optional):
+                initial noise scale value (overrides value given at Scheduler instantiation).
+            sigma_max (`float`, optional): final noise scale value (overrides value given at Scheduler instantiation).
+            sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
+        """
+        sigma_min = sigma_min if sigma_min is not None else self.config.sigma_min
+        sigma_max = sigma_max if sigma_max is not None else self.config.sigma_max
+        sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
+        if state.timesteps is None:
+            state = self.set_timesteps(state, num_inference_steps, sampling_eps)
+
+        discrete_sigmas = jnp.exp(jnp.linspace(jnp.log(sigma_min), jnp.log(sigma_max), num_inference_steps))
+        sigmas = jnp.array([sigma_min * (sigma_max / sigma_min) ** t for t in state.timesteps])
 
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
-                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
-                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
-                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
-                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
-            )
-            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["clip_sample"] = False
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        self.register_modules(
-            vae_encoder=vae_encoder,
-            vae_decoder=vae_decoder,
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
-            unet=unet,
-            scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
-        )
+        return state.replace(discrete_sigmas=discrete_sigmas, sigmas=sigmas)
+
+    def get_adjacent_sigma(self, state, timesteps, t):
+        return jnp.where(timesteps == 0, jnp.zeros_like(t), state.discrete_sigmas[timesteps - 1])
 
-    def __call__(
+    def step_pred(
         self,
-        prompt: Union[str, List[str]],
-        height: Optional[int] = 512,
-        width: Optional[int] = 512,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
-        num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
-        generator: Optional[np.random.RandomState] = None,
-        latents: Optional[np.ndarray] = None,
-        output_type: Optional[str] = "pil",
+        state: ScoreSdeVeSchedulerState,
+        model_output: jnp.ndarray,
+        timestep: int,
+        sample: jnp.ndarray,
+        key: random.KeyArray,
         return_dict: bool = True,
-        callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
-        callback_steps: Optional[int] = 1,
-        **kwargs,
-    ):
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
-
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
+    ) -> Union[FlaxSdeVeOutput, Tuple]:
+        """
+        Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
+        process from the learned model outputs (most often the predicted noise).
+
+        Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            model_output (`jnp.ndarray`): direct output from learned diffusion model.
+            timestep (`int`): current discrete timestep in the diffusion chain.
+            sample (`jnp.ndarray`):
+                current instance of sample being created by diffusion process.
+            generator: random number generator.
+            return_dict (`bool`): option for returning tuple rather than FlaxSdeVeOutput class
+
+        Returns:
+            [`FlaxSdeVeOutput`] or `tuple`: [`FlaxSdeVeOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            returning a tuple, the first element is the sample tensor.
+
+        """
+        if state.timesteps is None:
             raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
+                "`state.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
-        if generator is None:
-            generator = np.random
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
+        timestep = timestep * jnp.ones(
+            sample.shape[0],
         )
-        text_input_ids = text_inputs.input_ids
+        timesteps = (timestep * (len(state.timesteps) - 1)).long()
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
-        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
-
-        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-        # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""] * batch_size
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int32))[0]
-            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+        sigma = state.discrete_sigmas[timesteps]
+        adjacent_sigma = self.get_adjacent_sigma(state, timesteps, timestep)
+        drift = jnp.zeros_like(sample)
+        diffusion = (sigma**2 - adjacent_sigma**2) ** 0.5
+
+        # equation 6 in the paper: the model_output modeled by the network is grad_x log pt(x)
+        # also equation 47 shows the analog from SDE models to ancestral sampling methods
+        diffusion = diffusion.flatten()
+        diffusion = broadcast_to_shape_from_left(diffusion, sample.shape)
+        drift = drift - diffusion**2 * model_output
+
+        #  equation 6: sample noise for the diffusion term of
+        key = random.split(key, num=1)
+        noise = random.normal(key=key, shape=sample.shape)
+        prev_sample_mean = sample - drift  # subtract because `dt` is a small negative timestep
+        # TODO is the variable diffusion the correct scaling term for the noise?
+        prev_sample = prev_sample_mean + diffusion * noise  # add impact of diffusion field g
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
-
-        # get the initial random noise unless the user supplied it
-        latents_dtype = text_embeddings.dtype
-        latents_shape = (batch_size * num_images_per_prompt, 4, height // 8, width // 8)
-        if latents is None:
-            latents = generator.randn(*latents_shape).astype(latents_dtype)
-        elif latents.shape != latents_shape:
-            raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        latents = latents * self.scheduler.init_noise_sigma
-
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-
-        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(
-                sample=latent_model_input, timestep=np.array([t]), encoder_hidden_states=text_embeddings
-            )
-            noise_pred = noise_pred[0]
+        if not return_dict:
+            return (prev_sample, prev_sample_mean, state)
 
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
-                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-            latents = np.array(latents)
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
-
-        latents = 1 / 0.18215 * latents
-        # image = self.vae_decoder(latent_sample=latents)[0]
-        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
-        image = np.concatenate(
-            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
-        )
+        return FlaxSdeVeOutput(prev_sample=prev_sample, prev_sample_mean=prev_sample_mean, state=state)
 
-        image = np.clip(image / 2 + 0.5, 0, 1)
-        image = image.transpose((0, 2, 3, 1))
+    def step_correct(
+        self,
+        state: ScoreSdeVeSchedulerState,
+        model_output: jnp.ndarray,
+        sample: jnp.ndarray,
+        key: random.KeyArray,
+        return_dict: bool = True,
+    ) -> Union[FlaxSdeVeOutput, Tuple]:
+        """
+        Correct the predicted sample based on the output model_output of the network. This is often run repeatedly
+        after making the prediction for the previous timestep.
+
+        Args:
+            state (`ScoreSdeVeSchedulerState`): the `FlaxScoreSdeVeScheduler` state data class instance.
+            model_output (`jnp.ndarray`): direct output from learned diffusion model.
+            sample (`jnp.ndarray`):
+                current instance of sample being created by diffusion process.
+            generator: random number generator.
+            return_dict (`bool`): option for returning tuple rather than FlaxSdeVeOutput class
+
+        Returns:
+            [`FlaxSdeVeOutput`] or `tuple`: [`FlaxSdeVeOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            returning a tuple, the first element is the sample tensor.
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="np"
-            ).pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
-            images, has_nsfw_concept = [], []
-            for i in range(image.shape[0]):
-                image_i, has_nsfw_concept_i = self.safety_checker(
-                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
-                )
-                images.append(image_i)
-                has_nsfw_concept.append(has_nsfw_concept_i[0])
-            image = np.concatenate(images)
-        else:
-            has_nsfw_concept = None
+        """
+        if state.timesteps is None:
+            raise ValueError(
+                "`state.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
+            )
 
-        if output_type == "pil":
-            image = self.numpy_to_pil(image)
+        # For small batch sizes, the paper "suggest replacing norm(z) with sqrt(d), where d is the dim. of z"
+        # sample noise for correction
+        key = random.split(key, num=1)
+        noise = random.normal(key=key, shape=sample.shape)
+
+        # compute step size from the model_output, the noise, and the snr
+        grad_norm = jnp.linalg.norm(model_output)
+        noise_norm = jnp.linalg.norm(noise)
+        step_size = (self.config.snr * noise_norm / grad_norm) ** 2 * 2
+        step_size = step_size * jnp.ones(sample.shape[0])
+
+        # compute corrected sample: model_output term and noise term
+        step_size = step_size.flatten()
+        step_size = broadcast_to_shape_from_left(step_size, sample.shape)
+        prev_sample_mean = sample + step_size * model_output
+        prev_sample = prev_sample_mean + ((step_size * 2) ** 0.5) * noise
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (prev_sample, state)
 
-        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+        return FlaxSdeVeOutput(prev_sample=prev_sample, state=state)
 
-
-class StableDiffusionOnnxPipeline(OnnxStableDiffusionPipeline):
-    def __init__(
-        self,
-        vae_decoder: OnnxRuntimeModel,
-        text_encoder: OnnxRuntimeModel,
-        tokenizer: CLIPTokenizer,
-        unet: OnnxRuntimeModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
-        safety_checker: OnnxRuntimeModel,
-        feature_extractor: CLIPFeatureExtractor,
-    ):
-        deprecation_message = "Please use `OnnxStableDiffusionPipeline` instead of `StableDiffusionOnnxPipeline`."
-        deprecate("StableDiffusionOnnxPipeline", "1.0.0", deprecation_message)
-        super().__init__(
-            vae_decoder=vae_decoder,
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
-            unet=unet,
-            scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
-        )
+    def __len__(self):
+        return self.config.num_train_timesteps
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from transformers import CLIPFeatureExtractor, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
-from ...onnx_utils import OnnxRuntimeModel
+from ...onnx_utils import ORT_TO_NP_TYPE, OnnxRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
+from ...utils import PIL_INTERPOLATION, deprecate, logging
 from . import StableDiffusionPipelineOutput
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 def preprocess(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=PIL.Image.LANCZOS)
+    image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     return 2.0 * image - 1.0
 
 
 class OnnxStableDiffusionImg2ImgPipeline(DiffusionPipeline):
     r"""
@@ -42,15 +56,15 @@
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
@@ -59,24 +73,27 @@
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
@@ -99,34 +116,119 @@
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
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int32))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
 
     def __call__(
         self,
         prompt: Union[str, List[str]],
         init_image: Union[np.ndarray, PIL.Image.Image],
         strength: float = 0.8,
         num_inference_steps: Optional[int] = 50,
@@ -218,74 +320,22 @@
 
         # set timesteps
         self.scheduler.set_timesteps(num_inference_steps)
 
         if isinstance(init_image, PIL.Image.Image):
             init_image = preprocess(init_image)
 
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
-
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError("The length of `negative_prompt` should be equal to batch_size.")
-            else:
-                uncond_tokens = negative_prompt
 
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(input_ids=uncond_input_ids.astype(np.int32))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
         latents_dtype = text_embeddings.dtype
         init_image = init_image.astype(latents_dtype)
         # encode the init image into latents and scale the latents
         init_latents = self.vae_encoder(sample=init_image)[0]
         init_latents = 0.18215 * init_latents
 
@@ -334,32 +384,41 @@
             extra_step_kwargs["eta"] = eta
 
         latents = init_latents
 
         t_start = max(num_inference_steps - init_timestep + offset, 0)
         timesteps = self.scheduler.timesteps[t_start:].numpy()
 
+        timestep_dtype = next(
+            (input.type for input in self.unet.model.get_inputs() if input.name == "timestep"), "tensor(float)"
+        )
+        timestep_dtype = ORT_TO_NP_TYPE[timestep_dtype]
+
         for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
             latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
+            latent_model_input = self.scheduler.scale_model_input(torch.from_numpy(latent_model_input), t)
+            latent_model_input = latent_model_input.cpu().numpy()
 
             # predict the noise residual
+            timestep = np.array([t], dtype=timestep_dtype)
             noise_pred = self.unet(
-                sample=latent_model_input, timestep=np.array([t]), encoder_hidden_states=text_embeddings
+                sample=latent_model_input, timestep=timestep, encoder_hidden_states=text_embeddings
             )[0]
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-            latents = latents.numpy()
+            scheduler_output = self.scheduler.step(
+                torch.from_numpy(noise_pred), t, torch.from_numpy(latents), **extra_step_kwargs
+            )
+            latents = scheduler_output.prev_sample.numpy()
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
         latents = 1 / 0.18215 * latents
         # image = self.vae_decoder(latent_sample=latents)[0]
@@ -371,15 +430,15 @@
         image = np.clip(image / 2 + 0.5, 0, 1)
         image = image.transpose((0, 2, 3, 1))
 
         if self.safety_checker is not None:
             safety_checker_input = self.feature_extractor(
                 self.numpy_to_pil(image), return_tensors="np"
             ).pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
+            # safety_checker does not support batched inputs yet
             images, has_nsfw_concept = [], []
             for i in range(image.shape[0]):
                 image_i, has_nsfw_concept_i = self.safety_checker(
                     clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
                 )
                 images.append(image_i)
                 has_nsfw_concept.append(has_nsfw_concept_i[0])
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
 from transformers import CLIPFeatureExtractor, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
-from ...onnx_utils import OnnxRuntimeModel
+from ...onnx_utils import ORT_TO_NP_TYPE, OnnxRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
+from ...utils import PIL_INTERPOLATION, deprecate, logging
 from . import StableDiffusionPipelineOutput
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 NUM_UNET_INPUT_CHANNELS = 9
@@ -26,15 +40,15 @@
     image = np.array(image.convert("RGB").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
     image = image[None].transpose(0, 3, 1, 2)
     image = image.astype(np.float32) / 127.5 - 1.0
 
     image_mask = np.array(mask.convert("L").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
     masked_image = image * (image_mask < 127.5)
 
-    mask = mask.resize((latents_shape[1], latents_shape[0]), PIL.Image.NEAREST)
+    mask = mask.resize((latents_shape[1], latents_shape[0]), PIL_INTERPOLATION["nearest"])
     mask = np.array(mask.convert("L"))
     mask = mask.astype(np.float32) / 255.0
     mask = mask[None, None]
     mask[mask < 0.5] = 0
     mask[mask >= 0.5] = 1
 
     return mask, masked_image
@@ -55,15 +69,15 @@
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
@@ -72,24 +86,27 @@
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
@@ -113,43 +130,128 @@
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
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int32))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
 
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
@@ -216,14 +318,15 @@
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
 
@@ -240,78 +343,22 @@
 
         if generator is None:
             generator = np.random
 
         # set timesteps
         self.scheduler.set_timesteps(num_inference_steps)
 
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
-
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(input_ids=uncond_input_ids.astype(np.int32))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
         num_channels_latents = NUM_LATENT_CHANNELS
         latents_shape = (batch_size * num_images_per_prompt, num_channels_latents, height // 8, width // 8)
         latents_dtype = text_embeddings.dtype
         if latents is None:
             latents = generator.randn(*latents_shape).astype(latents_dtype)
         else:
@@ -348,46 +395,54 @@
                 " `pipeline.unet` or your `mask_image` or `image` input."
             )
 
         # set timesteps
         self.scheduler.set_timesteps(num_inference_steps)
 
         # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        latents = latents * np.float(self.scheduler.init_noise_sigma)
 
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
         accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_step_kwargs = {}
         if accepts_eta:
             extra_step_kwargs["eta"] = eta
 
+        timestep_dtype = next(
+            (input.type for input in self.unet.model.get_inputs() if input.name == "timestep"), "tensor(float)"
+        )
+        timestep_dtype = ORT_TO_NP_TYPE[timestep_dtype]
+
         for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
             # expand the latents if we are doing classifier free guidance
             latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
             # concat latents, mask, masked_image_latnets in the channel dimension
-            latent_model_input = np.concatenate([latent_model_input, mask, masked_image_latents], axis=1)
             latent_model_input = self.scheduler.scale_model_input(torch.from_numpy(latent_model_input), t)
-            latent_model_input = latent_model_input.numpy()
+            latent_model_input = latent_model_input.cpu().numpy()
+            latent_model_input = np.concatenate([latent_model_input, mask, masked_image_latents], axis=1)
 
             # predict the noise residual
+            timestep = np.array([t], dtype=timestep_dtype)
             noise_pred = self.unet(
-                sample=latent_model_input, timestep=np.array([t]), encoder_hidden_states=text_embeddings
+                sample=latent_model_input, timestep=timestep, encoder_hidden_states=text_embeddings
             )[0]
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-            latents = latents.numpy()
+            scheduler_output = self.scheduler.step(
+                torch.from_numpy(noise_pred), t, torch.from_numpy(latents), **extra_step_kwargs
+            )
+            latents = scheduler_output.prev_sample.numpy()
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
         latents = 1 / 0.18215 * latents
         # image = self.vae_decoder(latent_sample=latents)[0]
@@ -399,15 +454,15 @@
         image = np.clip(image / 2 + 0.5, 0, 1)
         image = image.transpose((0, 2, 3, 1))
 
         if self.safety_checker is not None:
             safety_checker_input = self.feature_extractor(
                 self.numpy_to_pil(image), return_tensors="np"
             ).pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
+            # safety_checker does not support batched inputs yet
             images, has_nsfw_concept = [], []
             for i in range(image.shape[0]):
                 image_i, has_nsfw_concept_i = self.safety_checker(
                     clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
                 )
                 images.append(image_i)
                 has_nsfw_concept.append(has_nsfw_concept_i[0])
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 import inspect
 from typing import Callable, List, Optional, Union
 
+import numpy as np
 import torch
 
-from diffusers.utils import is_accelerate_available
-from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+import PIL
+from packaging import version
+from transformers import CLIPFeatureExtractor, CLIPTokenizer
 
 from ...configuration_utils import FrozenDict
-from ...models import AutoencoderKL, UNet2DConditionModel
+from ...onnx_utils import OnnxRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import (
-    DDIMScheduler,
-    EulerAncestralDiscreteScheduler,
-    EulerDiscreteScheduler,
-    LMSDiscreteScheduler,
-    PNDMScheduler,
-)
+from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
 from ...utils import deprecate, logging
 from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-class StableDiffusionPipeline(DiffusionPipeline):
+def preprocess(image):
+    w, h = image.size
+    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
+    image = image.resize((w, h), resample=PIL.Image.LANCZOS)
+    image = np.array(image).astype(np.float32) / 255.0
+    image = image[None].transpose(0, 3, 1, 2)
+    return 2.0 * image - 1.0
+
+
+def preprocess_mask(mask, scale_factor=8):
+    mask = mask.convert("L")
+    w, h = mask.size
+    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
+    mask = mask.resize((w // scale_factor, h // scale_factor), resample=PIL.Image.NEAREST)
+    mask = np.array(mask).astype(np.float32) / 255.0
+    mask = np.tile(mask, (4, 1, 1))
+    mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
+    mask = 1 - mask  # repaint white, keep black
+    return mask
+
+
+class OnnxStableDiffusionInpaintPipelineLegacy(DiffusionPipeline):
     r"""
-    Pipeline for text-to-image generation using Stable Diffusion.
+    Pipeline for text-guided image inpainting using Stable Diffusion. This is a *legacy feature* for Onnx pipelines to
+    provide compatibility with StableDiffusionInpaintPipelineLegacy and may be removed in the future.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
@@ -39,34 +56,42 @@
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    vae_encoder: OnnxRuntimeModel
+    vae_decoder: OnnxRuntimeModel
+    text_encoder: OnnxRuntimeModel
+    tokenizer: CLIPTokenizer
+    unet: OnnxRuntimeModel
+    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
+    safety_checker: OnnxRuntimeModel
+    feature_extractor: CLIPFeatureExtractor
 
     def __init__(
         self,
-        vae: AutoencoderKL,
-        text_encoder: CLIPTextModel,
+        vae_encoder: OnnxRuntimeModel,
+        vae_decoder: OnnxRuntimeModel,
+        text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
-        unet: UNet2DConditionModel,
-        scheduler: Union[
-            DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler, EulerDiscreteScheduler, EulerAncestralDiscreteScheduler
-        ],
-        safety_checker: StableDiffusionSafetyChecker,
+        unet: OnnxRuntimeModel,
+        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        safety_checker: OnnxRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
@@ -89,158 +114,208 @@
                 " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
             )
             deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["clip_sample"] = False
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
-            logger.warn(
+        if safety_checker is None and requires_safety_checker:
+            logger.warning(
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
-            vae=vae,
+            vae_encoder=vae_encoder,
+            vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
-    def enable_xformers_memory_efficient_attention(self):
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_onnx_stable_diffusion.OnnxStableDiffusionPipeline._encode_prompt
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
-        Enable memory efficient attention as implemented in xformers.
+        Encodes the prompt into text encoder hidden states.
 
-        When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
-        time. Speed up at training time is not guaranteed.
-
-        Warning: When Memory Efficient Attention and Sliced attention are both enabled, the Memory Efficient Attention
-        is used.
-        """
-        self.unet.set_use_memory_efficient_attention_xformers(True)
-
-    def disable_xformers_memory_efficient_attention(self):
-        r"""
-        Disable memory efficient attention as implemented in xformers.
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
         """
-        self.unet.set_use_memory_efficient_attention_xformers(False)
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
 
-    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
-        r"""
-        Enable sliced attention computation.
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
 
-        When this option is enabled, the attention module will split the input tensor in slices, to compute attention
-        in several steps. This is useful to save some memory in exchange for a small speed decrease.
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
 
-        Args:
-            slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
-                When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
-                a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
-                `attention_head_dim` must be a multiple of `slice_size`.
-        """
-        if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
-        self.unet.set_attention_slice(slice_size)
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
 
-    def disable_attention_slicing(self):
-        r"""
-        Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
-        back to computing attention in one step.
-        """
-        # set slice_size = `None` to disable `attention slicing`
-        self.enable_attention_slicing(None)
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
 
-    def enable_sequential_cpu_offload(self):
-        r"""
-        Offloads all models to CPU using accelerate, significantly reducing memory usage. When called, unet,
-        text_encoder, vae and safety checker have their state dicts saved to CPU and then are moved to a
-        `torch.device('meta') and loaded to GPU only when their specific submodule has its `forward` method called.
-        """
-        if is_accelerate_available():
-            from accelerate import cpu_offload
-        else:
-            raise ImportError("Please install accelerate via `pip install accelerate`")
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int32))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
 
-        device = torch.device("cuda")
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
 
-        for cpu_offloaded_model in [self.unet, self.text_encoder, self.vae, self.safety_checker]:
-            if cpu_offloaded_model is not None:
-                cpu_offload(cpu_offloaded_model, device)
+        return text_embeddings
 
-    @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
-        num_inference_steps: int = 50,
-        guidance_scale: float = 7.5,
+        init_image: Union[np.ndarray, PIL.Image.Image],
+        mask_image: Union[np.ndarray, PIL.Image.Image],
+        strength: float = 0.8,
+        num_inference_steps: Optional[int] = 50,
+        guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
-        eta: float = 0.0,
-        generator: Optional[torch.Generator] = None,
-        latents: Optional[torch.FloatTensor] = None,
+        eta: Optional[float] = 0.0,
+        generator: Optional[np.random.RandomState] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
-        callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
+        callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
         callback_steps: Optional[int] = 1,
         **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
-                The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
-                The width in pixels of the generated image.
+            init_image (`nd.ndarray` or `PIL.Image.Image`):
+                `Image`, or tensor representing an image batch, that will be used as the starting point for the
+                process. This is the image whose masked region will be inpainted.
+            mask_image (`nd.ndarray` or `PIL.Image.Image`):
+                `Image`, or tensor representing an image batch, to mask `init_image`. White pixels in the mask will be
+                replaced by noise and therefore repainted, while black pixels will be preserved. If `mask_image` is a
+                PIL image, it will be converted to a single channel (luminance) before use. If it's a tensor, it should
+                contain one color channel (L) instead of 3, so the expected shape would be `(B, H, W, 1)`.uu
+            strength (`float`, *optional*, defaults to 0.8):
+                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
+                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
+                number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
+                noise will be maximum and the denoising process will run for the full number of iterations specified in
+                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference.
+                expense of slower inference. This parameter will be modulated by `strength`.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
                 1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
                 usually at the expense of lower image quality.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
-                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                Corresponds to parameter eta (?) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            generator (`torch.Generator`, *optional*):
-                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
-                deterministic.
-            latents (`torch.FloatTensor`, *optional*):
-                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
-                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                tensor will ge generated by sampling using the supplied random `generator`.
+            generator (`np.random.RandomState`, *optional*):
+                A np.random.RandomState to make generation deterministic.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
+                called with the following arguments: `callback(step: int, timestep: int, latents: np.ndarray)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
 
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
@@ -251,172 +326,150 @@
         if isinstance(prompt, str):
             batch_size = 1
         elif isinstance(prompt, list):
             batch_size = len(prompt)
         else:
             raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
 
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+        if strength < 0 or strength > 1:
+            raise ValueError(f"The value of strength should in [0.0, 1.0] but is {strength}")
 
         if (callback_steps is None) or (
             callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
         ):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pt",
-        )
-        text_input_ids = text_inputs.input_ids
+        if generator is None:
+            generator = np.random
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
+        # set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
 
-        # duplicate text embeddings for each generation per prompt, using mps friendly method
-        bs_embed, seq_len, _ = text_embeddings.shape
-        text_embeddings = text_embeddings.repeat(1, num_images_per_prompt, 1)
-        text_embeddings = text_embeddings.view(bs_embed * num_images_per_prompt, seq_len, -1)
+        if isinstance(init_image, PIL.Image.Image):
+            init_image = preprocess(init_image)
 
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""] * batch_size
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pt",
-            )
-            uncond_embeddings = self.text_encoder(uncond_input.input_ids.to(self.device))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.repeat(1, num_images_per_prompt, 1)
-            uncond_embeddings = uncond_embeddings.view(batch_size * num_images_per_prompt, seq_len, -1)
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = torch.cat([uncond_embeddings, text_embeddings])
-
-        # get the initial random noise unless the user supplied it
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        latents_shape = (batch_size * num_images_per_prompt, self.unet.in_channels, height // 8, width // 8)
         latents_dtype = text_embeddings.dtype
-        if latents is None:
-            if self.device.type == "mps":
-                # randn does not work reproducibly on mps
-                latents = torch.randn(latents_shape, generator=generator, device="cpu", dtype=latents_dtype).to(
-                    self.device
-                )
-            else:
-                latents = torch.randn(latents_shape, generator=generator, device=self.device, dtype=latents_dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-            latents = latents.to(self.device)
+        init_image = init_image.astype(latents_dtype)
 
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps.to(self.device)
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        # encode the init image into latents and scale the latents
+        init_latents = self.vae_encoder(sample=init_image)[0]
+        init_latents = 0.18215 * init_latents
+
+        # Expand init_latents for batch_size and num_images_per_prompt
+        init_latents = np.concatenate([init_latents] * num_images_per_prompt, axis=0)
+        init_latents_orig = init_latents
+
+        # preprocess mask
+        if not isinstance(mask_image, np.ndarray):
+            mask_image = preprocess_mask(mask_image, self.vae_scale_factor)
+        mask_image = mask_image.astype(latents_dtype)
+        mask = np.concatenate([mask_image] * num_images_per_prompt, axis=0)
+
+        # check sizes
+        if not mask.shape == init_latents.shape:
+            raise ValueError("The mask and init_image should be the same size!")
+
+        # get the original timestep using init_timestep
+        offset = self.scheduler.config.get("steps_offset", 0)
+        init_timestep = int(num_inference_steps * strength) + offset
+        init_timestep = min(init_timestep, num_inference_steps)
+
+        timesteps = self.scheduler.timesteps.numpy()[-init_timestep]
+        timesteps = np.array([timesteps] * batch_size * num_images_per_prompt)
+
+        # add noise to latents using the timesteps
+        noise = generator.randn(*init_latents.shape).astype(latents_dtype)
+        init_latents = self.scheduler.add_noise(
+            torch.from_numpy(init_latents), torch.from_numpy(noise), torch.from_numpy(timesteps)
+        )
+        init_latents = init_latents.numpy()
 
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # eta (?) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to ? in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
         accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_step_kwargs = {}
         if accepts_eta:
             extra_step_kwargs["eta"] = eta
 
-        # check if the scheduler accepts generator
-        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        if accepts_generator:
-            extra_step_kwargs["generator"] = generator
+        latents = init_latents
+
+        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        timesteps = self.scheduler.timesteps[t_start:].numpy()
 
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(
+                sample=latent_model_input, timestep=np.array([t]), encoder_hidden_states=text_embeddings
+            )[0]
 
             # perform guidance
             if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
+                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
+            latents = self.scheduler.step(
+                torch.from_numpy(noise_pred), t, torch.from_numpy(latents), **extra_step_kwargs
+            ).prev_sample
+
+            latents = latents.numpy()
+
+            init_latents_proper = self.scheduler.add_noise(
+                torch.from_numpy(init_latents_orig), torch.from_numpy(noise), torch.from_numpy(np.array([t]))
+            )
+
+            init_latents_proper = init_latents_proper.numpy()
+
+            latents = (init_latents_proper * mask) + (latents * (1 - mask))
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
         latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clamp(0, 1)
+        # image = self.vae_decoder(latent_sample=latents)[0]
+        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
+        image = np.concatenate(
+            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
+        )
 
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.cpu().permute(0, 2, 3, 1).float().numpy()
+        image = np.clip(image / 2 + 0.5, 0, 1)
+        image = image.transpose((0, 2, 3, 1))
 
         if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(
-                self.device
-            )
-            image, has_nsfw_concept = self.safety_checker(
-                images=image, clip_input=safety_checker_input.pixel_values.to(text_embeddings.dtype)
-            )
+            safety_checker_input = self.feature_extractor(
+                self.numpy_to_pil(image), return_tensors="np"
+            ).pixel_values.astype(image.dtype)
+            # There will throw an error if use safety_checker batchsize>1
+            images, has_nsfw_concept = [], []
+            for i in range(image.shape[0]):
+                image_i, has_nsfw_concept_i = self.safety_checker(
+                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
+                )
+                images.append(image_i)
+                has_nsfw_concept.append(has_nsfw_concept_i[0])
+            image = np.concatenate(images)
         else:
             has_nsfw_concept = None
 
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,56 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 
 import PIL
-from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from diffusers.utils import is_accelerate_available
+from transformers import CLIPTextModel, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
-from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import (
-    DDIMScheduler,
-    EulerAncestralDiscreteScheduler,
-    EulerDiscreteScheduler,
-    LMSDiscreteScheduler,
-    PNDMScheduler,
-)
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
+from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...schedulers import DDIMScheduler, DDPMScheduler, LMSDiscreteScheduler, PNDMScheduler
+from ...utils import logging
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 def preprocess(image):
-    w, h = image.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=PIL.Image.LANCZOS)
-    image = np.array(image).astype(np.float32) / 255.0
+    # resize to multiple of 64
+    width, height = image.size
+    width = width - width % 64
+    height = height - height % 64
+    image = image.resize((width, height))
+
+    image = np.array(image.convert("RGB"))
     image = image[None].transpose(0, 3, 1, 2)
-    image = torch.from_numpy(image)
-    return 2.0 * image - 1.0
+    image = torch.from_numpy(image).to(dtype=torch.float32) / 127.5 - 1.0
+    return image
 
 
-class StableDiffusionImg2ImgPipeline(DiffusionPipeline):
+class StableDiffusionUpscalePipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image to image generation using Stable Diffusion.
+    Pipeline for text-guided image super-resolution using Stable Diffusion 2.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
@@ -49,386 +58,494 @@
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        low_res_scheduler ([`SchedulerMixin`]):
+            A scheduler used to add initial noise to the low res conditioning image. It must be an instance of
+            [`DDPMScheduler`].
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
-            Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
-            Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
-        scheduler: Union[
-            DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler, EulerDiscreteScheduler, EulerAncestralDiscreteScheduler
-        ],
-        safety_checker: StableDiffusionSafetyChecker,
-        feature_extractor: CLIPFeatureExtractor,
+        low_res_scheduler: DDPMScheduler,
+        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        max_noise_level: int = 350,
     ):
         super().__init__()
 
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
-                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
-                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
-                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
-                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
-            )
-            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["clip_sample"] = False
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
-            logger.warn(
-                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
-                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. Both the diffusers team and Hugging Face"
-                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
-                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
-                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
-            )
-
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
+            low_res_scheduler=low_res_scheduler,
             scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
         )
+        self.register_to_config(max_noise_level=max_noise_level)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
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
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
-        # set slice_size = `None` to disable `set_attention_slice`
+        # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
+    def enable_sequential_cpu_offload(self, gpu_id=0):
+        r"""
+        Offloads all models to CPU using accelerate, significantly reducing memory usage. When called, unet,
+        text_encoder, vae and safety checker have their state dicts saved to CPU and then are moved to a
+        `torch.device('meta') and loaded to GPU only when their specific submodule has its `forward` method called.
+        """
+        if is_accelerate_available():
+            from accelerate import cpu_offload
+        else:
+            raise ImportError("Please install accelerate via `pip install accelerate`")
+
+        device = torch.device(f"cuda:{gpu_id}")
+
+        for cpu_offloaded_model in [self.unet, self.text_encoder]:
+            if cpu_offloaded_model is not None:
+                cpu_offload(cpu_offloaded_model, device)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
 
         Warning: When Memory Efficient Attention and Sliced attention are both enabled, the Memory Efficient Attention
         is used.
         """
         self.unet.set_use_memory_efficient_attention_xformers(True)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_xformers_memory_efficient_attention
     def disable_xformers_memory_efficient_attention(self):
         r"""
         Disable memory efficient attention as implemented in xformers.
         """
         self.unet.set_use_memory_efficient_attention_xformers(False)
 
-    @torch.no_grad()
-    def __call__(
-        self,
-        prompt: Union[str, List[str]],
-        init_image: Union[torch.FloatTensor, PIL.Image.Image],
-        strength: float = 0.8,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
-        num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
-        generator: Optional[torch.Generator] = None,
-        output_type: Optional[str] = "pil",
-        return_dict: bool = True,
-        callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
-        callback_steps: Optional[int] = 1,
-        **kwargs,
-    ):
+    @property
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._execution_device
+    def _execution_device(self):
         r"""
-        Function invoked when calling the pipeline for generation.
+        Returns the device on which the pipeline's models will be executed. After calling
+        `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
+        hooks.
+        """
+        if self.device != torch.device("meta") or not hasattr(self.unet, "_hf_hook"):
+            return self.device
+        for module in self.unet.modules():
+            if (
+                hasattr(module, "_hf_hook")
+                and hasattr(module._hf_hook, "execution_device")
+                and module._hf_hook.execution_device is not None
+            ):
+                return torch.device(module._hf_hook.execution_device)
+        return self.device
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._encode_prompt
+    def _encode_prompt(self, prompt, device, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
 
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            init_image (`torch.FloatTensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, that will be used as the starting point for the
-                process.
-            strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
-                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
-                number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
-                noise will be maximum and the denoising process will run for the full number of iterations specified in
-                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
-            num_inference_steps (`int`, *optional*, defaults to 50):
-                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference. This parameter will be modulated by `strength`.
-            guidance_scale (`float`, *optional*, defaults to 7.5):
-                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
-                `guidance_scale` is defined as `w` of equation 2. of [Imagen
-                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
-                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
-                usually at the expense of lower image quality.
-            negative_prompt (`str` or `List[str]`, *optional*):
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            device: (`torch.device`):
+                torch device
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
-            num_images_per_prompt (`int`, *optional*, defaults to 1):
-                The number of images to generate per prompt.
-            eta (`float`, *optional*, defaults to 0.0):
-                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
-                [`schedulers.DDIMScheduler`], will be ignored for others.
-            generator (`torch.Generator`, *optional*):
-                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
-                deterministic.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
-                plain tuple.
-            callback (`Callable`, *optional*):
-                A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
-            callback_steps (`int`, *optional*, defaults to 1):
-                The frequency at which the `callback` function will be called. If not specified, the callback will be
-                called at every step.
-
-        Returns:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
-            When returning a tuple, the first element is a list with the generated images, and the second element is a
-            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
-            (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if strength < 0 or strength > 1:
-            raise ValueError(f"The value of strength should in [0.0, 1.0] but is {strength}")
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
 
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = preprocess(init_image)
-
-        # get prompt text embeddings
         text_inputs = self.tokenizer(
             prompt,
             padding="max_length",
             max_length=self.tokenizer.model_max_length,
+            truncation=True,
             return_tensors="pt",
         )
         text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="pt").input_ids
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
+        if not torch.equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
             logger.warning(
                 "The following part of your input was truncated because CLIP can only handle sequences up to"
                 f" {self.tokenizer.model_max_length} tokens: {removed_text}"
             )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
 
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = text_embeddings.repeat_interleave(num_images_per_prompt, dim=0)
+        if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
+            attention_mask = text_inputs.attention_mask.to(device)
+        else:
+            attention_mask = None
+
+        text_embeddings = self.text_encoder(
+            text_input_ids.to(device),
+            attention_mask=attention_mask,
+        )
+        text_embeddings = text_embeddings[0]
+
+        # duplicate text embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = text_embeddings.shape
+        text_embeddings = text_embeddings.repeat(1, num_images_per_prompt, 1)
+        text_embeddings = text_embeddings.view(bs_embed * num_images_per_prompt, seq_len, -1)
 
-        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-        # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
         # get unconditional embeddings for classifier free guidance
         if do_classifier_free_guidance:
             uncond_tokens: List[str]
             if negative_prompt is None:
                 uncond_tokens = [""] * batch_size
             elif type(prompt) is not type(negative_prompt):
                 raise TypeError(
                     f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
                     f" {type(prompt)}."
                 )
             elif isinstance(negative_prompt, str):
                 uncond_tokens = [negative_prompt]
             elif batch_size != len(negative_prompt):
-                raise ValueError("The length of `negative_prompt` should be equal to batch_size.")
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
             else:
                 uncond_tokens = negative_prompt
 
             max_length = text_input_ids.shape[-1]
             uncond_input = self.tokenizer(
                 uncond_tokens,
                 padding="max_length",
                 max_length=max_length,
                 truncation=True,
                 return_tensors="pt",
             )
-            uncond_embeddings = self.text_encoder(uncond_input.input_ids.to(self.device))[0]
 
-            # duplicate unconditional embeddings for each generation per prompt
+            if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
+                attention_mask = uncond_input.attention_mask.to(device)
+            else:
+                attention_mask = None
+
+            uncond_embeddings = self.text_encoder(
+                uncond_input.input_ids.to(device),
+                attention_mask=attention_mask,
+            )
+            uncond_embeddings = uncond_embeddings[0]
+
+            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
             seq_len = uncond_embeddings.shape[1]
             uncond_embeddings = uncond_embeddings.repeat(1, num_images_per_prompt, 1)
             uncond_embeddings = uncond_embeddings.view(batch_size * num_images_per_prompt, seq_len, -1)
 
             # For classifier free guidance, we need to do two forward passes.
             # Here we concatenate the unconditional and text embeddings into a single batch
             # to avoid doing two forward passes
             text_embeddings = torch.cat([uncond_embeddings, text_embeddings])
 
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.to(device=self.device, dtype=latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample(generator=generator)
-        init_latents = 0.18215 * init_latents
-
-        if isinstance(prompt, str):
-            prompt = [prompt]
-        if len(prompt) > init_latents.shape[0] and len(prompt) % init_latents.shape[0] == 0:
-            # expand init_latents for batch_size
-            deprecation_message = (
-                f"You have passed {len(prompt)} text prompts (`prompt`), but only {init_latents.shape[0]} initial"
-                " images (`init_image`). Initial images are now duplicating to match the number of text prompts. Note"
-                " that this behavior is deprecated and will be removed in a version 1.0.0. Please make sure to update"
-                " your script to pass as many init images as text prompts to suppress this warning."
-            )
-            deprecate("len(prompt) != len(init_image)", "1.0.0", deprecation_message, standard_warn=False)
-            additional_image_per_prompt = len(prompt) // init_latents.shape[0]
-            init_latents = torch.cat([init_latents] * additional_image_per_prompt * num_images_per_prompt, dim=0)
-        elif len(prompt) > init_latents.shape[0] and len(prompt) % init_latents.shape[0] != 0:
-            raise ValueError(
-                f"Cannot duplicate `init_image` of batch size {init_latents.shape[0]} to {len(prompt)} text prompts."
-            )
-        else:
-            init_latents = torch.cat([init_latents] * num_images_per_prompt, dim=0)
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
-
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = torch.tensor([timesteps] * batch_size * num_images_per_prompt, device=self.device)
-
-        # add noise to latents using the timesteps
-        noise = torch.randn(init_latents.shape, generator=generator, device=self.device, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
+        return text_embeddings
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
+
         accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_step_kwargs = {}
         if accepts_eta:
             extra_step_kwargs["eta"] = eta
 
         # check if the scheduler accepts generator
         accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
         if accepts_generator:
             extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
 
-        latents = init_latents
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents with 0.18215->0.08333
+    def decode_latents(self, latents):
+        latents = 1 / 0.08333 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clamp(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.cpu().permute(0, 2, 3, 1).float().numpy()
+        return image
 
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+    def check_inputs(self, prompt, image, noise_level, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if (
+            not isinstance(image, torch.Tensor)
+            and not isinstance(image, PIL.Image.Image)
+            and not isinstance(image, list)
+        ):
+            raise ValueError(
+                f"`image` has to be of type `torch.Tensor`, `PIL.Image.Image` or `list` but is {type(image)}"
+            )
+
+        # verify batch size of prompt and image are same if image is a list or tensor
+        if isinstance(image, list) or isinstance(image, torch.Tensor):
+            if isinstance(prompt, str):
+                batch_size = 1
+            else:
+                batch_size = len(prompt)
+            if isinstance(image, list):
+                image_batch_size = len(image)
+            else:
+                image_batch_size = image.shape[0]
+            if batch_size != image_batch_size:
+                raise ValueError(
+                    f"`prompt` has batch size {batch_size} and `image` has batch size {image_batch_size}."
+                    " Please make sure that passed `prompt` matches the batch size of `image`."
+                )
+
+        # check noise level
+        if noise_level > self.config.max_noise_level:
+            raise ValueError(f"`noise_level` has to be <= {self.config.max_noise_level} but is {noise_level}")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:].to(self.device)
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
+        shape = (batch_size, num_channels_latents, height, width)
+        if latents is None:
+            if device.type == "mps":
+                # randn does not work reproducibly on mps
+                latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
+            else:
+                latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+            latents = latents.to(device)
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
 
-        for i, t in enumerate(self.progress_bar(timesteps)):
+    @torch.no_grad()
+    def __call__(
+        self,
+        prompt: Union[str, List[str]],
+        image: Union[torch.FloatTensor, PIL.Image.Image, List[PIL.Image.Image]],
+        num_inference_steps: int = 75,
+        guidance_scale: float = 9.0,
+        noise_level: int = 20,
+        negative_prompt: Optional[Union[str, List[str]]] = None,
+        num_images_per_prompt: Optional[int] = 1,
+        eta: float = 0.0,
+        generator: Optional[torch.Generator] = None,
+        latents: Optional[torch.FloatTensor] = None,
+        output_type: Optional[str] = "pil",
+        return_dict: bool = True,
+        callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
+        callback_steps: Optional[int] = 1,
+    ):
+        r"""
+        Function invoked when calling the pipeline for generation.
+
+        Args:
+            prompt (`str` or `List[str]`):
+                The prompt or prompts to guide the image generation.
+            image (`PIL.Image.Image` or List[`PIL.Image.Image`] or `torch.FloatTensor`):
+                `Image`, or tensor representing an image batch which will be upscaled. *
+            num_inference_steps (`int`, *optional*, defaults to 50):
+                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
+                expense of slower inference.
+            guidance_scale (`float`, *optional*, defaults to 7.5):
+                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
+                `guidance_scale` is defined as `w` of equation 2. of [Imagen
+                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
+                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
+                usually at the expense of lower image quality.
+            negative_prompt (`str` or `List[str]`, *optional*):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+            num_images_per_prompt (`int`, *optional*, defaults to 1):
+                The number of images to generate per prompt.
+            eta (`float`, *optional*, defaults to 0.0):
+                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                [`schedulers.DDIMScheduler`], will be ignored for others.
+            generator (`torch.Generator`, *optional*):
+                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
+                deterministic.
+            latents (`torch.FloatTensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
+            output_type (`str`, *optional*, defaults to `"pil"`):
+                The output format of the generate image. Choose between
+                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, *optional*, defaults to `True`):
+                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
+                plain tuple.
+            callback (`Callable`, *optional*):
+                A function that will be called every `callback_steps` steps during inference. The function will be
+                called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
+            callback_steps (`int`, *optional*, defaults to 1):
+                The frequency at which the `callback` function will be called. If not specified, the callback will be
+                called at every step.
+
+        Returns:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
+            When returning a tuple, the first element is a list with the generated images, and the second element is a
+            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
+            (nsfw) content, according to the `safety_checker`.
+        """
+
+        # 1. Check inputs
+        self.check_inputs(prompt, image, noise_level, callback_steps)
+
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
+        device = self._execution_device
+        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+        # corresponds to doing no classifier free guidance.
+        do_classifier_free_guidance = guidance_scale > 1.0
+
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, device, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
+
+        # 4. Preprocess image
+        image = [image] if isinstance(image, PIL.Image.Image) else image
+        if isinstance(image, list):
+            image = [preprocess(img) for img in image]
+            image = torch.cat(image, dim=0)
+        image = image.to(dtype=text_embeddings.dtype, device=device)
+
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps, device=device)
+        timesteps_tensor = self.scheduler.timesteps
+
+        # 5. Add noise to image
+        noise_level = torch.tensor([noise_level], dtype=torch.long, device=device)
+        if device.type == "mps":
+            # randn does not work reproducibly on mps
+            noise = torch.randn(image.shape, generator=generator, device="cpu", dtype=text_embeddings.dtype).to(device)
+        else:
+            noise = torch.randn(image.shape, generator=generator, device=device, dtype=text_embeddings.dtype)
+        image = self.low_res_scheduler.add_noise(image, noise, noise_level)
+        image = torch.cat([image] * 2) if do_classifier_free_guidance else image
+        noise_level = torch.cat([noise_level] * 2) if do_classifier_free_guidance else noise_level
+
+        # 6. Prepare latent variables
+        height, width = image.shape[2:]
+        num_channels_latents = self.vae.config.latent_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            device,
+            generator,
+            latents,
+        )
+
+        # 7. Check that sizes of image and latents match
+        num_channels_image = image.shape[1]
+        if num_channels_latents + num_channels_image != self.unet.config.in_channels:
+            raise ValueError(
+                f"Incorrect configuration settings! The config of `pipeline.unet`: {self.unet.config} expects"
+                f" {self.unet.config.in_channels} but received `num_channels_latents`: {num_channels_latents} +"
+                f" `num_channels_image`: {num_channels_image} "
+                f" = {num_channels_latents+num_channels_image}. Please verify the config of"
+                " `pipeline.unet` or your `image` input."
+            )
+
+        # 8. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
+
+        # 9. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
             # expand the latents if we are doing classifier free guidance
             latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
+
+            # concat latents, mask, masked_image_latents in the channel dimension
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
+            latent_model_input = torch.cat([latent_model_input, image], dim=1)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(
+                latent_model_input, t, encoder_hidden_states=text_embeddings, class_labels=noise_level
+            ).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
             latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clamp(0, 1)
-        image = image.cpu().permute(0, 2, 3, 1).numpy()
-
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(
-                self.device
-            )
-            image, has_nsfw_concept = self.safety_checker(
-                images=image, clip_input=safety_checker_input.pixel_values.to(text_embeddings.dtype)
-            )
-        else:
-            has_nsfw_concept = None
+        # 10. Post-processing
+        # make sure the VAE is in float32 mode, as it overflows in float16
+        self.vae.to(dtype=torch.float32)
+        image = self.decode_latents(latents.float())
 
+        # 11. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (image,)
 
-        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+        return ImagePipelineOutput(images=image)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,307 +1,256 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import Callable, List, Optional, Union
 
-import numpy as np
 import torch
+import torch.utils.checkpoint
 
-import PIL
-from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from transformers import CLIPFeatureExtractor, CLIPTextModelWithProjection, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
-from ...pipeline_utils import DiffusionPipeline
+from ...models.attention import Transformer2DModel
+from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
+from ...utils import is_accelerate_available, logging
+from .modeling_text_unet import UNetFlatConditionModel
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-def prepare_mask_and_masked_image(image, mask):
-    image = np.array(image.convert("RGB"))
-    image = image[None].transpose(0, 3, 1, 2)
-    image = torch.from_numpy(image).to(dtype=torch.float32) / 127.5 - 1.0
-
-    mask = np.array(mask.convert("L"))
-    mask = mask.astype(np.float32) / 255.0
-    mask = mask[None, None]
-    mask[mask < 0.5] = 0
-    mask[mask >= 0.5] = 1
-    mask = torch.from_numpy(mask)
-
-    masked_image = image * (mask < 0.5)
-
-    return mask, masked_image
-
-
-class StableDiffusionInpaintPipeline(DiffusionPipeline):
+class VersatileDiffusionTextToImagePipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
-
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
-    Args:
-        vae ([`AutoencoderKL`]):
-            Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
-            Frozen text-encoder. Stable Diffusion uses the text portion of
-            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
-            the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
-        tokenizer (`CLIPTokenizer`):
+    Parameters:
+        vqvae ([`VQModel`]):
+            Vector-quantized (VQ) Model to encode and decode images to and from latent representations.
+        bert ([`LDMBertModel`]):
+            Text-encoder model based on [BERT](https://huggingface.co/docs/transformers/model_doc/bert) architecture.
+        tokenizer (`transformers.BertTokenizer`):
             Tokenizer of class
-            [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
+            [BertTokenizer](https://huggingface.co/docs/transformers/model_doc/bert#transformers.BertTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
-            Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
-            Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    tokenizer: CLIPTokenizer
+    image_feature_extractor: CLIPFeatureExtractor
+    text_encoder: CLIPTextModelWithProjection
+    image_unet: UNet2DConditionModel
+    text_unet: UNetFlatConditionModel
+    vae: AutoencoderKL
+    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
+
+    _optional_components = ["text_unet"]
 
     def __init__(
         self,
-        vae: AutoencoderKL,
-        text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
-        unet: UNet2DConditionModel,
+        text_encoder: CLIPTextModelWithProjection,
+        image_unet: UNet2DConditionModel,
+        text_unet: UNetFlatConditionModel,
+        vae: AutoencoderKL,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
-        safety_checker: StableDiffusionSafetyChecker,
-        feature_extractor: CLIPFeatureExtractor,
     ):
         super().__init__()
-
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if hasattr(scheduler.config, "skip_prk_steps") and scheduler.config.skip_prk_steps is False:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} has not set the configuration"
-                " `skip_prk_steps`. `skip_prk_steps` should be set to True in the configuration file. Please make"
-                " sure to update the config accordingly as not setting `skip_prk_steps` in the config might lead to"
-                " incorrect results in future versions. If you have downloaded this checkpoint from the Hugging Face"
-                " Hub, it would be very nice if you could open a Pull request for the"
-                " `scheduler/scheduler_config.json` file"
-            )
-            deprecate("skip_prk_steps not set", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["skip_prk_steps"] = True
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
-            logger.warn(
-                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
-                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. Both the diffusers team and Hugging Face"
-                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
-                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
-                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
-            )
-
         self.register_modules(
-            vae=vae,
-            text_encoder=text_encoder,
             tokenizer=tokenizer,
-            unet=unet,
+            text_encoder=text_encoder,
+            image_unet=image_unet,
+            text_unet=text_unet,
+            vae=vae,
             scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+
+        if self.text_unet is not None:
+            self._swap_unet_attention_blocks()
 
+    def _swap_unet_attention_blocks(self):
+        """
+        Swap the `Transformer2DModel` blocks between the image and text UNets
+        """
+        for name, module in self.image_unet.named_modules():
+            if isinstance(module, Transformer2DModel):
+                parent_name, index = name.rsplit(".", 1)
+                index = int(index)
+                self.image_unet.get_submodule(parent_name)[index], self.text_unet.get_submodule(parent_name)[index] = (
+                    self.text_unet.get_submodule(parent_name)[index],
+                    self.image_unet.get_submodule(parent_name)[index],
+                )
+
+    def remove_unused_weights(self):
+        self.register_modules(text_unet=None)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention with unet->image_unet
+    def enable_xformers_memory_efficient_attention(self):
+        r"""
+        Enable memory efficient attention as implemented in xformers.
+
+        When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
+        time. Speed up at training time is not guaranteed.
+
+        Warning: When Memory Efficient Attention and Sliced attention are both enabled, the Memory Efficient Attention
+        is used.
+        """
+        self.image_unet.set_use_memory_efficient_attention_xformers(True)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_xformers_memory_efficient_attention with unet->image_unet
+    def disable_xformers_memory_efficient_attention(self):
+        r"""
+        Disable memory efficient attention as implemented in xformers.
+        """
+        self.image_unet.set_use_memory_efficient_attention_xformers(False)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing with unet->image_unet
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
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
-        self.unet.set_attention_slice(slice_size)
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
 
+        self.image_unet.set_attention_slice(slice_size)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
         # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
-    def enable_xformers_memory_efficient_attention(self):
+    def enable_sequential_cpu_offload(self, gpu_id=0):
         r"""
-        Enable memory efficient attention as implemented in xformers.
+        Offloads all models to CPU using accelerate, significantly reducing memory usage. When called, unet,
+        text_encoder, vae and safety checker have their state dicts saved to CPU and then are moved to a
+        `torch.device('meta') and loaded to GPU only when their specific submodule has its `forward` method called.
+        """
+        if is_accelerate_available():
+            from accelerate import cpu_offload
+        else:
+            raise ImportError("Please install accelerate via `pip install accelerate`")
 
-        When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
-        time. Speed up at training time is not guaranteed.
+        device = torch.device(f"cuda:{gpu_id}")
 
-        Warning: When Memory Efficient Attention and Sliced attention are both enabled, the Memory Efficient Attention
-        is used.
-        """
-        self.unet.set_use_memory_efficient_attention_xformers(True)
+        for cpu_offloaded_model in [self.image_unet, self.text_unet, self.text_encoder, self.vae]:
+            if cpu_offloaded_model is not None:
+                cpu_offload(cpu_offloaded_model, device)
 
-    def disable_xformers_memory_efficient_attention(self):
+    @property
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._execution_device with unet->image_unet
+    def _execution_device(self):
         r"""
-        Disable memory efficient attention as implemented in xformers.
+        Returns the device on which the pipeline's models will be executed. After calling
+        `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
+        hooks.
         """
-        self.unet.set_use_memory_efficient_attention_xformers(False)
+        if self.device != torch.device("meta") or not hasattr(self.image_unet, "_hf_hook"):
+            return self.device
+        for module in self.image_unet.modules():
+            if (
+                hasattr(module, "_hf_hook")
+                and hasattr(module._hf_hook, "execution_device")
+                and module._hf_hook.execution_device is not None
+            ):
+                return torch.device(module._hf_hook.execution_device)
+        return self.device
 
-    @torch.no_grad()
-    def __call__(
-        self,
-        prompt: Union[str, List[str]],
-        image: Union[torch.FloatTensor, PIL.Image.Image],
-        mask_image: Union[torch.FloatTensor, PIL.Image.Image],
-        height: int = 512,
-        width: int = 512,
-        num_inference_steps: int = 50,
-        guidance_scale: float = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
-        num_images_per_prompt: Optional[int] = 1,
-        eta: float = 0.0,
-        generator: Optional[torch.Generator] = None,
-        latents: Optional[torch.FloatTensor] = None,
-        output_type: Optional[str] = "pil",
-        return_dict: bool = True,
-        callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
-        callback_steps: Optional[int] = 1,
-        **kwargs,
-    ):
+    def _encode_prompt(self, prompt, device, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
-        Function invoked when calling the pipeline for generation.
+        Encodes the prompt into text encoder hidden states.
 
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch which will be inpainted, *i.e.* parts of the image will
-                be masked out with `mask_image` and repainted according to `prompt`.
-            mask_image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
-                repainted, while black pixels will be preserved. If `mask_image` is a PIL image, it will be converted
-                to a single channel (luminance) before use. If it's a tensor, it should contain one color channel (L)
-                instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            height (`int`, *optional*, defaults to 512):
-                The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
-                The width in pixels of the generated image.
-            num_inference_steps (`int`, *optional*, defaults to 50):
-                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference.
-            guidance_scale (`float`, *optional*, defaults to 7.5):
-                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
-                `guidance_scale` is defined as `w` of equation 2. of [Imagen
-                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
-                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
-                usually at the expense of lower image quality.
-            negative_prompt (`str` or `List[str]`, *optional*):
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            device: (`torch.device`):
+                torch device
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
-            num_images_per_prompt (`int`, *optional*, defaults to 1):
-                The number of images to generate per prompt.
-            eta (`float`, *optional*, defaults to 0.0):
-                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
-                [`schedulers.DDIMScheduler`], will be ignored for others.
-            generator (`torch.Generator`, *optional*):
-                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
-                deterministic.
-            latents (`torch.FloatTensor`, *optional*):
-                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
-                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                tensor will ge generated by sampling using the supplied random `generator`.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
-                plain tuple.
-            callback (`Callable`, *optional*):
-                A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
-            callback_steps (`int`, *optional*, defaults to 1):
-                The frequency at which the `callback` function will be called. If not specified, the callback will be
-                called at every step.
-
-        Returns:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
-            When returning a tuple, the first element is a list with the generated images, and the second element is a
-            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
-            (nsfw) content, according to the `safety_checker`.
         """
 
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+        def normalize_embeddings(encoder_output):
+            embeds = self.text_encoder.text_projection(encoder_output.last_hidden_state)
+            embeds_pooled = encoder_output.text_embeds
+            embeds = embeds / torch.norm(embeds_pooled.unsqueeze(1), dim=-1, keepdim=True)
+            return embeds
 
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
 
-        # get prompt text embeddings
         text_inputs = self.tokenizer(
             prompt,
             padding="max_length",
             max_length=self.tokenizer.model_max_length,
+            truncation=True,
             return_tensors="pt",
         )
         text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="pt").input_ids
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
+        if not torch.equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
             logger.warning(
                 "The following part of your input was truncated because CLIP can only handle sequences up to"
                 f" {self.tokenizer.model_max_length} tokens: {removed_text}"
             )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
+
+        if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
+            attention_mask = text_inputs.attention_mask.to(device)
+        else:
+            attention_mask = None
+
+        text_embeddings = self.text_encoder(
+            text_input_ids.to(device),
+            attention_mask=attention_mask,
+        )
+        text_embeddings = normalize_embeddings(text_embeddings)
 
         # duplicate text embeddings for each generation per prompt, using mps friendly method
         bs_embed, seq_len, _ = text_embeddings.shape
         text_embeddings = text_embeddings.repeat(1, num_images_per_prompt, 1)
         text_embeddings = text_embeddings.view(bs_embed * num_images_per_prompt, seq_len, -1)
 
-        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-        # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
         # get unconditional embeddings for classifier free guidance
         if do_classifier_free_guidance:
             uncond_tokens: List[str]
             if negative_prompt is None:
                 uncond_tokens = [""] * batch_size
             elif type(prompt) is not type(negative_prompt):
                 raise TypeError(
@@ -323,145 +272,254 @@
             uncond_input = self.tokenizer(
                 uncond_tokens,
                 padding="max_length",
                 max_length=max_length,
                 truncation=True,
                 return_tensors="pt",
             )
-            uncond_embeddings = self.text_encoder(uncond_input.input_ids.to(self.device))[0]
+
+            if hasattr(self.text_encoder.config, "use_attention_mask") and self.text_encoder.config.use_attention_mask:
+                attention_mask = uncond_input.attention_mask.to(device)
+            else:
+                attention_mask = None
+
+            uncond_embeddings = self.text_encoder(
+                uncond_input.input_ids.to(device),
+                attention_mask=attention_mask,
+            )
+            uncond_embeddings = normalize_embeddings(uncond_embeddings)
 
             # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
             seq_len = uncond_embeddings.shape[1]
             uncond_embeddings = uncond_embeddings.repeat(1, num_images_per_prompt, 1)
             uncond_embeddings = uncond_embeddings.view(batch_size * num_images_per_prompt, seq_len, -1)
 
             # For classifier free guidance, we need to do two forward passes.
             # Here we concatenate the unconditional and text embeddings into a single batch
             # to avoid doing two forward passes
             text_embeddings = torch.cat([uncond_embeddings, text_embeddings])
 
-        # get the initial random noise unless the user supplied it
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        num_channels_latents = self.vae.config.latent_channels
-        latents_shape = (batch_size * num_images_per_prompt, num_channels_latents, height // 8, width // 8)
-        latents_dtype = text_embeddings.dtype
-        if latents is None:
-            if self.device.type == "mps":
-                # randn does not exist on mps
-                latents = torch.randn(latents_shape, generator=generator, device="cpu", dtype=latents_dtype).to(
-                    self.device
-                )
-            else:
-                latents = torch.randn(latents_shape, generator=generator, device=self.device, dtype=latents_dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-            latents = latents.to(self.device)
-
-        # prepare mask and masked_image
-        mask, masked_image = prepare_mask_and_masked_image(image, mask_image)
-        mask = mask.to(device=self.device, dtype=text_embeddings.dtype)
-        masked_image = masked_image.to(device=self.device, dtype=text_embeddings.dtype)
-
-        # resize the mask to latents shape as we concatenate the mask to the latents
-        mask = torch.nn.functional.interpolate(mask, size=(height // 8, width // 8))
-
-        # encode the mask image into latents space so we can concatenate it to the latents
-        masked_image_latents = self.vae.encode(masked_image).latent_dist.sample(generator=generator)
-        masked_image_latents = 0.18215 * masked_image_latents
-
-        # duplicate mask and masked_image_latents for each generation per prompt, using mps friendly method
-        mask = mask.repeat(batch_size * num_images_per_prompt, 1, 1, 1)
-        masked_image_latents = masked_image_latents.repeat(batch_size * num_images_per_prompt, 1, 1, 1)
-
-        mask = torch.cat([mask] * 2) if do_classifier_free_guidance else mask
-        masked_image_latents = (
-            torch.cat([masked_image_latents] * 2) if do_classifier_free_guidance else masked_image_latents
-        )
-
-        num_channels_mask = mask.shape[1]
-        num_channels_masked_image = masked_image_latents.shape[1]
-
-        if num_channels_latents + num_channels_mask + num_channels_masked_image != self.unet.config.in_channels:
-            raise ValueError(
-                f"Incorrect configuration settings! The config of `pipeline.unet`: {self.unet.config} expects"
-                f" {self.unet.config.in_channels} but received `num_channels_latents`: {num_channels_latents} +"
-                f" `num_channels_mask`: {num_channels_mask} + `num_channels_masked_image`: {num_channels_masked_image}"
-                f" = {num_channels_latents+num_channels_masked_image+num_channels_mask}. Please verify the config of"
-                " `pipeline.unet` or your `mask_image` or `image` input."
-            )
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
+        return text_embeddings
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps.to(self.device)
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clamp(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.cpu().permute(0, 2, 3, 1).float().numpy()
+        return image
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
+
         accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_step_kwargs = {}
         if accepts_eta:
             extra_step_kwargs["eta"] = eta
 
         # check if the scheduler accepts generator
         accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
         if accepts_generator:
             extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
 
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.check_inputs
+    def check_inputs(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
 
-            # concat latents, mask, masked_image_latents in the channel dimension
-            latent_model_input = torch.cat([latent_model_input, mask, masked_image_latents], dim=1)
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
 
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
+        if latents is None:
+            if device.type == "mps":
+                # randn does not work reproducibly on mps
+                latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
+            else:
+                latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+            latents = latents.to(device)
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
+    @torch.no_grad()
+    def __call__(
+        self,
+        prompt: Union[str, List[str]],
+        height: Optional[int] = None,
+        width: Optional[int] = None,
+        num_inference_steps: int = 50,
+        guidance_scale: float = 7.5,
+        negative_prompt: Optional[Union[str, List[str]]] = None,
+        num_images_per_prompt: Optional[int] = 1,
+        eta: float = 0.0,
+        generator: Optional[torch.Generator] = None,
+        latents: Optional[torch.FloatTensor] = None,
+        output_type: Optional[str] = "pil",
+        return_dict: bool = True,
+        callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
+        callback_steps: Optional[int] = 1,
+        **kwargs,
+    ):
+        r"""
+        Function invoked when calling the pipeline for generation.
+
+        Args:
+            prompt (`str` or `List[str]`):
+                The prompt or prompts to guide the image generation.
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
+                The height in pixels of the generated image.
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
+                The width in pixels of the generated image.
+            num_inference_steps (`int`, *optional*, defaults to 50):
+                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
+                expense of slower inference.
+            guidance_scale (`float`, *optional*, defaults to 7.5):
+                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
+                `guidance_scale` is defined as `w` of equation 2. of [Imagen
+                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
+                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
+                usually at the expense of lower image quality.
+            negative_prompt (`str` or `List[str]`, *optional*):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+            num_images_per_prompt (`int`, *optional*, defaults to 1):
+                The number of images to generate per prompt.
+            eta (`float`, *optional*, defaults to 0.0):
+                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                [`schedulers.DDIMScheduler`], will be ignored for others.
+            generator (`torch.Generator`, *optional*):
+                A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
+                deterministic.
+            latents (`torch.FloatTensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
+            output_type (`str`, *optional*, defaults to `"pil"`):
+                The output format of the generate image. Choose between
+                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, *optional*, defaults to `True`):
+                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
+                plain tuple.
+            callback (`Callable`, *optional*):
+                A function that will be called every `callback_steps` steps during inference. The function will be
+                called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
+            callback_steps (`int`, *optional*, defaults to 1):
+                The frequency at which the `callback` function will be called. If not specified, the callback will be
+                called at every step.
+
+        Examples:
+
+        ```py
+        >>> from diffusers import VersatileDiffusionTextToImagePipeline
+        >>> import torch
+
+        >>> pipe = VersatileDiffusionTextToImagePipeline.from_pretrained(
+        ...     "shi-labs/versatile-diffusion", torch_dtype=torch.float16
+        ... )
+        >>> pipe.remove_unused_weights()
+        >>> pipe = pipe.to("cuda")
+
+        >>> generator = torch.Generator(device="cuda").manual_seed(0)
+        >>> image = pipe("an astronaut riding on a horse on mars", generator=generator).images[0]
+        >>> image.save("./astronaut.png")
+        ```
+
+        Returns:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
+            When returning a tuple, the first element is a list with the generated images, and the second element is a
+            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
+            (nsfw) content, according to the `safety_checker`.
+        """
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
+
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(prompt, height, width, callback_steps)
+
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
+        device = self._execution_device
+        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+        # corresponds to doing no classifier free guidance.
+        do_classifier_free_guidance = guidance_scale > 1.0
+
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, device, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
+
+        # 4. Prepare timesteps
+        self.scheduler.set_timesteps(num_inference_steps, device=device)
+        timesteps = self.scheduler.timesteps
+
+        # 5. Prepare latent variables
+        num_channels_latents = self.image_unet.in_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            device,
+            generator,
+            latents,
+        )
+
+        # 6. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
+
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
+            # expand the latents if we are doing classifier free guidance
+            latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.image_unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
             latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clamp(0, 1)
-
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.cpu().permute(0, 2, 3, 1).float().numpy()
-
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(
-                self.device
-            )
-            image, has_nsfw_concept = self.safety_checker(
-                images=image, clip_input=safety_checker_input.pixel_values.to(text_embeddings.dtype)
-            )
-        else:
-            has_nsfw_concept = None
+        # 9. Post-processing
+        image = self.decode_latents(latents)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (image,)
 
-        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+        return ImagePipelineOutput(images=image)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,223 +1,387 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import inspect
 from typing import Callable, List, Optional, Union
 
-import numpy as np
 import torch
 
 import PIL
-from tqdm.auto import tqdm
-from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from diffusers.utils import is_accelerate_available
+from packaging import version
+from transformers import CLIPFeatureExtractor, CLIPVisionModelWithProjection
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
 from ...utils import deprecate, logging
 from . import StableDiffusionPipelineOutput
 from .safety_checker import StableDiffusionSafetyChecker
 
 
-logger = logging.get_logger(__name__)
-
-
-def preprocess_image(image):
-    w, h = image.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=PIL.Image.LANCZOS)
-    image = np.array(image).astype(np.float32) / 255.0
-    image = image[None].transpose(0, 3, 1, 2)
-    image = torch.from_numpy(image)
-    return 2.0 * image - 1.0
-
-
-def preprocess_mask(mask):
-    mask = mask.convert("L")
-    w, h = mask.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    mask = mask.resize((w // 8, h // 8), resample=PIL.Image.NEAREST)
-    mask = np.array(mask).astype(np.float32) / 255.0
-    mask = np.tile(mask, (4, 1, 1))
-    mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
-    mask = 1 - mask  # repaint white, keep black
-    mask = torch.from_numpy(mask)
-    return mask
+logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-class StableDiffusionInpaintPipelineLegacy(DiffusionPipeline):
+class StableDiffusionImageVariationPipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
+    Pipeline to generate variations from an input image using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
-            Frozen text-encoder. Stable Diffusion uses the text portion of
-            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
-            the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
-        tokenizer (`CLIPTokenizer`):
-            Tokenizer of class
-            [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
+        image_encoder ([`CLIPVisionModelWithProjection`]):
+            Frozen CLIP image-encoder. Stable Diffusion Image Variation uses the vision portion of
+            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPVisionModelWithProjection),
+            specifically the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
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
-        text_encoder: CLIPTextModel,
-        tokenizer: CLIPTokenizer,
+        image_encoder: CLIPVisionModelWithProjection,
         unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
 
-        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
-                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
-                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
-                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
-                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
-            )
-            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["clip_sample"] = False
-            scheduler._internal_dict = FrozenDict(new_config)
-
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
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
+            image_encoder=image_encoder,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_xformers_memory_efficient_attention
+    def enable_xformers_memory_efficient_attention(self):
+        r"""
+        Enable memory efficient attention as implemented in xformers.
+
+        When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
+        time. Speed up at training time is not guaranteed.
 
+        Warning: When Memory Efficient Attention and Sliced attention are both enabled, the Memory Efficient Attention
+        is used.
+        """
+        self.unet.set_use_memory_efficient_attention_xformers(True)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_xformers_memory_efficient_attention
+    def disable_xformers_memory_efficient_attention(self):
+        r"""
+        Disable memory efficient attention as implemented in xformers.
+        """
+        self.unet.set_use_memory_efficient_attention_xformers(False)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
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
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
-        # set slice_size = `None` to disable `set_attention_slice`
+        # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
+    def enable_sequential_cpu_offload(self, gpu_id=0):
+        r"""
+        Offloads all models to CPU using accelerate, significantly reducing memory usage. When called, unet,
+        text_encoder, vae and safety checker have their state dicts saved to CPU and then are moved to a
+        `torch.device('meta') and loaded to GPU only when their specific submodule has its `forward` method called.
+        """
+        if is_accelerate_available():
+            from accelerate import cpu_offload
+        else:
+            raise ImportError("Please install accelerate via `pip install accelerate`")
+
+        device = torch.device(f"cuda:{gpu_id}")
+
+        for cpu_offloaded_model in [self.unet, self.image_encoder, self.vae, self.safety_checker]:
+            if cpu_offloaded_model is not None:
+                cpu_offload(cpu_offloaded_model, device)
+
+    @property
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._execution_device
+    def _execution_device(self):
+        r"""
+        Returns the device on which the pipeline's models will be executed. After calling
+        `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
+        hooks.
+        """
+        if self.device != torch.device("meta") or not hasattr(self.unet, "_hf_hook"):
+            return self.device
+        for module in self.unet.modules():
+            if (
+                hasattr(module, "_hf_hook")
+                and hasattr(module._hf_hook, "execution_device")
+                and module._hf_hook.execution_device is not None
+            ):
+                return torch.device(module._hf_hook.execution_device)
+        return self.device
+
+    def _encode_image(self, image, device, num_images_per_prompt, do_classifier_free_guidance):
+        dtype = next(self.image_encoder.parameters()).dtype
+
+        if not isinstance(image, torch.Tensor):
+            image = self.feature_extractor(images=image, return_tensors="pt").pixel_values
+
+        image = image.to(device=device, dtype=dtype)
+        image_embeddings = self.image_encoder(image).image_embeds
+        image_embeddings = image_embeddings.unsqueeze(1)
+
+        # duplicate image embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = image_embeddings.shape
+        image_embeddings = image_embeddings.repeat(1, num_images_per_prompt, 1)
+        image_embeddings = image_embeddings.view(bs_embed * num_images_per_prompt, seq_len, -1)
+
+        if do_classifier_free_guidance:
+            uncond_embeddings = torch.zeros_like(image_embeddings)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            image_embeddings = torch.cat([uncond_embeddings, image_embeddings])
+
+        return image_embeddings
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.run_safety_checker
+    def run_safety_checker(self, image, device, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(device)
+            image, has_nsfw_concept = self.safety_checker(
+                images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
+            )
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clamp(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.cpu().permute(0, 2, 3, 1).float().numpy()
+        return image
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    def check_inputs(self, image, height, width, callback_steps):
+        if (
+            not isinstance(image, torch.Tensor)
+            and not isinstance(image, PIL.Image.Image)
+            and not isinstance(image, list)
+        ):
+            raise ValueError(
+                f"`image` has to be of type `torch.FloatTensor` or `PIL.Image.Image` or `list` but is {type(image)}"
+            )
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, device, generator, latents=None):
+        shape = (batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor)
+        if latents is None:
+            if device.type == "mps":
+                # randn does not work reproducibly on mps
+                latents = torch.randn(shape, generator=generator, device="cpu", dtype=dtype).to(device)
+            else:
+                latents = torch.randn(shape, generator=generator, device=device, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+            latents = latents.to(device)
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
     @torch.no_grad()
     def __call__(
         self,
-        prompt: Union[str, List[str]],
-        init_image: Union[torch.FloatTensor, PIL.Image.Image],
-        mask_image: Union[torch.FloatTensor, PIL.Image.Image],
-        strength: float = 0.8,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
+        image: Union[PIL.Image.Image, List[PIL.Image.Image], torch.FloatTensor],
+        height: Optional[int] = None,
+        width: Optional[int] = None,
+        num_inference_steps: int = 50,
+        guidance_scale: float = 7.5,
         num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
+        eta: float = 0.0,
         generator: Optional[torch.Generator] = None,
+        latents: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
         callback_steps: Optional[int] = 1,
         **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            init_image (`torch.FloatTensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, that will be used as the starting point for the
-                process. This is the image whose masked region will be inpainted.
-            mask_image (`torch.FloatTensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `init_image`. White pixels in the mask will be
-                replaced by noise and therefore repainted, while black pixels will be preserved. If `mask_image` is a
-                PIL image, it will be converted to a single channel (luminance) before use. If it's a tensor, it should
-                contain one color channel (L) instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to inpaint the masked area. Must be between 0 and 1. When `strength`
-                is 1, the denoising process will be run on the masked area for the full number of iterations specified
-                in `num_inference_steps`. `init_image` will be used as a reference for the masked area, adding more
-                noise to that region the larger the `strength`. If `strength` is 0, no inpainting will occur.
+            image (`PIL.Image.Image` or `List[PIL.Image.Image]` or `torch.FloatTensor`):
+                The image or images to guide the image generation. If you provide a tensor, it needs to comply with the
+                configuration of
+                [this](https://huggingface.co/lambdalabs/sd-image-variations-diffusers/blob/main/feature_extractor/preprocessor_config.json)
+                `CLIPFeatureExtractor`
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
+                The height in pixels of the generated image.
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
+                The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
-                The reference number of denoising steps. More denoising steps usually lead to a higher quality image at
-                the expense of slower inference. This parameter will be modulated by `strength`, as explained above.
+                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
+                expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
                 1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
                 usually at the expense of lower image quality.
-            negative_prompt (`str` or `List[str]`, *optional*):
-                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
-                if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
             generator (`torch.Generator`, *optional*):
                 A [torch generator](https://pytorch.org/docs/stable/generated/torch.Generator.html) to make generation
                 deterministic.
+            latents (`torch.FloatTensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
@@ -230,198 +394,85 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
-        if strength < 0 or strength > 1:
-            raise ValueError(f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pt",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = text_embeddings.repeat_interleave(num_images_per_prompt, dim=0)
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(image, height, width, callback_steps)
 
+        # 2. Define call parameters
+        if isinstance(image, PIL.Image.Image):
+            batch_size = 1
+        elif isinstance(image, list):
+            batch_size = len(image)
+        else:
+            batch_size = image.shape[0]
+        device = self._execution_device
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""] * batch_size
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pt",
-            )
-            uncond_embeddings = self.text_encoder(uncond_input.input_ids.to(self.device))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.repeat(1, num_images_per_prompt, 1)
-            uncond_embeddings = uncond_embeddings.view(batch_size * num_images_per_prompt, seq_len, -1)
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = torch.cat([uncond_embeddings, text_embeddings])
-
-        # preprocess image
-        if not isinstance(init_image, torch.FloatTensor):
-            init_image = preprocess_image(init_image)
-
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.to(device=self.device, dtype=latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample(generator=generator)
-        init_latents = 0.18215 * init_latents
-
-        # Expand init_latents for batch_size and num_images_per_prompt
-        init_latents = torch.cat([init_latents] * batch_size * num_images_per_prompt, dim=0)
-        init_latents_orig = init_latents
-
-        # preprocess mask
-        if not isinstance(mask_image, torch.FloatTensor):
-            mask_image = preprocess_mask(mask_image)
-        mask_image = mask_image.to(device=self.device, dtype=latents_dtype)
-        mask = torch.cat([mask_image] * batch_size * num_images_per_prompt)
-
-        # check sizes
-        if not mask.shape == init_latents.shape:
-            raise ValueError("The mask and init_image should be the same size!")
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
-
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = torch.tensor([timesteps] * batch_size * num_images_per_prompt, device=self.device)
-
-        # add noise to latents using the timesteps
-        noise = torch.randn(init_latents.shape, generator=generator, device=self.device, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 3. Encode input image
+        image_embeddings = self._encode_image(image, device, num_images_per_prompt, do_classifier_free_guidance)
 
-        # check if the scheduler accepts generator
-        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        if accepts_generator:
-            extra_step_kwargs["generator"] = generator
-
-        latents = init_latents
-
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        # 4. Prepare timesteps
+        self.scheduler.set_timesteps(num_inference_steps, device=device)
+        timesteps = self.scheduler.timesteps
+
+        # 5. Prepare latent variables
+        num_channels_latents = self.unet.in_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            image_embeddings.dtype,
+            device,
+            generator,
+            latents,
+        )
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:].to(self.device)
+        # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
-        for i, t in tqdm(enumerate(timesteps)):
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
             latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
             latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=image_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
             latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-            # masking
-            init_latents_proper = self.scheduler.add_noise(init_latents_orig, noise, torch.tensor([t]))
-
-            latents = (init_latents_proper * mask) + (latents * (1 - mask))
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clamp(0, 1)
-        image = image.cpu().permute(0, 2, 3, 1).numpy()
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pt").to(
-                self.device
-            )
-            image, has_nsfw_concept = self.safety_checker(images=image, clip_input=safety_checker_input.pixel_values)
-        else:
-            has_nsfw_concept = None
+        # 9. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, device, image_embeddings.dtype)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
         return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/safety_checker.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-import numpy as np
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import torch
 import torch.nn as nn
 
 from transformers import CLIPConfig, CLIPVisionModel, PreTrainedModel
 
 from ...utils import logging
 
@@ -12,15 +25,15 @@
 
 def cosine_distance(image_embeds, text_embeds):
     normalized_image_embeds = nn.functional.normalize(image_embeds)
     normalized_text_embeds = nn.functional.normalize(text_embeds)
     return torch.mm(normalized_image_embeds, normalized_text_embeds.t())
 
 
-class StableDiffusionSafetyChecker(PreTrainedModel):
+class SafeStableDiffusionSafetyChecker(PreTrainedModel):
     config_class = CLIPConfig
 
     _no_split_modules = ["CLIPEncoderLayer"]
 
     def __init__(self, config: CLIPConfig):
         super().__init__(config)
 
@@ -66,19 +79,14 @@
                 if result_img["concept_scores"][concept_idx] > 0:
                     result_img["bad_concepts"].append(concept_idx)
 
             result.append(result_img)
 
         has_nsfw_concepts = [len(res["bad_concepts"]) > 0 for res in result]
 
-        if any(has_nsfw_concepts):
-            logger.warning(
-                "Potential NSFW content was detected in one or more images. Please use caution."
-            )
-
         return images, has_nsfw_concepts
 
     @torch.no_grad()
     def forward_onnx(self, clip_input: torch.FloatTensor, images: torch.FloatTensor):
         pooled_output = self.vision_model(clip_input)[1]  # pooled_output
         image_embeds = self.visual_projection(pooled_output)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 from flax import linen as nn
 from flax.core.frozen_dict import FrozenDict
 from transformers import CLIPConfig, FlaxPreTrainedModel
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-#!/usr/bin/env python3
+# Copyright 2022 The HuggingFace Team. All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Optional, Tuple, Union
 
 import torch
 
 from ...models import UNet2DModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import KarrasVeScheduler
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,21 +16,45 @@
 
 import torch
 
 from diffusers import Transformer2DModel, VQModel
 from diffusers.schedulers.scheduling_vq_diffusion import VQDiffusionScheduler
 from transformers import CLIPTextModel, CLIPTokenizer
 
+from ...configuration_utils import ConfigMixin, register_to_config
+from ...modeling_utils import ModelMixin
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
+class LearnedClassifierFreeSamplingEmbeddings(ModelMixin, ConfigMixin):
+    """
+    Utility class for storing learned text embeddings for classifier free sampling
+    """
+
+    @register_to_config
+    def __init__(self, learnable: bool, hidden_size: Optional[int] = None, length: Optional[int] = None):
+        super().__init__()
+
+        self.learnable = learnable
+
+        if self.learnable:
+            assert hidden_size is not None, "learnable=True requires `hidden_size` to be set"
+            assert length is not None, "learnable=True requires `length` to be set"
+
+            embeddings = torch.zeros(length, hidden_size)
+        else:
+            embeddings = None
+
+        self.embeddings = torch.nn.Parameter(embeddings)
+
+
 class VQDiffusionPipeline(DiffusionPipeline):
     r"""
     Pipeline for text-to-image generation using VQ Diffusion
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
@@ -51,39 +75,106 @@
             A scheduler to be used in combination with `transformer` to denoise the encoded image latents.
     """
 
     vqvae: VQModel
     text_encoder: CLIPTextModel
     tokenizer: CLIPTokenizer
     transformer: Transformer2DModel
+    learned_classifier_free_sampling_embeddings: LearnedClassifierFreeSamplingEmbeddings
     scheduler: VQDiffusionScheduler
 
     def __init__(
         self,
         vqvae: VQModel,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         transformer: Transformer2DModel,
         scheduler: VQDiffusionScheduler,
+        learned_classifier_free_sampling_embeddings: LearnedClassifierFreeSamplingEmbeddings,
     ):
         super().__init__()
 
         self.register_modules(
             vqvae=vqvae,
             transformer=transformer,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             scheduler=scheduler,
+            learned_classifier_free_sampling_embeddings=learned_classifier_free_sampling_embeddings,
+        )
+
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance):
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            return_tensors="pt",
         )
+        text_input_ids = text_inputs.input_ids
+
+        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
+            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
+        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
+
+        # NOTE: This additional step of normalizing the text embeddings is from VQ-Diffusion.
+        # While CLIP does normalize the pooled output of the text transformer when combining
+        # the image and text embeddings, CLIP does not directly normalize the last hidden state.
+        #
+        # CLIP normalizing the pooled output.
+        # https://github.com/huggingface/transformers/blob/d92e22d1f28324f513f3080e5c47c071a3916721/src/transformers/models/clip/modeling_clip.py#L1052-L1053
+        text_embeddings = text_embeddings / text_embeddings.norm(dim=-1, keepdim=True)
+
+        # duplicate text embeddings for each generation per prompt
+        text_embeddings = text_embeddings.repeat_interleave(num_images_per_prompt, dim=0)
+
+        if do_classifier_free_guidance:
+            if self.learned_classifier_free_sampling_embeddings.learnable:
+                uncond_embeddings = self.learned_classifier_free_sampling_embeddings.embeddings
+                uncond_embeddings = uncond_embeddings.unsqueeze(0).repeat(batch_size, 1, 1)
+            else:
+                uncond_tokens = [""] * batch_size
+
+                max_length = text_input_ids.shape[-1]
+                uncond_input = self.tokenizer(
+                    uncond_tokens,
+                    padding="max_length",
+                    max_length=max_length,
+                    truncation=True,
+                    return_tensors="pt",
+                )
+                uncond_embeddings = self.text_encoder(uncond_input.input_ids.to(self.device))[0]
+                # See comment for normalizing text embeddings
+                uncond_embeddings = uncond_embeddings / uncond_embeddings.norm(dim=-1, keepdim=True)
+
+            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
+            seq_len = uncond_embeddings.shape[1]
+            uncond_embeddings = uncond_embeddings.repeat(1, num_images_per_prompt, 1)
+            uncond_embeddings = uncond_embeddings.view(batch_size * num_images_per_prompt, seq_len, -1)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = torch.cat([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
 
     @torch.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
         num_inference_steps: int = 100,
+        guidance_scale: float = 5.0,
         truncation_rate: float = 1.0,
         num_images_per_prompt: int = 1,
         generator: Optional[torch.Generator] = None,
         latents: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
@@ -94,14 +185,20 @@
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
             num_inference_steps (`int`, *optional*, defaults to 100):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
+            guidance_scale (`float`, *optional*, defaults to 7.5):
+                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
+                `guidance_scale` is defined as `w` of equation 2. of [Imagen
+                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
+                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
+                usually at the expense of lower image quality.
             truncation_rate (`float`, *optional*, defaults to 1.0 (equivalent to no truncation)):
                 Used to "truncate" the predicted classes for x_0 such that the cumulative probability for a pixel is at
                 most `truncation_rate`. The lowest probabilities that would increase the cumulative probability above
                 `truncation_rate` are set to zero.
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             generator (`torch.Generator`, *optional*):
@@ -133,51 +230,26 @@
         elif isinstance(prompt, list):
             batch_size = len(prompt)
         else:
             raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
 
         batch_size = batch_size * num_images_per_prompt
 
+        do_classifier_free_guidance = guidance_scale > 1.0
+
+        text_embeddings = self._encode_prompt(prompt, num_images_per_prompt, do_classifier_free_guidance)
+
         if (callback_steps is None) or (
             callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
         ):
             raise ValueError(
                 f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
                 f" {type(callback_steps)}."
             )
 
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pt",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(text_input_ids.to(self.device))[0]
-
-        # NOTE: This additional step of normalizing the text embeddings is from VQ-Diffusion.
-        # While CLIP does normalize the pooled output of the text transformer when combining
-        # the image and text embeddings, CLIP does not directly normalize the last hidden state.
-        #
-        # CLIP normalizing the pooled output.
-        # https://github.com/huggingface/transformers/blob/d92e22d1f28324f513f3080e5c47c071a3916721/src/transformers/models/clip/modeling_clip.py#L1052-L1053
-        text_embeddings = text_embeddings / text_embeddings.norm(dim=-1, keepdim=True)
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = text_embeddings.repeat_interleave(num_images_per_prompt, dim=0)
-
         # get the initial completely masked latents unless the user supplied it
 
         latents_shape = (batch_size, self.transformer.num_latent_pixels)
         if latents is None:
             mask_class = self.transformer.num_vector_embeds - 1
             latents = torch.full(latents_shape, mask_class).to(self.device)
         else:
@@ -194,17 +266,27 @@
         self.scheduler.set_timesteps(num_inference_steps, device=self.device)
 
         timesteps_tensor = self.scheduler.timesteps.to(self.device)
 
         sample = latents
 
         for i, t in enumerate(self.progress_bar(timesteps_tensor)):
+            # expand the sample if we are doing classifier free guidance
+            latent_model_input = torch.cat([sample] * 2) if do_classifier_free_guidance else sample
+
             # predict the un-noised image
             # model_output == `log_p_x_0`
-            model_output = self.transformer(sample, encoder_hidden_states=text_embeddings, timestep=t).sample
+            model_output = self.transformer(
+                latent_model_input, encoder_hidden_states=text_embeddings, timestep=t
+            ).sample
+
+            if do_classifier_free_guidance:
+                model_output_uncond, model_output_text = model_output.chunk(2)
+                model_output = model_output_uncond + guidance_scale * (model_output_text - model_output_uncond)
+                model_output -= torch.logsumexp(model_output, dim=1, keepdim=True)
 
             model_output = self.truncate(model_output, truncation_rate)
 
             # remove `log(0)`'s (`-inf`s)
             model_output = model_output.clamp(-70)
 
             # compute the previous noisy sample x_t -> x_t-1
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from ..utils import is_flax_available, is_scipy_available, is_torch_available
 
 
 if is_torch_available():
     from .scheduling_ddim import DDIMScheduler
     from .scheduling_ddpm import DDPMScheduler
+    from .scheduling_dpmsolver_multistep import DPMSolverMultistepScheduler
     from .scheduling_euler_ancestral_discrete import EulerAncestralDiscreteScheduler
     from .scheduling_euler_discrete import EulerDiscreteScheduler
     from .scheduling_ipndm import IPNDMScheduler
     from .scheduling_karras_ve import KarrasVeScheduler
     from .scheduling_pndm import PNDMScheduler
     from .scheduling_repaint import RePaintScheduler
     from .scheduling_sde_ve import ScoreSdeVeScheduler
@@ -31,14 +32,15 @@
     from .scheduling_vq_diffusion import VQDiffusionScheduler
 else:
     from ..utils.dummy_pt_objects import *  # noqa F403
 
 if is_flax_available():
     from .scheduling_ddim_flax import FlaxDDIMScheduler
     from .scheduling_ddpm_flax import FlaxDDPMScheduler
+    from .scheduling_dpmsolver_multistep_flax import FlaxDPMSolverMultistepScheduler
     from .scheduling_karras_ve_flax import FlaxKarrasVeScheduler
     from .scheduling_lms_discrete_flax import FlaxLMSDiscreteScheduler
     from .scheduling_pndm_flax import FlaxPNDMScheduler
     from .scheduling_sde_ve_flax import FlaxScoreSdeVeScheduler
     from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
 else:
     from ..utils.dummy_flax_objects import *  # noqa F403
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddim.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddim.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, deprecate
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
 # Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->DDIM
 class DDIMSchedulerOutput(BaseOutput):
     """
@@ -78,16 +78,16 @@
 class DDIMScheduler(SchedulerMixin, ConfigMixin):
     """
     Denoising diffusion implicit models is a scheduler that extends the denoising procedure introduced in denoising
     diffusion probabilistic models (DDPMs) with non-Markovian guidance.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2010.02502
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -102,37 +102,45 @@
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
 
-    _compatible_classes = [
-        "PNDMScheduler",
-        "DDPMScheduler",
-        "LMSDiscreteScheduler",
-        "EulerDiscreteScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
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
@@ -204,14 +212,15 @@
         self,
         model_output: torch.FloatTensor,
         timestep: int,
         sample: torch.FloatTensor,
         eta: float = 0.0,
         use_clipped_model_output: bool = False,
         generator=None,
+        variance_noise: Optional[torch.FloatTensor] = None,
         return_dict: bool = True,
     ) -> Union[DDIMSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
@@ -221,14 +230,17 @@
                 current instance of sample being created by diffusion process.
             eta (`float`): weight of noise for added noise in diffusion step.
             use_clipped_model_output (`bool`): if `True`, compute "corrected" `model_output` from the clipped
                 predicted original sample. Necessary because predicted original sample is clipped to [-1, 1] when
                 `self.config.clip_sample` is `True`. If no clipping has happened, "corrected" `model_output` would
                 coincide with the one provided as input and `use_clipped_model_output` will have not effect.
             generator: random number generator.
+            variance_noise (`torch.FloatTensor`): instead of generating noise for the variance using `generator`, we
+                can directly provide the noise for the variance itself. This is useful for methods such as
+                CycleDiffusion. (https://arxiv.org/abs/2210.05559)
             return_dict (`bool`): option for returning tuple rather than DDIMSchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_utils.DDIMSchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.DDIMSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
@@ -256,15 +268,27 @@
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
@@ -279,17 +303,31 @@
         pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * model_output
 
         # 7. compute x_t without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
         prev_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
 
         if eta > 0:
             # randn_like does not support generator https://github.com/pytorch/pytorch/issues/27072
-            device = model_output.device if torch.is_tensor(model_output) else "cpu"
-            noise = torch.randn(model_output.shape, dtype=model_output.dtype, generator=generator).to(device)
-            variance = self._get_variance(timestep, prev_timestep) ** (0.5) * eta * noise
+            device = model_output.device
+            if variance_noise is not None and generator is not None:
+                raise ValueError(
+                    "Cannot pass both generator and variance_noise. Please make sure that either `generator` or"
+                    " `variance_noise` stays `None`."
+                )
+
+            if variance_noise is None:
+                if device.type == "mps":
+                    # randn does not work reproducibly on mps
+                    variance_noise = torch.randn(model_output.shape, dtype=model_output.dtype, generator=generator)
+                    variance_noise = variance_noise.to(device)
+                else:
+                    variance_noise = torch.randn(
+                        model_output.shape, generator=generator, device=device, dtype=model_output.dtype
+                    )
+            variance = self._get_variance(timestep, prev_timestep) ** (0.5) * eta * variance_noise
 
             prev_sample = prev_sample + variance
 
         if not return_dict:
             return (prev_sample,)
 
         return DDIMSchedulerOutput(prev_sample=prev_sample, pred_original_sample=pred_original_sample)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddim_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddpm_flax.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,39 @@
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
-from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
+from ..configuration_utils import ConfigMixin, FrozenDict, register_to_config
+from ..utils import deprecate
+from .scheduling_utils_flax import (
+    _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
+    FlaxSchedulerMixin,
+    FlaxSchedulerOutput,
+    broadcast_to_shape_from_left,
+)
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999) -> jnp.ndarray:
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
@@ -52,239 +58,260 @@
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
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
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
 
+    _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
+
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddpm.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ddpm.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
-from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput
+from ..configuration_utils import ConfigMixin, FrozenDict, register_to_config
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, deprecate
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
 class DDPMSchedulerOutput(BaseOutput):
     """
     Output class for the scheduler's step function output.
@@ -76,16 +76,16 @@
 class DDPMScheduler(SchedulerMixin, ConfigMixin):
     """
     Denoising diffusion probabilistic models (DDPMs) explores the connections between denoising score matching and
     Langevin dynamics sampling.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2006.11239
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -95,36 +95,43 @@
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         variance_type (`str`):
             options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
             `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
-
+        prediction_type (`str`, default `epsilon`):
+            indicates whether the model predicts the noise (epsilon), or the samples. One of `epsilon`, `sample`.
+            `v-prediction` is not supported for this scheduler.
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "PNDMScheduler",
-        "LMSDiscreteScheduler",
-        "EulerDiscreteScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
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
@@ -196,14 +203,15 @@
 
         # hacks - were probably added for training stability
         if variance_type == "fixed_small":
             variance = torch.clamp(variance, min=1e-20)
         # for rl-diffuser https://arxiv.org/abs/2205.09991
         elif variance_type == "fixed_small_log":
             variance = torch.log(torch.clamp(variance, min=1e-20))
+            variance = torch.exp(0.5 * variance)
         elif variance_type == "fixed_large":
             variance = self.betas[t]
         elif variance_type == "fixed_large_log":
             # Glide max_log
             variance = torch.log(self.betas[t])
         elif variance_type == "learned":
             return predicted_variance
@@ -216,38 +224,46 @@
         return variance
 
     def step(
         self,
         model_output: torch.FloatTensor,
         timestep: int,
         sample: torch.FloatTensor,
-        predict_epsilon=True,
         generator=None,
         return_dict: bool = True,
+        **kwargs,
     ) -> Union[DDPMSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
             model_output (`torch.FloatTensor`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`torch.FloatTensor`):
                 current instance of sample being created by diffusion process.
-            predict_epsilon (`bool`):
-                optional flag to use when model predicts the samples directly instead of the noise, epsilon.
             generator: random number generator.
             return_dict (`bool`): option for returning tuple rather than DDPMSchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
         """
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDPMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            new_config = dict(self.config)
+            new_config["prediction_type"] = "epsilon" if predict_epsilon else "sample"
+            self._internal_dict = FrozenDict(new_config)
+
         t = timestep
 
         if model_output.shape[1] == sample.shape[1] * 2 and self.variance_type in ["learned", "learned_range"]:
             model_output, predicted_variance = torch.split(model_output, sample.shape[1], dim=1)
         else:
             predicted_variance = None
 
@@ -255,18 +271,23 @@
         alpha_prod_t = self.alphas_cumprod[t]
         alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
         beta_prod_t = 1 - alpha_prod_t
         beta_prod_t_prev = 1 - alpha_prod_t_prev
 
         # 2. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        if predict_epsilon:
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
@@ -276,18 +297,27 @@
         # 5. Compute predicted previous sample µ_t
         # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
         pred_prev_sample = pred_original_sample_coeff * pred_original_sample + current_sample_coeff * sample
 
         # 6. Add noise
         variance = 0
         if t > 0:
-            noise = torch.randn(
-                model_output.size(), dtype=model_output.dtype, layout=model_output.layout, generator=generator
-            ).to(model_output.device)
-            variance = (self._get_variance(t, predicted_variance=predicted_variance) ** 0.5) * noise
+            device = model_output.device
+            if device.type == "mps":
+                # randn does not work reproducibly on mps
+                variance_noise = torch.randn(model_output.shape, dtype=model_output.dtype, generator=generator)
+                variance_noise = variance_noise.to(device)
+            else:
+                variance_noise = torch.randn(
+                    model_output.shape, generator=generator, device=device, dtype=model_output.dtype
+                )
+            if self.variance_type == "fixed_small_log":
+                variance = self._get_variance(t, predicted_variance=predicted_variance) * variance_noise
+            else:
+                variance = (self._get_variance(t, predicted_variance=predicted_variance) ** 0.5) * variance_noise
 
         pred_prev_sample = pred_prev_sample + variance
 
         if not return_dict:
             return (pred_prev_sample,)
 
         return DDPMSchedulerOutput(prev_sample=pred_prev_sample, pred_original_sample=pred_original_sample)
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ddpm_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_repaint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,285 +1,322 @@
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
+import numpy as np
+import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
+from ..utils import BaseOutput
+from .scheduling_utils import SchedulerMixin
+
 
+@dataclass
+class RePaintSchedulerOutput(BaseOutput):
+    """
+    Output class for the scheduler's step function output.
 
-def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999) -> jnp.ndarray:
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
+
+
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
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
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
-        tensor_format (`str`): whether the scheduler expects pytorch or numpy arrays.
 
     """
 
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
-            predict_epsilon (`bool`):
-                optional flag to use when model predicts the samples directly instead of the noise, epsilon.
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
-        if predict_epsilon:
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
+
+        # 8. Algorithm 1 Line 5 https://arxiv.org/pdf/2201.09865.pdf
+        prev_known_part = (alpha_prod_t**0.5) * original_image + ((1 - alpha_prod_t) ** 0.5) * noise
 
-        pred_prev_sample = pred_prev_sample + variance
+        # 9. Algorithm 1 Line 8 https://arxiv.org/pdf/2201.09865.pdf
+        pred_prev_sample = mask * prev_known_part + (1.0 - mask) * prev_unknown_part
 
         if not return_dict:
-            return (pred_prev_sample, state)
+            return (
+                pred_prev_sample,
+                pred_original_sample,
+            )
 
-        return FlaxDDPMSchedulerOutput(prev_sample=pred_prev_sample, state=state)
+        return RePaintSchedulerOutput(prev_sample=pred_prev_sample, pred_original_sample=pred_original_sample)
+
+    def undo_step(self, sample, timestep, generator=None):
+        n = self.config.num_train_timesteps // self.num_inference_steps
+
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput, deprecate, logging
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, logging
 from .scheduling_utils import SchedulerMixin
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 @dataclass
@@ -48,36 +48,30 @@
 class EulerAncestralDiscreteScheduler(SchedulerMixin, ConfigMixin):
     """
     Ancestral sampling with Euler method steps. Based on the original k-diffusion implementation by Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L72
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
 
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "LMSDiscreteScheduler",
-        "PNDMScheduler",
-        "EulerDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
@@ -146,15 +140,19 @@
         self.num_inference_steps = num_inference_steps
 
         timesteps = np.linspace(0, self.config.num_train_timesteps - 1, num_inference_steps, dtype=float)[::-1].copy()
         sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.interp(timesteps, np.arange(0, len(sigmas)), sigmas)
         sigmas = np.concatenate([sigmas, [0.0]]).astype(np.float32)
         self.sigmas = torch.from_numpy(sigmas).to(device=device)
-        self.timesteps = torch.from_numpy(timesteps).to(device=device)
+        if str(device).startswith("mps"):
+            # mps does not support float64
+            self.timesteps = torch.from_numpy(timesteps).to(device, dtype=torch.float32)
+        else:
+            self.timesteps = torch.from_numpy(timesteps).to(device=device)
 
     def step(
         self,
         model_output: torch.FloatTensor,
         timestep: Union[float, torch.FloatTensor],
         sample: torch.FloatTensor,
         generator: Optional[torch.Generator] = None,
@@ -187,15 +185,15 @@
             raise ValueError(
                 "Passing integer indices (e.g. from `enumerate(timesteps)`) as timesteps to"
                 " `EulerDiscreteScheduler.step()` is not supported. Make sure to pass"
                 " one of the `scheduler.timesteps` as a timestep.",
             )
 
         if not self.is_scale_input_called:
-            logger.warn(
+            logger.warning(
                 "The `scale_model_input` function should be called before `step` to ensure correct denoising. "
                 "See `StableDiffusionPipeline` for a usage example."
             )
 
         if isinstance(timestep, torch.Tensor):
             timestep = timestep.to(self.timesteps.device)
 
@@ -212,16 +210,16 @@
         # 2. Convert to an ODE derivative
         derivative = (sample - pred_original_sample) / sigma
 
         dt = sigma_down - sigma
 
         prev_sample = sample + derivative * dt
 
-        device = model_output.device if torch.is_tensor(model_output) else "cpu"
-        if str(device) == "mps":
+        device = model_output.device
+        if device.type == "mps":
             # randn does not work reproducibly on mps
             noise = torch.randn(model_output.shape, dtype=model_output.dtype, device="cpu", generator=generator).to(
                 device
             )
         else:
             noise = torch.randn(model_output.shape, dtype=model_output.dtype, device=device, generator=generator).to(
                 device
@@ -249,27 +247,15 @@
             self.timesteps = self.timesteps.to(original_samples.device, dtype=torch.float32)
             timesteps = timesteps.to(original_samples.device, dtype=torch.float32)
         else:
             self.timesteps = self.timesteps.to(original_samples.device)
             timesteps = timesteps.to(original_samples.device)
 
         schedule_timesteps = self.timesteps
-
-        if isinstance(timesteps, torch.IntTensor) or isinstance(timesteps, torch.LongTensor):
-            deprecate(
-                "timesteps as indices",
-                "0.8.0",
-                "Passing integer indices  (e.g. from `enumerate(timesteps)`) as timesteps to"
-                " `EulerAncestralDiscreteScheduler.add_noise()` will not be supported in future versions. Make sure to"
-                " pass values from `scheduler.timesteps` as timesteps.",
-                standard_warn=False,
-            )
-            step_indices = timesteps
-        else:
-            step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
+        step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
 
         sigma = self.sigmas[step_indices].flatten()
         while len(sigma.shape) < len(original_samples.shape):
             sigma = sigma.unsqueeze(-1)
 
         noisy_samples = original_samples + noise * sigma
         return noisy_samples
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_euler_discrete.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_euler_discrete.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput, deprecate, logging
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, logging
 from .scheduling_utils import SchedulerMixin
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 @dataclass
@@ -49,45 +49,40 @@
     """
     Euler scheduler (Algorithm 2) from Karras et al. (2022) https://arxiv.org/abs/2206.00364. . Based on the original
     k-diffusion implementation by Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L51
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
 
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "LMSDiscreteScheduler",
-        "PNDMScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
 
     @register_to_config
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
@@ -147,15 +142,19 @@
         self.num_inference_steps = num_inference_steps
 
         timesteps = np.linspace(0, self.config.num_train_timesteps - 1, num_inference_steps, dtype=float)[::-1].copy()
         sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.interp(timesteps, np.arange(0, len(sigmas)), sigmas)
         sigmas = np.concatenate([sigmas, [0.0]]).astype(np.float32)
         self.sigmas = torch.from_numpy(sigmas).to(device=device)
-        self.timesteps = torch.from_numpy(timesteps).to(device=device)
+        if str(device).startswith("mps"):
+            # mps does not support float64
+            self.timesteps = torch.from_numpy(timesteps).to(device, dtype=torch.float32)
+        else:
+            self.timesteps = torch.from_numpy(timesteps).to(device=device)
 
     def step(
         self,
         model_output: torch.FloatTensor,
         timestep: Union[float, torch.FloatTensor],
         sample: torch.FloatTensor,
         s_churn: float = 0.0,
@@ -196,29 +195,29 @@
             raise ValueError(
                 "Passing integer indices (e.g. from `enumerate(timesteps)`) as timesteps to"
                 " `EulerDiscreteScheduler.step()` is not supported. Make sure to pass"
                 " one of the `scheduler.timesteps` as a timestep.",
             )
 
         if not self.is_scale_input_called:
-            logger.warn(
+            logger.warning(
                 "The `scale_model_input` function should be called before `step` to ensure correct denoising. "
                 "See `StableDiffusionPipeline` for a usage example."
             )
 
         if isinstance(timestep, torch.Tensor):
             timestep = timestep.to(self.timesteps.device)
 
         step_index = (self.timesteps == timestep).nonzero().item()
         sigma = self.sigmas[step_index]
 
         gamma = min(s_churn / (len(self.sigmas) - 1), 2**0.5 - 1) if s_tmin <= sigma <= s_tmax else 0.0
 
-        device = model_output.device if torch.is_tensor(model_output) else "cpu"
-        if str(device) == "mps":
+        device = model_output.device
+        if device.type == "mps":
             # randn does not work reproducibly on mps
             noise = torch.randn(model_output.shape, dtype=model_output.dtype, device="cpu", generator=generator).to(
                 device
             )
         else:
             noise = torch.randn(model_output.shape, dtype=model_output.dtype, device=device, generator=generator).to(
                 device
@@ -227,15 +226,23 @@
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
@@ -258,27 +265,15 @@
             self.timesteps = self.timesteps.to(original_samples.device, dtype=torch.float32)
             timesteps = timesteps.to(original_samples.device, dtype=torch.float32)
         else:
             self.timesteps = self.timesteps.to(original_samples.device)
             timesteps = timesteps.to(original_samples.device)
 
         schedule_timesteps = self.timesteps
-
-        if isinstance(timesteps, torch.IntTensor) or isinstance(timesteps, torch.LongTensor):
-            deprecate(
-                "timesteps as indices",
-                "0.8.0",
-                "Passing integer indices  (e.g. from `enumerate(timesteps)`) as timesteps to"
-                " `EulerDiscreteScheduler.add_noise()` will not be supported in future versions. Make sure to"
-                " pass values from `scheduler.timesteps` as timesteps.",
-                standard_warn=False,
-            )
-            step_indices = timesteps
-        else:
-            step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
+        step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
 
         sigma = self.sigmas[step_indices].flatten()
         while len(sigma.shape) < len(original_samples.shape):
             sigma = sigma.unsqueeze(-1)
 
         noisy_samples = original_samples + noise * sigma
         return noisy_samples
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_ipndm.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_ipndm.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 class IPNDMScheduler(SchedulerMixin, ConfigMixin):
     """
     Improved Pseudo numerical methods for diffusion models (iPNDM) ported from @crowsonkb's amazing k-diffusion
     [library](https://github.com/crowsonkb/v-diffusion-pytorch/blob/987f8985e38208345c1959b0ea767a625831cc9b/diffusion/sampling.py#L296)
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2202.09778
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
     """
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_karras_ve.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_karras_ve.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
     [1] Karras, Tero, et al. "Elucidating the Design Space of Diffusion-Based Generative Models."
     https://arxiv.org/abs/2206.00364 [2] Song, Yang, et al. "Score-based generative modeling through stochastic
     differential equations." https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details on the parameters, see the original paper's Appendix E.: "Elucidating the Design Space of
     Diffusion-Based Generative Models." https://arxiv.org/abs/2206.00364. The grid search values used to find the
     optimal {s_noise, s_churn, s_min, s_max} for a specific model are described in Table 5 of the paper.
 
     Args:
         sigma_min (`float`): minimum noise magnitude
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_karras_ve_flax.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
     [1] Karras, Tero, et al. "Elucidating the Design Space of Diffusion-Based Generative Models."
     https://arxiv.org/abs/2206.00364 [2] Song, Yang, et al. "Score-based generative modeling through stochastic
     differential equations." https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details on the parameters, see the original paper's Appendix E.: "Elucidating the Design Space of
     Diffusion-Based Generative Models." https://arxiv.org/abs/2206.00364. The grid search values used to find the
     optimal {s_noise, s_churn, s_min, s_max} for a specific model are described in Table 5 of the paper.
 
     Args:
         sigma_min (`float`): minimum noise magnitude
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_lms_discrete.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import numpy as np
 import torch
 
 from scipy import integrate
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput, deprecate
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
 # Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->LMSDiscrete
 class LMSDiscreteSchedulerOutput(BaseOutput):
     """
@@ -48,36 +48,30 @@
     """
     Linear Multistep Scheduler for discrete beta schedules. Based on the original k-diffusion implementation by
     Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L181
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
 
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "PNDMScheduler",
-        "EulerDiscreteScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
@@ -168,16 +162,21 @@
         """
         self.num_inference_steps = num_inference_steps
 
         timesteps = np.linspace(0, self.config.num_train_timesteps - 1, num_inference_steps, dtype=float)[::-1].copy()
         sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.interp(timesteps, np.arange(0, len(sigmas)), sigmas)
         sigmas = np.concatenate([sigmas, [0.0]]).astype(np.float32)
+
         self.sigmas = torch.from_numpy(sigmas).to(device=device)
-        self.timesteps = torch.from_numpy(timesteps).to(device=device)
+        if str(device).startswith("mps"):
+            # mps does not support float64
+            self.timesteps = torch.from_numpy(timesteps).to(device, dtype=torch.float32)
+        else:
+            self.timesteps = torch.from_numpy(timesteps).to(device=device)
 
         self.derivatives = []
 
     def step(
         self,
         model_output: torch.FloatTensor,
         timestep: Union[float, torch.FloatTensor],
@@ -207,30 +206,15 @@
             warnings.warn(
                 "The `scale_model_input` function should be called before `step` to ensure correct denoising. "
                 "See `StableDiffusionPipeline` for a usage example."
             )
 
         if isinstance(timestep, torch.Tensor):
             timestep = timestep.to(self.timesteps.device)
-        if (
-            isinstance(timestep, int)
-            or isinstance(timestep, torch.IntTensor)
-            or isinstance(timestep, torch.LongTensor)
-        ):
-            deprecate(
-                "timestep as an index",
-                "0.8.0",
-                "Passing integer indices (e.g. from `enumerate(timesteps)`) as timesteps to"
-                " `LMSDiscreteScheduler.step()` will not be supported in future versions. Make sure to pass"
-                " one of the `scheduler.timesteps` as a timestep.",
-                standard_warn=False,
-            )
-            step_index = timestep
-        else:
-            step_index = (self.timesteps == timestep).nonzero().item()
+        step_index = (self.timesteps == timestep).nonzero().item()
         sigma = self.sigmas[step_index]
 
         # 1. compute predicted original sample (x_0) from sigma-scaled predicted noise
         pred_original_sample = sample - sigma * model_output
 
         # 2. Convert to an ODE derivative
         derivative = (sample - pred_original_sample) / sigma
@@ -255,39 +239,26 @@
     def add_noise(
         self,
         original_samples: torch.FloatTensor,
         noise: torch.FloatTensor,
         timesteps: torch.FloatTensor,
     ) -> torch.FloatTensor:
         # Make sure sigmas and timesteps have the same device and dtype as original_samples
-        self.sigmas = self.sigmas.to(device=original_samples.device, dtype=original_samples.dtype)
+        sigmas = self.sigmas.to(device=original_samples.device, dtype=original_samples.dtype)
         if original_samples.device.type == "mps" and torch.is_floating_point(timesteps):
             # mps does not support float64
-            self.timesteps = self.timesteps.to(original_samples.device, dtype=torch.float32)
+            schedule_timesteps = self.timesteps.to(original_samples.device, dtype=torch.float32)
             timesteps = timesteps.to(original_samples.device, dtype=torch.float32)
         else:
-            self.timesteps = self.timesteps.to(original_samples.device)
+            schedule_timesteps = self.timesteps.to(original_samples.device)
             timesteps = timesteps.to(original_samples.device)
 
-        schedule_timesteps = self.timesteps
-
-        if isinstance(timesteps, torch.IntTensor) or isinstance(timesteps, torch.LongTensor):
-            deprecate(
-                "timesteps as indices",
-                "0.8.0",
-                "Passing integer indices  (e.g. from `enumerate(timesteps)`) as timesteps to"
-                " `LMSDiscreteScheduler.add_noise()` will not be supported in future versions. Make sure to"
-                " pass values from `scheduler.timesteps` as timesteps.",
-                standard_warn=False,
-            )
-            step_indices = timesteps
-        else:
-            step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
+        step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
 
-        sigma = self.sigmas[step_indices].flatten()
+        sigma = sigmas[step_indices].flatten()
         while len(sigma.shape) < len(original_samples.shape):
             sigma = sigma.unsqueeze(-1)
 
         noisy_samples = original_samples + noise * sigma
         return noisy_samples
 
     def __len__(self):
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_lms_discrete_flax.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from typing import Optional, Tuple, Union
 
 import flax
 import jax.numpy as jnp
 from scipy import integrate
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
+from .scheduling_utils_flax import (
+    _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
+    FlaxSchedulerMixin,
+    FlaxSchedulerOutput,
+    broadcast_to_shape_from_left,
+)
 
 
 @flax.struct.dataclass
 class LMSDiscreteSchedulerState:
     # setable values
     num_inference_steps: Optional[int] = None
     timesteps: Optional[jnp.ndarray] = None
@@ -45,28 +50,30 @@
     """
     Linear Multistep Scheduler for discrete beta schedules. Based on the original k-diffusion implementation by
     Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L181
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`jnp.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
     """
 
+    _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+
     @property
     def has_state(self):
         return True
 
     @register_to_config
     def __init__(
         self,
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_pndm.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_pndm.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import math
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from ..configuration_utils import ConfigMixin, register_to_config
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS
 from .scheduling_utils import SchedulerMixin, SchedulerOutput
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
@@ -56,16 +57,16 @@
 class PNDMScheduler(SchedulerMixin, ConfigMixin):
     """
     Pseudo numerical methods for diffusion models (PNDM) proposes using more advanced ODE integration techniques,
     namely Runge-Kutta method and a linear multi-step method.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2202.09778
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -84,21 +85,15 @@
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
 
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "LMSDiscreteScheduler",
-        "EulerDiscreteScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_pndm_flax.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_pndm_flax.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 from typing import Optional, Tuple, Union
 
 import flax
 import jax
 import jax.numpy as jnp
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from .scheduling_utils_flax import FlaxSchedulerMixin, FlaxSchedulerOutput, broadcast_to_shape_from_left
+from .scheduling_utils_flax import (
+    _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS,
+    FlaxSchedulerMixin,
+    FlaxSchedulerOutput,
+    broadcast_to_shape_from_left,
+)
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps: int, max_beta=0.999) -> jnp.ndarray:
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
@@ -83,16 +88,16 @@
 class FlaxPNDMScheduler(FlaxSchedulerMixin, ConfigMixin):
     """
     Pseudo numerical methods for diffusion models (PNDM) proposes using more advanced ODE integration techniques,
     namely Runge-Kutta method and a linear multi-step method.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2202.09778
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -110,14 +115,16 @@
             otherwise it uses the value of alpha at step 0.
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
     """
 
+    _compatibles = _FLAX_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+
     @property
     def has_state(self):
         return True
 
     @register_to_config
     def __init__(
         self,
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_repaint.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_ve.py`

 * *Files 19% similar despite different names*

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
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
-
-    For more details, see the original paper: https://arxiv.org/pdf/2201.09865.pdf
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_sde_vp.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_sde_vp.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 class ScoreSdeVpScheduler(SchedulerMixin, ConfigMixin):
     """
     The variance preserving stochastic differential equation (SDE) scheduler.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more information, see the original paper: https://arxiv.org/abs/2011.13456
 
     UNDER CONSTRUCTION
 
     """
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/schedulers/scheduling_vq_diffusion.py` & `diffusers-unchained-0.9.0/src/diffusers/schedulers/scheduling_vq_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     The VQ-diffusion transformer outputs predicted probabilities of the initial unnoised image.
 
     The VQ-diffusion scheduler converts the transformer's output into a sample for the unnoised image at the previous
     diffusion timestep.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2111.14822
 
     Args:
         num_vec_classes (`int`):
             The number of classes of the vector embeddings of the latent pixels. Includes the class for the masked
             latent pixel.
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/training_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/training_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/__init__.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,20 +27,23 @@
     is_flax_available,
     is_inflect_available,
     is_modelcards_available,
     is_onnx_available,
     is_scipy_available,
     is_tf_available,
     is_torch_available,
+    is_torch_version,
     is_transformers_available,
+    is_transformers_version,
     is_unidecode_available,
     requires_backends,
 )
 from .logging import get_logger
 from .outputs import BaseOutput
+from .pil_utils import PIL_INTERPOLATION
 
 
 if is_torch_available():
     from .testing_utils import (
         floats_tensor,
         load_hf_numpy,
         load_image,
@@ -62,11 +65,22 @@
 default_cache_path = os.path.join(hf_cache_home, "diffusers")
 
 
 CONFIG_NAME = "config.json"
 WEIGHTS_NAME = "diffusion_pytorch_model.bin"
 FLAX_WEIGHTS_NAME = "diffusion_flax_model.msgpack"
 ONNX_WEIGHTS_NAME = "model.onnx"
+ONNX_EXTERNAL_WEIGHTS_NAME = "weights.pb"
 HUGGINGFACE_CO_RESOLVE_ENDPOINT = "https://huggingface.co"
 DIFFUSERS_CACHE = default_cache_path
 DIFFUSERS_DYNAMIC_MODULE_NAME = "diffusers_modules"
 HF_MODULES_CACHE = os.getenv("HF_MODULES_CACHE", os.path.join(hf_cache_home, "modules"))
+
+_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS = [
+    "DDIMScheduler",
+    "DDPMScheduler",
+    "PNDMScheduler",
+    "LMSDiscreteScheduler",
+    "EulerDiscreteScheduler",
+    "EulerAncestralDiscreteScheduler",
+    "DPMSolverMultistepScheduler",
+]
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/deprecation_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/deprecation_utils.py`

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

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/dummy_flax_and_transformers_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/dummy_flax_objects.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/dummy_flax_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,29 @@
         requires_backends(cls, ["flax"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["flax"])
 
 
+class FlaxDPMSolverMultistepScheduler(metaclass=DummyObject):
+    _backends = ["flax"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["flax"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["flax"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["flax"])
+
+
 class FlaxKarrasVeScheduler(metaclass=DummyObject):
     _backends = ["flax"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["flax"])
 
     @classmethod
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/dummy_pt_objects.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/dummy_pt_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,29 @@
         requires_backends(cls, ["torch"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
 
+class LDMSuperResolutionPipeline(metaclass=DummyObject):
+    _backends = ["torch"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["torch"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["torch"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["torch"])
+
+
 class PNDMPipeline(metaclass=DummyObject):
     _backends = ["torch"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch"])
 
     @classmethod
@@ -268,45 +283,45 @@
         requires_backends(cls, ["torch"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
 
-class VQDiffusionPipeline(metaclass=DummyObject):
+class DDIMScheduler(metaclass=DummyObject):
     _backends = ["torch"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
 
-class DDIMScheduler(metaclass=DummyObject):
+class DDPMScheduler(metaclass=DummyObject):
     _backends = ["torch"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch"])
 
 
-class DDPMScheduler(metaclass=DummyObject):
+class DPMSolverMultistepScheduler(metaclass=DummyObject):
     _backends = ["torch"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/dummy_torch_and_scipy_objects.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,29 @@
         requires_backends(cls, ["torch", "transformers", "onnx"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["torch", "transformers", "onnx"])
 
 
+class OnnxStableDiffusionInpaintPipelineLegacy(metaclass=DummyObject):
+    _backends = ["torch", "transformers", "onnx"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["torch", "transformers", "onnx"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["torch", "transformers", "onnx"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["torch", "transformers", "onnx"])
+
+
 class OnnxStableDiffusionPipeline(metaclass=DummyObject):
     _backends = ["torch", "transformers", "onnx"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["torch", "transformers", "onnx"])
 
     @classmethod
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/logging.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/logging.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/model_card_template.md` & `diffusers-unchained-0.9.0/src/diffusers/utils/model_card_template.md`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/outputs.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/outputs.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers/utils/testing_utils.py` & `diffusers-unchained-0.9.0/src/diffusers/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/PKG-INFO` & `diffusers-unchained-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: diffusers-unchained
-Version: 0.7.0
-Summary: Diffusers
-Home-page: https://github.com/ghunkins/diffusers-unchained
-Author: The HuggingFace Team ft. Mage Team
-Author-email: greg@mage.space
-License: Apache
-Keywords: deep learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: quality
-Provides-Extra: docs
-Provides-Extra: training
-Provides-Extra: test
-Provides-Extra: torch
-Provides-Extra: flax
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
     <br>
     <img src="https://github.com/huggingface/diffusers/raw/main/docs/source/imgs/diffusers_library.jpg" width="400"/>
     <br>
 <p>
 <p align="center">
     <a href="https://github.com/huggingface/diffusers/blob/main/LICENSE">
@@ -179,23 +148,15 @@
 
 If you wish to use a different scheduler (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate
 it before the pipeline and pass it to `from_pretrained`.
     
 ```python
 from diffusers import LMSDiscreteScheduler
 
-lms = LMSDiscreteScheduler.from_config("CompVis/stable-diffusion-v1-4", subfolder="scheduler")
-
-pipe = StableDiffusionPipeline.from_pretrained(
-    "runwayml/stable-diffusion-v1-5", 
-    revision="fp16", 
-    torch_dtype=torch.float16,
-    scheduler=lms,
-)
-pipe = pipe.to("cuda")
+pipe.scheduler = LMSDiscreteScheduler.from_config(pipe.scheduler.config)
 
 prompt = "a photo of an astronaut riding a horse on mars"
 image = pipe(prompt).images[0]  
     
 image.save("astronaut_rides_horse.png")
 ```
 
@@ -373,22 +334,23 @@
 
 Fine-tuning techniques make it possible to adapt Stable Diffusion to your own dataset, or add new subjects to it. These are some of the techniques supported in `diffusers`:
 
 Textual Inversion is a technique for capturing novel concepts from a small number of example images in a way that can later be used to control text-to-image pipelines. It does so by learning new 'words' in the embedding space of the pipeline's text encoder. These special words can then be used within text prompts to achieve very fine-grained control of the resulting images. 
 
 - Textual Inversion. Capture novel concepts from a small set of sample images, and associate them with new "words" in the embedding space of the text encoder. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation](https://huggingface.co/docs/diffusers/training/text_inversion) to try for yourself.
 
-- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training examples](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and training recommendations.
+- Dreambooth. Another technique to capture new concepts in Stable Diffusion. This method fine-tunes the UNet (and, optionally, also the text encoder) of the pipeline to achieve impressive results. Please, refer to [our training example](https://github.com/huggingface/diffusers/tree/main/examples/dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for additional details and training recommendations.
 
 - Full Stable Diffusion fine-tuning. If you have a more sizable dataset with a specific look or style, you can fine-tune Stable Diffusion so that it outputs images following those examples. This was the approach taken to create [a Pokémon Stable Diffusion model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at [our text-to-image fine-tuning example](https://github.com/huggingface/diffusers/tree/main/examples/text_to_image) and go from there.
 
 
 ## Stable Diffusion Community Pipelines
 
-The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! Take a look and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipelines).
+The release of Stable Diffusion as an open source model has fostered a lot of interesting ideas and experimentation. 
+Our [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/examples/community) contains many ideas worth exploring, like interpolating to create animated videos, using CLIP Guidance for additional prompt fidelity, term weighting, and much more! [Take a look](https://huggingface.co/docs/diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own](https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline).
 
 ## Other Examples
 
 There are many ways to try running Diffusers! Here we outline code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and interactive web-tools.
 
 ### Running Code
 
@@ -429,18 +391,22 @@
 
 # save image
 image.save("ddpm_generated_image.png")
 ```
 - [Unconditional Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256)
 - [Unconditional Diffusion with continuous scheduler](https://huggingface.co/google/ncsnpp-ffhq-1024)
 
-**Other Notebooks**:
+**Other Image Notebooks**:
 * [image-to-image generation with Stable Diffusion](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 * [tweak images via repeated Stable Diffusion seeds](https://colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
 
+**Diffusers for Other Modalities**:
+* [Molecule conformation generation](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/geodiff_molecule_conformation.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+* [Model-based reinforcement learning](https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg),
+
 ### Web Demos
 If you just want to play around with some web demos, you can try out the following 🚀 Spaces:
 | Model                          	| Hugging Face Spaces                                                                                                                                               	|
 |--------------------------------	|-------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
 | Text-to-Image Latent Diffusion 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/text2img-latent-diffusion) 	|
 | Faces generator                	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion)    	|
 | DDPM with different schedulers 	| [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/fusing/celeba-diffusion)           	|
@@ -455,15 +421,15 @@
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-429a-affe-096e8199ad5b.png" width="800"/>
     <br>
     <em> Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
     
 **Schedulers**: Algorithm class for both **inference** and **training**.
-The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training.
+The class provides functionality to compute previous image according to alpha, beta schedule as well as predict noise for training. Also known as **Samplers**.
 *Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-4cda-b3e8-432d9dc7ad38.png" width="800"/>
     <br>
     <em> Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/abs/2006.11239). </em>
 <p>
```

#### html2text {}

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1 Name: diffusers-unchained Version: 0.7.0 Summary:
-Diffusers Home-page: https://github.com/ghunkins/diffusers-unchained Author:
-The HuggingFace Team ft. Mage Team Author-email: greg@mage.space License:
-Apache Keywords: deep learning Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
-Provides-Extra: quality Provides-Extra: docs Provides-Extra: training Provides-
-Extra: test Provides-Extra: torch Provides-Extra: flax Provides-Extra: dev
-License-File: LICENSE
 
      [https://github.com/huggingface/diffusers/raw/main/docs/source/imgs/
                             diffusers_library.jpg]
                [GitHub] [GitHub_release] [Contributor_Covenant]
 ð¤ Diffusers provides pretrained diffusion models across multiple modalities,
 such as vision and audio, and serves as a modular toolbox for inference and
 training of diffusion models. More precisely, ð¤ Diffusers offers: - State-
@@ -115,34 +100,31 @@
 following snippet should result in less than 4GB VRAM. ```python pipe =
 StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="fp16", torch_dtype=torch.float16, ) pipe = pipe.to("cuda") prompt =
 "a photo of an astronaut riding a horse on mars" pipe.enable_attention_slicing
 () image = pipe(prompt).images[0] ``` If you wish to use a different scheduler
 (e.g.: DDIM, LMS, PNDM/PLMS), you can instantiate it before the pipeline and
 pass it to `from_pretrained`. ```python from diffusers import
-LMSDiscreteScheduler lms = LMSDiscreteScheduler.from_config("CompVis/stable-
-diffusion-v1-4", subfolder="scheduler") pipe =
-StableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
-revision="fp16", torch_dtype=torch.float16, scheduler=lms, ) pipe = pipe.to
-("cuda") prompt = "a photo of an astronaut riding a horse on mars" image = pipe
-(prompt).images[0] image.save("astronaut_rides_horse.png") ``` If you want to
-run Stable Diffusion on CPU or you want to have maximum precision on GPU,
-please run the model in the default *full-precision* setting: ```python # make
-sure you're logged in with `huggingface-cli login` from diffusers import
-StableDiffusionPipeline pipe = StableDiffusionPipeline.from_pretrained
-("runwayml/stable-diffusion-v1-5") # disable the following line if you run on
-CPU pipe = pipe.to("cuda") prompt = "a photo of an astronaut riding a horse on
+LMSDiscreteScheduler pipe.scheduler = LMSDiscreteScheduler.from_config
+(pipe.scheduler.config) prompt = "a photo of an astronaut riding a horse on
 mars" image = pipe(prompt).images[0] image.save("astronaut_rides_horse.png")
-``` ### JAX/Flax Diffusers offers a JAX / Flax implementation of Stable
-Diffusion for very fast inference. JAX shines specially on TPU hardware because
-each TPU server has 8 accelerators working in parallel, but it runs great on
-GPUs too. Running the pipeline with the default PNDMScheduler: ```python import
-jax import numpy as np from flax.jax_utils import replicate from
-flax.training.common_utils import shard from diffusers import
-FlaxStableDiffusionPipeline pipeline, params =
+``` If you want to run Stable Diffusion on CPU or you want to have maximum
+precision on GPU, please run the model in the default *full-precision* setting:
+```python # make sure you're logged in with `huggingface-cli login` from
+diffusers import StableDiffusionPipeline pipe =
+StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5") #
+disable the following line if you run on CPU pipe = pipe.to("cuda") prompt = "a
+photo of an astronaut riding a horse on mars" image = pipe(prompt).images[0]
+image.save("astronaut_rides_horse.png") ``` ### JAX/Flax Diffusers offers a JAX
+/ Flax implementation of Stable Diffusion for very fast inference. JAX shines
+specially on TPU hardware because each TPU server has 8 accelerators working in
+parallel, but it runs great on GPUs too. Running the pipeline with the default
+PNDMScheduler: ```python import jax import numpy as np from flax.jax_utils
+import replicate from flax.training.common_utils import shard from diffusers
+import FlaxStableDiffusionPipeline pipeline, params =
 FlaxStableDiffusionPipeline.from_pretrained( "runwayml/stable-diffusion-v1-5",
 revision="flax", dtype=jax.numpy.bfloat16 ) prompt = "a photo of an astronaut
 riding a horse on mars" prng_seed = jax.random.PRNGKey(0) num_inference_steps =
 50 num_samples = jax.device_count() prompt = num_samples * [prompt] prompt_ids
 = pipeline.prepare_inputs(prompt) # shard inputs and rng params = replicate
 (params) prng_seed = jax.random.split(prng_seed, jax.device_count()) prompt_ids
 = shard(prompt_ids) images = pipeline(prompt_ids, params, prng_seed,
@@ -233,36 +215,36 @@
 images, and associate them with new "words" in the embedding space of the text
 encoder. Please, refer to [our training examples](https://github.com/
 huggingface/diffusers/tree/main/examples/textual_inversion) or [documentation]
 (https://huggingface.co/docs/diffusers/training/text_inversion) to try for
 yourself. - Dreambooth. Another technique to capture new concepts in Stable
 Diffusion. This method fine-tunes the UNet (and, optionally, also the text
 encoder) of the pipeline to achieve impressive results. Please, refer to [our
-training examples](https://github.com/huggingface/diffusers/tree/main/examples/
-dreambooth) and [training report](https://wandb.ai/psuraj/dreambooth/reports/
-Dreambooth-Training-Analysis--VmlldzoyNzk0NDc3) for additional details and
-training recommendations. - Full Stable Diffusion fine-tuning. If you have a
-more sizable dataset with a specific look or style, you can fine-tune Stable
-Diffusion so that it outputs images following those examples. This was the
-approach taken to create [a PokÃ©mon Stable Diffusion model](https://
-huggingface.co/justinpinkney/pokemon-stable-diffusion) (by Justing Pinkney /
-Lambda Labs), [a Japanese specific version of Stable Diffusion](https://
-huggingface.co/spaces/rinna/japanese-stable-diffusion) (by [Rinna Co.](https://
-github.com/rinnakk/japanese-stable-diffusion/) and others. You can start at
-[our text-to-image fine-tuning example](https://github.com/huggingface/
-diffusers/tree/main/examples/text_to_image) and go from there. ## Stable
-Diffusion Community Pipelines The release of Stable Diffusion as an open source
-model has fostered a lot of interesting ideas and experimentation. Our
+training example](https://github.com/huggingface/diffusers/tree/main/examples/
+dreambooth) and [training report](https://huggingface.co/blog/dreambooth) for
+additional details and training recommendations. - Full Stable Diffusion fine-
+tuning. If you have a more sizable dataset with a specific look or style, you
+can fine-tune Stable Diffusion so that it outputs images following those
+examples. This was the approach taken to create [a PokÃ©mon Stable Diffusion
+model](https://huggingface.co/justinpinkney/pokemon-stable-diffusion) (by
+Justing Pinkney / Lambda Labs), [a Japanese specific version of Stable
+Diffusion](https://huggingface.co/spaces/rinna/japanese-stable-diffusion) (by
+[Rinna Co.](https://github.com/rinnakk/japanese-stable-diffusion/) and others.
+You can start at [our text-to-image fine-tuning example](https://github.com/
+huggingface/diffusers/tree/main/examples/text_to_image) and go from there. ##
+Stable Diffusion Community Pipelines The release of Stable Diffusion as an open
+source model has fostered a lot of interesting ideas and experimentation. Our
 [Community Examples folder](https://github.com/huggingface/diffusers/tree/main/
 examples/community) contains many ideas worth exploring, like interpolating to
 create animated videos, using CLIP Guidance for additional prompt fidelity,
-term weighting, and much more! Take a look and [contribute your own](https://
-huggingface.co/docs/diffusers/using-diffusers/custom_pipelines). ## Other
-Examples There are many ways to try running Diffusers! Here we outline code-
-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
+term weighting, and much more! [Take a look](https://huggingface.co/docs/
+diffusers/using-diffusers/custom_pipeline_overview) and [contribute your own]
+(https://huggingface.co/docs/diffusers/using-diffusers/contribute_pipeline). ##
+Other Examples There are many ways to try running Diffusers! Here we outline
+code-focused tools (primarily using `DiffusionPipeline`s and Google Colab) and
 interactive web-tools. ### Running Code If you want to run the code yourself
 ð», you can try out: - [Text-to-Image Latent Diffusion](https://
 huggingface.co/CompVis/ldm-text2im-large-256) ```python # !pip install
 diffusers["torch"] transformers from diffusers import DiffusionPipeline device
 = "cuda" model_id = "CompVis/ldm-text2im-large-256" # load model and scheduler
 ldm = DiffusionPipeline.from_pretrained(model_id) ldm = ldm.to(device) # run
 pipeline in inference (sample random noise and denoise) prompt = "A painting of
@@ -274,51 +256,59 @@
 ddpm-celebahq-256" device = "cuda" # load model and scheduler ddpm =
 DDPMPipeline.from_pretrained(model_id) # you can replace DDPMPipeline with
 DDIMPipeline or PNDMPipeline for faster inference ddpm.to(device) # run
 pipeline in inference (sample random noise and denoise) image = ddpm().images
 [0] # save image image.save("ddpm_generated_image.png") ``` - [Unconditional
 Latent Diffusion](https://huggingface.co/CompVis/ldm-celebahq-256) -
 [Unconditional Diffusion with continuous scheduler](https://huggingface.co/
-google/ncsnpp-ffhq-1024) **Other Notebooks**: * [image-to-image generation with
-Stable Diffusion](https://colab.research.google.com/github/huggingface/
-notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb) ![Open In
-Colab](https://colab.research.google.com/assets/colab-badge.svg), * [tweak
-images via repeated Stable Diffusion seeds](https://colab.research.google.com/
-github/pcuenca/diffusers-examples/blob/main/notebooks/stable-diffusion-
-seeds.ipynb) ![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg), ### Web Demos If you just want to play around with some web demos,
-you can try out the following ð Spaces: | Model | Hugging Face Spaces | |---
------------------------------ |------------------------------------------------
+google/ncsnpp-ffhq-1024) **Other Image Notebooks**: * [image-to-image
+generation with Stable Diffusion](https://colab.research.google.com/github/
+huggingface/notebooks/blob/main/diffusers/image_2_image_using_diffusers.ipynb)
+![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg), *
+[tweak images via repeated Stable Diffusion seeds](https://
+colab.research.google.com/github/pcuenca/diffusers-examples/blob/main/
+notebooks/stable-diffusion-seeds.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), **Diffusers for Other
+Modalities**: * [Molecule conformation generation](https://
+colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/
+geodiff_molecule_conformation.ipynb) ![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg), * [Model-based reinforcement
+learning](https://colab.research.google.com/github/huggingface/notebooks/blob/
+main/diffusers/reinforcement_learning_with_diffusers.ipynb) ![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg), ### Web Demos If
+you just want to play around with some web demos, you can try out the following
+ð Spaces: | Model | Hugging Face Spaces | |-------------------------------
+- |----------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------- | | Text-to-Image Latent Diffusion | [!
-[Hugging Face Spaces](https://img.shields.io/badge/
+-------- | | Text-to-Image Latent Diffusion | [![Hugging Face Spaces](https://
+img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://
+huggingface.co/spaces/CompVis/text2img-latent-diffusion) | | Faces generator |
+[![Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-CompVis/text2img-latent-diffusion) | | Faces generator | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/CompVis/celeba-latent-diffusion) | | DDPM
-with different schedulers | [![Hugging Face Spaces](https://img.shields.io/
-badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/
-spaces/fusing/celeba-diffusion) | | Conditional generation from sketch | [!
+CompVis/celeba-latent-diffusion) | | DDPM with different schedulers | [!
 [Hugging Face Spaces](https://img.shields.io/badge/
 %F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
-huggingface/diffuse-the-rest) | | Composable diffusion | [![Hugging Face
-Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
-blue)](https://huggingface.co/spaces/Shuang59/Composable-Diffusion) | ##
-Definitions **Models**: Neural network that models $p_\theta(\mathbf{x}_{t-
-1}|\mathbf{x}_t)$ (see image below) and is trained end-to-end to *denoise* a
-noisy input to an image. *Examples*: UNet, Conditioned UNet, 3D UNet,
-Transformer UNet
+fusing/celeba-diffusion) | | Conditional generation from sketch | [![Hugging
+Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-
+blue)](https://huggingface.co/spaces/huggingface/diffuse-the-rest) | |
+Composable diffusion | [![Hugging Face Spaces](https://img.shields.io/badge/
+%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/
+Shuang59/Composable-Diffusion) | ## Definitions **Models**: Neural network that
+models $p_\theta(\mathbf{x}_{t-1}|\mathbf{x}_t)$ (see image below) and is
+trained end-to-end to *denoise* a noisy input to an image. *Examples*: UNet,
+Conditioned UNet, 3D UNet, Transformer UNet
  [https://user-images.githubusercontent.com/10695622/174349667-04e9e485-793b-
                          429a-affe-096e8199ad5b.png]
           Figure from DDPM paper (https://arxiv.org/abs/2006.11239).
 **Schedulers**: Algorithm class for both **inference** and **training**. The
 class provides functionality to compute previous image according to alpha, beta
-schedule as well as predict noise for training. *Examples*: [DDPM](https://
-arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/abs/2010.02502), [PNDM]
-(https://arxiv.org/abs/2202.09778), [DEIS](https://arxiv.org/abs/2204.13902)
+schedule as well as predict noise for training. Also known as **Samplers**.
+*Examples*: [DDPM](https://arxiv.org/abs/2006.11239), [DDIM](https://arxiv.org/
+abs/2010.02502), [PNDM](https://arxiv.org/abs/2202.09778), [DEIS](https://
+arxiv.org/abs/2204.13902)
  [https://user-images.githubusercontent.com/10695622/174349706-53d58acc-a4d1-
                          4cda-b3e8-432d9dc7ad38.png]
  Sampling and training algorithms. Figure from DDPM paper (https://arxiv.org/
                                abs/2006.11239).
 **Diffusion Pipeline**: End-to-end pipeline that includes multiple diffusion
 models, possible text encoders, ... *Examples*: Glide, Latent-Diffusion,
 Imagen, DALL-E 2
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/SOURCES.txt` & `diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 src/diffusers/optimization.py
 src/diffusers/pipeline_flax_utils.py
 src/diffusers/pipeline_utils.py
 src/diffusers/training_utils.py
 src/diffusers/commands/__init__.py
 src/diffusers/commands/diffusers_cli.py
 src/diffusers/commands/env.py
+src/diffusers/experimental/__init__.py
+src/diffusers/experimental/rl/__init__.py
+src/diffusers/experimental/rl/value_guided_sampling.py
 src/diffusers/models/__init__.py
 src/diffusers/models/attention.py
 src/diffusers/models/attention_flax.py
 src/diffusers/models/embeddings.py
 src/diffusers/models/embeddings_flax.py
 src/diffusers/models/resnet.py
 src/diffusers/models/resnet_flax.py
@@ -34,50 +37,70 @@
 src/diffusers/models/unet_2d_blocks.py
 src/diffusers/models/unet_2d_blocks_flax.py
 src/diffusers/models/unet_2d_condition.py
 src/diffusers/models/unet_2d_condition_flax.py
 src/diffusers/models/vae.py
 src/diffusers/models/vae_flax.py
 src/diffusers/pipelines/__init__.py
+src/diffusers/pipelines/alt_diffusion/__init__.py
+src/diffusers/pipelines/alt_diffusion/modeling_roberta_series.py
+src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py
+src/diffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py
 src/diffusers/pipelines/dance_diffusion/__init__.py
 src/diffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
 src/diffusers/pipelines/ddim/__init__.py
 src/diffusers/pipelines/ddim/pipeline_ddim.py
 src/diffusers/pipelines/ddpm/__init__.py
 src/diffusers/pipelines/ddpm/pipeline_ddpm.py
 src/diffusers/pipelines/latent_diffusion/__init__.py
 src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
+src/diffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
 src/diffusers/pipelines/latent_diffusion_uncond/__init__.py
 src/diffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
 src/diffusers/pipelines/pndm/__init__.py
 src/diffusers/pipelines/pndm/pipeline_pndm.py
 src/diffusers/pipelines/repaint/__init__.py
 src/diffusers/pipelines/repaint/pipeline_repaint.py
 src/diffusers/pipelines/score_sde_ve/__init__.py
 src/diffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
 src/diffusers/pipelines/stable_diffusion/__init__.py
+src/diffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py
 src/diffusers/pipelines/stable_diffusion/pipeline_flax_stable_diffusion.py
 src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
 src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
 src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
+src/diffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint_legacy.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
 src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
+src/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
 src/diffusers/pipelines/stable_diffusion/safety_checker.py
 src/diffusers/pipelines/stable_diffusion/safety_checker_flax.py
+src/diffusers/pipelines/stable_diffusion_safe/__init__.py
+src/diffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
+src/diffusers/pipelines/stable_diffusion_safe/safety_checker.py
 src/diffusers/pipelines/stochastic_karras_ve/__init__.py
 src/diffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
+src/diffusers/pipelines/versatile_diffusion/__init__.py
+src/diffusers/pipelines/versatile_diffusion/modeling_text_unet.py
+src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py
+src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py
+src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py
+src/diffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py
 src/diffusers/pipelines/vq_diffusion/__init__.py
 src/diffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
 src/diffusers/schedulers/__init__.py
 src/diffusers/schedulers/scheduling_ddim.py
 src/diffusers/schedulers/scheduling_ddim_flax.py
 src/diffusers/schedulers/scheduling_ddpm.py
 src/diffusers/schedulers/scheduling_ddpm_flax.py
+src/diffusers/schedulers/scheduling_dpmsolver_multistep.py
+src/diffusers/schedulers/scheduling_dpmsolver_multistep_flax.py
 src/diffusers/schedulers/scheduling_euler_ancestral_discrete.py
 src/diffusers/schedulers/scheduling_euler_discrete.py
 src/diffusers/schedulers/scheduling_ipndm.py
 src/diffusers/schedulers/scheduling_karras_ve.py
 src/diffusers/schedulers/scheduling_karras_ve_flax.py
 src/diffusers/schedulers/scheduling_lms_discrete.py
 src/diffusers/schedulers/scheduling_lms_discrete_flax.py
@@ -91,22 +114,22 @@
 src/diffusers/schedulers/scheduling_utils_flax.py
 src/diffusers/schedulers/scheduling_vq_diffusion.py
 src/diffusers/utils/__init__.py
 src/diffusers/utils/deprecation_utils.py
 src/diffusers/utils/dummy_flax_and_transformers_objects.py
 src/diffusers/utils/dummy_flax_objects.py
 src/diffusers/utils/dummy_pt_objects.py
-src/diffusers/utils/dummy_torch_and_accelerate_objects.py
 src/diffusers/utils/dummy_torch_and_scipy_objects.py
 src/diffusers/utils/dummy_torch_and_transformers_and_onnx_objects.py
 src/diffusers/utils/dummy_torch_and_transformers_objects.py
 src/diffusers/utils/import_utils.py
 src/diffusers/utils/logging.py
 src/diffusers/utils/model_card_template.md
 src/diffusers/utils/outputs.py
+src/diffusers/utils/pil_utils.py
 src/diffusers/utils/testing_utils.py
 src/diffusers_unchained.egg-info/PKG-INFO
 src/diffusers_unchained.egg-info/SOURCES.txt
 src/diffusers_unchained.egg-info/dependency_links.txt
 src/diffusers_unchained.egg-info/entry_points.txt
 src/diffusers_unchained.egg-info/requires.txt
 src/diffusers_unchained.egg-info/top_level.txt
```

### Comparing `diffusers-unchained-0.7.0/src/diffusers_unchained.egg-info/requires.txt` & `diffusers-unchained-0.9.0/src/diffusers_unchained.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 importlib_metadata
 filelock
 huggingface-hub>=0.10.0
 numpy
 regex!=2019.12.17
 requests
-Pillow<10.0
+Pillow
 
 [dev]
 black==22.8
 isort>=5.5.4
 flake8>=3.8.3
 hf-doc-builder>=0.3.0
 datasets
 parameterized
 pytest
 pytest-timeout
 pytest-xdist
+sentencepiece!=0.1.92,>=0.1.91
 scipy
 torchvision
 transformers>=4.21.0
 accelerate>=0.11.0
 tensorboard
 modelcards>=0.1.4
 torch>=1.4
@@ -43,14 +44,15 @@
 
 [test]
 datasets
 parameterized
 pytest
 pytest-timeout
 pytest-xdist
+sentencepiece!=0.1.92,>=0.1.91
 scipy
 torchvision
 transformers>=4.21.0
 
 [torch]
 torch>=1.4
 accelerate>=0.11.0
```

