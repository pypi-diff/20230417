# Comparing `tmp/optimum-habana-1.4.2.tar.gz` & `tmp/optimum-habana-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-habana-1.4.2.tar", last modified: Thu Mar 16 13:32:57 2023, max compression
+gzip compressed data, was "optimum-habana-1.5.0.tar", last modified: Mon Apr 17 17:31:30 2023, max compression
```

## Comparing `optimum-habana-1.4.2.tar` & `optimum-habana-1.5.0.tar`

### file list

```diff
@@ -1,61 +1,72 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-02-02 13:32:16.000000 optimum-habana-1.4.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-02-02 13:32:16.000000 optimum-habana-1.4.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11497 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      974 2023-03-06 21:24:23.000000 optimum-habana-1.4.2/optimum/habana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/diffusers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/diffusers/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12095 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/pipeline_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    38786 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/diffusers/schedulers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/diffusers/schedulers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13483 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/diffusers/schedulers/scheduling_ddim.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.628915 optimum-habana-1.4.2/optimum/habana/distributed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-02-02 13:32:16.000000 optimum-habana-1.4.2/optimum/habana/distributed/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10624 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/distributed/distributed_runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8406 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/deepspeed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2428 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/gaudi_configuration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/generation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-03-11 15:31:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/generation/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   107543 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/generation/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8005 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/gradient_checkpointing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3157 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/modeling_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/models/albert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/albert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3752 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/albert/modeling_albert.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/models/gpt2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10396 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/modeling_all_models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/models/vit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/vit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1902 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum/habana/transformers/models/wav2vec2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10969 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78460 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13555 2023-03-16 13:05:56.000000 optimum-habana-1.4.2/optimum/habana/transformers/trainer_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2580 2023-03-06 21:22:05.000000 optimum-habana-1.4.2/optimum/habana/transformers/trainer_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22464 2023-03-16 13:02:12.000000 optimum-habana-1.4.2/optimum/habana/transformers/training_args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2954 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/transformers/training_args_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6820 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/optimum/habana/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      639 2023-03-16 13:13:46.000000 optimum-habana-1.4.2/optimum/habana/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/optimum_habana.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12648 2023-03-16 13:32:57.000000 optimum-habana-1.4.2/optimum_habana.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1844 2023-03-16 13:32:57.000000 optimum-habana-1.4.2/optimum_habana.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-16 13:32:57.000000 optimum-habana-1.4.2/optimum_habana.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-16 13:32:49.000000 optimum-habana-1.4.2/optimum_habana.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2023-03-16 13:32:57.000000 optimum-habana-1.4.2/optimum_habana.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-03-16 13:32:57.000000 optimum-habana-1.4.2/optimum_habana.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2023-03-16 13:02:03.000000 optimum-habana-1.4.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-03-16 13:32:57.632915 optimum-habana-1.4.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2268 2023-03-16 13:13:38.000000 optimum-habana-1.4.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11641 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      974 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/diffusers/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12732 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/pipeline_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39462 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/distributed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/distributed/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/distributed/distributed_runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.389443 optimum-habana-1.5.0/optimum/habana/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8435 2023-04-10 08:19:40.000000 optimum-habana-1.5.0/optimum/habana/transformers/deepspeed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/gaudi_configuration.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/generation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/generation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   113660 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/generation/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/gradient_checkpointing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/modeling_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/albert/modeling_albert.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20630 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/bloom/modeling_bloom.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10396 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4914 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/modeling_all_models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84175 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17409 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/trainer_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23777 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/optimum/habana/transformers/training_args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4082 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/optimum/habana/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4725 2023-04-12 07:37:50.000000 optimum-habana-1.5.0/optimum/habana/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 17:25:45.000000 optimum-habana-1.5.0/optimum/habana/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/optimum_habana.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2165 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 17:31:25.000000 optimum-habana-1.5.0/optimum_habana.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-17 17:31:30.000000 optimum-habana-1.5.0/optimum_habana.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2957 2023-04-17 17:31:03.000000 optimum-habana-1.5.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 17:31:30.393443 optimum-habana-1.5.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19824 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/tests/test_diffusers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17839 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/tests/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2774 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_gaudi_configuration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85824 2023-04-17 09:25:52.000000 optimum-habana-1.5.0/tests/test_trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5354 2023-04-17 17:23:33.000000 optimum-habana-1.5.0/tests/test_trainer_distributed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2023-04-08 17:50:23.000000 optimum-habana-1.5.0/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-habana-1.4.2/LICENSE` & `optimum-habana-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.4.2/MANIFEST.in` & `optimum-habana-1.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.4.2/PKG-INFO` & `optimum-habana-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.4.2
+Version: 1.5.0
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,43 +59,36 @@
 
 ```bash
 pip install optimum[habana]
 ```
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.8.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
 
-> Alternatively, you can install the package without pip as follows:
-> ```bash
-> git clone https://github.com/huggingface/optimum-habana.git
-> cd optimum-habana
-> python setup.py install
-> ```
-
 Last but not least, don't forget to install the requirements for every example:
 
 ```bash
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
 
 ## How to use it?
 
 ### Quick Start
 
-🤗 Optimum Habana was designed with one goal in mind: **to make training and evaluation straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
+🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
@@ -153,15 +146,14 @@
 )
 ```
 
 where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories). You can also give the path to a custom Gaudi configuration written in a JSON file such as this one:
 ```json
 {
   "use_habana_mixed_precision": true,
-  "hmp_opt_level": "O1",
   "hmp_is_verbose": false,
   "use_fused_adam": true,
   "use_fused_clip_norm": true,
   "hmp_bf16_ops": [
     "add",
     "addmm",
     "bmm",
@@ -201,15 +193,15 @@
 You can generate images from prompts using Stable Diffusion on Gaudi using the [`GaudiStableDiffusionPipeline`](https://huggingface.co/docs/optimum/habana/package_reference/stable_diffusion_pipeline) class and the [`GaudiDDIMScheduler`] which have been both optimized for HPUs. Here is how to use them and the differences with the 🤗 Diffusers library:
 
 ```diff
 - from diffusers import DDIMScheduler, StableDiffusionPipeline
 + from optimum.habana.diffusers import GaudiDDIMScheduler, GaudiStableDiffusionPipeline
 
 
-model_name = "CompVis/stable-diffusion-v1-4"
+model_name = "runwayml/stable-diffusion-v1-5"
 
 - scheduler = DDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 + scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 
 - pipeline = StableDiffusionPipeline.from_pretrained(
 + pipeline = GaudiStableDiffusionPipeline.from_pretrained(
     model_name,
@@ -246,22 +238,24 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | Stable Diffusion | :heavy_check_mark: | ✗ | ✗ | <li>[text-to-image generation](https://github.com/huggingface/optimum-habana/tree/main/examples/stable-diffusion)</li> |
+| CLIP | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
+| BLOOM(Z) | ✗ | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 
 </div>
 
 Other models and tasks supported by the 🤗 Transformers library may also work. You can refer to this [section](https://github.com/huggingface/optimum-habana#how-to-use-it) for using them with 🤗 Optimum Habana. Besides, [this page](https://github.com/huggingface/optimum-habana/tree/main/examples) explains how to modify any [example](https://github.com/huggingface/transformers/tree/main/examples/pytorch) from the 🤗 Transformers library to make it work with 🤗 Optimum Habana.
 
 If you find any issue while using those, please open an issue or a pull request.
 
 
 ## Gaudi Setup
 
 Please refer to Habana Gaudi's official [installation guide](https://docs.habana.ai/en/latest/Installation_Guide/index.html).
 
 > Tests should be run in a Docker container based on Habana Docker images.
 >
-> The current version has been validated for SynapseAI 1.8.
+> The current version has been validated for SynapseAI 1.9.
```

### Comparing `optimum-habana-1.4.2/README.md` & `optimum-habana-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,43 +36,36 @@
 
 ```bash
 pip install optimum[habana]
 ```
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.8.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
 
-> Alternatively, you can install the package without pip as follows:
-> ```bash
-> git clone https://github.com/huggingface/optimum-habana.git
-> cd optimum-habana
-> python setup.py install
-> ```
-
 Last but not least, don't forget to install the requirements for every example:
 
 ```bash
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
 
 ## How to use it?
 
 ### Quick Start
 
-🤗 Optimum Habana was designed with one goal in mind: **to make training and evaluation straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
+🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
@@ -130,15 +123,14 @@
 )
 ```
 
 where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories). You can also give the path to a custom Gaudi configuration written in a JSON file such as this one:
 ```json
 {
   "use_habana_mixed_precision": true,
-  "hmp_opt_level": "O1",
   "hmp_is_verbose": false,
   "use_fused_adam": true,
   "use_fused_clip_norm": true,
   "hmp_bf16_ops": [
     "add",
     "addmm",
     "bmm",
@@ -178,15 +170,15 @@
 You can generate images from prompts using Stable Diffusion on Gaudi using the [`GaudiStableDiffusionPipeline`](https://huggingface.co/docs/optimum/habana/package_reference/stable_diffusion_pipeline) class and the [`GaudiDDIMScheduler`] which have been both optimized for HPUs. Here is how to use them and the differences with the 🤗 Diffusers library:
 
 ```diff
 - from diffusers import DDIMScheduler, StableDiffusionPipeline
 + from optimum.habana.diffusers import GaudiDDIMScheduler, GaudiStableDiffusionPipeline
 
 
-model_name = "CompVis/stable-diffusion-v1-4"
+model_name = "runwayml/stable-diffusion-v1-5"
 
 - scheduler = DDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 + scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 
 - pipeline = StableDiffusionPipeline.from_pretrained(
 + pipeline = GaudiStableDiffusionPipeline.from_pretrained(
     model_name,
@@ -223,22 +215,24 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | Stable Diffusion | :heavy_check_mark: | ✗ | ✗ | <li>[text-to-image generation](https://github.com/huggingface/optimum-habana/tree/main/examples/stable-diffusion)</li> |
+| CLIP | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
+| BLOOM(Z) | ✗ | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 
 </div>
 
 Other models and tasks supported by the 🤗 Transformers library may also work. You can refer to this [section](https://github.com/huggingface/optimum-habana#how-to-use-it) for using them with 🤗 Optimum Habana. Besides, [this page](https://github.com/huggingface/optimum-habana/tree/main/examples) explains how to modify any [example](https://github.com/huggingface/transformers/tree/main/examples/pytorch) from the 🤗 Transformers library to make it work with 🤗 Optimum Habana.
 
 If you find any issue while using those, please open an issue or a pull request.
 
 
 ## Gaudi Setup
 
 Please refer to Habana Gaudi's official [installation guide](https://docs.habana.ai/en/latest/Installation_Guide/index.html).
 
 > Tests should be run in a Docker container based on Habana Docker images.
 >
-> The current version has been validated for SynapseAI 1.8.
+> The current version has been validated for SynapseAI 1.9.
```

### Comparing `optimum-habana-1.4.2/optimum/habana/__init__.py` & `optimum-habana-1.5.0/optimum/habana/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/pipeline_utils.py` & `optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/pipeline_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import inspect
 import os
 import tempfile
 from typing import Optional, Union
 
 import torch
 from diffusers.pipelines import DiffusionPipeline
+from diffusers.utils import is_compiled_module
 
 from optimum.utils import logging
 
 from ...transformers.gaudi_configuration import GaudiConfig
 
 
 logger = logging.get_logger(__name__)
@@ -78,30 +79,16 @@
         use_habana: bool = False,
         use_hpu_graphs: bool = False,
         gaudi_config: Union[str, GaudiConfig] = None,
     ):
         super().__init__()
 
         self.use_habana = use_habana
-        # HPU graphs and Gaudi configuration require `use_habana` to be True
-        if not use_habana:
-            if use_hpu_graphs:
-                raise ValueError(
-                    "`use_hpu_graphs` is True but `use_habana` is False, please set `use_habana=True` to use HPU"
-                    " graphs."
-                )
-            if gaudi_config is not None:
-                raise ValueError(
-                    "Got a non-None `gaudi_config` but `use_habana` is False, please set `use_habana=True` to use this"
-                    " Gaudi configuration."
-                )
-        self.use_hpu_graphs = use_hpu_graphs
-        self.gaudi_config = gaudi_config
-
         if self.use_habana:
+            self.use_hpu_graphs = use_hpu_graphs
             if self.use_hpu_graphs:
                 logger.info("Enabled HPU graphs.")
             else:
                 logger.info("Enabled lazy mode because `use_hpu_graphs=False`.")
 
             self._device = torch.device("hpu")
 
@@ -152,26 +139,40 @@
                         self.hmp.convert(
                             opt_level=self.gaudi_config.hmp_opt_level,
                             bf16_file_path=hmp_bf16_file.name,
                             fp32_file_path=hmp_fp32_file.name,
                             isVerbose=self.gaudi_config.hmp_is_verbose,
                         )
         else:
+            if use_hpu_graphs:
+                raise ValueError(
+                    "`use_hpu_graphs` is True but `use_habana` is False, please set `use_habana=True` to use HPU"
+                    " graphs."
+                )
+            if gaudi_config is not None:
+                raise ValueError(
+                    "Got a non-None `gaudi_config` but `use_habana` is False, please set `use_habana=True` to use this"
+                    " Gaudi configuration."
+                )
             logger.info("Running on CPU.")
             self._device = torch.device("cpu")
 
     def register_modules(self, **kwargs):
         # import it here to avoid circular import
         from diffusers import pipelines
 
         for name, module in kwargs.items():
             # retrieve library
             if module is None:
                 register_dict = {name: (None, None)}
             else:
+                # register the original module, not the dynamo compiled one
+                if is_compiled_module(module):
+                    module = module._orig_mod
+
                 library = module.__module__.split(".")[0]
                 if library == "optimum":
                     library = "optimum.habana.diffusers.schedulers"
 
                 # check if the module is a pipeline module
                 pipeline_dir = module.__module__.split(".")[-2] if len(module.__module__.split(".")) > 2 else None
                 path = module.__module__.split(".")
@@ -194,24 +195,27 @@
             # set models
             setattr(self, name, module)
 
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         safe_serialization: bool = False,
+        variant: Optional[str] = None,
     ):
         """
         Save the pipeline and Gaudi configurations.
         More information [here](https://huggingface.co/docs/diffusers/api/diffusion_pipeline#diffusers.DiffusionPipeline.save_pretrained).
 
         Arguments:
             save_directory (`str` or `os.PathLike`):
                 Directory to which to save. Will be created if it doesn't exist.
             safe_serialization (`bool`, *optional*, defaults to `False`):
                 Whether to save the model using `safetensors` or the traditional PyTorch way (that uses `pickle`).
+            variant (`str`, *optional*):
+                If specified, weights are saved in the format pytorch_model.<variant>.bin.
         """
         self.save_config(save_directory)
         if hasattr(self, "gaudi_config"):
             self.gaudi_config.save_pretrained(save_directory)
 
         model_index_dict = dict(self.config)
         model_index_dict.pop("_class_name")
@@ -229,14 +233,20 @@
 
         model_index_dict = {k: v for k, v in model_index_dict.items() if is_saveable_module(k, v)}
 
         for pipeline_component_name in model_index_dict.keys():
             sub_model = getattr(self, pipeline_component_name)
             model_cls = sub_model.__class__
 
+            # Dynamo wraps the original model in a private class.
+            # I didn't find a public API to get the original class.
+            if is_compiled_module(sub_model):
+                sub_model = sub_model._orig_mod
+                model_cls = sub_model.__class__
+
             save_method_name = None
             # search for the model's base class in GAUDI_LOADABLE_CLASSES
             for library_name, library_classes in GAUDI_LOADABLE_CLASSES.items():
                 library = importlib.import_module(library_name)
                 for base_class, save_load_methods in library_classes.items():
                     class_candidate = getattr(library, base_class, None)
                     if class_candidate is not None and issubclass(model_cls, class_candidate):
@@ -247,20 +257,23 @@
                     break
 
             save_method = getattr(sub_model, save_method_name)
 
             # Call the save method with the argument safe_serialization only if it's supported
             save_method_signature = inspect.signature(save_method)
             save_method_accept_safe = "safe_serialization" in save_method_signature.parameters
+            save_method_accept_variant = "variant" in save_method_signature.parameters
+
+            save_kwargs = {}
             if save_method_accept_safe:
-                save_method(
-                    os.path.join(save_directory, pipeline_component_name), safe_serialization=safe_serialization
-                )
-            else:
-                save_method(os.path.join(save_directory, pipeline_component_name))
+                save_kwargs["safe_serialization"] = safe_serialization
+            if save_method_accept_variant:
+                save_kwargs["variant"] = variant
+
+            save_method(os.path.join(save_directory, pipeline_component_name), **save_kwargs)
 
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path: Optional[Union[str, os.PathLike]], **kwargs):
         """
         More information [here](https://huggingface.co/docs/diffusers/api/diffusion_pipeline#diffusers.DiffusionPipeline.from_pretrained).
         """
```

### Comparing `optimum-habana-1.4.2/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-habana-1.5.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,26 +13,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 import time
 from dataclasses import dataclass
 from math import ceil
-from typing import Callable, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
 from diffusers.configuration_utils import FrozenDict
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 from diffusers.schedulers import KarrasDiffusionSchedulers
 from diffusers.utils import BaseOutput, deprecate
 from packaging import version
-from transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
 from optimum.utils import logging
 
 from ....transformers.gaudi_configuration import GaudiConfig
 from ....utils import speed_metrics
 from ..pipeline_utils import GaudiDiffusionPipeline
 
@@ -66,15 +67,15 @@
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
             A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
+        feature_extractor ([`CLIPImageProcessor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
         use_habana (bool, defaults to `False`):
             Whether to use Gaudi (`True`) or CPU (`False`).
         use_hpu_graphs (bool, defaults to `False`):
             Whether to use HPU graphs or not.
         gaudi_config (Union[str, [`GaudiConfig`]], defaults to `None`):
             Gaudi configuration to use. Can be a string to download it from the Hub.
@@ -87,15 +88,15 @@
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
         scheduler: KarrasDiffusionSchedulers,
         safety_checker: StableDiffusionSafetyChecker,
-        feature_extractor: CLIPFeatureExtractor,
+        feature_extractor: CLIPImageProcessor,
         requires_safety_checker: bool = True,
         use_habana: bool = False,
         use_hpu_graphs: bool = False,
         gaudi_config: Union[str, GaudiConfig] = None,
     ):
         super().__init__(
             use_habana,
@@ -184,15 +185,15 @@
     @property
     def _execution_device(self):
         r"""
         Returns the device on which the pipeline's models will be executed. After calling
         `pipeline.enable_sequential_cpu_offload()` the execution device can only be inferred from Accelerate's module
         hooks.
         """
-        if self.device != torch.device("meta") or not hasattr(self.unet, "_hf_hook"):
+        if not hasattr(self.unet, "_hf_hook"):
             return self.device
         for module in self.unet.modules():
             if (
                 hasattr(module, "_hf_hook")
                 and hasattr(module._hf_hook, "execution_device")
                 and module._hf_hook.execution_device is not None
             ):
@@ -217,18 +218,18 @@
                 prompt to be encoded
             device: (`torch.device`):
                 torch device
             num_images_per_prompt (`int`):
                 number of images that should be generated per prompt
             do_classifier_free_guidance (`bool`):
                 whether to use classifier free guidance or not
-            negative_ prompt (`str` or `List[str]`, *optional*):
+            negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. If not defined, one has to pass
-                `negative_prompt_embeds`. instead. If not defined, one has to pass `negative_prompt_embeds`. instead.
-                Ignored when not using guidance (i.e., ignored if `guidance_scale` is less than `1`).
+                `negative_prompt_embeds` instead. Ignored when not using guidance (i.e., ignored if `guidance_scale` is
+                less than `1`).
             prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt weighting. If not
                 provided, text embeddings will be generated from `prompt` input argument.
             negative_prompt_embeds (`torch.FloatTensor`, *optional*):
                 Pre-generated negative text embeddings. Can be used to easily tweak text inputs, *e.g.* prompt
                 weighting. If not provided, negative_prompt_embeds will be generated from `negative_prompt` input
                 argument.
@@ -339,18 +340,18 @@
                 images=image, clip_input=safety_checker_input.pixel_values.to(dtype)
             )
         else:
             has_nsfw_concept = None
         return image, has_nsfw_concept
 
     def decode_latents(self, latents):
-        latents = 1 / 0.18215 * latents
+        latents = 1 / self.vae.config.scaling_factor * latents
         image = self.vae.decode(latents).sample
         image = (image / 2 + 0.5).clamp(0, 1)
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloat16
         image = image.cpu().permute(0, 2, 3, 1).float().numpy()
         return image
 
     def prepare_extra_step_kwargs(self, generator, eta):
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
@@ -501,15 +502,16 @@
         generator: Optional[Union[torch.Generator, List[torch.Generator]]] = None,
         latents: Optional[torch.FloatTensor] = None,
         prompt_embeds: Optional[torch.FloatTensor] = None,
         negative_prompt_embeds: Optional[torch.FloatTensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, torch.FloatTensor], None]] = None,
-        callback_steps: Optional[int] = 1,
+        callback_steps: int = 1,
+        cross_attention_kwargs: Optional[Dict[str, Any]] = None,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts to guide the image generation. If not defined, one has to pass `prompt_embeds`.
@@ -525,16 +527,16 @@
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
                 1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
                 usually at the expense of lower image quality.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. If not defined, one has to pass
-                `negative_prompt_embeds`. instead. If not defined, one has to pass `negative_prompt_embeds`. instead.
-                Ignored when not using guidance (i.e., ignored if `guidance_scale` is less than `1`).
+                `negative_prompt_embeds` instead. Ignored when not using guidance (i.e., ignored if `guidance_scale` is
+                less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             batch_size (`int`, *optional*, defaults to 1):
                 The number of images in a batch.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
@@ -560,14 +562,18 @@
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
                 called with the following arguments: `callback(step: int, timestep: int, latents: torch.FloatTensor)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
+            cross_attention_kwargs (`dict`, *optional*):
+                A kwargs dictionary that if specified is passed along to the `AttentionProcessor` as defined under
+                `self.processor` in
+                [diffusers.cross_attention](https://github.com/huggingface/diffusers/blob/main/src/diffusers/models/cross_attention.py).
 
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple`.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
@@ -613,15 +619,15 @@
         )
 
         # 4. Prepare timesteps
         self.scheduler.set_timesteps(num_inference_steps, device="cpu")
         timesteps = self.scheduler.timesteps.to(device)
 
         # 5. Prepare latent variables
-        num_channels_latents = self.unet.in_channels
+        num_channels_latents = self.unet.config.in_channels
         latents = self.prepare_latents(
             num_prompts * num_images_per_prompt,
             num_channels_latents,
             height,
             width,
             prompt_embeds.dtype,
             device,
@@ -666,15 +672,21 @@
                 capture = True if self.use_hpu_graphs and i < 2 else False
 
                 # expand the latents if we are doing classifier free guidance
                 latent_model_input = torch.cat([latents_batch] * 2) if do_classifier_free_guidance else latents_batch
                 # latent_model_input = self.scheduler.scale_model_input(latent_model_input, timestep)
 
                 # predict the noise residual
-                noise_pred = self.unet_hpu(latent_model_input, timestep, text_embeddings_batch, capture)
+                noise_pred = self.unet_hpu(
+                    latent_model_input,
+                    timestep,
+                    text_embeddings_batch,
+                    cross_attention_kwargs,
+                    capture,
+                )
 
                 # perform guidance
                 if do_classifier_free_guidance:
                     noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                     noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
                 # compute the previous noisy sample x_t -> x_t-1
@@ -683,16 +695,19 @@
                 if not self.use_hpu_graphs:
                     self.htcore.mark_step()
 
                 # call the callback, if provided
                 if callback is not None and i % callback_steps == 0:
                     callback(i, timestep, latents_batch)
 
-            # 8. Post-processing
-            image = self.decode_latents(latents_batch)
+            if output_type == "latent":
+                image = latents_batch
+            else:
+                # 8. Post-processing
+                image = self.decode_latents(latents_batch)
             outputs["images"].append(image)
 
             self.scheduler.reset_timestep_dependent_params()
 
             if not self.use_hpu_graphs:
                 self.htcore.mark_step()
 
@@ -708,16 +723,19 @@
 
         # Remove dummy generations if needed
         if num_dummy_samples > 0:
             outputs["images"][-1] = outputs["images"][-1][:-num_dummy_samples]
 
         # Process generated images
         for i, image in enumerate(outputs["images"][:]):
-            # 9. Run safety checker
-            image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
+            if output_type == "latent":
+                has_nsfw_concept = None
+            else:
+                # 9. Run safety checker
+                image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
 
             if i == 0:
                 outputs["images"].clear()
 
             # 10. Convert to PIL
             if output_type == "pil":
                 image = self.numpy_to_pil(image)
@@ -736,19 +754,19 @@
         return GaudiStableDiffusionPipelineOutput(
             images=outputs["images"],
             nsfw_content_detected=outputs["has_nsfw_concept"],
             throughput=speed_measures[f"{speed_metrics_prefix}_samples_per_second"],
         )
 
     @torch.no_grad()
-    def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, capture):
+    def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs, capture):
         if self.use_hpu_graphs:
             return self.capture_replay(latent_model_input, timestep, encoder_hidden_states, capture)
         else:
-            return self.unet(latent_model_input, timestep, encoder_hidden_states).sample
+            return self.unet(latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs).sample
 
     @torch.no_grad()
     def capture_replay(self, latent_model_input, timestep, encoder_hidden_states, capture):
         inputs = [latent_model_input, timestep, encoder_hidden_states, False]
         h = self.ht.hpu.graphs.input_hash(inputs)
         cached = self.cache.get(h)
```

### Comparing `optimum-habana-1.4.2/optimum/habana/diffusers/schedulers/scheduling_ddim.py` & `optimum-habana-1.5.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # Copyright 2022 Stanford University Team and The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -37,53 +38,66 @@
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
+        clip_sample_range (`float`, default `1.0`):
+            the maximum magnitude for sample clipping. Valid only when `clip_sample=True`.
         set_alpha_to_one (`bool`, default `True`):
             each diffusion step uses the value of alphas product at that step and at the previous one. For the final
             step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
             otherwise it uses the value of alpha at step 0.
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
         prediction_type (`str`, default `epsilon`, optional):
             prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
             process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
             https://imagen.research.google/video/paper.pdf)
+        thresholding (`bool`, default `False`):
+            whether to use the "dynamic thresholding" method (introduced by Imagen, https://arxiv.org/abs/2205.11487).
+            Note that the thresholding method is unsuitable for latent-space diffusion models (such as
+            stable-diffusion).
+        dynamic_thresholding_ratio (`float`, default `0.995`):
+            the ratio for the dynamic thresholding method. Default is `0.995`, the same as Imagen
+            (https://arxiv.org/abs/2205.11487). Valid only when `thresholding=True`.
+        sample_max_value (`float`, default `1.0`):
+            the threshold value for dynamic thresholding. Valid only when `thresholding=True`.
     """
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
         trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
         clip_sample: bool = True,
         set_alpha_to_one: bool = True,
         steps_offset: int = 0,
         prediction_type: str = "epsilon",
-        **kwargs,
+        thresholding: bool = False,
+        dynamic_thresholding_ratio: float = 0.995,
+        clip_sample_range: float = 1.0,
+        sample_max_value: float = 1.0,
     ):
         super().__init__(
             num_train_timesteps,
             beta_start,
             beta_end,
             beta_schedule,
             trained_betas,
             clip_sample,
             set_alpha_to_one,
             steps_offset,
             prediction_type,
-            **kwargs,
         )
 
         self.reset_timestep_dependent_params()
 
     def reset_timestep_dependent_params(self):
         self.are_timestep_dependent_params_set = False
         self.alpha_prod_t_list = []
@@ -99,17 +113,17 @@
                     self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
                 )
 
                 self.alpha_prod_t_list.append(alpha_prod_t)
                 self.alpha_prod_t_prev_list.append(alpha_prod_t_prev)
                 self.variance_list.append(self._get_variance(alpha_prod_t, alpha_prod_t_prev))
 
-            self.alpha_prod_t_list = torch.stack([i for i in self.alpha_prod_t_list])
-            self.alpha_prod_t_prev_list = torch.stack([i for i in self.alpha_prod_t_prev_list])
-            self.variance_list = torch.stack([i for i in self.variance_list])
+            self.alpha_prod_t_list = torch.stack(self.alpha_prod_t_list)
+            self.alpha_prod_t_prev_list = torch.stack(self.alpha_prod_t_prev_list)
+            self.variance_list = torch.stack(self.variance_list)
             self.are_timestep_dependent_params_set = True
 
         alpha_prod_t = self.alpha_prod_t_list[0]
         self.alpha_prod_t_list = torch.roll(self.alpha_prod_t_list, shifts=-1, dims=0)
         alpha_prod_t_prev = self.alpha_prod_t_prev_list[0]
         self.alpha_prod_t_prev_list = torch.roll(self.alpha_prod_t_prev_list, shifts=-1, dims=0)
         variance = self.variance_list[0]
@@ -194,46 +208,50 @@
         alpha_prod_t, alpha_prod_t_prev, variance = self.get_params()
         beta_prod_t = 1 - alpha_prod_t
 
         # 3. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
         if self.config.prediction_type == "epsilon":
             pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+            pred_epsilon = model_output
         elif self.config.prediction_type == "sample":
             pred_original_sample = model_output
+            pred_epsilon = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
         elif self.config.prediction_type == "v_prediction":
             pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
-            # predict V
-            model_output = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
+            pred_epsilon = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
         else:
             raise ValueError(
                 f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
                 " `v_prediction`"
             )
 
-        # 4. Clip "predicted x_0"
-        if self.config.clip_sample:
-            pred_original_sample = torch.clamp(pred_original_sample, -1, 1)
+        # 4. Clip or threshold "predicted x_0"
+        if self.config.thresholding:
+            pred_original_sample = self._threshold_sample(pred_original_sample)
+        elif self.config.clip_sample:
+            pred_original_sample = pred_original_sample.clamp(
+                -self.config.clip_sample_range, self.config.clip_sample_range
+            )
 
         # 5. compute variance: "sigma_t(η)" -> see formula (16)
         # σ_t = sqrt((1 − α_t−1)/(1 − α_t)) * sqrt(1 − α_t/α_t−1)
         std_dev_t = eta * variance ** (0.5)
 
         if use_clipped_model_output:
-            # the model_output is always re-derived from the clipped x_0 in Glide
-            model_output = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
+            # the pred_epsilon is always re-derived from the clipped x_0 in Glide
+            pred_epsilon = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
 
         # 6. compute "direction pointing to x_t" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * model_output
+        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * pred_epsilon
 
         # 7. compute x_t without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
         prev_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
 
         if eta > 0:
-            # randn_like does not support generator https://github.com/pytorch/pytorch/issues/27072
             device = model_output.device
             if variance_noise is not None and generator is not None:
                 raise ValueError(
                     "Cannot pass both generator and variance_noise. Please make sure that either `generator` or"
                     " `variance_noise` stays `None`."
                 )
 
@@ -241,15 +259,15 @@
                 # torch.randn is broken on HPU so running it on CPU
                 variance_noise = torch.randn(
                     model_output.shape, dtype=model_output.dtype, device="cpu", generator=generator
                 )
                 if device.type == "hpu":
                     variance_noise = variance_noise.to(device)
 
-            prev_sample = prev_sample + variance ** (0.5) * eta * variance_noise
+            prev_sample = prev_sample + std_dev_t * variance_noise
 
         if not return_dict:
             return (prev_sample,)
 
         return DDIMSchedulerOutput(prev_sample=prev_sample, pred_original_sample=pred_original_sample)
 
     # def add_noise(
```

### Comparing `optimum-habana-1.4.2/optimum/habana/distributed/distributed_runner.py` & `optimum-habana-1.5.0/optimum/habana/distributed/distributed_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -26,15 +27,15 @@
 
 
 logger = logging.get_logger(__name__)
 
 
 class DistributedRunner:
     """
-    Set up training hardware configurations and run distributed training commands.
+    Set up training/inference hardware configurations and run distributed commands.
     """
 
     def __init__(
         self,
         command_list: List = [],
         world_size: int = 1,
         hostfile: Union[str, Path] = None,
@@ -78,42 +79,42 @@
 
         if use_deepspeed and use_mpi:
             raise ValueError("`use_mpi` and `use_deepspeed` cannot be both True.")
 
         if hostfile is not None:
             if isinstance(self._hostfile, str):
                 self._hostfile = Path(self._hostfile)
-            # Multi-node training
+            # Multi-node run
             if use_deepspeed:
                 self.create_multi_node_setup()
             else:
                 raise ValueError(
-                    "A hostfile is specified to perform multi-node training. This requires to enable DeepSpeed with"
+                    "A hostfile is specified to perform a multi-node run. This requires to enable DeepSpeed with"
                     " `use_deepspeed=True`."
                 )
         elif self._world_size > 1:
-            # Distributed training
+            # Distributed run
             if use_deepspeed:
-                # Single-node multi-card training with DeepSpeed
+                # Single-node multi-card run with DeepSpeed
                 self.create_single_node_setup_deepspeed()
             elif use_mpi:
-                # Single-node multi-card training with MPI
+                # Single-node multi-card run with MPI
                 self._model_env_vars["MASTER_ADDR"] = "localhost"
                 self._model_env_vars["MASTER_PORT"] = "12345"
                 self.create_single_node_setup_mpirun()
             else:
-                # Single-node multi-card training with torch.distributed
+                # Single-node multi-card run with torch.distributed
                 self.create_single_node_setup()
         else:
-            # Single-card training
+            # Single-card run
             logger.warning(
-                "The run will be executed on one device only. Specify `world_size` >= 1 or `hostfile` to perform a"
+                "The run will be executed on one device only. Specify `world_size` > 1 or `hostfile` to perform a"
                 " distributed run."
             )
-            self.create_single_card_setup()
+            self.create_single_card_setup(use_deepspeed)
 
     def get_peval(self):
         cmd1 = "lscpu 2>/dev/null | awk '/Socket\(s\)/  { print $2 }'"
         cmd2 = "lscpu 2>/dev/null | awk '/Core\(s\) per socket/  { print $4 }'"
         with subprocess.Popen(
             cmd1, shell=True, executable="/bin/bash", stdout=subprocess.PIPE, stderr=subprocess.STDOUT
         ) as proc:
@@ -137,20 +138,23 @@
             peval = (sockets * corespsocket) // self._world_size
         return peval, sockets, corespsocket
 
     def setup_config_env_mpirun(self):
         peval, _, _ = self.get_peval()
         return f"--map-by {self._map_by}:PE={peval}"
 
-    def create_single_card_setup(self):
+    def create_single_card_setup(self, use_deepspeed=False):
         """
         Single-card setup.
         """
 
-        self._interpreter = f"{sys.executable} "
+        if use_deepspeed:
+            self._interpreter = "deepspeed --num_gpus 1 "
+        else:
+            self._interpreter = f"{sys.executable} "
 
     def create_single_node_setup_mpirun(self):
         """
         Single-node multi-card configuration setup for mpirun.
         """
 
         mpi_cmd = self.setup_config_env_mpirun()
@@ -170,15 +174,15 @@
         """
         Single-node multi-card configuration setup.
         """
 
         use_env_param = "--use_env" if self._use_env else ""
 
         self._interpreter = (
-            f"{sys.executable} -um torch.distributed.launch --nproc_per_node={self._world_size} {use_env_param} "
+            f"{sys.executable} -um torch.distributed.run --nproc_per_node={self._world_size} {use_env_param} "
         )
 
     def create_multi_node_setup(self):
         """
         Multi-node configuration setup for DeepSpeed.
         """
 
@@ -242,15 +246,15 @@
                 try:
                     hostname, slots = line.split()
                     _, slot_count = slots.split("=")
                     slot_count = int(slot_count)
                     if master_addr is None:
                         master_addr = hostname
                 except ValueError as err:
-                    logger.error("Hostfile is not formatted correctly, unable to proceed with training.")
+                    logger.error("Hostfile is not formatted correctly, unable to proceed with training/inference.")
                     raise err
                 if hostname in resource_pool:
-                    logger.error("Hostfile contains duplicate hosts, unable to proceed with training.")
+                    logger.error("Hostfile contains duplicate hosts, unable to proceed with training/inference.")
                     raise ValueError(f"Host {hostname} is already defined")
                 resource_pool[hostname] = slot_count
 
         return master_addr
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/__init__.py` & `optimum-habana-1.5.0/optimum/habana/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/deepspeed.py` & `optimum-habana-1.5.0/optimum/habana/transformers/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # Copyright 2020 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -142,22 +143,22 @@
     HabanaArgs = make_dataclass("HabanaArgs", [("use_hpu", bool), ("no_cuda", bool)])
     habana_args = HabanaArgs(use_hpu=args.use_habana, no_cuda=args.no_cuda)
     if args.use_habana:
         # This env variable is initialized here to make sure it is set to "true"
         # It should be done by the launcher but it does not work for multi-node runs
         os.environ["DEEPSPEED_USE_HPU"] = "true"
 
-    kwargs = dict(
-        args=habana_args,
-        model=model,
-        model_parameters=model_parameters,
-        config_params=config,
-        optimizer=optimizer,
-        lr_scheduler=lr_scheduler,
-    )
+    kwargs = {
+        "args": habana_args,
+        "model": model,
+        "model_parameters": model_parameters,
+        "config_params": config,
+        "optimizer": optimizer,
+        "lr_scheduler": lr_scheduler,
+    }
 
     deepspeed_engine, optimizer, _, lr_scheduler = deepspeed.initialize(**kwargs)
 
     if resume_from_checkpoint is not None:
         # it's possible that the user is trying to resume from model_path, which doesn't necessarily
         # contain a deepspeed checkpoint. e.g. examples just check if the dir exists and assume it's
         # a resume from a checkpoint and not just a local pretrained weight. So we check here if the
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/gaudi_configuration.py` & `optimum-habana-1.5.0/optimum/habana/transformers/gaudi_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
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
 
+import warnings
 from pathlib import Path
 
 from optimum.configuration_utils import BaseConfig
 from optimum.utils import logging
 
 
 logger = logging.get_logger(__name__)
@@ -48,24 +50,31 @@
 class GaudiConfig(BaseConfig):
     CONFIG_NAME = "gaudi_config.json"
     FULL_CONFIGURATION_FILE = "gaudi_config.json"
 
     def __init__(self, **kwargs):
         # Habana Mixed Precision (MHP) configuration
         self.use_habana_mixed_precision = kwargs.pop("use_habana_mixed_precision", False)
-        self.hmp_opt_level = kwargs.pop("hmp_opt_level", "O1")
         self.hmp_bf16_ops = kwargs.pop("hmp_bf16_ops", DEFAULT_BF16_OPS)
         self.hmp_fp32_ops = kwargs.pop("hmp_fp32_ops", DEFAULT_FP32_OPS)
         self.hmp_is_verbose = kwargs.pop("hmp_is_verbose", False)
 
         # Use Habana's custom AdamW implementation
         self.use_fused_adam = kwargs.pop("use_fused_adam", False)
         # Use Habana's custom fused clip norm implementation
         self.use_fused_clip_norm = kwargs.pop("use_fused_clip_norm", False)
 
+        # TODO: to remove in a future version
+        if "hmp_opt_level" in kwargs:
+            warnings.warn(
+                "`hmp_opt_level` is deprecated and will be removed in a future version.",
+                FutureWarning,
+            )
+        self.hmp_opt_level = kwargs.pop("hmp_opt_level", "O1")
+
     def write_bf16_fp32_ops_to_text_files(
         self,
         path_to_bf16_file: Path,
         path_to_fp32_file: Path,
     ):
         for path, ops in zip(
             [Path(path_to_bf16_file), Path(path_to_fp32_file)], [self.hmp_bf16_ops, self.hmp_fp32_ops]
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/generation/utils.py` & `optimum-habana-1.5.0/optimum/habana/transformers/generation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import inspect
 import warnings
-from typing import Callable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import torch
 import torch.distributed as dist
+from transformers.deepspeed import is_deepspeed_zero3_enabled
 from transformers.generation.beam_constraints import DisjunctiveConstraint, PhrasalConstraint
 from transformers.generation.beam_search import BeamScorer, BeamSearchScorer, ConstrainedBeamSearchScorer
 from transformers.generation.configuration_utils import GenerationConfig
 from transformers.generation.logits_process import LogitsProcessorList
-from transformers.generation.stopping_criteria import StoppingCriteriaList, validate_stopping_criteria
+from transformers.generation.stopping_criteria import (
+    StoppingCriteria,
+    StoppingCriteriaList,
+    validate_stopping_criteria,
+)
 from transformers.generation.utils import (
     BeamSampleOutput,
     BeamSearchDecoderOnlyOutput,
     BeamSearchEncoderDecoderOutput,
     BeamSearchOutput,
     ContrastiveSearchOutput,
     GenerateOutput,
@@ -37,41 +42,108 @@
     GreedySearchDecoderOnlyOutput,
     GreedySearchEncoderDecoderOutput,
     GreedySearchOutput,
     SampleDecoderOnlyOutput,
     SampleEncoderDecoderOutput,
     SampleOutput,
 )
-from transformers.pytorch_utils import torch_int_div
+from transformers.utils import ModelOutput
 
 from optimum.utils import logging
 
 
+if TYPE_CHECKING:
+    from .streamers import BaseStreamer
+
+
 logger = logging.get_logger(__name__)
 
 
+class StaticMaxLengthCriteria(StoppingCriteria):
+    def __init__(self, max_steps: int):
+        self.max_steps = max_steps
+        self.cur_step = 0
+
+    def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
+        self.cur_step += 1
+        return self.cur_step >= self.max_steps
+
+
 class GaudiGenerationMixin(GenerationMixin):
     """
     This class enables to perform fast generation in lazy mode and with HPU graphs.
     The only difference with GenerationMixin is that the various generation
     methods will generate sequences whose size is max_length. Having constant
     sizes allows to make the most of lazy mode and HPU graphs.
     """
 
+    def _update_model_kwargs_for_generation(
+        self,
+        outputs: ModelOutput,
+        model_kwargs: Dict[str, Any],
+        is_encoder_decoder: bool = False,
+        standardize_cache_format: bool = False,
+    ) -> Dict[str, Any]:
+        # update past_key_values
+        model_kwargs["past_key_values"] = self._extract_past_from_model_output(
+            outputs, standardize_cache_format=standardize_cache_format
+        )
+
+        # update token_type_ids with last value
+        if "token_type_ids" in model_kwargs:
+            token_type_ids = model_kwargs["token_type_ids"]
+            model_kwargs["token_type_ids"] = torch.cat([token_type_ids, token_type_ids[:, -1].unsqueeze(-1)], dim=-1)
+
+        token_idx = model_kwargs.get("token_idx", None)
+
+        if not is_encoder_decoder:
+            # update attention mask
+            if "attention_mask" in model_kwargs:
+                attention_mask = model_kwargs["attention_mask"]
+                if token_idx is not None:
+                    attention_mask.index_fill_(1, token_idx, 1)
+                else:
+                    attention_mask = torch.cat(
+                        [attention_mask, attention_mask.new_ones((attention_mask.shape[0], 1))], dim=-1
+                    )
+                model_kwargs["attention_mask"] = attention_mask
+        else:
+            # update decoder attention mask
+            if "decoder_attention_mask" in model_kwargs:
+                decoder_attention_mask = model_kwargs["decoder_attention_mask"]
+                if token_idx is not None:
+                    decoder_attention_mask.index_fill_(1, token_idx, 1)
+                else:
+                    decoder_attention_mask = torch.cat(
+                        [
+                            decoder_attention_mask,
+                            decoder_attention_mask.new_ones((decoder_attention_mask.shape[0], 1)),
+                        ],
+                        dim=-1,
+                    )
+                model_kwargs["decoder_attention_mask"] = decoder_attention_mask
+
+        if token_idx is not None:
+            token_idx.add_(1)
+
+        return model_kwargs
+
     @torch.no_grad()
     def generate(
         self,
         inputs: Optional[torch.Tensor] = None,
         generation_config: Optional[GenerationConfig] = None,
         logits_processor: Optional[LogitsProcessorList] = None,
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         prefix_allowed_tokens_fn: Optional[Callable[[int, torch.Tensor], List[int]]] = None,
-        synced_gpus: Optional[bool] = False,
+        synced_gpus: Optional[bool] = None,
+        streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
         hpu_graphs: Optional[bool] = False,
+        ignore_eos: Optional[bool] = None,
         **kwargs,
     ) -> Union[GenerateOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head.
 
         <Tip warning={true}>
 
@@ -110,20 +182,27 @@
             prefix_allowed_tokens_fn (`Callable[[int, torch.Tensor], List[int]]`, *optional*):
                 If provided, this function constraints the beam search to allowed tokens only at each step. If not
                 provided no constraint is applied. This function takes 2 arguments: the batch ID `batch_id` and
                 `input_ids`. It has to return a list with the allowed tokens for the next generation step conditioned
                 on the batch ID `batch_id` and the previously generated tokens `inputs_ids`. This argument is useful
                 for constrained generation conditioned on the prefix, as described in [Autoregressive Entity
                 Retrieval](https://arxiv.org/abs/2010.00904).
-            synced_gpus (`bool`, *optional*, defaults to `False`):
-                Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
+            synced_gpus (`bool`, *optional*):
+                Whether to continue running the while loop until max_length. Unless overridden this flag will be set to
+                `True` under DeepSpeed ZeRO Stage 3 multiple GPUs environment to avoid hanging if one GPU finished
+                generating before other GPUs. Otherwise it'll be set to `False`.
+            streamer (`BaseStreamer`, *optional*):
+                Streamer object that will be used to stream the generated sequences. Generated tokens are passed
+                through `streamer.put(token_ids)` and the streamer is responsible for any further processing.
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
             hpu_graphs (`bool`, *optional*, defaults to `False`):
                 Whether to use HPU graphs for inference.
+            ignore_eos (`bool`, *optional*):
+                Whether to ignore finished sequences (faster in lazy mode and with HPU graphs) or not (eager mode).
             kwargs:
                 Ad hoc parametrization of `generate_config` and/or additional model-specific kwargs that will be
                 forwarded to the `forward` function of the model. If the model is an encoder-decoder model, encoder
                 specific kwargs should not be prefixed and decoder specific kwargs should be prefixed with *decoder_*.
 
         Return:
             [`transformers.utils.ModelOutput`] or `torch.LongTensor`: A [`transformers.generationutils.ModelOutput`] (if `return_dict_in_generate=True`
@@ -137,16 +216,28 @@
                 If the model is an encoder-decoder model (`model.config.is_encoder_decoder=True`), the possible
                 [`transformers.generationutils.ModelOutput`] types are:
                     - [`transformers.generation.GreedySearchEncoderDecoderOutput`],
                     - [`transformers.generation.SampleEncoderDecoderOutput`],
                     - [`transformers.generation.BeamSearchEncoderDecoderOutput`],
                     - [`transformers.generation.BeamSampleEncoderDecoderOutput`]
         """
+        if synced_gpus is None:
+            if is_deepspeed_zero3_enabled() and dist.get_world_size() > 1:
+                synced_gpus = True
+            else:
+                synced_gpus = False
+
         # 1. Handle `generation_config` and kwargs that might update it, and validate the `.generate()` call
         self._validate_model_class()
+        if hpu_graphs and not lazy_mode:
+            raise ValueError(
+                "`hpu_graphs` is True but `lazy_mode` is False. HPU graphs require `lazy_mode` to be set to True."
+            )
+        if ignore_eos is None:
+            ignore_eos = lazy_mode
 
         # priority: `generation_config` argument > `model.generation_config` (the default generation config)
         if generation_config is None:
             # legacy: users may modify the model configuration to control generation -- update the generation config
             # model attribute accordingly, if it was created from the model config
             if self.generation_config._from_model_config:
                 new_generation_config = GenerationConfig.from_model_config(self.config)
@@ -229,17 +320,24 @@
             input_ids = self._prepare_decoder_input_ids_for_generation(
                 batch_size,
                 decoder_start_token_id=generation_config.decoder_start_token_id,
                 bos_token_id=generation_config.bos_token_id,
                 model_kwargs=model_kwargs,
                 device=inputs_tensor.device,
             )
+
+            # conditional generation for multi-modal models.
+            if "input_ids" in model_kwargs and model_input_name == "pixel_values":
+                input_ids = torch.cat([input_ids, model_kwargs.pop("input_ids")], dim=-1)
         else:
             input_ids = inputs_tensor if model_input_name == "input_ids" else model_kwargs.pop("input_ids")
 
+        if streamer is not None:
+            streamer.put(input_ids.cpu())
+
         # 6. Prepare `max_length` depending on other stopping criteria.
         input_ids_seq_length = input_ids.shape[-1]
         has_default_max_length = kwargs.get("max_length") is None and generation_config.max_length is not None
         if has_default_max_length and generation_config.max_new_tokens is None:
             warnings.warn(
                 f"Using `max_length`'s default ({generation_config.max_length}) to control the generation length. "
                 "This behaviour is deprecated and will be removed from the config in v5 of Transformers -- we"
@@ -258,29 +356,30 @@
                 )
 
         if generation_config.min_length is not None and generation_config.min_length > generation_config.max_length:
             raise ValueError(
                 f"Unfeasible length constraints: the minimum length ({generation_config.min_length}) is larger than"
                 f" the maximum length ({generation_config.max_length})"
             )
-        if input_ids_seq_length >= generation_config.max_length:
+        if input_ids_seq_length >= generation_config.max_length and "token_idx" not in model_kwargs:
             input_ids_string = "decoder_input_ids" if self.config.is_encoder_decoder else "input_ids"
             logger.warning(
                 f"Input length of {input_ids_string} is {input_ids_seq_length}, but `max_length` is set to"
                 f" {generation_config.max_length}. This can lead to unexpected behavior. You should consider"
                 " increasing `max_new_tokens`."
             )
 
         # 7. determine generation mode
         is_constraint_gen_mode = (
             generation_config.constraints is not None or generation_config.force_words_ids is not None
         )
 
         is_contrastive_search_gen_mode = (
-            generation_config.top_k is not None
+            (generation_config.num_beams == 1)
+            and generation_config.top_k is not None
             and generation_config.top_k > 1
             and generation_config.do_sample is False
             and generation_config.penalty_alpha is not None
             and generation_config.penalty_alpha > 0
         )
 
         is_greedy_gen_mode = (
@@ -321,14 +420,19 @@
         if generation_config.num_beam_groups > generation_config.num_beams:
             raise ValueError("`num_beam_groups` has to be smaller or equal to `num_beams`")
         if is_group_beam_gen_mode and generation_config.do_sample is True:
             raise ValueError(
                 "Diverse beam search cannot be used in sampling mode. Make sure that `do_sample` is set to `False`."
             )
 
+        if streamer is not None and (generation_config.num_beams > 1):
+            raise ValueError(
+                "`streamer` cannot be used with beam search (yet!). Make sure that `num_beams` is set to 1."
+            )
+
         if self.device.type != input_ids.device.type:
             warnings.warn(
                 (
                     "You are calling .generate() with the `input_ids` being on a device type different"
                     f" than your model's device. `input_ids` is on {input_ids.device.type}, whereas the model"
                     f" is on {self.device.type}. You may experience unexpected behaviors or slower generation."
                     " Please make sure that you have put `input_ids` to the"
@@ -347,17 +451,24 @@
             logits_processor=logits_processor,
         )
 
         # 9. prepare stopping criteria
         stopping_criteria = self._get_stopping_criteria(
             generation_config=generation_config, stopping_criteria=stopping_criteria
         )
+        if "token_idx" in model_kwargs:
+            if generation_config.max_new_tokens is not None:
+                stopping_criteria.append(StaticMaxLengthCriteria(generation_config.max_new_tokens))
+            else:
+                raise ValueError(
+                    "You need to set `max_new_tokens` in your generation configuration to use static shapes."
+                )
 
         # In lazy mode, import Habana torch to be able to add mark_step()
-        if lazy_mode and not hpu_graphs:
+        if lazy_mode:
             import habana_frameworks.torch.core as htcore
 
             self.htcore_generation = htcore
 
         # 10. go into different generation modes
         if is_greedy_gen_mode:
             if generation_config.num_return_sequences > 1:
@@ -372,16 +483,17 @@
                 logits_processor=logits_processor,
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
+                streamer=streamer,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
+                ignore_eos=ignore_eos,
                 **model_kwargs,
             )
 
         elif is_contrastive_search_gen_mode:
             if generation_config.num_return_sequences > 1:
                 raise ValueError(
                     f"num_return_sequences has to be 1, but is {generation_config.num_return_sequences} when doing"
@@ -395,14 +507,15 @@
                 logits_processor=logits_processor,
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
+                streamer=streamer,
                 **model_kwargs,
             )
 
         elif is_sample_gen_mode:
             # 11. prepare logits warper
             logits_warper = self._get_logits_warper(generation_config)
 
@@ -421,16 +534,16 @@
                 logits_warper=logits_warper,
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
+                streamer=streamer,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
                 **model_kwargs,
             )
 
         elif is_beam_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -462,15 +575,14 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
                 **model_kwargs,
             )
 
         elif is_beam_sample_gen_mode:
             # 11. prepare logits warper
             logits_warper = self._get_logits_warper(generation_config)
 
@@ -503,15 +615,14 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
                 **model_kwargs,
             )
 
         elif is_group_beam_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -551,15 +662,14 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
                 **model_kwargs,
             )
 
         elif is_constraint_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -641,15 +751,14 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
-                hpu_graphs=hpu_graphs,
                 **model_kwargs,
             )
 
     @torch.no_grad()
     def contrastive_search(
         self,
         input_ids: torch.LongTensor,
@@ -661,16 +770,16 @@
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
+        streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
         **model_kwargs,
     ) -> Union[ContrastiveSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **contrastive search** and can
         be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -710,18 +819,19 @@
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
+            streamer (`BaseStreamer`, *optional*):
+                Streamer object that will be used to stream the generated sequences. Generated tokens are passed
+                through `streamer.put(token_ids)` and the streamer is responsible for any further processing.
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific keyword arguments will be forwarded to the `forward` function of the model.
                 If model is an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.ContrastiveSearchDecoderOnlyOutput`],
             [`transformers.generation.ContrastiveSearchEncoderDecoderOutput`] or `torch.LongTensor`: A `torch.LongTensor`
@@ -764,16 +874,17 @@
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
+        streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
+        ignore_eos: Optional[bool] = None,
         **model_kwargs,
     ) -> Union[GreedySearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **greedy decoding** and can be
         used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -809,18 +920,21 @@
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
+            streamer (`BaseStreamer`, *optional*):
+                Streamer object that will be used to stream the generated sequences. Generated tokens are passed
+                through `streamer.put(token_ids)` and the streamer is responsible for any further processing.
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
+            ignore_eos (`bool`, *optional*):
+                Whether to ignore finished sequences (faster in lazy mode and with HPU graphs) or not (eager mode).
             model_kwargs:
                 Additional model specific keyword arguments will be forwarded to the `forward` function of the model.
                 If model is an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.GreedySearchDecoderOnlyOutput`], [`transformers.generation.GreedySearchEncoderDecoderOutput`]
             or `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -904,18 +1018,22 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         # keep track of which sequences are already finished
-        unfinished_sequences = input_ids.new(input_ids.shape[0]).fill_(1)
+        if not ignore_eos:
+            unfinished_sequences = torch.ones(input_ids.shape[0], dtype=torch.long, device=input_ids.device)
 
         this_peer_finished = False  # used by synced_gpus only
         while True:
+            if lazy_mode:
+                self.htcore_generation.mark_step()
+
             if synced_gpus:
                 # Under synced_gpus the `forward` call must continue until all gpus complete their sequence.
                 # The following logic allows an early break if all peers finished generating their sequence
                 this_peer_finished_flag = torch.tensor(0.0 if this_peer_finished else 1.0).to(input_ids.device)
                 # send 0.0 if we finished, 1.0 otherwise
                 dist.all_reduce(this_peer_finished_flag, op=dist.ReduceOp.SUM)
                 # did all peers finish? the reduced sum will be 0.0 then
@@ -932,15 +1050,19 @@
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
 
             if synced_gpus and this_peer_finished:
                 continue  # don't waste resources running the code we don't need
 
-            next_token_logits = outputs.logits[:, -1, :]
+            token_idx = model_kwargs.get("token_idx", None)
+            if token_idx is not None and outputs.logits.shape[-2] > 1:
+                next_token_logits = torch.index_select(outputs.logits, -2, token_idx - 1)
+            else:
+                next_token_logits = outputs.logits[:, -1, :]
 
             # pre-process distribution
             next_tokens_scores = logits_processor(input_ids, next_token_logits)
 
             # Store scores, attentions and hidden_states when required
             if return_dict_in_generate:
                 if output_scores:
@@ -959,42 +1081,48 @@
                         else (outputs.hidden_states,)
                     )
 
             # argmax
             next_tokens = torch.argmax(next_tokens_scores, dim=-1)
 
             # finished sentences should have their next token be a padding token
-            if eos_token_id is not None:
+            if not ignore_eos and eos_token_id is not None:
                 if pad_token_id is None:
                     raise ValueError("If `eos_token_id` is defined, make sure that `pad_token_id` is defined.")
                 next_tokens = next_tokens * unfinished_sequences + pad_token_id * (1 - unfinished_sequences)
 
             # update generated ids, model inputs, and length for next step
-            input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
+            if token_idx is not None:
+                input_ids.index_copy_(
+                    1, token_idx, next_tokens.unsqueeze(-1) if next_tokens.dim() == 1 else next_tokens
+                )
+            else:
+                input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
+            if streamer is not None:
+                streamer.put(next_tokens.cpu())
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
 
             # if eos_token was found in one sentence, set sentence to finished
-            if eos_token_id_tensor is not None:
+            if not ignore_eos and eos_token_id_tensor is not None:
                 unfinished_sequences = unfinished_sequences.mul(
                     next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
                 )
 
-            if lazy_mode and not hpu_graphs:
-                self.htcore_generation.mark_step()
-
             # stop if we exceed the maximum length, or when each sentence is finished (eager mode only)
-            if stopping_criteria(input_ids, scores) or (unfinished_sequences.max() == 0 and not lazy_mode):
+            if (not ignore_eos and unfinished_sequences.max() == 0) or stopping_criteria(input_ids, scores):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
 
-        # input_ids = self._pad_tensors_to_max_len_lazy(input_ids, pad_token_id, 128)
+        if streamer is not None:
+            streamer.end()
+
         if return_dict_in_generate:
             if self.config.is_encoder_decoder:
                 return GreedySearchEncoderDecoderOutput(
                     sequences=input_ids,
                     scores=scores,
                     encoder_attentions=encoder_attentions,
                     encoder_hidden_states=encoder_hidden_states,
@@ -1022,16 +1150,16 @@
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
+        streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
         **model_kwargs,
     ) -> Union[SampleOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **multinomial sampling** and
         can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1070,18 +1198,19 @@
                 for more details.
             output_scores (`bool`, *optional*, defaults to `False`):
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
+            streamer (`BaseStreamer`, *optional*):
+                Streamer object that will be used to stream the generated sequences. Generated tokens are passed
+                through `streamer.put(token_ids)` and the streamer is responsible for any further processing.
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific kwargs will be forwarded to the `forward` function of the model. If model is
                 an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.SampleDecoderOnlyOutput`], [`transformers.generation.SampleEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -1185,19 +1314,22 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         # keep track of which sequences are already finished
-        unfinished_sequences = input_ids.new(input_ids.shape[0]).fill_(1)
+        unfinished_sequences = torch.ones(input_ids.shape[0], dtype=torch.long, device=input_ids.device)
 
         this_peer_finished = False  # used by synced_gpus only
         # auto-regressive generation
         while True:
+            if lazy_mode:
+                self.htcore_generation.mark_step()
+
             if synced_gpus:
                 # Under synced_gpus the `forward` call must continue until all gpus complete their sequence.
                 # The following logic allows an early break if all peers finished generating their sequence
                 this_peer_finished_flag = torch.tensor(0.0 if this_peer_finished else 1.0).to(input_ids.device)
                 # send 0.0 if we finished, 1.0 otherwise
                 dist.all_reduce(this_peer_finished_flag, op=dist.ReduceOp.SUM)
                 # did all peers finish? the reduced sum will be 0.0 then
@@ -1214,15 +1346,19 @@
                 output_attentions=output_attentions,
                 output_hidden_states=output_hidden_states,
             )
 
             if synced_gpus and this_peer_finished:
                 continue  # don't waste resources running the code we don't need
 
-            next_token_logits = outputs.logits[:, -1, :]
+            token_idx = model_kwargs.get("token_idx", None)
+            if token_idx is not None and outputs.logits.shape[-2] > 1:
+                next_token_logits = torch.index_select(outputs.logits, -2, token_idx - 1)
+            else:
+                next_token_logits = outputs.logits[:, -1, :]
 
             # pre-process distribution
             next_token_scores = logits_processor(input_ids, next_token_logits)
             next_token_scores = logits_warper(input_ids, next_token_scores)
 
             # Store scores, attentions and hidden_states when required
             if return_dict_in_generate:
@@ -1249,35 +1385,45 @@
             # finished sentences should have their next token be a padding token
             if eos_token_id is not None:
                 if pad_token_id is None:
                     raise ValueError("If `eos_token_id` is defined, make sure that `pad_token_id` is defined.")
                 next_tokens = next_tokens * unfinished_sequences + pad_token_id * (1 - unfinished_sequences)
 
             # update generated ids, model inputs, and length for next step
-            input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
+            if token_idx is not None:
+                input_ids.index_copy_(
+                    1, token_idx, next_tokens.unsqueeze(-1) if next_tokens.dim() == 1 else next_tokens
+                )
+            else:
+                input_ids = torch.cat([input_ids, next_tokens[:, None]], dim=-1)
+            if streamer is not None:
+                streamer.put(next_tokens.cpu())
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
 
             # if eos_token was found in one sentence, set sentence to finished
             if eos_token_id_tensor is not None:
                 unfinished_sequences = unfinished_sequences.mul(
                     next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
                 )
 
-            if lazy_mode and not hpu_graphs:
-                self.htcore_generation.mark_step()
+            # if lazy_mode and not hpu_graphs:
+            #     self.htcore_generation.mark_step()
 
             # stop if we exceed the maximum length, or when each sentence is finished (eager mode only)
             if stopping_criteria(input_ids, scores) or (unfinished_sequences.max() == 0 and not lazy_mode):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
 
+        if streamer is not None:
+            streamer.end()
+
         if return_dict_in_generate:
             if self.config.is_encoder_decoder:
                 return SampleEncoderDecoderOutput(
                     sequences=input_ids,
                     scores=scores,
                     encoder_attentions=encoder_attentions,
                     encoder_hidden_states=encoder_hidden_states,
@@ -1306,15 +1452,14 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
         **model_kwargs,
     ) -> Union[BeamSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **beam search decoding** and
         can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1354,16 +1499,14 @@
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific kwargs will be forwarded to the `forward` function of the model. If model is
                 an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.utils.BeamSearchDecoderOnlyOutput`], [`transformers.generation.BeamSearchEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -1543,15 +1686,15 @@
             next_token_scores = next_token_scores.view(batch_size, num_beams * vocab_size)
 
             # Sample 2 next tokens for each beam (so we have some spare tokens and match output of beam search)
             next_token_scores, next_tokens = torch.topk(
                 next_token_scores, 2 * num_beams, dim=1, largest=True, sorted=True
             )
 
-            next_indices = torch_int_div(next_tokens, vocab_size)
+            next_indices = torch.div(next_tokens, vocab_size, rounding_mode="floor")
             next_tokens = next_tokens % vocab_size
 
             # stateless
             beam_outputs = beam_scorer.process(
                 input_ids,
                 next_token_scores,
                 next_tokens,
@@ -1575,16 +1718,16 @@
 
             if return_dict_in_generate and output_scores:
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
             cur_len = cur_len + 1
 
-            if lazy_mode and not hpu_graphs:
-                self.htcore_generation.mark_step()
+            # if lazy_mode and not hpu_graphs:
+            #     self.htcore_generation.mark_step()
 
             if stopping_criteria(input_ids, scores) or (beam_scorer.is_done and not lazy_mode):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
 
@@ -1639,15 +1782,14 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
         **model_kwargs,
     ) -> Union[BeamSampleOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **beam search multinomial
         sampling** and can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1691,16 +1833,14 @@
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific kwargs will be forwarded to the `forward` function of the model. If model is
                 an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.BeamSampleDecoderOnlyOutput`], [`transformers.generation.BeamSampleEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -1830,16 +1970,14 @@
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific kwargs that will be forwarded to the `forward` function of the model. If
                 model is an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.BeamSearchDecoderOnlyOutput`], [`transformers.generation.BeamSearchEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -1917,15 +2055,14 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = None,
         lazy_mode: Optional[bool] = False,
-        hpu_graphs: Optional[bool] = False,
         **model_kwargs,
     ) -> Union[BeamSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **constrained beam search
         decoding** and can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1970,16 +2107,14 @@
                 Whether or not to return the prediction scores. See `scores` under returned tensors for more details.
             return_dict_in_generate (`bool`, *optional*, defaults to `False`):
                 Whether or not to return a [`transformers.generationutils.ModelOutput`] instead of a plain tuple.
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
-            hpu_graphs (`bool`, *optional*, defaults to `False`):
-                Whether to use HPU graphs for inference.
             model_kwargs:
                 Additional model specific kwargs will be forwarded to the `forward` function of the model. If model is
                 an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.utils.BeamSearchDecoderOnlyOutput`], [`transformers.generation.BeamSearchEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/gradient_checkpointing.py` & `optimum-habana-1.5.0/optimum/habana/transformers/gradient_checkpointing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# coding=utf-8
+# Copyright 2022 The HuggingFace Inc. team.
+# Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
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
 # This file just adds a mark_step() at the beginning of the
 # backward pass when gradient checkpointing is performed
 # Original implementation here: https://github.com/pytorch/pytorch/blob/v1.10.2/torch/utils/checkpoint.py
 
 import warnings
 from typing import Any, Iterable, Tuple
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/modeling_utils.py` & `optimum-habana-1.5.0/optimum/habana/transformers/modeling_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
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
 
-import transformers.models.gpt2.modeling_gpt2
+import transformers.models.bloom.modeling_bloom as modeling_bloom
+import transformers.models.gpt2.modeling_gpt2 as modeling_gpt2
 from transformers.generation import GenerationMixin
 from transformers.modeling_utils import ModuleUtilsMixin
 from transformers.models.albert.modeling_albert import AlbertModel
 from transformers.models.vit.modeling_vit import ViTSelfAttention
 from transformers.models.wav2vec2.modeling_wav2vec2 import Wav2Vec2Model
 
 from .generation import GaudiGenerationMixin
 from .models import (
+    GaudiBloomForCausalLM,
+    GaudiBloomMLP,
+    GaudiBloomModel,
     GaudiGPT2Attention,
     gaudi_albert_forward,
+    gaudi_bloom_attention_forward,
+    gaudi_bloom_block_forward,
     gaudi_get_extended_attention_mask,
     gaudi_invert_attention_mask,
     gaudi_vit_self_attention_forward,
     gaudi_wav2vec2_forward,
 )
 
 
@@ -46,24 +53,32 @@
     # modeling_wav2vec2._compute_mask_indices = _gaudi_wav2vec2_compute_mask_indices
     # modeling_wav2vec2._sample_negative_indices = _gaudi_wav2vec2_sample_negative_indices
     # Wav2Vec2Model._mask_hidden_states = _gaudi_wav2vec2_mask_hidden_states
     Wav2Vec2Model.forward = gaudi_wav2vec2_forward
 
     # Generation is modified to run faster in lazy mode
     GenerationMixin.generate = GaudiGenerationMixin.generate
+    GenerationMixin._update_model_kwargs_for_generation = GaudiGenerationMixin._update_model_kwargs_for_generation
     GenerationMixin.greedy_search = GaudiGenerationMixin.greedy_search
     GenerationMixin.sample = GaudiGenerationMixin.sample
     GenerationMixin.beam_search = GaudiGenerationMixin.beam_search
     GenerationMixin.beam_sample = GaudiGenerationMixin.beam_sample
     GenerationMixin.group_beam_search = GaudiGenerationMixin.group_beam_search
     GenerationMixin.constrained_beam_search = GaudiGenerationMixin.constrained_beam_search
 
+    # Optimization for BLOOM generation on Gaudi
+    modeling_bloom.BloomAttention.forward = gaudi_bloom_attention_forward
+    modeling_bloom.BloomBlock.forward = gaudi_bloom_block_forward
+    modeling_bloom.BloomModel = GaudiBloomModel
+    modeling_bloom.BloomMLP = GaudiBloomMLP
+    modeling_bloom.BloomForCausalLM = GaudiBloomForCausalLM
+
     # Replace invert_attention_mask and get_extended_attention_mask
     # so that HMP is disabled for specific parts of the code
     ModuleUtilsMixin.invert_attention_mask = gaudi_invert_attention_mask
     ModuleUtilsMixin.get_extended_attention_mask = gaudi_get_extended_attention_mask
     # AlbertModel.forward does not rely on get_extended_attention_mask so it also needs to be replaced
     AlbertModel.forward = gaudi_albert_forward
 
     # From Transformers 4.27, the bias in the GPT2Attention layer is a Boolean
     # Since HCCL cannot handle this dtype, we revert it back to uint8 (same behaviour as Transformers <= 4.26)
-    transformers.models.gpt2.modeling_gpt2.GPT2Attention = GaudiGPT2Attention
+    modeling_gpt2.GPT2Attention = GaudiGPT2Attention
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/models/gpt2/modeling_gpt2.py` & `optimum-habana-1.5.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py` & `optimum-habana-1.5.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# coding=utf-8
+# Copyright 2022 The HuggingFace Inc. team.
+# Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
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
 from transformers.modeling_outputs import Wav2Vec2BaseModelOutput
 
 
 def _gaudi_wav2vec2_compute_mask_indices(
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/trainer.py` & `optimum-habana-1.5.0/optimum/habana/transformers/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
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
 
 import copy
 import math
 import os
 import random
 import shutil
 import sys
@@ -35,18 +36,22 @@
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 from transformers.integrations import hp_params
 from transformers.modeling_utils import PreTrainedModel, unwrap_model
 from transformers.pytorch_utils import ALL_LAYERNORM_LAYERS
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from transformers.trainer_callback import TrainerCallback, TrainerState
 from transformers.trainer_pt_utils import (
+    DistributedLengthGroupedSampler,
+    DistributedSamplerWithLoop,
     DistributedTensorGatherer,
     IterableDatasetShard,
+    LengthGroupedSampler,
     SequentialDistributedSampler,
     find_batch_size,
+    get_model_param_count,
     get_parameter_names,
     nested_concat,
     nested_detach,
     nested_numpify,
     nested_truncate,
     reissue_pt_warnings,
 )
@@ -61,15 +66,21 @@
     denumpify_detensorize,
     enable_full_determinism,
     find_executable_batch_size,
     get_last_checkpoint,
     has_length,
 )
 from transformers.training_args import TrainingArguments
-from transformers.utils import CONFIG_NAME, WEIGHTS_NAME
+from transformers.utils import (
+    CONFIG_NAME,
+    SAFE_WEIGHTS_NAME,
+    WEIGHTS_NAME,
+    is_datasets_available,
+    is_safetensors_available,
+)
 
 from optimum.utils import logging
 
 from ..utils import (
     get_hpu_memory_stats,
     set_seed,
     speed_metrics,
@@ -77,14 +88,22 @@
 )
 from .deepspeed import deepspeed_init
 from .gaudi_configuration import GAUDI_CONFIG_NAME, GaudiConfig
 from .trainer_utils import convert_into_dtypes, get_dtype
 from .training_args import GaudiTrainingArguments
 
 
+if is_datasets_available():
+    import datasets
+
+
+if is_safetensors_available():
+    import safetensors.torch
+
+
 if TYPE_CHECKING:
     import optuna
 
 
 logger = logging.get_logger(__name__)
 
 
@@ -202,14 +221,94 @@
 
         # Suppress PyTorch autocast warnings with Wav2Vec2
         # This is a bug in PyTorch
         warnings.filterwarnings(
             "ignore", message="User provided device_type of 'cuda', but CUDA is not available. Disabling"
         )
 
+    def _get_train_sampler(self) -> Optional[torch.utils.data.Sampler]:
+        if self.train_dataset is None or not has_length(self.train_dataset):
+            return None
+
+        generator = None
+        if self.args.world_size <= 1:
+            generator = torch.Generator()
+            # for backwards compatibility, we generate a seed here (which is sampled from a generator seeded with
+            # `args.seed`) if data_seed isn't provided.
+            # Further on in this method, we default to `args.seed` instead.
+            if self.args.data_seed is None:
+                seed = int(torch.empty((), dtype=torch.int64).random_().item())
+            else:
+                seed = self.args.data_seed
+            generator.manual_seed(seed)
+
+        seed = self.args.data_seed if self.args.data_seed is not None else self.args.seed
+
+        # Build the sampler.
+        if self.args.group_by_length:
+            if is_datasets_available() and isinstance(self.train_dataset, datasets.Dataset):
+                lengths = (
+                    self.train_dataset[self.args.length_column_name]
+                    if self.args.length_column_name in self.train_dataset.column_names
+                    else None
+                )
+            else:
+                lengths = None
+            model_input_name = self.tokenizer.model_input_names[0] if self.tokenizer is not None else None
+            if self.args.world_size <= 1:
+                return LengthGroupedSampler(
+                    self.args.train_batch_size * self.args.gradient_accumulation_steps,
+                    dataset=self.train_dataset,
+                    lengths=lengths,
+                    model_input_name=model_input_name,
+                    generator=generator,
+                )
+            else:
+                return DistributedLengthGroupedSampler(
+                    self.args.train_batch_size * self.args.gradient_accumulation_steps,
+                    dataset=self.train_dataset,
+                    num_replicas=self.args.world_size,
+                    rank=self.args.process_index,
+                    lengths=lengths,
+                    model_input_name=model_input_name,
+                    seed=seed,
+                )
+
+        else:
+            if self.args.world_size <= 1:
+                num_samples = len(self.train_dataset)
+                if (
+                    self.args.use_lazy_mode
+                    and not self.args.dataloader_drop_last
+                    and len(self.train_dataset) % self.args.per_device_train_batch_size != 0
+                ):
+                    # Make the total number of samples divisible by the batch size in lazy mode if needed
+                    num_samples += (
+                        self.args.per_device_train_batch_size
+                        - len(self.train_dataset) % self.args.per_device_train_batch_size
+                    )
+                return RandomSampler(self.train_dataset, num_samples=num_samples, generator=generator)
+            else:
+                if self.args.use_lazy_mode and not self.args.dataloader_drop_last:
+                    # Use a loop for HPUs when drop_last is False to have all batches have the same size
+                    return DistributedSamplerWithLoop(
+                        self.train_dataset,
+                        batch_size=self.args.per_device_train_batch_size,
+                        num_replicas=self.args.world_size,
+                        rank=self.args.process_index,
+                        seed=seed,
+                    )
+                else:
+                    return DistributedSampler(
+                        self.train_dataset,
+                        num_replicas=self.args.world_size,
+                        rank=self.args.process_index,
+                        seed=seed,
+                    )
+
     def create_optimizer(self):
         """
         Setup the optimizer.
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
         Trainer's init through `optimizers`, or subclass and override this method in a subclass.
         """
         if self.optimizer is None:
@@ -303,14 +402,19 @@
             model = torch.nn.parallel.DistributedDataParallel(
                 model,
                 device_ids=[self.args.local_rank] if self.args._n_gpu != 0 and not self.args.use_habana else None,
                 output_device=self.args.local_rank if self.args._n_gpu != 0 and not self.args.use_habana else None,
                 **kwargs,
             )
 
+        # torch.compile() needs to be called after wrapping the model with FSDP or DDP
+        # to ensure that it accounts for the graph breaks required by those wrappers
+        if self.args.torch_compile:
+            model = torch.compile(model, backend=self.args.torch_compile_backend, mode=self.args.torch_compile_mode)
+
         return model
 
     def train(
         self,
         resume_from_checkpoint: Optional[Union[str, bool]] = None,
         trial: Union["optuna.Trial", Dict[str, Any]] = None,
         ignore_keys_for_eval: Optional[List[str]] = None,
@@ -391,14 +495,58 @@
         return inner_training_loop(
             args=args,
             resume_from_checkpoint=resume_from_checkpoint,
             trial=trial,
             ignore_keys_for_eval=ignore_keys_for_eval,
         )
 
+    def training_step(self, model: torch.nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
+        """
+        Perform a training step on a batch of inputs.
+
+        Subclass and override to inject custom behavior.
+
+        Args:
+            model (`torch.nn.Module`):
+                The model to train.
+            inputs (`Dict[str, Union[torch.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
+                argument `labels`. Check your model's documentation for all accepted arguments.
+
+        Return:
+            `torch.Tensor`: The tensor with training loss on this batch.
+        """
+        model.train()
+        inputs = self._prepare_inputs(inputs)
+
+        with self.compute_loss_context_manager():
+            loss = self.compute_loss(model, inputs)
+
+        if self.args.n_gpu > 1:
+            loss = loss.mean()  # mean() to average on multi-gpu parallel training
+
+        if self.args.gradient_accumulation_steps > 1 and not self.deepspeed:
+            # deepspeed handles loss scaling by gradient_accumulation_steps in its `backward`
+            loss = loss / self.args.gradient_accumulation_steps
+
+        if self.args.pipelining_fwd_bwd:
+            self.htcore.mark_step()
+
+        if self.do_grad_scaling:
+            self.scaler.scale(loss).backward()
+        elif self.deepspeed:
+            # loss gets scaled under gradient_accumulation_steps in deepspeed
+            loss = self.deepspeed.backward(loss)
+        else:
+            loss.backward()
+
+        return loss.detach()
+
     def _inner_training_loop(
         self,
         batch_size=None,
         args=None,
         resume_from_checkpoint=None,
         trial=None,
         ignore_keys_for_eval=None,
@@ -508,23 +656,21 @@
 
         # important: at this point:
         # self.model         is the Transformers Model
         # self.model_wrapped is DDP(Transformers Model), Deepspeed(Transformers Model), etc.
 
         # Train!
         logger.info("***** Running training *****")
-        logger.info(f"  Num examples = {num_examples}")
-        logger.info(f"  Num Epochs = {num_train_epochs}")
-        logger.info(f"  Instantaneous batch size per device = {args.per_device_train_batch_size}")
-        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size}")
+        logger.info(f"  Num examples = {num_examples:,}")
+        logger.info(f"  Num Epochs = {num_train_epochs:,}")
+        logger.info(f"  Instantaneous batch size per device = {args.per_device_train_batch_size:,}")
+        logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size:,}")
         logger.info(f"  Gradient Accumulation steps = {args.gradient_accumulation_steps}")
-        logger.info(f"  Total optimization steps = {max_steps}")
-        logger.info(
-            f"  Number of trainable parameters = {sum(p.numel() for p in model.parameters() if p.requires_grad)}"
-        )
+        logger.info(f"  Total optimization steps = {max_steps:,}")
+        logger.info(f"  Number of trainable parameters = {get_model_param_count(model, trainable_only=True):,}")
 
         self.state.epoch = 0
         start_time = time.time()
         start_time_after_warmup = None
         epochs_trained = 0
         steps_trained_in_current_epoch = 0
         steps_trained_progress_bar = None
@@ -827,26 +973,24 @@
                 return
 
         checkpoint_rng_state = torch.load(rng_file)
         random.setstate(checkpoint_rng_state["python"])
         np.random.set_state(checkpoint_rng_state["numpy"])
         torch.random.set_rng_state(checkpoint_rng_state["cpu"])
         if self.args.use_habana:
-            # TODO: uncomment the code block below when torch.hpu.random.get_rng_state_all is fixed in SynapseAI
-            # if self.args.local_rank != -1:
-            #     self.hpu_random.set_rng_state(checkpoint_rng_state["hpu"])
-            # else:
-            #     try:
-            #         self.hpu_random.set_rng_state_all(checkpoint_rng_state["hpu"])
-            #     except Exception as e:
-            #         logger.info(
-            #             f"Didn't manage to set back the RNG states of the HPU because of the following error:\n {e}"
-            #             "\nThis won't yield the same results as if the training had not been interrupted."
-            #         )
-            self.hpu_random.set_rng_state(checkpoint_rng_state["hpu"])
+            if self.args.local_rank != -1:
+                self.hpu_random.set_rng_state(checkpoint_rng_state["hpu"])
+            else:
+                try:
+                    self.hpu_random.set_rng_state_all(checkpoint_rng_state["hpu"])
+                except Exception as e:
+                    logger.info(
+                        f"Didn't manage to set back the RNG states of the HPU because of the following error:\n {e}"
+                        "\nThis won't yield the same results as if the training had not been interrupted."
+                    )
 
     def _save_checkpoint(self, model, trial, metrics=None):
         # In all cases, including ddp/dp/deepspeed, self.model is always a reference to the model we
         # want to save except FullyShardedDDP.
         # assert unwrap_model(model) is self.model, "internal model should be a reference to self.model"
 
         # Save model checkpoint
@@ -908,21 +1052,19 @@
         rng_states = {
             "python": random.getstate(),
             "numpy": np.random.get_state(),
             "cpu": torch.random.get_rng_state(),
         }
 
         if self.args.use_habana:
-            # TODO: uncomment the code block below when torch.hpu.random.get_rng_state_all is fixed in SynapseAI
-            # if self.args.local_rank == -1:
-            #     # In non distributed, we save the global HPU RNG state
-            #     rng_states["hpu"] = self.hpu_random.get_rng_state_all()
-            # else:
-            #     rng_states["hpu"] = self.hpu_random.get_rng_state()
-            rng_states["hpu"] = self.hpu_random.get_rng_state()
+            if self.args.local_rank == -1:
+                # In non distributed, we save the global HPU RNG state
+                rng_states["hpu"] = self.hpu_random.get_rng_state_all()
+            else:
+                rng_states["hpu"] = self.hpu_random.get_rng_state()
 
         # A process can arrive here before the process 0 has a chance to save the model, in which case output_dir may
         # not yet exist.
         os.makedirs(output_dir, exist_ok=True)
 
         if self.args.world_size <= 1:
             torch.save(rng_states, os.path.join(output_dir, "rng_state.pth"))
@@ -1004,28 +1146,21 @@
             self.deepspeed = deepspeed_engine
 
         model = self._wrap_model(self.model, training=False, dataloader=dataloader)
         model.eval()
 
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
         if args.use_hpu_graphs and not self.is_in_train:
-            if self.args.local_rank == -1:
-                logger.info("Using HPU graphs for inference.")
-                if not self.already_wrapped_for_hpu_graphs:
-                    # Do not wrap the model in HPU graphs if it has already been done
-                    from habana_frameworks.torch.hpu import wrap_in_hpu_graph
+            logger.info("Using HPU graphs for inference.")
+            # Do not wrap the model in HPU graphs if it has already been done
+            if not self.already_wrapped_for_hpu_graphs:
+                from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
-                    model = wrap_in_hpu_graph(model)
-                    self.already_wrapped_for_hpu_graphs = True
-            else:
-                # Do not use HPU graphs for distributed runs
-                logger.warning(
-                    "HPU graphs have not been validated for distributed runs yet. Disabling it, inference will be"
-                    " performed in lazy mode."
-                )
+                model = wrap_in_hpu_graph(model)
+                self.already_wrapped_for_hpu_graphs = True
 
         batch_size = self.args.eval_batch_size
 
         logger.info(f"***** Running {description} *****")
         if has_length(dataloader):
             logger.info(f"  Num examples = {self.num_examples(dataloader)}")
         else:
@@ -1213,23 +1348,23 @@
         prediction_loss_only: bool,
         ignore_keys: Optional[List[str]] = None,
     ) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
         """
         Perform an evaluation step on `model` using `inputs`.
         Subclass and override to inject custom behavior.
         Args:
-            model (`nn.Module`):
+            model (`torch.nn.Module`):
                 The model to evaluate.
             inputs (`Dict[str, Union[torch.Tensor, Any]]`):
                 The inputs and targets of the model.
                 The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
                 argument `labels`. Check your model's documentation for all accepted arguments.
             prediction_loss_only (`bool`):
                 Whether or not to return the loss only.
-            ignore_keys (`Lst[str]`, *optional*):
+            ignore_keys (`List[str]`, *optional*):
                 A list of keys in the output of your model (if it is a dictionary) that should be ignored when
                 gathering predictions.
         Return:
             Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss,
             logits and labels (each being optional).
         """
         has_labels = False if len(self.label_names) == 0 else all(inputs.get(k) is not None for k in self.label_names)
@@ -1333,28 +1468,21 @@
             deepspeed_engine.lr_scheduler = None
 
         model = self._wrap_model(self.model, training=False, dataloader=dataloader)
         model.eval()
 
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
         if args.use_hpu_graphs and not self.is_in_train:
-            if self.args.local_rank == -1:
-                logger.info("Using HPU graphs for inference.")
-                if not self.already_wrapped_for_hpu_graphs:
-                    # Do not wrap the model in HPU graphs if it has already been done
-                    from habana_frameworks.torch.hpu import wrap_in_hpu_graph
+            logger.info("Using HPU graphs for inference.")
+            # Do not wrap the model in HPU graphs if it has already been done
+            if not self.already_wrapped_for_hpu_graphs:
+                from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
-                    model = wrap_in_hpu_graph(model)
-                    self.already_wrapped_for_hpu_graphs = True
-            else:
-                # Do not use HPU graphs for distributed runs
-                logger.warning(
-                    "HPU graphs have not been validated for distributed runs yet. Disabling it, inference will be"
-                    " performed in lazy mode."
-                )
+                model = wrap_in_hpu_graph(model)
+                self.already_wrapped_for_hpu_graphs = True
 
         batch_size = dataloader.batch_size
         num_examples = self.num_examples(dataloader)
         logger.info(f"***** Running {description} *****")
         logger.info(f"  Num examples = {num_examples}")
         logger.info(f"  Batch size = {batch_size}")
         losses_host: torch.Tensor = None
@@ -1507,20 +1635,27 @@
             # state_dict items have to be saved on the CPU
             state_dict = to_device_dtype(state_dict, target_device=torch.device("cpu"))
 
         # Save a trained model and configuration using `save_pretrained()`.
         # They can then be reloaded using `from_pretrained()`
         if not isinstance(self.model, PreTrainedModel):
             if isinstance(unwrap_model(self.model), PreTrainedModel):
-                unwrap_model(self.model).save_pretrained(output_dir, state_dict=state_dict)
+                unwrap_model(self.model).save_pretrained(
+                    output_dir, state_dict=state_dict, safe_serialization=self.args.save_safetensors
+                )
             else:
                 logger.info("Trainer.model is not a `PreTrainedModel`, only saving its state dict.")
-                torch.save(state_dict, os.path.join(output_dir, WEIGHTS_NAME))
+                if self.args.save_safetensors:
+                    safetensors.torch.save_file(state_dict, os.path.join(output_dir, SAFE_WEIGHTS_NAME))
+                else:
+                    torch.save(state_dict, os.path.join(output_dir, WEIGHTS_NAME))
         else:
-            self.model.save_pretrained(output_dir, state_dict=state_dict)
+            self.model.save_pretrained(
+                output_dir, state_dict=state_dict, safe_serialization=self.args.save_safetensors
+            )
 
         if self.tokenizer is not None:
             self.tokenizer.save_pretrained(output_dir)
 
         self.gaudi_config.save_pretrained(output_dir)
 
         # Good practice: save your training arguments together with the trained model
@@ -1532,15 +1667,15 @@
             return
         # If we haven't finished the last push, we don't do this one.
         if self.push_in_progress is not None and not self.push_in_progress.is_done:
             return
 
         output_dir = self.args.output_dir
         # To avoid a new synchronization of all model weights, we just copy the file from the checkpoint folder
-        modeling_files = [CONFIG_NAME, WEIGHTS_NAME, GAUDI_CONFIG_NAME]
+        modeling_files = [CONFIG_NAME, WEIGHTS_NAME, SAFE_WEIGHTS_NAME, GAUDI_CONFIG_NAME]
         for modeling_file in modeling_files:
             if os.path.isfile(os.path.join(checkpoint_folder, modeling_file)):
                 shutil.copy(os.path.join(checkpoint_folder, modeling_file), os.path.join(output_dir, modeling_file))
         # Saving the tokenizer is fast and we don't know how many files it may have spawned, so we resave it to be sure.
         if self.tokenizer is not None:
             self.tokenizer.save_pretrained(output_dir)
         # Same for the training arguments
@@ -1567,16 +1702,17 @@
             if self.args.hub_strategy == HubStrategy.CHECKPOINT:
                 # Move back the checkpoint to its place
                 shutil.move(tmp_checkpoint, checkpoint_folder)
 
     def _load_best_model(self):
         logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
         best_model_path = os.path.join(self.state.best_model_checkpoint, WEIGHTS_NAME)
+        best_safe_model_path = os.path.join(self.state.best_model_checkpoint, SAFE_WEIGHTS_NAME)
         model = self.model
-        if os.path.exists(best_model_path):
+        if os.path.exists(best_model_path) or os.path.exists(best_safe_model_path):
             # TODO: the code below does not work with Habana DeepSpeed
             # if self.deepspeed:
 
             #     if self.model_wrapped is not None:
             #         # this removes the pre-hooks from the previous engine
             #         self.model_wrapped.destroy()
             #         self.model_wrapped = None
@@ -1590,15 +1726,19 @@
             #     self.model = deepspeed_engine.module
             #     self.model_wrapped = deepspeed_engine
             #     self.deepspeed = deepspeed_engine
             #     self.optimizer = optimizer
             #     self.lr_scheduler = lr_scheduler
             # else:
             # We load the model state dict on the CPU to avoid an OOM error.
-            state_dict = torch.load(best_model_path, map_location="cpu")
+            if self.args.save_safetensors and os.path.isfile(best_safe_model_path):
+                state_dict = safetensors.torch.load_file(best_safe_model_path, device="cpu")
+            else:
+                state_dict = torch.load(best_model_path, map_location="cpu")
+
             # If the model is on the GPU, it still works!
             load_result = model.load_state_dict(state_dict, strict=False)
             self._issue_warnings_after_load(load_result)
         else:
             logger.warning(
                 f"Could not locate the best model at {best_model_path}, if you are running a distributed training "
                 "on multiple nodes, you should activate `--save_on_each_node`."
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/trainer_seq2seq.py` & `optimum-habana-1.5.0/optimum/habana/transformers/trainer_seq2seq.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,123 @@
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
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+from copy import deepcopy
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from torch.utils.data import Dataset
 from transformers.deepspeed import is_deepspeed_zero3_enabled
-from transformers.trainer_utils import PredictionOutput
+from transformers.generation.configuration_utils import GenerationConfig
 
 from optimum.utils import logging
 
 from .trainer import GaudiTrainer
 
 
+if TYPE_CHECKING:
+    from transformers.data.data_collator import DataCollator
+    from transformers.modeling_utils import PreTrainedModel
+    from transformers.tokenization_utils_base import PreTrainedTokenizerBase
+    from transformers.trainer_callback import TrainerCallback
+    from transformers.trainer_utils import EvalPrediction, PredictionOutput
+
+    from .gaudi_configuration import GaudiConfig
+    from .training_args import GaudiTrainingArguments
+
+
 logger = logging.get_logger(__name__)
 
 
 class GaudiSeq2SeqTrainer(GaudiTrainer):
+    def __init__(
+        self,
+        model: Union["PreTrainedModel", torch.nn.Module] = None,
+        gaudi_config: "GaudiConfig" = None,
+        args: "GaudiTrainingArguments" = None,
+        data_collator: Optional["DataCollator"] = None,
+        train_dataset: Optional[Dataset] = None,
+        eval_dataset: Optional[Union[Dataset, Dict[str, Dataset]]] = None,
+        tokenizer: Optional["PreTrainedTokenizerBase"] = None,
+        model_init: Optional[Callable[[], "PreTrainedModel"]] = None,
+        compute_metrics: Optional[Callable[["EvalPrediction"], Dict]] = None,
+        callbacks: Optional[List["TrainerCallback"]] = None,
+        optimizers: Tuple[torch.optim.Optimizer, torch.optim.lr_scheduler.LambdaLR] = (None, None),
+        preprocess_logits_for_metrics: Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]] = None,
+    ):
+        super().__init__(
+            model=model,
+            gaudi_config=gaudi_config,
+            args=args,
+            data_collator=data_collator,
+            train_dataset=train_dataset,
+            eval_dataset=eval_dataset,
+            tokenizer=tokenizer,
+            model_init=model_init,
+            compute_metrics=compute_metrics,
+            callbacks=callbacks,
+            optimizers=optimizers,
+            preprocess_logits_for_metrics=preprocess_logits_for_metrics,
+        )
+
+        # Override self.model.generation_config if a GenerationConfig is specified in args.
+        # Priority: args.generation_config > model.generation_config > default GenerationConfig.
+        if self.args.generation_config is not None:
+            gen_config = self.load_generation_config(self.args.generation_config)
+            self.model.generation_config = gen_config
+
+    @staticmethod
+    def load_generation_config(gen_config_arg: Union[str, GenerationConfig]) -> GenerationConfig:
+        """
+        Loads a `~generation.GenerationConfig` from the `GaudiSeq2SeqTrainingArguments.generation_config` arguments.
+
+        Args:
+            gen_config_arg (`str` or [`~generation.GenerationConfig`]):
+                `GaudiSeq2SeqTrainingArguments.generation_config` argument.
+
+        Returns:
+            A `~generation.GenerationConfig`.
+        """
+
+        # GenerationConfig provided, nothing to do
+        if isinstance(gen_config_arg, GenerationConfig):
+            return deepcopy(gen_config_arg)
+
+        # str or Path
+        pretrained_model_name = Path(gen_config_arg) if isinstance(gen_config_arg, str) else gen_config_arg
+        config_file_name = None
+
+        # Figuring if it is path pointing to a file, pointing to a directory or else a model id or URL
+        # This step is required in order to determine config_file_name
+        if pretrained_model_name.is_file():
+            config_file_name = pretrained_model_name.name
+            pretrained_model_name = pretrained_model_name.parent
+        # dir path
+        elif pretrained_model_name.is_dir():
+            pass
+        # model id or URL
+        else:
+            pretrained_model_name = gen_config_arg
+
+        gen_config = GenerationConfig.from_pretrained(pretrained_model_name, config_file_name)
+        return gen_config
+
     def evaluate(
         self,
         eval_dataset: Optional[Dataset] = None,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "eval",
         **gen_kwargs,
     ) -> Dict[str, float]:
@@ -67,31 +153,23 @@
         if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
             gen_kwargs["max_length"] = self.args.generation_max_length
         gen_kwargs["num_beams"] = (
             gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.args.generation_num_beams
         )
         self._gen_kwargs = gen_kwargs
 
-        if self.args.use_hpu_graphs:
-            # Disable HPU graphs as generation needs to be fixed
-            self.args.use_hpu_graphs = False
-            logger.warning(
-                "HPU graphs have not been validated for generation yet. Disabling it, generation will be"
-                " performed in lazy mode."
-            )
-
         return super().evaluate(eval_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
 
     def predict(
         self,
         test_dataset: Dataset,
         ignore_keys: Optional[List[str]] = None,
         metric_key_prefix: str = "test",
         **gen_kwargs,
-    ) -> PredictionOutput:
+    ) -> "PredictionOutput":
         """
         Run prediction and returns predictions and potential metrics.
         Depending on the dataset and your use case, your test dataset may contain labels. In that case, this method
         will also return metrics, like in `evaluate()`.
         Args:
             test_dataset (`Dataset`):
                 Dataset to run the predictions on. If it is a [`~datasets.Dataset`], columns not accepted by the
@@ -168,14 +246,16 @@
                 model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
             )
 
         has_labels = "labels" in inputs
         inputs = self._prepare_inputs(inputs)
 
         # XXX: adapt synced_gpus for fairscale as well
+        # Priority (handled in generate):
+        # gen_kwargs > model.generation_config > default GenerationConfig()
         gen_kwargs = self._gen_kwargs.copy()
         if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
             gen_kwargs["max_length"] = self.model.config.max_length
         gen_kwargs["num_beams"] = (
             gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.model.config.num_beams
         )
         default_synced_gpus = True if is_deepspeed_zero3_enabled() else False
@@ -203,55 +283,61 @@
             raise error
 
         # Temporary hack to ensure the generation config is not initialized for each iteration of the evaluation loop
         # TODO: remove this hack when the legacy code that initializes generation_config from a model config is
         # removed in https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/generation/utils.py#L1183
         if self.model.generation_config._from_model_config:
             self.model.generation_config._from_model_config = False
+
+        # Retrieves GenerationConfig from model.generation_config
+        gen_config = self.model.generation_config
         # in case the batch is shorter than max length, the output should be padded
-        if gen_kwargs.get("max_length") is not None and generated_tokens.shape[-1] < gen_kwargs["max_length"]:
-            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_length"])
-        elif gen_kwargs.get("max_new_tokens") is not None and generated_tokens.shape[-1] < (
-            gen_kwargs["max_new_tokens"] + 1
-        ):
-            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_kwargs["max_new_tokens"] + 1)
+        if generated_tokens.shape[-1] < gen_config.max_length:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_length)
+        elif gen_config.max_new_tokens is not None and generated_tokens.shape[-1] < gen_config.max_new_tokens + 1:
+            generated_tokens = self._pad_tensors_to_max_len(generated_tokens, gen_config.max_new_tokens + 1)
 
         # Different processes may have different generation work in eager mode, hence this sync
         if not self.args.use_lazy_mode and self.args.local_rank != -1:
             torch.distributed.barrier()
 
         with torch.no_grad():
-            if has_labels:
-                with self.compute_loss_context_manager():
-                    outputs = model(**inputs)
-                if self.label_smoother is not None:
-                    loss = self.label_smoother(outputs, inputs["labels"]).mean().detach()
+            try:
+                if has_labels:
+                    with self.compute_loss_context_manager():
+                        outputs = model(**inputs)
+                    if self.label_smoother is not None:
+                        loss = self.label_smoother(outputs, inputs["labels"]).mean().detach()
+                    else:
+                        loss = (outputs["loss"] if isinstance(outputs, dict) else outputs[0]).mean().detach()
                 else:
-                    loss = (outputs["loss"] if isinstance(outputs, dict) else outputs[0]).mean().detach()
-            else:
-                loss = None
+                    loss = None
+            except RuntimeError as error:
+                if "cpu fallback is not supported during hpu graph capturing" in str(error):
+                    error.args = (
+                        f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs=False`.",
+                    )
+                raise error
 
         if self.args.use_lazy_mode and not (self.args.use_hpu_graphs and not self.is_in_train):
             self.htcore.mark_step()
 
         if self.args.prediction_loss_only:
-            return (loss, None, None)
+            return loss, None, None
 
         if has_labels:
             labels = inputs["labels"]
-            if gen_kwargs.get("max_length") is not None and labels.shape[-1] < gen_kwargs["max_length"]:
-                labels = self._pad_tensors_to_max_len(labels, gen_kwargs["max_length"])
-            elif gen_kwargs.get("max_new_tokens") is not None and labels.shape[-1] < (
-                gen_kwargs["max_new_tokens"] + 1
-            ):
-                labels = self._pad_tensors_to_max_len(labels, (gen_kwargs["max_new_tokens"] + 1))
+            if labels.shape[-1] < gen_config.max_length:
+                labels = self._pad_tensors_to_max_len(labels, gen_config.max_length)
+            elif gen_config.max_new_tokens is not None and labels.shape[-1] < gen_config.max_new_tokens + 1:
+                labels = self._pad_tensors_to_max_len(labels, gen_config.max_new_tokens + 1)
         else:
             labels = None
 
-        return (loss, generated_tokens, labels)
+        return loss, generated_tokens, labels
 
     def _pad_tensors_to_max_len(self, tensor, max_length):
         if self.tokenizer is not None and hasattr(self.tokenizer, "pad_token_id"):
             # If PAD token is not defined at least EOS token has to be defined
             pad_token_id = (
                 self.tokenizer.pad_token_id if self.tokenizer.pad_token_id is not None else self.tokenizer.eos_token_id
             )
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/trainer_utils.py` & `optimum-habana-1.5.0/optimum/habana/transformers/trainer_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         logits_dtype = str(logits.dtype).split(".")[-1]
         # If mixed-precision training was performed, dtype must be 'float32' to be understood by Numpy
         if logits_dtype == "bfloat16":
             logits_dtype = "float32"
         return logits_dtype
     elif isinstance(logits, tuple):
         return [get_dtype(logits_tensor) for logits_tensor in logits]
+    elif isinstance(logits, dict):
+        return {k: get_dtype(v) for k, v in logits.items()}
     else:
         raise TypeError(f"logits should be of type torch.Tensor or tuple, got {type(logits)} which is not supported")
 
 
 def convert_into_dtypes(
     preds: Union[np.ndarray, Tuple[np.ndarray]], dtypes: Union[str, List[str]]
 ) -> Union[np.ndarray, Tuple[np.ndarray]]:
```

### Comparing `optimum-habana-1.4.2/optimum/habana/transformers/training_args.py` & `optimum-habana-1.5.0/optimum/habana/transformers/training_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
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
 
 import os
 import warnings
 from dataclasses import asdict, dataclass, field
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional, Union
@@ -25,15 +26,21 @@
 from transformers.trainer_utils import EvaluationStrategy, HubStrategy, IntervalStrategy, SchedulerType
 from transformers.training_args import (
     OptimizerNames,
     TrainingArguments,
     default_logdir,
     get_int_from_env,
 )
-from transformers.utils import ccl_version, get_full_repo_name, is_accelerate_available, is_psutil_available
+from transformers.utils import (
+    ccl_version,
+    get_full_repo_name,
+    is_accelerate_available,
+    is_psutil_available,
+    is_safetensors_available,
+)
 
 from optimum.utils import logging
 
 
 if is_torch_available():
     import torch
 
@@ -88,15 +95,15 @@
 
     throughput_warmup_steps: int = field(
         default=0,
         metadata={
             "help": (
                 "Number of steps to ignore for throughput calculation. For example, with throughput_warmup_steps=N,"
                 " the first N steps will not be considered in the calculation of the throughput. This is especially"
-                " useful in lazy mode."
+                " useful in lazy mode where the first two or three training iterations typically take longer."
             )
         },
     )
 
     # Overriding the default value of optim because 'adamw_hf' is deprecated
     optim: Union[OptimizerNames, str] = field(
         default="adamw_torch",
@@ -131,14 +138,24 @@
             "help": (
                 "When using distributed training, the value of the flag `find_unused_parameters` passed to "
                 "`DistributedDataParallel`."
             )
         },
     )
 
+    pipelining_fwd_bwd: Optional[bool] = field(
+        default=False,
+        metadata={
+            "help": (
+                "Whether to add an additional mark_step between forward and backward for pipelining "
+                "host BWD building and HPU FWD computing."
+            )
+        },
+    )
+
     def __post_init__(self):
         if (self.use_lazy_mode or self.use_hpu_graphs or self.gaudi_config_name) and not self.use_habana:
             raise ValueError(
                 "--use_lazy_mode, --use_hpu_graphs and --gaudi_config_name cannot be used without --use_habana"
             )
 
         if self.use_hpu_graphs and not self.use_lazy_mode:
@@ -232,14 +249,25 @@
                 )
             if self.evaluation_strategy == IntervalStrategy.STEPS and self.save_steps % self.eval_steps != 0:
                 raise ValueError(
                     "--load_best_model_at_end requires the saving steps to be a round multiple of the evaluation "
                     f"steps, but found {self.save_steps}, which is not a round multiple of {self.eval_steps}."
                 )
 
+        safetensors_available = is_safetensors_available()
+        if self.save_safetensors and not safetensors_available:
+            raise ValueError(f"--save_safetensors={self.save_safetensors} requires safetensors to be installed!")
+        if not self.save_safetensors and safetensors_available:
+            logger.info(
+                f"Found safetensors installation, but --save_safetensors={self.save_safetensors}. "
+                f"Safetensors should be a preferred weights saving format due to security and performance reasons. "
+                f"If your model cannot be saved by safetensors please feel free to open an issue at "
+                f"https://github.com/huggingface/safetensors!"
+            )
+
         if self.load_best_model_at_end and self.metric_for_best_model is None:
             self.metric_for_best_model = "loss"
         if self.greater_is_better is None and self.metric_for_best_model is not None:
             self.greater_is_better = self.metric_for_best_model not in ["loss", "eval_loss"]
         if self.run_name is None:
             self.run_name = self.output_dir
 
@@ -461,26 +489,30 @@
             if self.deepspeed:
                 # deepspeed inits torch.distributed internally
                 from transformers.deepspeed import is_deepspeed_available
 
                 if not is_deepspeed_available():
                     raise ImportError(
                         "--deepspeed requires deepspeed: `pip install"
-                        " git+https://github.com/HabanaAI/DeepSpeed.git@1.8.0`."
+                        " git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0`."
                     )
                 import deepspeed
 
+                if world_size > 1:
+                    os.environ["HLS_MODULE_ID"] = str(self.local_rank)
+                    os.environ["ID"] = str(rank)
+
                 deepspeed.init_distributed(dist_backend="hccl", timeout=timedelta(seconds=self.ddp_timeout))
                 logger.info("DeepSpeed is enabled.")
             else:
                 if self.local_rank != -1:
                     if not torch.distributed.is_initialized():
                         torch.distributed.init_process_group(backend="hccl", rank=rank, world_size=world_size)
                         logger.info("Enabled distributed run.")
                 else:
-                    logger.info("Single node run.")
+                    logger.info("Single-device run.")
         else:
             raise ValueError(
                 "No device has been set. Use either --use_habana to run on HPU or --no_cuda to run on CPU."
             )
 
         return device
```

### Comparing `optimum-habana-1.4.2/optimum/habana/version.py` & `optimum-habana-1.5.0/optimum/habana/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-#  Copyright 2022 The HuggingFace Team. All rights reserved.
+# coding=utf-8
+# Copyright 2022 The HuggingFace Team. All rights reserved.
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
 
-__version__ = "1.4.2"
+__version__ = "1.5.0"
```

### Comparing `optimum-habana-1.4.2/optimum_habana.egg-info/PKG-INFO` & `optimum-habana-1.5.0/optimum_habana.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.4.2
+Version: 1.5.0
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,43 +59,36 @@
 
 ```bash
 pip install optimum[habana]
 ```
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.8.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
 
-> Alternatively, you can install the package without pip as follows:
-> ```bash
-> git clone https://github.com/huggingface/optimum-habana.git
-> cd optimum-habana
-> python setup.py install
-> ```
-
 Last but not least, don't forget to install the requirements for every example:
 
 ```bash
 cd <example-folder>
 pip install -r requirements.txt
 ```
 
 
 ## How to use it?
 
 ### Quick Start
 
-🤗 Optimum Habana was designed with one goal in mind: **to make training and evaluation straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
+🤗 Optimum Habana was designed with one goal in mind: **to make training and inference straightforward for any 🤗 Transformers and 🤗 Diffusers user while leveraging the complete power of Gaudi processors**.
 
 #### Transformers Interface
 
 There are two main classes one needs to know:
 - [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
@@ -153,15 +146,14 @@
 )
 ```
 
 where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories). You can also give the path to a custom Gaudi configuration written in a JSON file such as this one:
 ```json
 {
   "use_habana_mixed_precision": true,
-  "hmp_opt_level": "O1",
   "hmp_is_verbose": false,
   "use_fused_adam": true,
   "use_fused_clip_norm": true,
   "hmp_bf16_ops": [
     "add",
     "addmm",
     "bmm",
@@ -201,15 +193,15 @@
 You can generate images from prompts using Stable Diffusion on Gaudi using the [`GaudiStableDiffusionPipeline`](https://huggingface.co/docs/optimum/habana/package_reference/stable_diffusion_pipeline) class and the [`GaudiDDIMScheduler`] which have been both optimized for HPUs. Here is how to use them and the differences with the 🤗 Diffusers library:
 
 ```diff
 - from diffusers import DDIMScheduler, StableDiffusionPipeline
 + from optimum.habana.diffusers import GaudiDDIMScheduler, GaudiStableDiffusionPipeline
 
 
-model_name = "CompVis/stable-diffusion-v1-4"
+model_name = "runwayml/stable-diffusion-v1-5"
 
 - scheduler = DDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 + scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
 
 - pipeline = StableDiffusionPipeline.from_pretrained(
 + pipeline = GaudiStableDiffusionPipeline.from_pretrained(
     model_name,
@@ -246,22 +238,24 @@
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | Stable Diffusion | :heavy_check_mark: | ✗ | ✗ | <li>[text-to-image generation](https://github.com/huggingface/optimum-habana/tree/main/examples/stable-diffusion)</li> |
+| CLIP | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
+| BLOOM(Z) | ✗ | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 
 </div>
 
 Other models and tasks supported by the 🤗 Transformers library may also work. You can refer to this [section](https://github.com/huggingface/optimum-habana#how-to-use-it) for using them with 🤗 Optimum Habana. Besides, [this page](https://github.com/huggingface/optimum-habana/tree/main/examples) explains how to modify any [example](https://github.com/huggingface/transformers/tree/main/examples/pytorch) from the 🤗 Transformers library to make it work with 🤗 Optimum Habana.
 
 If you find any issue while using those, please open an issue or a pull request.
 
 
 ## Gaudi Setup
 
 Please refer to Habana Gaudi's official [installation guide](https://docs.habana.ai/en/latest/Installation_Guide/index.html).
 
 > Tests should be run in a Docker container based on Habana Docker images.
 >
-> The current version has been validated for SynapseAI 1.8.
+> The current version has been validated for SynapseAI 1.9.
```

### Comparing `optimum-habana-1.4.2/pyproject.toml` & `optimum-habana-1.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 [tool.black]
 line-length = 119
 target-version = ['py37']
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
-ignore = ["E501", "E741", "W605"]
-select = ["E", "F", "I", "W"]
+ignore = ["C901", "E501", "E741", "W605"]
+select = ["C", "E", "F", "I", "W"]
 line-length = 119
 
 # Ignore import violations in all `__init__.py` files.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 
 [tool.ruff.isort]
```

### Comparing `optimum-habana-1.4.2/setup.py` & `optimum-habana-1.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# coding=utf-8
+# Copyright 2022 The HuggingFace Inc. team.
+# Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
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
 import re
 
 from setuptools import find_namespace_packages, setup
 
 
 # Ensure we match the version set in optimum/habana/version.py
 try:
@@ -24,14 +40,15 @@
     "pytest",
     "psutil",
     "parameterized",
     "GitPython",
     "optuna",
     "sentencepiece",
     "datasets",
+    "safetensors",
 ]
 
 QUALITY_REQUIRES = [
     "black",
     "ruff",
     "hf_doc_builder",
 ]
```

