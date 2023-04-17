# Comparing `tmp/optimum-1.7.3.tar.gz` & `tmp/optimum-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.7.3.tar", last modified: Thu Mar 23 16:35:57 2023, max compression
+gzip compressed data, was "optimum-1.8.0.tar", last modified: Mon Apr 17 09:30:52 2023, max compression
```

## Comparing `optimum-1.7.3.tar` & `optimum-1.8.0.tar`

### file list

```diff
@@ -1,146 +1,153 @@
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.7.3/LICENSE
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.7.3/MANIFEST.in
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    14667 2023-03-23 16:35:57.151887 optimum-1.7.3/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13095 2023-03-21 08:52:27.000000 optimum-1.7.3/README.md
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/bettertransformer/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-02-09 07:31:23.000000 optimum-1.7.3/optimum/bettertransformer/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/bettertransformer/models/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8006 2023-03-21 08:52:48.000000 optimum-1.7.3/optimum/bettertransformer/models/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8138 2023-03-21 08:52:48.000000 optimum-1.7.3/optimum/bettertransformer/models/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    26636 2023-03-23 16:28:35.000000 optimum-1.7.3/optimum/bettertransformer/models/decoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    53744 2023-03-21 08:52:48.000000 optimum-1.7.3/optimum/bettertransformer/models/encoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16183 2023-03-21 08:53:05.000000 optimum-1.7.3/optimum/bettertransformer/transformation.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/commands/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      918 2023-02-09 07:31:23.000000 optimum-1.7.3/optimum/commands/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2709 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/commands/env.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/commands/export/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1899 2023-03-23 08:35:33.000000 optimum-1.7.3/optimum/commands/export/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-03-22 14:41:01.000000 optimum-1.7.3/optimum/commands/export/ggml.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1757 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/commands/export/onnx.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8289 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/commands/export/tflite.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/commands/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1273 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/commands/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2934 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/commands/onnxruntime/optimize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3014 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/commands/onnxruntime/quantize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1372 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/commands/optimum_cli.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/conftest.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/exporters/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-02-08 11:48:55.000000 optimum-1.7.3/optimum/exporters/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2022-12-05 12:56:27.000000 optimum-1.7.3/optimum/exporters/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      903 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/exporters/error_utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/exporters/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23309 2023-03-23 08:35:33.000000 optimum-1.7.3/optimum/exporters/onnx/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    39297 2023-03-22 08:53:47.000000 optimum-1.7.3/optimum/exporters/onnx/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17055 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/exporters/onnx/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      865 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/exporters/onnx/constants.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31653 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/onnx/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    36280 2023-03-22 08:53:47.000000 optimum-1.7.3/optimum/exporters/onnx/model_configs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7065 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/onnx/model_patcher.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9635 2023-03-22 08:53:47.000000 optimum-1.7.3/optimum/exporters/onnx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    51840 2023-03-23 08:35:33.000000 optimum-1.7.3/optimum/exporters/tasks.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/exporters/tflite/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/tflite/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5256 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/tflite/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15500 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/tflite/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/exporters/tflite/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16965 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/tflite/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/exporters/tflite/model_configs.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/fx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2022-10-28 14:20:22.000000 optimum-1.7.3/optimum/fx/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/fx/optimization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2022-12-05 12:56:27.000000 optimum-1.7.3/optimum/fx/optimization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-03-21 08:51:27.000000 optimum-1.7.3/optimum/fx/optimization/transformations.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/fx/quantization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2022-08-08 15:44:14.000000 optimum-1.7.3/optimum/fx/quantization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-02-28 09:19:08.000000 optimum-1.7.3/optimum/fx/quantization/functions.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2022-08-02 10:23:16.000000 optimum-1.7.3/optimum/fx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15117 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/modeling_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-03-21 08:53:05.000000 optimum-1.7.3/optimum/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnx/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10822 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/onnx/graph_transformations.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-02-09 07:31:23.000000 optimum-1.7.3/optimum/onnx/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9557 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/onnx/transformations_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/onnx/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    26044 2023-03-22 08:55:53.000000 optimum-1.7.3/optimum/onnxruntime/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45434 2023-03-21 08:51:27.000000 optimum-1.7.3/optimum/onnxruntime/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2022-04-11 08:30:37.000000 optimum-1.7.3/optimum/onnxruntime/graph.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/onnxruntime/io_binding/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-02-09 07:31:23.000000 optimum-1.7.3/optimum/onnxruntime/io_binding/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/model.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    27326 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/onnxruntime/modeling_decoder.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/onnxruntime/modeling_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    83391 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/onnxruntime/modeling_ort.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    50504 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/onnxruntime/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15083 2023-03-22 16:31:17.000000 optimum-1.7.3/optimum/onnxruntime/optimization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/onnxruntime/preprocessors/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2022-04-11 08:30:37.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2022-04-11 08:30:37.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/preprocessors/quantization.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23448 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/onnxruntime/quantization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/onnxruntime/runs/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8001 2023-03-21 08:51:27.000000 optimum-1.7.3/optimum/onnxruntime/runs/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2022-12-05 12:56:27.000000 optimum-1.7.3/optimum/onnxruntime/runs/calibrator.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      619 2023-02-09 07:31:23.000000 optimum-1.7.3/optimum/onnxruntime/runs/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    83898 2023-03-21 08:51:27.000000 optimum-1.7.3/optimum/onnxruntime/trainer.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38397 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/trainer_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16591 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/training_args.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/onnxruntime/training_args_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11721 2023-03-23 08:35:34.000000 optimum-1.7.3/optimum/onnxruntime/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/pipelines/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/pipelines/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/pipelines/diffusers/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/pipelines/diffusers/pipeline_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13522 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/pipelines/pipelines_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/quantization_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/runs_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/utils/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1966 2023-03-22 08:53:47.000000 optimum-1.7.3/optimum/utils/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/utils/constant.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/utils/doc.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/dummy_diffusers_objects.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-02-17 14:48:52.000000 optimum-1.7.3/optimum/utils/file_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6181 2023-03-22 08:53:47.000000 optimum-1.7.3/optimum/utils/import_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23612 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/input_generators.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7652 2023-03-21 08:47:53.000000 optimum-1.7.3/optimum/utils/logging.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-03-21 08:52:48.000000 optimum-1.7.3/optimum/utils/modeling_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9284 2023-03-22 15:41:33.000000 optimum-1.7.3/optimum/utils/normalized_config.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/optimum/utils/preprocessing/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/image_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/question_answering.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2173 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/task_processors_manager.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4437 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/text_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-03-21 09:04:22.000000 optimum-1.7.3/optimum/utils/preprocessing/token_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-03-21 08:51:55.000000 optimum-1.7.3/optimum/utils/runs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-03-22 16:08:18.000000 optimum-1.7.3/optimum/utils/save_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5586 2023-03-21 08:52:48.000000 optimum-1.7.3/optimum/utils/testing_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-03-23 16:33:36.000000 optimum-1.7.3/optimum/version.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.147887 optimum-1.7.3/optimum.egg-info/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    14667 2023-03-23 16:35:56.000000 optimum-1.7.3/optimum.egg-info/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4154 2023-03-23 16:35:57.000000 optimum-1.7.3/optimum.egg-info/SOURCES.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-03-23 16:35:56.000000 optimum-1.7.3/optimum.egg-info/dependency_links.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-03-23 16:35:56.000000 optimum-1.7.3/optimum.egg-info/entry_points.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-03-02 08:10:42.000000 optimum-1.7.3/optimum.egg-info/not-zip-safe
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      973 2023-03-23 16:35:57.000000 optimum-1.7.3/optimum.egg-info/requires.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-03-23 16:35:57.000000 optimum-1.7.3/optimum.egg-info/top_level.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.7.3/pyproject.toml
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-03-23 16:35:57.151887 optimum-1.7.3/setup.cfg
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3429 2023-03-21 09:04:22.000000 optimum-1.7.3/setup.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-03-23 16:35:57.151887 optimum-1.7.3/tests/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3432 2023-03-21 08:47:53.000000 optimum-1.7.3/tests/test_configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1936 2023-03-21 08:47:53.000000 optimum-1.7.3/tests/test_modeling_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.8.0/LICENSE
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.8.0/MANIFEST.in
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 09:30:52.402770 optimum-1.8.0/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9876 2023-04-17 07:37:27.000000 optimum-1.8.0/README.md
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/bettertransformer/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/bettertransformer/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/bettertransformer/models/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8420 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    21474 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/models/attention.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8092 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12222 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/models/decoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60023 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/encoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17127 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/transformation.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/commands/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      952 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5872 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2475 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/env.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/export/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      716 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1340 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/commands/export/ggml.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8554 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/onnx.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9016 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/commands/export/tflite.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      759 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1374 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3885 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/optimize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4011 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/quantize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6871 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/optimum_cli.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/register/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      621 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/register/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/configuration_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/conftest.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      903 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/error_utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17290 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    44198 2023-04-17 09:04:07.000000 optimum-1.8.0/optimum/exporters/onnx/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16221 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      865 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/onnx/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31628 2023-04-12 09:59:52.000000 optimum-1.8.0/optimum/exporters/onnx/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    37124 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/exporters/onnx/model_configs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7326 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/exporters/onnx/model_patcher.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9646 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    59776 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/exporters/tasks.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/tflite/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5256 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15507 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/tflite/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16963 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/tflite/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/model_configs.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/optimization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/optimization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/optimization/transformations.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/quantization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/quantization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/quantization/functions.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15117 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/modeling_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11198 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnx/graph_transformations.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13025 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnx/transformations_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32544 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45434 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      901 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/graph.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/io_binding/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/io_binding/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/model.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    30965 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/onnxruntime/modeling_decoder.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/modeling_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    83591 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/modeling_ort.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    58316 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15083 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/optimization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/preprocessors/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/quantization.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23448 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/quantization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/runs/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8001 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/runs/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/runs/calibrator.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      625 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/runs/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    88945 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/trainer.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38387 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/trainer_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17122 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/training_args.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/training_args_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11746 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/onnxruntime/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/pipelines/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/pipelines/diffusers/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13522 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/pipelines_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/quantization_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/runs_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/utils/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1989 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/constant.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/doc.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/dummy_diffusers_objects.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/file_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6181 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/import_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23612 2023-04-13 16:43:16.000000 optimum-1.8.0/optimum/utils/input_generators.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7836 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/logging.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/modeling_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9323 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/utils/normalized_config.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/utils/preprocessing/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/image_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/question_answering.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2169 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/utils/preprocessing/task_processors_manager.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4436 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/utils/preprocessing/text_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/token_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/runs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/save_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5762 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/testing_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-04-17 09:04:28.000000 optimum-1.8.0/optimum/version.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum.egg-info/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4365 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/SOURCES.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/dependency_links.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/entry_points.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-03-02 08:10:42.000000 optimum-1.8.0/optimum.egg-info/not-zip-safe
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      973 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/requires.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/top_level.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.8.0/pyproject.toml
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-04-17 09:30:52.402770 optimum-1.8.0/setup.cfg
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3429 2023-04-11 18:28:51.000000 optimum-1.8.0/setup.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/tests/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3432 2023-04-11 18:28:52.000000 optimum-1.8.0/tests/test_configuration_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1936 2023-04-11 18:28:52.000000 optimum-1.8.0/tests/test_modeling_base.py
```

### Comparing `optimum-1.7.3/LICENSE` & `optimum-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/MANIFEST.in` & `optimum-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/PKG-INFO` & `optimum-1.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.7.3
+Version: 1.8.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Platform: UNKNOWN
@@ -37,30 +37,15 @@
 Provides-Extra: benchmark
 License-File: LICENSE
 
 [![ONNX Runtime](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml/badge.svg)](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml)
 
 # Hugging Face Optimum
 
-🤗 Optimum is an extension of 🤗 Transformers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware.
-
-The AI ecosystem evolves quickly and more and more specialized hardware along with their own optimizations are emerging every day.
-As such, Optimum enables users to efficiently use any of these platforms with the same ease inherent to transformers.
-
-
-## Integration with Hardware Partners
-
-Optimum aims at providing more diversity towards the kind of hardware users can target to train and finetune their models.
-
-To achieve this, we are collaborating with the following hardware manufacturers in order to provide the best transformers integration:
-- [Graphcore IPUs](https://github.com/huggingface/optimum-graphcore) - IPUs are a completely new kind of massively parallel processor to accelerate machine intelligence. More information [here](https://www.graphcore.ai/products/ipu).
-- [Habana Gaudi Processor (HPU)](https://github.com/huggingface/optimum-habana) - [HPUs](https://docs.habana.ai/en/latest/Gaudi_Overview/Gaudi_Architecture.html) are designed to maximize training throughput and efficiency. More information [here](https://habana.ai/training/).
-- [Intel](https://github.com/huggingface/optimum-intel) - Enabling the usage of Intel tools to accelerate inference on Intel architectures. More information about [Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html) and [OpenVINO](https://docs.openvino.ai/latest/index.html).
-- More to come soon! :star:
-
+🤗 Optimum is an extension of 🤗 Transformers and Diffusers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware, while keeping things easy to use.
 
 ## Installation
 
 🤗 Optimum can be installed using `pip` as follows:
 
 ```bash
 python -m pip install optimum
@@ -69,128 +54,143 @@
 If you'd like to use the accelerator-specific features of 🤗 Optimum, you can install the required dependencies according to the table below:
 
 | Accelerator                                                                                                            | Installation                                      |
 |:-----------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------|
 | [ONNX Runtime](https://onnxruntime.ai/docs/)                                                                           | `python -m pip install optimum[onnxruntime]`      |
 | [Intel Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html)       | `python -m pip install optimum[neural-compressor]`|
 | [OpenVINO](https://docs.openvino.ai/latest/index.html)                                                                 | `python -m pip install optimum[openvino,nncf]`    |
-| [Graphcore IPU](https://www.graphcore.ai/products/ipu)                                                                 | `python -m pip install optimum[graphcore]`        |
 | [Habana Gaudi Processor (HPU)](https://habana.ai/training/)                                                            | `python -m pip install optimum[habana]`           |
 
-
-If you'd like to play with the examples or need the bleeding edge of the code and can't wait for a new release, you can install the base library from source as follows:
+To install from source:
 
 ```bash
 python -m pip install git+https://github.com/huggingface/optimum.git
 ```
 
-For the accelerator-specific features, you can install them by appending `#egg=optimum[accelerator_type]` to the `pip` command, e.g.
+For the accelerator-specific features, append `#egg=optimum[accelerator_type]` to the above command:
 
 ```bash
 python -m pip install git+https://github.com/huggingface/optimum.git#egg=optimum[onnxruntime]
 ```
 
+## Accelerated Inference
 
-## Optimizing models towards inference
+🤗 Optimum provides multiple tools to export and run optimized models on various ecosystems: 
 
-Along with supporting dedicated AI hardware for training, Optimum also provides inference optimizations towards various frameworks and
-platforms.
+- [ONNX](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model) / [ONNX Runtime](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/models)
+- TensorFlow Lite
+- [OpenVINO](https://huggingface.co/docs/optimum/intel/inference)
+- Habana first-gen Gaudi / Gaudi2, more details [here](https://huggingface.co/docs/optimum/main/en/habana/usage_guides/accelerate_inference)
 
-Optimum enables the usage of popular compression techniques such as quantization and pruning by supporting [ONNX Runtime](https://onnxruntime.ai/docs/) along with Intel [Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html) and OpenVINO [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html).
+The [export](https://huggingface.co/docs/optimum/exporters/overview) and optimizations can be done both programmatically and with a command line.
 
-| Features                           | ONNX Runtime          |     Neural Compressor   |         OpenVINO        |
-|:----------------------------------:|:---------------------:|:-----------------------:|:-----------------------:|
-| Post-training Dynamic Quantization |  :heavy_check_mark:   |    :heavy_check_mark:   |          N/A            |
-| Post-training Static Quantization  |  :heavy_check_mark:   |    :heavy_check_mark:   |    :heavy_check_mark:   |
-| Quantization Aware Training (QAT)  |  Stay tuned! :star:   |    :heavy_check_mark:   |    :heavy_check_mark:   |
-| Pruning                            |        N/A            |    :heavy_check_mark:   |    :heavy_check_mark:   |
+### Features summary
 
-## Quick tour
+| Features                           | ONNX Runtime       | Neural Compressor  | OpenVINO           | TensorFlow Lite    |
+|:----------------------------------:|:------------------:|:------------------:|:------------------:|:------------------:|
+| Graph optimization                 | :heavy_check_mark: | N/A                | :heavy_check_mark: | N/A                |
+| Post-training dynamic quantization | :heavy_check_mark: | :heavy_check_mark: | N/A                | :heavy_check_mark: |
+| Post-training static quantization  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
+| Quantization Aware Training (QAT)  | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
+| FP16 (half precision)              | :heavy_check_mark: | N/A                | :heavy_check_mark: | :heavy_check_mark: |
+| Pruning                            | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
+| Knowledge Distillation             | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 
-Check out the examples below to see how 🤗 Optimum can be used to train and run inference on various hardware accelerators.
+### ONNX + ONNX Runtime
 
-## Accelerated inference
+It is possible to export 🤗 Transformers models to the [ONNX](https://onnx.ai/) format and perform graph optimization as well as quantization easily:
 
-#### ONNX Runtime
+```plain
+optimum-cli export onnx -m deepset/roberta-base-squad2 --optimize O2 roberta_base_qa_onnx
+```
 
-To accelerate inference with ONNX Runtime, 🤗 Optimum uses _configuration objects_ to define parameters for graph optimization and quantization. These objects are then used to instantiate dedicated _optimizers_ and _quantizers_.
+The model can then be quantized using `onnxruntime`:
 
-Before applying quantization or optimization, first we need to load our model. To load a model and run inference with ONNX Runtime, you can just replace the canonical Transformers [`AutoModelForXxx`](https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModel) class with the corresponding [`ORTModelForXxx`](https://huggingface.co/docs/optimum/onnxruntime/package_reference/modeling_ort#optimum.onnxruntime.ORTModel) class. If you want to load from a PyTorch checkpoint, set `from_transformers=True` to export your model to the ONNX format.
+```bash
+optimum-cli onnxruntime quantize \
+  --avx512 \
+  --onnx_model roberta_base_qa_onnx \
+  -o quantized_roberta_base_qa_onnx
+```
 
-```python
-from optimum.onnxruntime import ORTModelForSequenceClassification
-from transformers import AutoTokenizer
+These commands will export `deepset/roberta-base-squad2` and perform [O2 graph optimization](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/optimization#optimization-configuration) on the exported model, and finally quantize it with the [avx512 configuration](https://huggingface.co/docs/optimum/main/en/onnxruntime/package_reference/configuration#optimum.onnxruntime.AutoQuantizationConfig.avx512).
 
-model_checkpoint = "distilbert-base-uncased-finetuned-sst-2-english"
-save_directory = "tmp/onnx/"
-# Load a model from transformers and export it to ONNX
-tokenizer = AutoTokenizer.from_pretrained(model_checkpoint)
-ort_model = ORTModelForSequenceClassification.from_pretrained(model_checkpoint, from_transformers=True)
-# Save the ONNX model and tokenizer
-ort_model.save_pretrained(save_directory)
-tokenizer.save_pretrained(save_directory)
-```
+For more information on the ONNX export, please check the [documentation](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model).
+
+#### Run the exported model using ONNX Runtime
 
-Let's see now how we can apply dynamic quantization with ONNX Runtime:
+Once the model is exported to the ONNX format, we provide Python classes enabling you to run the exported ONNX model in a seemless manner using [ONNX Runtime](https://onnxruntime.ai/) in the backend:
 
 ```python
-from optimum.onnxruntime.configuration import AutoQuantizationConfig
-from optimum.onnxruntime import ORTQuantizer
+from transformers import AutoTokenizer
+from optimum.onnxruntime import ORTModelForQuestionAnswering
 
-# Define the quantization methodology
-qconfig = AutoQuantizationConfig.arm64(is_static=False, per_channel=False)
-quantizer = ORTQuantizer.from_pretrained(ort_model)
-# Apply dynamic quantization on the model
-quantizer.quantize(save_dir=save_directory, quantization_config=qconfig)
-```
+model_name = "roberta_base_qa_onnx"
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+ort_model = ORTModelForQuestionAnswering.from_pretrained(model_name)
 
-In this example, we've quantized a model from the Hugging Face Hub, in the same manner we can quantize a model hosted locally by providing the path to the directory containing the model weights. The result from applying the `quantize()` method is a `model_quantized.onnx` file that can be used to run inference. Here's an example of how to load an ONNX Runtime model and generate predictions with it:
+question = "What's Optimum?"
+text = "Optimum is an awesome library everyone should use!"
+inputs = tokenizer(question, text, return_tensors="pt") 
 
-```python
-from optimum.onnxruntime import ORTModelForSequenceClassification
-from transformers import pipeline, AutoTokenizer
+# Run with ONNX Runtime.
+outputs = ort_model(**inputs)
+
+answer_start_index = outputs.start_logits.argmax()
+answer_end_index = outputs.end_logits.argmax()
 
-model = ORTModelForSequenceClassification.from_pretrained(save_directory, file_name="model_quantized.onnx")
-tokenizer = AutoTokenizer.from_pretrained(save_directory)
-classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
-results = classifier("I love burritos!")
+predict_answer_tokens = inputs.input_ids[0, answer_start_index : answer_end_index + 1]
+answer = tokenizer.decode(predict_answer_tokens, skip_special_tokens=True)
 ```
 
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/quickstart) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime).
+More details on how to run ONNX models with `ORTModelForXXX` classes [here](https://huggingface.co/docs/optimum/main/en/onnxruntime/usage_guides/models).
 
+### TensorFlow Lite
+
+Just as for ONNX, it is possible to export models to [TensorFlow Lite](https://www.tensorflow.org/lite) and quantize them:
+
+```plain
+optimum-cli export tflite \
+  -m deepset/roberta-base-squad2 \
+  --sequence_length 384  \
+  --quantize int8-dynamic roberta_tflite_model
+```
+### OpenVINO
 
-#### Intel
+*This requires to install the Optimum OpenVINO extra by doing `pip install optimum[openvino,nncf]`.*
 
-To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class.
-If you want to load a PyTorch checkpoint, set `from_transformers=True` to convert your model to the OpenVINO IR (Intermediate Representation).
+To load a model and run inference with [OpenVINO Runtime](https://docs.openvino.ai/latest/home.html), you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
 
 ```diff
 - from transformers import AutoModelForSequenceClassification
-+ from optimum.intel.openvino import OVModelForSequenceClassification
++ from optimum.intel import OVModelForSequenceClassification
   from transformers import AutoTokenizer, pipeline
 
-  # Download a tokenizer and model from the Hub and convert to OpenVINO format
-  tokenizer = AutoTokenizer.from_pretrained(model_id)
   model_id = "distilbert-base-uncased-finetuned-sst-2-english"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
 - model = AutoModelForSequenceClassification.from_pretrained(model_id)
-+ model = OVModelForSequenceClassification.from_pretrained(model_id, from_transformers=True)
++ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
+  model.save_pretrained("./distilbert")
 
-  # Run inference!
   classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
   results = classifier("He's a dreadful magician.")
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
 
 
 ## Accelerated training
 
-#### Habana
+🤗 Optimum provides wrappers around the original 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer) to enable training on powerful hardware easily.
+We support many providers:
+
+- Habana's Gaudi processors
+- ONNX Runtime (optimized for GPUs)
 
-To train transformers on Habana's Gaudi processors, 🤗 Optimum provides a `GaudiTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
+### Habana
 
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.habana import GaudiTrainer, GaudiTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForXxx.from_pretrained("bert-base-uncased")
@@ -216,57 +216,15 @@
 
   # Use Habana Gaudi processor for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/habana/quickstart) and in the [examples](https://github.com/huggingface/optimum-habana/tree/main/examples).
 
-
-#### Graphcore
-
-To train transformers on Graphcore's IPUs, 🤗 Optimum provides a `IPUTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
-
-```diff
-- from transformers import Trainer, TrainingArguments
-+ from optimum.graphcore import IPUConfig, IPUTrainer, IPUTrainingArguments
-
-  # Download a pretrained model from the Hub
-  model = AutoModelForXxx.from_pretrained("bert-base-uncased")
-
-  # Define the training arguments
-- training_args = TrainingArguments(
-+ training_args = IPUTrainingArguments(
-      output_dir="path/to/save/folder/",
-+     ipu_config_name="Graphcore/bert-base-ipu", # Any IPUConfig on the Hub or stored locally
-      ...
-  )
-
-  # Define the configuration to compile and put the model on the IPU
-+ ipu_config = IPUConfig.from_pretrained(training_args.ipu_config_name)
-
-  # Initialize the trainer
-- trainer = Trainer(
-+ trainer = IPUTrainer(
-      model=model,
-+     ipu_config=ipu_config
-      args=training_args,
-      train_dataset=train_dataset
-      ...
-  )
-
-  # Use Graphcore IPU for training!
-  trainer.train()
-```
-
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/graphcore/quickstart) and in the [examples](https://github.com/huggingface/optimum-graphcore/tree/main/examples).
-
-
-#### ONNX Runtime
-
-To train transformers with ONNX Runtime's acceleration features, 🤗 Optimum provides a `ORTTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
+### ONNX Runtime
 
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.onnxruntime import ORTTrainer, ORTTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForSequenceClassification.from_pretrained("bert-base-uncased")
```

### Comparing `optimum-1.7.3/README.md` & `optimum-1.8.0/optimum.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,51 @@
+Metadata-Version: 2.1
+Name: optimum
+Version: 1.8.0
+Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
+Home-page: https://github.com/huggingface/optimum
+Author: HuggingFace Inc. Special Ops Team
+Author-email: hardware@huggingface.co
+License: Apache
+Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: onnxruntime
+Provides-Extra: onnxruntime-gpu
+Provides-Extra: exporters
+Provides-Extra: exporters-gpu
+Provides-Extra: exporters-tf
+Provides-Extra: intel
+Provides-Extra: openvino
+Provides-Extra: nncf
+Provides-Extra: neural-compressor
+Provides-Extra: graphcore
+Provides-Extra: habana
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: quality
+Provides-Extra: benchmark
+License-File: LICENSE
+
 [![ONNX Runtime](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml/badge.svg)](https://github.com/huggingface/optimum/actions/workflows/test_onnxruntime.yml)
 
 # Hugging Face Optimum
 
-🤗 Optimum is an extension of 🤗 Transformers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware.
-
-The AI ecosystem evolves quickly and more and more specialized hardware along with their own optimizations are emerging every day.
-As such, Optimum enables users to efficiently use any of these platforms with the same ease inherent to transformers.
-
-
-## Integration with Hardware Partners
-
-Optimum aims at providing more diversity towards the kind of hardware users can target to train and finetune their models.
-
-To achieve this, we are collaborating with the following hardware manufacturers in order to provide the best transformers integration:
-- [Graphcore IPUs](https://github.com/huggingface/optimum-graphcore) - IPUs are a completely new kind of massively parallel processor to accelerate machine intelligence. More information [here](https://www.graphcore.ai/products/ipu).
-- [Habana Gaudi Processor (HPU)](https://github.com/huggingface/optimum-habana) - [HPUs](https://docs.habana.ai/en/latest/Gaudi_Overview/Gaudi_Architecture.html) are designed to maximize training throughput and efficiency. More information [here](https://habana.ai/training/).
-- [Intel](https://github.com/huggingface/optimum-intel) - Enabling the usage of Intel tools to accelerate inference on Intel architectures. More information about [Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html) and [OpenVINO](https://docs.openvino.ai/latest/index.html).
-- More to come soon! :star:
-
+🤗 Optimum is an extension of 🤗 Transformers and Diffusers, providing a set of optimization tools enabling maximum efficiency to train and run models on targeted hardware, while keeping things easy to use.
 
 ## Installation
 
 🤗 Optimum can be installed using `pip` as follows:
 
 ```bash
 python -m pip install optimum
@@ -30,128 +54,143 @@
 If you'd like to use the accelerator-specific features of 🤗 Optimum, you can install the required dependencies according to the table below:
 
 | Accelerator                                                                                                            | Installation                                      |
 |:-----------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------|
 | [ONNX Runtime](https://onnxruntime.ai/docs/)                                                                           | `python -m pip install optimum[onnxruntime]`      |
 | [Intel Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html)       | `python -m pip install optimum[neural-compressor]`|
 | [OpenVINO](https://docs.openvino.ai/latest/index.html)                                                                 | `python -m pip install optimum[openvino,nncf]`    |
-| [Graphcore IPU](https://www.graphcore.ai/products/ipu)                                                                 | `python -m pip install optimum[graphcore]`        |
 | [Habana Gaudi Processor (HPU)](https://habana.ai/training/)                                                            | `python -m pip install optimum[habana]`           |
 
-
-If you'd like to play with the examples or need the bleeding edge of the code and can't wait for a new release, you can install the base library from source as follows:
+To install from source:
 
 ```bash
 python -m pip install git+https://github.com/huggingface/optimum.git
 ```
 
-For the accelerator-specific features, you can install them by appending `#egg=optimum[accelerator_type]` to the `pip` command, e.g.
+For the accelerator-specific features, append `#egg=optimum[accelerator_type]` to the above command:
 
 ```bash
 python -m pip install git+https://github.com/huggingface/optimum.git#egg=optimum[onnxruntime]
 ```
 
+## Accelerated Inference
 
-## Optimizing models towards inference
+🤗 Optimum provides multiple tools to export and run optimized models on various ecosystems: 
 
-Along with supporting dedicated AI hardware for training, Optimum also provides inference optimizations towards various frameworks and
-platforms.
+- [ONNX](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model) / [ONNX Runtime](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/models)
+- TensorFlow Lite
+- [OpenVINO](https://huggingface.co/docs/optimum/intel/inference)
+- Habana first-gen Gaudi / Gaudi2, more details [here](https://huggingface.co/docs/optimum/main/en/habana/usage_guides/accelerate_inference)
 
-Optimum enables the usage of popular compression techniques such as quantization and pruning by supporting [ONNX Runtime](https://onnxruntime.ai/docs/) along with Intel [Neural Compressor](https://www.intel.com/content/www/us/en/developer/tools/oneapi/neural-compressor.html) and OpenVINO [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html).
+The [export](https://huggingface.co/docs/optimum/exporters/overview) and optimizations can be done both programmatically and with a command line.
 
-| Features                           | ONNX Runtime          |     Neural Compressor   |         OpenVINO        |
-|:----------------------------------:|:---------------------:|:-----------------------:|:-----------------------:|
-| Post-training Dynamic Quantization |  :heavy_check_mark:   |    :heavy_check_mark:   |          N/A            |
-| Post-training Static Quantization  |  :heavy_check_mark:   |    :heavy_check_mark:   |    :heavy_check_mark:   |
-| Quantization Aware Training (QAT)  |  Stay tuned! :star:   |    :heavy_check_mark:   |    :heavy_check_mark:   |
-| Pruning                            |        N/A            |    :heavy_check_mark:   |    :heavy_check_mark:   |
+### Features summary
 
-## Quick tour
+| Features                           | ONNX Runtime       | Neural Compressor  | OpenVINO           | TensorFlow Lite    |
+|:----------------------------------:|:------------------:|:------------------:|:------------------:|:------------------:|
+| Graph optimization                 | :heavy_check_mark: | N/A                | :heavy_check_mark: | N/A                |
+| Post-training dynamic quantization | :heavy_check_mark: | :heavy_check_mark: | N/A                | :heavy_check_mark: |
+| Post-training static quantization  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
+| Quantization Aware Training (QAT)  | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
+| FP16 (half precision)              | :heavy_check_mark: | N/A                | :heavy_check_mark: | :heavy_check_mark: |
+| Pruning                            | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
+| Knowledge Distillation             | N/A                | :heavy_check_mark: | :heavy_check_mark: | N/A                |
 
-Check out the examples below to see how 🤗 Optimum can be used to train and run inference on various hardware accelerators.
+### ONNX + ONNX Runtime
 
-## Accelerated inference
+It is possible to export 🤗 Transformers models to the [ONNX](https://onnx.ai/) format and perform graph optimization as well as quantization easily:
 
-#### ONNX Runtime
+```plain
+optimum-cli export onnx -m deepset/roberta-base-squad2 --optimize O2 roberta_base_qa_onnx
+```
 
-To accelerate inference with ONNX Runtime, 🤗 Optimum uses _configuration objects_ to define parameters for graph optimization and quantization. These objects are then used to instantiate dedicated _optimizers_ and _quantizers_.
+The model can then be quantized using `onnxruntime`:
 
-Before applying quantization or optimization, first we need to load our model. To load a model and run inference with ONNX Runtime, you can just replace the canonical Transformers [`AutoModelForXxx`](https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoModel) class with the corresponding [`ORTModelForXxx`](https://huggingface.co/docs/optimum/onnxruntime/package_reference/modeling_ort#optimum.onnxruntime.ORTModel) class. If you want to load from a PyTorch checkpoint, set `from_transformers=True` to export your model to the ONNX format.
+```bash
+optimum-cli onnxruntime quantize \
+  --avx512 \
+  --onnx_model roberta_base_qa_onnx \
+  -o quantized_roberta_base_qa_onnx
+```
 
-```python
-from optimum.onnxruntime import ORTModelForSequenceClassification
-from transformers import AutoTokenizer
+These commands will export `deepset/roberta-base-squad2` and perform [O2 graph optimization](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/optimization#optimization-configuration) on the exported model, and finally quantize it with the [avx512 configuration](https://huggingface.co/docs/optimum/main/en/onnxruntime/package_reference/configuration#optimum.onnxruntime.AutoQuantizationConfig.avx512).
 
-model_checkpoint = "distilbert-base-uncased-finetuned-sst-2-english"
-save_directory = "tmp/onnx/"
-# Load a model from transformers and export it to ONNX
-tokenizer = AutoTokenizer.from_pretrained(model_checkpoint)
-ort_model = ORTModelForSequenceClassification.from_pretrained(model_checkpoint, from_transformers=True)
-# Save the ONNX model and tokenizer
-ort_model.save_pretrained(save_directory)
-tokenizer.save_pretrained(save_directory)
-```
+For more information on the ONNX export, please check the [documentation](https://huggingface.co/docs/optimum/exporters/onnx/usage_guides/export_a_model).
 
-Let's see now how we can apply dynamic quantization with ONNX Runtime:
+#### Run the exported model using ONNX Runtime
+
+Once the model is exported to the ONNX format, we provide Python classes enabling you to run the exported ONNX model in a seemless manner using [ONNX Runtime](https://onnxruntime.ai/) in the backend:
 
 ```python
-from optimum.onnxruntime.configuration import AutoQuantizationConfig
-from optimum.onnxruntime import ORTQuantizer
+from transformers import AutoTokenizer
+from optimum.onnxruntime import ORTModelForQuestionAnswering
 
-# Define the quantization methodology
-qconfig = AutoQuantizationConfig.arm64(is_static=False, per_channel=False)
-quantizer = ORTQuantizer.from_pretrained(ort_model)
-# Apply dynamic quantization on the model
-quantizer.quantize(save_dir=save_directory, quantization_config=qconfig)
-```
+model_name = "roberta_base_qa_onnx"
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+ort_model = ORTModelForQuestionAnswering.from_pretrained(model_name)
 
-In this example, we've quantized a model from the Hugging Face Hub, in the same manner we can quantize a model hosted locally by providing the path to the directory containing the model weights. The result from applying the `quantize()` method is a `model_quantized.onnx` file that can be used to run inference. Here's an example of how to load an ONNX Runtime model and generate predictions with it:
+question = "What's Optimum?"
+text = "Optimum is an awesome library everyone should use!"
+inputs = tokenizer(question, text, return_tensors="pt") 
 
-```python
-from optimum.onnxruntime import ORTModelForSequenceClassification
-from transformers import pipeline, AutoTokenizer
+# Run with ONNX Runtime.
+outputs = ort_model(**inputs)
 
-model = ORTModelForSequenceClassification.from_pretrained(save_directory, file_name="model_quantized.onnx")
-tokenizer = AutoTokenizer.from_pretrained(save_directory)
-classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
-results = classifier("I love burritos!")
+answer_start_index = outputs.start_logits.argmax()
+answer_end_index = outputs.end_logits.argmax()
+
+predict_answer_tokens = inputs.input_ids[0, answer_start_index : answer_end_index + 1]
+answer = tokenizer.decode(predict_answer_tokens, skip_special_tokens=True)
 ```
 
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/quickstart) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime).
+More details on how to run ONNX models with `ORTModelForXXX` classes [here](https://huggingface.co/docs/optimum/main/en/onnxruntime/usage_guides/models).
+
+### TensorFlow Lite
+
+Just as for ONNX, it is possible to export models to [TensorFlow Lite](https://www.tensorflow.org/lite) and quantize them:
 
+```plain
+optimum-cli export tflite \
+  -m deepset/roberta-base-squad2 \
+  --sequence_length 384  \
+  --quantize int8-dynamic roberta_tflite_model
+```
+### OpenVINO
 
-#### Intel
+*This requires to install the Optimum OpenVINO extra by doing `pip install optimum[openvino,nncf]`.*
 
-To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class.
-If you want to load a PyTorch checkpoint, set `from_transformers=True` to convert your model to the OpenVINO IR (Intermediate Representation).
+To load a model and run inference with [OpenVINO Runtime](https://docs.openvino.ai/latest/home.html), you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class. To load a PyTorch checkpoint and convert it to the OpenVINO format on-the-fly, you can set `export=True` when loading your model.
 
 ```diff
 - from transformers import AutoModelForSequenceClassification
-+ from optimum.intel.openvino import OVModelForSequenceClassification
++ from optimum.intel import OVModelForSequenceClassification
   from transformers import AutoTokenizer, pipeline
 
-  # Download a tokenizer and model from the Hub and convert to OpenVINO format
-  tokenizer = AutoTokenizer.from_pretrained(model_id)
   model_id = "distilbert-base-uncased-finetuned-sst-2-english"
+  tokenizer = AutoTokenizer.from_pretrained(model_id)
 - model = AutoModelForSequenceClassification.from_pretrained(model_id)
-+ model = OVModelForSequenceClassification.from_pretrained(model_id, from_transformers=True)
++ model = OVModelForSequenceClassification.from_pretrained(model_id, export=True)
+  model.save_pretrained("./distilbert")
 
-  # Run inference!
   classifier = pipeline("text-classification", model=model, tokenizer=tokenizer)
   results = classifier("He's a dreadful magician.")
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/intel/inference) and in the [examples](https://github.com/huggingface/optimum-intel/tree/main/examples/openvino).
 
 
 ## Accelerated training
 
-#### Habana
+🤗 Optimum provides wrappers around the original 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer) to enable training on powerful hardware easily.
+We support many providers:
+
+- Habana's Gaudi processors
+- ONNX Runtime (optimized for GPUs)
 
-To train transformers on Habana's Gaudi processors, 🤗 Optimum provides a `GaudiTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
+### Habana
 
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.habana import GaudiTrainer, GaudiTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForXxx.from_pretrained("bert-base-uncased")
@@ -177,57 +216,15 @@
 
   # Use Habana Gaudi processor for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/habana/quickstart) and in the [examples](https://github.com/huggingface/optimum-habana/tree/main/examples).
 
-
-#### Graphcore
-
-To train transformers on Graphcore's IPUs, 🤗 Optimum provides a `IPUTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
-
-```diff
-- from transformers import Trainer, TrainingArguments
-+ from optimum.graphcore import IPUConfig, IPUTrainer, IPUTrainingArguments
-
-  # Download a pretrained model from the Hub
-  model = AutoModelForXxx.from_pretrained("bert-base-uncased")
-
-  # Define the training arguments
-- training_args = TrainingArguments(
-+ training_args = IPUTrainingArguments(
-      output_dir="path/to/save/folder/",
-+     ipu_config_name="Graphcore/bert-base-ipu", # Any IPUConfig on the Hub or stored locally
-      ...
-  )
-
-  # Define the configuration to compile and put the model on the IPU
-+ ipu_config = IPUConfig.from_pretrained(training_args.ipu_config_name)
-
-  # Initialize the trainer
-- trainer = Trainer(
-+ trainer = IPUTrainer(
-      model=model,
-+     ipu_config=ipu_config
-      args=training_args,
-      train_dataset=train_dataset
-      ...
-  )
-
-  # Use Graphcore IPU for training!
-  trainer.train()
-```
-
-You can find more examples in the [documentation](https://huggingface.co/docs/optimum/graphcore/quickstart) and in the [examples](https://github.com/huggingface/optimum-graphcore/tree/main/examples).
-
-
-#### ONNX Runtime
-
-To train transformers with ONNX Runtime's acceleration features, 🤗 Optimum provides a `ORTTrainer` that is very similar to the 🤗 Transformers [Trainer](https://huggingface.co/docs/transformers/main_classes/trainer). Here is a simple example:
+### ONNX Runtime
 
 ```diff
 - from transformers import Trainer, TrainingArguments
 + from optimum.onnxruntime import ORTTrainer, ORTTrainingArguments
 
   # Download a pretrained model from the Hub
   model = AutoModelForSequenceClassification.from_pretrained("bert-base-uncased")
@@ -251,7 +248,9 @@
   )
 
   # Use ONNX Runtime for training!
   trainer.train()
 ```
 
 You can find more examples in the [documentation](https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer) and in the [examples](https://github.com/huggingface/optimum/tree/main/examples/onnxruntime/training).
+
+
```

### Comparing `optimum-1.7.3/optimum/bettertransformer/__init__.py` & `optimum-1.8.0/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/bettertransformer/models/__init__.py` & `optimum-1.8.0/optimum/bettertransformer/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,35 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import warnings
 
 from .decoder_models import (
     BartAttentionLayerBetterTransformer,
+    BlenderbotAttentionLayerBetterTransformer,
     CodegenAttentionLayerBetterTransformer,
     GPT2AttentionLayerBetterTransformer,
+    GPTJAttentionLayerBetterTransformer,
     GPTNeoAttentionLayerBetterTransformer,
+    GPTNeoXAttentionLayerBetterTransformer,
+    M2M100AttentionLayerBetterTransformer,
+    MarianAttentionLayerBetterTransformer,
     OPTAttentionLayerBetterTransformer,
+    PegasusAttentionLayerBetterTransformer,
     T5AttentionLayerBetterTransformer,
 )
 from .encoder_models import (
     AlbertLayerBetterTransformer,
     BartEncoderLayerBetterTransformer,
     BertLayerBetterTransformer,
     CLIPLayerBetterTransformer,
     DistilBertLayerBetterTransformer,
     FSMTEncoderLayerBetterTransformer,
     MBartEncoderLayerBetterTransformer,
+    ProphetNetEncoderLayerBetterTransformer,
     ViltLayerBetterTransformer,
     ViTLayerBetterTransformer,
     Wav2Vec2EncoderLayerBetterTransformer,
     WhisperEncoderLayerBetterTransformer,
 )
 
 
@@ -41,43 +48,44 @@
         "albert": {"AlbertLayer": AlbertLayerBetterTransformer},
         "bart": {
             "BartEncoderLayer": BartEncoderLayerBetterTransformer,
             "BartAttention": BartAttentionLayerBetterTransformer,
         },
         "bert": {"BertLayer": BertLayerBetterTransformer},
         "bert-generation": {"BertGenerationLayer": BertLayerBetterTransformer},
-        "blenderbot": {"BlenderbotAttention": BartAttentionLayerBetterTransformer},
+        "blenderbot": {"BlenderbotAttention": BlenderbotAttentionLayerBetterTransformer},
         "camembert": {"CamembertLayer": BertLayerBetterTransformer},
         "clip": {"CLIPEncoderLayer": CLIPLayerBetterTransformer},
         "codegen": {"CodeGenAttention": CodegenAttentionLayerBetterTransformer},
         "data2vec-text": {"Data2VecTextLayer": BertLayerBetterTransformer},
         "deit": {"DeiTLayer": ViTLayerBetterTransformer},
         "distilbert": {"TransformerBlock": DistilBertLayerBetterTransformer},
         "electra": {"ElectraLayer": BertLayerBetterTransformer},
         "ernie": {"ErnieLayer": BertLayerBetterTransformer},
         "fsmt": {"EncoderLayer": FSMTEncoderLayerBetterTransformer},
         "gpt2": {"GPT2Attention": GPT2AttentionLayerBetterTransformer},
-        "gptj": {"GPTJAttention": GPT2AttentionLayerBetterTransformer},
+        "gptj": {"GPTJAttention": GPTJAttentionLayerBetterTransformer},
         "gpt_neo": {"GPTNeoSelfAttention": GPTNeoAttentionLayerBetterTransformer},
-        "gpt_neox": {"GPTNeoXAttention": GPT2AttentionLayerBetterTransformer},
+        "gpt_neox": {"GPTNeoXAttention": GPTNeoXAttentionLayerBetterTransformer},
         "hubert": {"HubertEncoderLayer": Wav2Vec2EncoderLayerBetterTransformer},
         "layoutlm": {"LayoutLMLayer": BertLayerBetterTransformer},
         "m2m_100": {
             "M2M100EncoderLayer": MBartEncoderLayerBetterTransformer,
-            "M2M100Attention": BartAttentionLayerBetterTransformer,
+            "M2M100Attention": M2M100AttentionLayerBetterTransformer,
         },
         "marian": {
             "MarianEncoderLayer": BartEncoderLayerBetterTransformer,
-            "MarianAttention": BartAttentionLayerBetterTransformer,
+            "MarianAttention": MarianAttentionLayerBetterTransformer,
         },
         "markuplm": {"MarkupLMLayer": BertLayerBetterTransformer},
         "mbart": {"MBartEncoderLayer": MBartEncoderLayerBetterTransformer},
         "opt": {"OPTAttention": OPTAttentionLayerBetterTransformer},
-        "pegasus": {"PegasusAttention": BartAttentionLayerBetterTransformer},
+        "pegasus": {"PegasusAttention": PegasusAttentionLayerBetterTransformer},
         "rembert": {"RemBertLayer": BertLayerBetterTransformer},
+        "prophetnet": {"ProphetNetEncoderLayer": ProphetNetEncoderLayerBetterTransformer},
         "roberta": {"RobertaLayer": BertLayerBetterTransformer},
         "roc_bert": {"RoCBertLayer": BertLayerBetterTransformer},
         "roformer": {"RoFormerLayer": BertLayerBetterTransformer},
         "splinter": {"SplinterLayer": BertLayerBetterTransformer},
         "tapas": {"TapasLayer": BertLayerBetterTransformer},
         "t5": {"T5Attention": T5AttentionLayerBetterTransformer},
         "vilt": {"ViltLayer": ViltLayerBetterTransformer},
```

### Comparing `optimum-1.7.3/optimum/bettertransformer/models/base.py` & `optimum-1.8.0/optimum/bettertransformer/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
 import torch
-import torch.nn as nn
 
 from ...utils import logging, recurse_getattr, recurse_setattr
 
 
 KNOWN_ACTIVATION_ATTRIBUTES = ["hidden_act", "activation", "act_fn", "activation_function"]
 KNOWN_POS_EMB_ATTRIBUTES = ["position_embedding_type"]
 KNOWN_NUM_LAYERS = ["num_hidden_layers", "num_layers", "encoder_layers", "n_layers"]
@@ -30,38 +29,37 @@
 SUPPORTED_ACTIVATION_FUNCTIONS = ["gelu", "relu", "gelu_new"]
 USE_AT_OWN_RISK_ACTIVATION_FUNCTIONS = ["quick_gelu"]
 
 
 logger = logging.get_logger(__name__)
 
 
-class BetterTransformerBaseLayer(nn.Module):
+class BetterTransformerBaseLayer:
     def __init__(
         self,
         config: "PretrainedConfig",
     ):
         r"""
         Base layer for `BetterTransformer` integration. This class is used to wrap all the necessary
         components for the `BetterTransformer` integration.
 
         Args:
             config (`transformers.PretrainedConfig`):
                 The config of the model.
         """
-        super().__init__()
         self.norm_first = False
         self.use_gelu = False
         self.act_fn = None
         self.pos_emb_type = None
         self.num_heads = None
         self.embed_dim = None
         self.num_layers = None
         self.original_layers_mapping = {}
         self.module_mapping = None
-        self.is_decoder = False
+        self.supports_training = False
         # Some models does not have some attributes thus needs to be ignored
         # e.g. whisper does not have self_attn.k_proj.bias but has self_attn.v_proj.bias & self_attn.q_proj.bias
         self.keys_to_ignore = []
 
         # Get activation function
         for attr in KNOWN_ACTIVATION_ATTRIBUTES:
             if hasattr(config, attr):
@@ -129,15 +127,15 @@
                 f" Number of heads must be even."
             )
 
     def forward_checker(self, *args, **kwargs):
         if torch.is_autocast_enabled() or torch.is_autocast_cpu_enabled():
             raise ValueError("Autocast is not supported for `BetterTransformer` integration.")
 
-        if self.training and not self.is_decoder:
+        if self.training and not self.supports_training:
             raise ValueError(
                 "Training is not supported for `BetterTransformer` integration.",
                 " Please use `model.eval()` before running the model.",
             )
 
     def _revert(self, module: torch.nn.Module) -> torch.nn.Module:
         if self.module_mapping is not None:
```

### Comparing `optimum-1.7.3/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.8.0/optimum/bettertransformer/models/encoder_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 from .base import BetterTransformerBaseLayer
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig
 
 
-class AlbertLayerBetterTransformer(BetterTransformerBaseLayer):
+class AlbertLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, albert_layer, config):
         r"""
         A simple conversion of the ALBERT layer to its `BetterTransformer` implementation.
 
         Args:
             albert_layer (`torch.nn.Module`):
                 The original ALBERT Layer where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     albert_layer.attention.query.weight,
                     albert_layer.attention.key.weight,
                     albert_layer.attention.value.weight,
@@ -141,24 +142,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class BertLayerBetterTransformer(BetterTransformerBaseLayer):
+class BertLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, bert_layer, config):
         r"""
         A simple conversion of the BERT layer to its `BetterTransformer` implementation.
 
         Args:
             bert_layer (`torch.nn.Module`):
                 The original BERT Layer where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     bert_layer.attention.self.query.weight,
                     bert_layer.attention.self.key.weight,
                     bert_layer.attention.self.value.weight,
@@ -267,24 +269,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class BartEncoderLayerBetterTransformer(BetterTransformerBaseLayer):
+class BartEncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, bart_layer, config):
         r"""
         A simple conversion of the `BartEncoderLayer` to its `BetterTransformer` implementation.
 
         Args:
             bart_layer (`torch.nn.Module`):
                 The original `BartEncoderLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     bart_layer.self_attn.q_proj.weight,
                     bart_layer.self_attn.k_proj.weight,
                     bart_layer.self_attn.v_proj.weight,
@@ -400,23 +403,24 @@
         if not self.is_last_layer:
             hidden_states.original_shape = original_shape
         elif hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0, original_shape)
         return (hidden_states,)
 
 
-class MBartEncoderLayerBetterTransformer(BetterTransformerBaseLayer):
+class MBartEncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, mbart_layer, config):
         r"""
         A simple conversion of the `MBartEncoderLayer` to its `BetterTransformer` implementation.
         Args:
             mbart_layer (`torch.nn.Module`):
                 The original `MBartEncoderLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     mbart_layer.self_attn.q_proj.weight,
                     mbart_layer.self_attn.k_proj.weight,
                     mbart_layer.self_attn.v_proj.weight,
@@ -537,24 +541,25 @@
         if not self.is_last_layer:
             hidden_states.original_shape = original_shape
         elif hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0, original_shape)
         return (hidden_states,)
 
 
-class DistilBertLayerBetterTransformer(BetterTransformerBaseLayer):
+class DistilBertLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, bert_layer, config):
         r"""
         A simple conversion of the Distill-BERTLayer to its `BetterTransformer` implementation.
 
         Args:
             bert_layer (`torch.nn.Module`):
                 The original Distill-BERT Layer where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     bert_layer.attention.q_lin.weight,
                     bert_layer.attention.k_lin.weight,
                     bert_layer.attention.v_lin.weight,
@@ -660,24 +665,25 @@
             attn_mask,
         )
         if x.is_nested and self.is_last_layer:
             x = x.to_padded_tensor(0.0)
         return (x,)
 
 
-class WhisperEncoderLayerBetterTransformer(BetterTransformerBaseLayer):
+class WhisperEncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, whisper_layer, config):
         r"""
         A simple conversion of the WhisperEncoderLayer to its `BetterTransformer` implementation.
 
         Args:
             whisper_layer (`torch.nn.Module`):
                 The original `WhisperEncoderLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     whisper_layer.self_attn.q_proj.weight,
                     whisper_layer.self_attn.k_proj.weight,
                     whisper_layer.self_attn.v_proj.weight,
@@ -772,24 +778,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class ViTLayerBetterTransformer(BetterTransformerBaseLayer):
+class ViTLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, vit_layer, config):
         r"""
         A simple conversion of the ViTLayer to its `BetterTransformer` implementation.
 
         Args:
             vit_layer (`torch.nn.Module`):
                 The original `ViTLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     vit_layer.attention.attention.query.weight,
                     vit_layer.attention.attention.key.weight,
                     vit_layer.attention.attention.value.weight,
@@ -891,24 +898,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class ViltLayerBetterTransformer(BetterTransformerBaseLayer):
+class ViltLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, vilt_layer, config):
         r"""
         A simple conversion of the VilTLayer to its `BetterTransformer` implementation.
 
         Args:
             vilt_layer (`torch.nn.Module`):
                 The original `VilTLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     vilt_layer.attention.attention.query.weight,
                     vilt_layer.attention.attention.key.weight,
                     vilt_layer.attention.attention.value.weight,
@@ -1010,24 +1018,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class Wav2Vec2EncoderLayerBetterTransformer(BetterTransformerBaseLayer):
+class Wav2Vec2EncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, wav2vec2_layer, config):
         r"""
         A simple conversion of the Wav2Vec2EncoderLayer to its `BetterTransformer` implementation.
 
         Args:
             wav2vec2_layer (`torch.nn.Module`):
                 The original `Wav2Vec2EncoderLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     wav2vec2_layer.attention.q_proj.weight,
                     wav2vec2_layer.attention.k_proj.weight,
                     wav2vec2_layer.attention.v_proj.weight,
@@ -1136,24 +1145,25 @@
             attention_mask,
         )
         if hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0)
         return (hidden_states,)
 
 
-class FSMTEncoderLayerBetterTransformer(BetterTransformerBaseLayer):
+class FSMTEncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, fsmt_layer, config):
         r"""
         A simple conversion of the FSMT Encoder layer to its `BetterTransformer` implementation.
 
         Args:
             fsmt_layer (`torch.nn.Module`):
                 The original FSMT Layer where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     fsmt_layer.self_attn.q_proj.weight,
                     fsmt_layer.self_attn.k_proj.weight,
                     fsmt_layer.self_attn.v_proj.weight,
@@ -1271,26 +1281,161 @@
         if not self.is_last_layer:
             hidden_states.original_shape = original_shape
         elif hidden_states.is_nested and self.is_last_layer:
             hidden_states = hidden_states.to_padded_tensor(0.0, original_shape)
         return (hidden_states, attention_mask)
 
 
-class CLIPLayerBetterTransformer(BetterTransformerBaseLayer):
+class ProphetNetEncoderLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
+    def __init__(self, prophetnet_layer, config):
+        r"""
+        A simple conversion of the ProphetNet Encoder layer to its `BetterTransformer` implementation.
+
+        Args:
+            prophet_net_layer (`torch.nn.Module`):
+                The original ProphetNet Layer where the weights needs to be retrieved.
+        """
+        super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
+        self.config = config
+        # In_proj layer
+        self.in_proj_weight = nn.Parameter(
+            torch.cat(
+                [
+                    prophetnet_layer.self_attn.query_proj.weight,
+                    prophetnet_layer.self_attn.key_proj.weight,
+                    prophetnet_layer.self_attn.value_proj.weight,
+                ]
+            )
+        )
+        self.in_proj_bias = nn.Parameter(
+            torch.cat(
+                [
+                    prophetnet_layer.self_attn.query_proj.bias,
+                    prophetnet_layer.self_attn.key_proj.bias,
+                    prophetnet_layer.self_attn.value_proj.bias,
+                ]
+            )
+        )
+
+        # Out proj layer
+        self.out_proj_weight = prophetnet_layer.self_attn.out_proj.weight
+        self.out_proj_bias = prophetnet_layer.self_attn.out_proj.bias
+
+        # Linear layer 1
+        self.linear1_weight = prophetnet_layer.feed_forward.intermediate.weight
+        self.linear1_bias = prophetnet_layer.feed_forward.intermediate.bias
+
+        # Linear layer 2
+        self.linear2_weight = prophetnet_layer.feed_forward.output.weight
+        self.linear2_bias = prophetnet_layer.feed_forward.output.bias
+
+        # Layer norm 1
+        self.norm1_eps = prophetnet_layer.self_attn_layer_norm.eps
+        self.norm1_weight = prophetnet_layer.self_attn_layer_norm.weight
+        self.norm1_bias = prophetnet_layer.self_attn_layer_norm.bias
+
+        # Layer norm 2
+        self.norm2_eps = prophetnet_layer.feed_forward_layer_norm.eps
+        self.norm2_weight = prophetnet_layer.feed_forward_layer_norm.weight
+        self.norm2_bias = prophetnet_layer.feed_forward_layer_norm.bias
+
+        # Model hyper parameters
+        self.num_heads = prophetnet_layer.self_attn.num_attn_heads
+        self.embed_dim = prophetnet_layer.self_attn.head_dim * self.num_heads
+
+        # Last step: set the last layer to `False` -> this will be set to `True` when converting the model
+        self.is_last_layer = False
+
+        self.original_layers_mapping = {
+            "in_proj_weight": [
+                "self_attn.query_proj.weight",
+                "self_attn.key_proj.weight",
+                "self_attn.value_proj.weight",
+            ],
+            "in_proj_bias": ["self_attn.query_proj.bias", "self_attn.key_proj.bias", "self_attn.value_proj.bias"],
+            "out_proj_weight": "self_attn.out_proj.weight",
+            "out_proj_bias": "self_attn.out_proj.bias",
+            "linear1_weight": "feed_forward.intermediate.weight",
+            "linear1_bias": "feed_forward.intermediate.bias",
+            "linear2_weight": "feed_forward.output.weight",
+            "linear2_bias": "feed_forward.output.bias",
+            "norm1_weight": "self_attn_layer_norm.weight",
+            "norm1_bias": "self_attn_layer_norm.bias",
+            "norm2_weight": "feed_forward_layer_norm.weight",
+            "norm2_bias": "feed_forward_layer_norm.bias",
+        }
+
+        self.validate_bettertransformer()
+
+    def forward(self, hidden_states, attention_mask, *_, **__):
+        r"""
+        This is just a wrapper around the forward function proposed in:
+        https://github.com/huggingface/transformers/pull/19553
+        """
+        super().forward_checker()
+
+        if not hasattr(hidden_states, "original_shape"):
+            original_shape = hidden_states.shape
+        else:
+            original_shape = hidden_states.original_shape
+
+        if hidden_states.is_nested:
+            attention_mask = None
+
+        if attention_mask is not None:
+            # attention mask comes in with values 0 and -inf. we convert to torch.nn.TransformerEncoder style bool mask
+            # 0->false->keep this token -inf->true->mask this token
+            attention_mask = attention_mask.squeeze(1)[:, 0]
+            attention_mask = attention_mask.bool()
+            attention_mask = torch.reshape(attention_mask, (attention_mask.shape[0], attention_mask.shape[-1]))
+            hidden_states = torch._nested_tensor_from_mask(hidden_states, ~attention_mask)
+            attention_mask = None
+
+        hidden_states = torch._transformer_encoder_layer_fwd(
+            hidden_states,
+            self.embed_dim,
+            self.num_heads,
+            self.in_proj_weight,
+            self.in_proj_bias,
+            self.out_proj_weight,
+            self.out_proj_bias,
+            self.use_gelu,
+            self.norm_first,
+            self.norm1_eps,
+            self.norm1_weight,
+            self.norm1_bias,
+            self.norm2_weight,
+            self.norm2_bias,
+            self.linear1_weight,
+            self.linear1_bias,
+            self.linear2_weight,
+            self.linear2_bias,
+            attention_mask,
+        )
+        if not self.is_last_layer:
+            hidden_states.original_shape = original_shape
+        elif hidden_states.is_nested and self.is_last_layer:
+            hidden_states = hidden_states.to_padded_tensor(0.0, original_shape)
+        return (hidden_states,)
+
+
+class CLIPLayerBetterTransformer(BetterTransformerBaseLayer, nn.Module):
     def __init__(self, layer, config):
         r"""
         A simple conversion of the CLIPEncoderLayer to its `BetterTransformer` implementation.
 
         **The implementation is valid only for the vision model, that does not use `causal_attention_mask`.**
 
         Args:
             layer (`torch.nn.Module`):
                 The original `CLIPEncoderLayer` where the weights needs to be retrieved.
         """
         super().__init__(config)
+        super(BetterTransformerBaseLayer, self).__init__()
         # In_proj layer
         self.in_proj_weight = nn.Parameter(
             torch.cat(
                 [
                     layer.self_attn.q_proj.weight,
                     layer.self_attn.k_proj.weight,
                     layer.self_attn.v_proj.weight,
```

### Comparing `optimum-1.7.3/optimum/bettertransformer/transformation.py` & `optimum-1.8.0/optimum/bettertransformer/transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         Returns:
             The converted model if the conversion has been successful.
         """
 
         # Check if we have to load the model using `accelerate`
         if hasattr(model, "hf_device_map"):
             load_accelerate = True
+            hf_device_map = model.hf_device_map
         else:
             load_accelerate = False
 
         if hasattr(model, "use_bettertransformer") and model.use_bettertransformer is True:
             raise Exception(
                 "`BetterTransform.transform()` was called on a model already using Better Transformer modeling."
             )
@@ -220,16 +221,15 @@
             raise ValueError(
                 f"BetterTransformer for {model.config.model_type} requires torch>=2.0 but {torch.__version__} is installed. Please upgrade PyTorch."
             )
 
         hf_config = model.config
 
         if load_accelerate:
-            # remove the hooks from the original model to
-            # avoid weights being on `meta` device.
+            # Remove the hooks from the original model to avoid weights being on `meta` device.
             remove_hook_from_module(model, recurse=True)
 
         if keep_original_model:
             try:
                 if not check_if_pytorch_greater(2.0, "Please upgrade PyTorch to >=2.0 to use training mode"):
                     model = model.requires_grad_(False)
                 model_fast = deepcopy(model)
@@ -245,32 +245,46 @@
         else:
             model_fast = replace_to_bettertransformer(model, hf_config).eval()
             model = None
 
         if BetterTransformerManager.requires_nested_tensor(model_fast.config.model_type):
             set_last_layer(model_fast)
 
-        # Step 6: Add a class arguments, we might need to identify whether the model
+        # Add a class arguments, we might need to identify whether the model
         # has been correctly converted to its `BetterTransformer` version.
         setattr(model_fast, "use_bettertransformer", True)
 
-        # Step 7: dispatch model if `accelerate` is enabled
         if load_accelerate:
-            device_map_bt = infer_auto_device_map(model_fast, max_memory=max_memory)
+            all_model_tensors = [name for name, _ in model_fast.state_dict().items()]
+            for module_name in hf_device_map.keys():
+                all_model_tensors = [name for name in all_model_tensors if not name.startswith(module_name)]
+
+            if len(all_model_tensors) > 0:
+                # This is the case where a transformed submodule is broken into several devices:
+                # as the submodules map may differ, we need to reinfer the device map
+                bt_device_map = infer_auto_device_map(model_fast, max_memory=max_memory)
+            else:
+                bt_device_map = hf_device_map
 
-            remove_hook_from_module(model_fast, recurse=True)
-
-            model_fast = dispatch_model(model_fast, device_map_bt)
+            model_fast = dispatch_model(model_fast, bt_device_map)
 
+            # It is not recommended to have `keep_original_model=True` with a model
+            # that is loaded with accelerate but just in case
             if keep_original_model:
-                # It is not recommended to have `keep_original_model=True` with a model
-                # that is loaded with accelerate but just in case ..
-                model = dispatch_model(model, model.hf_device_map)
+                model = dispatch_model(model, hf_device_map)
+
+        # See: https://github.com/pytorch/pytorch/issues/96099
+        if BetterTransformerManager.requires_torch_20(model_fast.config.model_type):
+            logging.warning(
+                f"For training, the BetterTransformer implementation for {model_fast.config.model_type} "
+                " architecture currently does not support padding as fused kernels do not support custom"
+                " attention masks. Beware that passing padded batched training data may result in unexpected outputs."
+            )
 
-        # Step 8: overwrite the `save_pretrained` method
+        # Overwrite the `save_pretrained` method
         # by raising an error if the user tries to save the model
         # or push it to the hub.
         model_fast._old_save_pretrained = model_fast.save_pretrained
         model_fast._old_push_to_hub = model_fast.push_to_hub
 
         model_fast.save_pretrained = raise_save_or_push_incompatible
         model_fast.push_to_hub = raise_save_or_push_incompatible
```

### Comparing `optimum-1.7.3/optimum/commands/__init__.py` & `optimum-1.8.0/optimum/exporters/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,21 @@
+# coding=utf-8
 # Copyright 2022 The HuggingFace Team. All rights reserved.
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
+"""Base exporters config."""
 
-from abc import ABC, abstractmethod
-from argparse import ArgumentParser
+from abc import ABC
 
 
-class BaseOptimumCLICommand(ABC):
-    @staticmethod
-    @abstractmethod
-    def register_subcommand(parser: ArgumentParser):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def run(self):
-        raise NotImplementedError()
+class ExportConfig(ABC):
+    pass
```

### Comparing `optimum-1.7.3/optimum/commands/env.py` & `optimum-1.8.0/optimum/commands/env.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,33 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import platform
-from argparse import ArgumentParser
 
 import huggingface_hub
 from transformers import __version__ as transformers_version
 from transformers.utils import is_tf_available, is_torch_available
 
 from ..version import __version__ as version
-from . import BaseOptimumCLICommand
-
-
-def info_command_factory(_):
-    return EnvironmentCommand()
+from . import BaseOptimumCLICommand, CommandInfo
 
 
 class EnvironmentCommand(BaseOptimumCLICommand):
+    COMMAND = CommandInfo(name="env", help="Get information about the environment used.")
+
     @staticmethod
-    def register_subcommand(parser: ArgumentParser):
-        download_parser = parser.add_parser("env", help="Get information about the environment used.")
-        download_parser.set_defaults(func=info_command_factory)
+    def format_dict(d):
+        return "\n".join([f"- {prop}: {val}" for prop, val in d.items()]) + "\n"
 
     def run(self):
         pt_version = "not installed"
         pt_cuda_available = "NA"
         if is_torch_available():
             import torch
 
@@ -65,11 +61,7 @@
             "Tensorflow version (GPU?)": f"{tf_version} (cuda availabe: {tf_cuda_available})",
         }
 
         print("\nCopy-and-paste the text below in your GitHub issue:\n")
         print(self.format_dict(info))
 
         return info
-
-    @staticmethod
-    def format_dict(d):
-        return "\n".join([f"- {prop}: {val}" for prop, val in d.items()]) + "\n"
```

### Comparing `optimum-1.7.3/optimum/commands/export/ggml.py` & `optimum-1.8.0/optimum/commands/export/ggml.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/commands/export/tflite.py` & `optimum-1.8.0/optimum/commands/export/tflite.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Defines the command line for the export with TensorFlow Lite."""
 
 import subprocess
+import sys
 from pathlib import Path
+from typing import TYPE_CHECKING, Optional
 
 from ...exporters import TasksManager
 from ...exporters.tflite import QuantizationApproach
+from ..base import BaseOptimumCLICommand
 
 
-def parse_args_tflite(parser):
+if TYPE_CHECKING:
+    from argparse import ArgumentParser, Namespace, _SubParsersAction
+
+    from ..base import CommandInfo
+
+
+def parse_args_tflite(parser: "ArgumentParser"):
     required_group = parser.add_argument_group("Required arguments")
     required_group.add_argument(
         "-m", "--model", type=str, required=True, help="Model ID on huggingface.co or path on disk to load model from."
     )
     required_group.add_argument(
         "output", type=Path, help="Path indicating the directory where to store generated TFLite model."
     )
@@ -151,15 +160,15 @@
 
     calibration_dataset_group = parser.add_argument_group("Quantization Calibration dataset")
     calibration_dataset_group.add_argument(
         "--calibration_dataset",
         type=str,
         default=None,
         help=(
-            "The dataset to use to calibration integer ranges when quantizing the model. This is needed to perform "
+            "The dataset to use to calibrate integer ranges when quantizing the model. This is needed to perform "
             "static quantization."
         ),
     )
     calibration_dataset_group.add_argument(
         "--calibration_dataset_config_name",
         type=str,
         default=None,
@@ -176,24 +185,24 @@
     )
     calibration_dataset_group.add_argument(
         "--primary_key",
         type=str,
         default=None,
         help=(
             "The name of the column in the dataset containing the main data to preprocess. "
-            "Only for sequence-classification and token-classification. "
+            "Only for text-classification and token-classification. "
         ),
     )
     calibration_dataset_group.add_argument(
         "--secondary_key",
         type=str,
         default=None,
         help=(
             "The name of the second column in the dataset containing the main data to preprocess, not always needed. "
-            "Only for sequence-classification and token-classification. "
+            "Only for text-classification and token-classification. "
         ),
     )
     calibration_dataset_group.add_argument(
         "--question_key",
         type=str,
         default=None,
         help=("The name of the column containing the question in the dataset. Only for question-answering."),
@@ -208,14 +217,26 @@
         "--image_key",
         type=str,
         default=None,
         help=("The name of the column containing the image in the dataset. Only for image-classification."),
     )
 
 
-class TFLiteExportCommand:
-    def __init__(self, args_string):
-        self.args_string = args_string
+class TFLiteExportCommand(BaseOptimumCLICommand):
+    def __init__(
+        self,
+        parser: "_SubParsersAction",
+        args: Optional["Namespace"] = None,
+        command: Optional["CommandInfo"] = None,
+        from_defaults_factory: bool = False,
+    ):
+        super().__init__(parser, args, command=command, from_defaults_factory=from_defaults_factory)
+        # TODO: hack until TFLiteExportCommand does not use subprocess anymore.
+        self.args_string = " ".join(sys.argv[3:])
+
+    @staticmethod
+    def parse_args(parser: "ArgumentParser"):
+        return parse_args_tflite(parser)
 
     def run(self):
         full_command = f"python3 -m optimum.exporters.tflite {self.args_string}"
         subprocess.run(full_command, shell=True, check=True)
```

### Comparing `optimum-1.7.3/optimum/configuration_utils.py` & `optimum-1.8.0/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/conftest.py` & `optimum-1.8.0/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/__init__.py` & `optimum-1.8.0/optimum/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/error_utils.py` & `optimum-1.8.0/optimum/exporters/error_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/onnx/__init__.py` & `optimum-1.8.0/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/onnx/__main__.py` & `optimum-1.8.0/optimum/exporters/onnx/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import argparse
 from pathlib import Path
 
 from transformers import AutoTokenizer
 from transformers.utils import is_torch_available
 
+from ...commands.export.onnx import parse_args_onnx
 from ...utils import DEFAULT_DUMMY_SHAPES, logging
 from ...utils.save_utils import maybe_save_preprocessors
 from ..error_utils import AtolError, OutputMatchError, ShapeError
 from ..tasks import TasksManager
 from .base import OnnxConfigWithPast
 from .convert import export_models, validate_models_outputs
 from .utils import (
@@ -39,175 +40,14 @@
 from typing import Optional, Union
 
 
 logger = logging.get_logger()
 logger.setLevel(logging.INFO)
 
 
-def parse_args_onnx(parser):
-    required_group = parser.add_argument_group("Required arguments")
-    required_group.add_argument(
-        "-m", "--model", type=str, required=True, help="Model ID on huggingface.co or path on disk to load model from."
-    )
-    required_group.add_argument(
-        "output", type=Path, help="Path indicating the directory where to store the generated ONNX model."
-    )
-
-    optional_group = parser.add_argument_group("Optional arguments")
-    optional_group.add_argument(
-        "--task",
-        default="auto",
-        help=(
-            "The task to export the model for. If not specified, the task will be auto-inferred based on the model. Available tasks depend on the model, but are among:"
-            f" {str(list(TasksManager._TASKS_TO_AUTOMODELS.keys()))}. For decoder models, use `xxx-with-past` to export the model using past key values in the decoder."
-        ),
-    )
-    optional_group.add_argument(
-        "--opset",
-        type=int,
-        default=None,
-        help="If specified, ONNX opset version to export the model with. Otherwise, the default opset for the given model architecture will be used.",
-    )
-    optional_group.add_argument(
-        "--device",
-        type=str,
-        default="cpu",
-        help='The device to use to do the export. Defaults to "cpu".',
-    )
-    optional_group.add_argument(
-        "--fp16",
-        action="store_true",
-        help="Use half precision during the export. PyTorch-only, requires `--device cuda`.",
-    )
-    optional_group.add_argument(
-        "--optimize",
-        type=str,
-        default=None,
-        choices=["O1", "O2", "O3", "O4"],
-        help=(
-            "Allows to run ONNX Runtime optimizations directly during the export. Some of these optimizations are specific to ONNX Runtime, and the resulting ONNX will not be usable with other runtime as OpenVINO or TensorRT. Possible options:\n"
-            "    - O1: Basic general optimizations\n"
-            "    - O2: Basic and extended general optimizations, transformers-specific fusions\n"
-            "    - O3: Same as O2 with GELU approximation\n"
-            "    - O4: Same as O3 with mixed precision (fp16, GPU-only, requires `--device cuda`)"
-        ),
-    )
-    optional_group.add_argument(
-        "--monolith",
-        action="store_true",
-        help=(
-            "Forces to export the model as a single ONNX file. By default, the ONNX exporter may break the model in several"
-            " ONNX files, for example for encoder-decoder models where the encoder should be run only once while the"
-            " decoder is looped over."
-        ),
-    )
-    optional_group.add_argument(
-        "--no-post-process",
-        action="store_true",
-        help=(
-            "Allows to disable any post-processing done by default on the exported ONNX models. For example, the merging of decoder"
-            " and decoder-with-past models into a single ONNX model file to reduce memory usage."
-        ),
-    )
-    optional_group.add_argument(
-        "--framework",
-        type=str,
-        choices=["pt", "tf"],
-        default=None,
-        help=(
-            "The framework to use for the ONNX export."
-            " If not provided, will attempt to use the local checkpoint's original framework"
-            " or what is available in the environment."
-        ),
-    )
-    optional_group.add_argument(
-        "--atol",
-        type=float,
-        default=None,
-        help="If specified, the absolute difference tolerance when validating the model. Otherwise, the default atol for the model will be used.",
-    )
-    optional_group.add_argument("--cache_dir", type=str, default=None, help="Path indicating where to store cache.")
-    optional_group.add_argument(
-        "--trust-remote-code",
-        action="store_true",
-        help="Allows to use custom code for the modeling hosted in the model repository. This option should only be set for repositories you trust and in which you have read the code, as it will execute on your local machine arbitrary code present in the model repository.",
-    )
-    optional_group.add_argument(
-        "--pad_token_id",
-        type=int,
-        default=None,
-        help=(
-            "This is needed by some models, for some tasks. If not provided, will attempt to use the tokenizer to guess"
-            " it."
-        ),
-    )
-
-    input_group = parser.add_argument_group(
-        "Input shapes (if necessary, this allows to override the shapes of the input given to the ONNX exporter, that requires an example input)."
-    )
-    doc_input = "to use in the example input given to the ONNX export."
-    input_group.add_argument(
-        "--batch_size",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["batch_size"],
-        help=f"Text tasks only. Batch size {doc_input}",
-    )
-    input_group.add_argument(
-        "--sequence_length",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["sequence_length"],
-        help=f"Text tasks only. Sequence length {doc_input}",
-    )
-    input_group.add_argument(
-        "--num_choices",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["num_choices"],
-        help=f"Text tasks only. Num choices {doc_input}",
-    )
-    input_group.add_argument(
-        "--width",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["width"],
-        help=f"Image tasks only. Width {doc_input}",
-    )
-    input_group.add_argument(
-        "--height",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["height"],
-        help=f"Image tasks only. Height {doc_input}",
-    )
-    input_group.add_argument(
-        "--num_channels",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["num_channels"],
-        help=f"Image tasks only. Number of channels {doc_input}",
-    )
-    input_group.add_argument(
-        "--feature_size",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["feature_size"],
-        help=f"Audio tasks only. Feature size {doc_input}",
-    )
-    input_group.add_argument(
-        "--nb_max_frames",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["nb_max_frames"],
-        help=f"Audio tasks only. Maximum number of frames {doc_input}",
-    )
-    input_group.add_argument(
-        "--audio_sequence_length",
-        type=int,
-        default=DEFAULT_DUMMY_SHAPES["audio_sequence_length"],
-        help=f"Audio tasks only. Audio sequence length {doc_input}",
-    )
-
-    # deprecated argument
-    parser.add_argument("--for-ort", action="store_true", help=argparse.SUPPRESS)
-
-
 def main_export(
     model_name_or_path: str,
     output: Union[str, Path],
     task: str = "auto",
     opset: Optional[int] = None,
     device: str = "cpu",
     fp16: Optional[bool] = False,
@@ -302,22 +142,15 @@
     if for_ort:
         logger.warning(
             "The option --for-ort was passed, but its behavior is now the default in the ONNX exporter"
             " and passing it is not required anymore."
         )
 
     original_task = task
-    # Infer the task
-    if task == "auto":
-        try:
-            task = TasksManager.infer_task_from_model(model_name_or_path)
-        except KeyError as e:
-            raise KeyError(
-                f"The task could not be automatically inferred. Please provide the argument --task with the task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
-            )
+    task = TasksManager.map_from_synonym(task)
 
     framework = TasksManager.determine_framework(model_name_or_path, subfolder=subfolder, framework=framework)
 
     if (framework == "tf" and fp16 is True) or not is_torch_available():
         raise ValueError("The --fp16 option is supported only for PyTorch.")
 
     if fp16 is True and device == "cpu":
@@ -343,14 +176,22 @@
         local_files_only=local_files_only,
         force_download=force_download,
         trust_remote_code=trust_remote_code,
         framework=framework,
         torch_dtype=torch_dtype,
     )
 
+    if task == "auto":
+        try:
+            task = TasksManager.infer_task_from_model(model_name_or_path)
+        except KeyError as e:
+            raise KeyError(
+                f"The task could not be automatically inferred. Please provide the argument --task with the task from {', '.join(TasksManager.get_all_tasks())}. Detailed error: {e}"
+            )
+
     if task != "stable-diffusion" and task + "-with-past" in TasksManager.get_supported_tasks_for_model_type(
         model.config.model_type.replace("_", "-"), "onnx"
     ):
         if original_task == "auto":  # Make -with-past the default if --task was not explicitely specified
             task = task + "-with-past"
         else:
             logger.info(
@@ -371,15 +212,15 @@
     if task != "stable-diffusion":
         onnx_config_constructor = TasksManager.get_exporter_config_constructor(model=model, exporter="onnx", task=task)
         onnx_config = onnx_config_constructor(model.config)
 
         needs_pad_token_id = (
             isinstance(onnx_config, OnnxConfigWithPast)
             and getattr(model.config, "pad_token_id", None) is None
-            and task in ["sequence_classification"]
+            and task in ["text-classification"]
         )
         if needs_pad_token_id:
             if pad_token_id is not None:
                 model.config.pad_token_id = pad_token_id
             else:
                 try:
                     tok = AutoTokenizer.from_pretrained(model_name_or_path)
@@ -401,14 +242,17 @@
         if atol is None:
             atol = onnx_config.ATOL_FOR_VALIDATION
             if isinstance(atol, dict):
                 atol = atol[task.replace("-with-past", "")]
 
         # Saving the model config and preprocessor as this is needed sometimes.
         model.config.save_pretrained(output)
+        generation_config = getattr(model, "generation_config", None)
+        if generation_config is not None:
+            generation_config.save_pretrained(output)
         maybe_save_preprocessors(model_name_or_path, output)
 
     if task == "stable-diffusion":
         onnx_files_subpaths = [
             "text_encoder/model.onnx",
             "unet/model.onnx",
             "vae_encoder/model.onnx",
@@ -418,29 +262,36 @@
         # Saving the additional components needed to perform inference.
         model.tokenizer.save_pretrained(output.joinpath("tokenizer"))
         model.scheduler.save_pretrained(output.joinpath("scheduler"))
         if model.feature_extractor is not None:
             model.feature_extractor.save_pretrained(output.joinpath("feature_extractor"))
         model.save_config(output)
     else:
-        if model.config.is_encoder_decoder and task.startswith("causal-lm"):
+        if model.config.is_encoder_decoder and task.startswith("text-generation"):
             raise ValueError(
                 f"model.config.is_encoder_decoder is True and task is `{task}`, which are incompatible. If the task was auto-inferred, please fill a bug report"
                 f"at https://github.com/huggingface/optimum, if --task was explicitely passed, make sure you selected the right task for the model,"
                 f" referring to `optimum.exporters.tasks.TaskManager`'s `_TASKS_TO_AUTOMODELS`."
             )
 
         onnx_files_subpaths = None
         if (
             model.config.is_encoder_decoder
-            and task.startswith(("seq2seq-lm", "speech2seq-lm", "vision2seq-lm", "default-with-past"))
+            and task.startswith(
+                (
+                    "text2text-generation",
+                    "automatic-speech-recognition",
+                    "image-to-text",
+                    "feature-extraction-with-past",
+                )
+            )
             and not monolith
         ):
             models_and_onnx_configs = get_encoder_decoder_models_for_export(model, onnx_config)
-        elif task.startswith("causal-lm") and not monolith:
+        elif task.startswith("text-generation") and not monolith:
             models_and_onnx_configs = get_decoder_models_for_export(model, onnx_config)
         else:
             models_and_onnx_configs = {"model": (model, onnx_config)}
 
     _, onnx_outputs = export_models(
         models_and_onnx_configs=models_and_onnx_configs,
         opset=opset,
@@ -469,14 +320,15 @@
         optimization_config.disable_shape_inference = True
         optimizer.optimize(save_dir=output, optimization_config=optimization_config, file_suffix="")
 
     # Optionally post process the obtained ONNX file(s), for example to merge the decoder / decoder with past if any
     # TODO: treating stable diffusion separately is quite ugly
     if not no_post_process and task != "stable-diffusion":
         try:
+            logger.info("Post-processing the exported models...")
             models_and_onnx_configs, onnx_files_subpaths = onnx_config.post_process_exported_models(
                 output, models_and_onnx_configs, onnx_files_subpaths
             )
         except Exception as e:
             raise Exception(
                 f"The post-processing of the ONNX export failed. The export can still be performed by passing the option --no-post-process. Detailed error: {e}"
             )
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/base.py` & `optimum-1.8.0/optimum/exporters/onnx/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,36 +18,38 @@
 import enum
 import gc
 import inspect
 import itertools
 import re
 from abc import ABC, abstractmethod
 from collections import OrderedDict
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 from transformers.utils import is_torch_available
 
+from ...onnx import merge_decoders
 from ...utils import (
     DEFAULT_DUMMY_SHAPES,
     DummyInputGenerator,
     DummyLabelsGenerator,
+    DummySeq2SeqPastKeyValuesGenerator,
     is_diffusers_available,
     logging,
 )
 from ...utils import TORCH_MINIMUM_VERSION as GLOBAL_MIN_TORCH_VERSION
 from ...utils.doc import add_dynamic_docstring
 from ...utils.import_utils import is_onnx_available, is_onnxruntime_available
 from ..base import ExportConfig
+from .constants import ONNX_DECODER_MERGED_NAME, ONNX_DECODER_NAME, ONNX_DECODER_WITH_PAST_NAME, ONNX_ENCODER_NAME
 from .model_patcher import ModelPatcher, Seq2SeqModelPatcher
 
 
 if TYPE_CHECKING:
-    from pathlib import Path
-
     from transformers import PretrainedConfig, PreTrainedModel, TFPreTrainedModel
 
     if is_diffusers_available():
         from diffusers import ModelMixin
 
     from .model_patcher import PatchingSpec
 
@@ -103,61 +105,60 @@
     - PATCHING_SPECS (`Optional[List[PatchingSpec]]`, defaults to `None`) -- Specify which operators / modules should be
     patched before performing the export, and how. This is useful when some operator is not supported in ONNX for
     instance.
 
     Args:
         config (`transformers.PretrainedConfig`):
             The model configuration.
-        task (`str`, defaults to `"default"`):
+        task (`str`, defaults to `"feature-extraction"`):
             The task the model should be exported for.
     """
 
     NORMALIZED_CONFIG_CLASS = None
     DUMMY_INPUT_GENERATOR_CLASSES = ()
     DEFAULT_ONNX_OPSET = 11
     ATOL_FOR_VALIDATION: Union[float, Dict[str, float]] = 1e-5
     MIN_TORCH_VERSION = GLOBAL_MIN_TORCH_VERSION
     PATCHING_SPECS: Optional[List["PatchingSpec"]] = None
     _TASK_TO_COMMON_OUTPUTS = {
         "audio-classification": OrderedDict({"logits": {0: "batch_size"}}),
         "audio-frame-classification": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
-        "audio-ctc": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "automatic-speech-recognition": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "audio-xvector": OrderedDict({"logits": {0: "batch_size"}, "embeddings": {0: "batch_size"}}),
-        "causal-lm": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
-        "default": OrderedDict({"last_hidden_state": {0: "batch_size", 1: "sequence_length"}}),
+        "text-generation": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "feature-extraction": OrderedDict({"last_hidden_state": {0: "batch_size", 1: "sequence_length"}}),
         "image-classification": OrderedDict({"logits": {0: "batch_size"}}),
         # TODO: Is this the same thing as semantic-segmentation?
         "image-segmentation": OrderedDict(
             {
                 "logits": {0: "batch_size", 1: "num_queries"},
                 "pred_boxes": {0: "batch_size", 1: "num_queries"},
                 "pred_masks": {0: "batch_size", 1: "num_queries"},
             }
         ),
         "masked-im": OrderedDict({"logits": {0: "batch_size"}}),
-        "masked-lm": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "fill-mask": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "multiple-choice": OrderedDict({"logits": {0: "batch_size", 1: "num_choices"}}),
         "object-detection": OrderedDict(
             {
                 "logits": {0: "batch_size", 1: "num_queries"},
                 "pred_boxes": {0: "batch_size", 1: "num_queries"},
             }
         ),
         "question-answering": OrderedDict(
             {
                 "start_logits": {0: "batch_size", 1: "sequence_length"},
                 "end_logits": {0: "batch_size", 1: "sequence_length"},
             }
         ),
         "semantic-segmentation": OrderedDict({"logits": {0: "batch_size", 1: "num_labels", 2: "height", 3: "width"}}),
-        "seq2seq-lm": OrderedDict({"logits": {0: "batch_size", 1: "decoder_sequence_length"}}),
-        "sequence-classification": OrderedDict({"logits": {0: "batch_size"}}),
-        "speech2seq-lm": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "text2text-generation": OrderedDict({"logits": {0: "batch_size", 1: "decoder_sequence_length"}}),
+        "text-classification": OrderedDict({"logits": {0: "batch_size"}}),
         "token-classification": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
-        "vision2seq-lm": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
+        "image-to-text": OrderedDict({"logits": {0: "batch_size", 1: "sequence_length"}}),
         "zero-shot-image-classification": OrderedDict(
             {
                 "logits_per_image": {0: "image_batch_size", 1: "text_batch_size"},
                 "logits_per_text": {0: "text_batch_size", 1: "image_batch_size"},
                 "text_embeds": {0: "text_batch_size"},
                 "image_embeds": {0: "image_batch_size"},
             }
@@ -165,15 +166,15 @@
         # TODO: enable that and verify that once OwlViTOnnxConfig can work.
         # "zero-shot-object-detection": OrderedDict({
         #     "logits": {0: "batch_size"},
         #     "pred_boxes": {0: "batch_size"},
         # }),
     }
 
-    def __init__(self, config: "PretrainedConfig", task: str = "default"):
+    def __init__(self, config: "PretrainedConfig", task: str = "feature-extraction"):
         if task not in self._TASK_TO_COMMON_OUTPUTS:
             raise ValueError(
                 f"{task} is not a supported task, supported tasks: {', '.join(self._TASK_TO_COMMON_OUTPUTS.keys())}"
             )
         self.task = task
 
         self._config = config
@@ -265,15 +266,15 @@
                 input_shapes = {}
             dummy_inputs = self.generate_dummy_inputs(framework="np", **input_shapes)
             dummy_inputs = self.generate_dummy_inputs_for_validation(dummy_inputs)
             onnx_inputs = {}
             for name, value in dummy_inputs.items():
                 if isinstance(value, (list, tuple)):
                     value = self.flatten_output_collection_property(name, value)
-                    onnx_inputs.update({tensor_name: tensor for tensor_name, tensor in value.items()})
+                    onnx_inputs.update(dict(value.items()))
                 else:
                     onnx_inputs[name] = value
             for name, value in onnx_inputs.items():
                 if value.dtype == np.float32 and dtype == "fp16":
                     onnx_inputs[name] = onnx_inputs[name].astype(np.float16)
             outputs = session.run(None, onnx_inputs)
             del session
@@ -454,15 +455,15 @@
     PAD_ATTENTION_MASK_TO_PAST: bool = False
     USE_PAST_IN_INPUTS: Optional[bool] = None
     USE_PRESENT_IN_OUTPUTS: Optional[bool] = None
 
     def __init__(
         self,
         config: "PretrainedConfig",
-        task: str = "default",
+        task: str = "feature-extraction",
         use_past: bool = False,
         use_past_in_inputs: Optional[bool] = None,
         use_present_in_outputs: Optional[bool] = None,
     ):
         self.use_past = use_past
         if use_past_in_inputs is None:
             use_past_in_inputs = self.USE_PAST_IN_INPUTS
@@ -483,35 +484,35 @@
                 "of use_present_in_outputs value will be used for the outputs."
             )
         self.is_merged = False
         self.use_cache_branch = None
         super().__init__(config, task=task)
 
     @classmethod
-    def with_past(cls, config: "PretrainedConfig", task: str = "default") -> "OnnxConfigWithPast":
+    def with_past(cls, config: "PretrainedConfig", task: str = "feature-extraction") -> "OnnxConfigWithPast":
         """
         Instantiates a [`~optimum.exporters.onnx.OnnxConfig`] with `use_past` attribute set to `True`.
 
         Args:
             config (`transformers.PretrainedConfig`):
                 The underlying model's config to use when exporting to ONNX.
-            task (`str`, defaults to `"default"`):
+            task (`str`, defaults to `"feature-extraction"`):
                 The task the model should be exported for.
 
         Returns:
             [`~optimum.exporters.onnx.OnnxConfig`]: The onnx config with `.use_past = True`
         """
         return cls(config, task=task, use_past=True)
 
     @property
     def outputs(self) -> Dict[str, Dict[int, str]]:
         if self.use_past is False:
             common_outputs = super().outputs
         # In the other cases, the sequence_length axis is not dynamic, always of length 1
-        elif self.task == "default":
+        elif self.task == "feature-extraction":
             common_outputs = OrderedDict({"last_hidden_state": {0: "batch_size"}})
         else:
             common_outputs = OrderedDict({"logits": {0: "batch_size"}})
         if self.use_present_in_outputs:
             self.add_past_key_values(common_outputs, direction="outputs")
         return common_outputs
 
@@ -610,14 +611,30 @@
             for idx, t in enumerate(field):
                 self.flatten_past_key_values(flattened_output, name, idx, t)
         else:
             flattened_output = super().flatten_output_collection_property(name, field)
 
         return flattened_output
 
+    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+        if self.is_merged is True and self.use_cache_branch is True:
+            reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=True)
+        elif self.is_merged is True and self.use_cache_branch is False:
+            reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=False)
+
+            # We don't support optional inputs for now, so even though the non-cache branch is used,
+            # dummy past key values are necessary
+            batch_size = reference_model_inputs["input_ids"].shape[0]
+            pkv_generator = self.DUMMY_PKV_GENERATOR_CLASS(
+                task=self.task, normalized_config=self._normalized_config, sequence_length=1, batch_size=batch_size
+            )
+            reference_model_inputs["past_key_values"] = pkv_generator.generate("past_key_values", framework="pt")
+
+        return reference_model_inputs
+
 
 class ConfigBehavior(str, enum.Enum):
     """
     Specifies the behavior of the [`~exporters.onnx.base.OnnxSeq2SeqConfigWithPast`]:
         - MONOLITH: the config can be used to export the whole seq2seq model as a single file.
         - ENCODER: the config can be used to export the encoder part of the seq2seq model.
         - DECODER: the config can be used to export the decoder part of the seq2seq model.
@@ -629,18 +646,20 @@
 
 
 class OnnxSeq2SeqConfigWithPast(OnnxConfigWithPast):
     """
     Inherits from [`~exporters.onnx.OnnxConfigWithPast`]. A base class to handle the ONNX configuration of encoder-decoder models.
     """
 
+    DUMMY_PKV_GENERATOR_CLASS = DummySeq2SeqPastKeyValuesGenerator
+
     def __init__(
         self,
         config: "PretrainedConfig",
-        task: str = "default",
+        task: str = "feature-extraction",
         use_past: bool = False,
         use_past_in_inputs: Optional[bool] = None,
         use_present_in_outputs: Optional[bool] = None,
         behavior: ConfigBehavior = ConfigBehavior.MONOLITH,
     ):
         super().__init__(
             config,
@@ -651,15 +670,15 @@
         )
         self._behavior = behavior
         self.override_attributes_for_behavior()
 
     def override_attributes_for_behavior(self):
         """Override this to specify custom attribute change for a given behavior."""
         if self._behavior is ConfigBehavior.ENCODER:
-            self.task = "default"
+            self.task = "feature-extraction"
             self.use_past_in_inputs = False
             self.use_present_in_outputs = False
         if self._behavior is ConfigBehavior.DECODER:
             self.use_past_in_inputs = self.use_past
             self.use_present_in_outputs = True
 
     def with_behavior(
@@ -695,26 +714,23 @@
                 sequence_name = "encoder_sequence_length"
             else:
                 sequence_name = "decoder_sequence_length"
 
             new_axes_names = {}
             for axis_idx, axis_name in axes_names.items():
                 if "sequence" in axis_name:
-                    if not self.use_past_in_inputs:
+                    if self.use_past_in_inputs is False or self.is_merged is True:
                         new_axes_names[axis_idx] = sequence_name
                     else:
                         # Trick to force it since ONNX sometimes infer a dynamic axis where it's not.
                         new_axes_names[axis_idx] = "1"
                 else:
                     new_axes_names[axis_idx] = axis_name
             common_outputs[name] = new_axes_names
 
-        if self._behavior is not ConfigBehavior.ENCODER:
-            common_outputs["encoder_last_hidden_state"] = {0: "batch_size", 1: "encoder_sequence_length"}
-
         if self.use_present_in_outputs:
             self.add_past_key_values(common_outputs, direction="outputs")
 
         return common_outputs
 
     def add_past_key_values(self, inputs_or_outputs: Dict[str, Dict[int, str]], direction: str):
         if direction not in ["inputs", "outputs"]:
@@ -727,56 +743,125 @@
             decoder_sequence_name = "past_decoder_sequence_length + 1"
             name = "present"
 
         for i in range(self._normalized_config.decoder_num_layers):
             inputs_or_outputs[f"{name}.{i}.decoder.key"] = {0: "batch_size", 2: decoder_sequence_name}
             inputs_or_outputs[f"{name}.{i}.decoder.value"] = {0: "batch_size", 2: decoder_sequence_name}
 
-            if direction == "inputs" or (self._behavior is ConfigBehavior.DECODER and self.use_past is False):
-                inputs_or_outputs[f"{name}.{i}.encoder.key"] = {0: "batch_size", 2: "encoder_sequence_length"}
-                inputs_or_outputs[f"{name}.{i}.encoder.value"] = {0: "batch_size", 2: "encoder_sequence_length"}
-
-        if direction == "outputs" and "encoder_last_hidden_state" in inputs_or_outputs:
-            inputs_or_outputs.move_to_end("encoder_last_hidden_state")
+            if (
+                self.is_merged is True
+                or (self._behavior is ConfigBehavior.DECODER and self.use_past is False)
+                or direction == "inputs"
+            ):
+                # TODO: we only need to call it encoder_sequence_length_out in the merge case - but at torch.onnx.export()
+                # time we have currently no case to check whether we will merge at a later step or not (self.is_merged is
+                # not yet set at this time)
+                inputs_or_outputs[f"{name}.{i}.encoder.key"] = {0: "batch_size", 2: "encoder_sequence_length_out"}
+                inputs_or_outputs[f"{name}.{i}.encoder.value"] = {0: "batch_size", 2: "encoder_sequence_length_out"}
 
     def flatten_past_key_values(self, flattened_output, name, idx, t):
         flattened_output[f"{name}.{idx}.decoder.key"] = t[0]
         flattened_output[f"{name}.{idx}.decoder.value"] = t[1]
         flattened_output[f"{name}.{idx}.encoder.key"] = t[2]
         flattened_output[f"{name}.{idx}.encoder.value"] = t[3]
 
     def patch_model_for_export(self, model: Union["PreTrainedModel", "TFPreTrainedModel"]) -> ModelPatcher:
         return Seq2SeqModelPatcher(self, model)
 
+    def post_process_exported_models(
+        self,
+        path: Path,
+        models_and_onnx_configs: Dict[
+            str, Tuple[Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"], "OnnxConfig"]
+        ],
+        onnx_files_subpaths: List[str],
+    ):
+        # Attempt to merge only if the decoder was exported without/with past
+        if self.use_past is True and len(models_and_onnx_configs) == 3:
+            if onnx_files_subpaths is not None:
+                decoder_path = Path(path, onnx_files_subpaths[1])
+                decoder_with_past_path = Path(path, onnx_files_subpaths[2])
+            else:
+                decoder_path = Path(path, ONNX_DECODER_NAME + ".onnx")
+                decoder_with_past_path = Path(path, ONNX_DECODER_WITH_PAST_NAME + ".onnx")
+            decoder_merged_path = Path(path, ONNX_DECODER_MERGED_NAME + ".onnx")
+            try:
+                # The decoder with past does not output the cross attention past key values as they are constant,
+                # hence the need for strict=False
+                merge_decoders(
+                    decoder=decoder_path,
+                    decoder_with_past=decoder_with_past_path,
+                    save_path=decoder_merged_path,
+                    strict=False,
+                )
+            except Exception as e:
+                raise Exception(f"Unable to merge decoders. Detailed error: {e}")
+
+            # In order to do the validation of the two branches on the same file
+            if onnx_files_subpaths is not None:
+                encoder_path = onnx_files_subpaths[0]
+            else:
+                encoder_path = ONNX_ENCODER_NAME + ".onnx"
+
+            onnx_files_subpaths = [encoder_path, decoder_merged_path.name, decoder_merged_path.name]
+
+            # We validate the two branches of the decoder model then
+            models_and_onnx_configs[ONNX_DECODER_NAME][1].is_merged = True
+            models_and_onnx_configs[ONNX_DECODER_NAME][1].use_cache_branch = False
+
+            # Past key values won't be generated by default, but added in the input
+            models_and_onnx_configs[ONNX_DECODER_NAME][1].use_past = False
+            models_and_onnx_configs[ONNX_DECODER_NAME][1].use_past_in_inputs = True
+
+            models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].use_cache_branch = True
+            models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].is_merged = True
+
+        return models_and_onnx_configs, onnx_files_subpaths
+
+    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+        if self._behavior is ConfigBehavior.DECODER:
+            if "decoder_input_ids" in reference_model_inputs:
+                reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
+
+            if "encoder_outputs" in reference_model_inputs:
+                if self.use_past_in_inputs is False or self.is_merged:
+                    # ONNX without past uses encoder_hidden_states even when we don't outputing them
+                    reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+                else:
+                    # ONNX with past does not use encoder_hidden_states when we don't output them
+                    reference_model_inputs.pop("encoder_outputs")
+
+        return super().generate_dummy_inputs_for_validation(reference_model_inputs)
+
 
 class OnnxConfigWithLoss(OnnxConfig, ABC):
     """
     Wrapper for the children classes of `optimum.exporters.onnx.OnnxConfig` to export the model through the ONNX format
     with loss in outputs and labels in the inputs. For seq-to-seq models, labels will be appended to the inputs of
     decoders.
     """
 
     _tasks_to_extra_inputs = {
-        "default": {"labels": {0: "batch_size"}},
-        "masked-lm": {"labels": {0: "batch_size", 1: "sequence_length"}},
-        "causal-lm": {"labels": {0: "batch_size", 1: "sequence_length"}},
-        "causal-lm-with-past": {"labels": {0: "batch_size"}},
-        "seq2seq-lm": {"labels": {0: "batch_size", 1: "sequence_length"}},
-        "seq2seq-lm-with-past": {"labels": {0: "batch_size"}},
-        "sequence-classification": {"labels": {0: "batch_size"}},
+        "feature-extraction": {"labels": {0: "batch_size"}},
+        "fill-mask": {"labels": {0: "batch_size", 1: "sequence_length"}},
+        "text-generation": {"labels": {0: "batch_size", 1: "sequence_length"}},
+        "text-generation-with-past": {"labels": {0: "batch_size"}},
+        "text2text-generation": {"labels": {0: "batch_size", 1: "sequence_length"}},
+        "text2text-generation-with-past": {"labels": {0: "batch_size"}},
+        "text-classification": {"labels": {0: "batch_size"}},
         "token-classification": {"labels": {0: "batch_size", 1: "sequence_length"}},
         "multiple-choice": {"labels": {0: "batch_size"}},
         "question-answering": {
             "start_positions": {0: "batch_size"},
             "end_positions": {0: "batch_size"},
         },
         "image-classification": {"labels": {0: "batch_size"}},
     }
     _tasks_to_extra_outputs = {
-        "default": OrderedDict({"loss": {}}),
+        "feature-extraction": OrderedDict({"loss": {}}),
     }
 
     DUMMY_EXTRA_INPUT_GENERATOR_CLASSES = (DummyLabelsGenerator,)
 
     def __init__(self, config: OnnxConfig):
         self._onnx_config = config
         self.task = self._onnx_config.task
@@ -792,15 +877,15 @@
         inputs = self._onnx_config.inputs
         inputs.update(self._tasks_to_extra_inputs[self.task])
         return inputs
 
     @property
     def outputs(self) -> Dict[str, Dict[int, str]]:
         common_outputs = self._onnx_config.outputs
-        extra_outputs = self._tasks_to_extra_outputs["default"]
+        extra_outputs = self._tasks_to_extra_outputs["feature-extraction"]
         common_outputs.update(extra_outputs)
         for key in reversed(extra_outputs.keys()):
             common_outputs.move_to_end(key, last=False)
         return copy.deepcopy(common_outputs)
 
     def generate_dummy_inputs(self, framework: str = "pt", **kwargs):
         dummy_inputs = self._onnx_config.generate_dummy_inputs(framework=framework, **kwargs)
@@ -848,18 +933,18 @@
         flattened_output[f"{name}.{idx}.decoder.value"] = t[1]
         flattened_output[f"{name}.{idx}.encoder.key"] = t[2]
         flattened_output[f"{name}.{idx}.encoder.value"] = t[3]
 
     def flatten_output_collection_property(self, name: str, field: Iterable[Any]) -> Dict[str, Any]:
         flattened_output = {}
         if name in ["present", "past_key_values"]:
-            if "causal-lm" in self.task:
+            if "text-generation" in self.task:
                 for idx, t in enumerate(field):
                     self.flatten_decoder_past_key_values(flattened_output, name, idx, t)
-            elif "seq2seq-lm" in self.task:
+            elif "text2text-generation" in self.task:
                 for idx, t in enumerate(field):
                     self.flatten_seq2seq_past_key_values(flattened_output, name, idx, t)
         else:
             flattened_output = super().flatten_output_collection_property(name, field)
 
         return flattened_output
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/config.py` & `optimum-1.8.0/optimum/exporters/onnx/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Common ONNX configuration classes that handle most of the features for building model specific configurations."""
 
 from collections import OrderedDict
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Mapping, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from transformers.utils import is_tf_available
 
 from ...onnx import merge_decoders
 from ...utils import (
     DummyAudioInputGenerator,
     DummyBboxInputGenerator,
@@ -128,30 +128,14 @@
             models_and_onnx_configs[ONNX_DECODER_NAME][1].use_past_in_inputs = True
 
             models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].use_cache_branch = True
             models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1].is_merged = True
 
         return models_and_onnx_configs, onnx_files_subpaths
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Mapping[str, Any]) -> Mapping[str, Any]:
-        if self.is_merged is True and self.use_cache_branch is True:
-            reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=True)
-        elif self.is_merged is True and self.use_cache_branch is False:
-            reference_model_inputs["use_cache_branch"] = DummyInputGenerator.constant_tensor(shape=[1], value=False)
-
-            # We don't support optional inputs for now, so even though the non-cache branch is used,
-            # dummy past key values are necessary
-            batch_size = reference_model_inputs["input_ids"].shape[0]
-            pkv_generator = self.DUMMY_PKV_GENERATOR_CLASS(
-                task=self.task, normalized_config=self._normalized_config, sequence_length=1, batch_size=batch_size
-            )
-            reference_model_inputs["past_key_values"] = pkv_generator.generate("past_key_values", framework="pt")
-
-        return reference_model_inputs
-
 
 class TextSeq2SeqOnnxConfig(OnnxSeq2SeqConfigWithPast):
     """
     Handles encoder-decoder-based text architectures.
     """
 
     DUMMY_INPUT_GENERATOR_CLASSES = (
@@ -217,22 +201,14 @@
             dummy_text_input_generator,
             dummy_decoder_text_input_generator,
             dummy_seq2seq_past_key_values_generator,
         ]
 
         return dummy_inputs_generators
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
-        if self._behavior is ConfigBehavior.DECODER:
-            reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
-            reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
-            # TODO: validate that it should be removed.
-            # reference_model_inputs["encoder_attention_mask"] = reference_model_inputs.pop("attention_mask")
-        return reference_model_inputs
-
 
 class VisionOnnxConfig(OnnxConfig):
     """
     Handles vision architectures.
     """
 
     DUMMY_INPUT_GENERATOR_CLASSES = (DummyVisionInputGenerator,)
@@ -292,29 +268,22 @@
             return {
                 "decoder_input_ids": "input_ids",
                 "encoder_outputs": "encoder_hidden_states",
                 "attention_mask": "encoder_attention_mask",
             }
         return {}
 
-    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
-        if self._behavior is ConfigBehavior.DECODER:
-            reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
-            reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
-
-        return reference_model_inputs
-
 
 class EncoderDecoderOnnxConfig(OnnxSeq2SeqConfigWithPast):
     DUMMY_INPUT_GENERATOR_CLASSES = (DummyTextInputGenerator,)
 
     def __init__(
         self,
         config: "PretrainedConfig",
-        task: str = "default",
+        task: str = "feature-extraction",
         use_past: bool = False,
         use_past_in_inputs: Optional[bool] = None,
         use_present_in_outputs: Optional[bool] = None,
         behavior: ConfigBehavior = ConfigBehavior.MONOLITH,
     ):
         super().__init__(
             config,
@@ -327,22 +296,22 @@
 
         from ..tasks import TasksManager
 
         self.is_decoder_with_past = False
 
         if self._behavior is not ConfigBehavior.DECODER:
             encoder_onnx_config_constructor = TasksManager.get_exporter_config_constructor(
-                exporter="onnx", task="default", model_type=config.encoder.model_type
+                exporter="onnx", task="feature-extraction", model_type=config.encoder.model_type
             )
             self._encoder_onnx_config = encoder_onnx_config_constructor(config.encoder)
             self._normalized_config.ENCODER_NORMALIZED_CONFIG_CLASS = self._encoder_onnx_config._normalized_config
 
         if self._behavior is not ConfigBehavior.ENCODER:
             decoder_onnx_config_constructor = TasksManager.get_exporter_config_constructor(
-                exporter="onnx", task="default", model_type=config.decoder.model_type
+                exporter="onnx", task="feature-extraction", model_type=config.decoder.model_type
             )
             kwargs = {}
             if issubclass(decoder_onnx_config_constructor.func, OnnxConfigWithPast):
                 self.is_decoder_with_past = True
                 kwargs["use_past"] = use_past
             else:
                 self.use_present_in_outputs = False
@@ -387,21 +356,41 @@
         if self.is_decoder_with_past:
             return self._decoder_onnx_config.flatten_past_key_values(flattened_output, name, idx, t)
 
     def flatten_output_collection_property(self, name: str, field: Iterable[Any]) -> Dict[str, Any]:
         return self._decoder_onnx_config.flatten_output_collection_property(name, field)
 
     def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
-        if self._behavior is ConfigBehavior.DECODER:
-            reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
-            reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+        if self._behavior is ConfigBehavior.ENCODER:
+            return self._encoder_onnx_config.generate_dummy_inputs_for_validation(reference_model_inputs)
+        else:
+            if self._behavior is ConfigBehavior.DECODER:
+                reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
 
-        return reference_model_inputs
+                # for encoder-decoder custom models, always pass encoder_hidden_states as input
+                reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
 
-    @property
-    def outputs(self) -> Dict[str, Dict[int, str]]:
-        common_outputs = super().outputs
-        # This is handled by OnnxSeq2SeqConfigWithPast, but not by OnnxConfigWithPast, so we take care of this here to
-        # make sure this output is moved at the end.
-        if "encoder_last_hidden_state" in common_outputs:
-            common_outputs.move_to_end("encoder_last_hidden_state")
-        return common_outputs
+            return self._decoder_onnx_config.generate_dummy_inputs_for_validation(reference_model_inputs)
+
+    def post_process_exported_models(
+        self,
+        path: Path,
+        models_and_onnx_configs: Dict[
+            str, Tuple[Union["PreTrainedModel", "TFPreTrainedModel", "ModelMixin"], "OnnxConfig"]
+        ],
+        onnx_files_subpaths: List[str],
+    ):
+        models_and_onnx_configs, onnx_files_subpaths = super().post_process_exported_models(
+            path, models_and_onnx_configs, onnx_files_subpaths
+        )
+        if self.use_past is True and len(models_and_onnx_configs) == 3:
+            models_and_onnx_configs[ONNX_DECODER_NAME][1]._decoder_onnx_config.is_merged = True
+            models_and_onnx_configs[ONNX_DECODER_NAME][1]._decoder_onnx_config.use_cache_branch = False
+
+            # Past key values won't be generated by default, but added in the input
+            models_and_onnx_configs[ONNX_DECODER_NAME][1]._decoder_onnx_config.use_past = False
+            models_and_onnx_configs[ONNX_DECODER_NAME][1]._decoder_onnx_config.use_past_in_inputs = True
+
+            models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1]._decoder_onnx_config.use_cache_branch = True
+            models_and_onnx_configs[ONNX_DECODER_WITH_PAST_NAME][1]._decoder_onnx_config.is_merged = True
+
+        return models_and_onnx_configs, onnx_files_subpaths
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/constants.py` & `optimum-1.8.0/optimum/exporters/onnx/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/onnx/convert.py` & `optimum-1.8.0/optimum/exporters/onnx/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
                 # tuple.
                 onnx_export(
                     model,
                     (dummy_inputs,),
                     f=output.as_posix(),
                     input_names=input_names,
                     output_names=output_names,
-                    dynamic_axes={name: axes for name, axes in chain(inputs.items(), config.outputs.items())},
+                    dynamic_axes=dict(chain(inputs.items(), config.outputs.items())),
                     do_constant_folding=True,
                     opset_version=opset,
                 )
 
             # check if external data was exported
             # TODO: this is quite inefficient as we load in memory if models are <2GB without external data
             onnx_model = onnx.load(str(output), load_external_data=False)
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/model_configs.py` & `optimum-1.8.0/optimum/exporters/onnx/model_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,14 +204,19 @@
 
 
 class OPTOnnxConfig(TextDecoderOnnxConfig):
     DEFAULT_ONNX_OPSET = 13
     NORMALIZED_CONFIG_CLASS = NormalizedTextConfig
 
 
+class LlamaOnnxConfig(TextDecoderOnnxConfig):
+    DEFAULT_ONNX_OPSET = 13
+    NORMALIZED_CONFIG_CLASS = NormalizedTextConfig
+
+
 class BloomDummyPastKeyValuesGenerator(DummyPastKeyValuesGenerator):
     def generate(self, input_name: str, framework: str = "pt"):
         past_key_shape = (
             self.batch_size * self.num_attention_heads,
             self.hidden_size // self.num_attention_heads,
             self.sequence_length,
         )
@@ -296,14 +301,24 @@
         num_attention_heads="num_heads",
         encoder_num_layers="num_layers",
         decoder_num_layers="num_decoder_layers",
         key_value_dim="d_kv",
         allow_new=True,
     )
 
+    def generate_dummy_inputs_for_validation(self, reference_model_inputs: Dict[str, Any]) -> Dict[str, Any]:
+        if self._behavior is ConfigBehavior.DECODER:
+            reference_model_inputs["input_ids"] = reference_model_inputs.pop("decoder_input_ids")
+
+            # T5 requires encoder_hidden_states as an input for both the without/with past models,
+            # which is different than other architectures that require it only for the without past case
+            reference_model_inputs["encoder_hidden_states"] = reference_model_inputs.pop("encoder_outputs")[0]
+
+        return super().generate_dummy_inputs_for_validation(reference_model_inputs)
+
 
 class MT5OnnxConfig(T5OnnxConfig):
     ATOL_FOR_VALIDATION = 1e-4
 
 
 class LongT5OnnxConfig(T5OnnxConfig):
     DEFAULT_ONNX_OPSET = 14
@@ -335,54 +350,54 @@
         )
         self.force_eos_token_id_presence = force_eos_token_id_presence
         self.eos_token_id = normalized_config.eos_token_id
 
     def generate(self, input_name: str, framework: str = "pt"):
         int_tensor = super().generate(input_name, framework=framework)
         # This inserts EOS_TOKEN_ID at random locations along the sequence length dimension.
-        if self.force_eos_token_id_presence and "input_ids" in input_name and self.task == "sequence-classification":
+        if self.force_eos_token_id_presence and "input_ids" in input_name and self.task == "text-classification":
             for idx in range(self.batch_size):
                 if self.eos_token_id in int_tensor[idx]:
                     continue
                 random_idx = random.randint(1, self.sequence_length - 1)
                 int_tensor[idx][random_idx] = self.eos_token_id
 
         return int_tensor
 
 
 class BartOnnxConfig(TextSeq2SeqOnnxConfig):
     NORMALIZED_CONFIG_CLASS = NormalizedSeq2SeqConfig.with_args(
         encoder_num_layers="encoder_layers",
         decoder_num_layers="decoder_layers",
-        num_layers="decoder_layers",  # Used for the causal-lm task past key values input generation.
+        num_layers="decoder_layers",  # Used for the text-generation task past key values input generation.
         encoder_num_attention_heads="encoder_attention_heads",
         decoder_num_attention_heads="decoder_attention_heads",
         eos_token_id="eos_token_id",
     )
     DUMMY_INPUT_GENERATOR_CLASSES = (
         BartDummyTextInputGenerator,
         {
-            "default": DummySeq2SeqDecoderTextInputGenerator,
-            "causal-lm": DummyDecoderTextInputGenerator,
+            "feature-extraction": DummySeq2SeqDecoderTextInputGenerator,
+            "text-generation": DummyDecoderTextInputGenerator,
         },
         {
-            "default": DummySeq2SeqPastKeyValuesGenerator,
-            "causal-lm": DummyPastKeyValuesGenerator,
+            "feature-extraction": DummySeq2SeqPastKeyValuesGenerator,
+            "text-generation": DummyPastKeyValuesGenerator,
         },
     )
 
     def _create_dummy_input_generator_classes(self, **kwargs) -> List["DummyInputGenerator"]:
         dummy_text_input_generator = self.DUMMY_INPUT_GENERATOR_CLASSES[0](
             self.task, self._normalized_config, **kwargs
         )
-        task = "default" if self.task != "causal-lm" else "causal-lm"
+        task = "feature-extraction" if self.task != "text-generation" else "text-generation"
         dummy_decoder_text_input_generator = self.DUMMY_INPUT_GENERATOR_CLASSES[1][task](
             self.task, self._normalized_config, **kwargs
         )
-        if self.task != "causal-lm":
+        if self.task != "text-generation":
             kwargs["encoder_sequence_length"] = dummy_text_input_generator.sequence_length
 
         dummy_seq2seq_past_key_values_generator = self.DUMMY_INPUT_GENERATOR_CLASSES[2][task](
             self.task, self._normalized_config, **kwargs
         )
         dummy_inputs_generators = [
             dummy_text_input_generator,
@@ -426,51 +441,49 @@
             "input_ids": {0: "batch_size", 1: "sequence_length"},
             "attention_mask": {0: "batch_size", 1: "sequence_length"},
         }
 
     @property
     def inputs(self) -> Dict[str, Dict[int, str]]:
         inputs_properties = {
-            "default": self.inputs_for_default_and_seq2seq_lm,
-            "seq2seq-lm": self.inputs_for_default_and_seq2seq_lm,
-            "causal-lm": self.inputs_for_causal_lm,
+            "feature-extraction": self.inputs_for_default_and_seq2seq_lm,
+            "text2text-generation": self.inputs_for_default_and_seq2seq_lm,
+            "text-generation": self.inputs_for_causal_lm,
             "other": self.inputs_for_other_tasks,
         }
         return inputs_properties.get(self.task, inputs_properties["other"])
 
     @property
     def outputs(self) -> Dict[str, Dict[int, str]]:
-        if self.task in ["default", "seq2seq-lm"]:
+        if self.task in ["feature-extraction", "text2text-generation"]:
             common_outputs = super().outputs
         else:
             common_outputs = super(OnnxConfigWithPast, self).outputs
-            if self.task != "causal-lm":
-                common_outputs["encoder_last_hidden_state"] = {0: "batch_size", 1: "sequence_length"}
             if self.use_present_in_outputs:
                 for i in range(self._normalized_config.encoder_num_layers):
                     common_outputs[f"present.{i}.key"] = {0: "batch_size", 2: "past_sequence_length + sequence_length"}
                     common_outputs[f"present.{i}.value"] = {
                         0: "batch_size",
                         2: "past_sequence_length + sequence_length",
                     }
         return common_outputs
 
     def generate_dummy_inputs(self, framework: str = "pt", **kwargs):
-        # This will handle the attention mask padding when Bart is used for causal-lm.
-        if self.task == "causal-lm":
+        # This will handle the attention mask padding when Bart is used for text-generation.
+        if self.task == "text-generation":
             self.PAD_ATTENTION_MASK_TO_PAST = True
 
         dummy_inputs = super().generate_dummy_inputs(framework=framework, **kwargs)
 
         # Setting it back to the default version.
         self.PAD_ATTENTION_MASK_TO_PAST = False
         return dummy_inputs
 
     def flatten_past_key_values(self, flattened_output, name, idx, t):
-        if self.task in ["default", "seq2seq-lm"]:
+        if self.task in ["feature-extraction", "text2text-generation"]:
             flattened_output = super().flatten_past_key_values(flattened_output, name, idx, t)
         else:
             flattened_output = super(OnnxSeq2SeqConfigWithPast, self).flatten_past_key_values(
                 flattened_output, name, idx, t
             )
 
 
@@ -782,15 +795,15 @@
         MAX_2D_POSITION_EMBEDDINGS="max_2d_position_embeddings",
         image_size="input_size",
     )
     DEFAULT_ONNX_OPSET = 12
 
     @property
     def inputs(self) -> Dict[str, Dict[int, str]]:
-        if self.task in ["sequence-classification", "question-answering"]:
+        if self.task in ["text-classification", "question-answering"]:
             pixel_values_dynamic_axes = {0: "batch_size", 1: "num_channels", 2: "height", 3: "width"}
         else:
             pixel_values_dynamic_axes = {0: "batch_size", 1: "num_channels"}
         return {
             "input_ids": {0: "batch_size", 1: "sequence_length"},
             "attention_mask": {0: "batch_size", 1: "sequence_length"},
             "bbox": {0: "batch_size", 1: "sequence_length"},
@@ -821,22 +834,22 @@
 
 class PerceiverOnnxConfig(TextAndVisionOnnxConfig):
     NORMALIZED_CONFIG_CLASS = NormalizedTextConfig
     DUMMY_INPUT_GENERATOR_CLASSES = (
         PerceiverDummyInputGenerator,
     ) + TextAndVisionOnnxConfig.DUMMY_INPUT_GENERATOR_CLASSES
 
-    def __init__(self, config: "PretrainedConfig", task: str = "default"):
+    def __init__(self, config: "PretrainedConfig", task: str = "feature-extraction"):
         super().__init__(config, task=task)
         self.is_generating_dummy_inputs = False
 
     @property
     def inputs_name(self):
         if self.is_generating_dummy_inputs:
-            if self.task in ["masked-lm", "sequence-classification"]:
+            if self.task in ["fill-mask", "text-classification"]:
                 return "input_ids"
             else:
                 return "pixel_values"
         else:
             return "inputs"
 
     @property
@@ -940,15 +953,15 @@
 class WhisperOnnxConfig(AudioToTextOnnxConfig):
     NORMALIZED_CONFIG_CLASS = NormalizedSeq2SeqConfig
     ATOL_FOR_VALIDATION = 1e-3
 
     @property
     def inputs(self) -> Dict[str, Dict[int, str]]:
         common_inputs = super().inputs
-        if self._behavior is ConfigBehavior.DECODER:
+        if self._behavior is ConfigBehavior.DECODER and self.use_past_in_inputs is False:
             common_inputs["encoder_outputs"][1] = f"{common_inputs['encoder_outputs'][1]} / 2"
         return common_inputs
 
     @property
     def outputs(self) -> Dict[str, Dict[int, str]]:
         common_outputs = super().outputs
         if self._behavior is ConfigBehavior.ENCODER:
@@ -1034,15 +1047,15 @@
     ATOL_FOR_VALIDATION = 1e-3
 
     DUMMY_INPUT_GENERATOR_CLASSES = (DummyVisionInputGenerator,)
 
     def __init__(
         self,
         config: "PretrainedConfig",
-        task: str = "default",
+        task: str = "feature-extraction",
         use_past: bool = False,
         use_past_in_inputs: Optional[bool] = None,
         use_present_in_outputs: Optional[bool] = None,
         behavior: ConfigBehavior = ConfigBehavior.MONOLITH,
     ):
         super().__init__(config, task, use_past, use_past_in_inputs, use_present_in_outputs, behavior)
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/model_patcher.py` & `optimum-1.8.0/optimum/exporters/onnx/model_patcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,15 +126,19 @@
             # Filter out cross attention past key values
             filterd_outputs = {}
             for name, value in outputs.items():
                 if config.torch_to_onnx_output_map.get(name, name) in config.outputs or (
                     allow_past_in_outputs and name.startswith("past_key_values")
                 ):
                     if name != "past_key_values":
-                        filterd_outputs[name] = value
+                        if self.real_config._behavior == "decoder" and name == "encoder_last_hidden_state":
+                            # Who cares about the encoder outputs in the decoder?
+                            continue
+                        else:
+                            filterd_outputs[name] = value
                     else:
                         if self.real_config._behavior == "monolith" or (
                             self.real_config._behavior == "decoder" and self.real_config.use_past is False
                         ):
                             filterd_outputs[name] = value
                         elif self.real_config._behavior == "decoder" and self.real_config.use_past is True:
                             filterd_outputs[name] = tuple([v[:2] for v in value])
```

### Comparing `optimum-1.7.3/optimum/exporters/onnx/utils.py` & `optimum-1.8.0/optimum/exporters/onnx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         `Dict[str, Tuple[Union[`PreTrainedModel`, `TFPreTrainedModel`], `OnnxConfig`]: A Dict containing the model and
         onnx configs for the different components of the model.
     """
     models_for_export = {}
 
     # Text encoder
     text_encoder_config_constructor = TasksManager.get_exporter_config_constructor(
-        model=pipeline.text_encoder, exporter="onnx", task="default"
+        model=pipeline.text_encoder, exporter="onnx", task="feature-extraction"
     )
     text_encoder_onnx_config = text_encoder_config_constructor(pipeline.text_encoder.config)
     models_for_export["text_encoder"] = (pipeline.text_encoder, text_encoder_onnx_config)
 
     # U-NET
     onnx_config_constructor = TasksManager.get_exporter_config_constructor(
         model=pipeline.unet, exporter="onnx", task="semantic-segmentation", model_type="unet"
```

### Comparing `optimum-1.7.3/optimum/exporters/tflite/__init__.py` & `optimum-1.8.0/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/tflite/__main__.py` & `optimum-1.8.0/optimum/exporters/tflite/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/tflite/base.py` & `optimum-1.8.0/optimum/exporters/tflite/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,34 +63,34 @@
 
         approach (`Optional[Union[str, QuantizationApproach]]`, defaults to `None`):
             The quantization approach to perform. No quantization is applied if left unspecified.
         fallback_to_float (`bool`, defaults to `False`):
             Allows to fallback to float kernels in quantization.
         inputs_dtype (`Optional[str]`, defaults to `None`):
             The data type of the inputs. If specified it must be either "int8" or "uint8". It allows to always take
-            integers as inputs, it is useful for interger-only hardware.
+            integers as inputs, it is useful for integer-only hardware.
         outputs_dtype (`Optional[str]`, defaults to `None`):
             The data type of the outputs. If specified it must be either "int8" or "uint8". It allows to always output
-            integers, it is useful for interger-only hardware.
+            integers, it is useful for integer-only hardware.
         calibration_dataset_name_or_path (`Optional[Union[str, Path]]`, defaults to `None`):
             The dataset to use for calibrating the quantization parameters for static quantization. If left unspecified,
             a default dataset for the considered task will be used.
         calibration_dataset_config_name (`Optional[str]`, defaults to `None`):
             The configuration name of the dataset if needed.
         num_calibration_samples (`int`, defaults to `200`):
-            The number of example from the calibration dataset to use to compute the quantization parameters.
+            The number of examples from the calibration dataset to use to compute the quantization parameters.
         calibration_split (`Optional[str]`, defaults to `None`):
             The split of the dataset to use. If none is specified and the dataset contains multiple splits, the
             smallest split will be used.
         primary_key (`Optional[str]`, defaults `None`):
             The name of the column in the dataset containing the main data to preprocess. Only for
-            sequence-classification and token-classification.
+            text-classification and token-classification.
         secondary_key (`Optional[str]`, defaults `None`):
             The name of the second column in the dataset containing the main data to preprocess, not always needed.
-            Only for sequence-classification and token-classification.
+            Only for text-classification and token-classification.
         question_key (`Optional[str]`, defaults `None`):
             The name of the column containing the question in the dataset. Only for question-answering.
         context_key (`Optional[str]`, defaults `None`):
             The name of the column containing the context in the dataset. Only for question-answering.
         image_key (`Optional[str]`, defaults `None`):
             The name of the column containing the image in the dataset. Only for image-classification.
     """
@@ -137,15 +137,15 @@
         For example: `MANDATORY_AXES = ("batch_size", "sequence_length", ("multiple-choice", "num_choices"))` means that
         to export the model, the batch size and sequence length values always need to be specified, and that a value
         for the number of possible choices is needed when the task is multiple-choice.
 
     Args:
         config (`transformers.PretrainedConfig`):
             The model configuration.
-        task (`str`, defaults to `"default"`):
+        task (`str`, defaults to `"feature-extraction"`):
             The task the model should be exported for.
 
         The rest of the arguments are used to specify the shape of the inputs the model can take.
         They are required or not depending on the model the `TFLiteConfig` is designed for.
     """
 
     NORMALIZED_CONFIG_CLASS: Type = None
@@ -153,31 +153,30 @@
     ATOL_FOR_VALIDATION: Union[float, Dict[str, float]] = 1e-5
     MANDATORY_AXES = ()
     SUPPORTED_QUANTIZATION_APPROACHES: Union[
         Dict[str, Tuple[QuantizationApproach, ...]], Tuple[QuantizationApproach, ...]
     ] = tuple(approach for approach in QuantizationApproach)
 
     _TASK_TO_COMMON_OUTPUTS = {
-        "causal-lm": ["logits"],
-        "default": ["last_hidden_state"],
+        "text-generation": ["logits"],
+        "feature-extraction": ["last_hidden_state"],
         "image-classification": ["logits"],
         "image-segmentation": ["logits", "pred_boxes", "pred_masks"],
         "masked-im": ["logits"],
-        "masked-lm": ["logits"],
+        "fill-mask": ["logits"],
         "multiple-choice": ["logits"],
         "object-detection": ["logits", "pred_boxes"],
         "question-answering": ["start_logits", "end_logits"],
         "semantic-segmentation": ["logits"],
-        "seq2seq-lm": ["logits", "encoder_last_hidden_state"],
-        "sequence-classification": ["logits"],
+        "text2text-generation": ["logits", "encoder_last_hidden_state"],
+        "text-classification": ["logits"],
         "token-classification": ["logits"],
-        "speech2seq-lm": ["logits"],
+        "automatic-speech-recognition": ["logits"],
         "audio-classification": ["logits"],
         "audio-frame-classification": ["logits"],
-        "audio-ctc": ["logits"],
         "audio-xvector": ["logits"],
     }
 
     def __init__(
         self,
         config: "PretrainedConfig",
         task: str,
```

### Comparing `optimum-1.7.3/optimum/exporters/tflite/config.py` & `optimum-1.8.0/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/exporters/tflite/convert.py` & `optimum-1.8.0/optimum/exporters/tflite/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                 "the calibration dataset."
             )
 
         converter.optimizations = [tf.lite.Optimize.DEFAULT]
 
         # Handling the calibration dataset:
         # - Either loading the default dataset if no calibration dataset was provided or the required dataset,
-        # - Splitting the dataset with the provided a dataset split or with the first split if none is provided.
+        # - Splitting the dataset with the provided dataset split or with the first split if none is provided.
         # - Shuffling the split.
         # - Selecting num_calibration_samples in the dataset split.
         # - Batching the dataset.
         # - Converting it to the TensorFlow format.
 
         if task is None:
             from ...exporters import TasksManager
```

### Comparing `optimum-1.7.3/optimum/exporters/tflite/model_configs.py` & `optimum-1.8.0/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/__init__.py` & `optimum-1.8.0/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/optimization/__init__.py` & `optimum-1.8.0/optimum/fx/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/optimization/transformations.py` & `optimum-1.8.0/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/quantization/__init__.py` & `optimum-1.8.0/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/quantization/functions.py` & `optimum-1.8.0/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/fx/utils.py` & `optimum-1.8.0/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/modeling_base.py` & `optimum-1.8.0/optimum/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnx/__init__.py` & `optimum-1.8.0/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnx/configuration.py` & `optimum-1.8.0/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnx/graph_transformations.py` & `optimum-1.8.0/optimum/onnx/graph_transformations.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
 def merge_decoders(
     decoder: Union[ModelProto, Path, str],
     decoder_with_past: Union[ModelProto, Path, str],
     graph_name: str = "merged",
     producer_name: str = "optimum-onnx",
     save_path: Optional[Union[str, Path]] = None,
+    strict: bool = True,
 ) -> ModelProto:
     """
     Fuses decoder ONNX model and decoder with past ONNX model into one ONNX model with if logic.
 
     Args:
         decoder (`Union[ModelProto, Path, str]`):
             Decoder ONNX model.
@@ -109,14 +110,18 @@
             Decoder with past ONNX model.
         graph_name (`str`, defaults to `"merged"`):
             Name of the parent graph (graph of the control flow node).
         producer_name (`str`, defaults to `"optimum-onnx"`):
             Graph producer name.
         save_path (`Optional[Union[str, Path]]`, defaults to `None`):
             The path to save merged ONNX model. The model will be saved if the path is given.
+        strict (`bool`, defaults to `True`):
+            When set, the decoder and decoder_with_past are expected to have strictly the same number of outputs. When False,
+            the decoder is allowed to have more outputs that decoder_with_past, in which case constant outputs are added to match
+            the number of outputs.
 
     Returns:
         `~onnx.ModelProto`: The fused decoder ONNX model.
     """
     if isinstance(decoder, (str, Path)):
         decoder = Path(decoder).as_posix()
         decoder = onnx.load(decoder)
@@ -128,15 +133,15 @@
     decoder_opset = _get_onnx_opset(decoder)
     decoder_with_past_opset = _get_onnx_opset(decoder_with_past)
     if decoder_opset != decoder_with_past_opset:
         raise ValueError(
             f"Decoder's opset is {decoder_opset}, but decoder with past's opset is {decoder_with_past_opset}. Make sure having the same opset before merging."
         )
 
-    _unify_onnx_outputs(decoder, decoder_with_past)
+    _unify_onnx_outputs(decoder, decoder_with_past, strict=strict)
     all_inputs = _get_all_inputs([decoder, decoder_with_past])
 
     # Replace the axis name `sequence_length` of the attention_mask input by `attention_mask_sequence_length`.
     # This is because the merged model `input_ids` and `attention_mask` inputs may not always have the same length on the 2nd axis.
     # In the first pass, `input_ids` and `attention_mask` are indeed of the same length, but in later pass `input_ids` is of length 1
     # while `attention_mask` is of length `past_sequence_length + 1`
     for _, inp in enumerate(all_inputs):
```

### Comparing `optimum-1.7.3/optimum/onnx/modeling_seq2seq.py` & `optimum-1.8.0/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnx/transformations_utils.py` & `optimum-1.8.0/optimum/onnx/transformations_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,48 +8,58 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import hashlib
 from collections import defaultdict
 from typing import DefaultDict, Dict, List, Set, Tuple
 
 import numpy as np
 
 import onnx
 from onnx import ModelProto, ValueInfoProto, numpy_helper
 
+from ..utils import logging
+
+
+logger = logging.get_logger()
+logger.setLevel(logging.INFO)
+
 
 def _find_duplicate_initializers(
     models: List[ModelProto],
-) -> DefaultDict[Tuple[int, bytes, Tuple], Set[Tuple[str, int]]]:
+) -> DefaultDict[Tuple[int, str, Tuple], Set[Tuple[str, int]]]:
     """
     Creates a map (unique data) --> set of (initializer name, model id)
 
     Initializers with a dimension 0, or dimension 1 with data type int32 or int64, are not included in the generated map.
     """
     duplicates = defaultdict(set)
     for i in range(len(models)):
         for initializer in models[i].graph.initializer:
             tensor_dims = tuple(getattr(initializer, "dims"))
             if len(tensor_dims) > 1 or (len(tensor_dims) == 1 and initializer.data_type not in [6, 7]):
-                for data_attr in ["raw_data", "int32_data", "int64_data", "uint64_data", "float_data", "double_data"]:
-                    tensor_data = getattr(initializer, data_attr)
-                    if tensor_data:
-                        tensor_data = tuple(tensor_data)
-                        break
-                duplicates[(initializer.data_type, tensor_data, tensor_dims)].add((initializer.name, i))
+                # Extract tensor data as numpy array
+                tensor_data = numpy_helper.to_array(initializer)
+
+                # Hash tensor data to avoid storing large amounts of data in memory
+                hashed = hashlib.sha512()
+                hashed.update(tensor_data)
+                tensor_digest = hashed.hexdigest()
+
+                duplicates[(initializer.data_type, tensor_digest, tensor_dims)].add((initializer.name, i))
 
     return duplicates
 
 
 def _create_name_sharing_dict(
-    duplicate_weights: DefaultDict[Tuple[int, bytes], Set[Tuple[str, int]]], suffix: str = ""
+    duplicate_weights: DefaultDict[Tuple[int, str, Tuple], Set[Tuple[str, int]]], suffix: str = ""
 ) -> Dict[Tuple[str, int], str]:
     """
     Creates a map mapping old initializer names to new initializer names. As different ONNX models
     may use the same initializer name but need to be mapped to a different new name, the map is actually from
     (old name, model id) to new name.
 
     Example of initializers with the same name that will need to be mapped to a different one:
@@ -124,52 +134,108 @@
             output_shape.append(getattr(dim, "dim_value"))
         else:
             raise ValueError("Cannot find `dim_param` nor `dim_value` in the output dimension info.")
 
     return output_shape
 
 
-def _check_num_outputs(model1: ModelProto, model2: ModelProto):
-    """
-    Checks that `model1` and `model2` have the same number of outputs.
-    """
-    if not len(model1.graph.output) == len(model2.graph.output):
-        raise ValueError(
-            f"Two model protos need to have the same outputs. But one has {len(model1.graph.output)} "
-            f"outputs while the other has {len(model2.graph.output)} outputs."
-        )
-
-
-def _unify_onnx_outputs(model1: ModelProto, model2: ModelProto):
+def _unify_onnx_outputs(model1: ModelProto, model2: ModelProto, strict: bool):
     """
     Unifies the outputs of two ONNX model protos. The outputs of model1 will be replaced by outputs of model2.
     According to the rules of "If" op, two subgraphs must have the same number of outputs.
     """
-    _check_num_outputs(model1, model2)
+
+    model1_outputs = {output.name for output in model1.graph.output}
+    model2_outputs = {output.name for output in model2.graph.output}
+
+    if model1_outputs != model2_outputs:
+        if strict is True:
+            raise ValueError(
+                f"The two model protos outputs are expected to have the same number of outputs and output names when strict=True. Found"
+                f" the outputs {model1_outputs - model2_outputs} only in model1, and {model2_outputs - model1_outputs} only in model2."
+            )
+        else:
+            logger.info(
+                f"The two models proto have different outputs ({len(model1_outputs)} and {len(model2_outputs)} outputs)."
+                " Constant outputs will be added to unify the two models outputs."
+            )
+
+    if model2_outputs.issubset(model1_outputs) is False:
+        raise ValueError("The second ModelProto should not have more outputs than the first.")
 
     for idx in range(len(model1.graph.output)):
         model_output_1 = model1.graph.output[idx]
-        model_output_2 = model2.graph.output[idx]
-        if not model_output_1 == model_output_2:
-            if not (
+        model_output_2 = model2.graph.output[idx] if idx < len(model2.graph.output) else None
+
+        if model_output_2 is None or model_output_1 != model_output_2:
+            if model_output_2 is None or not (
                 model_output_1.name == model_output_2.name
                 and model_output_1.type.tensor_type.elem_type == model_output_2.type.tensor_type.elem_type
             ):
-                raise ValueError(
-                    f"Can not match {model_output_1.name} with {model_output_2.name}. Make sure your"
-                    f" model protos have same outputs, have same data types and are in the same order."
+                if strict is False and model_output_1.name not in model2_outputs:
+                    data_type = model_output_1.type.tensor_type.elem_type
+                    dims_output_1 = _infer_output_shape(model_output_1)
+                    if not isinstance(dims_output_1[0], str):
+                        raise ValueError(
+                            f"Expected a dynamic shape for the axis zero of {model_output_1.name}, found a static shape: {dims_output_1[0]}"
+                        )
+
+                    # fill the constant shape with the original shape, except for the axis zero that is 0 for an empty constant,
+                    # and the dynamic axis set to 1
+                    dims_dummy_output = [0]
+                    for dim in dims_output_1[1:]:
+                        if isinstance(dim, str):
+                            dims_dummy_output.append(1)
+                        else:
+                            dims_dummy_output.append(dim)
+
+                    logger.info(
+                        f"Addind a constant output for {model_output_1.name} of shape {dims_dummy_output} in model2."
+                    )
+                    value = onnx.helper.make_tensor(
+                        name="const_tensor", data_type=data_type, dims=dims_dummy_output, vals=[]
+                    )
+                    constant_node = onnx.helper.make_node(
+                        "Constant",
+                        name=f"Constant_{len(model2.graph.node) + 1}",
+                        inputs=[],
+                        outputs=[f"{model_output_1.name}"],
+                        value=value,
+                    )
+                    model2.graph.node.append(constant_node)
+
+                    constant_empty_output = onnx.helper.make_tensor_value_info(
+                        model_output_1.name,
+                        model_output_1.type.tensor_type.elem_type,
+                        _infer_output_shape(model_output_1),
+                    )
+                    model2.graph.output.insert(idx, constant_empty_output)
+                else:
+                    if model_output_2 is not None:
+                        raise ValueError(
+                            f"Cannot match {model_output_1.name} with {model_output_2.name}. Make sure your"
+                            f" model protos have same outputs, have same data types and are in the same order."
+                        )
+                    else:
+                        raise ValueError(
+                            f"Too few outputs of model2 were found to match with {model_output_1.name}."
+                            f" Please try to pass strict=False, or fill a bug report at https://github.com/huggingface/optimum."
+                        )
+            else:
+                model2.graph.output.remove(model_output_2)
+
+                # We use model1 (normally the decoder) for the output shape
+                # TODO: relax this, and keep the most permissive output shape between model1 and model2
+                # while checking they are compatible
+                new_output = onnx.helper.make_tensor_value_info(
+                    model_output_1.name,
+                    model_output_1.type.tensor_type.elem_type,
+                    _infer_output_shape(model_output_1),
                 )
-            model2.graph.output.remove(model_output_2)
-
-            new_output = onnx.helper.make_tensor_value_info(
-                model_output_1.name,
-                model_output_1.type.tensor_type.elem_type,
-                _infer_output_shape(model_output_1),
-            )
-            model2.graph.output.insert(idx, new_output)
+                model2.graph.output.insert(idx, new_output)
 
     if not all(
         model_output_1 == model_output_2
         for model_output_1, model_output_2 in zip(model1.graph.output, model2.graph.output)
     ):
         raise RuntimeError("Failed to unify outputs of given ONNX model protos.")
```

### Comparing `optimum-1.7.3/optimum/onnx/utils.py` & `optimum-1.8.0/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/__init__.py` & `optimum-1.8.0/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/base.py` & `optimum-1.8.0/optimum/onnxruntime/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,28 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """Defines the base classes that are used to perform inference with ONNX Runtime of Transformers models."""
 
 from abc import abstractmethod
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Dict, List, Optional, Set, Tuple, Union
 
+import numpy as np
 import torch
 from transformers.modeling_outputs import BaseModelOutput, CausalLMOutputWithCrossAttentions, Seq2SeqLMOutput
 
 from onnxruntime import InferenceSession
 
 from ..utils import NormalizedConfigManager
-from .utils import get_ordered_input_names
+from ..utils.logging import warn_once
+from .utils import get_ordered_input_names, logging
+
+
+logger = logging.get_logger(__name__)
 
 
 if TYPE_CHECKING:
     from .modeling_ort import ORTModel
 
 
 class ORTModelPart:
@@ -174,46 +179,59 @@
             if (
                 isinstance(self.expected_value_symbolic_shape[-1], str)
                 and "sequence_length" in self.expected_value_symbolic_shape[-1]
             ):
                 self.value_sequence_length_idx = -1
 
     def prepare_inputs_for_merged(
-        self, input_ids: Optional[torch.LongTensor] = None, past_key_values: Optional[List[torch.FloatTensor]] = None
+        self,
+        input_ids: Union[None, torch.LongTensor, np.ndarray] = None,
+        past_key_values: Union[None, Tuple[torch.FloatTensor], Tuple[np.ndarray]] = None,
+        use_torch: bool = False,
     ):
-        if past_key_values is None and self.parent_model.use_merged:
-            # Uses "no past" branch of a merged decoder
-            use_cache_branch = torch.full((1,), False).to(self.device)
-        elif past_key_values is not None and self.parent_model.use_merged:
-            # Uses "with past" branch of a merged decoder
-            use_cache_branch = torch.full((1,), True).to(self.device)
+        constructor = torch if use_torch is True else np
+        if self.parent_model.use_merged:
+            # Uses without/with branch of a merged decoder depending on whether real past key values are passed
+            use_cache_branch = constructor.full((1,), past_key_values is not None)
         else:
             # Uses separate decoders
             use_cache_branch = None
 
+        if use_torch and use_cache_branch is not None:
+            use_cache_branch = use_cache_branch.to(self.device)
+
         # Generate dummy past for the first forward if uses a merged decoder
         if self.parent_model.use_merged and past_key_values is None:
-            batch_size = input_ids.size(0)
+            batch_size = input_ids.shape[0]
             num_attention_heads = self.normalized_config.num_attention_heads
             embed_size_per_head = self.normalized_config.hidden_size // num_attention_heads
 
             # TODO: find a way to better handle this controlflow, this is EXTREMELY ugly
             # "1" is the dummy sequence length
             if self.parent_model.config.model_type == "bloom":
                 shape_value = (batch_size * num_attention_heads, 1, embed_size_per_head)
                 shape_key = (batch_size * num_attention_heads, embed_size_per_head, 1)
-                key = torch.zeros(shape_key, dtype=torch.float32).to(self.device)
-                value = torch.zeros(shape_value, dtype=torch.float32).to(self.device)
-                past_key_values = [
+                key = constructor.zeros(shape_key, dtype=constructor.float32)
+                value = constructor.zeros(shape_value, dtype=constructor.float32)
+
+                if use_torch is True:
+                    key = key.to(self.device)
+                    value = value.to(self.device)
+
+                past_key_values = tuple(
                     key_or_value for _ in range(len(self.key_value_input_names) // 2) for key_or_value in [key, value]
-                ]
+                )
             else:
                 shape = (batch_size, num_attention_heads, 1, embed_size_per_head)
-                key_or_value = torch.zeros(shape, dtype=torch.float32).to(self.device)
-                past_key_values = [key_or_value for _ in range(len(self.key_value_input_names))]
+                key_or_value = constructor.zeros(shape, dtype=constructor.float32)
+
+                if use_torch is True:
+                    key_or_value = key_or_value.to(self.device)
+
+                past_key_values = tuple(key_or_value for _ in range(len(self.key_value_input_names)))
 
         return use_cache_branch, past_key_values
 
     def compute_past_key_values_output_shapes(
         self,
         input_ids: torch.Tensor,
         use_cache_branch: Optional[bool],
@@ -273,36 +291,40 @@
     ) -> CausalLMOutputWithCrossAttentions:
         # adding use_cache_branch in the signature here is just a hack for IO Binding
         use_torch = isinstance(input_ids, torch.Tensor)
         self.parent_model.raise_on_numpy_input_io_binding(use_torch)
 
         # Flatten the past_key_values
         if past_key_values is not None:
-            past_key_values = [past_key_value for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer]
+            past_key_values = tuple(
+                past_key_value for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
+            )
 
         # no-ops if merged decoder is not used
-        use_cache_branch, past_key_values = self.prepare_inputs_for_merged(input_ids, past_key_values)
+        use_cache_branch_tensor, past_key_values = self.prepare_inputs_for_merged(
+            input_ids, past_key_values, use_torch=use_torch
+        )
 
         if self.device.type == "cuda" and self.parent_model.use_io_binding:
             known_output_shapes = self.compute_past_key_values_output_shapes(
                 input_ids,
-                use_cache_branch=use_cache_branch.item() if use_cache_branch is not None else None,
+                use_cache_branch=use_cache_branch_tensor.item() if use_cache_branch_tensor is not None else None,
                 past_key_values=past_key_values,
             )
 
             model_inputs = [input_ids]
 
             if "attention_mask" in self.input_names:
                 model_inputs.append(attention_mask)
 
             if past_key_values is not None:
                 model_inputs += past_key_values
 
-            if use_cache_branch is not None:
-                model_inputs.append(use_cache_branch)
+            if use_cache_branch_tensor is not None:
+                model_inputs.append(use_cache_branch_tensor)
 
             if "labels" in self.input_names:
                 model_inputs.append(labels)
                 known_output_shapes.update({"loss": []})
 
             io_binding, output_shapes, output_buffers = self.parent_model._prepare_io_binding(
                 self.session,
@@ -333,15 +355,15 @@
             if use_torch:
                 onnx_inputs = {
                     "input_ids": input_ids.cpu().detach().numpy(),
                     "attention_mask": attention_mask.cpu().detach().numpy(),
                 }
 
                 if self.parent_model.use_merged is True:
-                    onnx_inputs["use_cache_branch"] = use_cache_branch.cpu().detach().numpy()
+                    onnx_inputs["use_cache_branch"] = use_cache_branch_tensor.cpu().detach().numpy()
 
                 if past_key_values is not None:
                     # Add the past_key_values to the decoder inputs
                     for input_name, past_key_value in zip(self.key_value_input_names, past_key_values):
                         onnx_inputs[input_name] = past_key_value.cpu().detach().numpy()
 
                 if "labels" in self.input_names:
@@ -349,15 +371,15 @@
             else:
                 onnx_inputs = {
                     "input_ids": input_ids,
                     "attention_mask": attention_mask,
                 }
 
                 if self.parent_model.use_merged is True:
-                    onnx_inputs["use_cache_branch"] = use_cache_branch
+                    onnx_inputs["use_cache_branch"] = use_cache_branch_tensor
 
                 if past_key_values is not None:
                     # Add the past_key_values to the decoder inputs
                     for input_name, past_key_value in zip(self.key_value_input_names, past_key_values):
                         onnx_inputs[input_name] = past_key_value
 
                 if "labels" in self.input_names:
@@ -393,80 +415,126 @@
     def __init__(
         self,
         session: InferenceSession,
         parent_model: "ORTModel",
     ):
         super().__init__(session, parent_model)
 
-        if self.use_past:
+        if self.parent_model.use_merged is False and self.use_past is True:
             self.num_pkv = 2
         else:
+            # When using a merged model, we always have the same number of output whether we use past key values or not,
+            # and in the case past key values are used, empty tensors are given as cross-attention past key values as they
+            # are constants
             self.num_pkv = 4
 
+        self.past_key_values_cross_attention_output_names = set()
+        for output_name in self.output_names:
+            if output_name.startswith("present") and "encoder" in output_name:
+                self.past_key_values_cross_attention_output_names.add(output_name)
+
+        self.use_legacy_outputs = (
+            self.parent_model.use_merged is False and len(self.past_key_values_cross_attention_output_names) > 0
+        )
+
     def compute_past_key_values_output_shapes(
-        self, input_ids, encoder_hidden_states, past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None
+        self,
+        input_ids: torch.Tensor,
+        encoder_hidden_states: torch.Tensor,
+        use_cache_branch: Optional[bool],
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
     ) -> Dict[str, int]:
         batch_size = input_ids.size(0)
         num_attention_heads = self.normalized_config.num_attention_heads
         embed_size_per_head = self.normalized_config.hidden_size // num_attention_heads
 
         sequence_length = input_ids.size(1)
         encoder_sequence_length = encoder_hidden_states.size(1)
-        if past_key_values is not None:
+        if past_key_values is not None and use_cache_branch is not False:
+            # Here, use_cache_branch may be None in the case of separate decoder without/with past, or True if the with past branch
+            # of a merged decoder is used
             sequence_length += past_key_values[0].size(2)
 
         self_attn_shape = (batch_size, num_attention_heads, sequence_length, embed_size_per_head)
-        cross_attn_shape = (batch_size, num_attention_heads, encoder_sequence_length, embed_size_per_head)
+
+        if past_key_values is not None and use_cache_branch is True:
+            cross_attn_shape = (0, num_attention_heads, 1, embed_size_per_head)
+        else:
+            cross_attn_shape = (batch_size, num_attention_heads, encoder_sequence_length, embed_size_per_head)
 
         past_key_values_shapes = {}
         for idx, name in enumerate(self.key_value_output_names):
             is_self_attn = idx % 4 < 2
             # decoder with past does not ouput cross attention key/values as they are constants
-            past_key_values_shapes[name] = self_attn_shape if (is_self_attn or self.use_past) else cross_attn_shape
+            past_key_values_shapes[name] = self_attn_shape if (is_self_attn or self.num_pkv == 2) else cross_attn_shape
         return past_key_values_shapes
 
+    def get_outputs_not_to_bind(self, use_merged_cache: bool) -> Set[str]:
+        result = {
+            output_name
+            for output_name in self.output_names
+            if (not output_name.startswith("present") and output_name not in {"loss", "logits"})
+        }
+        if use_merged_cache is True:
+            # When using a merged decoder and the use cache branch, we output 0-dim tensors that IO Binding do not support.
+            # Therefore, we do not bind them.
+            result = result.union(self.past_key_values_cross_attention_output_names)
+        return result
+
     def forward(
         self,
         input_ids: torch.LongTensor,
         encoder_hidden_states: torch.FloatTensor,
         encoder_attention_mask: Optional[torch.LongTensor] = None,
         past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
         labels: Optional[torch.LongTensor] = None,
+        use_cache_branch: None = None,
     ) -> Seq2SeqLMOutput:
+        # Adding use_cache_branch in the signature here is just a hack for IO Binding
+
         use_torch = isinstance(input_ids, torch.Tensor)
         self.parent_model.raise_on_numpy_input_io_binding(use_torch)
+
         # Flatten the past_key_values
         if past_key_values is not None:
             past_key_values = tuple(
                 past_key_value for pkv_per_layer in past_key_values for past_key_value in pkv_per_layer
             )
 
+        # no-ops if merged decoder is not used
+        use_merged_no_cache = past_key_values is None and self.parent_model.use_merged
+        use_merged_cache = past_key_values is not None and self.parent_model.use_merged
+        use_cache_branch_tensor, past_key_values = self.prepare_inputs_for_merged(
+            input_ids, past_key_values, use_torch=use_torch
+        )
+
         if self.parent_model.device.type == "cuda" and self.parent_model.use_io_binding:
             known_output_shapes = self.compute_past_key_values_output_shapes(
                 input_ids,
                 encoder_hidden_states,
+                use_cache_branch=use_cache_branch_tensor.item() if use_cache_branch_tensor is not None else None,
                 past_key_values=past_key_values,
             )
 
-            def filter_out_output(output_name):
-                return not output_name.startswith("present") and output_name not in {"loss", "logits"}
-
-            outputs_to_not_bind = {name for name in self.output_names if filter_out_output(name)}
+            outputs_to_not_bind = self.get_outputs_not_to_bind(use_merged_cache)
 
             model_inputs = [input_ids]
 
             if "encoder_attention_mask" in self.input_names:
                 model_inputs.append(encoder_attention_mask)
 
             if "encoder_hidden_states" in self.input_names:
                 model_inputs.append(encoder_hidden_states)
 
             if past_key_values is not None:
                 model_inputs += past_key_values
 
+            if use_cache_branch_tensor is not None:
+                model_inputs.append(use_cache_branch_tensor)
+
             if "labels" in self.input_names:
                 model_inputs.append(labels)
                 known_output_shapes.update({"loss": []})
 
             io_binding, output_shapes, output_buffers = self.parent_model._prepare_io_binding(
                 self.session,
                 *model_inputs,
@@ -484,21 +552,57 @@
             self.session.run_with_iobinding(io_binding)
             io_binding.synchronize_outputs()
 
             # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the
             # self-attention layer and 2 to the cross-attention layer)
             out_past_key_values = ()
             for name in self.key_value_output_names:
+                # TODO: this should be improved
+                if name in self.past_key_values_cross_attention_output_names and use_merged_cache:
+                    continue
                 out_past_key_values += (output_buffers[name].view(output_shapes[name]),)
 
             logits = output_buffers["logits"].view(output_shapes["logits"])
 
             loss = None
             if "loss" in self.output_names:
                 loss = output_buffers["loss"].view(output_shapes["loss"])
+
+            # IO Binding does not support 0-dim output with null pointer, so handle this case here
+            if self.use_past is False or use_merged_no_cache:
+                out_past_key_values = tuple(
+                    out_past_key_values[i : i + self.num_pkv] for i in range(0, len(out_past_key_values), self.num_pkv)
+                )
+            else:
+                if self.use_legacy_outputs is True:
+                    msg = (
+                        "For the decoder with past, using ONNX models outputting cross attention past key values"
+                        " is deprecated and the support will be removed in optimum 2.0. We recommend exporting again the model"
+                        " with optimum>=1.7.3."
+                    )
+                    warn_once(logger, msg=msg)
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + self.num_pkv]
+                        for i in range(0, len(out_past_key_values), self.num_pkv)
+                    )
+                # grab the cross attention key/values from the inputs
+                elif self.num_pkv == 2:
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + self.num_pkv]
+                        + past_key_values[2 * i + 2 : 2 * i + 2 + self.num_pkv]
+                        for i in range(0, len(out_past_key_values), self.num_pkv)
+                    )
+                elif self.num_pkv == 4:
+                    # despite num_pkv being 4, we did not bind the cross-attention output
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + 2] + past_key_values[2 * i + 2 : 2 * i + 4]
+                        for i in range(0, len(out_past_key_values), 2)
+                    )
+                else:
+                    raise ValueError("Unsupported num_pkv")
         else:
             if use_torch:
                 onnx_inputs = {
                     "input_ids": input_ids.cpu().detach().numpy(),
                 }
 
                 # Add the encoder_attention_mask inputs when needed
@@ -513,14 +617,17 @@
                     # Add the past_key_values to the decoder inputs
                     for input_name, past_key_value in zip(self.key_value_input_names, past_key_values):
                         onnx_inputs[input_name] = past_key_value.cpu().detach().numpy()
 
                 if "labels" in self.input_names:
                     # TODO: Any preprocessing like  `self._shift_right(labels)`?
                     onnx_inputs["labels"] = labels.cpu().detach().numpy()
+
+                if self.parent_model.use_merged is True:
+                    onnx_inputs["use_cache_branch"] = use_cache_branch_tensor.cpu().detach().numpy()
             else:
                 onnx_inputs = {
                     "input_ids": input_ids,
                 }
 
                 # Add the encoder_attention_mask inputs when needed
                 if "encoder_attention_mask" in self.input_names:
@@ -535,14 +642,17 @@
                     for input_name, past_key_value in zip(self.key_value_input_names, past_key_values):
                         onnx_inputs[input_name] = past_key_value
 
                 if "labels" in self.input_names:
                     # TODO: Any preprocessing like  `self._shift_right(labels)`?
                     onnx_inputs["labels"] = labels
 
+                if self.parent_model.use_merged is True:
+                    onnx_inputs["use_cache_branch"] = use_cache_branch_tensor
+
             # Run inference
             outputs = self.session.run(None, onnx_inputs)
 
             # TODO: using two loops here is probably unefficient
             # Tuple of length equal to : number of layer * number of past_key_value per decoder layer (2 corresponds to the
             # self-attention layer and 2 to the cross-attention layer)
             out_past_key_values = tuple(
@@ -556,23 +666,43 @@
 
             loss = None
             if "loss" in self.output_names:
                 loss = outputs[self.output_names["loss"]]
                 if use_torch:
                     loss = torch.from_numpy(loss).to(self.device)
 
-        # TODO: this is extremely ugly and unreadable. What if cross-attention k/v change?
-        # Tuple of tuple of length `n_layers`, with each tuple of length equal to:
-        # * 4 for the decoder without cache (k/v of self-attention + k/v of cross-attention)
-        # * 2 for the decoder with cache (k/v of self-attention as cross-attention cache is constant)
-        if self.use_past is False:
-            out_past_key_values = tuple(
-                out_past_key_values[i : i + self.num_pkv] for i in range(0, len(out_past_key_values), self.num_pkv)
-            )
-        else:
-            # grab the cross attention key/values from the inputs
-            out_past_key_values = tuple(
-                out_past_key_values[i : i + self.num_pkv] + past_key_values[2 * i + 2 : 2 * i + 2 + self.num_pkv]
-                for i in range(0, len(out_past_key_values), self.num_pkv)
-            )
+            # TODO: this is extremely ugly and unreadable. What if cross-attention k/v change?
+            # Tuple of tuple of length `n_layers`, with each tuple of length equal to:
+            # * 4 for the decoder without cache (k/v of self-attention + k/v of cross-attention)
+            # * 2 for the decoder with cache (k/v of self-attention as cross-attention cache is constant)
+            if self.use_past is False or use_merged_no_cache:
+                out_past_key_values = tuple(
+                    out_past_key_values[i : i + self.num_pkv] for i in range(0, len(out_past_key_values), self.num_pkv)
+                )
+            else:
+                if self.use_legacy_outputs is True:
+                    msg = (
+                        "For the decoder with past, using ONNX models outputting cross attention past key values"
+                        " is deprecated and the support will be removed in optimum 2.0. We recommend exporting again the model"
+                        " with optimum>=1.7.3."
+                    )
+                    warn_once(logger, msg=msg)
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + self.num_pkv]
+                        for i in range(0, len(out_past_key_values), self.num_pkv)
+                    )
+                # grab the cross attention key/values from the inputs
+                elif self.num_pkv == 2:
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + self.num_pkv]
+                        + past_key_values[2 * i + 2 : 2 * i + 2 + self.num_pkv]
+                        for i in range(0, len(out_past_key_values), self.num_pkv)
+                    )
+                elif self.num_pkv == 4:
+                    out_past_key_values = tuple(
+                        out_past_key_values[i : i + 2] + past_key_values[i + 2 : i + 4]
+                        for i in range(0, len(out_past_key_values), self.num_pkv)
+                    )
+                else:
+                    raise ValueError("Unsupported num_pkv")
 
         return Seq2SeqLMOutput(loss=loss, logits=logits, past_key_values=out_past_key_values)
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/configuration.py` & `optimum-1.8.0/optimum/onnxruntime/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/graph.py` & `optimum-1.8.0/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.8.0/optimum/onnxruntime/io_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.8.0/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/model.py` & `optimum-1.8.0/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.8.0/optimum/onnxruntime/modeling_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 import logging
 import shutil
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import torch
+from huggingface_hub import hf_hub_download
+from huggingface_hub.utils import EntryNotFoundError
 from transformers import AutoModelForCausalLM, GenerationConfig
 from transformers.file_utils import add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import CausalLMOutputWithCrossAttentions
 
 import onnxruntime
 
 from ..exporters.onnx import main_export
 from ..onnx.utils import _get_external_data_paths
 from ..utils import check_if_transformers_greater
 from ..utils.file_utils import validate_file_exists
 from ..utils.save_utils import maybe_load_preprocessors, maybe_save_preprocessors
 from .base import ORTDecoder
+from .constants import DECODER_MERGED_ONNX_FILE_PATTERN, DECODER_ONNX_FILE_PATTERN, DECODER_WITH_PAST_ONNX_FILE_PATTERN
 from .modeling_ort import ORTModel
 from .utils import (
     ONNX_DECODER_NAME,
     ONNX_DECODER_WITH_PAST_NAME,
     get_provider_for_device,
     parse_device,
     validate_provider_availability,
@@ -110,18 +113,14 @@
     >>> onnx_gen = pipeline("text-generation", model=model, tokenizer=tokenizer)
 
     >>> text = "My name is Arthur and I live in"
     >>> gen = onnx_gen(text)
     ```
 """
 
-DECODER_ONNX_FILE_PATTERN = r"(.*)?decoder((?!with_past).)*?\.onnx"
-DECODER_WITH_PAST_ONNX_FILE_PATTERN = r"(.*)?decoder(.*)?with_past(.*)?\.onnx"
-DECODER_MERGED_ONNX_FILE_PATTERN = r"(.*)?decoder(.*)?merged(.*)?\.onnx"
-
 
 class ORTModelDecoder(ORTModel):
     """
     Base class for implementing models with a causal language modeling head using ONNX Runtime inference.
     """
 
     def __init__(
@@ -158,14 +157,20 @@
                 The directory under which the model exported to ONNX was saved.
             preprocessors (`Optional[List]`, defaults to `None`):
                 The list of the preprocessors (tokenizer, processor, feature_extractor) to save alongside the ORTModel.
             generation_config (`Optional[GenerationConfig]`, defaults to `None`):
                 The generation configuration used by default when calling `generate()`.
                 Refer to https://huggingface.co/docs/transformers/main/en/main_classes/text_generation#transformers.GenerationMixin.generate.
         """
+        if use_io_binding is None:
+            if decoder_session.get_providers()[0] == "CUDAExecutionProvider":
+                use_io_binding = True
+            else:
+                use_io_binding = False
+
         self.shared_attributes_init(
             decoder_session,
             use_io_binding=use_io_binding,
             model_save_dir=model_save_dir,
         )
         self.config = config
 
@@ -204,14 +209,22 @@
             use_merged = False
 
             if decoder_with_past_session is not None:
                 raise ValueError(
                     "The parameter decoder_with_past_session was passed, although use_cache is False."
                     "Please pass use_cache=True for decoder_with_past_session to be used."
                 )
+
+        if use_cache is False and use_io_binding is True:
+            raise ValueError(
+                "When using CUDAExecutionProvider, the parameters combination use_cache=False, use_io_binding=True"
+                " is not supported. Please either pass use_cache=True, use_io_binding=True (default),"
+                " or use_cache=False, use_io_binding=False."
+            )
+
         self.onnx_paths = onnx_paths
         self.use_cache = use_cache
         self.use_merged = use_merged
         self.decoder = ORTDecoder(decoder_session, self)
         self.decoder_model_path = Path(decoder_session._model_path)
         self.decoder_model_name = self.decoder_model_path.name
 
@@ -291,14 +304,16 @@
 
         # add external data paths in case of large models
         src_paths, dst_paths = _get_external_data_paths(src_paths, dst_paths)
 
         for src_path, dst_path in zip(src_paths, dst_paths):
             shutil.copyfile(src_path, dst_path)
 
+        self.generation_config.save_pretrained(save_directory)
+
     @classmethod
     def _from_pretrained(
         cls,
         model_id: Union[str, Path],
         config: "PretrainedConfig",
         use_auth_token: Optional[Union[bool, str]] = None,
         revision: Optional[str] = None,
@@ -315,102 +330,160 @@
         provider_options: Optional[Dict[str, Any]] = None,
         use_io_binding: Optional[bool] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         **kwargs,
     ):
         model_path = Path(model_id)
 
+        # We do not implement the logic for use_cache=False, use_merged=True
+        if use_cache is False:
+            if use_merged is True:
+                raise ValueError(
+                    "The parameters combination use_cache=False, use_merged=True is not supported."
+                    " To use a merged decoder, past key values must be used."
+                )
+            use_merged = False
+
         decoder_merged_path = None
+        # We use `is not False` here to include two cases: use_merged = None (in which case we auto-detect it),
+        # and use_merged = True (explicitely specified by the user)
         if use_merged is not False:
             try:
                 decoder_merged_path = ORTModelDecoder.infer_onnx_filename(
                     model_id,
                     [DECODER_MERGED_ONNX_FILE_PATTERN],
                     argument_name=None,
                     subfolder=subfolder,
                     use_auth_token=use_auth_token,
                     revision=revision,
                 )
                 use_merged = True
+                decoder_path = decoder_merged_path
             except FileNotFoundError as e:
                 if use_merged is True:
                     raise FileNotFoundError(
                         "The parameter `use_merged=True` was passed to ORTModelForCausalLM.from_pretrained()"
                         " but no ONNX file for a merged decoder could be found in"
                         f" {str(Path(model_id, subfolder))}, with the error: {e}"
                     )
                 use_merged = False
 
-        if not validate_file_exists(model_id, decoder_file_name, subfolder=subfolder, revision=revision):
-            decoder_without_past_path = ORTModelDecoder.infer_onnx_filename(
-                model_id,
-                [DECODER_ONNX_FILE_PATTERN],
-                "decoder_file_name",
-                subfolder=subfolder,
-                use_auth_token=use_auth_token,
-                revision=revision,
-            )
-        else:
-            decoder_without_past_path = model_path / subfolder / decoder_file_name
-
-        if use_merged is True:
-            decoder_path = decoder_merged_path
-        else:
-            decoder_path = decoder_without_past_path
-
-        decoder_regular_onnx_filenames = ORTModelDecoder._generate_regular_names_for_filename(ONNX_DECODER_NAME)
-        if decoder_path.name not in decoder_regular_onnx_filenames:
-            logger.warning(
-                f"The ONNX file {decoder_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_regular_onnx_filenames}, the "
-                f"{cls.__name__} might not behave as expected."
-            )
-
-        # If the decoder without / with past has been merged, we do not need to look for any additional file
+        decoder_without_past_path = None
         decoder_with_past_path = None
-        if not validate_file_exists(model_id, decoder_with_past_file_name, subfolder=subfolder, revision=revision):
-            try:
-                decoder_with_past_path = ORTModelDecoder.infer_onnx_filename(
+        if use_merged is False:
+            if not validate_file_exists(model_id, decoder_file_name, subfolder=subfolder, revision=revision):
+                decoder_without_past_path = ORTModelDecoder.infer_onnx_filename(
                     model_id,
-                    [DECODER_WITH_PAST_ONNX_FILE_PATTERN],
-                    "decoder_with_past_file_name",
+                    [DECODER_ONNX_FILE_PATTERN],
+                    "decoder_file_name",
                     subfolder=subfolder,
                     use_auth_token=use_auth_token,
                     revision=revision,
                 )
-            except FileNotFoundError as e:
-                if use_cache is True and use_merged is False:
-                    raise FileNotFoundError(
-                        "The parameter `use_cache=True` was passed to ORTModelForCausalLM.from_pretrained()"
-                        " but no ONNX file using past key values could be found in"
-                        f" {str(Path(model_id, subfolder))}, with the error: {e}"
-                    )
-        else:
-            decoder_with_past_path = model_path / subfolder / decoder_with_past_file_name
+            else:
+                decoder_without_past_path = model_path / subfolder / decoder_file_name
 
-        if use_cache is True and use_merged is False:
-            decoder_with_past_regular_onnx_filenames = ORTModelDecoder._generate_regular_names_for_filename(
-                ONNX_DECODER_WITH_PAST_NAME
-            )
+            decoder_path = decoder_without_past_path
 
-            if decoder_with_past_path.name not in decoder_with_past_regular_onnx_filenames:
+            decoder_regular_onnx_filenames = ORTModelDecoder._generate_regular_names_for_filename(ONNX_DECODER_NAME)
+            if decoder_path.name not in decoder_regular_onnx_filenames:
                 logger.warning(
-                    f"The ONNX file {decoder_with_past_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_with_past_regular_onnx_filenames}, "
-                    f"the {cls.__name__} might not behave as expected."
+                    f"The ONNX file {decoder_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_regular_onnx_filenames}, the "
+                    f"{cls.__name__} might not behave as expected."
+                )
+
+            # If the decoder without / with past has been merged, we do not need to look for any additional file
+            if use_cache is True:
+                if not validate_file_exists(
+                    model_id, decoder_with_past_file_name, subfolder=subfolder, revision=revision
+                ):
+                    try:
+                        decoder_with_past_path = ORTModelDecoder.infer_onnx_filename(
+                            model_id,
+                            [DECODER_WITH_PAST_ONNX_FILE_PATTERN],
+                            "decoder_with_past_file_name",
+                            subfolder=subfolder,
+                            use_auth_token=use_auth_token,
+                            revision=revision,
+                        )
+                    except FileNotFoundError as e:
+                        raise FileNotFoundError(
+                            "The parameter `use_cache=True` was passed to ORTModelForCausalLM.from_pretrained()"
+                            " but no ONNX file using past key values could be found in"
+                            f" {str(Path(model_id, subfolder))}, with the error: {e}"
+                        )
+                else:
+                    decoder_with_past_path = model_path / subfolder / decoder_with_past_file_name
+
+                decoder_with_past_regular_onnx_filenames = ORTModelDecoder._generate_regular_names_for_filename(
+                    ONNX_DECODER_WITH_PAST_NAME
                 )
 
+                if decoder_with_past_path.name not in decoder_with_past_regular_onnx_filenames:
+                    logger.warning(
+                        f"The ONNX file {decoder_with_past_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_with_past_regular_onnx_filenames}, "
+                        f"the {cls.__name__} might not behave as expected."
+                    )
+
         preprocessors = None
         if model_path.is_dir():
             new_model_save_dir = model_path
             preprocessors = maybe_load_preprocessors(model_id)
+        else:
+            attribute_name_to_filename = {
+                "last_decoder_model_name": decoder_path.name if use_merged is False else None,
+                "last_decoder_with_past_model_name": decoder_with_past_path.name
+                if (use_cache is True and use_merged is False)
+                else None,
+                "last_decoder_merged_name": decoder_merged_path.name if use_merged is True else None,
+            }
+            paths = {}
+            for attr_name, filename in attribute_name_to_filename.items():
+                if filename is None:
+                    continue
+                model_cache_path = hf_hub_download(
+                    repo_id=model_id,
+                    subfolder=subfolder,
+                    filename=filename,
+                    use_auth_token=use_auth_token,
+                    revision=revision,
+                    cache_dir=cache_dir,
+                    force_download=force_download,
+                    local_files_only=local_files_only,
+                )
 
-        onnx_paths = [decoder_path]
-        if use_cache is True and use_merged is False:
-            onnx_paths.append(decoder_with_past_path)
-        if use_cache is True and use_merged is True:
-            onnx_paths.append(decoder_with_past_path)
+                # try download external data
+                try:
+                    hf_hub_download(
+                        repo_id=model_id,
+                        subfolder=subfolder,
+                        filename=filename + "_data",
+                        use_auth_token=use_auth_token,
+                        revision=revision,
+                        cache_dir=cache_dir,
+                        force_download=force_download,
+                        local_files_only=local_files_only,
+                    )
+                except EntryNotFoundError:
+                    # model doesn't use external data
+                    pass
+
+                paths[attr_name] = Path(model_cache_path).name
+            new_model_save_dir = Path(model_cache_path).parent
+            preprocessors = maybe_load_preprocessors(model_id, subfolder=subfolder)
+
+            if use_merged is True:
+                decoder_path = new_model_save_dir / paths["last_decoder_merged_name"]
+                decoder_merged_path = new_model_save_dir / paths["last_decoder_merged_name"]
+            else:
+                decoder_path = new_model_save_dir / paths["last_decoder_model_name"]
+                decoder_without_past_path = new_model_save_dir / paths["last_decoder_model_name"]
+
+                if use_cache is True:
+                    decoder_with_past_path = new_model_save_dir / paths["last_decoder_with_past_model_name"]
 
         ort_inference_sessions = cls.load_model(
             decoder_path=decoder_path,
             decoder_with_past_path=None if use_merged is True or use_cache is False else decoder_with_past_path,
             provider=provider,
             session_options=session_options,
             provider_options=provider_options,
@@ -429,19 +502,21 @@
                 use_auth_token=use_auth_token,
                 revision=revision,
                 subfolder=subfolder,
             )
         except OSError:
             logger.info("Generation config file not found, using a generation config created from the model config.")
 
-        onnx_paths = [decoder_without_past_path]
-        if decoder_merged_path is not None:
+        onnx_paths = []
+        if use_merged is False:
+            onnx_paths.append(decoder_without_past_path)
+            if use_cache is True:
+                onnx_paths.append(decoder_with_past_path)
+        else:
             onnx_paths.append(decoder_merged_path)
-        if decoder_with_past_path is not None:
-            onnx_paths.append(decoder_with_past_path)
 
         return cls(
             ort_inference_sessions[0],
             config,
             decoder_with_past_session=ort_inference_sessions[1],
             use_cache=use_cache,
             use_io_binding=use_io_binding,
@@ -603,15 +678,14 @@
 
         return {
             "input_ids": input_ids,
             "past_key_values": past_key_values,
             "use_cache": use_cache,
             "position_ids": None,
             "attention_mask": attention_mask,
-            "token_type_ids": None,
         }
 
     # Copied from transformers.models.gpt2.modeling_gpt2.GPT2LMHeadModel._reorder_cache
     @staticmethod
     def _reorder_cache(past: Tuple[Tuple[torch.Tensor]], beam_idx: torch.Tensor) -> Tuple[Tuple[torch.Tensor]]:
         return tuple(
             tuple(past_state.index_select(0, beam_idx.to(past_state.device)) for past_state in layer_past)
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.8.0/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/modeling_ort.py` & `optimum-1.8.0/optimum/onnxruntime/modeling_ort.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,20 @@
         use_io_binding: Optional[bool] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         preprocessors: Optional[List] = None,
         **kwargs,
     ):
         super().__init__(model, config)
 
+        if use_io_binding is None:
+            if model.get_providers()[0] == "CUDAExecutionProvider":
+                use_io_binding = True
+            else:
+                use_io_binding = False
+
         self.model_path = Path(model._model_path)
         self.model_name = self.model_path.name
 
         self.shared_attributes_init(
             model,
             use_io_binding,
             model_save_dir,
@@ -779,14 +785,15 @@
             if output_name in known_output_shapes:
                 output_shape = known_output_shapes[output_name]
             else:
                 output_shape = []
                 for axis_name in output_node.shape:
                     output_shape.append(self._output_shape_inference(axis_name, dimensions))
             output_buffer = self._prepare_output_buffer(model, output_shape, output_name)
+
             io_binding.bind_output(
                 output_name,
                 output_buffer.device.type,
                 self.device.index,
                 name_to_np_type[output_name],
                 output_shape,
                 output_buffer.data_ptr(),
@@ -970,15 +977,15 @@
     auto_model_class = AutoModelForMaskedLM
 
     @add_start_docstrings_to_model_forward(
         ONNX_TEXT_INPUTS_DOCSTRING.format("batch_size, sequence_length")
         + MASKED_LM_EXAMPLE.format(
             processor_class=_TOKENIZER_FOR_DOC,
             model_class="ORTModelForMaskedLM",
-            checkpoint="optimum/bert-base-uncased-for-masked-lm",
+            checkpoint="optimum/bert-base-uncased-for-fill-mask",
         )
     )
     def forward(
         self,
         input_ids: Optional[Union[torch.Tensor, np.ndarray]] = None,
         attention_mask: Optional[Union[torch.Tensor, np.ndarray]] = None,
         token_type_ids: Optional[Union[torch.Tensor, np.ndarray]] = None,
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.8.0/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,47 @@
 """
 ORTModelForXXX classes related to seq2seq, allowing to run ONNX Models with ONNX Runtime using the same API as
 Transformers.
 """
 
 import logging
 import shutil
-from abc import ABC, abstractmethod
+from abc import ABC, ABCMeta, abstractmethod
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from huggingface_hub import hf_hub_download
-from transformers import AutoModelForSeq2SeqLM, AutoModelForSpeechSeq2Seq, AutoModelForVision2Seq, GenerationConfig
+from transformers import (
+    AutoModelForSeq2SeqLM,
+    AutoModelForSpeechSeq2Seq,
+    AutoModelForVision2Seq,
+    GenerationConfig,
+    WhisperForConditionalGeneration,
+)
 from transformers.file_utils import add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
 
 import onnxruntime as ort
 
 from ..exporters.onnx import main_export
 from ..onnx.utils import _get_external_data_paths
 from ..utils import check_if_transformers_greater
 from ..utils.file_utils import validate_file_exists
 from ..utils.normalized_config import NormalizedConfigManager
 from ..utils.save_utils import maybe_load_preprocessors, maybe_save_preprocessors
 from .base import ORTDecoderForSeq2Seq, ORTEncoder
+from .constants import (
+    DECODER_MERGED_ONNX_FILE_PATTERN,
+    DECODER_ONNX_FILE_PATTERN,
+    DECODER_WITH_PAST_ONNX_FILE_PATTERN,
+    ENCODER_ONNX_FILE_PATTERN,
+)
 from .modeling_ort import ORTModel
 from .utils import (
     ONNX_DECODER_NAME,
     ONNX_DECODER_WITH_PAST_NAME,
     ONNX_ENCODER_NAME,
     get_provider_for_device,
     parse_device,
@@ -264,18 +276,14 @@
     >>> image = Image.open(requests.get(url, stream=True).raw)
 
     >>> image_to_text = pipeline("image-to-text", model=model, tokenizer=tokenizer, feature_extractor=processor, image_processor=processor)
     >>> pred = image_to_text(image)
     ```
 """
 
-ENCODER_ONNX_FILE_PATTERN = r"(.*)?encoder(.*)?\.onnx"
-DECODER_ONNX_FILE_PATTERN = r"(.*)?decoder((?!with_past).)*?\.onnx"
-DECODER_WITH_PAST_ONNX_FILE_PATTERN = r"(.*)?decoder(.*)?with_past(.*)?\.onnx"
-
 
 class ORTEncoderForSpeech(ORTEncoder):
     """
     Encoder model for ONNX Runtime inference for Whisper model.
 
     Args:
         session (`ort.InferenceSession`):
@@ -415,15 +423,17 @@
     base_model_prefix = "onnx_model"
 
     def __init__(
         self,
         encoder_session: ort.InferenceSession,
         decoder_session: ort.InferenceSession,
         config: "PretrainedConfig",
+        onnx_paths: List[str],
         decoder_with_past_session: Optional[ort.InferenceSession] = None,
+        use_cache: bool = True,
         use_io_binding: Optional[bool] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         preprocessors: Optional[List] = None,
         generation_config: Optional[GenerationConfig] = None,
         **kwargs,
     ):
         """
@@ -431,14 +441,16 @@
             encoder_session (`ort.InferenceSession`):
                 The ONNX Runtime inference session associated to the encoder.
             decoder_session (`ort.InferenceSession`):
                 The ONNX Runtime inference session associated to the decoder.
             config ([`PretrainedConfig`]):
                 `config` is an instance of the configuration associated to the model. Initializing with a config file
                 does not load the weights associated with the model, only the configuration.
+            onnx_paths (`List[str]`):
+                Path to ONNX files associated with the model.
             decoder_with_past_session (`Optional[ort.InferenceSession]`, *optional*):
                 The ONNX Runtime inference session associated to the decoder with past key values.
             use_io_binding (`bool`, *optional*, defaults to `None`):
                 Whether use IOBinding during inference to avoid memory copy between the host and devices. Defaults to
                 `True` if the device is CUDA, otherwise defaults to `False`.
             model_save_dir (`str`, *optional*, defaults to `""`):
                 The directory under which the model exported to ONNX was saved.
@@ -463,37 +475,79 @@
         if kwargs:
             raise ValueError(
                 f"{self.__class__.__name__} received {', '.join(kwargs.keys())}, but do not accept those arguments."
             )
 
         ABC.__init__(self)
 
+        if use_io_binding is None:
+            if decoder_session.get_providers()[0] == "CUDAExecutionProvider":
+                use_io_binding = True
+            else:
+                use_io_binding = False
+
         self.shared_attributes_init(
             encoder_session,
             use_io_binding=use_io_binding,
             model_save_dir=model_save_dir,
             preprocessors=preprocessors,
         )
         self.config = config
-        self.use_cache = decoder_with_past_session is not None
+
+        self.onnx_paths = onnx_paths
+        self.use_cache = use_cache
+
+        if use_cache is True:
+            # Auto-detect whether the provided session is a merged non-past / with-past or not
+            # TODO: make __init__ private and pass `use_merged` as an argument
+            use_merged = "use_cache_branch" in [inp.name for inp in decoder_session.get_inputs()]
+
+            if use_merged is True and decoder_with_past_session is not None:
+                raise ValueError(
+                    "Detected a merged decoder, but decoder_with_past_session was provided."
+                    "Please only set decoder_session, or provide a non-merged decoder_session."
+                )
+            if use_cache is True and use_merged is False and decoder_with_past_session is None:
+                raise ValueError(
+                    "The parameter use_cache was set as True, but neither decoder_with_past_session was passed"
+                    " nor a use_cache branch can be found in the decoder_session."
+                    " Please pass a decoder_with_past_session or set use_cache=False."
+                )
+        else:
+            use_merged = False
+
+            if decoder_with_past_session is not None:
+                raise ValueError(
+                    "The parameter decoder_with_past_session was passed, although use_cache is False."
+                    "Please pass use_cache=True for decoder_with_past_session to be used."
+                )
+
+        if use_cache is False and use_io_binding is True:
+            raise ValueError(
+                "When using CUDAExecutionProvider, the parameters combination use_cache=False, use_io_binding=True"
+                " is not supported. Please either pass use_cache=True, use_io_binding=True (default),"
+                " or use_cache=False, use_io_binding=False."
+            )
+
+        self.use_merged = use_merged
 
         self.encoder = self._initialize_encoder(encoder_session)
         self.encoder_model_path = Path(encoder_session._model_path)
         self.encoder_model_name = self.encoder_model_path.name
 
         self.decoder = ORTDecoderForSeq2Seq(decoder_session, self)
         self.decoder_model_path = Path(decoder_session._model_path)
         self.decoder_model_name = self.decoder_model_path.name
 
         # If a decoder_with_past_path is provided, an inference session for the decoder with past key/values as inputs
         # will be enabled
         self.decoder_with_past = None
         self.decoder_with_past_model_path = None
         self.decoder_with_past_model_name = None
-        if self.use_cache:
+        if self.use_cache is True and self.use_merged is False:
             self.decoder_with_past = ORTDecoderForSeq2Seq(decoder_with_past_session, self)
             self.decoder_with_past_model_path = Path(decoder_with_past_session._model_path)
             self.decoder_with_past_model_name = self.decoder_with_past_model_path.name
 
         if generation_config is None:
             generation_config = GenerationConfig.from_model_config(config)
         self.generation_config = generation_config
@@ -552,27 +606,25 @@
         [`~optimum.onnxruntime.modeling_seq2seq.ORTModelForSeq2SeqLM.from_pretrained`] class method.
 
         Args:
             save_directory (`Union[str, Path`]):
                 The directory where to save the model files.
         """
         save_directory = Path(save_directory)
-        src_paths = [self.encoder_model_path, self.decoder_model_path]
-        dst_paths = [save_directory / self.encoder_model_path.name, save_directory / self.decoder_model_path.name]
-        if self.use_cache:
-            src_paths.append(self.decoder_with_past_model_path)
-            dst_paths.append(save_directory / self.decoder_with_past_model_path.name)
+        src_paths = [Path(path) for path in self.onnx_paths]
+        dst_paths = [save_directory / path.name for path in src_paths]
 
         # add external data paths in case of large models
         src_paths, dst_paths = _get_external_data_paths(src_paths, dst_paths)
 
         for src_path, dst_path in zip(src_paths, dst_paths):
-            dst_path.parent.mkdir(parents=True, exist_ok=True)
             shutil.copyfile(src_path, dst_path)
 
+        self.generation_config.save_pretrained(save_directory)
+
     @classmethod
     def _from_pretrained(
         cls,
         model_id: Union[str, Path],
         config: "PretrainedConfig",
         use_auth_token: Optional[Union[bool, str]] = None,
         revision: Optional[str] = None,
@@ -580,116 +632,151 @@
         cache_dir: Optional[str] = None,
         encoder_file_name: str = ONNX_ENCODER_NAME,
         decoder_file_name: str = ONNX_DECODER_NAME,
         decoder_with_past_file_name: str = ONNX_DECODER_WITH_PAST_NAME,
         subfolder: str = "",
         local_files_only: bool = False,
         use_cache: bool = True,
+        use_merged: Optional[bool] = None,
         provider: str = "CPUExecutionProvider",
         session_options: Optional[ort.SessionOptions] = None,
         provider_options: Optional[Dict[str, Any]] = None,
         use_io_binding: Optional[bool] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         **kwargs,
     ):
         model_path = Path(model_id)
 
+        # We do not implement the logic for use_cache=False, use_merged=True
+        if use_cache is False:
+            if use_merged is True:
+                raise ValueError(
+                    "The parameters combination use_cache=False, use_merged=True is not supported."
+                    " To use a merged decoder, past key values must be used."
+                )
+            use_merged = False
+
+        decoder_merged_path = None
+        # We use `is not False` here to include two cases: use_merged = None (in which case we auto-detect it),
+        # and use_merged = True (explicitely specified by the user)
+        if use_merged is not False:
+            try:
+                decoder_merged_path = ORTModelForConditionalGeneration.infer_onnx_filename(
+                    model_id,
+                    [DECODER_MERGED_ONNX_FILE_PATTERN],
+                    argument_name=None,
+                    subfolder=subfolder,
+                    use_auth_token=use_auth_token,
+                    revision=revision,
+                )
+                use_merged = True
+                decoder_path = decoder_merged_path
+            except FileNotFoundError as e:
+                if use_merged is True:
+                    raise FileNotFoundError(
+                        "The parameter `use_merged=True` was passed to ORTModelForCausalLM.from_pretrained()"
+                        " but no ONNX file for a merged decoder could be found in"
+                        f" {str(Path(model_id, subfolder))}, with the error: {e}"
+                    )
+                use_merged = False
+
+        decoder_without_past_path = None
+        decoder_with_past_path = None
+        if use_merged is False:
+            if not validate_file_exists(model_id, decoder_file_name, subfolder=subfolder, revision=revision):
+                decoder_without_past_path = ORTModelForConditionalGeneration.infer_onnx_filename(
+                    model_id,
+                    [DECODER_ONNX_FILE_PATTERN],
+                    "decoder_file_name",
+                    subfolder=subfolder,
+                    use_auth_token=use_auth_token,
+                    revision=revision,
+                )
+            else:
+                decoder_without_past_path = model_path / subfolder / decoder_file_name
+
+            decoder_path = decoder_without_past_path
+
+            decoder_regular_onnx_filenames = ORTModelForConditionalGeneration._generate_regular_names_for_filename(
+                ONNX_DECODER_NAME
+            )
+            if decoder_path.name not in decoder_regular_onnx_filenames:
+                logger.warning(
+                    f"The ONNX file {decoder_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_regular_onnx_filenames}, the "
+                    f"{cls.__name__} might not behave as expected."
+                )
+
+            # If the decoder without / with past has been merged, we do not need to look for any additional file
+            if use_cache is True and use_merged is False:
+                if not validate_file_exists(
+                    model_id, decoder_with_past_file_name, subfolder=subfolder, revision=revision
+                ):
+                    try:
+                        decoder_with_past_path = ORTModelForConditionalGeneration.infer_onnx_filename(
+                            model_id,
+                            [DECODER_WITH_PAST_ONNX_FILE_PATTERN],
+                            "decoder_with_past_file_name",
+                            subfolder=subfolder,
+                            use_auth_token=use_auth_token,
+                            revision=revision,
+                        )
+                    except FileNotFoundError as e:
+                        raise FileNotFoundError(
+                            "The parameter `use_cache=True` was passed to ORTModelForCausalLM.from_pretrained()"
+                            " but no ONNX file using past key values could be found in"
+                            f" {str(Path(model_id, subfolder))}, with the error: {e}"
+                        )
+                else:
+                    decoder_with_past_path = model_path / subfolder / decoder_with_past_file_name
+
+                decoder_path = decoder_without_past_path
+
+                decoder_with_past_regular_onnx_filenames = (
+                    ORTModelForConditionalGeneration._generate_regular_names_for_filename(ONNX_DECODER_WITH_PAST_NAME)
+                )
+
+                if decoder_with_past_path.name not in decoder_with_past_regular_onnx_filenames:
+                    logger.warning(
+                        f"The ONNX file {decoder_with_past_path.name} is not a regular name used in optimum.onnxruntime that are {decoder_with_past_regular_onnx_filenames}, "
+                        f"the {cls.__name__} might not behave as expected."
+                    )
+
         if not validate_file_exists(model_id, encoder_file_name, subfolder=subfolder, revision=revision):
             encoder_path = ORTModelForConditionalGeneration.infer_onnx_filename(
                 model_id,
                 [ENCODER_ONNX_FILE_PATTERN],
                 "encoder_file_name",
                 subfolder=subfolder,
                 use_auth_token=use_auth_token,
                 revision=revision,
             )
         else:
             encoder_path = model_path / subfolder / encoder_file_name
-        if not validate_file_exists(model_id, decoder_file_name, subfolder=subfolder, revision=revision):
-            decoder_path = ORTModelForConditionalGeneration.infer_onnx_filename(
-                model_id,
-                [DECODER_ONNX_FILE_PATTERN],
-                "decoder_file_name",
-                subfolder=subfolder,
-                use_auth_token=use_auth_token,
-                revision=revision,
-            )
-        else:
-            decoder_path = model_path / subfolder / decoder_file_name
-
-        if use_cache is True:
-            if not validate_file_exists(model_id, decoder_with_past_file_name, subfolder=subfolder, revision=revision):
-                try:
-                    decoder_with_past_path = ORTModelForConditionalGeneration.infer_onnx_filename(
-                        model_id,
-                        [DECODER_WITH_PAST_ONNX_FILE_PATTERN],
-                        "decoder_with_past_file_name",
-                        subfolder=subfolder,
-                        use_auth_token=use_auth_token,
-                        revision=revision,
-                    )
-                except FileNotFoundError as e:
-                    raise FileNotFoundError(
-                        "The parameter `use_cache=True` was passed to `ORTModelForConditionalGeneration.from_pretrained()`"
-                        " but no ONNX file using past key values could be found in"
-                        f" {str(Path(model_id, subfolder))}, with the error:\n    {e}"
-                    )
-            else:
-                decoder_with_past_path = model_path / subfolder / decoder_with_past_file_name
 
         encoder_regular_onnx_filenames = ORTModelForConditionalGeneration._generate_regular_names_for_filename(
             ONNX_ENCODER_NAME
         )
-        decoder_regular_onnx_filenames = ORTModelForConditionalGeneration._generate_regular_names_for_filename(
-            ONNX_DECODER_NAME
-        )
-        decoder_with_past_regular_onnx_filenames = (
-            ORTModelForConditionalGeneration._generate_regular_names_for_filename(ONNX_DECODER_WITH_PAST_NAME)
-        )
-
         if encoder_path.name not in encoder_regular_onnx_filenames:
             logger.warning(
                 f"The ONNX file {encoder_path.name} is not a regular name used in optimum.onnxruntime, the "
                 "ORTModelForConditionalGeneration might not behave as expected."
             )
 
-        if decoder_path.name not in decoder_regular_onnx_filenames:
-            logger.warning(
-                f"The ONNX file {decoder_path.name} is not a regular name used in optimum.onnxruntime, the "
-                "ORTModelForConditionalGeneration might not behave as expected."
-            )
-        if (
-            use_cache is True
-            and decoder_with_past_path is not None
-            and decoder_with_past_path.name not in decoder_with_past_regular_onnx_filenames
-        ):
-            logger.warning(
-                f"The ONNX file {decoder_with_past_path.name} is not a regular name used in optimum.onnxruntime, "
-                "the ORTModelForConditionalGeneration might not behave as expected."
-            )
-
-        decoder_with_past_path = decoder_with_past_path if use_cache else None
-
         preprocessors = None
         if model_path.is_dir():
-            inference_sessions = cls.load_model(
-                encoder_path=encoder_path,
-                decoder_path=decoder_path,
-                decoder_with_past_path=decoder_with_past_path,
-                provider=provider,
-                session_options=session_options,
-                provider_options=provider_options,
-            )
             new_model_save_dir = model_path
             preprocessors = maybe_load_preprocessors(model_id)
         else:
             attribute_name_to_filename = {
                 "last_encoder_model_name": encoder_path.name,
-                "last_decoder_model_name": decoder_path.name,
-                "last_decoder_with_past_model_name": decoder_with_past_path.name if use_cache else None,
+                "last_decoder_model_name": decoder_path.name if use_merged is False else None,
+                "last_decoder_with_past_model_name": decoder_with_past_path.name
+                if (use_merged is False and use_cache is True)
+                else None,
+                "last_decoder_merged_name": decoder_merged_path.name if use_merged is True else None,
             }
             paths = {}
             for attr_name, filename in attribute_name_to_filename.items():
                 if filename is None:
                     continue
                 model_cache_path = hf_hub_download(
                     repo_id=model_id,
@@ -717,26 +804,34 @@
                     # model doesn't use external data
                     pass
 
                 paths[attr_name] = Path(model_cache_path).name
             new_model_save_dir = Path(model_cache_path).parent
             preprocessors = maybe_load_preprocessors(model_id, subfolder=subfolder)
 
-            last_decoder_with_past_name = paths.get("last_decoder_with_past_model_name", None)
-            if last_decoder_with_past_name is not None:
-                last_decoder_with_past_name = new_model_save_dir / last_decoder_with_past_name
-
-            inference_sessions = cls.load_model(
-                encoder_path=new_model_save_dir / paths["last_encoder_model_name"],
-                decoder_path=new_model_save_dir / paths["last_decoder_model_name"],
-                decoder_with_past_path=last_decoder_with_past_name,
-                provider=provider,
-                session_options=session_options,
-                provider_options=provider_options,
-            )
+            if use_merged is True:
+                decoder_path = new_model_save_dir / paths["last_decoder_merged_name"]
+                decoder_merged_path = new_model_save_dir / paths["last_decoder_merged_name"]
+            else:
+                decoder_path = new_model_save_dir / paths["last_decoder_model_name"]
+                decoder_without_past_path = new_model_save_dir / paths["last_decoder_model_name"]
+
+                if use_cache is True:
+                    decoder_with_past_path = new_model_save_dir / paths["last_decoder_with_past_model_name"]
+
+            encoder_path = new_model_save_dir / paths["last_encoder_model_name"]
+
+        ort_inference_sessions = cls.load_model(
+            encoder_path=encoder_path,
+            decoder_path=decoder_path,
+            decoder_with_past_path=None if use_merged is True or use_cache is False else decoder_with_past_path,
+            provider=provider,
+            session_options=session_options,
+            provider_options=provider_options,
+        )
 
         if model_save_dir is None:
             model_save_dir = new_model_save_dir
 
         generation_config = None
         try:
             generation_config = GenerationConfig.from_pretrained(
@@ -747,18 +842,28 @@
                 use_auth_token=use_auth_token,
                 revision=revision,
                 subfolder=subfolder,
             )
         except OSError:
             logger.info("Generation config file not found, using a generation config created from the model config.")
 
+        onnx_paths = [encoder_path]
+        if use_merged is False:
+            onnx_paths.append(decoder_without_past_path)
+            if use_cache is True:
+                onnx_paths.append(decoder_with_past_path)
+        else:
+            onnx_paths.append(decoder_merged_path)
+
         return cls(
-            *inference_sessions[:2],
+            *ort_inference_sessions[:2],
             config,
-            decoder_with_past_session=inference_sessions[2],
+            onnx_paths=onnx_paths,
+            use_cache=use_cache,
+            decoder_with_past_session=ort_inference_sessions[2],
             use_io_binding=use_io_binding,
             model_save_dir=model_save_dir,
             preprocessors=preprocessors,
             generation_config=generation_config,
         )
 
     @classmethod
@@ -770,35 +875,44 @@
         revision: str = "main",
         force_download: bool = True,
         cache_dir: Optional[str] = None,
         subfolder: str = "",
         local_files_only: bool = False,
         trust_remote_code: bool = False,
         use_cache: bool = True,
+        use_merged: bool = False,
         provider: str = "CPUExecutionProvider",
         session_options: Optional[ort.SessionOptions] = None,
         provider_options: Optional[Dict[str, Any]] = None,
         use_io_binding: Optional[bool] = None,
         task: Optional[str] = None,
     ) -> "ORTModelForConditionalGeneration":
+        if use_cache is False and use_merged is True:
+            raise ValueError(
+                "The incompatible arguments use_cache=False, use_merged=True were passed to"
+                " ORTModelForConditionalGeneration.from_pretrained(). Please pass either use_cache=False,"
+                " use_merged=False to disable past key value caching, or use_cache=True, use_merged=False"
+                " to disable the merging of the decoder not using / using past key and value."
+            )
+
         if task is None:
             task = cls._auto_model_to_task(cls.auto_model_class)
 
             if use_cache is True:
                 task = task + "-with-past"
 
         save_dir = TemporaryDirectory()
         save_dir_path = Path(save_dir.name)
 
         main_export(
             model_name_or_path=model_id,
             output=save_dir_path,
             task=task,
             do_validation=False,
-            no_post_process=True,
+            no_post_process=not use_merged,
             subfolder=subfolder,
             revision=revision,
             cache_dir=cache_dir,
             use_auth_token=use_auth_token,
             local_files_only=local_files_only,
             force_download=force_download,
             trust_remote_code=trust_remote_code,
@@ -807,14 +921,15 @@
         config.save_pretrained(save_dir_path)
         maybe_save_preprocessors(model_id, save_dir_path, src_subfolder=subfolder)
 
         return cls._from_pretrained(
             save_dir_path,
             config,
             use_cache=use_cache,
+            use_merged=use_merged,
             provider=provider,
             session_options=session_options,
             provider_options=provider_options,
             use_io_binding=use_io_binding,
             model_save_dir=save_dir,
         )
 
@@ -884,21 +999,29 @@
         **kwargs,
     ) -> Seq2SeqLMOutput:
         # Encode if needed : first prediction pass
         if encoder_outputs is None:
             encoder_outputs = self.encoder(input_ids=input_ids, attention_mask=attention_mask)
 
         # Decode
-        if past_key_values is None or self.decoder_with_past is None:
+        if past_key_values is None or self.use_cache is False:
             decoder_outputs = self.decoder(
                 input_ids=decoder_input_ids,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 encoder_attention_mask=attention_mask,
                 labels=labels,
             )
+        elif self.use_merged is True:
+            decoder_outputs = self.decoder(
+                input_ids=decoder_input_ids[:, -1:],
+                encoder_hidden_states=encoder_outputs.last_hidden_state,
+                past_key_values=past_key_values,
+                encoder_attention_mask=attention_mask,
+                labels=labels,
+            )
         else:
             decoder_outputs = self.decoder_with_past(
                 input_ids=decoder_input_ids[:, -1:],  # Cut decoder_input_ids if past is used
                 past_key_values=past_key_values,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 encoder_attention_mask=attention_mask,
                 labels=labels,
@@ -982,20 +1105,28 @@
         **kwargs,
     ) -> Seq2SeqLMOutput:
         # Encode if needed : first prediction pass
         if encoder_outputs is None:
             encoder_outputs = self.encoder(input_features=input_features, attention_mask=attention_mask)
 
         # Decode
-        if past_key_values is None or self.decoder_with_past is None:
+        if past_key_values is None or self.use_cache is False:
             decoder_outputs = self.decoder(
                 input_ids=decoder_input_ids,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 labels=labels,
             )
+        elif self.use_merged is True:
+            decoder_outputs = self.decoder(
+                input_ids=decoder_input_ids[:, -1:],
+                encoder_hidden_states=encoder_outputs.last_hidden_state,
+                past_key_values=past_key_values,
+                encoder_attention_mask=attention_mask,
+                labels=labels,
+            )
         else:
             decoder_outputs = self.decoder_with_past(
                 input_ids=decoder_input_ids[:, -1:],  # Cut decoder_input_ids if past is used
                 past_key_values=past_key_values,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 labels=labels,
             )
@@ -1042,40 +1173,88 @@
             )
         return reordered_past
 
     def can_generate(self):
         """Returns True to validate the check that the model using `GenerationMixin.generate()` can indeed generate."""
         return True
 
+    @classmethod
+    def _from_pretrained(
+        cls,
+        model_id: Union[str, Path],
+        config: "PretrainedConfig",
+        **kwargs,
+    ):
+        if "WhisperForConditionalGeneration" in config.architectures:
+            return _ORTModelForWhisper._from_pretrained(model_id, config, **kwargs)
+        else:
+            return super()._from_pretrained(model_id, config, **kwargs)
+
+
+class MetaClassRemoveParentsAndReorder(ABCMeta):
+    def mro(cls):
+        """
+        Avoids inheritting from PreTrainedModel, nn.Module, ModuleUtilsMixin, PushToHubMixin,
+        and put GenerationMixin at the end of the MRO
+        """
+        top_inheritance_index = ORTModelForSpeechSeq2Seq.__mro__.index(GenerationMixin)
+        return (
+            (cls,)
+            + ORTModelForSpeechSeq2Seq.__mro__[:top_inheritance_index]
+            + (WhisperForConditionalGeneration,)
+            + ORTModelForSpeechSeq2Seq.__mro__[top_inheritance_index:]
+        )
+
+
+class _ORTModelForWhisper(
+    ORTModelForSpeechSeq2Seq, WhisperForConditionalGeneration, metaclass=MetaClassRemoveParentsAndReorder
+):
+    """
+    Whisper implements its own generate() method.
+    """
+
+    @classmethod
+    def _from_pretrained(
+        cls,
+        model_id: Union[str, Path],
+        config: "PretrainedConfig",
+        **kwargs,
+    ):
+        return super(ORTModelForSpeechSeq2Seq, cls)._from_pretrained(model_id, config, **kwargs)
+
 
 class ORTModelForVision2Seq(ORTModelForConditionalGeneration, GenerationMixin):
     """
     VisionEncoderDecoder Sequence-to-sequence model with a language modeling head for ONNX Runtime inference.
     """
 
     auto_model_class = AutoModelForVision2Seq
     main_input_name = "pixel_values"
 
     def __init__(
         self,
         encoder_session: ort.InferenceSession,
         decoder_session: ort.InferenceSession,
         config: "PretrainedConfig",
+        onnx_paths: List[str],
         decoder_with_past_session: Optional[ort.InferenceSession] = None,
+        use_cache: bool = True,
         use_io_binding: Optional[bool] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
         preprocessors: Optional[List] = None,
         generation_config: Optional[GenerationConfig] = None,
         **kwargs,
     ):
         super().__init__(
             encoder_session,
             decoder_session,
             config,
+            onnx_paths,
             decoder_with_past_session,
+            use_cache,
             use_io_binding,
             model_save_dir,
             preprocessors,
             generation_config,
             **kwargs,
         )
 
@@ -1109,20 +1288,27 @@
         **kwargs,
     ) -> Seq2SeqLMOutput:
         # Encode if needed : first prediction pass
         if encoder_outputs is None:
             encoder_outputs = self.encoder(pixel_values=pixel_values)
 
         # Decode
-        if past_key_values is None or self.decoder_with_past is None:
+        if past_key_values is None or self.use_cache is False:
             decoder_outputs = self.decoder(
                 input_ids=decoder_input_ids,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 labels=labels,
             )
+        elif self.use_merged is True:
+            decoder_outputs = self.decoder(
+                input_ids=decoder_input_ids[:, -1:],
+                encoder_hidden_states=encoder_outputs.last_hidden_state,
+                past_key_values=past_key_values,
+                labels=labels,
+            )
         else:
             decoder_outputs = self.decoder_with_past(
                 input_ids=decoder_input_ids[:, -1:],  # Cut decoder_input_ids if past is used
                 past_key_values=past_key_values,
                 encoder_hidden_states=encoder_outputs.last_hidden_state,
                 labels=labels,
             )
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/optimization.py` & `optimum-1.8.0/optimum/onnxruntime/optimization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.8.0/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/quantization.py` & `optimum-1.8.0/optimum/onnxruntime/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/runs/__init__.py` & `optimum-1.8.0/optimum/onnxruntime/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.8.0/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/runs/utils.py` & `optimum-1.8.0/optimum/onnxruntime/runs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
     ORTModelForQuestionAnswering,
     ORTModelForSequenceClassification,
     ORTModelForTokenClassification,
 )
 
 
 task_ortmodel_map = {
-    "causal-lm": ORTModelForCausalLM,
+    "text-generation": ORTModelForCausalLM,
     "feature-extraction": ORTModelForFeatureExtraction,
     "image-classification": ORTModelForImageClassification,
     "question-answering": ORTModelForQuestionAnswering,
     "text-classification": ORTModelForSequenceClassification,
     "token-classification": ORTModelForTokenClassification,
 }
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/trainer.py` & `optimum-1.8.0/optimum/onnxruntime/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """
 import functools
 import math
 import os
 import shutil
 import sys
 import time
+import types
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 
 # Integrations must be imported before ML frameworks:
 # isort: off
@@ -33,14 +34,15 @@
 )
 
 # isort: on
 
 import numpy as np
 import torch
 import torch.distributed as dist
+from packaging import version
 from torch import nn
 from torch.utils.data import DataLoader, Dataset, RandomSampler
 from torch.utils.data.distributed import DistributedSampler
 from tqdm.auto import tqdm
 from transformers.data.data_collator import DataCollator
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
 from transformers.deepspeed import deepspeed_init, is_deepspeed_zero3_enabled
@@ -80,18 +82,19 @@
     enable_full_determinism,
     find_executable_batch_size,
     get_last_checkpoint,
     has_length,
     set_seed,
     speed_metrics,
 )
-from transformers.utils import logging
+from transformers.utils import is_accelerate_available
 
 from ..exporters import TasksManager
 from ..exporters.onnx import OnnxConfigWithPast, export, export_models, get_decoder_models_for_export
+from ..utils import logging
 from .modeling_decoder import ORTModelForCausalLM
 from .modeling_ort import (
     ORTModel,
     ORTModelForCustomTasks,
     ORTModelForFeatureExtraction,
     ORTModelForImageClassification,
     ORTModelForMaskedLM,
@@ -116,43 +119,76 @@
     from apex import amp
 
 if is_fairscale_available():
     dep_version_check("fairscale")
     from fairscale.nn.data_parallel import ShardedDataParallel as ShardedDDP
     from fairscale.optim import OSS
 
+skip_first_batches = None
+if is_accelerate_available():
+    from accelerate import __version__ as accelerate_version
+
+    if version.parse(accelerate_version) >= version.parse("0.16"):
+        from accelerate import skip_first_batches
+
 if TYPE_CHECKING:
     import optuna
 
 
 logger = logging.get_logger(__name__)
 
 # Name of the files used for checkpointing
 TRAINING_ARGS_NAME = "training_args.bin"
 TRAINER_STATE_NAME = "trainer_state.json"
 OPTIMIZER_NAME = "optimizer.pt"
 SCHEDULER_NAME = "scheduler.pt"
 SCALER_NAME = "scaler.pt"
 
 
+class ModuleWithLoss(nn.Module):
+    def __init__(self, model, args, label_smoother):
+        super().__init__()
+        self._original_model = model
+        self.args = args
+        # Label smoothing
+        self.label_smoother = label_smoother
+
+    def forward(self, inputs: Dict[str, Union[torch.Tensor, Any]], return_outputs):
+        # The compute_model_plus_loss_internal is assigned once the class is instantiated.
+        # It should have same signature as Trainer.compute_loss().
+        # We do this to avoid potential un-synced states if we duplicated compute loss codes .
+        return self.compute_model_plus_loss_internal(self._original_model, inputs, return_outputs)
+
+    @property
+    def module(self):
+        """The original `torch.nn.Module` that this module wraps.
+        This property provides access to methods and properties on the original module."""
+
+        return self._original_model.module
+
+    @property
+    def config(self):
+        return self._original_model.config
+
+
 class ORTFeaturesManager:
     _TASKS_TO_ORTMODELS = {
-        "default": ORTModelForFeatureExtraction,
-        "masked-lm": ORTModelForMaskedLM,
-        "causal-lm": ORTModelForCausalLM,
-        "causal-lm-with-past": ORTModelForCausalLM,
-        "seq2seq-lm": ORTModelForSeq2SeqLM,
-        "seq2seq-lm-with-past": ORTModelForSeq2SeqLM,
-        "sequence-classification": ORTModelForSequenceClassification,
+        "feature-extraction": ORTModelForFeatureExtraction,
+        "fill-mask": ORTModelForMaskedLM,
+        "text-generation": ORTModelForCausalLM,
+        "text-generation-with-past": ORTModelForCausalLM,
+        "text2text-generation": ORTModelForSeq2SeqLM,
+        "text2text-generation-with-past": ORTModelForSeq2SeqLM,
+        "text-classification": ORTModelForSequenceClassification,
         "token-classification": ORTModelForTokenClassification,
         "multiple-choice": ORTModelForMultipleChoice,
         "question-answering": ORTModelForQuestionAnswering,
         "image-classification": ORTModelForImageClassification,
         "semantic-segmentation": ORTModelForSemanticSegmentation,
-        "speech2seq-lm": ORTModelForSpeechSeq2Seq,
+        "automatic-speech-recognition": ORTModelForSpeechSeq2Seq,
     }
 
     SUPPORTED_FEATURES = _TASKS_TO_ORTMODELS.keys()
 
     @staticmethod
     def get_model_class_for_feature(feature: str) -> Type:
         """
@@ -249,15 +285,15 @@
           in `train`)
     """
 
     def __init__(
         self,
         model: Union[PreTrainedModel, nn.Module] = None,
         tokenizer: Optional[PreTrainedTokenizerBase] = None,
-        feature: str = "default",
+        feature: str = "feature-extraction",
         args: ORTTrainingArguments = None,
         data_collator: Optional[DataCollator] = None,
         train_dataset: Optional[Dataset] = None,
         eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
         model_init: Optional[Callable[[], PreTrainedModel]] = None,
         compute_metrics: Optional[Callable[[EvalPrediction], Dict]] = None,
         callbacks: Optional[List[TrainerCallback]] = None,
@@ -275,20 +311,63 @@
             model_init=model_init,
             compute_metrics=compute_metrics,
             callbacks=callbacks,
             optimizers=optimizers,
             preprocess_logits_for_metrics=preprocess_logits_for_metrics,
         )
 
+        # We leverage both training_model and inference_model in conjunction with model.
+        # _training_model will be wrapped so it will use ORT and will use the overriden functions in ModuleWithLoss.
+        # _training_model will be storing the default version of the model and will unwrap it in case of eval/test.
+
+        # Only Wrap the model if we pass --use_module_with_loss flag.
+        if args.use_module_with_loss:
+            self._training_model = self.create_model_with_loss()
+
+        self.model = model
+
         self.feature = feature
         self.onnx_model_path = onnx_model_path
         self.exported_with_loss = False
         if self.args.local_rank:
             torch.cuda.set_device(self.args.local_rank)
 
+    # this method will create a ModuleWithLoss Instance to use if you are passing --use_module_with_loss flag.
+    # It will help reducing the peak memory usage by computing loss inside training.
+    def create_model_with_loss(self):
+        model_with_loss = ModuleWithLoss(self.model, self.args, self.label_smoother)
+        model_with_loss.compute_model_plus_loss_internal = types.MethodType(Trainer.compute_loss, model_with_loss)
+
+        return model_with_loss
+
+    # we assume that training_model and inference_model have the same forward signature column.
+    # self._signature_columns attribute only stores the first-time parsed signature
+    def _set_signature_columns_if_needed(self):
+        if self._signature_columns is None:
+            # Inspect model forward signature to keep only the arguments it accepts.
+            import inspect
+
+            if isinstance(self.model, ModuleWithLoss):
+                signature = inspect.signature(self.model._original_model.forward)
+            else:
+                signature = inspect.signature(self.model.forward)
+
+            self._signature_columns = list(signature.parameters.keys())
+            # Labels may be named label or label_ids, the default data collator handles that.
+            self._signature_columns += list(set(["label", "label_ids"] + self.label_names))
+
+    def compute_loss(self, model_with_loss, inputs, return_outputs=False):
+        # Run model forward + loss compute.
+        if isinstance(self.model, ModuleWithLoss):
+            # ORTModule Does not support the BatchEncoding Type so we have to convert to a dict.
+            dict_inputs = dict(inputs.items())
+            return model_with_loss(dict_inputs, return_outputs)
+        else:
+            return super().compute_loss(model_with_loss, inputs, return_outputs)
+
     def train(
         self,
         resume_from_checkpoint: Optional[Union[str, bool]] = None,
         trial: Union["optuna.Trial", Dict[str, Any]] = None,
         ignore_keys_for_eval: Optional[List[str]] = None,
         **kwargs,
     ):
@@ -309,14 +388,16 @@
                 Additional keyword arguments used to hide deprecated arguments
         """
         if not is_onnxruntime_training_available():
             raise ImportError(
                 "You need to install `onnxruntime-training` to use `ORTTrainer` for training. Check out "
                 "https://huggingface.co/docs/optimum/onnxruntime/usage_guides/trainer#install-onnx-runtime."
             )
+        if self.args.use_module_with_loss:
+            self.model = self._training_model
 
         if resume_from_checkpoint is False:
             resume_from_checkpoint = None
 
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
 
@@ -354,15 +435,15 @@
 
         # Load potential model checkpoint
         if isinstance(resume_from_checkpoint, bool) and resume_from_checkpoint:
             resume_from_checkpoint = get_last_checkpoint(args.output_dir)
             if resume_from_checkpoint is None:
                 raise ValueError(f"No valid checkpoint found in output directory ({args.output_dir})")
 
-        if resume_from_checkpoint is not None and not is_sagemaker_mp_enabled():
+        if resume_from_checkpoint is not None and not is_sagemaker_mp_enabled() and args.deepspeed is None:
             self._load_from_checkpoint(resume_from_checkpoint)
 
         # If model was re-initialized, put it on the right device and update self.model_wrapped
         if model_reloaded:
             if self.place_model_on_device:
                 self._move_model_to_device(self.model, args.device)
             self.model_wrapped = self.model
@@ -534,20 +615,28 @@
             else:
                 steps_trained_in_current_epoch = 0
 
             logger.info("  Continuing training from checkpoint, will skip to saved global_step")
             logger.info(f"  Continuing training from epoch {epochs_trained}")
             logger.info(f"  Continuing training from global step {self.state.global_step}")
             if not args.ignore_data_skip:
-                logger.info(
-                    f"  Will skip the first {epochs_trained} epochs then the first {steps_trained_in_current_epoch} "
-                    "batches in the first epoch. If this takes a lot of time, you can add the `--ignore_data_skip` "
-                    "flag to your launch command, but you will resume the training on data already seen by your model."
-                )
-                if self.is_local_process_zero() and not args.disable_tqdm:
+                if skip_first_batches is None:
+                    logger.info(
+                        f"  Will skip the first {epochs_trained} epochs then the first"
+                        f" {steps_trained_in_current_epoch} batches in the first epoch. If this takes a lot of time,"
+                        " you can install the latest version of Accelerate with `pip install -U accelerate`.You can"
+                        " also add the `--ignore_data_skip` flag to your launch command, but you will resume the"
+                        " training on data already seen by your model."
+                    )
+                else:
+                    logger.info(
+                        f"  Will skip the first {epochs_trained} epochs then the first"
+                        f" {steps_trained_in_current_epoch} batches in the first epoch."
+                    )
+                if self.is_local_process_zero() and not args.disable_tqdm and skip_first_batches is None:
                     steps_trained_progress_bar = tqdm(total=steps_trained_in_current_epoch)
                     steps_trained_progress_bar.set_description("Skipping the first batches")
 
         # Update the references
         self.callback_handler.model = self.model
         self.callback_handler.optimizer = self.optimizer
         self.callback_handler.lr_scheduler = self.lr_scheduler
@@ -589,36 +678,52 @@
                     for _ in train_dataloader:
                         break
                 else:
                     # Otherwise we need to call the whooooole sampler cause there is some random operation added
                     # AT THE VERY END!
                     _ = list(train_dataloader.sampler)
 
+        total_batched_samples = 0
         for epoch in range(epochs_trained, num_train_epochs):
             if isinstance(train_dataloader, DataLoader) and isinstance(train_dataloader.sampler, DistributedSampler):
                 train_dataloader.sampler.set_epoch(epoch)
             elif hasattr(train_dataloader, "dataset") and isinstance(train_dataloader.dataset, IterableDatasetShard):
                 train_dataloader.dataset.set_epoch(epoch)
 
+            epoch_iterator = train_dataloader
+
             # Reset the past mems state at the beginning of each epoch if necessary.
             if args.past_index >= 0:
                 self._past = None
 
             steps_in_epoch = (
                 len(train_dataloader)
                 if len_dataloader is not None
                 else args.max_steps * args.gradient_accumulation_steps
             )
             self.control = self.callback_handler.on_epoch_begin(args, self.state, self.control)
 
             if epoch == epochs_trained and resume_from_checkpoint is not None and steps_trained_in_current_epoch == 0:
                 self._load_rng_state(resume_from_checkpoint)
 
+            rng_to_sync = False
+            steps_skipped = 0
+            if skip_first_batches is not None and steps_trained_in_current_epoch > 0:
+                skip_first_batches(epoch_iterator, steps_trained_in_current_epoch)
+                steps_skipped = steps_trained_in_current_epoch
+                steps_trained_in_current_epoch = 0
+                rng_to_sync = True
+
             step = -1
             for step, inputs in enumerate(train_dataloader):
+                total_batched_samples += 1
+                if rng_to_sync:
+                    self._load_rng_state(resume_from_checkpoint)
+                    rng_to_sync = False
+
                 # Skip past any already trained steps if resuming training
                 if steps_trained_in_current_epoch > 0:
                     steps_trained_in_current_epoch -= 1
                     if steps_trained_progress_bar is not None:
                         steps_trained_progress_bar.update(1)
                     if steps_trained_in_current_epoch == 0:
                         self._load_rng_state(resume_from_checkpoint)
@@ -627,15 +732,15 @@
                     steps_trained_progress_bar.close()
                     steps_trained_progress_bar = None
 
                 if step % args.gradient_accumulation_steps == 0:
                     self.control = self.callback_handler.on_step_begin(args, self.state, self.control)
 
                 if (
-                    ((step + 1) % args.gradient_accumulation_steps != 0)
+                    (total_batched_samples % args.gradient_accumulation_steps != 0)
                     and args.local_rank != -1
                     and args._no_sync_in_gradient_accumulation
                 ):
                     # Avoid unnecessary DDP synchronization since there will be no backward pass on this example.
                     with model.no_sync():
                         tr_loss_step = self.training_step(model, inputs)
                 else:
@@ -653,15 +758,15 @@
 
                 self.current_flos += float(self.floating_point_ops(inputs))
 
                 # Optimizer step for deepspeed must be called on every step regardless of the value of gradient_accumulation_steps
                 if self.deepspeed:
                     self.deepspeed.step()
 
-                if (step + 1) % args.gradient_accumulation_steps == 0 or (
+                if total_batched_samples % args.gradient_accumulation_steps == 0 or (
                     # last step in epoch but step is always smaller than gradient_accumulation_steps
                     steps_in_epoch <= args.gradient_accumulation_steps
                     and (step + 1) == steps_in_epoch
                 ):
                     # Gradient clipping
                     if args.max_grad_norm is not None and args.max_grad_norm > 0 and not self.deepspeed:
                         # deepspeed does its own clipping
@@ -701,15 +806,15 @@
                         self.optimizer.step()
 
                     if optimizer_was_run and not self.deepspeed:
                         self.lr_scheduler.step()
 
                     model.zero_grad()
                     self.state.global_step += 1
-                    self.state.epoch = epoch + (step + 1) / steps_in_epoch
+                    self.state.epoch = epoch + (step + 1 + steps_skipped) / steps_in_epoch
                     self.control = self.callback_handler.on_step_end(args, self.state, self.control)
 
                     self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
                 else:
                     self.control = self.callback_handler.on_substep_end(args, self.state, self.control)
 
                 if self.control.should_epoch_stop or self.control.should_training_stop:
@@ -797,14 +902,16 @@
                 "eval_bleu" if the prefix is "eval" (default)
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
         # memory metrics - must set up as early as possible
+        # TODO: We need to enable evaluation using ORT backend.
+        self.model = unwrap_model(self.model)
         self._memory_tracker.start()
 
         eval_dataloader = self.get_eval_dataloader(eval_dataset)
         start_time = time.time()
 
         if inference_with_ort:
             logger.info("[INFO] Evaluating with ONNX Runtime backend.")
@@ -888,14 +995,17 @@
         Returns: *NamedTuple* A namedtuple with the following keys:
 
             - predictions (`np.ndarray`): The predictions on `test_dataset`.
             - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
             - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
               labels).
         """
+        # TODO: We need to enable evaluation using ORT backend.
+        self.model = unwrap_model(self.model)
+
         # memory metrics - must set up as early as possible
         self._memory_tracker.start()
 
         test_dataloader = self.get_test_dataloader(test_dataset)
         start_time = time.time()
 
         if inference_with_ort:
@@ -905,18 +1015,15 @@
             logger.info(
                 "[INFO] Predicting with PyTorch backend. If you want to use ONNX Runtime for the prediction, set `trainer.predict(inference_with_ort=True)`."
             )
             eval_loop = self.prediction_loop if self.args.use_legacy_prediction_loop else self.evaluation_loop
 
         try:
             output = eval_loop(
-                test_dataloader,
-                description="Prediction",
-                ignore_keys=ignore_keys,
-                metric_key_prefix=metric_key_prefix,
+                test_dataloader, description="Prediction", ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix
             )
         except Exception as error:
             logger.error(error)
             if inference_with_ort:
                 logger.error(
                     f"[ERROR!] Prediction with ONNX Runtime is not available for {self.model.config.name_or_path} model. Set `inference_with_ort=False` to predict with PyTorch."
                 )
@@ -972,22 +1079,22 @@
 
             # With `label_smoother` the loss will be computed outside modeling
             with_loss = has_labels and not self.label_smoother
             self._export(onnx_model_path, with_loss=with_loss, device=export_device, use_cache=use_cache)
 
             self.exported_with_loss = with_loss
             self.onnx_model_path = onnx_model_path.as_posix()
-            logger.info("[INFO] ONNX model is stored in:\n", self.onnx_model_path)
+            logger.info(f"[INFO] ONNX model is stored in: {self.onnx_model_path}")
 
         # Load ORT model
         support_loss_in_modeling = self.feature in [
-            "causal-lm",
-            "causal-lm-with-past",
-            "seq2seq-lm",
-            "seq2seq-lm-with-past",
+            "text-generation",
+            "text-generation-with-past",
+            "text2text-generation",
+            "text2text-generation-with-past",
         ]
         support_feature = self.feature in ORTFeaturesManager.SUPPORTED_FEATURES
         if support_loss_in_modeling or (not self.exported_with_loss and support_feature):
             # Exported with standard outputs, use specific ORTModels
             ort_model_cls = ORTFeaturesManager.get_model_class_for_feature(self.feature)
         else:
             ort_model_cls = ORTModelForCustomTasks
@@ -1207,18 +1314,18 @@
 
             self.exported_with_loss = with_loss
             self.onnx_model_path = onnx_model_path.as_posix()
             logger.info("[INFO] ONNX model is stored in:\n", self.onnx_model_path)
 
         # Load ORT model
         support_loss_in_modeling = self.feature in [
-            "causal-lm",
-            "causal-lm-with-past",
-            "seq2seq-lm",
-            "seq2seq-lm-with-past",
+            "text-generation",
+            "text-generation-with-past",
+            "text2text-generation",
+            "text2text-generation-with-past",
         ]
         support_feature = self.feature in ORTFeaturesManager.SUPPORTED_FEATURES
         if support_loss_in_modeling or (not self.exported_with_loss and support_feature):
             # Exported with standard outputs, use specific ORTModels
             ort_model_cls = ORTFeaturesManager.get_model_class_for_feature(self.feature)
         else:
             ort_model_cls = ORTModelForCustomTasks
@@ -1436,15 +1543,15 @@
         outputs = model(**inputs)
         # Save past state if it exists
         # TODO: this needs to be fixed and made cleaner later.
         if self.args.past_index >= 0:
             self._past = outputs[self.args.past_index]
 
         if labels is not None:
-            if "causal-lm" in self.feature:
+            if "text-generation" in self.feature:
                 loss = self.label_smoother(outputs, labels, shift_labels=True)
             else:
                 loss = self.label_smoother(outputs, labels)
         else:
             if isinstance(outputs, dict) and "loss" not in outputs:
                 raise ValueError(
                     "The model did not return a loss from the inputs, only the following keys: "
@@ -1518,21 +1625,15 @@
             )
         else:
             if with_loss is True:
                 onnx_config = wrap_onnx_config_for_loss(onnx_config)
                 opset = max(opset, 12)  # Operators like `nll_loss`are added for opset>=12
 
             output_path = model_path / ONNX_WEIGHTS_NAME
-            _ = export(
-                model=model,
-                config=onnx_config,
-                opset=opset,
-                output=output_path,
-                device=device,
-            )
+            _ = export(model=model, config=onnx_config, opset=opset, output=output_path, device=device)
 
         model.config.save_pretrained(model_path)
 
     def _wrap_model(self, model, training=True, dataloader=None):
         # TODO: torchdynamo works for inference with PyTorch in ORTTrainer, will move `inference_with_ort` to training arguments and
         # whether be able to use ipex will depend on both `self.args.torchdynamo` and `self.args.ort_mode_eval`.
         if self.args.torchdynamo is not None:
@@ -1693,19 +1794,15 @@
 
             if self.args.optim in ORTOptimizerNames:
                 optimizer_cls, optimizer_kwargs = ORTTrainer.get_ort_optimizer_cls_and_kwargs(self.args)
             else:
                 optimizer_cls, optimizer_kwargs = Trainer.get_optimizer_cls_and_kwargs(self.args)
 
             if self.sharded_ddp == ShardedDDPOption.SIMPLE:
-                self.optimizer = OSS(
-                    params=optimizer_grouped_parameters,
-                    optim=optimizer_cls,
-                    **optimizer_kwargs,
-                )
+                self.optimizer = OSS(params=optimizer_grouped_parameters, optim=optimizer_cls, **optimizer_kwargs)
             else:
                 self.optimizer = optimizer_cls(optimizer_grouped_parameters, **optimizer_kwargs)
                 if optimizer_cls.__name__ == "Adam8bit":
                     import bitsandbytes
 
                     manager = bitsandbytes.optim.GlobalOptimManager.get_instance()
 
@@ -1727,18 +1824,15 @@
         Returns the optimizer class and optimizer parameters implemented in ONNX Runtime based on `ORTTrainingArguments`.
 
         Args:
             args (`ORTTrainingArguments`):
                 The training arguments for the training session.
         """
         optimizer_kwargs = {"lr": args.learning_rate}
-        adam_kwargs = {
-            "betas": (args.adam_beta1, args.adam_beta2),
-            "eps": args.adam_epsilon,
-        }
+        adam_kwargs = {"betas": (args.adam_beta1, args.adam_beta2), "eps": args.adam_epsilon}
         if args.optim == ORTOptimizerNames.ADAMW_ORT_FUSED:
             try:
                 from onnxruntime.training.optim import FusedAdam
 
                 optimizer_cls = FusedAdam
                 optimizer_kwargs.update(adam_kwargs)
             except ImportError:
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.8.0/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,34 +561,24 @@
             gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.model.config.num_beams
         )
         default_synced_gpus = True if is_deepspeed_zero3_enabled() else False
         gen_kwargs["synced_gpus"] = (
             gen_kwargs["synced_gpus"] if gen_kwargs.get("synced_gpus") is not None else default_synced_gpus
         )
 
-        if "attention_mask" in inputs:
-            gen_kwargs["attention_mask"] = inputs.get("attention_mask", None)
-        if "global_attention_mask" in inputs:
-            gen_kwargs["global_attention_mask"] = inputs.get("global_attention_mask", None)
+        # TODO (Joao): the following line is needed to keep a consistent result on SQUAD. Ideally, we should not block
+        # users from preparing a dataset with `decoder_input_ids`.
+        inputs = {k: v for k, v in inputs.items() if k != "decoder_input_ids"}
+        generated_tokens = self.model.generate(**inputs, **gen_kwargs)
 
-        # prepare generation inputs
-        # some encoder-decoder models can have varying encoder's and thus
-        # varying model input names
-        if hasattr(self.model, "encoder") and self.model.encoder.main_input_name != self.model.main_input_name:
-            generation_inputs = inputs[self.model.encoder.main_input_name]
-        else:
-            generation_inputs = inputs[self.model.main_input_name]
-
-        if torch.cuda.is_available():
-            self.model.to("cuda")
-
-        generated_tokens = self.model.generate(
-            generation_inputs,
-            **gen_kwargs,
-        )
+        # Temporary hack to ensure the generation config is not initialized for each iteration of the evaluation loop
+        # TODO: remove this hack when the legacy code that initializes generation_config from a model config is
+        # removed in https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/generation/utils.py#L1183
+        if self.model.generation_config._from_model_config:
+            self.model.generation_config._from_model_config = False
         # in case the batch is shorter than max length, the output should be padded
         if gen_kwargs.get("max_length") is not None and generated_tokens.shape[-1] < gen_kwargs["max_length"]:
             generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_length"])
         elif gen_kwargs.get("max_new_tokens") is not None and generated_tokens.shape[-1] < (
             gen_kwargs["max_new_tokens"] + 1
         ):
             generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_new_tokens"] + 1)
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/training_args.py` & `optimum-1.8.0/optimum/onnxruntime/training_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,21 @@
 class ORTTrainingArguments(TrainingArguments):
     """
     Parameters:
         optim (`str` or [`training_args.ORTOptimizerNames`] or [`transformers.training_args.OptimizerNames`], *optional*, defaults to `"adamw_hf"`):
             The optimizer to use, including optimizers in Transformers: adamw_hf, adamw_torch, adamw_apex_fused, or adafactor. And optimizers implemented by ONNX Runtime: adamw_ort_fused.
     """
 
-    optim: Optional[str] = field(
-        default="adamw_hf",
-        metadata={"help": "The optimizer to use."},
+    optim: Optional[str] = field(default="adamw_hf", metadata={"help": "The optimizer to use."})
+
+    use_module_with_loss: Optional[bool] = field(
+        default=False,
+        metadata={
+            "help": "Use ModuleWithLoss Wrapper to compute loss inside the training loop, having this will help save memory for ORTModule Runs."
+        },
     )
 
     # This method will not need to be overriden after the deprecation of `--adafactor` in version 5 of 🤗 Transformers.
     def __post_init__(self):
         # Handle --use_env option in torch.distributed.launch (local_rank not passed as an arg then).
         # This needs to happen before any call to self.device or self.n_gpu.
         env_local_rank = int(os.environ.get("LOCAL_RANK", -1))
@@ -332,7 +336,14 @@
             self.hub_model_id = f"{self.push_to_hub_organization}/{Path(self.output_dir).name}"
             warnings.warn(
                 "`--push_to_hub_organization` is deprecated and will be removed in version 5 of 🤗 Transformers. Use "
                 "`--hub_model_id` instead and pass the full repo name to this argument (in this case "
                 f"{self.hub_model_id}).",
                 FutureWarning,
             )
+        if self.use_module_with_loss is True:
+            logger.info(
+                "Using ModuleWithLoss Wrapper."
+                "loss will be computed during training loop and it will save memory peak "
+            )
+        else:
+            logger.info("Not Using ModuleWithLoss Wrapper.")
```

### Comparing `optimum-1.7.3/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.8.0/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/onnxruntime/utils.py` & `optimum-1.8.0/optimum/onnxruntime/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         "electra": "bert",
         "gpt2": "gpt2",
         "gpt_neo": "gpt2",
         "gpt_neox": "gpt2",
         "gptj": "gpt2",
         # longt5 with O4 results in segmentation fault
         "longt5": "bert",
+        "llama": "gpt2",
         "marian": "bart",
         "mbart": "bart",
         "mt5": "bart",
         "m2m_100": "bart",
         "nystromformer": "bert",
         "pegasus": "bert",
         "roberta": "bert",
@@ -244,15 +245,15 @@
         )
 
 
 def check_io_binding(providers: List[str], use_io_binding: Optional[bool] = None) -> bool:
     """
     Whether to use IOBinding or not.
     """
-    if providers[0] == "CUDAExecutionProvider" and use_io_binding is None:
+    if use_io_binding is None and providers[0] == "CUDAExecutionProvider":
         use_io_binding = True
     elif providers[0] != "CUDAExecutionProvider":
         if use_io_binding is True:
             logger.warning(
                 "No need to enable IO Binding if the provider used is not CUDAExecutionProvider. IO Binding will be turned off."
             )
         use_io_binding = False
```

### Comparing `optimum-1.7.3/optimum/pipelines/__init__.py` & `optimum-1.8.0/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.8.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.8.0/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/pipelines/pipelines_base.py` & `optimum-1.8.0/optimum/pipelines/pipelines_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/quantization_base.py` & `optimum-1.8.0/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/runs_base.py` & `optimum-1.8.0/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/__init__.py` & `optimum-1.8.0/optimum/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ORT_QUANTIZE_MINIMUM_VERSION,
     TORCH_MINIMUM_VERSION,
     check_if_diffusers_greater,
     check_if_pytorch_greater,
     check_if_transformers_greater,
     is_accelerate_available,
     is_diffusers_available,
+    is_onnx_available,
     is_onnxruntime_available,
     is_pydantic_available,
     is_torch_onnx_support_available,
     require_numpy_strictly_lower,
     torch_version,
 )
 from .input_generators import (
```

### Comparing `optimum-1.7.3/optimum/utils/constant.py` & `optimum-1.8.0/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/doc.py` & `optimum-1.8.0/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.8.0/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/file_utils.py` & `optimum-1.8.0/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/import_utils.py` & `optimum-1.8.0/optimum/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/input_generators.py` & `optimum-1.8.0/optimum/utils/input_generators.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/logging.py` & `optimum-1.8.0/optimum/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,30 @@
 # limitations under the License.
 """ Logging utilities. """
 
 import logging
 import os
 import sys
 import threading
+from functools import lru_cache
 from logging import (
     CRITICAL,  # NOQA
     DEBUG,  # NOQA
     ERROR,  # NOQA
     FATAL,  # NOQA
     INFO,  # NOQA
     NOTSET,  # NOQA
     WARN,  # NOQA
     WARNING,  # NOQA
 )
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
+
+
+if TYPE_CHECKING:
+    from logging import Logger
 
 
 _lock = threading.Lock()
 _default_handler: Optional[logging.Handler] = None
 
 log_levels = {
     "debug": logging.DEBUG,
@@ -258,7 +263,12 @@
 
     All handlers currently bound to the root logger are affected by this method.
     """
     handlers = _get_library_root_logger().handlers
 
     for handler in handlers:
         handler.setFormatter(None)
+
+
+@lru_cache(None)
+def warn_once(logger: "Logger", msg: str):
+    logger.warning(msg)
```

### Comparing `optimum-1.7.3/optimum/utils/modeling_utils.py` & `optimum-1.8.0/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/normalized_config.py` & `optimum-1.8.0/optimum/utils/normalized_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
         "deit": NormalizedVisionConfig,
         "distilbert": NormalizedTextConfig.with_args(num_attention_heads="n_heads", hidden_size="dim"),
         "donut-swin": NormalizedVisionConfig,
         "electra": NormalizedTextConfig,
         "gpt2": GPT2LikeNormalizedTextConfig,
         "gpt_neo": NormalizedTextConfig.with_args(num_attention_heads="num_heads"),
         "gpt_neox": NormalizedTextConfig,
+        "llama": NormalizedTextConfig,
         "gptj": GPT2LikeNormalizedTextConfig,
         "imagegpt": GPT2LikeNormalizedTextConfig,
         "longt5": T5LikeNormalizedTextConfig,
         "marian": BartLikeNormalizedTextConfig,
         "mbart": BartLikeNormalizedTextConfig,
         "mt5": T5LikeNormalizedTextConfig,
         "m2m_100": BartLikeNormalizedTextConfig,
```

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/__init__.py` & `optimum-1.8.0/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/base.py` & `optimum-1.8.0/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/image_classification.py` & `optimum-1.8.0/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/question_answering.py` & `optimum-1.8.0/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.8.0/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from .base import DatasetProcessing
 
 
 class TaskProcessorsManager:
     _TASK_TO_DATASET_PROCESSING_CLASS = {
-        "sequence-classification": TextClassificationProcessing,
+        "text-classification": TextClassificationProcessing,
         "token-classification": TokenClassificationProcessing,
         "question-answering": QuestionAnsweringProcessing,
         "image-classification": ImageClassificationProcessing,
     }
 
     @classmethod
     def get_task_processor_class_for_task(cls, task: str) -> Type:
```

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/text_classification.py` & `optimum-1.8.0/optimum/utils/preprocessing/text_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 secondary_key_name = name
                 break
 
         if primary_key_name is None:
             return None
         elif secondary_key_name is None:
             logger.info(
-                "Could not infer the secondary key in the dataset, if it does contain one, please provided it manually."
+                "Could not infer the secondary key in the dataset, if it does contain one, please provide it manually."
             )
             return {"primary": primary_key_name}
         else:
             return {"primary": primary_key_name, "secondary": secondary_key_name}
 
     def try_to_guess_ref_keys(self, column_names: List[str]) -> Optional[List[str]]:
         for name in column_names:
```

### Comparing `optimum-1.7.3/optimum/utils/preprocessing/token_classification.py` & `optimum-1.8.0/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/runs.py` & `optimum-1.8.0/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/save_utils.py` & `optimum-1.8.0/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/optimum/utils/testing_utils.py` & `optimum-1.8.0/optimum/utils/testing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,37 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-import collections
 import importlib.util
 import itertools
 import os
 import subprocess
 import sys
 import unittest
+from collections.abc import MutableMapping
 from typing import Any, Callable, Dict, Iterable, Optional, Tuple
 
 import torch
 from packaging.version import parse
 
 from . import is_accelerate_available, is_diffusers_available
 
 
+# Used to test the hub
+USER = "__DUMMY_OPTIMUM_USER__"
+
+# Not critical, only usable on the sandboxed CI instance.
+TOKEN = "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"
+
+
 def flatten_dict(dictionary: Dict):
     """
     Flatten a nested dictionaries as a flat dictionary.
     """
     items = []
     for k, v in dictionary.items():
         new_key = k
-        if isinstance(v, collections.MutableMapping):
+        if isinstance(v, MutableMapping):
             items.extend(flatten_dict(v).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 
 def require_accelerate(test_case):
```

### Comparing `optimum-1.7.3/optimum/version.py` & `optimum-1.8.0/optimum/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.7.3"
+__version__ = "1.8.0"
```

### Comparing `optimum-1.7.3/optimum.egg-info/SOURCES.txt` & `optimum-1.8.0/optimum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,32 @@
 optimum.egg-info/entry_points.txt
 optimum.egg-info/not-zip-safe
 optimum.egg-info/requires.txt
 optimum.egg-info/top_level.txt
 optimum/bettertransformer/__init__.py
 optimum/bettertransformer/transformation.py
 optimum/bettertransformer/models/__init__.py
+optimum/bettertransformer/models/attention.py
 optimum/bettertransformer/models/base.py
 optimum/bettertransformer/models/decoder_models.py
 optimum/bettertransformer/models/encoder_models.py
 optimum/commands/__init__.py
+optimum/commands/base.py
 optimum/commands/env.py
 optimum/commands/optimum_cli.py
 optimum/commands/export/__init__.py
+optimum/commands/export/base.py
 optimum/commands/export/ggml.py
 optimum/commands/export/onnx.py
 optimum/commands/export/tflite.py
 optimum/commands/onnxruntime/__init__.py
+optimum/commands/onnxruntime/base.py
 optimum/commands/onnxruntime/optimize.py
 optimum/commands/onnxruntime/quantize.py
+optimum/commands/register/__init__.py
 optimum/exporters/__init__.py
 optimum/exporters/base.py
 optimum/exporters/error_utils.py
 optimum/exporters/tasks.py
 optimum/exporters/onnx/__init__.py
 optimum/exporters/onnx/__main__.py
 optimum/exporters/onnx/base.py
@@ -63,14 +68,15 @@
 optimum/onnx/graph_transformations.py
 optimum/onnx/modeling_seq2seq.py
 optimum/onnx/transformations_utils.py
 optimum/onnx/utils.py
 optimum/onnxruntime/__init__.py
 optimum/onnxruntime/base.py
 optimum/onnxruntime/configuration.py
+optimum/onnxruntime/constants.py
 optimum/onnxruntime/graph.py
 optimum/onnxruntime/model.py
 optimum/onnxruntime/modeling_decoder.py
 optimum/onnxruntime/modeling_diffusion.py
 optimum/onnxruntime/modeling_ort.py
 optimum/onnxruntime/modeling_seq2seq.py
 optimum/onnxruntime/optimization.py
```

### Comparing `optimum-1.7.3/optimum.egg-info/requires.txt` & `optimum-1.8.0/optimum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/pyproject.toml` & `optimum-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/setup.py` & `optimum-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/tests/test_configuration_utils.py` & `optimum-1.8.0/tests/test_configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.7.3/tests/test_modeling_base.py` & `optimum-1.8.0/tests/test_modeling_base.py`

 * *Files identical despite different names*

