# Comparing `tmp/ptflops-0.6.9.tar.gz` & `tmp/ptflops-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptflops-0.6.9.tar", last modified: Fri May  6 19:44:14 2022, max compression
+gzip compressed data, was "ptflops-0.7.tar", last modified: Tue Apr 18 00:44:40 2023, max compression
```

## Comparing `ptflops-0.6.9.tar` & `ptflops-0.7.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 sovrasov  (1000) sovrasov  (1000)        0 2022-05-06 19:44:14.608920 ptflops-0.6.9/
--rw-r--r--   0 sovrasov  (1000) sovrasov  (1000)     1075 2020-04-13 14:29:03.000000 ptflops-0.6.9/LICENSE
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     9749 2022-05-06 19:44:14.608920 ptflops-0.6.9/PKG-INFO
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     9358 2022-04-07 14:10:03.000000 ptflops-0.6.9/README.md
-drwxrwxr-x   0 sovrasov  (1000) sovrasov  (1000)        0 2022-05-06 19:44:14.608920 ptflops-0.6.9/ptflops/
--rw-r--r--   0 sovrasov  (1000) sovrasov  (1000)       53 2020-04-13 14:29:03.000000 ptflops-0.6.9/ptflops/__init__.py
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     2105 2022-04-07 14:10:03.000000 ptflops-0.6.9/ptflops/flops_counter.py
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)    10125 2022-04-07 14:10:03.000000 ptflops-0.6.9/ptflops/pytorch_engine.py
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     8836 2022-04-07 14:10:03.000000 ptflops-0.6.9/ptflops/pytorch_ops.py
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     1671 2022-04-07 14:10:03.000000 ptflops-0.6.9/ptflops/utils.py
-drwxrwxr-x   0 sovrasov  (1000) sovrasov  (1000)        0 2022-05-06 19:44:14.608920 ptflops-0.6.9/ptflops.egg-info/
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)     9749 2022-05-06 19:44:14.000000 ptflops-0.6.9/ptflops.egg-info/PKG-INFO
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)      317 2022-05-06 19:44:14.000000 ptflops-0.6.9/ptflops.egg-info/SOURCES.txt
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)        1 2022-05-06 19:44:14.000000 ptflops-0.6.9/ptflops.egg-info/dependency_links.txt
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)        6 2022-05-06 19:44:14.000000 ptflops-0.6.9/ptflops.egg-info/requires.txt
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)        8 2022-05-06 19:44:14.000000 ptflops-0.6.9/ptflops.egg-info/top_level.txt
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)        1 2020-10-11 16:28:20.000000 ptflops-0.6.9/ptflops.egg-info/zip-safe
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)       38 2022-05-06 19:44:14.608920 ptflops-0.6.9/setup.cfg
--rw-rw-r--   0 sovrasov  (1000) sovrasov  (1000)      754 2022-05-06 19:41:49.000000 ptflops-0.6.9/setup.py
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2023-04-18 00:44:40.017729 ptflops-0.7/
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    11286 2023-04-18 00:44:40.017729 ptflops-0.7/PKG-INFO
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     9676 2023-04-17 22:13:59.000000 ptflops-0.7/README.md
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2023-04-18 00:44:40.017729 ptflops-0.7/ptflops/
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       53 2022-11-16 21:01:54.000000 ptflops-0.7/ptflops/__init__.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     2105 2022-11-16 21:01:54.000000 ptflops-0.7/ptflops/flops_counter.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    10413 2023-04-18 00:40:30.000000 ptflops-0.7/ptflops/pytorch_engine.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     8907 2023-04-18 00:40:30.000000 ptflops-0.7/ptflops/pytorch_ops.py
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)     1671 2022-11-16 21:01:54.000000 ptflops-0.7/ptflops/utils.py
+drwxrwxr-x   0 vsovraso  (1002) vsovraso  (1002)        0 2023-04-18 00:44:40.017729 ptflops-0.7/ptflops.egg-info/
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)    11286 2023-04-18 00:44:39.000000 ptflops-0.7/ptflops.egg-info/PKG-INFO
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      309 2023-04-18 00:44:40.000000 ptflops-0.7/ptflops.egg-info/SOURCES.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2023-04-18 00:44:39.000000 ptflops-0.7/ptflops.egg-info/dependency_links.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        6 2023-04-18 00:44:39.000000 ptflops-0.7/ptflops.egg-info/requires.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        8 2023-04-18 00:44:39.000000 ptflops-0.7/ptflops.egg-info/top_level.txt
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)        1 2022-11-16 21:12:09.000000 ptflops-0.7/ptflops.egg-info/zip-safe
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)       38 2023-04-18 00:44:40.017729 ptflops-0.7/setup.cfg
+-rw-rw-r--   0 vsovraso  (1002) vsovraso  (1002)      752 2023-04-18 00:40:30.000000 ptflops-0.7/setup.py
```

### Comparing `ptflops-0.6.9/PKG-INFO` & `ptflops-0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-Metadata-Version: 2.1
-Name: ptflops
-Version: 0.6.9
-Summary: Flops counter for convolutional networks inpytorch framework
-Home-page: https://github.com/sovrasov/flops-counter.pytorch
-Author: Vladislav Sovrasov
-Author-email: sovrasov.vlad@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Flops counter for convolutional networks in pytorch framework
+# Flops counting tool for neural networks in pytorch framework
 [![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
 [![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
 
 This script is designed to compute the theoretical amount of multiply-add operations
 in convolutional neural networks. It can also compute the number of parameters and
 print per-layer computational cost of a given network.
 
 Supported layers:
 - Conv1d/2d/3d (including grouping)
 - ConvTranspose1d/2d/3d (including grouping)
-- BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d
+- BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d, LayerNorm
 - Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
 - Linear
 - Upsample
 - Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
 
 Experimental support:
 - RNN, LSTM, GRU (NLH layout is assumed)
@@ -67,14 +54,25 @@
   net = models.densenet161()
   macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
                                            print_per_layer_stat=True, verbose=True)
   print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
   print('{:<30}  {:<8}'.format('Number of parameters: ', params))
 ```
 
+## Citation
+If ptflops was useful for your paper or tech report, please cite me:
+```
+@online{ptflops,
+  author = {Vladislav Sovrasov},
+  title = {ptflops: a flops counting tool for neural networks in pytorch framework},
+  year = 2018-2023,
+  url = {https://github.com/sovrasov/flops-counter.pytorch},
+}
+```
+
 ## Benchmark
 
 ### [torchvision](https://pytorch.org/docs/1.0.0/torchvision/models.html)
 
 Model         | Input Resolution | Params(M) | MACs(G) | Top-1 error | Top-5 error
 ---           |---               |---        |---      |---          |---
 alexnet       |224x224           | 61.1      | 0.72    | 43.45       | 20.91
@@ -150,9 +148,7 @@
 vgg16_bn            | 224x224          | 138.37    | 15.53       | 73.518      | 91.608
 vgg19               | 224x224          | 143.67    | 19.67       | 72.08       | 90.822
 vgg19_bn            | 224x224          | 143.68    | 19.7        | 74.266      | 92.066
 xception            | 299x299          | 22.86     | 8.42        | 78.888      | 94.292
 
 * Acc@1 - ImageNet single-crop top-1 accuracy on validation images of the same size used during the training process.
 * Acc@5 - ImageNet single-crop top-5 accuracy on validation images of the same size used during the training process.
-
-
```

### Comparing `ptflops-0.6.9/README.md` & `ptflops-0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,166 @@
-# Flops counter for convolutional networks in pytorch framework
-[![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
-[![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
-
-This script is designed to compute the theoretical amount of multiply-add operations
-in convolutional neural networks. It can also compute the number of parameters and
-print per-layer computational cost of a given network.
-
-Supported layers:
-- Conv1d/2d/3d (including grouping)
-- ConvTranspose1d/2d/3d (including grouping)
-- BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d
-- Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
-- Linear
-- Upsample
-- Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
-
-Experimental support:
-- RNN, LSTM, GRU (NLH layout is assumed)
-- RNNCell, LSTMCell, GRUCell
-- MultiheadAttention
-
-Requirements: Pytorch >= 1.1, torchvision >= 0.3
-
-Thanks to @warmspringwinds for the initial version of script.
-
-## Usage tips
-
-- This script doesn't take into account `torch.nn.functional.*` operations. For an instance, if one have a semantic segmentation model and use `torch.nn.functional.interpolate` to upscale features, these operations won't contribute to overall amount of flops. To avoid that one can use `torch.nn.Upsample` instead of `torch.nn.functional.interpolate`.
-- `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
-- `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
-- `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
-for research purposes. For an instance, one can drop all convolutuions from the counting process
-specifying `ignore_modules=[torch.nn.Conv2d]`.
-
-## Install the latest version
-From PyPI:
-```bash
-pip install ptflops
-```
-
-From this repository:
-```bash
-pip install --upgrade git+https://github.com/sovrasov/flops-counter.pytorch.git
-```
-
-## Example
-```python
-import torchvision.models as models
-import torch
-from ptflops import get_model_complexity_info
-
-with torch.cuda.device(0):
-  net = models.densenet161()
-  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
-                                           print_per_layer_stat=True, verbose=True)
-  print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
-  print('{:<30}  {:<8}'.format('Number of parameters: ', params))
-```
-
-## Benchmark
-
-### [torchvision](https://pytorch.org/docs/1.0.0/torchvision/models.html)
-
-Model         | Input Resolution | Params(M) | MACs(G) | Top-1 error | Top-5 error
----           |---               |---        |---      |---          |---
-alexnet       |224x224           | 61.1      | 0.72    | 43.45       | 20.91
-vgg11         |224x224           | 132.86    | 7.63    | 30.98       | 11.37
-vgg13         |224x224           | 133.05    | 11.34   | 30.07       | 10.75
-vgg16         |224x224           | 138.36    | 15.5    | 28.41       | 9.62
-vgg19         |224x224           | 143.67    | 19.67   | 27.62       | 9.12
-vgg11_bn      |224x224           | 132.87    | 7.64    | 29.62       | 10.19
-vgg13_bn      |224x224           | 133.05    | 11.36   | 28.45       | 9.63
-vgg16_bn      |224x224           | 138.37    | 15.53   | 26.63       | 8.50
-vgg19_bn      |224x224           | 143.68    | 19.7    | 25.76       | 8.15
-resnet18      |224x224           | 11.69     | 1.82    | 30.24       | 10.92
-resnet34      |224x224           | 21.8      | 3.68    | 26.70       | 8.58
-resnet50      |224x224           | 25.56     | 4.12    | 23.85       | 7.13
-resnet101     |224x224           | 44.55     | 7.85    | 22.63       | 6.44
-resnet152     |224x224           | 60.19     | 11.58   | 21.69       | 5.94
-squeezenet1_0 |224x224           | 1.25      | 0.83    | 41.90       | 19.58
-squeezenet1_1 |224x224           | 1.24      | 0.36    | 41.81       | 19.38
-densenet121   |224x224           | 7.98      | 2.88    | 25.35       | 7.83
-densenet169   |224x224           | 14.15     | 3.42    | 24.00       | 7.00
-densenet201   |224x224           | 20.01     | 4.37    | 22.80       | 6.43
-densenet161   |224x224           | 28.68     | 7.82    | 22.35       | 6.20
-inception_v3  |224x224           | 27.16     | 2.85    | 22.55       | 6.44
-
-* Top-1 error - ImageNet single-crop top-1 error (224x224)
-* Top-5 error - ImageNet single-crop top-5 error (224x224)
-
-### [Cadene/pretrained-models.pytorch](https://github.com/Cadene/pretrained-models.pytorch)
-
-Model               | Input Resolution | Params(M) | MACs(G)     | Acc@1       | Acc@5
----                 |---               |---        |---          |---          |---
-alexnet             | 224x224          | 61.1      | 0.72        | 56.432      | 79.194
-bninception         | 224x224          | 11.3      | 2.05        | 73.524      | 91.562
-cafferesnet101      | 224x224          | 44.55     | 7.62        | 76.2        | 92.766
-densenet121         | 224x224          | 7.98      | 2.88        | 74.646      | 92.136
-densenet161         | 224x224          | 28.68     | 7.82        | 77.56       | 93.798
-densenet169         | 224x224          | 14.15     | 3.42        | 76.026      | 92.992
-densenet201         | 224x224          | 20.01     | 4.37        | 77.152      | 93.548
-dpn107              | 224x224          | 86.92     | 18.42       | 79.746      | 94.684
-dpn131              | 224x224          | 79.25     | 16.13       | 79.432      | 94.574
-dpn68               | 224x224          | 12.61     | 2.36        | 75.868      | 92.774
-dpn68b              | 224x224          | 12.61     | 2.36        | 77.034      | 93.59
-dpn92               | 224x224          | 37.67     | 6.56        | 79.4        | 94.62
-dpn98               | 224x224          | 61.57     | 11.76       | 79.224      | 94.488
-fbresnet152         | 224x224          | 60.27     | 11.6        | 77.386      | 93.594
-inceptionresnetv2   | 299x299          | 55.84     | 13.22       | 80.17       | 95.234
-inceptionv3         | 299x299          | 27.16     | 5.73        | 77.294      | 93.454
-inceptionv4         | 299x299          | 42.68     | 12.31       | 80.062      | 94.926
-nasnetalarge        | 331x331          | 88.75     | 24.04       | 82.566      | 96.086
-nasnetamobile       | 224x224          | 5.29      | 0.59        | 74.08       | 91.74
-pnasnet5large       | 331x331          | 86.06     | 25.21       | 82.736      | 95.992
-polynet             | 331x331          | 95.37     | 34.9        | 81.002      | 95.624
-resnet101           | 224x224          | 44.55     | 7.85        | 77.438      | 93.672
-resnet152           | 224x224          | 60.19     | 11.58       | 78.428      | 94.11
-resnet18            | 224x224          | 11.69     | 1.82        | 70.142      | 89.274
-resnet34            | 224x224          | 21.8      | 3.68        | 73.554      | 91.456
-resnet50            | 224x224          | 25.56     | 4.12        | 76.002      | 92.98
-resnext101_32x4d    | 224x224          | 44.18     | 8.03        | 78.188      | 93.886
-resnext101_64x4d    | 224x224          | 83.46     | 15.55       | 78.956      | 94.252
-se_resnet101        | 224x224          | 49.33     | 7.63        | 78.396      | 94.258
-se_resnet152        | 224x224          | 66.82     | 11.37       | 78.658      | 94.374
-se_resnet50         | 224x224          | 28.09     | 3.9         | 77.636      | 93.752
-se_resnext101_32x4d | 224x224          | 48.96     | 8.05        | 80.236      | 95.028
-se_resnext50_32x4d  | 224x224          | 27.56     | 4.28        | 79.076      | 94.434
-senet154            | 224x224          | 115.09    | 20.82       | 81.304      | 95.498
-squeezenet1_0       | 224x224          | 1.25      | 0.83        | 58.108      | 80.428
-squeezenet1_1       | 224x224          | 1.24      | 0.36        | 58.25       | 80.8
-vgg11               | 224x224          | 132.86    | 7.63        | 68.97       | 88.746
-vgg11_bn            | 224x224          | 132.87    | 7.64        | 70.452      | 89.818
-vgg13               | 224x224          | 133.05    | 11.34       | 69.662      | 89.264
-vgg13_bn            | 224x224          | 133.05    | 11.36       | 71.508      | 90.494
-vgg16               | 224x224          | 138.36    | 15.5        | 71.636      | 90.354
-vgg16_bn            | 224x224          | 138.37    | 15.53       | 73.518      | 91.608
-vgg19               | 224x224          | 143.67    | 19.67       | 72.08       | 90.822
-vgg19_bn            | 224x224          | 143.68    | 19.7        | 74.266      | 92.066
-xception            | 299x299          | 22.86     | 8.42        | 78.888      | 94.292
-
-* Acc@1 - ImageNet single-crop top-1 accuracy on validation images of the same size used during the training process.
-* Acc@5 - ImageNet single-crop top-5 accuracy on validation images of the same size used during the training process.
+Metadata-Version: 2.1
+Name: ptflops
+Version: 0.7
+Summary: Flops counter for convolutional networks inpytorch framework
+Home-page: https://github.com/sovrasov/flops-counter.pytorch
+Author: Vladislav Sovrasov
+Author-email: sovrasov.vlad@gmail.com
+License: MIT
+Description: # Flops counting tool for neural networks in pytorch framework
+        [![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
+        [![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
+        
+        This script is designed to compute the theoretical amount of multiply-add operations
+        in convolutional neural networks. It can also compute the number of parameters and
+        print per-layer computational cost of a given network.
+        
+        Supported layers:
+        - Conv1d/2d/3d (including grouping)
+        - ConvTranspose1d/2d/3d (including grouping)
+        - BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d, LayerNorm
+        - Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
+        - Linear
+        - Upsample
+        - Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
+        
+        Experimental support:
+        - RNN, LSTM, GRU (NLH layout is assumed)
+        - RNNCell, LSTMCell, GRUCell
+        - MultiheadAttention
+        
+        Requirements: Pytorch >= 1.1, torchvision >= 0.3
+        
+        Thanks to @warmspringwinds for the initial version of script.
+        
+        ## Usage tips
+        
+        - This script doesn't take into account `torch.nn.functional.*` operations. For an instance, if one have a semantic segmentation model and use `torch.nn.functional.interpolate` to upscale features, these operations won't contribute to overall amount of flops. To avoid that one can use `torch.nn.Upsample` instead of `torch.nn.functional.interpolate`.
+        - `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
+        - `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
+        - `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
+        for research purposes. For an instance, one can drop all convolutuions from the counting process
+        specifying `ignore_modules=[torch.nn.Conv2d]`.
+        
+        ## Install the latest version
+        From PyPI:
+        ```bash
+        pip install ptflops
+        ```
+        
+        From this repository:
+        ```bash
+        pip install --upgrade git+https://github.com/sovrasov/flops-counter.pytorch.git
+        ```
+        
+        ## Example
+        ```python
+        import torchvision.models as models
+        import torch
+        from ptflops import get_model_complexity_info
+        
+        with torch.cuda.device(0):
+          net = models.densenet161()
+          macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
+                                                   print_per_layer_stat=True, verbose=True)
+          print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
+          print('{:<30}  {:<8}'.format('Number of parameters: ', params))
+        ```
+        
+        ## Citation
+        If ptflops was useful for your paper or tech report, please cite me:
+        ```
+        @online{ptflops,
+          author = {Vladislav Sovrasov},
+          title = {ptflops: a flops counting tool for neural networks in pytorch framework},
+          year = 2018-2023,
+          url = {https://github.com/sovrasov/flops-counter.pytorch},
+        }
+        ```
+        
+        ## Benchmark
+        
+        ### [torchvision](https://pytorch.org/docs/1.0.0/torchvision/models.html)
+        
+        Model         | Input Resolution | Params(M) | MACs(G) | Top-1 error | Top-5 error
+        ---           |---               |---        |---      |---          |---
+        alexnet       |224x224           | 61.1      | 0.72    | 43.45       | 20.91
+        vgg11         |224x224           | 132.86    | 7.63    | 30.98       | 11.37
+        vgg13         |224x224           | 133.05    | 11.34   | 30.07       | 10.75
+        vgg16         |224x224           | 138.36    | 15.5    | 28.41       | 9.62
+        vgg19         |224x224           | 143.67    | 19.67   | 27.62       | 9.12
+        vgg11_bn      |224x224           | 132.87    | 7.64    | 29.62       | 10.19
+        vgg13_bn      |224x224           | 133.05    | 11.36   | 28.45       | 9.63
+        vgg16_bn      |224x224           | 138.37    | 15.53   | 26.63       | 8.50
+        vgg19_bn      |224x224           | 143.68    | 19.7    | 25.76       | 8.15
+        resnet18      |224x224           | 11.69     | 1.82    | 30.24       | 10.92
+        resnet34      |224x224           | 21.8      | 3.68    | 26.70       | 8.58
+        resnet50      |224x224           | 25.56     | 4.12    | 23.85       | 7.13
+        resnet101     |224x224           | 44.55     | 7.85    | 22.63       | 6.44
+        resnet152     |224x224           | 60.19     | 11.58   | 21.69       | 5.94
+        squeezenet1_0 |224x224           | 1.25      | 0.83    | 41.90       | 19.58
+        squeezenet1_1 |224x224           | 1.24      | 0.36    | 41.81       | 19.38
+        densenet121   |224x224           | 7.98      | 2.88    | 25.35       | 7.83
+        densenet169   |224x224           | 14.15     | 3.42    | 24.00       | 7.00
+        densenet201   |224x224           | 20.01     | 4.37    | 22.80       | 6.43
+        densenet161   |224x224           | 28.68     | 7.82    | 22.35       | 6.20
+        inception_v3  |224x224           | 27.16     | 2.85    | 22.55       | 6.44
+        
+        * Top-1 error - ImageNet single-crop top-1 error (224x224)
+        * Top-5 error - ImageNet single-crop top-5 error (224x224)
+        
+        ### [Cadene/pretrained-models.pytorch](https://github.com/Cadene/pretrained-models.pytorch)
+        
+        Model               | Input Resolution | Params(M) | MACs(G)     | Acc@1       | Acc@5
+        ---                 |---               |---        |---          |---          |---
+        alexnet             | 224x224          | 61.1      | 0.72        | 56.432      | 79.194
+        bninception         | 224x224          | 11.3      | 2.05        | 73.524      | 91.562
+        cafferesnet101      | 224x224          | 44.55     | 7.62        | 76.2        | 92.766
+        densenet121         | 224x224          | 7.98      | 2.88        | 74.646      | 92.136
+        densenet161         | 224x224          | 28.68     | 7.82        | 77.56       | 93.798
+        densenet169         | 224x224          | 14.15     | 3.42        | 76.026      | 92.992
+        densenet201         | 224x224          | 20.01     | 4.37        | 77.152      | 93.548
+        dpn107              | 224x224          | 86.92     | 18.42       | 79.746      | 94.684
+        dpn131              | 224x224          | 79.25     | 16.13       | 79.432      | 94.574
+        dpn68               | 224x224          | 12.61     | 2.36        | 75.868      | 92.774
+        dpn68b              | 224x224          | 12.61     | 2.36        | 77.034      | 93.59
+        dpn92               | 224x224          | 37.67     | 6.56        | 79.4        | 94.62
+        dpn98               | 224x224          | 61.57     | 11.76       | 79.224      | 94.488
+        fbresnet152         | 224x224          | 60.27     | 11.6        | 77.386      | 93.594
+        inceptionresnetv2   | 299x299          | 55.84     | 13.22       | 80.17       | 95.234
+        inceptionv3         | 299x299          | 27.16     | 5.73        | 77.294      | 93.454
+        inceptionv4         | 299x299          | 42.68     | 12.31       | 80.062      | 94.926
+        nasnetalarge        | 331x331          | 88.75     | 24.04       | 82.566      | 96.086
+        nasnetamobile       | 224x224          | 5.29      | 0.59        | 74.08       | 91.74
+        pnasnet5large       | 331x331          | 86.06     | 25.21       | 82.736      | 95.992
+        polynet             | 331x331          | 95.37     | 34.9        | 81.002      | 95.624
+        resnet101           | 224x224          | 44.55     | 7.85        | 77.438      | 93.672
+        resnet152           | 224x224          | 60.19     | 11.58       | 78.428      | 94.11
+        resnet18            | 224x224          | 11.69     | 1.82        | 70.142      | 89.274
+        resnet34            | 224x224          | 21.8      | 3.68        | 73.554      | 91.456
+        resnet50            | 224x224          | 25.56     | 4.12        | 76.002      | 92.98
+        resnext101_32x4d    | 224x224          | 44.18     | 8.03        | 78.188      | 93.886
+        resnext101_64x4d    | 224x224          | 83.46     | 15.55       | 78.956      | 94.252
+        se_resnet101        | 224x224          | 49.33     | 7.63        | 78.396      | 94.258
+        se_resnet152        | 224x224          | 66.82     | 11.37       | 78.658      | 94.374
+        se_resnet50         | 224x224          | 28.09     | 3.9         | 77.636      | 93.752
+        se_resnext101_32x4d | 224x224          | 48.96     | 8.05        | 80.236      | 95.028
+        se_resnext50_32x4d  | 224x224          | 27.56     | 4.28        | 79.076      | 94.434
+        senet154            | 224x224          | 115.09    | 20.82       | 81.304      | 95.498
+        squeezenet1_0       | 224x224          | 1.25      | 0.83        | 58.108      | 80.428
+        squeezenet1_1       | 224x224          | 1.24      | 0.36        | 58.25       | 80.8
+        vgg11               | 224x224          | 132.86    | 7.63        | 68.97       | 88.746
+        vgg11_bn            | 224x224          | 132.87    | 7.64        | 70.452      | 89.818
+        vgg13               | 224x224          | 133.05    | 11.34       | 69.662      | 89.264
+        vgg13_bn            | 224x224          | 133.05    | 11.36       | 71.508      | 90.494
+        vgg16               | 224x224          | 138.36    | 15.5        | 71.636      | 90.354
+        vgg16_bn            | 224x224          | 138.37    | 15.53       | 73.518      | 91.608
+        vgg19               | 224x224          | 143.67    | 19.67       | 72.08       | 90.822
+        vgg19_bn            | 224x224          | 143.68    | 19.7        | 74.266      | 92.066
+        xception            | 299x299          | 22.86     | 8.42        | 78.888      | 94.292
+        
+        * Acc@1 - ImageNet single-crop top-1 accuracy on validation images of the same size used during the training process.
+        * Acc@5 - ImageNet single-crop top-5 accuracy on validation images of the same size used during the training process.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
```

### Comparing `ptflops-0.6.9/ptflops/flops_counter.py` & `ptflops-0.7/ptflops/flops_counter.py`

 * *Files identical despite different names*

### Comparing `ptflops-0.6.9/ptflops/pytorch_engine.py` & `ptflops-0.7/ptflops/pytorch_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,19 @@
             for m in self.children():
                 sum += m.accumulate_params()
             return sum
 
     def flops_repr(self):
         accumulated_params_num = self.accumulate_params()
         accumulated_flops_cost = self.accumulate_flops() / model.__batch_counter__
+        if accumulated_params_num > total_params:
+            print('Warning: parameters of some of the modules were counted twice because'
+                  ' of multiple links to the same modules.'
+                  ' Extended per layer parameters num statistic could be unreliable.')
+
         return ', '.join([params_to_string(accumulated_params_num,
                                            units=param_units, precision=precision),
                           '{:.3%} Params'.format(accumulated_params_num / total_params),
                           flops_to_string(accumulated_flops_cost,
                                           units=flops_units, precision=precision),
                           '{:.3%} MACs'.format(accumulated_flops_cost / total_flops),
                           self.original_extra_repr()])
```

### Comparing `ptflops-0.6.9/ptflops/pytorch_ops.py` & `ptflops-0.7/ptflops/pytorch_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     module.__flops__ += int(np.prod(input.shape))
 
 
 def bn_flops_counter_hook(module, input, output):
     input = input[0]
 
     batch_flops = np.prod(input.shape)
-    if module.affine:
+    if hasattr(module, "affine") and module.affine:
         batch_flops *= 2
     module.__flops__ += int(batch_flops)
 
 
 def conv_flops_counter_hook(conv_module, input, output):
     # Can have multiple inputs, getting the first one
     input = input[0]
@@ -253,14 +253,15 @@
     nn.BatchNorm2d: bn_flops_counter_hook,
     nn.BatchNorm3d: bn_flops_counter_hook,
 
     nn.InstanceNorm1d: bn_flops_counter_hook,
     nn.InstanceNorm2d: bn_flops_counter_hook,
     nn.InstanceNorm3d: bn_flops_counter_hook,
     nn.GroupNorm: bn_flops_counter_hook,
+    nn.LayerNorm: bn_flops_counter_hook,
     # FC
     nn.Linear: linear_flops_counter_hook,
     # Upscale
     nn.Upsample: upsample_flops_counter_hook,
     # Deconvolution
     nn.ConvTranspose1d: conv_flops_counter_hook,
     nn.ConvTranspose2d: conv_flops_counter_hook,
```

### Comparing `ptflops-0.6.9/ptflops/utils.py` & `ptflops-0.7/ptflops/utils.py`

 * *Files identical despite different names*

### Comparing `ptflops-0.6.9/ptflops.egg-info/PKG-INFO` & `ptflops-0.7/ptflops.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,158 +1,166 @@
 Metadata-Version: 2.1
 Name: ptflops
-Version: 0.6.9
+Version: 0.7
 Summary: Flops counter for convolutional networks inpytorch framework
 Home-page: https://github.com/sovrasov/flops-counter.pytorch
 Author: Vladislav Sovrasov
 Author-email: sovrasov.vlad@gmail.com
 License: MIT
+Description: # Flops counting tool for neural networks in pytorch framework
+        [![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
+        [![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
+        
+        This script is designed to compute the theoretical amount of multiply-add operations
+        in convolutional neural networks. It can also compute the number of parameters and
+        print per-layer computational cost of a given network.
+        
+        Supported layers:
+        - Conv1d/2d/3d (including grouping)
+        - ConvTranspose1d/2d/3d (including grouping)
+        - BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d, LayerNorm
+        - Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
+        - Linear
+        - Upsample
+        - Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
+        
+        Experimental support:
+        - RNN, LSTM, GRU (NLH layout is assumed)
+        - RNNCell, LSTMCell, GRUCell
+        - MultiheadAttention
+        
+        Requirements: Pytorch >= 1.1, torchvision >= 0.3
+        
+        Thanks to @warmspringwinds for the initial version of script.
+        
+        ## Usage tips
+        
+        - This script doesn't take into account `torch.nn.functional.*` operations. For an instance, if one have a semantic segmentation model and use `torch.nn.functional.interpolate` to upscale features, these operations won't contribute to overall amount of flops. To avoid that one can use `torch.nn.Upsample` instead of `torch.nn.functional.interpolate`.
+        - `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
+        - `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
+        - `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
+        for research purposes. For an instance, one can drop all convolutuions from the counting process
+        specifying `ignore_modules=[torch.nn.Conv2d]`.
+        
+        ## Install the latest version
+        From PyPI:
+        ```bash
+        pip install ptflops
+        ```
+        
+        From this repository:
+        ```bash
+        pip install --upgrade git+https://github.com/sovrasov/flops-counter.pytorch.git
+        ```
+        
+        ## Example
+        ```python
+        import torchvision.models as models
+        import torch
+        from ptflops import get_model_complexity_info
+        
+        with torch.cuda.device(0):
+          net = models.densenet161()
+          macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
+                                                   print_per_layer_stat=True, verbose=True)
+          print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
+          print('{:<30}  {:<8}'.format('Number of parameters: ', params))
+        ```
+        
+        ## Citation
+        If ptflops was useful for your paper or tech report, please cite me:
+        ```
+        @online{ptflops,
+          author = {Vladislav Sovrasov},
+          title = {ptflops: a flops counting tool for neural networks in pytorch framework},
+          year = 2018-2023,
+          url = {https://github.com/sovrasov/flops-counter.pytorch},
+        }
+        ```
+        
+        ## Benchmark
+        
+        ### [torchvision](https://pytorch.org/docs/1.0.0/torchvision/models.html)
+        
+        Model         | Input Resolution | Params(M) | MACs(G) | Top-1 error | Top-5 error
+        ---           |---               |---        |---      |---          |---
+        alexnet       |224x224           | 61.1      | 0.72    | 43.45       | 20.91
+        vgg11         |224x224           | 132.86    | 7.63    | 30.98       | 11.37
+        vgg13         |224x224           | 133.05    | 11.34   | 30.07       | 10.75
+        vgg16         |224x224           | 138.36    | 15.5    | 28.41       | 9.62
+        vgg19         |224x224           | 143.67    | 19.67   | 27.62       | 9.12
+        vgg11_bn      |224x224           | 132.87    | 7.64    | 29.62       | 10.19
+        vgg13_bn      |224x224           | 133.05    | 11.36   | 28.45       | 9.63
+        vgg16_bn      |224x224           | 138.37    | 15.53   | 26.63       | 8.50
+        vgg19_bn      |224x224           | 143.68    | 19.7    | 25.76       | 8.15
+        resnet18      |224x224           | 11.69     | 1.82    | 30.24       | 10.92
+        resnet34      |224x224           | 21.8      | 3.68    | 26.70       | 8.58
+        resnet50      |224x224           | 25.56     | 4.12    | 23.85       | 7.13
+        resnet101     |224x224           | 44.55     | 7.85    | 22.63       | 6.44
+        resnet152     |224x224           | 60.19     | 11.58   | 21.69       | 5.94
+        squeezenet1_0 |224x224           | 1.25      | 0.83    | 41.90       | 19.58
+        squeezenet1_1 |224x224           | 1.24      | 0.36    | 41.81       | 19.38
+        densenet121   |224x224           | 7.98      | 2.88    | 25.35       | 7.83
+        densenet169   |224x224           | 14.15     | 3.42    | 24.00       | 7.00
+        densenet201   |224x224           | 20.01     | 4.37    | 22.80       | 6.43
+        densenet161   |224x224           | 28.68     | 7.82    | 22.35       | 6.20
+        inception_v3  |224x224           | 27.16     | 2.85    | 22.55       | 6.44
+        
+        * Top-1 error - ImageNet single-crop top-1 error (224x224)
+        * Top-5 error - ImageNet single-crop top-5 error (224x224)
+        
+        ### [Cadene/pretrained-models.pytorch](https://github.com/Cadene/pretrained-models.pytorch)
+        
+        Model               | Input Resolution | Params(M) | MACs(G)     | Acc@1       | Acc@5
+        ---                 |---               |---        |---          |---          |---
+        alexnet             | 224x224          | 61.1      | 0.72        | 56.432      | 79.194
+        bninception         | 224x224          | 11.3      | 2.05        | 73.524      | 91.562
+        cafferesnet101      | 224x224          | 44.55     | 7.62        | 76.2        | 92.766
+        densenet121         | 224x224          | 7.98      | 2.88        | 74.646      | 92.136
+        densenet161         | 224x224          | 28.68     | 7.82        | 77.56       | 93.798
+        densenet169         | 224x224          | 14.15     | 3.42        | 76.026      | 92.992
+        densenet201         | 224x224          | 20.01     | 4.37        | 77.152      | 93.548
+        dpn107              | 224x224          | 86.92     | 18.42       | 79.746      | 94.684
+        dpn131              | 224x224          | 79.25     | 16.13       | 79.432      | 94.574
+        dpn68               | 224x224          | 12.61     | 2.36        | 75.868      | 92.774
+        dpn68b              | 224x224          | 12.61     | 2.36        | 77.034      | 93.59
+        dpn92               | 224x224          | 37.67     | 6.56        | 79.4        | 94.62
+        dpn98               | 224x224          | 61.57     | 11.76       | 79.224      | 94.488
+        fbresnet152         | 224x224          | 60.27     | 11.6        | 77.386      | 93.594
+        inceptionresnetv2   | 299x299          | 55.84     | 13.22       | 80.17       | 95.234
+        inceptionv3         | 299x299          | 27.16     | 5.73        | 77.294      | 93.454
+        inceptionv4         | 299x299          | 42.68     | 12.31       | 80.062      | 94.926
+        nasnetalarge        | 331x331          | 88.75     | 24.04       | 82.566      | 96.086
+        nasnetamobile       | 224x224          | 5.29      | 0.59        | 74.08       | 91.74
+        pnasnet5large       | 331x331          | 86.06     | 25.21       | 82.736      | 95.992
+        polynet             | 331x331          | 95.37     | 34.9        | 81.002      | 95.624
+        resnet101           | 224x224          | 44.55     | 7.85        | 77.438      | 93.672
+        resnet152           | 224x224          | 60.19     | 11.58       | 78.428      | 94.11
+        resnet18            | 224x224          | 11.69     | 1.82        | 70.142      | 89.274
+        resnet34            | 224x224          | 21.8      | 3.68        | 73.554      | 91.456
+        resnet50            | 224x224          | 25.56     | 4.12        | 76.002      | 92.98
+        resnext101_32x4d    | 224x224          | 44.18     | 8.03        | 78.188      | 93.886
+        resnext101_64x4d    | 224x224          | 83.46     | 15.55       | 78.956      | 94.252
+        se_resnet101        | 224x224          | 49.33     | 7.63        | 78.396      | 94.258
+        se_resnet152        | 224x224          | 66.82     | 11.37       | 78.658      | 94.374
+        se_resnet50         | 224x224          | 28.09     | 3.9         | 77.636      | 93.752
+        se_resnext101_32x4d | 224x224          | 48.96     | 8.05        | 80.236      | 95.028
+        se_resnext50_32x4d  | 224x224          | 27.56     | 4.28        | 79.076      | 94.434
+        senet154            | 224x224          | 115.09    | 20.82       | 81.304      | 95.498
+        squeezenet1_0       | 224x224          | 1.25      | 0.83        | 58.108      | 80.428
+        squeezenet1_1       | 224x224          | 1.24      | 0.36        | 58.25       | 80.8
+        vgg11               | 224x224          | 132.86    | 7.63        | 68.97       | 88.746
+        vgg11_bn            | 224x224          | 132.87    | 7.64        | 70.452      | 89.818
+        vgg13               | 224x224          | 133.05    | 11.34       | 69.662      | 89.264
+        vgg13_bn            | 224x224          | 133.05    | 11.36       | 71.508      | 90.494
+        vgg16               | 224x224          | 138.36    | 15.5        | 71.636      | 90.354
+        vgg16_bn            | 224x224          | 138.37    | 15.53       | 73.518      | 91.608
+        vgg19               | 224x224          | 143.67    | 19.67       | 72.08       | 90.822
+        vgg19_bn            | 224x224          | 143.68    | 19.7        | 74.266      | 92.066
+        xception            | 299x299          | 22.86     | 8.42        | 78.888      | 94.292
+        
+        * Acc@1 - ImageNet single-crop top-1 accuracy on validation images of the same size used during the training process.
+        * Acc@5 - ImageNet single-crop top-5 accuracy on validation images of the same size used during the training process.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Flops counter for convolutional networks in pytorch framework
-[![Pypi version](https://img.shields.io/pypi/v/ptflops.svg)](https://pypi.org/project/ptflops/)
-[![Build Status](https://travis-ci.com/sovrasov/flops-counter.pytorch.svg?branch=master)](https://travis-ci.com/sovrasov/flops-counter.pytorch)
-
-This script is designed to compute the theoretical amount of multiply-add operations
-in convolutional neural networks. It can also compute the number of parameters and
-print per-layer computational cost of a given network.
-
-Supported layers:
-- Conv1d/2d/3d (including grouping)
-- ConvTranspose1d/2d/3d (including grouping)
-- BatchNorm1d/2d/3d, GroupNorm, InstanceNorm1d/2d/3d
-- Activations (ReLU, PReLU, ELU, ReLU6, LeakyReLU, GELU)
-- Linear
-- Upsample
-- Poolings (AvgPool1d/2d/3d, MaxPool1d/2d/3d and adaptive ones)
-
-Experimental support:
-- RNN, LSTM, GRU (NLH layout is assumed)
-- RNNCell, LSTMCell, GRUCell
-- MultiheadAttention
-
-Requirements: Pytorch >= 1.1, torchvision >= 0.3
-
-Thanks to @warmspringwinds for the initial version of script.
-
-## Usage tips
-
-- This script doesn't take into account `torch.nn.functional.*` operations. For an instance, if one have a semantic segmentation model and use `torch.nn.functional.interpolate` to upscale features, these operations won't contribute to overall amount of flops. To avoid that one can use `torch.nn.Upsample` instead of `torch.nn.functional.interpolate`.
-- `ptflops` launches a given model on a random tensor and estimates amount of computations during inference. Complicated models can have several inputs, some of them could be optional. To construct non-trivial input one can use the `input_constructor` argument of the `get_model_complexity_info`. `input_constructor` is a function that takes the input spatial resolution as a tuple and returns a dict with named input arguments of the model. Next this dict would be passed to the model as a keyword arguments.
-- `verbose` parameter allows to get information about modules that don't contribute to the final numbers.
-- `ignore_modules` option forces `ptflops` to ignore the listed modules. This can be useful
-for research purposes. For an instance, one can drop all convolutuions from the counting process
-specifying `ignore_modules=[torch.nn.Conv2d]`.
-
-## Install the latest version
-From PyPI:
-```bash
-pip install ptflops
-```
-
-From this repository:
-```bash
-pip install --upgrade git+https://github.com/sovrasov/flops-counter.pytorch.git
-```
-
-## Example
-```python
-import torchvision.models as models
-import torch
-from ptflops import get_model_complexity_info
-
-with torch.cuda.device(0):
-  net = models.densenet161()
-  macs, params = get_model_complexity_info(net, (3, 224, 224), as_strings=True,
-                                           print_per_layer_stat=True, verbose=True)
-  print('{:<30}  {:<8}'.format('Computational complexity: ', macs))
-  print('{:<30}  {:<8}'.format('Number of parameters: ', params))
-```
-
-## Benchmark
-
-### [torchvision](https://pytorch.org/docs/1.0.0/torchvision/models.html)
-
-Model         | Input Resolution | Params(M) | MACs(G) | Top-1 error | Top-5 error
----           |---               |---        |---      |---          |---
-alexnet       |224x224           | 61.1      | 0.72    | 43.45       | 20.91
-vgg11         |224x224           | 132.86    | 7.63    | 30.98       | 11.37
-vgg13         |224x224           | 133.05    | 11.34   | 30.07       | 10.75
-vgg16         |224x224           | 138.36    | 15.5    | 28.41       | 9.62
-vgg19         |224x224           | 143.67    | 19.67   | 27.62       | 9.12
-vgg11_bn      |224x224           | 132.87    | 7.64    | 29.62       | 10.19
-vgg13_bn      |224x224           | 133.05    | 11.36   | 28.45       | 9.63
-vgg16_bn      |224x224           | 138.37    | 15.53   | 26.63       | 8.50
-vgg19_bn      |224x224           | 143.68    | 19.7    | 25.76       | 8.15
-resnet18      |224x224           | 11.69     | 1.82    | 30.24       | 10.92
-resnet34      |224x224           | 21.8      | 3.68    | 26.70       | 8.58
-resnet50      |224x224           | 25.56     | 4.12    | 23.85       | 7.13
-resnet101     |224x224           | 44.55     | 7.85    | 22.63       | 6.44
-resnet152     |224x224           | 60.19     | 11.58   | 21.69       | 5.94
-squeezenet1_0 |224x224           | 1.25      | 0.83    | 41.90       | 19.58
-squeezenet1_1 |224x224           | 1.24      | 0.36    | 41.81       | 19.38
-densenet121   |224x224           | 7.98      | 2.88    | 25.35       | 7.83
-densenet169   |224x224           | 14.15     | 3.42    | 24.00       | 7.00
-densenet201   |224x224           | 20.01     | 4.37    | 22.80       | 6.43
-densenet161   |224x224           | 28.68     | 7.82    | 22.35       | 6.20
-inception_v3  |224x224           | 27.16     | 2.85    | 22.55       | 6.44
-
-* Top-1 error - ImageNet single-crop top-1 error (224x224)
-* Top-5 error - ImageNet single-crop top-5 error (224x224)
-
-### [Cadene/pretrained-models.pytorch](https://github.com/Cadene/pretrained-models.pytorch)
-
-Model               | Input Resolution | Params(M) | MACs(G)     | Acc@1       | Acc@5
----                 |---               |---        |---          |---          |---
-alexnet             | 224x224          | 61.1      | 0.72        | 56.432      | 79.194
-bninception         | 224x224          | 11.3      | 2.05        | 73.524      | 91.562
-cafferesnet101      | 224x224          | 44.55     | 7.62        | 76.2        | 92.766
-densenet121         | 224x224          | 7.98      | 2.88        | 74.646      | 92.136
-densenet161         | 224x224          | 28.68     | 7.82        | 77.56       | 93.798
-densenet169         | 224x224          | 14.15     | 3.42        | 76.026      | 92.992
-densenet201         | 224x224          | 20.01     | 4.37        | 77.152      | 93.548
-dpn107              | 224x224          | 86.92     | 18.42       | 79.746      | 94.684
-dpn131              | 224x224          | 79.25     | 16.13       | 79.432      | 94.574
-dpn68               | 224x224          | 12.61     | 2.36        | 75.868      | 92.774
-dpn68b              | 224x224          | 12.61     | 2.36        | 77.034      | 93.59
-dpn92               | 224x224          | 37.67     | 6.56        | 79.4        | 94.62
-dpn98               | 224x224          | 61.57     | 11.76       | 79.224      | 94.488
-fbresnet152         | 224x224          | 60.27     | 11.6        | 77.386      | 93.594
-inceptionresnetv2   | 299x299          | 55.84     | 13.22       | 80.17       | 95.234
-inceptionv3         | 299x299          | 27.16     | 5.73        | 77.294      | 93.454
-inceptionv4         | 299x299          | 42.68     | 12.31       | 80.062      | 94.926
-nasnetalarge        | 331x331          | 88.75     | 24.04       | 82.566      | 96.086
-nasnetamobile       | 224x224          | 5.29      | 0.59        | 74.08       | 91.74
-pnasnet5large       | 331x331          | 86.06     | 25.21       | 82.736      | 95.992
-polynet             | 331x331          | 95.37     | 34.9        | 81.002      | 95.624
-resnet101           | 224x224          | 44.55     | 7.85        | 77.438      | 93.672
-resnet152           | 224x224          | 60.19     | 11.58       | 78.428      | 94.11
-resnet18            | 224x224          | 11.69     | 1.82        | 70.142      | 89.274
-resnet34            | 224x224          | 21.8      | 3.68        | 73.554      | 91.456
-resnet50            | 224x224          | 25.56     | 4.12        | 76.002      | 92.98
-resnext101_32x4d    | 224x224          | 44.18     | 8.03        | 78.188      | 93.886
-resnext101_64x4d    | 224x224          | 83.46     | 15.55       | 78.956      | 94.252
-se_resnet101        | 224x224          | 49.33     | 7.63        | 78.396      | 94.258
-se_resnet152        | 224x224          | 66.82     | 11.37       | 78.658      | 94.374
-se_resnet50         | 224x224          | 28.09     | 3.9         | 77.636      | 93.752
-se_resnext101_32x4d | 224x224          | 48.96     | 8.05        | 80.236      | 95.028
-se_resnext50_32x4d  | 224x224          | 27.56     | 4.28        | 79.076      | 94.434
-senet154            | 224x224          | 115.09    | 20.82       | 81.304      | 95.498
-squeezenet1_0       | 224x224          | 1.25      | 0.83        | 58.108      | 80.428
-squeezenet1_1       | 224x224          | 1.24      | 0.36        | 58.25       | 80.8
-vgg11               | 224x224          | 132.86    | 7.63        | 68.97       | 88.746
-vgg11_bn            | 224x224          | 132.87    | 7.64        | 70.452      | 89.818
-vgg13               | 224x224          | 133.05    | 11.34       | 69.662      | 89.264
-vgg13_bn            | 224x224          | 133.05    | 11.36       | 71.508      | 90.494
-vgg16               | 224x224          | 138.36    | 15.5        | 71.636      | 90.354
-vgg16_bn            | 224x224          | 138.37    | 15.53       | 73.518      | 91.608
-vgg19               | 224x224          | 143.67    | 19.67       | 72.08       | 90.822
-vgg19_bn            | 224x224          | 143.68    | 19.7        | 74.266      | 92.066
-xception            | 299x299          | 22.86     | 8.42        | 78.888      | 94.292
-
-* Acc@1 - ImageNet single-crop top-1 accuracy on validation images of the same size used during the training process.
-* Acc@5 - ImageNet single-crop top-5 accuracy on validation images of the same size used during the training process.
-
-
```

### Comparing `ptflops-0.6.9/setup.py` & `ptflops-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 readme = open('README.md').read()
 
-VERSION = '0.6.9'
+VERSION = '0.7'
 
 requirements = [
     'torch',
 ]
 
 setup(
     # Metadata
```

