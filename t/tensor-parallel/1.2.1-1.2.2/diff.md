# Comparing `tmp/tensor_parallel-1.2.1.tar.gz` & `tmp/tensor_parallel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.1.tar", last modified: Mon Apr 10 16:52:57 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.2.tar", last modified: Mon Apr 17 07:49:25 2023, max compression
```

## Comparing `tensor_parallel-1.2.1.tar` & `tensor_parallel-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.518557 tensor_parallel-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.522557 tensor_parallel-1.2.1/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.522557 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 16:52:57.000000 tensor_parallel-1.2.1/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:57.526558 tensor_parallel-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-10 16:52:48.000000 tensor_parallel-1.2.1/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.474471 tensor_parallel-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.486471 tensor_parallel-1.2.2/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.486471 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 07:49:25.000000 tensor_parallel-1.2.2/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:49:25.490471 tensor_parallel-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-04-17 07:49:07.000000 tensor_parallel-1.2.2/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.1/LICENCE` & `tensor_parallel-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/PKG-INFO` & `tensor_parallel-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.2 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.1/README.md` & `tensor_parallel-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/setup.cfg` & `tensor_parallel-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.1
+version = 1.2.2
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.2/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.2/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.2/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.2/src/tensor_parallel/communications.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,20 @@
                 self.ranks_updated = []
                 self.parts_ready = threading.Event()
             # note: we can safely update these properties because all ranks have
             # copied self.parts_* to locals before passing parts_ready.wait
 
 
 class DistributedAllReduce(CollectiveOpetationBase):
+    def __init__(self, world_size: int):
+        pass
+
     def __call__(self, x: torch.Tensor, rank: int):
         all_reduce(x)
+        return x
 
 
 class DistributedAllGather(CollectiveOpetationBase):
     def __init__(self, world_size: int, dim: int):
         self.dim = dim
         self.world_size = world_size
```

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/config.py` & `tensor_parallel-1.2.2/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.2/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.2/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.2/src/tensor_parallel/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import torch
 import torch.distributed
 from torch import nn
 from transformers import PreTrainedModel
 
 from tensor_parallel.config import Config
 from tensor_parallel.pretrained_model import TensorParallelPreTrainedModel
+from tensor_parallel.shard import make_distributed_shard
 from tensor_parallel.sharding import Sharded
 from tensor_parallel.tensor_parallel import TensorParallel
 
 logger = logging.getLogger(__file__)
 
 
 def tensor_parallel(
@@ -52,15 +53,15 @@
 
     if distributed:
         if device_ids is None:
             device_ids = [torch.device("cuda" if torch.cuda.is_available() else "cpu")]
         assert len(device_ids) == 1, "if distributed=True, please specify a single (current) device"
         assert not sharded, "distributed + sharded mode is not implemented, please keep one"
 
-        return tensor_parallel_config.make_distributed_shard(module, device=torch.device(device_ids[0]), **kwargs)
+        return make_distributed_shard(module, device=torch.device(device_ids[0]), **kwargs)
     else:
         if isinstance(module, PreTrainedModel):
             module = TensorParallelPreTrainedModel(
                 module, device_ids=device_ids, tensor_parallel_config=tensor_parallel_config, **kwargs
             )
             module.wrapped_model = _maybe_sharded(
                 module.wrapped_model, sharded, num_trainable_parameters, sharded_param_names=sharded_param_names
```

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.2/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.2/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.2/src/tensor_parallel/shard.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # automatically fixes certain submodule attributes such that
     # it's not necessary to specify in a config
     fix_general_attributes(shard)
 
     return unique_wrappers.get(shard, shard)  # wrap the root module if needed
 
 
-def make_distributed_shard(config: Optional[Config], module: nn.Module, device: torch.device):
+def make_distributed_shard(module: nn.Module, device: torch.device, config: Optional[Config] = None):
     if config is None:
         config = get_default_config(module, device_ids=range(torch.distributed.get_world_size()))
         logger.info("Using automatic config: sharding individual linear/conv/emb layers")
 
     config_with_ops = config.create_collective_ops([torch.device("cpu")] * torch.distributed.get_world_size())
     return make_shard(
         module,
```

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.2/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.2/src/tensor_parallel/slicing_configs.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.2/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.2/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.2/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.2/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.2/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.2 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.1/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.2/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/tests/test_basic.py` & `tensor_parallel-1.2.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/tests/test_factory.py` & `tensor_parallel-1.2.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/tests/test_integration.py` & `tensor_parallel-1.2.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/tests/test_saving.py` & `tensor_parallel-1.2.2/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.1/tests/test_transformers.py` & `tensor_parallel-1.2.2/tests/test_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 @pytest.mark.parametrize(
     "model_name",
     [
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Salesforce/codegen-350M-mono",
-        "decapoda-research/llama-7b-hf",
+        "Bingsu/llama-190m-arch",
     ],
 )
 def test_forward_gpt2_like(use_config, devices, model_name):
     torch.manual_seed(0)
 
     try:
         model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
@@ -155,15 +155,15 @@
 @pytest.mark.parametrize(
     "model_name",
     [
         "t5-small",
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
-        "decapoda-research/llama-7b-hf",
+        "Bingsu/llama-190m-arch",
     ],
 )
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 def test_generate(generate_kwargs, model_name, devices):
     torch.manual_seed(0)
 
     def _generate_scores(model, input_ids, generate_kwargs):
```

