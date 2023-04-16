# Comparing `tmp/hordelib-0.8.8.tar.gz` & `tmp/hordelib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.8.8.tar", last modified: Sat Apr 15 16:02:34 2023, max compression
+gzip compressed data, was "hordelib-0.9.0.tar", last modified: Sun Apr 16 22:23:13 2023, max compression
```

## Comparing `hordelib-0.8.8.tar` & `hordelib-0.9.0.tar`

### file list

```diff
@@ -1,886 +1,892 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.816554 hordelib-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-15 16:02:19.000000 hordelib-0.8.8/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-15 16:02:19.000000 hordelib-0.8.8/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.688553 hordelib-0.8.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.704553 hordelib-0.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-15 16:02:19.000000 hordelib-0.8.8/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-15 16:02:19.000000 hordelib-0.8.8/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-15 16:02:19.000000 hordelib-0.8.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-15 16:02:19.000000 hordelib-0.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-04-15 16:02:25.000000 hordelib-0.8.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-15 16:02:19.000000 hordelib-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-15 16:02:19.000000 hordelib-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-15 16:02:34.816554 hordelib-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-15 16:02:19.000000 hordelib-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-15 16:02:19.000000 hordelib-0.8.8/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.704553 hordelib-0.8.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 16:02:19.000000 hordelib-0.8.8/examples/run_upscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.708553 hordelib-0.8.8/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.708553 hordelib-0.8.8/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.712553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.716553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.720553 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38515 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.720553 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.720553 hordelib-0.8.8/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.724553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.724553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.724553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.692553 hordelib-0.8.8/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.728553 hordelib-0.8.8/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    43784 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.732553 hordelib-0.8.8/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    31347 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-15 16:02:27.000000 hordelib-0.8.8/hordelib/_comfyui/web/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.736554 hordelib-0.8.8/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.740553 hordelib-0.8.8/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.740553 hordelib-0.8.8/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28045 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.744553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.748554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.696553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.752554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.756554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.696553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.760554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.764554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.764554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.764554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.764554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.768554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.768554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.768554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.776554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.776554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.776554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.780554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.780554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.780554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.700553 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.784554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.788554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.792554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.792554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.796554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.796554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.796554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.796554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.800554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.804554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.804554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.804554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.804554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.804554 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.808554 hordelib-0.8.8/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.808554 hordelib-0.8.8/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.808554 hordelib-0.8.8/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.808554 hordelib-0.8.8/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 16:02:19.000000 hordelib-0.8.8/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.708553 hordelib-0.8.8/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49297 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 16:02:34.000000 hordelib-0.8.8/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.812554 hordelib-0.8.8/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-15 16:02:19.000000 hordelib-0.8.8/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-15 16:02:27.000000 hordelib-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 16:02:19.000000 hordelib-0.8.8/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 16:02:27.000000 hordelib-0.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 16:02:34.816554 hordelib-0.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.816554 hordelib-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:02:34.816554 hordelib-0.8.8/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-15 16:02:19.000000 hordelib-0.8.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-15 16:02:19.000000 hordelib-0.8.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.590484 hordelib-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 22:22:51.000000 hordelib-0.9.0/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-16 22:22:51.000000 hordelib-0.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.462473 hordelib-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.474474 hordelib-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-16 22:22:51.000000 hordelib-0.9.0/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-16 22:22:51.000000 hordelib-0.9.0/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-16 22:22:51.000000 hordelib-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-16 22:22:51.000000 hordelib-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    22172 2023-04-16 22:23:01.000000 hordelib-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-16 22:22:51.000000 hordelib-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-16 22:22:51.000000 hordelib-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-16 22:23:13.590484 hordelib-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-16 22:22:51.000000 hordelib-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-16 22:22:51.000000 hordelib-0.9.0/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.478474 hordelib-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 22:22:51.000000 hordelib-0.9.0/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.478474 hordelib-0.9.0/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.482475 hordelib-0.9.0/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.482475 hordelib-0.9.0/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.486475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37813 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.490475 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.494476 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38722 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.494476 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.494476 hordelib-0.9.0/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.498476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.498476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.498476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.466473 hordelib-0.9.0/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.502476 hordelib-0.9.0/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    43898 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.506477 hordelib-0.9.0/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/keybinds.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/noteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   482237 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/_comfyui/web/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/types/comfy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-16 22:23:04.000000 hordelib-0.9.0/hordelib/_comfyui/web/types/litegraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.510477 hordelib-0.9.0/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.514478 hordelib-0.9.0/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.514478 hordelib-0.9.0/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.514478 hordelib-0.9.0/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.518478 hordelib-0.9.0/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/model_manager/torch_hijack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.518478 hordelib-0.9.0/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.522478 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.526479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.466473 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.530479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.530479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.534479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.534479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.470474 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.534479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.534479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.534479 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.538480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.538480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.538480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.542480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.542480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.542480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.542480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.542480 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.550481 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.550481 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.554481 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.554481 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.558482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.558482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.558482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.558482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.558482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.470474 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.562482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.566482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.566482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.566482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.566482 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.570483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.570483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.570483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.574483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.578483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.578483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.578483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.578483 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.578483 hordelib-0.9.0/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.582484 hordelib-0.9.0/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.582484 hordelib-0.9.0/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.582484 hordelib-0.9.0/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 22:22:51.000000 hordelib-0.9.0/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.482475 hordelib-0.9.0/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50204 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49507 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 22:23:13.000000 hordelib-0.9.0/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.586484 hordelib-0.9.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-16 22:22:51.000000 hordelib-0.9.0/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-16 22:23:04.000000 hordelib-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-16 22:22:51.000000 hordelib-0.9.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 22:23:04.000000 hordelib-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:23:13.590484 hordelib-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.590484 hordelib-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:23:13.590484 hordelib-0.9.0/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 22:22:51.000000 hordelib-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-16 22:22:51.000000 hordelib-0.9.0/tox.ini
```

### Comparing `hordelib-0.8.8/.changelog` & `hordelib-0.9.0/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/.github/workflows/maintests.yml` & `hordelib-0.9.0/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/.github/workflows/prtests.yml` & `hordelib-0.9.0/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/.github/workflows/release.yml` & `hordelib-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/.gitignore` & `hordelib-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/CHANGELOG.md` & `hordelib-0.9.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ## hordelib Changelog
 
+## [v0.9.0](https://github.com/jug-dev/hordelib/compare/v0.8.8...v0.9.0)
+
+16 April 2023
+
+- feat: active memory and model management [`#144`](https://github.com/jug-dev/hordelib/pull/144) (Jug)
+
 ## [v0.8.8](https://github.com/jug-dev/hordelib/compare/v0.8.7...v0.8.8)
 
 15 April 2023
 
 - fix: Make thread locking as minimalist as possible [`#142`](https://github.com/jug-dev/hordelib/pull/142) (Jug)
 - fix: fix broken stress test [`be9567e`](https://github.com/jug-dev/hordelib/commit/be9567e8935f6016a607ad7de58522d2d84b21f7)  (Jug)
```

### Comparing `hordelib-0.8.8/LICENSE` & `hordelib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/PKG-INFO` & `hordelib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.8.8
+Version: 0.9.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -906,17 +906,17 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-We need to patch the ComfyUI source code. It's only a small patch to:
+We patch the ComfyUI source code to:
 
-1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+1. Modify the model manager to allow us to dynamically move models between VRAM, RAM and disk cache.
 2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
```

### Comparing `hordelib-0.8.8/README.md` & `hordelib-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -227,17 +227,17 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-We need to patch the ComfyUI source code. It's only a small patch to:
+We patch the ComfyUI source code to:
 
-1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+1. Modify the model manager to allow us to dynamically move models between VRAM, RAM and disk cache.
 2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
```

### Comparing `hordelib-0.8.8/build_helper.py` & `hordelib-0.9.0/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_controlnet.py` & `hordelib-0.9.0/examples/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_controlnet_annotator.py` & `hordelib-0.9.0/examples/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_facefix.py` & `hordelib-0.9.0/examples/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_img2img.py` & `hordelib-0.9.0/examples/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_img2img_hires.py` & `hordelib-0.9.0/examples/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_img2img_inpaint.py` & `hordelib-0.9.0/examples/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_img2img_inpaint_mask.py` & `hordelib-0.9.0/examples/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_img2img_outpaint.py` & `hordelib-0.9.0/examples/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_inpainting.py` & `hordelib-0.9.0/examples/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_stress_test.py` & `hordelib-0.9.0/examples/run_stress_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 SharedModelManager.manager.load("Papercutcraft")
 
 models = ["Deliberate", "Anything Diffusion", "Realistic Vision", "Papercutcraft"]
 cnets = ["openpose", "canny", "fakescribbes", "hed", "depth"]
 
 start_time = time.time()
 
-ITERATIONS = 5
+ITERATIONS = 1
 CONTROL_NET = True
 
 mutex = threading.Lock()
 count = 0
 
 
 def inc():
@@ -193,14 +193,18 @@
         threading.Thread(daemon=True, target=run_iterations),
         threading.Thread(daemon=True, target=run_iterations),
         threading.Thread(daemon=True, target=run_iterations),
     ]
     [x.start() for x in threads]
     [x.join() for x in threads if x]
 
-    expected_iterations = ITERATIONS * 5
+    expected_iterations = (ITERATIONS * 5) * len(threads)
     logger.warning(f"Test took {round(time.time() - start_time)} seconds ({count} generations)")
     if expected_iterations != count:
         logger.error("Test did not finsihed all iterations")
 
 
 main()
+
+# 275 seconds, 3 threads, 5 iterations, 5 tests = 3.6 seconds per gen
+# 311 seconds, 3 threads, 5 iterations, 5 tests, 1 at a time (mutex locked) = 4.14
+# 265 seconds, 3 threads, 5 iterations, 5 tests, sampler_mutex = 3.5 seconds per gen
```

### Comparing `hordelib-0.8.8/examples/run_txt2img.py` & `hordelib-0.9.0/examples/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_txt2img_hires.py` & `hordelib-0.9.0/examples/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/examples/run_upscale.py` & `hordelib-0.9.0/examples/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/LICENSE` & `hordelib-0.9.0/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/README.md` & `hordelib-0.9.0/hordelib/_comfyui/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,22 +28,36 @@
 - Starts up very fast.
 - Works fully offline: will never download anything.
 - [Config file](extra_model_paths.yaml.example) to set the search paths for models.
 
 Workflow examples can be found on the [Examples page](https://comfyanonymous.github.io/ComfyUI_examples/)
 
 ## Shortcuts
-- **Ctrl + A** select all nodes
-- **Ctrl + M** mute/unmute selected nodes
-- **Delete** or **Backspace** delete selected nodes
-- **Space** Holding space key while moving the cursor moves the canvas around. It works when holding the mouse button down so it is easier to connect different nodes when the canvas gets too large.
-- **Ctrl/Shift + Click** Add clicked node to selection.
-- **Ctrl + C/Ctrl + V** - Copy and paste selected nodes, without maintaining the connection to the outputs of unselected nodes.
-- **Ctrl + C/Ctrl + Shift + V** - Copy and paste selected nodes, and maintaining the connection from the outputs of unselected nodes to the inputs of the newly pasted nodes.
-- Holding **Shift** and drag selected nodes - Move multiple selected nodes at the same time.
+
+| Keybind | Explanation |
+| - | - |
+| Ctrl + Enter | Queue up current graph for generation |
+| Ctrl + Shift + Enter | Queue up current graph as first for generation |
+| Ctrl + S | Save workflow |
+| Ctrl + O | Load workflow |
+| Ctrl + A | Select all nodes |
+| Ctrl + M | Mute/unmute selected nodes |
+| Delete/Backspace | Delete selected nodes |
+| Ctrl + Delete/Backspace | Delete the current graph |
+| Space | Move the canvas around when held and moving the cursor |
+| Ctrl/Shift + Click | Add clicked node to selection |
+| Ctrl + C/Ctrl + V | Copy and paste selected nodes (without maintaining connections to outputs of unselected nodes) |
+| Ctrl + C/Ctrl + Shift + V| Copy and paste selected nodes (maintaining connections from outputs of unselected nodes to inputs of pasted nodes) |
+| Shift + Drag | Move multiple selected nodes at the same time |
+| Ctrl + D | Load default graph |
+| Q | Toggle visibility of the queue |
+| H | Toggle visibility of history |
+| R | Refresh graph |
+
+Ctrl can also be replaced with Cmd instead for MacOS users
 
 # Installing
 
 ## Windows
 
 There is a portable standalone build for Windows that should work for running on Nvidia GPUs or for running on your CPU only on the [releases page](https://github.com/comfyanonymous/ComfyUI/releases).
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from torch import nn, einsum
 from einops import rearrange, repeat
 from typing import Optional, Any
 
 from ldm.modules.diffusionmodules.util import checkpoint
 from .sub_quadratic_attention import efficient_dot_product_attention
 
-import model_management
+from comfy import model_management
 
 from . import tomesd
 
 if model_management.xformers_enabled():
     import xformers
     import xformers.ops
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import torch.nn as nn
 import numpy as np
 from einops import rearrange
 from typing import Optional, Any
 
 from ldm.modules.attention import MemoryEfficientCrossAttention
-import model_management
+from comfy import model_management
 
 if model_management.xformers_enabled_vae():
     import xformers
     import xformers.ops
 
 def get_timestep_embedding(timesteps, embedding_dim):
     """
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except ImportError:
 	from typing import Optional, NamedTuple, List
 	from typing_extensions import Protocol
 
 from torch import Tensor
 from typing import List
 
-import model_management
+from comfy import model_management
 
 def dynamic_slice(
     x: Tensor,
     starts: List[int],
     sizes: List[int],
 ) -> Tensor:
     slicing = [slice(start, start + size) for start, size in zip(starts, sizes)]
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/model_management.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/model_management.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import psutil
 from enum import Enum
 from cli_args import args
 import threading
+from loguru import logger
 
 class VRAMState(Enum):
     CPU = 0
     NO_VRAM = 1
     LOW_VRAM = 2
     NORMAL_VRAM = 3
     HIGH_VRAM = 4
@@ -110,97 +111,138 @@
 
 if args.cpu:
     vram_state = VRAMState.CPU
 
 print(f"Set vram state to: {vram_state.name}")
 
 
-current_loaded_model = None
-current_gpu_controlnets = []
+class ModelManager:
+    _instance = None
+    _initialised = False
+    _mutex = threading.RLock()
+    sampler_mutex = threading.RLock()
+    system_reserved_vram_mb = 6 * 1024
+    user_reserved_vram_mb = 0
+
+    # We are a singleton
+    def __new__(cls):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+        return cls._instance
+
+    # We initialise only ever once (in the lifetime of the singleton)
+    def __init__(self):
+        if not self._initialised:
+            self.models_in_use = []
+            self.current_loaded_models = []
+            self.current_gpu_controlnets = []
+            self.models_accelerated = []
+            self.__class__._initialised = True    
+
+    def set_user_reserved_vram(self, vram_mb):
+        with self._mutex:
+            self.user_reserved_vram_mb = vram_mb
+
+    def get_models_on_gpu(self):
+        with self._mutex:
+            return self.current_loaded_models[:]
+
+    def model_in_use(self, model):
+        with self._mutex:
+            return model in self.models_in_use
+
+    def unload_model(self, model):
+        global vram_state
+        with self._mutex:
+            if model not in self.current_loaded_models:
+                logger.debug("Skip GPU unload as not on the GPU")
+                return
+
+            if model in self.models_in_use:
+                logger.debug("Not unloaded model as it is in use right now")
+                return
+
+            if model in self.models_accelerated:
+                accelerate.hooks.remove_hook_from_submodules(model.model)
+                self.models_accelerated.remove(model)
+
+            # Unload to RAM
+            model.model.cpu()
+            model.unpatch_model()
+            self.current_loaded_models.remove(model)
+
+    def done_with_model(self, model):
+        with self._mutex:
+            if model in self.models_in_use:
+                self.models_in_use.remove(model)
+
+    def load_model_gpu(self, model):
+        global vram_state
+
+        with self._mutex:
+
+            # Don't run out of vram
+            if self.current_loaded_models:
+                freemem = round(get_free_memory(get_torch_device()) / (1024 * 1024))
+                logger.debug(f"Free VRAM is: {freemem}MB ({len(self.current_loaded_models)} models loaded on GPU)")
+                if freemem < (self.system_reserved_vram_mb + self.user_reserved_vram_mb):
+                    # release the least used model
+                    self.unload_model(self.current_loaded_models[-1])
+                    freemem = round(get_free_memory(get_torch_device()) / (1024 * 1024))
+                    logger.debug(f"Unloaded a model, free VRAM is now: {freemem}MB ({len(self.current_loaded_models)} models loaded on GPU)")
+
+            if model in self.current_loaded_models:
+                # Move this model to the top of the list
+                self.current_loaded_models.insert(0, self.current_loaded_models.pop(self.current_loaded_models.index(model)))
+                return model
+            
+            try:
+                real_model = model.patch_model()
+            except Exception as e:
+                model.unpatch_model()
+                raise e
+            
+            self.current_loaded_models.insert(0, model)
+
+            if vram_state == VRAMState.CPU:
+                pass
+            elif vram_state == VRAMState.MPS:
+                mps_device = torch.device("mps")
+                real_model.to(mps_device)
+            elif vram_state == VRAMState.NORMAL_VRAM or vram_state == VRAMState.HIGH_VRAM:
+                if model in self.models_accelerated:
+                    self.models_accelerated.remove(model)
+                real_model.to(get_torch_device())
+            else:
+                if vram_state == VRAMState.NO_VRAM:
+                    device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "256MiB", "cpu": "16GiB"})
+                elif vram_state == VRAMState.LOW_VRAM:
+                    device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "{}MiB".format(total_vram_available_mb), "cpu": "16GiB"})
+
+                accelerate.dispatch_model(real_model, device_map=device_map, main_device=get_torch_device())
+                self.models_accelerated.append(model)
+            return model
+
+    def load_controlnet_gpu(self, models):        
+        global vram_state
+        with self._mutex:
+            if vram_state == VRAMState.CPU:
+                return
+
+            if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
+                #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
+                return
+
+            device = get_torch_device()
+            for m in models:
+                if m not in self.current_gpu_controlnets:
+                    self.current_gpu_controlnets.append(m.to(device))
 
-model_accelerated = False
 
-mutex = threading.RLock()
-
-def unload_model():
-    global current_loaded_model
-    global model_accelerated
-    global current_gpu_controlnets
-    global vram_state
-
-    if current_loaded_model is not None:
-        if model_accelerated:
-            accelerate.hooks.remove_hook_from_submodules(current_loaded_model.model)
-            model_accelerated = False
-
-        #never unload models from GPU on high vram
-        if vram_state != VRAMState.HIGH_VRAM:
-            current_loaded_model.model.cpu()
-        current_loaded_model.unpatch_model()
-        current_loaded_model = None
-
-    # if vram_state != VRAMState.HIGH_VRAM:
-    #     if len(current_gpu_controlnets) > 0:
-    #         for n in current_gpu_controlnets:
-    #             n.cpu()
-    #         current_gpu_controlnets = []
-
-
-def load_model_gpu(model):
-    global current_loaded_model
-    global vram_state
-    global model_accelerated
-
-    if model is current_loaded_model:
-        return
-    if model:
-        unload_model()
-    try:
-        real_model = model.patch_model()
-    except Exception as e:
-        model.unpatch_model()
-        raise e
-    current_loaded_model = model
-    if vram_state == VRAMState.CPU:
-        pass
-    elif vram_state == VRAMState.MPS:
-        mps_device = torch.device("mps")
-        real_model.to(mps_device)
-        pass
-    elif vram_state == VRAMState.NORMAL_VRAM or vram_state == VRAMState.HIGH_VRAM:
-        model_accelerated = False
-        real_model.to(get_torch_device())
-    else:
-        if vram_state == VRAMState.NO_VRAM:
-            device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "256MiB", "cpu": "16GiB"})
-        elif vram_state == VRAMState.LOW_VRAM:
-            device_map = accelerate.infer_auto_device_map(real_model, max_memory={0: "{}MiB".format(total_vram_available_mb), "cpu": "16GiB"})
-
-        accelerate.dispatch_model(real_model, device_map=device_map, main_device=get_torch_device())
-        model_accelerated = True
-    return current_loaded_model
-
-def load_controlnet_gpu(models):
-    global current_gpu_controlnets
-    global vram_state
-    if vram_state == VRAMState.CPU:
-        return
-
-    if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
-        #don't load controlnets like this if low vram because they will be loaded right before running and unloaded right after
-        return
-
-    for m in current_gpu_controlnets:
-        if m not in models:
-            m.cpu()
-
-    device = get_torch_device()
-    current_gpu_controlnets = []
-    for m in models:
-        current_gpu_controlnets.append(m.to(device))
+model_manager = ModelManager()
 
 
 def load_if_low_vram(model):
     global vram_state
     if vram_state == VRAMState.LOW_VRAM or vram_state == VRAMState.NO_VRAM:
         return model.to(get_torch_device())
     return model
@@ -306,14 +348,23 @@
     nvidia_16_series = ["1660", "1650", "1630", "T500", "T550", "T600"]
     for x in nvidia_16_series:
         if x in props.name:
             return False
 
     return True
 
+def soft_empty_cache():
+    global xpu_available
+    if xpu_available:
+        torch.xpu.empty_cache()
+    elif torch.cuda.is_available():
+        if torch.version.cuda: #This seems to make things worse on ROCm so I only do it for cuda
+            torch.cuda.empty_cache()
+            torch.cuda.ipc_collect()
+
 #TODO: might be cleaner to put this somewhere else
 import threading
 
 class InterruptProcessingException(Exception):
     pass
 
 interrupt_processing_mutex = threading.RLock()
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/samplers.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .k_diffusion import sampling as k_diffusion_sampling
 from .k_diffusion import external as k_diffusion_external
 from .extra_samplers import uni_pc
 import torch
 import contextlib
-import model_management
+from comfy import model_management
 from .ldm.models.diffusion.ddim import DDIMSampler
 from .ldm.modules.diffusionmodules.util import make_ddim_timesteps
 
 class CFGDenoiser(torch.nn.Module):
     def __init__(self, model):
         super().__init__()
         self.inner_model = model
@@ -493,55 +493,56 @@
             extra_args["cond_concat"] = cond_concat
 
         if sigmas[0] != self.sigmas[0] or (self.denoise is not None and self.denoise < 1.0):
             max_denoise = False
         else:
             max_denoise = True
 
-        with precision_scope(model_management.get_autocast_device(self.device)):
-            if self.sampler == "uni_pc":
-                samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask)
-            elif self.sampler == "uni_pc_bh2":
-                samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask, variant='bh2')
-            elif self.sampler == "ddim":
-                timesteps = []
-                for s in range(sigmas.shape[0]):
-                    timesteps.insert(0, self.model_wrap.sigma_to_t(sigmas[s]))
-                noise_mask = None
-                if denoise_mask is not None:
-                    noise_mask = 1.0 - denoise_mask
-                sampler = DDIMSampler(self.model, device=self.device)
-                sampler.make_schedule_timesteps(ddim_timesteps=timesteps, verbose=False)
-                z_enc = sampler.stochastic_encode(latent_image, torch.tensor([len(timesteps) - 1] * noise.shape[0]).to(self.device), noise=noise, max_denoise=max_denoise)
-                samples, _ = sampler.sample_custom(ddim_timesteps=timesteps,
-                                                     conditioning=positive,
-                                                     batch_size=noise.shape[0],
-                                                     shape=noise.shape[1:],
-                                                     verbose=False,
-                                                     unconditional_guidance_scale=cfg,
-                                                     unconditional_conditioning=negative,
-                                                     eta=0.0,
-                                                     x_T=z_enc,
-                                                     x0=latent_image,
-                                                     denoise_function=sampling_function,
-                                                     extra_args=extra_args,
-                                                     mask=noise_mask,
-                                                     to_zero=sigmas[-1]==0,
-                                                     end_step=sigmas.shape[0] - 1)
-
-            else:
-                extra_args["denoise_mask"] = denoise_mask
-                self.model_k.latent_image = latent_image
-                self.model_k.noise = noise
+        with model_management.model_manager.sampler_mutex:
+            with precision_scope(model_management.get_autocast_device(self.device)):
+                if self.sampler == "uni_pc":
+                    samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask)
+                elif self.sampler == "uni_pc_bh2":
+                    samples = uni_pc.sample_unipc(self.model_wrap, noise, latent_image, sigmas, sampling_function=sampling_function, max_denoise=max_denoise, extra_args=extra_args, noise_mask=denoise_mask, variant='bh2')
+                elif self.sampler == "ddim":
+                    timesteps = []
+                    for s in range(sigmas.shape[0]):
+                        timesteps.insert(0, self.model_wrap.sigma_to_t(sigmas[s]))
+                    noise_mask = None
+                    if denoise_mask is not None:
+                        noise_mask = 1.0 - denoise_mask
+                    sampler = DDIMSampler(self.model, device=self.device)
+                    sampler.make_schedule_timesteps(ddim_timesteps=timesteps, verbose=False)
+                    z_enc = sampler.stochastic_encode(latent_image, torch.tensor([len(timesteps) - 1] * noise.shape[0]).to(self.device), noise=noise, max_denoise=max_denoise)
+                    samples, _ = sampler.sample_custom(ddim_timesteps=timesteps,
+                                                        conditioning=positive,
+                                                        batch_size=noise.shape[0],
+                                                        shape=noise.shape[1:],
+                                                        verbose=False,
+                                                        unconditional_guidance_scale=cfg,
+                                                        unconditional_conditioning=negative,
+                                                        eta=0.0,
+                                                        x_T=z_enc,
+                                                        x0=latent_image,
+                                                        denoise_function=sampling_function,
+                                                        extra_args=extra_args,
+                                                        mask=noise_mask,
+                                                        to_zero=sigmas[-1]==0,
+                                                        end_step=sigmas.shape[0] - 1)
 
-                noise = noise * sigmas[0]
-
-                if latent_image is not None:
-                    noise += latent_image
-                if self.sampler == "dpm_fast":
-                    samples = k_diffusion_sampling.sample_dpm_fast(self.model_k, noise, sigma_min, sigmas[0], self.steps, extra_args=extra_args)
-                elif self.sampler == "dpm_adaptive":
-                    samples = k_diffusion_sampling.sample_dpm_adaptive(self.model_k, noise, sigma_min, sigmas[0], extra_args=extra_args)
                 else:
-                    samples = getattr(k_diffusion_sampling, "sample_{}".format(self.sampler))(self.model_k, noise, sigmas, extra_args=extra_args)
+                    extra_args["denoise_mask"] = denoise_mask
+                    self.model_k.latent_image = latent_image
+                    self.model_k.noise = noise
+
+                    noise = noise * sigmas[0]
+
+                    if latent_image is not None:
+                        noise += latent_image
+                    if self.sampler == "dpm_fast":
+                        samples = k_diffusion_sampling.sample_dpm_fast(self.model_k, noise, sigma_min, sigmas[0], self.steps, extra_args=extra_args)
+                    elif self.sampler == "dpm_adaptive":
+                        samples = k_diffusion_sampling.sample_dpm_adaptive(self.model_k, noise, sigma_min, sigmas[0], extra_args=extra_args)
+                    else:
+                        samples = getattr(k_diffusion_sampling, "sample_{}".format(self.sampler))(self.model_k, noise, sigmas, extra_args=extra_args)
 
         return samples.to(torch.float32)
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import contextlib
 import copy
 
 import sd1_clip
 import sd2_clip
-import model_management
+from comfy import model_management
 from .ldm.util import instantiate_from_config
 from .ldm.models.autoencoder import AutoencoderKL
 import yaml
 from .cldm import cldm
 from .t2i_adapter import adapter
 
 from . import utils
@@ -368,27 +368,33 @@
 
     def add_patches(self, patches, strength=1.0):
         return self.patcher.add_patches(patches, strength)
 
     def clip_layer(self, layer_idx):
         self.layer_idx = layer_idx
 
-    def encode(self, text):
+    def tokenize(self, text, return_word_ids=False):
+        return self.tokenizer.tokenize_with_weights(text, return_word_ids)
+
+    def encode_from_tokens(self, tokens):
         if self.layer_idx is not None:
             self.cond_stage_model.clip_layer(self.layer_idx)
-        tokens = self.tokenizer.tokenize_with_weights(text)
         try:
             self.patcher.patch_model()
             cond = self.cond_stage_model.encode_token_weights(tokens)
             self.patcher.unpatch_model()
         except Exception as e:
             self.patcher.unpatch_model()
             raise e
         return cond
 
+    def encode(self, text):
+        tokens = self.tokenize(text)
+        return self.encode_from_tokens(tokens)
+
 class VAE:
     def __init__(self, ckpt_path=None, scale_factor=0.18215, device=None, config=None):
         if config is None:
             #default SD1.x/SD2.x VAE parameters
             ddconfig = {'double_z': True, 'z_channels': 4, 'resolution': 256, 'in_channels': 3, 'out_ch': 3, 'ch': 128, 'ch_mult': [1, 2, 4, 4], 'num_res_blocks': 2, 'attn_resolutions': [], 'dropout': 0.0}
             self.first_stage_model = AutoencoderKL(ddconfig, {'target': 'torch.nn.Identity'}, 4, monitor="val/rec_loss", ckpt_path=ckpt_path)
         else:
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import sd1_clip
+from comfy import sd1_clip
 import torch
 import os
 
 class SD2ClipModel(sd1_clip.SD1ClipModel):
     def __init__(self, arch="ViT-H-14", device="cpu", max_length=77, freeze=True, layer="penultimate", layer_idx=None):
         textmodel_json_config = os.path.join(os.path.dirname(os.path.realpath(__file__)), "sd2_clip_config.json")
         super().__init__(device=device, freeze=freeze, textmodel_json_config=textmodel_json_config)
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-0.9.0/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy/utils.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_mask.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-0.9.0/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from comfy_extras.chainner_models import model_loading
-import model_management
+from comfy import model_management
 import torch
 import comfy.utils
 import folder_paths
 
 class UpscaleModelLoader:
     @classmethod
     def INPUT_TYPES(s):
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-0.9.0/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-0.9.0/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/execution.py` & `hordelib-0.9.0/hordelib/_comfyui/execution.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import heapq
 import traceback
 import gc
 
 import torch
 import nodes
 
+import comfy.model_management
+
 def get_input_data(inputs, class_def, unique_id, outputs={}, prompt={}, extra_data={}):
     valid_inputs = class_def.INPUT_TYPES()
     input_data_all = {}
     for x in inputs:
         input_data = inputs[x]
         if isinstance(input_data, list):
             input_unique_id = input_data[0]
@@ -198,18 +200,15 @@
                     self.old_prompt[x] = copy.deepcopy(prompt[x])
             finally:
                 self.server.last_node_id = None
                 if self.server.client_id is not None:
                     self.server.send_sync("executing", { "node": None }, self.server.client_id)
 
         gc.collect()
-        if torch.cuda.is_available():
-            if torch.version.cuda: #This seems to make things worse on ROCm so I only do it for cuda
-                torch.cuda.empty_cache()
-                torch.cuda.ipc_collect()
+        comfy.model_management.soft_empty_cache()
 
 
 def validate_inputs(prompt, item):
     unique_id = item
     inputs = prompt[unique_id]['inputs']
     class_type = prompt[unique_id]['class_type']
     obj_class = nodes.NODE_CLASS_MAPPINGS[class_type]
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-0.9.0/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files 19% similar despite different names*

```diff
@@ -14,10 +14,10 @@
                   models/SwinIR
     embeddings: embeddings
     controlnet: models/ControlNet
 
 #other_ui:
 #    base_path: path/to/ui
 #    checkpoints: models/checkpoints
-
+#    custom_nodes: path/custom_nodes
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/folder_paths.py` & `hordelib-0.9.0/hordelib/_comfyui/folder_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,33 @@
     supported_pt_extensions.add('.safetensors')
 except:
     print("Could not import safetensors, safetensors support disabled.")
 
 
 folder_names_and_paths = {}
 
-
-models_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "models")
+base_path = os.path.dirname(os.path.realpath(__file__))
+models_dir = os.path.join(base_path, "models")
 folder_names_and_paths["checkpoints"] = ([os.path.join(models_dir, "checkpoints")], supported_ckpt_extensions)
 folder_names_and_paths["configs"] = ([os.path.join(models_dir, "configs")], [".yaml"])
 
 folder_names_and_paths["loras"] = ([os.path.join(models_dir, "loras")], supported_pt_extensions)
 folder_names_and_paths["vae"] = ([os.path.join(models_dir, "vae")], supported_pt_extensions)
 folder_names_and_paths["clip"] = ([os.path.join(models_dir, "clip")], supported_pt_extensions)
 folder_names_and_paths["clip_vision"] = ([os.path.join(models_dir, "clip_vision")], supported_pt_extensions)
 folder_names_and_paths["style_models"] = ([os.path.join(models_dir, "style_models")], supported_pt_extensions)
 folder_names_and_paths["embeddings"] = ([os.path.join(models_dir, "embeddings")], supported_pt_extensions)
 folder_names_and_paths["diffusers"] = ([os.path.join(models_dir, "diffusers")], ["folder"])
 
 folder_names_and_paths["controlnet"] = ([os.path.join(models_dir, "controlnet"), os.path.join(models_dir, "t2i_adapter")], supported_pt_extensions)
 folder_names_and_paths["upscale_models"] = ([os.path.join(models_dir, "upscale_models")], supported_pt_extensions)
 
+folder_names_and_paths["custom_nodes"] = ([os.path.join(base_path, "custom_nodes")], [])
+
+
 output_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "output")
 temp_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "temp")
 input_directory = os.path.join(os.path.dirname(os.path.realpath(__file__)), "input")
 
 if not os.path.exists(input_directory):
     os.makedirs(input_directory)
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/input/example.png` & `hordelib-0.9.0/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/main.py` & `hordelib-0.9.0/hordelib/_comfyui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,32 +77,33 @@
     cleanup_temp()
 
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     server = server.PromptServer(loop)
     q = execution.PromptQueue(server)
 
+    extra_model_paths_config_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extra_model_paths.yaml")
+    if os.path.isfile(extra_model_paths_config_path):
+        load_extra_path_config(extra_model_paths_config_path)
+
+    if args.extra_model_paths_config:
+        for config_path in itertools.chain(*args.extra_model_paths_config):
+            load_extra_path_config(config_path)
+
     init_custom_nodes()
     load_custom_nodes(os.getenv("AIWORKER_CUSTOM_NODES"))
     server.add_routes()
     hijack_progress(server)
 
     threading.Thread(target=prompt_worker, daemon=True, args=(q,server,)).start()
 
     address = args.listen
 
     dont_print = args.dont_print_server
 
-    extra_model_paths_config_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extra_model_paths.yaml")
-    if os.path.isfile(extra_model_paths_config_path):
-        load_extra_path_config(extra_model_paths_config_path)
-
-    if args.extra_model_paths_config:
-        for config_path in itertools.chain(*args.extra_model_paths_config):
-            load_extra_path_config(config_path)
 
     if args.output_directory:
         output_dir = os.path.abspath(args.output_directory)
         print(f"Setting output directory to: {output_dir}")
         folder_paths.set_output_directory(output_dir)
 
     port = args.port
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-0.9.0/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/nodes.py` & `hordelib-0.9.0/hordelib/_comfyui/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 import comfy.diffusers_convert
 import comfy.samplers
 import comfy.sd
 import comfy.utils
 
 import comfy.clip_vision
 
-import model_management
+import comfy.model_management
 import importlib
 
 import folder_paths
 
 def before_node_execution():
-    model_management.throw_exception_if_processing_interrupted()
+    comfy.model_management.throw_exception_if_processing_interrupted()
 
 def interrupt_processing(value=True):
-    model_management.interrupt_current_processing(value)
+    comfy.model_management.interrupt_current_processing(value)
 
 MAX_RESOLUTION=8192
 
 class CLIPTextEncode:
     @classmethod
     def INPUT_TYPES(s):
         return {"required": {"text": ("STRING", {"multiline": True}), "clip": ("CLIP", )}}
@@ -237,15 +237,15 @@
         for search_path in folder_paths.get_folder_paths("diffusers"):
             if os.path.exists(search_path):
                 paths = next(os.walk(search_path))[1]
                 if model_path in paths:
                     model_path = os.path.join(search_path, model_path)
                     break
 
-        return comfy.diffusers_convert.load_diffusers(model_path, fp16=model_management.should_use_fp16(), output_vae=output_vae, output_clip=output_clip, embedding_directory=folder_paths.get_folder_paths("embeddings"))
+        return comfy.diffusers_convert.load_diffusers(model_path, fp16=comfy.model_management.should_use_fp16(), output_vae=output_vae, output_clip=output_clip, embedding_directory=folder_paths.get_folder_paths("embeddings"))
 
 
 class unCLIPCheckpointLoader:
     @classmethod
     def INPUT_TYPES(s):
         return {"required": { "ckpt_name": (folder_paths.get_filename_list("checkpoints"), ),
                              }}
@@ -674,18 +674,17 @@
     def set_mask(self, samples, mask):
         s = samples.copy()
         s["noise_mask"] = mask
         return (s,)
 
 
 def common_ksampler(model, seed, steps, cfg, sampler_name, scheduler, positive, negative, latent, denoise=1.0, disable_noise=False, start_step=None, last_step=None, force_full_denoise=False):
-    model_management.mutex.acquire()
     latent_image = latent["samples"]
     noise_mask = None
-    device = model_management.get_torch_device()
+    device = comfy.model_management.get_torch_device()
 
     if disable_noise:
         noise = torch.zeros(latent_image.size(), dtype=latent_image.dtype, layout=latent_image.layout, device="cpu")
     else:
         noise = torch.randn(latent_image.size(), dtype=latent_image.dtype, layout=latent_image.layout, generator=torch.manual_seed(seed), device="cpu")
 
     if "noise_mask" in latent:
@@ -693,15 +692,16 @@
         noise_mask = torch.nn.functional.interpolate(noise_mask[None,None,], size=(noise.shape[2], noise.shape[3]), mode="bilinear")
         noise_mask = noise_mask.round()
         noise_mask = torch.cat([noise_mask] * noise.shape[1], dim=1)
         noise_mask = torch.cat([noise_mask] * noise.shape[0])
         noise_mask = noise_mask.to(device)
 
     real_model = None
-    model_management.load_model_gpu(model)
+    comfy.model_management.model_manager.model_in_use(model)
+    comfy.model_management.model_manager.load_model_gpu(model)
     real_model = model.model
 
     noise = noise.to(device)
     latent_image = latent_image.to(device)
 
     positive_copy = []
     negative_copy = []
@@ -723,30 +723,30 @@
         if 'control' in n[1]:
             control_nets += [n[1]['control']]
         negative_copy += [[t] + n[1:]]
 
     control_net_models = []
     for x in control_nets:
         control_net_models += x.get_control_models()
-    model_management.load_controlnet_gpu(control_net_models)
+    comfy.model_management.model_manager.load_controlnet_gpu(control_net_models)
 
     if sampler_name in comfy.samplers.KSampler.SAMPLERS:
         sampler = comfy.samplers.KSampler(real_model, steps=steps, device=device, sampler=sampler_name, scheduler=scheduler, denoise=denoise, model_options=model.model_options)
     else:
         #other samplers
         pass
 
     samples = sampler.sample(noise, positive_copy, negative_copy, cfg=cfg, latent_image=latent_image, start_step=start_step, last_step=last_step, force_full_denoise=force_full_denoise, denoise_mask=noise_mask)
     samples = samples.cpu()
     for c in control_nets:
         c.cleanup()
 
     out = latent.copy()
     out["samples"] = samples
-    model_management.mutex.release()
+    comfy.model_management.model_manager.done_with_model(model)
     return (out, )
 
 class KSampler:
     @classmethod
     def INPUT_TYPES(s):
         return {"required":
                     {"model": ("MODEL",),
@@ -1175,25 +1175,24 @@
                 NODE_DISPLAY_NAME_MAPPINGS.update(module.NODE_DISPLAY_NAME_MAPPINGS)
         else:
             print(f"Skip {module_path} module for custom nodes due to the lack of NODE_CLASS_MAPPINGS.")
     except Exception as e:
         print(traceback.format_exc())
         print(f"Cannot import {module_path} module for custom nodes:", e)
 
-def load_custom_nodes(path=os.path.join(os.path.dirname(os.path.realpath(__file__)), "custom_nodes")):
-    if not path:
-        return
-    CUSTOM_NODE_PATH = path
-    possible_modules = os.listdir(CUSTOM_NODE_PATH)
-    if "__pycache__" in possible_modules:
-        possible_modules.remove("__pycache__")
-
-    for possible_module in possible_modules:
-        module_path = os.path.join(CUSTOM_NODE_PATH, possible_module)
-        if os.path.isfile(module_path) and os.path.splitext(module_path)[1] != ".py": continue
-        load_custom_node(module_path)
+def load_custom_nodes():
+    node_paths = folder_paths.get_folder_paths("custom_nodes")
+    for custom_node_path in node_paths:
+        possible_modules = os.listdir(custom_node_path)
+        if "__pycache__" in possible_modules:
+            possible_modules.remove("__pycache__")
+
+        for possible_module in possible_modules:
+            module_path = os.path.join(custom_node_path, possible_module)
+            if os.path.isfile(module_path) and os.path.splitext(module_path)[1] != ".py": continue
+            load_custom_node(module_path)
 
 def init_custom_nodes():
     load_custom_nodes()
     load_custom_node(os.path.join(os.path.join(os.path.dirname(os.path.realpath(__file__)), "comfy_extras"), "nodes_upscale_model.py"))
     load_custom_node(os.path.join(os.path.join(os.path.dirname(os.path.realpath(__file__)), "comfy_extras"), "nodes_post_processing.py"))
     load_custom_node(os.path.join(os.path.join(os.path.dirname(os.path.realpath(__file__)), "comfy_extras"), "nodes_mask.py"))
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-0.9.0/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-0.9.0/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/server.py` & `hordelib-0.9.0/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -170,17 +170,19 @@
         // Double click a widget input to automatically attach a primitive
         const origOnInputDblClick = nodeType.prototype.onInputDblClick;
         const ignoreDblClick = Symbol();
         nodeType.prototype.onInputDblClick = function(slot) {
             const r = origOnInputDblClick ? origOnInputDblClick.apply(this, arguments) : undefined;
 
             const input = this.inputs[slot];
-            if (!input.widget || !input[ignoreDblClick]) // Not a widget input or already handled input
-            {
-                if (!(input.type in ComfyWidgets)) return r; //also Not a ComfyWidgets input (do nothing)
+            if (!input.widget || !input[ignoreDblClick]) {
+                // Not a widget input or already handled input
+                if (!(input.type in ComfyWidgets) && !(input.widget.config?.[0] instanceof Array)) {
+                    return r; //also Not a ComfyWidgets input or combo (do nothing)
+                }
             }
 
             // Create a primitive node
             const node = LiteGraph.createNode("PrimitiveNode");
             app.graph.add(node);
 
             // Calculate a position that wont directly overlap another node
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-0.9.0/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/index.html` & `hordelib-0.9.0/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-0.9.0/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-0.9.0/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/api.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/app.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/app.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,35 +12,56 @@
     defaultGraph
 } from "./defaultGraph.js";
 import {
     getPngMetadata,
     importA1111
 } from "./pnginfo.js";
 
-class ComfyApp {
-    /** 
-     * List of {number, batchCount} entries to queue
+/** 
+ * @typedef {import("types/comfy").ComfyExtension} ComfyExtension
+ */
+
+export class ComfyApp {
+    /**
+     * List of entries to queue
+     * @type {{number: number, batchCount: number}[]}
      */
     #queueItems = [];
     /**
      * If the queue is currently being processed
+     * @type {boolean}
      */
     #processingQueue = false;
 
     constructor() {
         this.ui = new ComfyUI(this);
+
+        /**
+         * List of extensions that are registered with the app
+         * @type {ComfyExtension[]}
+         */
         this.extensions = [];
+
+        /**
+         * Stores the execution output data for each node
+         * @type {Record<string, any>}
+         */
         this.nodeOutputs = {};
+
+        /**
+         * If the shift key on the keyboard is pressed
+         * @type {boolean}
+         */
         this.shiftDown = false;
     }
 
     /**
      * Invoke an extension callback
-     * @param {string} method The extension callback to execute
-     * @param  {...any} args Any arguments to pass to the callback
+     * @param {keyof ComfyExtension} method The extension callback to execute
+     * @param  {any[]} args Any arguments to pass to the callback
      * @returns
      */
     #invokeExtensions(method, ...args) {
         let results = [];
         for (const ext of this.extensions) {
             if (method in ext) {
                 try {
@@ -719,19 +740,14 @@
 
         api.init();
     }
 
     #addKeyboardHandler() {
         window.addEventListener("keydown", (e) => {
             this.shiftDown = e.shiftKey;
-
-            // Queue prompt using ctrl or command + enter
-            if ((e.ctrlKey || e.metaKey) && (e.key === "Enter" || e.keyCode === 13 || e.keyCode === 10)) {
-                this.queuePrompt(e.shiftKey ? -1 : 0);
-            }
         });
         window.addEventListener("keyup", (e) => {
             this.shiftDown = e.shiftKey;
         });
     }
 
     /**
@@ -1167,14 +1183,18 @@
             reader.onload = () => {
                 this.loadGraphData(JSON.parse(reader.result));
             };
             reader.readAsText(file);
         }
     }
 
+    /**
+     * Registers a Comfy web extension with the app
+     * @param {ComfyExtension} extension
+     */
     registerExtension(extension) {
         if (!extension.name) {
             throw new Error("Extensions must have a 'name' property.");
         }
         if (this.extensions.find((ext) => ext.name === extension.name)) {
             throw new Error(`Extension named '${extension.name}' already registered.`);
         }
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/ui.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -458,15 +458,23 @@
         const confirmClear = this.settings.addSetting({
             id: "Comfy.ConfirmClear",
             name: "Require confirmation when clearing workflow",
             type: "boolean",
             defaultValue: true,
         });
 
+        const promptFilename = this.settings.addSetting({
+            id: "Comfy.PromptFilename",
+            name: "Prompt for filename when saving workflow",
+            type: "boolean",
+            defaultValue: true,
+        });
+
         const fileInput = $el("input", {
+            id: "comfy-file-input",
             type: "file",
             accept: ".json,image/png",
             style: {
                 display: "none"
             },
             parent: document.body,
             onchange: () => {
@@ -491,14 +499,15 @@
                 }),
                 $el("button.comfy-settings-btn", {
                     textContent: "⚙️",
                     onclick: () => this.settings.show()
                 }),
             ]),
             $el("button.comfy-queue-btn", {
+                id: "queue-button",
                 textContent: "Queue Prompt",
                 onclick: () => app.queuePrompt(0, this.batchCount),
             }),
             $el("div", {}, [
                 $el("label", {
                     innerHTML: "Extra options"
                 }, [
@@ -553,77 +562,93 @@
                         checked: false,
                         title: "automatically queue prompt when the queue size hits 0",
                     }),
                 ]),
             ]),
             $el("div.comfy-menu-btns", [
                 $el("button", {
+                    id: "queue-front-button",
                     textContent: "Queue Front",
                     onclick: () => app.queuePrompt(-1, this.batchCount)
                 }),
                 $el("button", {
                     $: (b) => (this.queue.button = b),
+                    id: "comfy-view-queue-button",
                     textContent: "View Queue",
                     onclick: () => {
                         this.history.hide();
                         this.queue.toggle();
                     },
                 }),
                 $el("button", {
                     $: (b) => (this.history.button = b),
+                    id: "comfy-view-history-button",
                     textContent: "View History",
                     onclick: () => {
                         this.queue.hide();
                         this.history.toggle();
                     },
                 }),
             ]),
             this.queue.element,
             this.history.element,
             $el("button", {
+                id: "comfy-save-button",
                 textContent: "Save",
                 onclick: () => {
+                    let filename = "workflow.json";
+                    if (promptFilename.value) {
+                        filename = prompt("Save workflow as:", filename);
+                        if (!filename) return;
+                        if (!filename.toLowerCase().endsWith(".json")) {
+                            filename += ".json";
+                        }
+                    }
                     const json = JSON.stringify(app.graph.serialize(), null, 2); // convert the data to a JSON string
                     const blob = new Blob([json], {
                         type: "application/json"
                     });
                     const url = URL.createObjectURL(blob);
                     const a = $el("a", {
                         href: url,
-                        download: "workflow.json",
+                        download: filename,
                         style: {
                             display: "none"
                         },
                         parent: document.body,
                     });
                     a.click();
                     setTimeout(function() {
                         a.remove();
                         window.URL.revokeObjectURL(url);
                     }, 0);
                 },
             }),
             $el("button", {
+                id: "comfy-load-button",
                 textContent: "Load",
                 onclick: () => fileInput.click()
             }),
             $el("button", {
+                id: "comfy-refresh-button",
                 textContent: "Refresh",
                 onclick: () => app.refreshComboInNodes()
             }),
             $el("button", {
+                id: "comfy-clear-button",
                 textContent: "Clear",
                 onclick: () => {
                     if (!confirmClear.value || confirm("Clear workflow?")) {
                         app.clean();
                         app.graph.clear();
                     }
                 }
             }),
             $el("button", {
+                id: "comfy-load-default-button",
                 textContent: "Load Default",
                 onclick: () => {
                     if (!confirmClear.value || confirm("Load default workflow?")) {
                         app.loadGraphData()
                     }
                 }
             }),
```

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-0.9.0/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/_comfyui/web/style.css` & `hordelib-0.9.0/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/blip/caption.py` & `hordelib-0.9.0/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/cache/cache.py` & `hordelib-0.9.0/hordelib/cache/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from pathlib import Path
 
 from loguru import logger
 from PIL import Image
 from tqdm import tqdm
 
-from hordelib.settings import WorkerSettings
+from hordelib.settings import UserSettings
 
 if sys.version_info < (3, 9):  # XXX is <3.9 support going to be a thing?
     import importlib_resources
 else:
     import importlib.resources as importlib_resources
 
 
@@ -78,15 +78,15 @@
         :param input_directory: Directory to list
         :param extensions: List of extensions to filter for
         :return: List of files
         """
         files = []
         for file in tqdm(
             os.listdir(input_directory),
-            disable=WorkerSettings.disable_progress.active,
+            disable=UserSettings.disable_progress.active,
         ):
             if os.path.splitext(file)[1] in extensions:
                 files.append(os.path.splitext(file)[0])
         return files
 
     def get_all(self):
         """
@@ -146,15 +146,15 @@
         """
         Hash all files in a directory
         :param input_directory: Directory to hash
         :return: List of hashes
         """
         pil_hashes = []
         file_hashes = []
-        for file in tqdm(files_list, disable=WorkerSettings.disable_progress.active):
+        for file in tqdm(files_list, disable=UserSettings.disable_progress.active):
             for extension in extensions:
                 file = file + extension
                 file_path = os.path.join(input_directory, file)
                 file_hash = self.hash_file(file_path)
                 pil_image_hash = self.hash_pil_image_file(file_path)
                 pil_hashes.append(pil_image_hash)
                 file_hashes.append(file_hash)
```

### Comparing `hordelib-0.8.8/hordelib/clip/bulk.py` & `hordelib-0.9.0/hordelib/clip/bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from loguru import logger
 from PIL import Image
 from tqdm import tqdm
 
 from hordelib.cache import Cache
 from hordelib.clip.image import ImageEmbed
 from hordelib.model_manager.clip import ClipModelManager
-from hordelib.settings import WorkerSettings
+from hordelib.settings import UserSettings
 
 
 class BulkImageEmbedder:
     def __init__(self):
         self.model_manager = None
         self.model_name = None
         self.image_embed = None
@@ -58,10 +58,10 @@
         logger.info(f"Reading from {input_directory}")
         directory_list = self.cache_image.list_dir(input_directory)
         logger.info(f"Found {len(directory_list)} files. Filtering...")
         filtered_list = self.cache_image.filter_list(directory_list)
         logger.info(f"Found {len(filtered_list)} files to embed.")
         for image in tqdm(
             filtered_list,
-            disable=WorkerSettings.disable_progress.active,
+            disable=UserSettings.disable_progress.active,
         ):
             self.insert(image, input_directory)
```

### Comparing `hordelib-0.8.8/hordelib/clip/coca.py` & `hordelib-0.9.0/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/image.py` & `hordelib-0.9.0/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/interrogate.py` & `hordelib-0.9.0/hordelib/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/artists.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/movements.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/tags.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-0.9.0/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/clip/text.py` & `hordelib-0.9.0/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/comfy_horde.py` & `hordelib-0.9.0/hordelib/comfy_horde.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 # comfy.py
 # Wrapper around comfy to allow usage by the horde worker.
 import contextlib
 import copy
+import gc
 import glob
 import json
 import os
 import re
 import time
-import threading
 import typing
 from pprint import pformat
 
+import torch
 from loguru import logger
 
+from hordelib.settings import UserSettings
 from hordelib.utils.ioredirect import OutputCollector
+from hordelib.config_path import get_hordelib_path
 
 # Note these imports are intentionally somewhat obfuscated as a reminder to other modules
 # that they should never call through this module into comfy directly. All calls into
 # comfy should be abstracted through functions in this module.
 # isort: off
 from execution import nodes as _comfy_nodes
 from execution import PromptExecutor as _comfy_PromptExecutor
+from folder_paths import folder_names_and_paths as _comfy_folder_paths
 from comfy.sd import load_checkpoint_guess_config as __comfy_load_checkpoint_guess_config
 from comfy.sd import load_controlnet as __comfy_load_controlnet
+from comfy.model_management import model_manager as _comfy_model_manager
 from comfy.utils import load_torch_file as __comfy_load_torch_file
 from comfy_extras.chainner_models import model_loading as _comfy_model_loading
 
 # isort: on
 
 
+def get_models_on_gpu():
+    return _comfy_model_manager.get_models_on_gpu()
+
+
+def unload_model_from_gpu(model):
+    _comfy_model_manager.unload_model(model)
+    gc.collect()
+    if torch.cuda.is_available():
+        if torch.version.cuda:  # This seems to make things worse on ROCm so I only do it for cuda
+            torch.cuda.empty_cache()
+            torch.cuda.ipc_collect()
+
+
+def is_model_in_use(model):
+    return _comfy_model_manager.model_in_use(model)
+
+
 def load_torch_file(filename):
     result = __comfy_load_torch_file(filename)
     return result
 
 
 def load_state_dict(state_dict):
     result = _comfy_model_loading.load_state_dict(state_dict)
@@ -46,22 +68,26 @@
     embeddings_path: str | None = None,
 ) -> dict[str, typing.Any]:  # XXX # FIXME 'any'
     # XXX Needs docstring
     # XXX # TODO One day this signature should be generic, and not comfy specific
     # XXX # This can remain a comfy call, but the rest of the code should be able
     # XXX # to pretend it isn't
     # Redirect IO
-    stdio = OutputCollector()
-    with contextlib.redirect_stdout(stdio):
-        (modelPatcher, clipModel, vae, clipVisionModel) = __comfy_load_checkpoint_guess_config(
-            ckpt_path=ckpt_path,
-            output_vae=output_vae,
-            output_clip=output_clip,
-            embedding_directory=embeddings_path,
-        )
+    try:
+        stdio = OutputCollector()
+        with contextlib.redirect_stdout(stdio):
+            (modelPatcher, clipModel, vae, clipVisionModel) = __comfy_load_checkpoint_guess_config(
+                ckpt_path=ckpt_path,
+                output_vae=output_vae,
+                output_clip=output_clip,
+                embedding_directory=embeddings_path,
+            )
+    except RuntimeError:
+        # Failed, hard to tell why, bad checkpoint, not enough ram, for example
+        raise
 
     return {
         "model": modelPatcher,
         "clip": clipModel,
         "vae": vae,
         "clipVisionModel": clipVisionModel,
     }
@@ -113,14 +139,16 @@
         "latent_upscale.height": (64, 8192),
     }
 
     def __init__(self) -> None:
         self.client_id = None  # used for receiving comfyUI async events
         self.pipelines = {}
         self.exit_time = 0
+        # Set custom node path
+        _comfy_folder_paths["custom_nodes"] = ([os.path.join(get_hordelib_path(), "nodes")], [])
         # Load our pipelines
         self._load_pipelines()
 
         stdio = OutputCollector()
         with contextlib.redirect_stdout(stdio):
             # Load our custom nodes
             self._load_custom_nodes()
@@ -130,15 +158,14 @@
         target_dir = os.path.dirname(os.path.realpath(__file__))
         if subdir:
             target_dir = os.path.join(target_dir, subdir)
         return os.path.join(target_dir, filename)
 
     def _load_custom_nodes(self) -> None:
         _comfy_nodes.init_custom_nodes()
-        _comfy_nodes.load_custom_nodes(self._this_dir("nodes"))
 
     def _get_executor(self, pipeline):
         executor = _comfy_PromptExecutor(self)
         return executor
 
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
@@ -313,14 +340,17 @@
     # For the horde we assume the pipeline returns an array of images.
     def run_pipeline(self, pipeline_name: str, params: dict) -> dict | None:
         # Sanity
         if pipeline_name not in self.pipelines:
             logger.error(f"Unknown inference pipeline: {pipeline_name}")
             return None
 
+        # Update user settings
+        _comfy_model_manager.set_user_reserved_vram(UserSettings.vram_to_leave_free_mb)
+
         logger.info(f"Running pipeline {pipeline_name}")
 
         # Grab a copy of the pipeline
         pipeline = copy.deepcopy(self.pipelines[pipeline_name])
 
         # Inject our model manager if required
         from hordelib.shared_model_manager import SharedModelManager
```

### Comparing `hordelib-0.8.8/hordelib/config_path.py` & `hordelib-0.9.0/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/consts.py` & `hordelib-0.9.0/hordelib/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # consts.py
 import os
 from enum import Enum, auto
 
 from hordelib.config_path import get_hordelib_path
 
-COMFYUI_VERSION = "7f23353d6382f974281ccc38097a93c831b38a9a"
+COMFYUI_VERSION = "74fc7b772656a59b344508480632d9d45f9127de"
 """The exact version of ComfyUI version to load."""
 
 REMOTE_MODEL_DB = "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/"
 """The default base endpoint where to find model databases. See MODEL_DB_NAMES for valid database names."""
 
 RELEASE_VERSION = os.path.exists(os.path.join(get_hordelib_path(), "_version.py"))
 """A flag for if this is a pypi release or a git dev mode"""
```

### Comparing `hordelib-0.8.8/hordelib/horde.py` & `hordelib-0.9.0/hordelib/horde.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/initialisation.py` & `hordelib-0.9.0/hordelib/initialisation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/install_comfy.py` & `hordelib-0.9.0/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/aitemplate.json` & `hordelib-0.9.0/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/blip.json` & `hordelib-0.9.0/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/clip.json` & `hordelib-0.9.0/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/controlnet.json` & `hordelib-0.9.0/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/db.json` & `hordelib-0.9.0/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/db_dep.json` & `hordelib-0.9.0/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/db_embeds.json` & `hordelib-0.9.0/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/diffusers.json` & `hordelib-0.9.0/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/esrgan.json` & `hordelib-0.9.0/hordelib/model_database/esrgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/gfpgan.json` & `hordelib-0.9.0/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/safety_checker.json` & `hordelib-0.9.0/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_database/stable_diffusion.json` & `hordelib-0.9.0/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/base.py` & `hordelib-0.9.0/hordelib/model_manager/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+import gc
 import hashlib
 import importlib.resources as importlib_resources
 import json
 import os
 import shutil
 import time
 import typing
 import zipfile
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any
 from uuid import uuid4
 
 import git
+import psutil
 import requests
 import torch
 from loguru import logger
 from tqdm import tqdm
 from transformers import logging
 
 from hordelib.cache import get_cache_directory
+from hordelib.comfy_horde import get_models_on_gpu, is_model_in_use, unload_model_from_gpu
 from hordelib.config_path import get_hordelib_path
 from hordelib.consts import REMOTE_MODEL_DB
-from hordelib.settings import WorkerSettings
+from hordelib.settings import UserSettings
 
 logging.set_verbosity_error()
 
 
 class BaseModelManager(ABC):
     modelFolderPath: str  # XXX # TODO Convert to `Path`
     """The path to the directory to store this model type."""
@@ -133,23 +136,68 @@
             logger.init_err(
                 "Model Reference",
                 status=f"Download failed: {e}",
             )
             logger.init_warn("Model Reference", status="Local")
             return json.loads((self.models_db_path).read_text())
 
+    def _modelref_to_name(self, modelref):
+        for name, data in self.loaded_models.items():
+            if modelref and data["model"] is modelref:
+                return name
+        return None
+
+    def ensure_memory_available(self):
+        # Can this type of model be cached?
+        if not self.can_cache_on_disk():
+            return
+        # If we have less than the minimum RAM free, free some up
+        freemem = round(psutil.virtual_memory().available / (1024 * 1024))
+        logger.debug(f"Free RAM is: {freemem} MB, ({len(self.loaded_models)} models loaded in RAM)")
+        if freemem > UserSettings.ram_to_leave_free_mb + 4096:
+            return
+        logger.debug(f"Not enough free RAM attempting to free some")
+        # Grab a list of models (ModelPatcher) that are loaded on the gpu
+        # These are actually returned with the least important at the bottom of the list
+        busy_models = get_models_on_gpu()
+        # Try to find one we have in ram that isn't on the gpu
+        idle_model = None
+        for ram_model_name, ram_model_data in self.loaded_models.items():
+            if type(ram_model_data["model"]) is not str and ram_model_data["model"] not in busy_models:
+                idle_model = ram_model_name
+                break
+        # If we didn't have one hanging around in ram not on the gpu
+        # pick the least used gpu model
+        if not idle_model and busy_models:
+            idle_model = self._modelref_to_name(busy_models[-1])
+
+        if idle_model:
+            logger.debug(f"Moving model {idle_model} to disk to free up RAM")
+            self.move_to_disk_cache(idle_model)
+        else:
+            # Nothing else to release
+            logger.debug(f"Could not find a model to free RAM")
+
+    def move_to_disk_cache(self, model_name):
+        pass
+
+    def can_cache_on_disk(self):
+        """Can this of type model be cached on disk?"""
+        return False
+
     def load(
         self,
         model_name: str,
         *,
         half_precision: bool = True,
         gpu_id: int | None = 0,
         cpu_only: bool = False,
         **kwargs,
     ):  # XXX # FIXME
+        self.ensure_memory_available()
         if model_name not in self.model_reference:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
             download_succeeded = self.download_model(model_name)
             if not download_succeeded:
@@ -161,21 +209,28 @@
             if not model_validated:
                 return False
             logger.init(f"{model_name}", status="Loading")
 
             tic = time.time()
             logger.init(f"{model_name}", status="Loading")
 
-            self.loaded_models[model_name] = self.modelToRam(
-                model_name=model_name,
-                half_precision=half_precision,
-                gpu_id=gpu_id,
-                cpu_only=cpu_only,
-                **kwargs,
-            )
+            try:
+                self.loaded_models[model_name] = self.modelToRam(
+                    model_name=model_name,
+                    half_precision=half_precision,
+                    gpu_id=gpu_id,
+                    cpu_only=cpu_only,
+                    **kwargs,
+                )
+
+            except RuntimeError:
+                # It failed, it happens.
+                logger.error(f"Failed to load model {model_name}")
+                return None
+
             toc = time.time()
 
             logger.init_ok(f"{model_name}: {round(toc-tic,2)} seconds", status="Loaded")
             return True
         return None
 
     def getFullModelPath(self, model_name: str):
@@ -243,15 +298,15 @@
     def count_available_models_by_types(self, model_types: list[str] | None = None):
         return len(self.get_available_models_by_types(model_types))
 
     def get_loaded_models(self):
         """
         Returns the loaded models
         """
-        return self.loaded_models
+        return self.loaded_models[:]
 
     def get_loaded_model(self, model_name: str):
         """
         :param model_name: Name of the model
         Returns the loaded model
         """
         return self.loaded_models[model_name]
@@ -277,30 +332,56 @@
             model_name (str): The name of the model to check.
 
         Returns:
             _type_: _description_
         """
         return model_name in self.loaded_models
 
+    def remove_model_from_ram(self, model_name):
+        if model_name not in self.loaded_models:
+            return
+        # Remove the model from ram. Just removing from the dictionary
+        # wasn't actually releasing the RAM
+        model = self.loaded_models[model_name]
+        del self.loaded_models[model_name]
+        if "model" in model:
+            del model["model"]
+        if "clip" in model:
+            del model["clip"]
+        if "vae" in model:
+            del model["vae"]
+        if "clipVisionModel" in model:
+            del model["clipVisionModel"]
+        del model
+        gc.collect()
+
     def unload_model(self, model_name: str):
         """
         :param model_name: Name of the model
-        Unloads a model
+        Unloads a model. Completely remove it, free all resources, forget it exists.
         """
         if model_name in self.loaded_models:
-            del self.loaded_models[model_name]
-            return True
-        return False
+            if not is_model_in_use(self.loaded_models[model_name]["model"]):
+                # Unload it from the GPU if it has been loaded there
+                try:
+                    unload_model_from_gpu(self.loaded_models[model_name]["model"])
+                    # Free it's ram
+                    self.remove_model_from_ram(model_name)
+                    return True
+                except Exception as e:
+                    logger.warning(f"Failed to unload model {model_name}: {e}")
+                    return False
+        return None
 
     def unload_all_models(self):
         """
         Unloads all models
         """
         for model in self.loaded_models:
-            del self.loaded_models[model]
+            self.unload_model(model)
         return True
 
     def taint_model(self, model_name: str):
         """Marks a model as not valid by removing it from available_models"""
         if model_name in self.available_models:
             self.available_models.remove(model_name)
             self.tainted_models.append(model_name)
@@ -486,15 +567,15 @@
                 # all optional kwargs
                 unit="B",
                 unit_scale=True,
                 unit_divisor=1024,
                 miniters=1,
                 desc=pbar_desc,
                 total=int(response.headers.get("content-length", 0)),
-                disable=WorkerSettings.disable_download_progress.active,
+                disable=UserSettings.disable_download_progress.active,
             ) as pbar:
                 for chunk in response.iter_content(chunk_size=16 * 1024):
                     response.raise_for_status()
                     if chunk:
                         f.write(chunk)
                         pbar.update(len(chunk))
             return True
```

### Comparing `hordelib-0.8.8/hordelib/model_manager/blip.py` & `hordelib-0.9.0/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/clip.py` & `hordelib-0.9.0/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/codeformer.py` & `hordelib-0.9.0/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/compvis.py` & `hordelib-0.9.0/hordelib/model_manager/diffusers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-import os
 import typing
 
 from typing_extensions import override
 
 from hordelib.comfy_horde import horde_load_checkpoint
-from hordelib.consts import (
-    MODEL_CATEGORY_NAMES,
-    MODEL_DB_NAMES,
-    MODEL_FOLDER_NAMES,
-)
+from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
+# from nataili.util.voodoo import push_diffusers_pipeline_to_plasma
 
-class CompVisModelManager(BaseModelManager):
-    def __init__(
-        self,
-        download_reference=False,
-        # custom_path="models/custom",  # XXX Remove this and any others like it?
-    ):
+
+class DiffusersModelManager(BaseModelManager):
+    def __init__(self, download_reference=False):
         super().__init__(
-            modelFolder=MODEL_FOLDER_NAMES[MODEL_CATEGORY_NAMES.compvis],
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.compvis],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.diffusers],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
-
-        embeddings_path = os.getenv("HORDE_MODEL_DIR_EMBEDDINGS", "./")
-
         return horde_load_checkpoint(
             ckpt_path=self.getFullModelPath(model_name),
-            embeddings_path=embeddings_path,
         )
```

### Comparing `hordelib-0.8.8/hordelib/model_manager/controlnet.py` & `hordelib-0.9.0/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/diffusers.py` & `hordelib-0.9.0/hordelib/model_manager/esrgan.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import typing
 
-from typing_extensions import override
+from typing_extensions import override  # noqa: I001
 
-from hordelib.comfy_horde import horde_load_checkpoint
+from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
-# from nataili.util.voodoo import push_diffusers_pipeline_to_plasma
 
-
-class DiffusersModelManager(BaseModelManager):
+class EsrganModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.diffusers],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.esrgan],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
         **kwargs,
     ) -> dict[str, typing.Any]:
-        return horde_load_checkpoint(
-            ckpt_path=self.getFullModelPath(model_name),
-        )
+        model_path = self.getFullModelPath(model_name)
+        sd = comfy_horde.load_torch_file(model_path)
+        out = comfy_horde.load_state_dict(sd).eval()
+        return {"model": out}
```

### Comparing `hordelib-0.8.8/hordelib/model_manager/esrgan.py` & `hordelib-0.9.0/hordelib/model_manager/gfpgan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing
 
-from typing_extensions import override  # noqa: I001
+from typing_extensions import override
 
 from hordelib import comfy_horde
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
 from hordelib.model_manager.base import BaseModelManager
 
 
-class EsrganModelManager(BaseModelManager):
+class GfpganModelManager(BaseModelManager):
     def __init__(self, download_reference=False):
         super().__init__(
-            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.esrgan],
+            models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.gfpgan],
             download_reference=download_reference,
         )
 
     @override
     def modelToRam(
         self,
         model_name: str,
```

### Comparing `hordelib-0.8.8/hordelib/model_manager/safety_checker.py` & `hordelib-0.9.0/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/model_manager/torch_hijack.py` & `hordelib-0.9.0/hordelib/model_manager/torch_hijack.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.9.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.9.0/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.9.0/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.9.0/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/node_image_loader.py` & `hordelib-0.9.0/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/node_image_output.py` & `hordelib-0.9.0/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.9.0/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.9.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.9.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/run_comfyui.py` & `hordelib-0.9.0/hordelib/run_comfyui.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/safety_checker.py` & `hordelib-0.9.0/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/shared_model_manager.py` & `hordelib-0.9.0/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/blip/blip.py` & `hordelib-0.9.0/hordelib/utils/blip/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/blip/med.py` & `hordelib-0.9.0/hordelib/utils/blip/med.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/blip/vit.py` & `hordelib-0.9.0/hordelib/utils/blip/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/cast.py` & `hordelib-0.9.0/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/ioredirect.py` & `hordelib-0.9.0/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/hordelib/utils/logger.py` & `hordelib-0.9.0/hordelib/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
                 {
                     "sink": "logs/bridge.log",
                     "format": cls.logfmt,
                     "level": "DEBUG",
                     "colorize": False,
                     "filter": cls.is_not_stats_log,
                     "retention": "2 days",
-                    "rotation": "3 hours",
+                    "rotation": "1 days",
                 },
                 {
                     "sink": "logs/stats.log",
                     "format": cls.logfmt,
                     "level": "STATS",
                     "colorize": False,
                     "filter": cls.is_stats_log,
```

### Comparing `hordelib-0.8.8/hordelib.egg-info/PKG-INFO` & `hordelib-0.9.0/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.8.8
+Version: 0.9.0
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -906,17 +906,17 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-We need to patch the ComfyUI source code. It's only a small patch to:
+We patch the ComfyUI source code to:
 
-1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+1. Modify the model manager to allow us to dynamically move models between VRAM, RAM and disk cache.
 2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
```

### Comparing `hordelib-0.8.8/hordelib.egg-info/SOURCES.txt` & `hordelib-0.9.0/hordelib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 examples/run_facefix.py
 examples/run_img2img.py
 examples/run_img2img_hires.py
 examples/run_img2img_inpaint.py
 examples/run_img2img_inpaint_mask.py
 examples/run_img2img_outpaint.py
 examples/run_inpainting.py
+examples/run_memory_test.py
 examples/run_stress_test.py
 examples/run_txt2img.py
 examples/run_txt2img_hires.py
 examples/run_upscale.py
 hordelib/__init__.py
 hordelib/_version.py
 hordelib/comfy_horde.py
@@ -203,29 +204,33 @@
 hordelib/_comfyui/web/jsconfig.json
 hordelib/_comfyui/web/style.css
 hordelib/_comfyui/web/extensions/logging.js.example
 hordelib/_comfyui/web/extensions/core/colorPalette.js
 hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
 hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
 hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+hordelib/_comfyui/web/extensions/core/keybinds.js
 hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+hordelib/_comfyui/web/extensions/core/noteNode.js
 hordelib/_comfyui/web/extensions/core/rerouteNode.js
 hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
 hordelib/_comfyui/web/extensions/core/slotDefaults.js
 hordelib/_comfyui/web/extensions/core/snapToGrid.js
 hordelib/_comfyui/web/extensions/core/uploadImage.js
 hordelib/_comfyui/web/extensions/core/widgetInputs.js
 hordelib/_comfyui/web/lib/litegraph.core.js
 hordelib/_comfyui/web/lib/litegraph.css
 hordelib/_comfyui/web/scripts/api.js
 hordelib/_comfyui/web/scripts/app.js
 hordelib/_comfyui/web/scripts/defaultGraph.js
 hordelib/_comfyui/web/scripts/pnginfo.js
 hordelib/_comfyui/web/scripts/ui.js
 hordelib/_comfyui/web/scripts/widgets.js
+hordelib/_comfyui/web/types/comfy.d.ts
+hordelib/_comfyui/web/types/litegraph.d.ts
 hordelib/blip/__init__.py
 hordelib/blip/caption.py
 hordelib/cache/__init__.py
 hordelib/cache/cache.py
 hordelib/clip/__init__.py
 hordelib/clip/bulk.py
 hordelib/clip/coca.py
```

### Comparing `hordelib-0.8.8/images/test_annotator.jpg` & `hordelib-0.9.0/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_db0.jpg` & `hordelib-0.9.0/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_facefix.png` & `hordelib-0.9.0/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_inpaint.png` & `hordelib-0.9.0/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_inpaint_alpha.png` & `hordelib-0.9.0/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_inpaint_mask.png` & `hordelib-0.9.0/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_inpaint_original.png` & `hordelib-0.9.0/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/images/test_outpaint.png` & `hordelib-0.9.0/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/pyproject.toml` & `hordelib-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/requirements.txt` & `hordelib-0.9.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 pyyaml
 pillow
 loguru
 GitPython
 clip-anytorch
 diffusers
 omegaconf
+psutil
 # face fixer custom nodes
 opencv-python
 # controlnet custom nodes
 opencv-contrib-python
 opencv-python
 timm==0.6.12
 torchvision
```

### Comparing `hordelib-0.8.8/tests/make_index.py` & `hordelib-0.9.0/tests/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/model_managers/test_comvis.py` & `hordelib-0.9.0/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/model_managers/test_diffusers.py` & `hordelib-0.9.0/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/model_managers/test_safety_checker.py` & `hordelib-0.9.0/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_blip.py` & `hordelib-0.9.0/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_clip.py` & `hordelib-0.9.0/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_comfy.py` & `hordelib-0.9.0/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_controlnet_annotator.py` & `hordelib-0.9.0/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_inference.py` & `hordelib-0.9.0/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_inference_controlnet.py` & `hordelib-0.9.0/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_inference_img2img.py` & `hordelib-0.9.0/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_inference_painting.py` & `hordelib-0.9.0/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_horde_pp.py` & `hordelib-0.9.0/tests/test_horde_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_inference.py` & `hordelib-0.9.0/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_safety_checker.py` & `hordelib-0.9.0/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tests/test_shared_model_manager.py` & `hordelib-0.9.0/tests/test_shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.8/tox.ini` & `hordelib-0.9.0/tox.ini`

 * *Files identical despite different names*

