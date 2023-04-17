# Comparing `tmp/optimum-1.8.0.tar.gz` & `tmp/optimum-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.8.0.tar", last modified: Mon Apr 17 09:30:52 2023, max compression
+gzip compressed data, was "optimum-1.8.1.tar", last modified: Mon Apr 17 12:34:09 2023, max compression
```

## Comparing `optimum-1.8.0.tar` & `optimum-1.8.1.tar`

### file list

```diff
@@ -1,153 +1,150 @@
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.8.0/LICENSE
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.8.0/MANIFEST.in
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 09:30:52.402770 optimum-1.8.0/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9876 2023-04-17 07:37:27.000000 optimum-1.8.0/README.md
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/bettertransformer/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/bettertransformer/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/bettertransformer/models/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8420 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    21474 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/models/attention.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8092 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12222 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/models/decoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60023 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/bettertransformer/models/encoder_models.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17127 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/bettertransformer/transformation.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum/commands/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      952 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5872 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2475 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/env.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/export/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      716 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1340 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/commands/export/ggml.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8554 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/export/onnx.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9016 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/commands/export/tflite.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      759 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1374 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3885 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/optimize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4011 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/onnxruntime/quantize.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6871 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/optimum_cli.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/commands/register/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      621 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/commands/register/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/conftest.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      903 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/error_utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17290 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    44198 2023-04-17 09:04:07.000000 optimum-1.8.0/optimum/exporters/onnx/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16221 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      865 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/onnx/constants.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31628 2023-04-12 09:59:52.000000 optimum-1.8.0/optimum/exporters/onnx/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    37124 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/exporters/onnx/model_configs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7326 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/exporters/onnx/model_patcher.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9646 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/onnx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    59776 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/exporters/tasks.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/exporters/tflite/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5256 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/__main__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15507 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/tflite/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/config.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16963 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/exporters/tflite/convert.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/exporters/tflite/model_configs.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/optimization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/optimization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/optimization/transformations.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/fx/quantization/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/quantization/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/quantization/functions.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/fx/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15117 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/modeling_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnx/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11198 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnx/graph_transformations.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13025 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnx/transformations_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/onnx/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32544 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45434 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/configuration.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      901 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/constants.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/graph.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/io_binding/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/io_binding/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/model.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    30965 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/onnxruntime/modeling_decoder.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/modeling_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    83591 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/modeling_ort.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    58316 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/modeling_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15083 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/optimization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/preprocessors/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/preprocessors/quantization.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23448 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/quantization.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/onnxruntime/runs/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8001 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/runs/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/runs/calibrator.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      625 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/runs/utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    88945 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/onnxruntime/trainer.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38387 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/trainer_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17122 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/onnxruntime/training_args.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/onnxruntime/training_args_seq2seq.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11746 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/onnxruntime/utils.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/pipelines/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/__init__.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/pipelines/diffusers/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/diffusers/pipeline_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13522 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/pipelines/pipelines_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/quantization_base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-04-11 18:28:51.000000 optimum-1.8.0/optimum/runs_base.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/utils/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1989 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/constant.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/doc.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/dummy_diffusers_objects.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/file_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6181 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/import_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23612 2023-04-13 16:43:16.000000 optimum-1.8.0/optimum/utils/input_generators.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7836 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/logging.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/modeling_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9323 2023-04-17 09:03:56.000000 optimum-1.8.0/optimum/utils/normalized_config.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/optimum/utils/preprocessing/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/__init__.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/base.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/image_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/question_answering.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2169 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/utils/preprocessing/task_processors_manager.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4436 2023-04-17 08:20:06.000000 optimum-1.8.0/optimum/utils/preprocessing/text_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/preprocessing/token_classification.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/runs.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-04-11 18:28:52.000000 optimum-1.8.0/optimum/utils/save_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5762 2023-04-17 07:37:27.000000 optimum-1.8.0/optimum/utils/testing_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-04-17 09:04:28.000000 optimum-1.8.0/optimum/version.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.398770 optimum-1.8.0/optimum.egg-info/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/PKG-INFO
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4365 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/SOURCES.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/dependency_links.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/entry_points.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-03-02 08:10:42.000000 optimum-1.8.0/optimum.egg-info/not-zip-safe
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      973 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/requires.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-04-17 09:30:52.000000 optimum-1.8.0/optimum.egg-info/top_level.txt
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.8.0/pyproject.toml
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-04-17 09:30:52.402770 optimum-1.8.0/setup.cfg
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3429 2023-04-11 18:28:51.000000 optimum-1.8.0/setup.py
-drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 09:30:52.402770 optimum-1.8.0/tests/
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3432 2023-04-11 18:28:52.000000 optimum-1.8.0/tests/test_configuration_utils.py
--rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1936 2023-04-11 18:28:52.000000 optimum-1.8.0/tests/test_modeling_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11357 2022-04-11 08:30:37.000000 optimum-1.8.1/LICENSE
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      651 2022-04-11 08:30:37.000000 optimum-1.8.1/MANIFEST.in
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 12:34:09.575548 optimum-1.8.1/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9876 2023-04-17 07:37:27.000000 optimum-1.8.1/README.md
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/bettertransformer/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/bettertransformer/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/bettertransformer/models/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8420 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/bettertransformer/models/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    21474 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/bettertransformer/models/attention.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8092 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/bettertransformer/models/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    12222 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/bettertransformer/models/decoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60023 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/bettertransformer/models/encoder_models.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17127 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/bettertransformer/transformation.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/commands/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      952 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5872 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2475 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/env.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/commands/export/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      716 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/export/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1340 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/export/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      998 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/commands/export/ggml.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8554 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/export/onnx.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9016 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/commands/export/tflite.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/commands/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      759 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1374 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3885 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/onnxruntime/optimize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4011 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/onnxruntime/quantize.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6871 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/optimum_cli.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/commands/register/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      621 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/commands/register/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17957 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/configuration_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1454 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/conftest.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/exporters/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      688 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      707 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      903 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/error_utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/exporters/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1918 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17290 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/onnx/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    44198 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/onnx/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16221 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/onnx/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      865 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/onnx/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    31628 2023-04-12 09:59:52.000000 optimum-1.8.1/optimum/exporters/onnx/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    37124 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/onnx/model_configs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7326 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/exporters/onnx/model_patcher.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9646 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/onnx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    60524 2023-04-17 11:22:41.000000 optimum-1.8.1/optimum/exporters/tasks.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/exporters/tflite/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1209 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/tflite/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5256 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/tflite/__main__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15507 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/tflite/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1397 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/tflite/config.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    16963 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/exporters/tflite/convert.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3588 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/exporters/tflite/model_configs.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/fx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      672 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/fx/optimization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      866 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/optimization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32725 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/optimization/transformations.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum/fx/quantization/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/quantization/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13591 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/quantization/functions.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1450 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/fx/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15117 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/modeling_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnx/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1276 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/onnx/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3830 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/onnx/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11198 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/onnx/graph_transformations.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4316 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/onnx/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13025 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/onnx/transformations_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3307 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/onnx/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnxruntime/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4279 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    32544 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/onnxruntime/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    45434 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/configuration.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      901 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/onnxruntime/constants.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      955 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/graph.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnxruntime/io_binding/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      675 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/io_binding/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7767 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3915 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/model.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    30965 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/modeling_decoder.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17940 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/modeling_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    83591 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/modeling_ort.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    58316 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/modeling_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    15083 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/optimization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnxruntime/preprocessors/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      686 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      760 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3048 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1377 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1415 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1580 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2350 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/preprocessors/quantization.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23448 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/quantization.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/onnxruntime/runs/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     8001 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/runs/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4070 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/runs/calibrator.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      625 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/runs/utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    88945 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/trainer.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    38387 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/trainer_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    17122 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/onnxruntime/training_args.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1362 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/onnxruntime/training_args_seq2seq.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11746 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/onnxruntime/utils.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/pipelines/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      770 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/pipelines/__init__.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/pipelines/diffusers/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11266 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2211 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    13522 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/pipelines/pipelines_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      948 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/quantization_base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10268 2023-04-11 18:28:51.000000 optimum-1.8.1/optimum/runs_base.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/utils/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1989 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/utils/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      845 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/constant.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2001 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/doc.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      953 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/dummy_diffusers_objects.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3747 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/file_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     6181 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/import_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    23612 2023-04-13 16:43:16.000000 optimum-1.8.1/optimum/utils/input_generators.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     7836 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/utils/logging.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1295 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/modeling_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     9323 2023-04-17 09:03:56.000000 optimum-1.8.1/optimum/utils/normalized_config.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.575548 optimum-1.8.1/optimum/utils/preprocessing/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      977 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/preprocessing/__init__.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    10271 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/preprocessing/base.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4263 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/preprocessing/image_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3995 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/preprocessing/question_answering.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2169 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/utils/preprocessing/task_processors_manager.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4436 2023-04-17 09:33:41.000000 optimum-1.8.1/optimum/utils/preprocessing/text_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3940 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/preprocessing/token_classification.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11609 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/runs.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     2364 2023-04-11 18:28:52.000000 optimum-1.8.1/optimum/utils/save_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     5762 2023-04-17 07:37:27.000000 optimum-1.8.1/optimum/utils/testing_utils.py
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      639 2023-04-17 11:22:59.000000 optimum-1.8.1/optimum/version.py
+drwxrwxr-x   0 fxmarty   (1000) fxmarty   (1000)        0 2023-04-17 12:34:09.571548 optimum-1.8.1/optimum.egg-info/
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)    11448 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/PKG-INFO
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     4303 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/SOURCES.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/dependency_links.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)       66 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/entry_points.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        1 2023-04-17 12:34:05.000000 optimum-1.8.1/optimum.egg-info/not-zip-safe
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      973 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/requires.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)        8 2023-04-17 12:34:09.000000 optimum-1.8.1/optimum.egg-info/top_level.txt
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     1212 2023-03-21 09:04:22.000000 optimum-1.8.1/pyproject.toml
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)      423 2023-04-17 12:34:09.575548 optimum-1.8.1/setup.cfg
+-rw-rw-r--   0 fxmarty   (1000) fxmarty   (1000)     3429 2023-04-11 18:28:51.000000 optimum-1.8.1/setup.py
```

### Comparing `optimum-1.8.0/LICENSE` & `optimum-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/MANIFEST.in` & `optimum-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/PKG-INFO` & `optimum-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.0
+Version: 1.8.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Platform: UNKNOWN
```

### Comparing `optimum-1.8.0/README.md` & `optimum-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/__init__.py` & `optimum-1.8.1/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/models/__init__.py` & `optimum-1.8.1/optimum/bettertransformer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/models/attention.py` & `optimum-1.8.1/optimum/bettertransformer/models/attention.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/models/base.py` & `optimum-1.8.1/optimum/bettertransformer/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/models/decoder_models.py` & `optimum-1.8.1/optimum/bettertransformer/models/decoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.8.1/optimum/bettertransformer/models/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/bettertransformer/transformation.py` & `optimum-1.8.1/optimum/bettertransformer/transformation.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/__init__.py` & `optimum-1.8.1/optimum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/base.py` & `optimum-1.8.1/optimum/commands/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/env.py` & `optimum-1.8.1/optimum/commands/env.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/export/__init__.py` & `optimum-1.8.1/optimum/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/export/base.py` & `optimum-1.8.1/optimum/commands/export/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/export/ggml.py` & `optimum-1.8.1/optimum/commands/export/ggml.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/export/onnx.py` & `optimum-1.8.1/optimum/commands/export/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/export/tflite.py` & `optimum-1.8.1/optimum/commands/export/tflite.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/onnxruntime/__init__.py` & `optimum-1.8.1/optimum/commands/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/onnxruntime/base.py` & `optimum-1.8.1/optimum/commands/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/onnxruntime/optimize.py` & `optimum-1.8.1/optimum/commands/onnxruntime/optimize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/onnxruntime/quantize.py` & `optimum-1.8.1/optimum/commands/onnxruntime/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/optimum_cli.py` & `optimum-1.8.1/optimum/commands/optimum_cli.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/commands/register/__init__.py` & `optimum-1.8.1/optimum/commands/register/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/configuration_utils.py` & `optimum-1.8.1/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/conftest.py` & `optimum-1.8.1/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/__init__.py` & `optimum-1.8.1/optimum/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/base.py` & `optimum-1.8.1/optimum/exporters/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/error_utils.py` & `optimum-1.8.1/optimum/exporters/error_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/__init__.py` & `optimum-1.8.1/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/__main__.py` & `optimum-1.8.1/optimum/exporters/onnx/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/base.py` & `optimum-1.8.1/optimum/exporters/onnx/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/config.py` & `optimum-1.8.1/optimum/exporters/onnx/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/constants.py` & `optimum-1.8.1/optimum/exporters/onnx/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/convert.py` & `optimum-1.8.1/optimum/exporters/onnx/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/model_configs.py` & `optimum-1.8.1/optimum/exporters/onnx/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/model_patcher.py` & `optimum-1.8.1/optimum/exporters/onnx/model_patcher.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/onnx/utils.py` & `optimum-1.8.1/optimum/exporters/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tasks.py` & `optimum-1.8.1/optimum/exporters/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     _TASKS_TO_AUTOMODELS = {}
     _TASKS_TO_TF_AUTOMODELS = {}
     if is_torch_available():
         # Refer to https://huggingface.co/datasets/huggingface/transformers-metadata/blob/main/pipeline_tags.json
         # In case the same task (pipeline tag) may map to several loading classes, we use a tuple and the
         # auto-class _model_mapping to determine the right one.
         _TASKS_TO_AUTOMODELS = {
+            "conversational": ("AutoModelForCausalLM", "AutoModelForSeq2SeqLM"),
             "feature-extraction": "AutoModel",
             "fill-mask": "AutoModelForMaskedLM",
             "text-generation": "AutoModelForCausalLM",
             "text2text-generation": "AutoModelForSeq2SeqLM",
             "text-classification": "AutoModelForSequenceClassification",
             "token-classification": "AutoModelForTokenClassification",
             "multiple-choice": "AutoModelForMultipleChoice",
@@ -165,14 +166,15 @@
             "image-to-text": "AutoModelForVision2Seq",
             "stable-diffusion": "StableDiffusionPipeline",
             "zero-shot-image-classification": "AutoModelForZeroShotImageClassification",
             "zero-shot-object-detection": "AutoModelForZeroShotObjectDetection",
         }
     if is_tf_available():
         _TASKS_TO_TF_AUTOMODELS = {
+            "conversational": ("TFAutoModelForCausalLM", "TFAutoModelForSeq2SeqLM"),
             "feature-extraction": "TFAutoModel",
             "fill-mask": "TFAutoModelForMaskedLM",
             "text-generation": "TFAutoModelForCausalLM",
             "image-classification": "TFAutoModelForImageClassification",
             "text2text-generation": "TFAutoModelForSeq2SeqLM",
             "text-classification": "TFAutoModelForSequenceClassification",
             "token-classification": "TFAutoModelForTokenClassification",
@@ -200,45 +202,52 @@
         "speech2seq-lm": "automatic-speech-recognition",
         "speech2seq-lm-with-past": "automatic-speech-recognition-with-past",
         "masked-lm": "fill-mask",
         "vision2seq-lm": "image-to-text",
         "default": "feature-extraction",
         "default-with-past": "feature-extraction-with-past",
         "audio-ctc": "automatic-speech-recognition",
+        "translation": "text2text-generation",
+        "summarization": "text2text-generation",
+        "zero-shot-classification": "text-classification",
     }
 
     # Reverse dictionaries str -> str, where several automodels may map to the same task
     _AUTOMODELS_TO_TASKS = get_automodels_to_tasks(_TASKS_TO_AUTOMODELS)
     _TF_AUTOMODELS_TO_TASKS = get_automodels_to_tasks(_TASKS_TO_TF_AUTOMODELS)
 
     _CUSTOM_CLASSES = {
         ("pt", "pix2struct", "image-to-text"): ("transformers", "Pix2StructForConditionalGeneration"),
         ("pt", "visual-bert", "question-answering"): ("transformers", "VisualBertForQuestionAnswering"),
     }
 
     _TASKS_TO_LIBRARY = {
+        "conversational": "transformers",
         "feature-extraction": "transformers",
         "fill-mask": "transformers",
         "text-generation": "transformers",
         "text2text-generation": "transformers",
         "text-classification": "transformers",
         "token-classification": "transformers",
+        "translation": "transformers",
         "multiple-choice": "transformers",
         "object-detection": "transformers",
         "question-answering": "transformers",
         "image-classification": "transformers",
         "image-segmentation": "transformers",
         "masked-im": "transformers",
         "semantic-segmentation": "transformers",
         "automatic-speech-recognition": "transformers",
         "audio-classification": "transformers",
         "audio-frame-classification": "transformers",
         "audio-xvector": "transformers",
         "image-to-text": "transformers",
         "stable-diffusion": "diffusers",
+        "summarization": "transformers",
+        "zero-shot-classification": "transformers",
         "zero-shot-image-classification": "transformers",
         "zero-shot-object-detection": "transformers",
     }
 
     # TODO: some models here support text-generation export but are not supported in ORTModelForCausalLM
     # Set of model topologies we support associated to the tasks supported by each topology and the factory
     _SUPPORTED_MODEL_TYPE = {
@@ -1026,24 +1035,24 @@
             return getattr(loaded_library, class_name)
         else:
             if framework == "pt":
                 tasks_to_automodel = TasksManager._TASKS_TO_AUTOMODELS
             else:
                 tasks_to_automodel = TasksManager._TASKS_TO_TF_AUTOMODELS
 
-            if task not in tasks_to_automodel:
-                raise KeyError(
-                    f"Unknown task: {task}. Possible values are: "
-                    + ", ".join([f"`{key}` for {tasks_to_automodel[key]}" for key in tasks_to_automodel])
-                )
-
             library = TasksManager._TASKS_TO_LIBRARY[task]
             loaded_library = importlib.import_module(library)
 
             if model_class_name is None:
+                if task not in tasks_to_automodel:
+                    raise KeyError(
+                        f"Unknown task: {task}. Possible values are: "
+                        + ", ".join([f"`{key}` for {tasks_to_automodel[key]}" for key in tasks_to_automodel])
+                    )
+
                 if isinstance(tasks_to_automodel[task], str):
                     model_class_name = tasks_to_automodel[task]
                 else:
                     # automatic-speech-recognition case, which may map to several auto class
                     if library == "transformers":
                         if model_type is None:
                             logger.warning(
@@ -1219,15 +1228,18 @@
                 )
             model_info = huggingface_hub.model_info(model_name_or_path, revision=revision)
             if model_info.library_name == "diffusers":
                 # TODO : getattr(model_info, "model_index") defining auto_model_class_name currently set to None
                 if "stable-diffusion" in model_info.tags:
                     inferred_task_name = "stable-diffusion"
             else:
-                if getattr(model_info, "pipeline_tag", None) is not None:
+                pipeline_tag = getattr(model_info, "pipeline_tag", None)
+                # conversational is not a supported task per se, just an alias that may map to
+                # text-generaton or text2text-generation
+                if pipeline_tag is not None and pipeline_tag != "conversational":
                     inferred_task_name = model_info.pipeline_tag
                 else:
                     transformers_info = model_info.transformersInfo
 
                     if transformers_info is None or transformers_info.get("auto_model") is None:
                         raise RuntimeError(f"Could not infer the task from the model repo {model_name_or_path}")
                     auto_model_class_name = transformers_info["auto_model"]
```

### Comparing `optimum-1.8.0/optimum/exporters/tflite/__init__.py` & `optimum-1.8.1/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tflite/__main__.py` & `optimum-1.8.1/optimum/exporters/tflite/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tflite/base.py` & `optimum-1.8.1/optimum/exporters/tflite/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tflite/config.py` & `optimum-1.8.1/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tflite/convert.py` & `optimum-1.8.1/optimum/exporters/tflite/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/exporters/tflite/model_configs.py` & `optimum-1.8.1/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/__init__.py` & `optimum-1.8.1/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/optimization/__init__.py` & `optimum-1.8.1/optimum/fx/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/optimization/transformations.py` & `optimum-1.8.1/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/quantization/__init__.py` & `optimum-1.8.1/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/quantization/functions.py` & `optimum-1.8.1/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/fx/utils.py` & `optimum-1.8.1/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/modeling_base.py` & `optimum-1.8.1/optimum/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/__init__.py` & `optimum-1.8.1/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/configuration.py` & `optimum-1.8.1/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/graph_transformations.py` & `optimum-1.8.1/optimum/onnx/graph_transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/modeling_seq2seq.py` & `optimum-1.8.1/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/transformations_utils.py` & `optimum-1.8.1/optimum/onnx/transformations_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnx/utils.py` & `optimum-1.8.1/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/__init__.py` & `optimum-1.8.1/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/base.py` & `optimum-1.8.1/optimum/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/configuration.py` & `optimum-1.8.1/optimum/onnxruntime/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/constants.py` & `optimum-1.8.1/optimum/onnxruntime/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/graph.py` & `optimum-1.8.1/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.8.1/optimum/onnxruntime/io_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.8.1/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/model.py` & `optimum-1.8.1/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.8.1/optimum/onnxruntime/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.8.1/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/modeling_ort.py` & `optimum-1.8.1/optimum/onnxruntime/modeling_ort.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.8.1/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/optimization.py` & `optimum-1.8.1/optimum/onnxruntime/optimization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.8.1/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/quantization.py` & `optimum-1.8.1/optimum/onnxruntime/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/runs/__init__.py` & `optimum-1.8.1/optimum/onnxruntime/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.8.1/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/runs/utils.py` & `optimum-1.8.1/optimum/onnxruntime/runs/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/trainer.py` & `optimum-1.8.1/optimum/onnxruntime/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.8.1/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/training_args.py` & `optimum-1.8.1/optimum/onnxruntime/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.8.1/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/onnxruntime/utils.py` & `optimum-1.8.1/optimum/onnxruntime/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/pipelines/__init__.py` & `optimum-1.8.1/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.8.1/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.8.1/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/pipelines/pipelines_base.py` & `optimum-1.8.1/optimum/pipelines/pipelines_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/quantization_base.py` & `optimum-1.8.1/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/runs_base.py` & `optimum-1.8.1/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/__init__.py` & `optimum-1.8.1/optimum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/constant.py` & `optimum-1.8.1/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/doc.py` & `optimum-1.8.1/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.8.1/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/file_utils.py` & `optimum-1.8.1/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/import_utils.py` & `optimum-1.8.1/optimum/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/input_generators.py` & `optimum-1.8.1/optimum/utils/input_generators.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/logging.py` & `optimum-1.8.1/optimum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/modeling_utils.py` & `optimum-1.8.1/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/normalized_config.py` & `optimum-1.8.1/optimum/utils/normalized_config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/__init__.py` & `optimum-1.8.1/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/base.py` & `optimum-1.8.1/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/image_classification.py` & `optimum-1.8.1/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/question_answering.py` & `optimum-1.8.1/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.8.1/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/text_classification.py` & `optimum-1.8.1/optimum/utils/preprocessing/text_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/preprocessing/token_classification.py` & `optimum-1.8.1/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/runs.py` & `optimum-1.8.1/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/save_utils.py` & `optimum-1.8.1/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/utils/testing_utils.py` & `optimum-1.8.1/optimum/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/optimum/version.py` & `optimum-1.8.1/optimum/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
```

### Comparing `optimum-1.8.0/optimum.egg-info/PKG-INFO` & `optimum-1.8.1/optimum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.0
+Version: 1.8.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Platform: UNKNOWN
```

### Comparing `optimum-1.8.0/optimum.egg-info/SOURCES.txt` & `optimum-1.8.1/optimum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,10 +117,8 @@
 optimum/utils/testing_utils.py
 optimum/utils/preprocessing/__init__.py
 optimum/utils/preprocessing/base.py
 optimum/utils/preprocessing/image_classification.py
 optimum/utils/preprocessing/question_answering.py
 optimum/utils/preprocessing/task_processors_manager.py
 optimum/utils/preprocessing/text_classification.py
-optimum/utils/preprocessing/token_classification.py
-tests/test_configuration_utils.py
-tests/test_modeling_base.py
+optimum/utils/preprocessing/token_classification.py
```

### Comparing `optimum-1.8.0/optimum.egg-info/requires.txt` & `optimum-1.8.1/optimum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/pyproject.toml` & `optimum-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.8.0/setup.py` & `optimum-1.8.1/setup.py`

 * *Files identical despite different names*

