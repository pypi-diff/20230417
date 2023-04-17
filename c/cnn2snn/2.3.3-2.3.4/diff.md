# Comparing `tmp/cnn2snn-2.3.3.tar.gz` & `tmp/cnn2snn-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cnn2snn-2.3.3.tar", last modified: Tue Apr  4 14:27:10 2023, max compression
+gzip compressed data, was "dist/cnn2snn-2.3.4.tar", last modified: Mon Apr 17 08:48:50 2023, max compression
```

## Comparing `cnn2snn-2.3.3.tar` & `cnn2snn-2.3.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn/
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/akida_versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn/calibration/
--rw-r--r--   0 root         (0) root         (0)      958 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16847 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/calibration/adaround.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/calibration/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)    12381 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/calibration/calibration.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/cli.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/cnn2snn_objects.py
--rw-r--r--   0 root         (0) root         (0)    12382 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/converter.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/min_value_constraint.py
--rw-r--r--   0 root         (0) root         (0)    14077 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/model_generator.py
--rw-r--r--   0 root         (0) root         (0)    13749 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantization.py
--rw-r--r--   0 root         (0) root         (0)    26028 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantization_layers.py
--rw-r--r--   0 root         (0) root         (0)    12977 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantization_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      882 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/activations.py
--rw-r--r--   0 root         (0) root         (0)     3671 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/add.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/attention.py
--rw-r--r--   0 root         (0) root         (0)     5253 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/batchnorm.py
--rw-r--r--   0 root         (0) root         (0)     7844 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/compatibility_checks.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/concatenate.py
--rw-r--r--   0 root         (0) root         (0)     6573 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     7803 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/convolution.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/dense.py
--rw-r--r--   0 root         (0) root         (0)     6266 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     6342 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/dequantizer.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/extract_token.py
--rw-r--r--   0 root         (0) root         (0)     3442 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/input_data.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/layer_utils.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/madnorm.py
--rw-r--r--   0 root         (0) root         (0)     6680 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/model_generator.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/outputs.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/padding.py
--rw-r--r--   0 root         (0) root         (0)     4068 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/pooling.py
--rw-r--r--   0 root         (0) root         (0)     5549 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     3083 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     9310 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/stem.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/quantizeml/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn/transforms/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/clone.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/equalization.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/reshape.py
--rw-r--r--   0 root         (0) root         (0)    14261 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/transforms/sequential.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/utils.py
--rw-r--r--   0 root         (0) root         (0)    11223 2023-04-04 14:27:06.000000 cnn2snn-2.3.3/cnn2snn/weights_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1760 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/cnn2snn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 14:27:10.000000 cnn2snn-2.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2023-04-04 14:27:01.000000 cnn2snn-2.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/akida_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/calibration/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16847 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/adaround.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)    12381 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/calibration/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    10739 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/cnn2snn_objects.py
+-rw-r--r--   0 root         (0) root         (0)    12382 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/min_value_constraint.py
+-rw-r--r--   0 root         (0) root         (0)    14077 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)    13749 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    26028 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization_layers.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantization_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)      882 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/activations.py
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/add.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/batchnorm.py
+-rw-r--r--   0 root         (0) root         (0)     7844 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13873 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/compatibility_checks.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/concatenate.py
+-rw-r--r--   0 root         (0) root         (0)     6573 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/convolution.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/dense.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     6342 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/dequantizer.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/extract_token.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/input_data.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/layer_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/madnorm.py
+-rw-r--r--   0 root         (0) root         (0)     6680 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/model_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/outputs.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/padding.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     5549 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     9310 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/stem.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/quantizeml/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/clone.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/equalization.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/reshape.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/transforms/sequential.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11223 2023-04-17 08:48:47.000000 cnn2snn-2.3.4/cnn2snn/weights_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/cnn2snn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 08:48:50.000000 cnn2snn-2.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-04-17 08:48:41.000000 cnn2snn-2.3.4/setup.py
```

### Comparing `cnn2snn-2.3.3/LICENSE` & `cnn2snn-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/PKG-INFO` & `cnn2snn-2.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.3
+Version: 2.3.4
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.3/cnn2snn/__init__.py` & `cnn2snn-2.3.4/cnn2snn/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/akida_versions.py` & `cnn2snn-2.3.4/cnn2snn/akida_versions.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/calibration/__init__.py` & `cnn2snn-2.3.4/cnn2snn/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/calibration/adaround.py` & `cnn2snn-2.3.4/cnn2snn/calibration/adaround.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/calibration/bias_correction.py` & `cnn2snn-2.3.4/cnn2snn/calibration/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/calibration/calibration.py` & `cnn2snn-2.3.4/cnn2snn/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/cli.py` & `cnn2snn-2.3.4/cnn2snn/cli.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/cnn2snn_objects.py` & `cnn2snn-2.3.4/cnn2snn/cnn2snn_objects.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/compatibility_checks.py` & `cnn2snn-2.3.4/cnn2snn/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/converter.py` & `cnn2snn-2.3.4/cnn2snn/converter.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/min_value_constraint.py` & `cnn2snn-2.3.4/cnn2snn/min_value_constraint.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/model_generator.py` & `cnn2snn-2.3.4/cnn2snn/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantization.py` & `cnn2snn-2.3.4/cnn2snn/quantization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantization_layers.py` & `cnn2snn-2.3.4/cnn2snn/quantization_layers.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantization_ops.py` & `cnn2snn-2.3.4/cnn2snn/quantization_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/__init__.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/activations.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/activations.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/add.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/add.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/attention.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/attention.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/batchnorm.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/batchnorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     assert isinstance(layer_bn.b_quantizer, qlayers.AlignedWeightQuantizer)
 
     # get the QuantizedBatchNormalization a, b and shift
     a_ak = layer_bn.a_quantizer.qweights.value.values.numpy()
     b_quantizer = layer_bn.b_quantizer
     b = b_quantizer.qweights.value.values.numpy().astype(np.int32)
     b_shift = b_quantizer.shift.value.numpy().astype(np.uint8)
-    b_ak = b >> b_shift
+    b_ak = (b >> b_shift).astype(np.int8)
 
     variables_ak = ak_layer.variables
 
     input_shift = layer_bn.input_shift.value
     if input_shift is not None:
         broadcast_and_set_variable(variables_ak, "input_shift",
                                    input_shift.numpy().astype(np.uint8))
```

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/blocks.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/blocks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/compatibility_checks.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/compatibility_checks.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/concatenate.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/concatenate.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/conv2d_transpose.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/convolution.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/dense.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/dense.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/depthwise_conv2d.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/depthwise_conv2d_transpose.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/depthwise_conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/dequantizer.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/dequantizer.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/extract_token.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/extract_token.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/input_data.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/input_data.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/layer_utils.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/layer_utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/madnorm.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/madnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,29 +43,29 @@
     # get the QuantizedLayerNormalization gamma and shift
     gamma_ak = k_layer.gamma_quantizer.qweights.value.values.numpy()
     gamma_shift = k_layer.gamma_shift.value.numpy().astype(np.uint8)
     # get the QuantizedLayerNormalization beta and shift
     beta_quantizer = k_layer.beta_quantizer
     beta = beta_quantizer.qweights.value.values.numpy().astype(np.int32)
     beta_shift = beta_quantizer.shift.value.numpy().astype(np.uint8)
-    beta_ak = beta >> beta_shift
+    beta_ak = (beta >> beta_shift).astype(np.int8)
 
     variables_ak = ak_layer.variables
 
     input_shift = getattr(k_layer, 'input_shift', None)
     if input_shift is not None:
         if np.any(input_shift.value < 0):
             raise RuntimeError(
                 f"Layer {k_layer.name} contains negative values for " +
                 "input_shift, that is not supported")
         broadcast_and_set_variable(variables_ak, "input_shift",
                                    input_shift.value.numpy().astype(np.uint8))
-    variables_ak["gamma"] = gamma_ak.astype(np.int32)
+    variables_ak["gamma"] = gamma_ak.astype(np.int8)
     broadcast_and_set_variable(variables_ak, "gamma_shift", gamma_shift)
-    variables_ak["beta"] = beta_ak
+    variables_ak["beta"] = beta_ak.astype(np.int8)
     broadcast_and_set_variable(variables_ak, "beta_shift", beta_shift)
     out_quantizer = getattr(k_layer, "out_quantizer", False)
     if out_quantizer:
         set_output_variables(ak_layer, out_quantizer)
 
 
 def _create_madnorm(layer):
```

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/model_generator.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/model_generator.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/outputs.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/outputs.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/padding.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/padding.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/pooling.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/pooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,14 @@
     if get_akida_version() == AkidaVersion.v1:
         return dict(pool_type=PoolType.Average)
 
     # Check if there is an output_quantizer
     out_quantizer = getattr(layer, "out_quantizer", None)
 
     assert isinstance(out_quantizer, OutputQuantizer)
-    if out_quantizer.signed:
-        raise ValueError(f"{layer.name}: output_quantizer should not be signed")
 
     return dict(pool_type=PoolType.Average, output_bits=out_quantizer.bitwidth)
 
 
 def set_pooling_variables(layer_ak, layer_k):
     """Computes and sets the pooling variables in an akida layer.
```

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/separable_convolution.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/separable_convolution.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/shiftmax.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/shiftmax.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/stem.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/stem.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/quantizeml/weights.py` & `cnn2snn-2.3.4/cnn2snn/quantizeml/weights.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/__init__.py` & `cnn2snn-2.3.4/cnn2snn/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/batch_normalization.py` & `cnn2snn-2.3.4/cnn2snn/transforms/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/clone.py` & `cnn2snn-2.3.4/cnn2snn/transforms/clone.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/equalization.py` & `cnn2snn-2.3.4/cnn2snn/transforms/equalization.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/reshape.py` & `cnn2snn-2.3.4/cnn2snn/transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/transforms/sequential.py` & `cnn2snn-2.3.4/cnn2snn/transforms/sequential.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/utils.py` & `cnn2snn-2.3.4/cnn2snn/utils.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn/weights_ops.py` & `cnn2snn-2.3.4/cnn2snn/weights_ops.py`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/cnn2snn.egg-info/PKG-INFO` & `cnn2snn-2.3.4/cnn2snn.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnn2snn
-Version: 2.3.3
+Version: 2.3.4
 Summary: Keras to Akida CNN Converter
 Home-page: https://doc.brainchipinc.com
 Author: Alvaro Moran
 Author-email: amoran@brainchip.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnn2snn-2.3.3/cnn2snn.egg-info/SOURCES.txt` & `cnn2snn-2.3.4/cnn2snn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnn2snn-2.3.3/setup.py` & `cnn2snn-2.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cnn2snn',
-    version='2.3.3',
+    version='2.3.4',
     description='Keras to Akida CNN Converter',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Alvaro Moran',
     author_email='amoran@brainchip.com',
     url='https://doc.brainchipinc.com',
     license='Apache 2.0',
     packages=['cnn2snn', 'cnn2snn.transforms', 'cnn2snn.calibration', 'cnn2snn.quantizeml'],
     entry_points={
         'console_scripts': [ 'cnn2snn = cnn2snn.cli:main' ]
     },
     install_requires=[get_tf_dep(), 'keras~=2.10.0',
-        'akida==2.3.3', 'quantizeml~=0.4.1'],
+        'akida==2.3.4', 'quantizeml~=0.4.1'],
 )
```

