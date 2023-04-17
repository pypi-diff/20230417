# Comparing `tmp/tabpfn-0.1.8.tar.gz` & `tmp/tabpfn-0.1.9.tar.gz`

## Comparing `tabpfn-0.1.8.tar` & `tabpfn-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 tabpfn-0.1.8/how_to_put_on_pypi.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tabpfn-0.1.8/requirements.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tabpfn-0.1.8/setup.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tabpfn-0.1.8/test.py
--rw-r--r--   0        0        0    10329 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/PrepareDatasets.ipynb
--rw-r--r--   0        0        0    76754 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/PriorFittingCustomPrior.ipynb
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/QuickPredictionDemo.ipynb
--rw-r--r--   0        0        0    32675 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/RunFullDatasetAnalyses.ipynb
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/decoders.py
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/encoders.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/initializers.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/layer.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/losses.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/model_configs.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/notebook_utils.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/positional_encodings.py
--rw-r--r--   0        0        0    17756 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/train.py
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/transformer.py
--rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/utils.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/datasets/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/datasets/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/__init__.py
--rw-r--r--   0        0        0    19627 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/differentiable_prior.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/fast_gp.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/flexible_categorical.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/mlp.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/prior.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/prior_bag.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/priors/utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/baseline_prediction_interface.py
--rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/decision_boundary.py
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/differentiable_pfn_evaluation.py
--rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/model_builder.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/model_configs.py
--rw-r--r--   0        0        0    54761 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/tabular_baselines.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/tabular_baselines_deep.py
--rw-r--r--   0        0        0    14268 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/tabular_evaluation.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/tabular_metrics.py
--rw-r--r--   0        0        0    21958 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/scripts/transformer_prediction_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/tests/__init__.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/tests/test_deterministic_and_model_caching.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/tests/test_follow_sklearn_interface.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 tabpfn-0.1.8/tabpfn/tests/test_load_module_only_inference.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tabpfn-0.1.8/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 tabpfn-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tabpfn-0.1.8/NOTICE.txt
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 tabpfn-0.1.8/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 tabpfn-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 tabpfn-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tabpfn-0.1.9/CITATION.bib
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 tabpfn-0.1.9/how_to_put_on_pypi.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tabpfn-0.1.9/requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tabpfn-0.1.9/setup.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tabpfn-0.1.9/test.py
+-rw-r--r--   0        0        0    10329 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/PrepareDatasets.ipynb
+-rw-r--r--   0        0        0    76754 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/PriorFittingCustomPrior.ipynb
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/QuickPredictionDemo.ipynb
+-rw-r--r--   0        0        0    32675 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/RunFullDatasetAnalyses.ipynb
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/decoders.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/encoders.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/initializers.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/layer.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/losses.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/model_configs.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/notebook_utils.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/positional_encodings.py
+-rw-r--r--   0        0        0    17756 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/train.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/transformer.py
+-rw-r--r--   0        0        0    13052 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/utils.py
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/datasets/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/datasets/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/__init__.py
+-rw-r--r--   0        0        0    19627 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/differentiable_prior.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/fast_gp.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/flexible_categorical.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/mlp.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/prior.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/prior_bag.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/priors/utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/baseline_prediction_interface.py
+-rw-r--r--   0        0        0    11913 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/decision_boundary.py
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/differentiable_pfn_evaluation.py
+-rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/model_builder.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/model_configs.py
+-rw-r--r--   0        0        0    54761 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/tabular_baselines.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/tabular_baselines_deep.py
+-rw-r--r--   0        0        0    14268 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/tabular_evaluation.py
+-rw-r--r--   0        0        0     9527 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/tabular_metrics.py
+-rw-r--r--   0        0        0    25719 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/scripts/transformer_prediction_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/test_deterministic_and_model_caching.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/test_follow_sklearn_interface.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/test_get_gradients.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/test_load_module_only_inference.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 tabpfn-0.1.9/tabpfn/tests/test_standardization.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 tabpfn-0.1.9/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 tabpfn-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tabpfn-0.1.9/NOTICE.txt
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tabpfn-0.1.9/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 tabpfn-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 tabpfn-0.1.9/PKG-INFO
```

### Comparing `tabpfn-0.1.8/how_to_put_on_pypi.md` & `tabpfn-0.1.9/how_to_put_on_pypi.md`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/test.py` & `tabpfn-0.1.9/test.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/PrepareDatasets.ipynb` & `tabpfn-0.1.9/tabpfn/PrepareDatasets.ipynb`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/PriorFittingCustomPrior.ipynb` & `tabpfn-0.1.9/tabpfn/PriorFittingCustomPrior.ipynb`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/QuickPredictionDemo.ipynb` & `tabpfn-0.1.9/tabpfn/QuickPredictionDemo.ipynb`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/RunFullDatasetAnalyses.ipynb` & `tabpfn-0.1.9/tabpfn/RunFullDatasetAnalyses.ipynb`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/decoders.py` & `tabpfn-0.1.9/tabpfn/decoders.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/encoders.py` & `tabpfn-0.1.9/tabpfn/encoders.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/layer.py` & `tabpfn-0.1.9/tabpfn/layer.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/losses.py` & `tabpfn-0.1.9/tabpfn/losses.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/model_configs.py` & `tabpfn-0.1.9/tabpfn/model_configs.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/notebook_utils.py` & `tabpfn-0.1.9/tabpfn/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/positional_encodings.py` & `tabpfn-0.1.9/tabpfn/positional_encodings.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class NoPositionalEncoding(nn.Module):
     def __init__(self, d_model, max_len=None):
         super(NoPositionalEncoding, self).__init__()
         pass
 
     def forward(self, x):
-        return x #* math.sqrt(x.shape[-1])
+        return x
 
 
 class PositionalEncoding(nn.Module):
     def __init__(self, d_model, max_len=5000):
         super(PositionalEncoding, self).__init__()
         pe = torch.zeros(max_len, d_model)
         position = torch.arange(0, max_len, dtype=torch.float).unsqueeze(1)
```

### Comparing `tabpfn-0.1.8/tabpfn/train.py` & `tabpfn-0.1.9/tabpfn/train.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/transformer.py` & `tabpfn-0.1.9/tabpfn/transformer.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/utils.py` & `tabpfn-0.1.9/tabpfn/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import random
 import datetime
 import itertools
 
 import torch
 from torch import nn
 from torch.optim.lr_scheduler import LambdaLR
-import numpy as np
 
 # copied from huggingface
 def get_cosine_schedule_with_warmup(optimizer, num_warmup_steps, num_training_steps, num_cycles=0.5, last_epoch=-1):
     """ Create a schedule with a learning rate that decreases following the
     values of the cosine function between 0 and `pi * cycles` after a warmup
     period during which it increases linearly between 0 and 1.
     """
@@ -168,53 +167,69 @@
 
 def nan_handling_missing_for_no_reason_value(set_value_to_nan=0.0):
     return get_nan_value(float('-inf'), set_value_to_nan)
 
 def nan_handling_missing_for_a_reason_value(set_value_to_nan=0.0):
     return get_nan_value(float('inf'), set_value_to_nan)
 
-def torch_nanmean(x, axis=0, return_nanshare=False):
-    num = torch.where(torch.isnan(x), torch.full_like(x, 0), torch.full_like(x, 1)).sum(axis=axis)
-    value = torch.where(torch.isnan(x), torch.full_like(x, 0), x).sum(axis=axis)
-    if return_nanshare:
-        return value / num, 1.-num/x.shape[axis]
+def torch_masked_mean(x, mask, dim=0, return_share_of_ignored_values=False):
+    """
+    Returns the mean of a torch tensor and only considers the elements, where the mask is true.
+    If return_share_of_ignored_values is true it returns a second tensor with the percentage of ignored values
+    because of the mask.
+    """
+    num = torch.where(mask, torch.full_like(x, 1), torch.full_like(x, 0)).sum(dim=dim)
+    value = torch.where(mask, x, torch.full_like(x, 0)).sum(dim=dim)
+    if return_share_of_ignored_values:
+        return value / num, 1.-num/x.shape[dim]
     return value / num
 
-def torch_nanstd(x, axis=0):
-    num = torch.where(torch.isnan(x), torch.full_like(x, 0), torch.full_like(x, 1)).sum(axis=axis)
-    value = torch.where(torch.isnan(x), torch.full_like(x, 0), x).sum(axis=axis)
+def torch_masked_std(x, mask, dim=0):
+    """
+    Returns the std of a torch tensor and only considers the elements, where the mask is true.
+    If get_mean is true it returns as a first Tensor the mean and as a second tensor the std.
+    """
+    num = torch.where(mask, torch.full_like(x, 1), torch.full_like(x, 0)).sum(dim=dim)
+    value = torch.where(mask, x, torch.full_like(x, 0)).sum(dim=dim)
     mean = value / num
-    mean_broadcast = torch.repeat_interleave(mean.unsqueeze(axis), x.shape[axis], dim=axis)
-    return torch.sqrt(torch.nansum(torch.square(mean_broadcast - x), axis=axis) / (num - 1))
+    mean_broadcast = torch.repeat_interleave(mean.unsqueeze(dim), x.shape[dim], dim=dim)
+    quadratic_difference_from_mean = torch.square(torch.where(mask, mean_broadcast - x, torch.full_like(x, 0)))
+    return torch.sqrt(torch.sum(quadratic_difference_from_mean, dim=dim) / (num - 1))
+
+def torch_nanmean(x, dim=0, return_nanshare=False):
+    return torch_masked_mean(x, ~torch.isnan(x), dim=dim, return_share_of_ignored_values=return_nanshare)
+
+def torch_nanstd(x, dim=0):
+    return torch_masked_std(x, ~torch.isnan(x), dim=dim)
 
 def normalize_data(data, normalize_positions=-1):
     if normalize_positions > 0:
-        mean = torch_nanmean(data[:normalize_positions], axis=0)
-        std = torch_nanstd(data[:normalize_positions], axis=0) + .000001
+        mean = torch_nanmean(data[:normalize_positions], dim=0)
+        std = torch_nanstd(data[:normalize_positions], dim=0) + .000001
     else:
-        mean = torch_nanmean(data, axis=0)
-        std = torch_nanstd(data, axis=0) + .000001
+        mean = torch_nanmean(data, dim=0)
+        std = torch_nanstd(data, dim=0) + .000001
     data = (data - mean) / std
     data = torch.clip(data, min=-100, max=100)
 
     return data
 
 def remove_outliers(X, n_sigma=4, normalize_positions=-1):
     # Expects T, B, H
     assert len(X.shape) == 3, "X must be T,B,H"
-    #for b in range(X.shape[1]):
-        #for col in range(X.shape[2]):
+
     data = X if normalize_positions == -1 else X[:normalize_positions]
-    data_clean = data[:].clone()
-    data_mean, data_std = torch_nanmean(data, axis=0), torch_nanstd(data, axis=0)
+
+    data_mean, data_std = torch_nanmean(data, dim=0), torch_nanstd(data, dim=0)
     cut_off = data_std * n_sigma
     lower, upper = data_mean - cut_off, data_mean + cut_off
 
-    data_clean[torch.logical_or(data_clean > upper, data_clean < lower)] = np.nan
-    data_mean, data_std = torch_nanmean(data_clean, axis=0), torch_nanstd(data_clean, axis=0)
+    mask = (data <= upper) & (data >= lower) & ~torch.isnan(data)
+    data_mean, data_std = torch_masked_mean(data, mask), torch_masked_std(data, mask)
+
     cut_off = data_std * n_sigma
     lower, upper = data_mean - cut_off, data_mean + cut_off
 
     X = torch.maximum(-torch.log(1+torch.abs(X)) + lower, X)
     X = torch.minimum(torch.log(1+torch.abs(X)) + upper, X)
             # print(ds[1][data < lower, col], ds[1][data > upper, col], ds[1][~np.isnan(data), col].shape, data_mean, data_std)
     return X
```

### Comparing `tabpfn-0.1.8/tabpfn/datasets/__init__.py` & `tabpfn-0.1.9/tabpfn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/differentiable_prior.py` & `tabpfn-0.1.9/tabpfn/priors/differentiable_prior.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/fast_gp.py` & `tabpfn-0.1.9/tabpfn/priors/fast_gp.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/flexible_categorical.py` & `tabpfn-0.1.9/tabpfn/priors/flexible_categorical.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/mlp.py` & `tabpfn-0.1.9/tabpfn/priors/mlp.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/prior_bag.py` & `tabpfn-0.1.9/tabpfn/priors/prior_bag.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/priors/utils.py` & `tabpfn-0.1.9/tabpfn/priors/utils.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/baseline_prediction_interface.py` & `tabpfn-0.1.9/tabpfn/scripts/baseline_prediction_interface.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/decision_boundary.py` & `tabpfn-0.1.9/tabpfn/scripts/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/differentiable_pfn_evaluation.py` & `tabpfn-0.1.9/tabpfn/scripts/differentiable_pfn_evaluation.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/model_builder.py` & `tabpfn-0.1.9/tabpfn/scripts/model_builder.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/model_configs.py` & `tabpfn-0.1.9/tabpfn/scripts/model_configs.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/tabular_baselines.py` & `tabpfn-0.1.9/tabpfn/scripts/tabular_baselines.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/tabular_baselines_deep.py` & `tabpfn-0.1.9/tabpfn/scripts/tabular_baselines_deep.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/tabular_evaluation.py` & `tabpfn-0.1.9/tabpfn/scripts/tabular_evaluation.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/scripts/tabular_metrics.py` & `tabpfn-0.1.9/tabpfn/scripts/tabular_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     pred = torch.tensor(pred) if not torch.is_tensor(pred) else pred
     return torch.tensor(neg_r2(target, pred))
 
 def neg_r2(target, pred):
     return -r2_score(pred.float(), target.float())
 
 def is_classification(metric_used):
-    if metric_used == auc_metric or metric_used == cross_entropy:
+    if metric_used.__name__ in ["auc_metric", "cross_entropy"]:
         return True
     return False
 
 def time_metric():
     """
     Dummy function, will just be used as a handler.
     """
```

### Comparing `tabpfn-0.1.8/tabpfn/scripts/transformer_prediction_interface.py` & `tabpfn-0.1.9/tabpfn/scripts/transformer_prediction_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import numpy as np
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from sklearn.utils.multiclass import unique_labels
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils import column_or_1d
+from sklearn.preprocessing import LabelEncoder
 from pathlib import Path
 from tabpfn.scripts.model_builder import load_model, load_model_only_inference
 import os
 import pickle
 import io
 
 class CustomUnpickler(pickle.Unpickler):
@@ -102,16 +103,48 @@
 
 
 class TabPFNClassifier(BaseEstimator, ClassifierMixin):
 
     models_in_memory = {}
 
     def __init__(self, device='cpu', base_path=pathlib.Path(__file__).parent.parent.resolve(), model_string='',
-                 N_ensemble_configurations=3, combine_preprocessing=False, no_preprocess_mode=False,
-                 multiclass_decoder='permutation', feature_shift_decoder=True, only_inference=True, seed=0):
+                 N_ensemble_configurations=3, no_preprocess_mode=False, multiclass_decoder='permutation',
+                 feature_shift_decoder=True, only_inference=True, seed=0, no_grad=True, batch_size_inference=32):
+        """
+        Initializes the classifier and loads the model. 
+        Depending on the arguments, the model is either loaded from memory, from a file, or downloaded from the 
+        repository if no model is found.
+        
+        Can also be used to compute gradients with respect to the inputs X_train and X_test. Therefore no_grad has to be 
+        set to False and no_preprocessing_mode must be True. Furthermore, X_train and X_test need to be given as 
+        torch.Tensors and their requires_grad parameter must be set to True.
+        
+        
+        :param device: If the model should run on cuda or cpu.
+        :param base_path: Base path of the directory, from which the folders like models_diff can be accessed.
+        :param model_string: Name of the model. Used first to check if the model is already in memory, and if not, 
+               tries to load a model with that name from the models_diff directory. It looks for files named as 
+               follows: "prior_diff_real_checkpoint" + model_string + "_n_0_epoch_e.cpkt", where e can be a number 
+               between 100 and 0, and is checked in a descending order. 
+        :param N_ensemble_configurations: The number of ensemble configurations used for the prediction. Thereby the 
+               accuracy, but also the running time, increases with this number. 
+        :param no_preprocess_mode: Specifies whether preprocessing is to be performed.
+        :param multiclass_decoder: If set to permutation, randomly shifts the classes for each ensemble configuration. 
+        :param feature_shift_decoder: If set to true shifts the features for each ensemble configuration according to a 
+               random permutation.
+        :param only_inference: Indicates if the model should be loaded to only restore inference capabilities or also 
+               training capabilities. Note that the training capabilities are currently not being fully restored.
+        :param seed: Seed that is used for the prediction. Allows for a deterministic behavior of the predictions.
+        :param batch_size_inference: This parameter is a trade-off between performance and memory consumption.
+               The computation done with different values for batch_size_inference is the same,
+               but it is split into smaller/larger batches.
+        :param no_grad: If set to false, allows for the computation of gradients with respect to X_train and X_test. 
+               For this to correctly function no_preprocessing_mode must be set to true.
+        """
+
         # Model file specification (Model name, Epoch)
         i = 0
         model_key = model_string+'|'+str(device)
         if model_string in self.models_in_memory:
             model, c, results_file = self.models_in_memory[model_key]
         else:
             model, c, results_file = load_model_workflow(i, -1, add_name=model_string, base_path=base_path, device=device,
@@ -133,19 +166,24 @@
         self.model_string = model_string
 
         self.max_num_features = self.c['num_features']
         self.max_num_classes = self.c['max_num_classes']
         self.differentiable_hps_as_style = self.c['differentiable_hps_as_style']
 
         self.no_preprocess_mode = no_preprocess_mode
-        self.combine_preprocessing = combine_preprocessing
         self.feature_shift_decoder = feature_shift_decoder
         self.multiclass_decoder = multiclass_decoder
         self.only_inference = only_inference
         self.seed = seed
+        self.no_grad = no_grad
+
+        assert self.no_preprocess_mode if not self.no_grad else True, \
+            "If no_grad is false, no_preprocess_mode must be true, because otherwise no gradient can be computed."
+
+        self.batch_size_inference = batch_size_inference
 
     def remove_models_from_memory(self):
         self.models_in_memory = {}
 
     def load_result_minimal(self, path, i, e):
         with open(path, 'rb') as output:
             _, _, _, style, temperature, optimization_route = CustomUnpickler(output).load()
@@ -163,63 +201,91 @@
             )
 
         self.classes_ = cls
 
         return np.asarray(y, dtype=np.float64, order="C")
 
     def fit(self, X, y, overwrite_warning=False):
-        # Check that X and y have correct shape
-        X, y = check_X_y(X, y, force_all_finite=False)
+        """
+        Validates the training set and stores it.
+
+        If clf.no_grad (default is True):
+        X, y should be of type np.array
+        else:
+        X should be of type torch.Tensors (y can be np.array or torch.Tensor)
+        """
+        if self.no_grad:
+            # Check that X and y have correct shape
+            X, y = check_X_y(X, y, force_all_finite=False)
         # Store the classes seen during fit
         y = self._validate_targets(y)
+        self.label_encoder = LabelEncoder()
+        y = self.label_encoder.fit_transform(y)
 
         self.X_ = X
         self.y_ = y
 
         if X.shape[1] > self.max_num_features:
             raise ValueError("The number of features for this classifier is restricted to ", self.max_num_features)
         if len(np.unique(y)) > self.max_num_classes:
             raise ValueError("The number of classes for this classifier is restricted to ", self.max_num_classes)
         if X.shape[0] > 1024 and not overwrite_warning:
             raise ValueError("⚠️ WARNING: TabPFN is not made for datasets with a trainingsize > 1024. Prediction might take a while, be less reliable. We advise not to run datasets > 10k samples, which might lead to your machine crashing (due to quadratic memory scaling of TabPFN). Please confirm you want to run by passing overwrite_warning=True to the fit function.")
-            
+
 
         # Return the classifier
         return self
 
-    def predict_proba(self, X, normalize_with_test=False):
+    def predict_proba(self, X, normalize_with_test=False, return_logits=False):
+        """
+        Predict the probabilities for the input X depending on the training set previously passed in the method fit.
+
+        If no_grad is true in the classifier the function takes X as a numpy.ndarray. If no_grad is false X must be a
+        torch tensor and is not fully checked.
+        """
         # Check is fit had been called
         check_is_fitted(self)
 
         # Input validation
-        X = check_array(X, force_all_finite=False)
-        X_full = np.concatenate([self.X_, X], axis=0)
-        X_full = torch.tensor(X_full, device=self.device).float().unsqueeze(1)
-        y_full = np.concatenate([self.y_, np.zeros_like(X[:, 0])], axis=0)
+        if self.no_grad:
+            X = check_array(X, force_all_finite=False)
+            X_full = np.concatenate([self.X_, X], axis=0)
+            X_full = torch.tensor(X_full, device=self.device).float().unsqueeze(1)
+        else:
+            assert (torch.is_tensor(self.X_) & torch.is_tensor(X)), "If no_grad is false, this function expects X as " \
+                                                                    "a tensor to calculate a gradient"
+            X_full = torch.cat((self.X_, X), dim=0).float().unsqueeze(1).to(self.device)
+
+            if int(torch.isnan(X_full).sum()):
+                print('X contains nans and the gradient implementation is not designed to handel nans.')
+
+        y_full = np.concatenate([self.y_, np.zeros(shape=X.shape[0])], axis=0)
         y_full = torch.tensor(y_full, device=self.device).float().unsqueeze(1)
 
         eval_pos = self.X_.shape[0]
 
         prediction = transformer_predict(self.model[2], X_full, y_full, eval_pos,
                                          device=self.device,
                                          style=self.style,
                                          inference_mode=True,
                                          preprocess_transform='none' if self.no_preprocess_mode else 'mix',
                                          normalize_with_test=normalize_with_test,
                                          N_ensemble_configurations=self.N_ensemble_configurations,
                                          softmax_temperature=self.temperature,
-                                         combine_preprocessing=self.combine_preprocessing,
                                          multiclass_decoder=self.multiclass_decoder,
                                          feature_shift_decoder=self.feature_shift_decoder,
                                          differentiable_hps_as_style=self.differentiable_hps_as_style,
                                          seed=self.seed,
+                                         return_logits=return_logits,
+                                         no_grad=self.no_grad,
+                                         batch_size_inference=self.batch_size_inference,
                                          **get_params_from_config(self.c))
         prediction_, y_ = prediction.squeeze(0), y_full.squeeze(1).long()[eval_pos:]
 
-        return prediction_.detach().cpu().numpy()
+        return prediction_.detach().cpu().numpy() if self.no_grad else prediction_
 
     def predict(self, X, return_winning_probability=False, normalize_with_test=False):
         p = self.predict_proba(X, normalize_with_test=normalize_with_test)
         y = np.argmax(p, axis=-1)
         y = self.classes_.take(np.asarray(y, dtype=np.intp))
         if return_winning_probability:
             return y, p.max(axis=-1)
@@ -237,21 +303,22 @@
                         normalize_to_ranking=False,
                         softmax_temperature=0.0,
                         multiclass_decoder='permutation',
                         preprocess_transform='mix',
                         categorical_feats=[],
                         feature_shift_decoder=False,
                         N_ensemble_configurations=10,
-                        combine_preprocessing=False,
                         batch_size_inference=16,
                         differentiable_hps_as_style=False,
                         average_logits=True,
                         fp16_inference=False,
                         normalize_with_sqrt=False,
                         seed=0,
+                        no_grad=True,
+                        return_logits=False,
                         **kwargs):
     """
 
     :param model:
     :param eval_xs:
     :param eval_ys:
     :param eval_position:
@@ -275,15 +342,16 @@
     :return:
     """
     num_classes = len(torch.unique(eval_ys))
 
     def predict(eval_xs, eval_ys, used_style, softmax_temperature, return_logits):
         # Initialize results array size S, B, Classes
 
-        inference_mode_call = torch.inference_mode() if inference_mode else NOP()
+        # no_grad disables inference_mode, because otherwise the gradients are lost
+        inference_mode_call = torch.inference_mode() if inference_mode and no_grad else NOP()
         with inference_mode_call:
             start = time.time()
             output = model(
                     (used_style.repeat(eval_xs.shape[1], 1) if used_style is not None else None, eval_xs, eval_ys.float()),
                     single_eval_pos=eval_position)[:, :, 0:num_classes]
 
             output = output[:, :, 0:num_classes] / torch.exp(softmax_temperature)
@@ -335,21 +403,22 @@
                 except:
                     pass
             eval_xs = torch.tensor(eval_xs).float()
         warnings.simplefilter('default')
 
         eval_xs = eval_xs.unsqueeze(1)
 
-        # TODO: Cautian there is information leakage when to_ranking is used, we should not use it
-        eval_xs = remove_outliers(eval_xs, normalize_positions=-1 if normalize_with_test else eval_position) if not normalize_to_ranking else normalize_data(to_ranking_low_mem(eval_xs))
+        # TODO: Caution there is information leakage when to_ranking is used, we should not use it
+        eval_xs = remove_outliers(eval_xs, normalize_positions=-1 if normalize_with_test else eval_position) \
+                if not normalize_to_ranking else normalize_data(to_ranking_low_mem(eval_xs))
         # Rescale X
         eval_xs = normalize_by_used_features_f(eval_xs, eval_xs.shape[-1], max_features,
                                                normalize_with_sqrt=normalize_with_sqrt)
 
-        return eval_xs.detach().to(device)
+        return eval_xs.to(device)
 
     eval_xs, eval_ys = eval_xs.to(device), eval_ys.to(device)
     eval_ys = eval_ys[:eval_position]
 
     model.to(device)
 
     model.eval()
@@ -408,24 +477,17 @@
         softmax_temperature_ = softmax_temperature[styles_configuration]
 
         eval_xs_, eval_ys_ = eval_xs.clone(), eval_ys.clone()
 
         if preprocess_transform_configuration in eval_xs_transformed:
             eval_xs_ = eval_xs_transformed[preprocess_transform_configuration].clone()
         else:
-            if eval_xs_.shape[-1] * 3 < max_features and combine_preprocessing:
-                eval_xs_ = torch.cat([preprocess_input(eval_xs_, preprocess_transform='power_all'),
-                            preprocess_input(eval_xs_, preprocess_transform='quantile_all')], -1)
-                eval_xs_ = normalize_data(eval_xs_, normalize_positions=-1 if normalize_with_test else eval_position)
-                #eval_xs_ = torch.stack([preprocess_input(eval_xs_, preprocess_transform='power_all'),
-                #                        preprocess_input(eval_xs_, preprocess_transform='robust_all'),
-                #                        preprocess_input(eval_xs_, preprocess_transform='none')], -1)
-                #eval_xs_ = torch.flatten(torch.swapaxes(eval_xs_, -2, -1), -2)
-            else:
-                eval_xs_ = preprocess_input(eval_xs_, preprocess_transform=preprocess_transform_configuration)
+            eval_xs_ = preprocess_input(eval_xs_, preprocess_transform=preprocess_transform_configuration)
+            if no_grad:
+                eval_xs_ = eval_xs_.detach()
             eval_xs_transformed[preprocess_transform_configuration] = eval_xs_
 
         eval_ys_ = ((eval_ys_ + class_shift_configuration) % num_classes).float()
 
         eval_xs_ = torch.cat([eval_xs_[..., feature_shift_configuration:],eval_xs_[..., :feature_shift_configuration]],dim=-1)
 
         # Extend X
@@ -462,20 +524,21 @@
     outputs = torch.cat(outputs, 1)
     for i, ensemble_configuration in enumerate(ensemble_configurations):
         (class_shift_configuration, feature_shift_configuration), preprocess_transform_configuration, styles_configuration = ensemble_configuration
         output_ = outputs[:, i:i+1, :]
         output_ = torch.cat([output_[..., class_shift_configuration:],output_[..., :class_shift_configuration]],dim=-1)
 
         #output_ = predict(eval_xs, eval_ys, style_, preprocess_transform_)
-        if not average_logits:
+        if not average_logits and not return_logits:
+            # transforms every ensemble_configuration into a probability -> equal contribution of every configuration
             output_ = torch.nn.functional.softmax(output_, dim=-1)
         output = output_ if output is None else output + output_
 
     output = output / len(ensemble_configurations)
-    if average_logits:
+    if average_logits and not return_logits:
         output = torch.nn.functional.softmax(output, dim=-1)
 
     output = torch.transpose(output, 0, 1)
 
     return output
 
 def get_params_from_config(c):
```

### Comparing `tabpfn-0.1.8/tabpfn/tests/test_deterministic_and_model_caching.py` & `tabpfn-0.1.9/tabpfn/tests/test_deterministic_and_model_caching.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/tests/test_follow_sklearn_interface.py` & `tabpfn-0.1.9/tabpfn/tests/test_follow_sklearn_interface.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/tabpfn/tests/test_load_module_only_inference.py` & `tabpfn-0.1.9/tabpfn/tests/test_load_module_only_inference.py`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/.gitignore` & `tabpfn-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/LICENSE.txt` & `tabpfn-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabpfn-0.1.8/README.md` & `tabpfn-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 pip install tabpfn
 ```
 
 If you want to train and evaluate our method like we did in the paper (including baselines) please install with
 ```bash
 pip install tabpfn[full]
 ```
-To run the autogluon and autosklearn baseline please create a separate environment and install autosklearn / autogluon==0.4.0, installation in the same environment as our other baselines is not possible.
+To run the autogluon and autosklearn baseline please create a separate environment and install autosklearn==0.14.5 / autogluon==0.4.0, installation in the same environment as our other baselines is not possible.
 
 ## Getting started
 
 A simple usage of our sklearn interface is:
 ```python
 from sklearn.metrics import accuracy_score
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 
-from tabpfn.scripts.transformer_prediction_interface import TabPFNClassifier
+from tabpfn import TabPFNClassifier
 
 X, y = load_breast_cancer(return_X_y=True)
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, random_state=42)
 
 # N_ensemble_configurations controls the number of model predictions that are ensembled with feature and class rotations (See our work for details).
 # When N_ensemble_configurations > #features * #classes, no further averaging is applied.
```

### Comparing `tabpfn-0.1.8/pyproject.toml` & `tabpfn-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tabpfn"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
 {name="Noah Hollmann"},
 {name="Samuel Muller", email="muellesa@tf.uni-freiburg.de"},
 {name="Katharina Eggensperger"},
 {name="Frank Hutter"},
 ]
 description = "Interface for using TabPFN and library to train TabPFN'"
@@ -38,13 +38,13 @@
     'gpytorch>=1.5.0', # training
     'catboost>=0.26.1', # baselines
     'auto-sklearn>=0.14.5', # baselines
     'xgboost>=1.4.0', # baselines
     'hyperopt>=0.2.5', # baselines
     'configspace>=0.4.21', # baselins + training + evaluation
     'openml>=0.12.2', # evaluation + baselines
-    'seaborn>=0.11.2', # evaluation
+    'seaborn==0.11', # evaluation
     'tqdm>=4.62.1', # training + evaluation
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/automl/TabPFN'"
```

### Comparing `tabpfn-0.1.8/PKG-INFO` & `tabpfn-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpfn
-Version: 0.1.8
+Version: 0.1.9
 Summary: Interface for using TabPFN and library to train TabPFN'
 Project-URL: Homepage, https://github.com/automl/TabPFN'
 Author: Noah Hollmann, Katharina Eggensperger, Frank Hutter
 Author-email: Samuel Muller <muellesa@tf.uni-freiburg.de>
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Provides-Extra: full
 Requires-Dist: auto-sklearn>=0.14.5; extra == 'full'
 Requires-Dist: catboost>=0.26.1; extra == 'full'
 Requires-Dist: configspace>=0.4.21; extra == 'full'
 Requires-Dist: gpytorch>=1.5.0; extra == 'full'
 Requires-Dist: hyperopt>=0.2.5; extra == 'full'
 Requires-Dist: openml>=0.12.2; extra == 'full'
-Requires-Dist: seaborn>=0.11.2; extra == 'full'
+Requires-Dist: seaborn==0.11; extra == 'full'
 Requires-Dist: tqdm>=4.62.1; extra == 'full'
 Requires-Dist: xgboost>=1.4.0; extra == 'full'
 Description-Content-Type: text/markdown
 
 # TabPFN
 
 The TabPFN is a neural network that learned to do tabular data prediction.
@@ -45,25 +45,25 @@
 pip install tabpfn
 ```
 
 If you want to train and evaluate our method like we did in the paper (including baselines) please install with
 ```bash
 pip install tabpfn[full]
 ```
-To run the autogluon and autosklearn baseline please create a separate environment and install autosklearn / autogluon==0.4.0, installation in the same environment as our other baselines is not possible.
+To run the autogluon and autosklearn baseline please create a separate environment and install autosklearn==0.14.5 / autogluon==0.4.0, installation in the same environment as our other baselines is not possible.
 
 ## Getting started
 
 A simple usage of our sklearn interface is:
 ```python
 from sklearn.metrics import accuracy_score
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
 
-from tabpfn.scripts.transformer_prediction_interface import TabPFNClassifier
+from tabpfn import TabPFNClassifier
 
 X, y = load_breast_cancer(return_X_y=True)
 X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.33, random_state=42)
 
 # N_ensemble_configurations controls the number of model predictions that are ensembled with feature and class rotations (See our work for details).
 # When N_ensemble_configurations > #features * #classes, no further averaging is applied.
```

