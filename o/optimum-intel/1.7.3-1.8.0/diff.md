# Comparing `tmp/optimum-intel-1.7.3.tar.gz` & `tmp/optimum-intel-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/optimum-intel-1.7.3.tar", last modified: Wed Mar 29 13:07:24 2023, max compression
+gzip compressed data, was "optimum-intel-1.8.0.tar", last modified: Mon Apr 17 13:06:57 2023, max compression
```

## Comparing `optimum-intel-1.7.3.tar` & `optimum-intel-1.8.0.tar`

### file list

```diff
@@ -1,51 +1,60 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    10805 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9558 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.796754 optimum-intel-1.7.3/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.796754 optimum-intel-1.7.3/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     5959 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.796754 optimum-intel-1.7.3/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5717 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.796754 optimum-intel-1.7.3/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1397 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8239 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      474 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1129 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    26904 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38649 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10813 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3910 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     2247 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3014 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    27271 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15860 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18319 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    20694 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    19619 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13974 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38592 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1973 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4497 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8799 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-03-29 12:05:31.000000 optimum-intel-1.7.3/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    10805 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     1530 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      464 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-03-29 13:07:24.000000 optimum-intel-1.7.3/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)      674 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-03-29 13:07:24.806753 optimum-intel-1.7.3/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2602 2023-03-29 12:04:20.000000 optimum-intel-1.7.3/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9957 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.641269 optimum-intel-1.8.0/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.641269 optimum-intel-1.8.0/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6003 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5717 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1063 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3744 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    27524 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    39116 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10813 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3905 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.661269 optimum-intel-1.8.0/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1514 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3014 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    22259 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15305 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18165 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    19198 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    20602 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    19620 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13635 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38278 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.661269 optimum-intel-1.8.0/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1278 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-04-17 13:04:42.000000 optimum-intel-1.8.0/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     1777 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      459 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2679 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/setup.py
```

### Comparing `optimum-intel-1.7.3/LICENSE` & `optimum-intel-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/MANIFEST.in` & `optimum-intel-1.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/PKG-INFO` & `optimum-intel-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.7.3
+Version: 1.8.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,16 +97,28 @@
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
+#### Apply dynamic quantization on your model using the CLI
+
+Dynamic quantization can be used through the Optimum Intel command-line:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
+
+For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+
+
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
 
 To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class.
@@ -196,15 +208,15 @@
     args=TrainingArguments(save_dir, num_train_epochs=1.0, do_train=True, do_eval=True),
     train_dataset=dataset["train"].select(range(300)),
     eval_dataset=dataset["validation"],
     compute_metrics=compute_metrics,
     tokenizer=tokenizer,
     data_collator=default_data_collator,
 +   ov_config=ov_config,
-+   task="sequence-classification",
++   task="text-classification",
 )
 train_result = trainer.train()
 metrics = trainer.evaluate()
 trainer.save_model()
 
 + optimized_model = OVModelForSequenceClassification.from_pretrained(save_dir)
 ```
```

### Comparing `optimum-intel-1.7.3/README.md` & `optimum-intel-1.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -68,16 +68,28 @@
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
+#### Apply dynamic quantization on your model using the CLI
+
+Dynamic quantization can be used through the Optimum Intel command-line:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
+
+For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+
+
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
 
 To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class.
@@ -167,15 +179,15 @@
     args=TrainingArguments(save_dir, num_train_epochs=1.0, do_train=True, do_eval=True),
     train_dataset=dataset["train"].select(range(300)),
     eval_dataset=dataset["validation"],
     compute_metrics=compute_metrics,
     tokenizer=tokenizer,
     data_collator=default_data_collator,
 +   ov_config=ov_config,
-+   task="sequence-classification",
++   task="text-classification",
 )
 train_result = trainer.train()
 metrics = trainer.evaluate()
 trainer.save_model()
 
 + optimized_model = OVModelForSequenceClassification.from_pretrained(save_dir)
 ```
```

### Comparing `optimum-intel-1.7.3/optimum/intel/__init__.py` & `optimum-intel-1.8.0/optimum/intel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     from .utils import dummy_neural_compressor_objects
 
     _import_structure["utils.dummy_neural_compressor_objects"] = [
         name for name in dir(dummy_neural_compressor_objects) if not name.startswith("_")
     ]
 else:
     _import_structure["neural_compressor"] = [
+        "INCConfig",
         "INCModelForCausalLM",
         "INCModelForMaskedLM",
         "INCModelForMultipleChoice",
         "INCModelForQuestionAnswering",
         "INCModelForSeq2SeqLM",
         "INCModelForSequenceClassification",
         "INCModelForTokenClassification",
@@ -156,14 +157,15 @@
     try:
         if not is_neural_compressor_available():
             raise OptionalDependencyNotAvailable()
     except OptionalDependencyNotAvailable:
         from .utils.dummy_neural_compressor_objects import *
     else:
         from .neural_compressor import (
+            INCConfig,
             INCModel,
             INCModelForCausalLM,
             INCModelForMaskedLM,
             INCModelForMultipleChoice,
             INCModelForQuestionAnswering,
             INCModelForSeq2SeqLM,
             INCModelForSequenceClassification,
```

### Comparing `optimum-intel-1.7.3/optimum/intel/ipex/inference.py` & `optimum-intel-1.8.0/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.8.0/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 class NeuralCoderAdaptor:
     """API design adaption for Neural Coder"""
 
-    default_quant_dynamic = f"""\
+    default_quant_dynamic = """\
 def eval_func(model):
     EVAL_FUNC_LINES
 from neural_compressor.config import PostTrainingQuantConfig
 from optimum.intel.neural_compressor import INCQuantizer
 quantization_config = PostTrainingQuantConfig(approach="dynamic")
 quantizer = INCQuantizer.from_pretrained(MODEL_NAME, eval_fn=eval_func)
 quantizer.quantize(quantization_config=quantization_config, save_directory="quantized_model", save_onnx_model=False)
 MODEL_NAME = quantizer._quantized_model
 MODEL_NAME.eval()
 """
 
-    default_quant_static = f"""\
+    default_quant_static = """\
 def eval_func(model):
     EVAL_FUNC_LINES
 from neural_compressor.config import PostTrainingQuantConfig
 from optimum.intel.neural_compressor import INCQuantizer
 quantization_config = PostTrainingQuantConfig(approach="static")
 quantizer = INCQuantizer.from_pretrained(MODEL_NAME, eval_fn=eval_func)
 quantizer.quantize(quantization_config=quantization_config, calibration_dataset=eval_dataset, save_directory="quantized_model", save_onnx_model=False)
```

### Comparing `optimum-intel-1.7.3/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.8.0/optimum/intel/neural_compressor/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,24 @@
 import inspect
 import logging
 import os
 import warnings
 from enum import Enum
 from itertools import chain
 from pathlib import Path
-from typing import Callable, ClassVar, Dict, Optional, Union
+from typing import TYPE_CHECKING, Callable, ClassVar, Dict, Optional, Union
 
 import torch
-import transformers
 from datasets import Dataset, load_dataset
-from packaging import version
+from huggingface_hub import HfApi, hf_hub_download
+from neural_compressor.adaptor.pytorch import PyTorch_FXAdaptor, _cfg_to_qconfig, _propagate_qconfig
+from neural_compressor.experimental.export import torch_to_int8_onnx
+from neural_compressor.model.torch_model import IPEXModel, PyTorchModel
+from neural_compressor.quantization import fit
+from neural_compressor.utils.pytorch import load
 from torch.utils.data import DataLoader, RandomSampler
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForCausalLM,
     AutoModelForMaskedLM,
     AutoModelForMultipleChoice,
@@ -45,30 +49,33 @@
     default_data_collator,
 )
 from transformers.modeling_utils import no_init_weights
 from transformers.models.auto.auto_factory import _get_model_class
 from transformers.utils import TRANSFORMERS_CACHE, is_offline_mode
 from transformers.utils.generic import ContextManagers
 
-import neural_compressor
-from huggingface_hub import HfApi, hf_hub_download
-from neural_compressor.adaptor.pytorch import PyTorch_FXAdaptor, _cfg_to_qconfig, _propagate_qconfig
-from neural_compressor.experimental.export import torch_to_int8_onnx
-from neural_compressor.model.torch_model import IPEXModel, PyTorchModel
-from neural_compressor.quantization import fit
-from neural_compressor.utils.pytorch import load
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 from optimum.quantization_base import OptimumQuantizer
 
-from ..utils.import_utils import _neural_compressor_version, is_neural_compressor_version
-from .configuration import IncOptimizedConfig, IncQuantizationConfig
+from ..utils.constant import _TASK_ALIASES
+from ..utils.import_utils import (
+    _neural_compressor_version,
+    _torch_version,
+    is_neural_compressor_version,
+    is_torch_version,
+)
+from .configuration import INCConfig
 from .utils import MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, WEIGHTS_NAME, INCDataLoader, _cfgs_to_fx_cfgs
 
 
+if TYPE_CHECKING:
+    from neural_compressor.config import PostTrainingQuantConfig
+
+
 logger = logging.getLogger(__name__)
 
 NEURAL_COMPRESSOR_MINIMUM_VERSION = "2.1.0"
 
 if is_neural_compressor_version("<", NEURAL_COMPRESSOR_MINIMUM_VERSION):
     raise ImportError(
         f"Found an incompatible version of neural-compressor. Found version {_neural_compressor_version}, "
@@ -78,15 +85,15 @@
 
 class INCQuantizationMode(Enum):
     DYNAMIC = "post_training_dynamic_quant"
     STATIC = "post_training_static_quant"
     AWARE_TRAINING = "quant_aware_training"
 
 
-SUPPORTED_QUANT_MODE = set([approach.value for approach in INCQuantizationMode])
+SUPPORTED_QUANT_MODE = {approach.value for approach in INCQuantizationMode}
 
 
 class INCQuantizer(OptimumQuantizer):
     """
     Handle the Neural Compressor quantization process.
     """
 
@@ -158,14 +165,16 @@
         save_onnx_model = kwargs.pop("save_onnx_model", False)
         output_path = save_directory.joinpath(WEIGHTS_NAME)
         calibration_dataloader = None
 
         if INCQuantizationMode(quantization_config.approach) == INCQuantizationMode.STATIC:
             if calibration_dataset is None:
                 raise ValueError("Post-training static quantization needs a calibration dataset.")
+
+            quantization_config.calibration_sampling_size = len(calibration_dataset)
             calibration_dataloader = self._get_calibration_dataloader(
                 calibration_dataset=calibration_dataset,
                 batch_size=batch_size,
                 remove_unused_columns=remove_unused_columns,
                 data_collator=data_collator,
             )
 
@@ -205,15 +214,16 @@
             compressed_model.eval()
             output_onnx_path = save_directory.joinpath(ONNX_WEIGHTS_NAME)
             # Export the compressed model to the ONNX format
             self._onnx_export(compressed_model, onnx_config, output_onnx_path)
 
         # Save the quantized model
         self._save_pretrained(compressed_model, output_path)
-        # TODO : Save quantization_config
+        quantization_config = INCConfig(quantization=quantization_config, save_onnx_model=save_onnx_model)
+        quantization_config.save_pretrained(save_directory)
 
     @staticmethod
     def _save_pretrained(model: Union[PyTorchModel, IPEXModel], output_path: str):
         if isinstance(model, IPEXModel):
             model._model.save(output_path)
             logger.info(f"Model weights saved to {output_path}")
             return
@@ -226,18 +236,18 @@
     def _onnx_export(
         self,
         model: PyTorchModel,
         config: OnnxConfig,
         output_path: Union[str, Path],
     ):
         opset = min(config.DEFAULT_ONNX_OPSET, MIN_QDQ_ONNX_OPSET)
-        dynamic_axes = {name: axes for name, axes in chain(config.inputs.items(), config.outputs.items())}
+        dynamic_axes = dict(chain(config.inputs.items(), config.outputs.items()))
         inputs = config.generate_dummy_inputs(framework="pt")
         device = model.model.device
-        inputs = dict((k, v.to(device)) for k, v in inputs.items())
+        inputs = {k: v.to(device) for k, v in inputs.items()}
         torch_to_int8_onnx(
             fp32_model=self._original_model.to(device),
             int8_model=model.model,
             q_config=model.q_config,
             save_path=str(output_path),
             example_inputs=inputs,
             opset_version=opset,
@@ -245,24 +255,23 @@
             input_names=list(config.inputs.keys()),
             output_names=list(config.outputs.keys()),
         )
 
     def _set_task(self):
         if self.task is None:
             self.task = HfApi().model_info(self._original_model.config._name_or_path).pipeline_tag
-            if self.task in ["sentiment-analysis", "text-classification", "zero-shot-classification"]:
-                self.task = "sequence-classification"
-            elif self.task in ["feature-extraction", "fill-mask"]:
-                self.task = "default"
-            elif self.task is None:
+            if self.task is None:
                 raise ValueError(
                     "The task defining the model topology could not be extracted and needs to be specified for the ONNX export."
                 )
-        if self.task in ["seq2seq-lm", "translation", "summarization"]:
-            raise ValueError(f"Seq2Seq models are currently not supported for post-training static quantization.")
+
+        self.task = _TASK_ALIASES.get(self.task, self.task)
+
+        if self.task == "text2text-generation":
+            raise ValueError("Seq2Seq models are currently not supported for post-training static quantization.")
 
     def get_calibration_dataset(
         self,
         dataset_name: str,
         num_samples: int = 100,
         dataset_config_name: Optional[str] = None,
         dataset_split: str = "train",
@@ -527,26 +536,40 @@
                         msg += (
                             f"- or '{revision}' is a valid git identifier (branch name, a tag name, or a commit id) that "
                             f"exists for this model name as listed on its model page on 'https://huggingface.co/models'\n\n"
                         )
 
                     raise EnvironmentError(msg)
 
+        msg = None
+        try:
+            inc_config = INCConfig.from_pretrained(model_name_or_path)
+            if not is_torch_version("==", inc_config.torch_version):
+                msg = f"Quantized model was obtained with torch version {inc_config.torch_version} but {_torch_version} was found."
+                logger.warning(f"{msg}")
+        except Exception:
+            logger.info("Couldn't verify torch version.")
+
         if getattr(config, "backend", None) == "ipex":
             # NOTE: Will improve to use load function when Intel Neural Compressor next 2.1 release.
             # return load(state_dict_path)
             load_model = torch.jit.load(state_dict_path)
             load_model = torch.jit.freeze(load_model.eval())
             return load_model
 
         # Load the state dictionary of the model to verify whether the model is quantized or not
         state_dict = torch.load(state_dict_path, map_location="cpu")
 
         if "best_configure" in state_dict and state_dict["best_configure"] is not None:
-            model = load(state_dict_path, model)
+            try:
+                model = load(state_dict_path, model)
+            except Exception as e:
+                if msg is not None:
+                    e.args += (msg,)
+                raise
 
         return model.eval()
 
 
 class INCModelForQuestionAnswering(INCModel):
     TRANSFORMERS_AUTO_CLASS = AutoModelForQuestionAnswering
```

### Comparing `optimum-intel-1.7.3/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 from collections.abc import Mapping
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import datasets
 import torch
 import torch.distributed as dist
+from neural_compressor import training
+from neural_compressor.compression import DistillationCallbacks
+from neural_compressor.conf.pythonic_config import _BaseQuantizationConfig
+from neural_compressor.experimental.export import torch_to_fp32_onnx, torch_to_int8_onnx
 
 # from packaging import version
 from torch import nn
 from torch.utils.data import Dataset, RandomSampler
 from torch.utils.data.dataloader import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm.auto import tqdm
@@ -52,29 +56,33 @@
     HPSearchBackend,
     ShardedDDPOption,
     TrainOutput,
     has_length,
     speed_metrics,
 )
 from transformers.training_args import TrainingArguments
-from transformers.utils import is_sagemaker_mp_enabled, logging
+from transformers.utils import is_apex_available, is_sagemaker_mp_enabled, logging
 
-from neural_compressor import training
-from neural_compressor.compression import DistillationCallbacks
-from neural_compressor.conf.pythonic_config import _BaseQuantizationConfig
-from neural_compressor.experimental.export import torch_to_fp32_onnx, torch_to_int8_onnx
-from neural_compressor.model.torch_model import PyTorchModel
 from optimum.exporters import TasksManager
 
+from ..utils.constant import _TASK_ALIASES
 from ..utils.import_utils import is_neural_compressor_version
+from .configuration import INCConfig
 from .utils import MIN_QDQ_ONNX_OPSET, ONNX_WEIGHTS_NAME, TRAINING_ARGS_NAME
 
 
+if is_apex_available():
+    from apex import amp
+
+if is_sagemaker_mp_enabled():
+    import smdistributed.modelparallel.torch as smp
+
+
 if TYPE_CHECKING:
-    import optuna
+    from optimum.exporters.onnx import OnnxConfig
 
 
 __version__ = "4.22.2"
 
 
 logger = logging.get_logger(__name__)
 
@@ -152,14 +160,21 @@
             self.model_wrapped = self.model
 
         for callback in self._compression_manager.callbacks.callbacks_list:
             if isinstance(callback, DistillationCallbacks):
                 self.distillation_callback = callback
                 break
 
+        self.inc_config = INCConfig(
+            quantization=self.quantization_config,
+            pruning=self.pruning_config,
+            distillation=self.distillation_config,
+            save_onnx_model=save_onnx_model,
+        )
+
     def _inner_training_loop(
         self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
     ):
         self._train_batch_size = batch_size
         # Data loader and number of training steps
         train_dataloader = self.get_train_dataloader()
 
@@ -597,30 +612,32 @@
                 set(self._signature_columns) - set(["label", "label_ids"] + self.label_names)
             )
             self._signature_columns = signature_columns
 
             self.model.eval()
             self._onnx_export(self.model, onnx_config, output_onnx_path)
 
+        if self.pruning_config is not None:
+            self.inc_config.pruning["sparsity"] = round(self.get_model_sparsity(), 2)
+        self.inc_config.save_onnx_model = save_onnx_model
+        self.inc_config.save_pretrained(output_dir)
+
         logger.info(f"Model weights saved in {output_model_file}")
 
     def _set_task(self):
         if self.task is None:
             raise ValueError("The model task defining the model topology needs to be specified for the ONNX export.")
-        elif self.task in ["sentiment-analysis", "text-classification", "zero-shot-classification"]:
-            self.task = "sequence-classification"
-        elif self.task in ["feature-extraction", "fill-mask"]:
-            self.task = "default"
+        self.task = _TASK_ALIASES.get(self.task, self.task)
 
     def _onnx_export(self, model: nn.Module, config: "OnnxConfig", output_path: str):
         opset = min(config.DEFAULT_ONNX_OPSET, MIN_QDQ_ONNX_OPSET)
-        dynamic_axes = {name: axes for name, axes in chain(config.inputs.items(), config.outputs.items())}
+        dynamic_axes = dict(chain(config.inputs.items(), config.outputs.items()))
         inputs = config.generate_dummy_inputs(framework="pt")
         device = model.device
-        inputs = dict((k, v.to(device)) for k, v in inputs.items())
+        inputs = {k: v.to(device) for k, v in inputs.items()}
 
         if self.dtype == "int8":
             torch_to_int8_onnx(
                 fp32_model=self._compression_manager.model.fp32_model.to(device),
                 int8_model=model,
                 q_config=self._compression_manager.model.q_config,
                 save_path=output_path,
@@ -655,15 +672,15 @@
             logger.info(
                 f"The following columns {dset_description} don't have a corresponding argument in "
                 f"`{self.model.__class__.__name__}.forward` and have been ignored: {', '.join(ignored_columns)}."
                 f" If {', '.join(ignored_columns)} are not expected by `{self.model.__class__.__name__}.forward`, "
                 " you can safely ignore this message."
             )
 
-        columns = [k for k in signature_columns if k in dataset.column_names]
+        [k for k in signature_columns if k in dataset.column_names]
 
         return dataset.remove_columns(ignored_columns)
 
     @staticmethod
     def _get_logits(model_outputs):
         output_names = ["logits", "start_logits", "end_logits"]
         return tuple(model_outputs.get(name) for name in output_names if name in model_outputs)
@@ -726,20 +743,20 @@
         Prepares one `data` before feeding it to the model, be it a tensor or a nested list/dictionary of tensors.
         """
         if isinstance(data, Mapping):
             return type(data)({k: self._prepare_input(v) for k, v in data.items()})
         elif isinstance(data, (tuple, list)):
             return type(data)(self._prepare_input(v) for v in data)
         elif isinstance(data, torch.Tensor):
-            kwargs = dict(device=self.model.device)
+            kwargs = {"device": self.model.device}
             if self.deepspeed and data.dtype != torch.int64:
                 # NLP models inputs are int64 and those get adjusted to the right dtype of the
                 # embedding. Other models such as wav2vec2's inputs are already float and thus
                 # may need special handling to match the dtypes of the model
-                kwargs.update(dict(dtype=self.args.hf_deepspeed_config.dtype()))
+                kwargs.update({"dtype": self.args.hf_deepspeed_config.dtype()})
             return data.to(**kwargs)
         return data
 
     @staticmethod
     def _get_logits(model_outputs):
         output_names = ["logits", "start_logits", "end_logits"]
         return tuple(model_outputs.get(name) for name in output_names if name in model_outputs)
```

### Comparing `optimum-intel-1.7.3/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.8.0/optimum/intel/neural_compressor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 
 import logging
 import os
 from collections import UserDict
 from typing import Dict
 
 import torch
+from neural_compressor.utils.pytorch import load
 from packaging import version
 from torch.utils.data import DataLoader
 
-from neural_compressor.utils.pytorch import load
-
 
 logger = logging.getLogger(__name__)
 
 
 CONFIG_NAME = "best_configure.yaml"
 WEIGHTS_NAME = "pytorch_model.bin"
 TRAINING_ARGS_NAME = "training_args.bin"
@@ -68,15 +67,15 @@
             Dictionary of quantization configure that meets the requirements of torch.fx.
     """
     if not is_torch_less_than_1_13:
         from torch.ao.quantization import QConfigMapping
 
         fx_op_cfgs = QConfigMapping()
     else:
-        fx_op_cfgs = dict()
+        fx_op_cfgs = {}
         op_tuple_cfg_list = []
     for key, value in op_cfgs.items():
         if key == "default_qconfig":
             if not is_torch_less_than_1_13:
                 fx_op_cfgs.set_global(value)
             else:
                 fx_op_cfgs[""] = value
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/configuration.py` & `optimum-intel-1.8.0/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/modeling.py` & `optimum-intel-1.8.0/optimum/intel/openvino/modeling.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,52 +9,43 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
-from typing import Any, Dict, Optional, Union
+from typing import Optional, Union
 
 import numpy as np
+import openvino
 import torch
 import transformers
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForAudioClassification,
-    AutoModelForCausalLM,
     AutoModelForImageClassification,
     AutoModelForMaskedLM,
     AutoModelForQuestionAnswering,
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
 )
 from transformers.file_utils import add_start_docstrings, add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import (
     BaseModelOutput,
-    CausalLMOutputWithCrossAttentions,
     ImageClassifierOutput,
     MaskedLMOutput,
     QuestionAnsweringModelOutput,
     SequenceClassifierOutput,
     TokenClassifierOutput,
 )
 
-import openvino
-
-from ..utils.import_utils import is_transformers_version
 from .modeling_base import OVBaseModel
 
 
-if is_transformers_version("<", "4.25.0"):
-    from transformers.generation_utils import GenerationMixin
-else:
-    from transformers.generation import GenerationMixin
-
 logger = logging.getLogger(__name__)
 
 
 _TOKENIZER_FOR_DOC = "AutoTokenizer"
 _FEATURE_EXTRACTOR_FOR_DOC = "AutoFeatureExtractor"
 
 MODEL_START_DOCSTRING = r"""
@@ -111,14 +102,18 @@
         super().__init__(model, config, **kwargs)
         # Avoid warnings when creating a transformers pipeline
         AutoConfig.register(self.base_model_prefix, AutoConfig)
         self.auto_model_class.register(AutoConfig, self.__class__)
         self.device = torch.device("cpu")
 
     def to(self, device: str):
+        """
+        Use the specified `device` for inference. For example: "cpu" or "gpu". `device` can
+        be in upper or lower case. To speed up first inference, call `.compile()` after `.to()`.
+        """
         self._device = device.upper()
         self.request = None
         return self
 
     def forward(self, *args, **kwargs):
         raise NotImplementedError
 
@@ -140,15 +135,15 @@
 @add_start_docstrings(
     """
     OpenVINO Model with a SequenceClassifierOutput for sequence classification tasks.
     """,
     MODEL_START_DOCSTRING,
 )
 class OVModelForSequenceClassification(OVModel):
-    export_feature = "sequence-classification"
+    export_feature = "text-classification"
     auto_model_class = AutoModelForSequenceClassification
 
     def __init__(self, model=None, config=None, **kwargs):
         super().__init__(model, config, **kwargs)
 
     @add_start_docstrings_to_model_forward(
         INPUTS_DOCSTRING.format("batch_size, sequence_length")
@@ -344,15 +339,15 @@
 @add_start_docstrings(
     """
     OpenVINO Model with a BaseModelOutput for feature extraction tasks.
     """,
     MODEL_START_DOCSTRING,
 )
 class OVModelForFeatureExtraction(OVModel):
-    export_feature = "default"
+    export_feature = "feature-extraction"
     auto_model_class = AutoModel
 
     def __init__(self, model=None, config=None, **kwargs):
         super().__init__(model, config, **kwargs)
 
     @add_start_docstrings_to_model_forward(
         INPUTS_DOCSTRING.format("batch_size, sequence_length")
@@ -393,145 +388,14 @@
         last_hidden_state = outputs["last_hidden_state"]
         if not np_inputs:
             last_hidden_state = torch.from_numpy(last_hidden_state).to(self.device)
 
         return BaseModelOutput(last_hidden_state=last_hidden_state)
 
 
-TEXT_GENERATION_EXAMPLE = r"""
-    Example of text generation:
-    ```python
-    >>> from transformers import {processor_class}
-    >>> from optimum.intel import {model_class}
-
-    >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
-    >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
-    >>> inputs = tokenizer("I love this story because", return_tensors="pt")
-    >>> gen_tokens = model.generate(**inputs, do_sample=True, temperature=0.9, min_length=20, max_length=20)
-    >>> tokenizer.batch_decode(gen_tokens)
-    ```
-    Example using `transformers.pipelines`:
-    ```python
-    >>> from transformers import {processor_class}, pipeline
-    >>> from optimum.intel import {model_class}
-
-    >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
-    >>> model = {model_class}.from_pretrained("{checkpoint}", export=True)
-    >>> gen_pipeline = pipeline("text-generation", model=model, tokenizer=tokenizer)
-    >>> text = "I love this story because"
-    >>> gen = gen_pipeline(text)
-    ```
-"""
-
-
-@add_start_docstrings(
-    """
-    OpenVINO Model with a causal language modeling head on top (linear layer with weights tied to the input
-    embeddings).
-    """,
-    MODEL_START_DOCSTRING,
-)
-class OVModelForCausalLM(OVModel, GenerationMixin):
-    """
-    Causal LM model for OpenVINO.
-    """
-
-    export_feature = "causal-lm"
-    auto_model_class = AutoModelForCausalLM
-
-    def __init__(self, model=None, config=None, **kwargs):
-        super().__init__(model, config, **kwargs)
-        self.main_input_name = "input_ids"
-
-    def prepare_inputs_for_generation(self, input_ids: torch.LongTensor, **kwargs) -> Dict[str, Any]:
-        inputs = {"input_ids": input_ids}
-        if kwargs.get("attention_mask", None) is not None:
-            inputs["attention_mask"] = kwargs["attention_mask"]
-        if kwargs.get("token_type_ids") is not None:
-            inputs["token_type_ids"] = kwargs["token_type_ids"]
-        return inputs
-
-    @add_start_docstrings_to_model_forward(
-        INPUTS_DOCSTRING.format("batch_size, sequence_length")
-        + TEXT_GENERATION_EXAMPLE.format(
-            processor_class=_TOKENIZER_FOR_DOC,
-            model_class="OVModelForCausalLM",
-            checkpoint="gpt2",
-        )
-    )
-    def forward(
-        self,
-        input_ids: Union[torch.Tensor, np.ndarray],
-        attention_mask: Union[torch.Tensor, np.ndarray],
-        token_type_ids: Optional[Union[torch.Tensor, np.ndarray]] = None,
-        **kwargs,
-    ):
-        self.compile()
-
-        inputs = {
-            "input_ids": np.array(input_ids),
-            "attention_mask": np.array(attention_mask),
-        }
-
-        # Add the token_type_ids when needed
-        if "token_type_ids" in self.input_names:
-            inputs["token_type_ids"] = np.array(token_type_ids)
-
-        # Run inference
-        outputs = self.request.infer(inputs)
-        outputs = {key.get_any_name(): value for key, value in outputs.items()}
-        logits = torch.from_numpy(outputs["logits"]).to(self.device)
-
-        return CausalLMOutputWithCrossAttentions(logits=logits)
-
-    # Adapted from https://github.com/huggingface/transformers/blob/99289c08a1b16a805dd4ee46de029e9fd23cba3d/src/transformers/generation_utils.py#L490
-    def _prepare_attention_mask_for_generation(
-        self,
-        inputs: torch.Tensor,
-        pad_token_id: int,
-        eos_token_id: int,
-    ) -> torch.LongTensor:
-        """
-        Overrides the base method of `GenerationMixin` to ensure input IDs and
-        attention mask are on the same device.
-        """
-        is_input_ids = len(inputs.shape) == 2 and inputs.dtype in [torch.int, torch.long]
-        is_pad_token_in_inputs = (pad_token_id is not None) and (pad_token_id in inputs)
-        is_pad_token_not_equal_to_eos_token_id = (eos_token_id is None) or (
-            (eos_token_id is not None) and (pad_token_id != eos_token_id)
-        )
-        # Check if input is input_ids and padded -> only then is attention_mask defined
-        if is_input_ids and is_pad_token_in_inputs and is_pad_token_not_equal_to_eos_token_id:
-            return inputs.ne(pad_token_id).long()
-        else:
-            # Ensure attention mask is on the same device as the input IDs
-            return torch.ones(inputs.shape[:2], dtype=torch.long, device=inputs.device)
-
-    def _reshape(
-        self,
-        model: openvino.runtime.Model,
-        batch_size: int,
-        sequence_length: int,
-        height: int = None,
-        width: int = None,
-    ):
-        if batch_size != -1 or sequence_length != -1:
-            logger.warning("Static shapes are not supported for causal language model.")
-            batch_size = -1
-            sequence_length = -1
-
-        return super()._reshape(
-            model=model,
-            batch_size=batch_size,
-            sequence_length=sequence_length,
-            height=height,
-            width=width,
-        )
-
-
 MASKED_LM_EXAMPLE = r"""
     Example of masked language modeling using `transformers.pipelines`:
     ```python
     >>> from transformers import {processor_class}, pipeline
     >>> from optimum.intel import {model_class}
 
     >>> tokenizer = {processor_class}.from_pretrained("{checkpoint}")
@@ -546,15 +410,15 @@
 @add_start_docstrings(
     """
     OpenVINO Model with a MaskedLMOutput for masked language modeling tasks.
     """,
     MODEL_START_DOCSTRING,
 )
 class OVModelForMaskedLM(OVModel):
-    export_feature = "masked-lm"
+    export_feature = "fill-mask"
     auto_model_class = AutoModelForMaskedLM
 
     def __init__(self, model=None, config=None, **kwargs):
         super().__init__(model, config, **kwargs)
 
     @add_start_docstrings_to_model_forward(
         INPUTS_DOCSTRING.format("batch_size, sequence_length")
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.8.0/optimum/intel/openvino/modeling_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 
 import logging
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Dict, Optional, Union
 
-import transformers
-from transformers import AutoConfig, PretrainedConfig
-from transformers.file_utils import add_start_docstrings, default_cache_path
-from transformers.onnx.utils import get_preprocessor
-
 import openvino
-from huggingface_hub import HfApi, hf_hub_download
+from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
 from openvino._offline_transformations import apply_moc_transformations, compress_model_transformation
 from openvino.runtime import Core
+from transformers import PretrainedConfig
+from transformers.file_utils import add_start_docstrings
+
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import export
 from optimum.modeling_base import OptimizedModel
 
 from ..utils.import_utils import is_transformers_version
 from .utils import ONNX_WEIGHTS_NAME, OV_XML_FILE_NAME
 
@@ -71,29 +69,24 @@
         self,
         model: openvino.runtime.Model,
         config: PretrainedConfig = None,
         device: str = "CPU",
         dynamic_shapes: bool = True,
         ov_config: Optional[Dict[str, str]] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
-        **kwargs
+        **kwargs,
     ):
         self.config = config
         self.model_save_dir = model_save_dir
         self._device = device.upper()
         self.is_dynamic = dynamic_shapes
         self.ov_config = ov_config if ov_config is not None else {"PERFORMANCE_HINT": "LATENCY"}
         self.preprocessors = kwargs.get("preprocessors", [])
         enable_compilation = kwargs.get("compile", True)
 
-        if "GPU" in self._device and self.is_dynamic:
-            raise ValueError(
-                "Support of dynamic shapes for GPU devices is not yet available. Set `dynamic_shapes` to `False` to continue."
-            )
-
         if self.is_dynamic:
             height = -1 if self.export_feature == "image-classification" else None
             width = -1 if self.export_feature == "image-classification" else None
             model = self._reshape(model, -1, -1, height, width)
         self.input_names = {key.get_any_name(): idx for idx, key in enumerate(model.inputs)}
         self.model = model
         self.request = None
@@ -310,19 +303,16 @@
             local_files_only=local_files_only,
             **kwargs,
         )
 
     def compile(self):
         if self.request is None:
             logger.info("Compiling the model and creating the inference request ...")
-            # Only enable CACHE_DIR for GPU because CACHE_DIR fails with some INT8 models on CPU with 2022.3
-            ov_config = self.ov_config.copy()
-            if self._device == "GPU":
-                cache_dir = Path(self.model_save_dir).joinpath("model_cache")
-                ov_config["CACHE_DIR"] = str(cache_dir)
+            cache_dir = Path(self.model_save_dir).joinpath("model_cache")
+            ov_config = {**self.ov_config, "CACHE_DIR": str(cache_dir)}
             compiled_model = core.compile_model(self.model, self._device, ov_config)
             self.request = compiled_model.create_infer_request()
 
     def _reshape(
         self,
         model: openvino.runtime.Model,
         batch_size: int,
@@ -359,15 +349,15 @@
         self.is_dynamic = True if batch_size == -1 and sequence_length == -1 else False
         self.model = self._reshape(self.model, batch_size, sequence_length, height, width)
         self.request = None
         return self
 
     def half(self):
         """
-        Converts all the model weights to FP16 for more efficient inference on GPU.
+        Converts all the model weights to FP16
         """
         apply_moc_transformations(self.model, cf=False)
         compress_model_transformation(self.model)
         self.request = None
         return self
 
     def _ensure_supported_device(self, device: str = None):
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.8.0/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,21 @@
 
 import logging
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Dict, Optional, Union
 
-import transformers
-from transformers import AutoConfig, PretrainedConfig
-from transformers.file_utils import add_start_docstrings, default_cache_path
-from transformers.onnx import FeaturesManager, export
-from transformers.onnx.utils import get_preprocessor
-
 import openvino
-from huggingface_hub import HfApi, hf_hub_download
+from huggingface_hub import hf_hub_download
 from huggingface_hub.utils import EntryNotFoundError
 from openvino._offline_transformations import apply_moc_transformations, compress_model_transformation
+from transformers import PretrainedConfig
+from transformers.file_utils import add_start_docstrings
+
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import export_models, get_encoder_decoder_models_for_export
 
 from ..utils.import_utils import is_transformers_version
 from .modeling_base import OVBaseModel
 from .utils import (
     ONNX_DECODER_NAME,
@@ -48,27 +45,27 @@
 
 @add_start_docstrings(
     """
     Base OVModelForSeq2SeqLM class.
     """,
 )
 class OVBaseModelForSeq2SeqLM(OVBaseModel):
-    export_feature = "seq2seq-lm"
+    export_feature = "text2text-generation"
 
     def __init__(
         self,
         encoder: openvino.runtime.Model,
         decoder: openvino.runtime.Model,
         decoder_with_past: openvino.runtime.Model = None,
         config: PretrainedConfig = None,
         device: str = "CPU",
         dynamic_shapes: bool = True,
         ov_config: Optional[Dict[str, str]] = None,
         model_save_dir: Optional[Union[str, Path, TemporaryDirectory]] = None,
-        **kwargs
+        **kwargs,
     ):
         self.config = config
         self.use_cache = decoder_with_past is not None
         self.model_save_dir = model_save_dir
         self._device = device.upper()
         self.is_dynamic = dynamic_shapes
         self.ov_config = ov_config if ov_config is not None else {}
@@ -93,15 +90,15 @@
 
     def _save_pretrained(
         self,
         save_directory: Union[str, Path],
         encoder_file_name: Optional[str] = None,
         decoder_file_name: Optional[str] = None,
         decoder_with_past_file_name: Optional[str] = None,
-        **kwargs
+        **kwargs,
     ):
         """
         Saves the model to the OpenVINO IR format so that it can be re-loaded using the
         [`~optimum.intel.openvino.modeling.OVModel.from_pretrained`] class method.
 
         Arguments:
             save_directory (`str` or `Path`):
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.8.0/optimum/intel/openvino/modeling_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,27 @@
 import logging
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Dict, Optional, Union
 
 import numpy as np
-from transformers import CLIPFeatureExtractor, CLIPTokenizer
-
 import openvino
 from diffusers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, StableDiffusionPipeline
 from diffusers.schedulers.scheduling_utils import SCHEDULER_CONFIG_NAME
 from diffusers.utils import CONFIG_NAME
 from huggingface_hub import snapshot_download
 from openvino._offline_transformations import compress_model_transformation
-from openvino.offline_transformations import compress_model_transformation
 from openvino.runtime import Core
+from transformers import CLIPFeatureExtractor, CLIPTokenizer
+
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import export_models, get_stable_diffusion_models_for_export
 from optimum.pipelines.diffusers.pipeline_stable_diffusion import StableDiffusionPipelineMixin
 from optimum.utils import (
-    CONFIG_NAME,
     DIFFUSION_MODEL_TEXT_ENCODER_SUBFOLDER,
     DIFFUSION_MODEL_UNET_SUBFOLDER,
     DIFFUSION_MODEL_VAE_DECODER_SUBFOLDER,
     DIFFUSION_MODEL_VAE_ENCODER_SUBFOLDER,
 )
 
 from .modeling_base import OVBaseModel
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.8.0/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 #  limitations under the License.
 
 import logging
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import numpy as np
+import openvino
 import torch
 import transformers
+from openvino.runtime import Core, Tensor
 from transformers import AutoConfig, AutoModelForSeq2SeqLM
 from transformers.file_utils import add_start_docstrings, add_start_docstrings_to_model_forward
 from transformers.modeling_outputs import BaseModelOutput, Seq2SeqLMOutput
 
-import openvino
-from openvino.runtime import Core, Tensor
-
 from ..utils.import_utils import is_transformers_version
 from .modeling_base_seq2seq import OVBaseModelForSeq2SeqLM
 
 
 if is_transformers_version("<", "4.25.0"):
     from transformers.generation_utils import GenerationMixin
 else:
@@ -142,15 +141,15 @@
 
     def __init__(
         self,
         encoder: openvino.runtime.Model,
         decoder: openvino.runtime.Model,
         decoder_with_past: openvino.runtime.Model = None,
         config: transformers.PretrainedConfig = None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             encoder=encoder, decoder=decoder, decoder_with_past=decoder_with_past, config=config, **kwargs
         )
         self.device = torch.device("cpu")
         self.main_input_name = "input_ids"
         self.decoder_with_past = None
@@ -228,15 +227,15 @@
         past_key_values=None,
         attention_mask=None,
         head_mask=None,
         decoder_head_mask=None,
         cross_attn_head_mask=None,
         use_cache=None,
         encoder_outputs=None,
-        **kwargs
+        **kwargs,
     ) -> Dict:
         return {
             "decoder_input_ids": input_ids,
             "past_key_values": past_key_values or kwargs.get("past", None),
             "encoder_outputs": encoder_outputs,
             "attention_mask": attention_mask,
             "head_mask": head_mask,
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/quantization.py` & `optimum-intel-1.8.0/optimum/intel/openvino/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 #  limitations under the License.
 
 import inspect
 import io
 import logging
 from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
+import openvino
 import torch
 import transformers
 from datasets import Dataset, load_dataset
-from torch.onnx import export as onnx_export
-from torch.utils.data import DataLoader, RandomSampler
-from transformers import DataCollator, PreTrainedModel, default_data_collator
-
-import openvino
 from huggingface_hub import HfApi
 from nncf import NNCFConfig
 from nncf.torch import create_compressed_model, register_default_init_args
 from nncf.torch.dynamic_graph.io_handling import wrap_nncf_model_inputs_with_objwalk
 from nncf.torch.initialization import PTInitializingDataLoader
 from nncf.torch.nncf_network import NNCFNetwork
 from openvino._offline_transformations import compress_quantize_weights_transformation
 from openvino.runtime import Core
+from torch.onnx import export as onnx_export
+from torch.utils.data import DataLoader, RandomSampler
+from transformers import DataCollator, PreTrainedModel, default_data_collator
+
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 from optimum.quantization_base import OptimumQuantizer
 
+from ..utils.constant import _TASK_ALIASES
 from .configuration import OVConfig
 from .utils import (
     MAX_ONNX_OPSET,
-    MAX_ONNX_OPSET_2022_2_0,
     MIN_ONNX_QDQ_OPSET,
     ONNX_WEIGHTS_NAME,
     OV_XML_FILE_NAME,
     use_external_data_format,
 )
 
 
@@ -196,48 +196,45 @@
         config: OnnxConfig,
         model_inputs: Dict,
         ov_config: OVConfig,
         f: Union[str, io.BytesIO],
     ):
         opset = min(config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
         opset = opset if not ov_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
-        model_inputs = dict((k, v.to(model.device)) for k, v in model_inputs.items())
+        model_inputs = {k: v.to(model.device) for k, v in model_inputs.items()}
         # Create ordered inputs for the ONNX export of NNCFNetwork as keyword arguments are currently not supported
         inputs = tuple([model_inputs.pop(key, None) for key in self._export_input_names if len(model_inputs) != 0])
 
         with torch.no_grad():
             # Disable node additions to be exported in the graph
             model.disable_dynamic_graph_building()
             onnx_export(
                 model,
                 inputs,
                 f=f,
                 input_names=list(config.inputs.keys()),
                 output_names=list(config.outputs.keys()),
-                dynamic_axes={name: axes for name, axes in chain(config.inputs.items(), config.outputs.items())},
+                dynamic_axes=dict(chain(config.inputs.items(), config.outputs.items())),
                 do_constant_folding=True,
                 opset_version=opset,
             )
             model.enable_dynamic_graph_building()
 
     def _set_task(self):
         if self.task is None:
             self.task = HfApi().model_info(self.model.config._name_or_path).pipeline_tag
-            if self.task in ["sentiment-analysis", "text-classification", "zero-shot-classification"]:
-                self.task = "sequence-classification"
-            elif self.task in ["feature-extraction", "fill-mask"]:
-                self.task = "default"
-            elif self.task == "text-generation":
-                self.task = "causal-lm"
-            elif self.task is None:
+            if self.task is None:
                 raise ValueError(
                     "The task defining the model topology could not be extracted and needs to be specified for the ONNX export."
                 )
-        if self.task in ["seq2seq-lm", "translation", "summarization"]:
-            raise ValueError(f"Seq2Seq models are currently not supported for post-training static quantization.")
+
+        self.task = _TASK_ALIASES.get(self.task, self.task)
+
+        if self.task == "text2text-generation":
+            raise ValueError("Seq2Seq models are currently not supported for post-training static quantization.")
 
     def get_calibration_dataset(
         self,
         dataset_name: str,
         num_samples: int = 100,
         dataset_config_name: Optional[str] = None,
         dataset_split: str = "train",
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/trainer.py` & `optimum-intel-1.8.0/optimum/intel/openvino/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,37 @@
 import sys
 import time
 from collections import defaultdict
 from itertools import chain
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 
+import openvino
+import openvino.runtime
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
+from nncf import NNCFConfig
+from nncf.common.logging.logger import nncf_logger, set_log_level
+from nncf.common.utils.tensorboard import prepare_for_tensorboard
+from nncf.config.structures import BNAdaptationInitArgs, QuantizationRangeInitArgs
+from nncf.experimental.torch.sparsity.movement.algo import MovementSparsityController
+from nncf.experimental.torch.sparsity.movement.scheduler import MovementSchedulerStage
+from nncf.torch import create_compressed_model
+from nncf.torch.composite_compression import PTCompositeCompressionAlgorithmController
+from nncf.torch.compression_method_api import PTCompressionAlgorithmController
+from nncf.torch.nncf_network import NNCFNetwork
+from nncf.torch.quantization.algo import QuantizationController
+from openvino._offline_transformations import compress_quantize_weights_transformation
+from openvino.runtime import Core, PartialShape, serialize
+from openvino.tools.mo.back.offline_transformations import (
+    apply_fused_names_cleanup,
+    apply_moc_transformations,
+    apply_user_transformations,
+)
 from torch.onnx import export as onnx_export
 from torch.utils.data import DataLoader, Dataset, RandomSampler
 from torch.utils.data.distributed import DistributedSampler
 from tqdm.auto import tqdm
 from transformers import Trainer
 from transformers.data.data_collator import DataCollator
 from transformers.debug_utils import DebugOption, DebugUnderflowOverflow
@@ -47,51 +67,29 @@
     ShardedDDPOption,
     TrainOutput,
     has_length,
     speed_metrics,
 )
 from transformers.utils import (
     WEIGHTS_NAME,
-    TensorType,
     is_apex_available,
     is_sagemaker_mp_enabled,
     is_torch_tpu_available,
     logging,
 )
 
-import openvino
-import openvino.runtime
-from nncf import NNCFConfig
-from nncf.common.logging.logger import nncf_logger, set_log_level
-from nncf.common.utils.tensorboard import prepare_for_tensorboard
-from nncf.config.structures import BNAdaptationInitArgs, QuantizationRangeInitArgs
-from nncf.experimental.torch.sparsity.movement.algo import MovementSparsityController
-from nncf.experimental.torch.sparsity.movement.scheduler import MovementSchedulerStage
-from nncf.torch import create_compressed_model
-from nncf.torch.composite_compression import PTCompositeCompressionAlgorithmController
-from nncf.torch.compression_method_api import PTCompressionAlgorithmController
-from nncf.torch.nncf_network import NNCFNetwork
-from nncf.torch.quantization.algo import QuantizationController
-from openvino._offline_transformations import compress_quantize_weights_transformation
-from openvino.runtime import Core, PartialShape, serialize
-from openvino.tools.mo.back.offline_transformations import (
-    apply_fused_names_cleanup,
-    apply_moc_transformations,
-    apply_user_transformations,
-)
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
-from optimum.utils import logging
 
+from ..utils.constant import _TASK_ALIASES
 from .configuration import OVConfig
 from .quantization import OVDataLoader
 from .training_args import OVTrainingArguments
 from .utils import (
     MAX_ONNX_OPSET,
-    MAX_ONNX_OPSET_2022_2_0,
     MIN_ONNX_QDQ_OPSET,
     ONNX_WEIGHTS_NAME,
     OV_XML_FILE_NAME,
     use_external_data_format,
 )
 
 
@@ -657,17 +655,16 @@
         logger.info(f"Saving model checkpoint to {output_dir}")
         # Save a trained model and configuration using `save_pretrained()`.
         # They can then be reloaded using `from_pretrained()`
 
         if not isinstance(self.model, PreTrainedModel):
             unwrapped_model = unwrap_model(self.model)
             if isinstance(unwrapped_model, NNCFNetwork):
-                is_pretrained_model = isinstance(unwrapped_model.get_nncf_wrapped_model(), PreTrainedModel)
-            else:
-                is_pretrained_model = isinstance(unwrapped_model, PreTrainedModel)
+                unwrapped_model = unwrapped_model.get_nncf_wrapped_model()
+            is_pretrained_model = isinstance(unwrapped_model, PreTrainedModel)
             if state_dict is None:
                 state_dict = self.model.state_dict()
             if is_pretrained_model:
                 unwrapped_model.save_pretrained(output_dir, state_dict=state_dict)
             else:
                 logger.info("Trainer.model is not a `PreTrainedModel`, only saving its state dict.")
                 torch.save(state_dict, os.path.join(output_dir, WEIGHTS_NAME))
@@ -690,16 +687,16 @@
             model_type = self.model.config.model_type.replace("_", "-")
             onnx_config_class = TasksManager.get_exporter_config_constructor(
                 exporter="onnx",
                 model=self.model,
                 task=self.task,
                 model_type=model_type,
             )
-            onnx_config = onnx_config_class(self.model.config)
 
+            onnx_config = onnx_config_class(self.model.config)
             num_parameters = self.model.num_parameters()
             save_as_external_data = use_external_data_format(num_parameters) or self.ov_config.save_onnx_model
             f = io.BytesIO() if not save_as_external_data else os.path.join(output_dir, ONNX_WEIGHTS_NAME)
             self._onnx_export(self.model, onnx_config, self.ov_config, f)
             ov_model = core.read_model(f) if save_as_external_data else core.read_model(f.getvalue(), b"")
 
             # Prune IR if structured pruning is conducted on the model
@@ -745,52 +742,49 @@
         return (
             movement_controller is not None
             and movement_controller.scheduler.enable_structured_masking
             and movement_controller.scheduler.current_stage == MovementSchedulerStage.POST_WARMUP
         )
 
     def _reshape_ir(self, ov_model: openvino.runtime.Model, static_shape: bool) -> openvino.runtime.Model:
-        new_input_cfg = dict()
+        new_input_cfg = {}
         input_name_vs_shape = {item["keyword"]: item["sample_size"] for item in self.ov_config.input_info}
         for input_ in ov_model.inputs:
             if static_shape is True:
                 new_input_cfg[input_.any_name] = PartialShape(
                     [1] + input_name_vs_shape[input_.any_name][1:]
                 )  # use batch size of 1 for static shape IR
             else:
                 new_input_cfg[input_.any_name] = PartialShape([-1] * len(input_.partial_shape))
         ov_model.reshape(new_input_cfg)
         return ov_model
 
     def _set_task(self):
         if self.task is None:
             raise ValueError("The model task defining the model topology needs to be specified for the ONNX export.")
-        elif self.task in ["sentiment-analysis", "text-classification", "zero-shot-classification"]:
-            self.task = "sequence-classification"
-        elif self.task in ["feature-extraction", "fill-mask"]:
-            self.task = "default"
+        self.task = _TASK_ALIASES.get(self.task, self.task)
 
     def _onnx_export(self, model: NNCFNetwork, config: OnnxConfig, ov_config: OVConfig, f: Union[str, io.BytesIO]):
         opset = min(config.DEFAULT_ONNX_OPSET, MAX_ONNX_OPSET)
         opset = opset if not ov_config.save_onnx_model else max(opset, MIN_ONNX_QDQ_OPSET)
         model_inputs = config.generate_dummy_inputs(framework="pt")
         device = model.device
-        model_inputs = dict((k, v.to(device)) for k, v in model_inputs.items())
+        model_inputs = {k: v.to(device) for k, v in model_inputs.items()}
         self._set_signature_columns_if_needed()  # find model input names needed in ONNX export
         # Create ordered inputs for the ONNX export of NNCFNetwork as keyword arguments are currently not supported
         inputs = tuple([model_inputs.pop(key, None) for key in self._signature_columns if len(model_inputs) != 0])
 
         with torch.no_grad():
             model.eval()
             # Disable node additions to be exported in the graph
             model.disable_dynamic_graph_building()
             onnx_export(
                 model,
                 inputs,
                 f=f,
                 input_names=list(config.inputs.keys()),
                 output_names=list(config.outputs.keys()),
-                dynamic_axes={name: axes for name, axes in chain(config.inputs.items(), config.outputs.items())},
+                dynamic_axes=dict(chain(config.inputs.items(), config.outputs.items())),
                 do_constant_folding=True,
                 opset_version=opset,
             )
             model.enable_dynamic_graph_building()
```

### Comparing `optimum-intel-1.7.3/optimum/intel/openvino/training_args.py` & `optimum-intel-1.8.0/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/__init__.py` & `optimum-intel-1.8.0/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.8.0/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.8.0/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,7 +141,18 @@
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["neural_compressor"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["neural_compressor"])
+
+
+class INCConfig(metaclass=DummyObject):
+    _backends = ["neural_compressor"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["neural_compressor"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["neural_compressor"])
```

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/optimum/intel/utils/import_utils.py` & `optimum-intel-1.8.0/optimum/intel/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import importlib.util
 import operator as op
 import sys
 from collections import OrderedDict
-from typing import Any, List, Union
+from typing import Union
 
 from packaging.version import Version, parse
 
 
 if sys.version_info < (3, 8):
     import importlib_metadata
 else:
@@ -179,35 +179,35 @@
     """
     if not _torch_available:
         return False
     return compare_versions(parse(_torch_version), operation, version)
 
 
 DIFFUSERS_IMPORT_ERROR = """
-{0} requires the diffusers library but it was not found in your environment. You can install it with pip: 
+{0} requires the diffusers library but it was not found in your environment. You can install it with pip:
 `pip install diffusers`. Please note that you may need to restart your runtime after installation.
 """
 
 IPEX_IMPORT_ERROR = """
-{0} requires the ipex library but it was not found in your environment. You can install it with pip: 
+{0} requires the ipex library but it was not found in your environment. You can install it with pip:
 `pip install intel_extension_for_pytorch`. Please note that you may need to restart your runtime after installation.
 """
 
 NNCF_IMPORT_ERROR = """
-{0} requires the nncf library but it was not found in your environment. You can install it with pip: 
+{0} requires the nncf library but it was not found in your environment. You can install it with pip:
 `pip install nncf`. Please note that you may need to restart your runtime after installation.
 """
 
 OPENVINO_IMPORT_ERROR = """
-{0} requires the openvino library but it was not found in your environment. You can install it with pip: 
+{0} requires the openvino library but it was not found in your environment. You can install it with pip:
 `pip install openvino`. Please note that you may need to restart your runtime after installation.
 """
 
 NEURAL_COMPRESSOR_IMPORT_ERROR = """
-{0} requires the neural-compressor library but it was not found in your environment. You can install it with pip: 
+{0} requires the neural-compressor library but it was not found in your environment. You can install it with pip:
 `pip install neural-compressor`. Please note that you may need to restart your runtime after installation.
 """
 
 BACKENDS_MAPPING = OrderedDict(
     [
         ("diffusers", (is_diffusers_available, DIFFUSERS_IMPORT_ERROR)),
         ("ipex", (is_ipex_available, IPEX_IMPORT_ERROR)),
```

### Comparing `optimum-intel-1.7.3/optimum/intel/version.py` & `optimum-intel-1.8.0/optimum/intel/version.py`

 * *Files 3% similar despite different names*

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

### Comparing `optimum-intel-1.7.3/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.8.0/optimum_intel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.7.3
+Version: 1.8.0
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,16 +97,28 @@
 
 # Load the PyTorch model hosted on the hub
 loaded_model_from_hub = INCModelForSequenceClassification.from_pretrained(
     "Intel/distilbert-base-uncased-finetuned-sst-2-english-int8-dynamic"
 )
 ```
 
+#### Apply dynamic quantization on your model using the CLI
+
+Dynamic quantization can be used through the Optimum Intel command-line:
+
+```bash
+optimum-cli inc quantize --model distilbert-base-cased-distilled-squad --output ./quantized_distilbert
+```
+
 You can load many more quantized models hosted on the hub under the Intel organization [`here`](https://huggingface.co/Intel).
 
+
+For more details, please refer to this [guide](https://huggingface.co/docs/optimum/main/en/intel/optimization_inc#apply-quantization-using-the-cli).
+
+
 ## OpenVINO
 
 Below are the examples of how to use OpenVINO and its [NNCF](https://docs.openvino.ai/latest/tmo_introduction.html) framework to accelerate inference.
 
 #### Inference:
 
 To load a model and run inference with OpenVINO Runtime, you can just replace your `AutoModelForXxx` class with the corresponding `OVModelForXxx` class.
@@ -196,15 +208,15 @@
     args=TrainingArguments(save_dir, num_train_epochs=1.0, do_train=True, do_eval=True),
     train_dataset=dataset["train"].select(range(300)),
     eval_dataset=dataset["validation"],
     compute_metrics=compute_metrics,
     tokenizer=tokenizer,
     data_collator=default_data_collator,
 +   ov_config=ov_config,
-+   task="sequence-classification",
++   task="text-classification",
 )
 train_result = trainer.train()
 metrics = trainer.evaluate()
 trainer.save_model()
 
 + optimized_model = OVModelForSequenceClassification.from_pretrained(save_dir)
 ```
```

### Comparing `optimum-intel-1.7.3/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.8.0/optimum_intel.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+optimum/commands/neural_compressor/base.py
+optimum/commands/neural_compressor/quantize.py
+optimum/commands/register/register_inc.py
 optimum/intel/__init__.py
 optimum/intel/version.py
 optimum/intel/ipex/__init__.py
 optimum/intel/ipex/inference.py
 optimum/intel/neural_compressor/__init__.py
 optimum/intel/neural_compressor/configuration.py
 optimum/intel/neural_compressor/launcher.py
@@ -17,26 +20,29 @@
 optimum/intel/neural_compressor/trainer_seq2seq.py
 optimum/intel/neural_compressor/utils.py
 optimum/intel/openvino/__init__.py
 optimum/intel/openvino/configuration.py
 optimum/intel/openvino/modeling.py
 optimum/intel/openvino/modeling_base.py
 optimum/intel/openvino/modeling_base_seq2seq.py
+optimum/intel/openvino/modeling_decoder.py
 optimum/intel/openvino/modeling_diffusion.py
 optimum/intel/openvino/modeling_seq2seq.py
 optimum/intel/openvino/quantization.py
 optimum/intel/openvino/trainer.py
 optimum/intel/openvino/training_args.py
 optimum/intel/openvino/utils.py
 optimum/intel/utils/__init__.py
+optimum/intel/utils/constant.py
 optimum/intel/utils/dummy_ipex_objects.py
 optimum/intel/utils/dummy_neural_compressor_objects.py
 optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
 optimum/intel/utils/dummy_openvino_and_nncf_objects.py
 optimum/intel/utils/dummy_openvino_objects.py
 optimum/intel/utils/import_utils.py
 optimum_intel.egg-info/PKG-INFO
 optimum_intel.egg-info/SOURCES.txt
 optimum_intel.egg-info/dependency_links.txt
+optimum_intel.egg-info/entry_points.txt
 optimum_intel.egg-info/not-zip-safe
 optimum_intel.egg-info/requires.txt
 optimum_intel.egg-info/top_level.txt
```

### Comparing `optimum-intel-1.7.3/pyproject.toml` & `optimum-intel-1.8.0/optimum/commands/register/register_inc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# Copyright 2023 The HuggingFace Team. All rights reserved.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-[tool.black]
-line-length = 119
-target-version = ['py35']
+from ..neural_compressor.base import INCCommand
+
+
+REGISTER_COMMANDS = [INCCommand]
```

### Comparing `optimum-intel-1.7.3/setup.cfg` & `optimum-intel-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.7.3/setup.py` & `optimum-intel-1.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,24 @@
     filepath = "optimum/intel/version.py"
     with open(filepath) as version_file:
         (__version__,) = re.findall('__version__ = "(.*)"', version_file.read())
 except Exception as error:
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 INSTALL_REQUIRE = [
-    "optimum>=1.7.3",
+    "optimum>=1.8.0",
     "transformers>=4.20.0",
     "datasets>=1.4.0",
-    "torch",
     "sentencepiece",
     "scipy",
 ]
 
 TESTS_REQUIRE = ["pytest", "parameterized", "Pillow", "evaluate", "diffusers", "py-cpuinfo"]
 
-QUALITY_REQUIRE = ["black==22.3", "isort>=5.5.4"]
+QUALITY_REQUIRE = ["black~=23.1", "ruff>=0.0.241"]
 
 EXTRAS_REQUIRE = {
     "neural-compressor": [
         "neural-compressor>=2.1.0",
         "onnx",
         "onnxruntime",
         "torch<2.0.0",  # remove after neural-compressor next release
@@ -66,8 +65,9 @@
     author_email="hardware@huggingface.co",
     license="Apache",
     packages=find_namespace_packages(include=["optimum*"]),
     install_requires=INSTALL_REQUIRE,
     extras_require=EXTRAS_REQUIRE,
     include_package_data=True,
     zip_safe=False,
+    entry_points={"console_scripts": ["optimum-cli=optimum.commands.optimum_cli:main"]},
 )
```

