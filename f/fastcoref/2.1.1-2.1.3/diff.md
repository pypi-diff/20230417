# Comparing `tmp/fastcoref-2.1.1.tar.gz` & `tmp/fastcoref-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastcoref-2.1.1.tar", last modified: Thu Nov 24 17:12:17 2022, max compression
+gzip compressed data, was "fastcoref-2.1.3.tar", last modified: Sun Apr 16 22:20:17 2023, max compression
```

## Comparing `fastcoref-2.1.1.tar` & `fastcoref-2.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/
--rw-r--r--   0 sotmazgin   (501) staff       (20)     1070 2022-07-02 08:46:57.000000 fastcoref-2.1.1/LICENSE
--rw-r--r--   0 sotmazgin   (501) staff       (20)     6297 2022-11-24 17:12:17.000000 fastcoref-2.1.1/PKG-INFO
--rw-r--r--   0 sotmazgin   (501) staff       (20)     6031 2022-11-10 18:01:10.000000 fastcoref-2.1.1/README.md
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref/
--rw-r--r--   0 sotmazgin   (501) staff       (20)      104 2022-10-25 10:11:47.000000 fastcoref-2.1.1/fastcoref/__init__.py
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref/coref_models/
--rw-r--r--   0 sotmazgin   (501) staff       (20)        0 2022-10-17 11:24:52.000000 fastcoref-2.1.1/fastcoref/coref_models/__init__.py
--rwxr-xr-x   0 sotmazgin   (501) staff       (20)    14767 2022-10-19 13:19:29.000000 fastcoref-2.1.1/fastcoref/coref_models/modeling_fcoref.py
--rwxr-xr-x   0 sotmazgin   (501) staff       (20)    19662 2022-10-19 13:19:29.000000 fastcoref-2.1.1/fastcoref/coref_models/modeling_lingmess.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)    11240 2022-11-24 17:05:19.000000 fastcoref-2.1.1/fastcoref/modeling.py
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref/spacy_component/
--rw-r--r--   0 sotmazgin   (501) staff       (20)       46 2022-10-19 22:11:24.000000 fastcoref-2.1.1/fastcoref/spacy_component/__init__.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)     7554 2022-11-24 17:05:19.000000 fastcoref-2.1.1/fastcoref/spacy_component/spacy_component.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)    12653 2022-10-25 10:51:07.000000 fastcoref-2.1.1/fastcoref/trainer.py
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref/utilities/
--rw-r--r--   0 sotmazgin   (501) staff       (20)        0 2022-10-17 11:24:52.000000 fastcoref-2.1.1/fastcoref/utilities/__init__.py
--rwxr-xr-x   0 sotmazgin   (501) staff       (20)     4548 2022-10-25 10:11:47.000000 fastcoref-2.1.1/fastcoref/utilities/collate.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)      984 2022-10-25 10:11:47.000000 fastcoref-2.1.1/fastcoref/utilities/consts.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)     6185 2022-10-25 11:10:48.000000 fastcoref-2.1.1/fastcoref/utilities/coref_dataset.py
--rwxr-xr-x   0 sotmazgin   (501) staff       (20)     5003 2022-10-25 10:11:47.000000 fastcoref-2.1.1/fastcoref/utilities/metrics.py
--rw-r--r--   0 sotmazgin   (501) staff       (20)     9393 2022-11-10 18:01:10.000000 fastcoref-2.1.1/fastcoref/utilities/util.py
-drwxr-xr-x   0 sotmazgin   (501) staff       (20)        0 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/
--rw-r--r--   0 sotmazgin   (501) staff       (20)     6297 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/PKG-INFO
--rw-r--r--   0 sotmazgin   (501) staff       (20)      648 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/SOURCES.txt
--rw-r--r--   0 sotmazgin   (501) staff       (20)        1 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/dependency_links.txt
--rw-r--r--   0 sotmazgin   (501) staff       (20)      118 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/requires.txt
--rw-r--r--   0 sotmazgin   (501) staff       (20)       10 2022-11-24 17:12:17.000000 fastcoref-2.1.1/fastcoref.egg-info/top_level.txt
--rw-r--r--   0 sotmazgin   (501) staff       (20)       38 2022-11-24 17:12:17.000000 fastcoref-2.1.1/setup.cfg
--rw-r--r--   0 sotmazgin   (501) staff       (20)      953 2022-11-24 17:08:37.000000 fastcoref-2.1.1/setup.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.462231 fastcoref-2.1.3/
+-rw-r--r--   0 shono    (847860209) 305066103     1070 2023-04-16 21:51:10.000000 fastcoref-2.1.3/LICENSE
+-rw-r--r--   0 shono    (847860209) 305066103     6754 2023-04-16 22:20:17.462094 fastcoref-2.1.3/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103     6467 2023-04-16 21:51:10.000000 fastcoref-2.1.3/README.md
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.458819 fastcoref-2.1.3/fastcoref/
+-rw-r--r--   0 shono    (847860209) 305066103      104 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/__init__.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.460209 fastcoref-2.1.3/fastcoref/coref_models/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/coref_models/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    14767 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/coref_models/modeling_fcoref.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    19662 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/coref_models/modeling_lingmess.py
+-rw-r--r--   0 shono    (847860209) 305066103    11670 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/modeling.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.460674 fastcoref-2.1.3/fastcoref/spacy_component/
+-rw-r--r--   0 shono    (847860209) 305066103       46 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/spacy_component/__init__.py
+-rw-r--r--   0 shono    (847860209) 305066103     7554 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/spacy_component/spacy_component.py
+-rw-r--r--   0 shono    (847860209) 305066103    12762 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/trainer.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.461835 fastcoref-2.1.3/fastcoref/utilities/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     4548 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/collate.py
+-rw-r--r--   0 shono    (847860209) 305066103      984 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/consts.py
+-rw-r--r--   0 shono    (847860209) 305066103     6185 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/coref_dataset.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     5003 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/metrics.py
+-rw-r--r--   0 shono    (847860209) 305066103     9393 2023-04-16 21:51:10.000000 fastcoref-2.1.3/fastcoref/utilities/util.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-04-16 22:20:17.459714 fastcoref-2.1.3/fastcoref.egg-info/
+-rw-r--r--   0 shono    (847860209) 305066103     6754 2023-04-16 22:20:17.000000 fastcoref-2.1.3/fastcoref.egg-info/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103      648 2023-04-16 22:20:17.000000 fastcoref-2.1.3/fastcoref.egg-info/SOURCES.txt
+-rw-r--r--   0 shono    (847860209) 305066103        1 2023-04-16 22:20:17.000000 fastcoref-2.1.3/fastcoref.egg-info/dependency_links.txt
+-rw-r--r--   0 shono    (847860209) 305066103      127 2023-04-16 22:20:17.000000 fastcoref-2.1.3/fastcoref.egg-info/requires.txt
+-rw-r--r--   0 shono    (847860209) 305066103       10 2023-04-16 22:20:17.000000 fastcoref-2.1.3/fastcoref.egg-info/top_level.txt
+-rw-r--r--   0 shono    (847860209) 305066103       38 2023-04-16 22:20:17.462276 fastcoref-2.1.3/setup.cfg
+-rw-r--r--   0 shono    (847860209) 305066103      991 2023-04-16 22:15:19.000000 fastcoref-2.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fastcoref-2.1.1/LICENSE` & `fastcoref-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/PKG-INFO` & `fastcoref-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: fastcoref
-Version: 2.1.1
+Version: 2.1.3
 Home-page: https://github.com/shon-otmazgin/fastcoref
 Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
 Author-email: shon711@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
+Provides-Extra: train
 License-File: LICENSE
 
 This repository is the official implementation of the paper ["F-COREF: Fast, Accurate and Easy to Use Coreference Resolution"](https://arxiv.org/abs/2209.04280).
 
 The `fastcoref` Python package provides an easy and fast API for coreference information with only few lines of code without any prepossessing steps.
 
 - [Installation](#Installation)
@@ -17,16 +18,18 @@
 - [Quick start](#quick-start)
 - [Spacy component](#spacy-component)
 - [Training](#distil-your-own-coref-model)
 - [Citation](#citation)
 
 ## Installation
 
-```python
+```bash
 pip install fastcoref
+# or for training:
+pip install fastcoref[train]
 ```
 
 ## Demo
 
 **NEW** try out the FastCoref web demo
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pythiccoder/FastCoref)
@@ -127,20 +130,20 @@
    config={'model_architecture': 'LingMessCoref', 'model_path': 'biu-nlp/lingmess-coref', 'device': 'cpu'}
 )
 ```
 
 By specifying `resolve_text=True` in the pipe call, you can get the resolved text for each cluster:
 
 ```python
-docs = nlp.pipe(
-   texts, 
+doc = nlp(      # for multiple texts use nlp.pipe
+   text, 
    component_cfg={"fastcoref": {'resolve_text': True}}
 )
 
-docs[0]._.resolved_text
+doc._.resolved_text
 > "Alice goes down the rabbit hole. Where Alice would discover a new reality beyond Alice's expectations."
 ```
 
 ## Distil your own coref model
 On top of the provided models, the package also provides the ability to train and distill coreference models on your own data, opening the possibility for fast and accurate coreference models for additional languages and domains.
 
 To be able to distil your own model you need:
@@ -200,7 +203,18 @@
    model_name_or_path='your-fast-coref-model-path',
    device='cuda:0'
 )
 ```
 
 
 ## Citation
+
+```
+@inproceedings{Otmazgin2022FcorefFA,
+  title={F-coref: Fast, Accurate and Easy to Use Coreference Resolution},
+  author={Shon Otmazgin and Arie Cattan and Yoav Goldberg},
+  booktitle={AACL},
+  year={2022}
+}
+```
+
+[F-coref: Fast, Accurate and Easy to Use Coreference Resolution](https://aclanthology.org/2022.aacl-demo.6) (Otmazgin et al., AACL-IJCNLP 2022)
```

### Comparing `fastcoref-2.1.1/README.md` & `fastcoref-2.1.3/fastcoref.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+Metadata-Version: 2.1
+Name: fastcoref
+Version: 2.1.3
+Home-page: https://github.com/shon-otmazgin/fastcoref
+Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
+Author-email: shon711@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: train
+License-File: LICENSE
+
 This repository is the official implementation of the paper ["F-COREF: Fast, Accurate and Easy to Use Coreference Resolution"](https://arxiv.org/abs/2209.04280).
 
 The `fastcoref` Python package provides an easy and fast API for coreference information with only few lines of code without any prepossessing steps.
 
 - [Installation](#Installation)
 - [Demo](#demo)
 - [Quick start](#quick-start)
 - [Spacy component](#spacy-component)
 - [Training](#distil-your-own-coref-model)
 - [Citation](#citation)
 
 ## Installation
 
-```python
+```bash
 pip install fastcoref
+# or for training:
+pip install fastcoref[train]
 ```
 
 ## Demo
 
 **NEW** try out the FastCoref web demo
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pythiccoder/FastCoref)
@@ -117,20 +130,20 @@
    config={'model_architecture': 'LingMessCoref', 'model_path': 'biu-nlp/lingmess-coref', 'device': 'cpu'}
 )
 ```
 
 By specifying `resolve_text=True` in the pipe call, you can get the resolved text for each cluster:
 
 ```python
-docs = nlp.pipe(
-   texts, 
+doc = nlp(      # for multiple texts use nlp.pipe
+   text, 
    component_cfg={"fastcoref": {'resolve_text': True}}
 )
 
-docs[0]._.resolved_text
+doc._.resolved_text
 > "Alice goes down the rabbit hole. Where Alice would discover a new reality beyond Alice's expectations."
 ```
 
 ## Distil your own coref model
 On top of the provided models, the package also provides the ability to train and distill coreference models on your own data, opening the possibility for fast and accurate coreference models for additional languages and domains.
 
 To be able to distil your own model you need:
@@ -189,8 +202,19 @@
 model = FCoref(
    model_name_or_path='your-fast-coref-model-path',
    device='cuda:0'
 )
 ```
 
 
-## Citation
+## Citation
+
+```
+@inproceedings{Otmazgin2022FcorefFA,
+  title={F-coref: Fast, Accurate and Easy to Use Coreference Resolution},
+  author={Shon Otmazgin and Arie Cattan and Yoav Goldberg},
+  booktitle={AACL},
+  year={2022}
+}
+```
+
+[F-coref: Fast, Accurate and Easy to Use Coreference Resolution](https://aclanthology.org/2022.aacl-demo.6) (Otmazgin et al., AACL-IJCNLP 2022)
```

### Comparing `fastcoref-2.1.1/fastcoref/coref_models/modeling_fcoref.py` & `fastcoref-2.1.3/fastcoref/coref_models/modeling_fcoref.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/coref_models/modeling_lingmess.py` & `fastcoref-2.1.3/fastcoref/coref_models/modeling_lingmess.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/modeling.py` & `fastcoref-2.1.3/fastcoref/modeling.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         return f'CorefResult(text="{text_to_print}", clusters={self.get_clusters()})'
 
     def __repr__(self):
         return self.__str__()
 
 
 class CorefModel(ABC):
-    def __init__(self, model_name_or_path, coref_class, collator_class, enable_progress_bar, device=None, nlp=None):
+    def __init__(self, model_name_or_path, coref_class, collator_class, enable_progress_bar, device=None, nlp="en_core_web_sm"):
         self.model_name_or_path = model_name_or_path
         self.device = device
         self.seed = 42
         self._set_device()
         self.enable_progress_bar = enable_progress_bar
 
         config = AutoConfig.from_pretrained(self.model_name_or_path)
@@ -88,23 +88,26 @@
             self.collator = LeftOversCollator(
                 tokenizer=self.tokenizer, device=self.device,
                 max_segment_len=config.coref_head['max_segment_len']
             )
         else:
             raise NotImplementedError(f"Class collator {type(collator_class)} is not supported! "
                                       f"only LeftOversCollator or PadCollator supported")
-        if nlp is not None:
-            self.nlp = nlp
+        if nlp is None:
+            self.nlp = None
+            logger.warning(
+                "You didn't specify a spacy model, you'll need to provide tokenized text in the `predict` function."
+            )
         else:
             try:
-                self.nlp = spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
+                self.nlp = spacy.load(nlp, exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
             except OSError:
                 # TODO: this is a workaround it is not clear how to add "en_core_web_sm" to setup.py
-                download('en_core_web_sm')
-                self.nlp = spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
+                download(nlp)
+                self.nlp = spacy.load(nlp, exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
 
         self.model, loading_info = coref_class.from_pretrained(
             self.model_name_or_path, config=config,
             output_loading_info=True
         )
         self.model.to(self.device)
 
@@ -235,14 +238,20 @@
 
         if not _is_valid_text_input(texts, is_split_into_words):
             raise ValueError(
                 "text input must be of type `str` (single example), `List[str]` (batch or single pretokenized example) "
                 "or `List[List[str]]` (batch of pretokenized examples)."
             )
 
+        if not is_split_into_words and not self.nlp:
+            raise ValueError(
+                "Model initialized with no nlp component for tokenizing the text, please pass pretokenized text,"
+                "or initialize the model with an nlp component."
+            )
+
         if is_split_into_words:
             is_batched = isinstance(texts, (list, tuple)) and texts and isinstance(texts[0], (list, tuple))
         else:
             is_batched = isinstance(texts, (list, tuple))
 
         if not is_batched:
             texts = [texts]
@@ -260,14 +269,14 @@
                 f.write('\n'.join(map(json.dumps, data)))
         if not is_batched:
             return preds[0]
         return preds
 
 
 class FCoref(CorefModel):
-    def __init__(self, model_name_or_path='biu-nlp/f-coref', device=None, nlp=None, enable_progress_bar=True):
+    def __init__(self, model_name_or_path='biu-nlp/f-coref', device=None, nlp="en_core_web_sm", enable_progress_bar=True):
         super().__init__(model_name_or_path, FCorefModel, LeftOversCollator, enable_progress_bar, device, nlp)
 
 
 class LingMessCoref(CorefModel):
-    def __init__(self, model_name_or_path='biu-nlp/lingmess-coref', device=None, nlp=None, enable_progress_bar=True):
+    def __init__(self, model_name_or_path='biu-nlp/lingmess-coref', device=None, nlp="en_core_web_sm", enable_progress_bar=True):
         super().__init__(model_name_or_path, LingMessModel, PadCollator, enable_progress_bar, device, nlp)
```

### Comparing `fastcoref-2.1.1/fastcoref/spacy_component/spacy_component.py` & `fastcoref-2.1.3/fastcoref/spacy_component/spacy_component.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/trainer.py` & `fastcoref-2.1.3/fastcoref/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import logging
 import numpy as np
 import torch
 import spacy
-import wandb
 from dataclasses import dataclass
 
 from torch.optim.adamw import AdamW
 from tqdm.auto import tqdm
 
 import transformers
 from transformers import AutoConfig, AutoTokenizer, get_linear_schedule_with_warmup
@@ -82,14 +81,18 @@
         raise NotImplementedError(f'Not supporting {model.base_model_prefix}, choose one of {SUPPORTED_MODELS}')
 
     return model, tokenizer
 
 
 class CorefTrainer:
     def __init__(self, args: TrainingArgs, train_file, dev_file=None, test_file=None):
+        import wandb
+        self.wandb_logger = wandb.log
+        self.wandb_runner = wandb.run
+
         transformers.logging.set_verbosity_error()
         self.args = args
         wandb.init(project=self.args.output_dir, config=self.args)
 
         self._set_device()
 
         self.nlp = spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
@@ -211,26 +214,26 @@
                 scaler.update()  # Updates the scale for next iteration
                 global_step += 1
 
                 # Log metrics
                 if global_step % self.args.logging_steps == 0:
                     loss = (tr_loss - logging_loss) / self.args.logging_steps
                     logger.info(f"loss step {global_step}: {loss}")
-                    wandb.log({'loss': loss}, step=global_step)
+                    self.wandb_logger({'loss': loss}, step=global_step)
                     logging_loss = tr_loss
 
                 # Evaluation
                 if self.dev_sampler is not None and global_step % self.args.eval_steps == 0:
                     results = self.evaluate(prefix=f'step_{global_step}', test=False)
-                    wandb.log(results, step=global_step)
+                    self.wandb_logger(results, step=global_step)
 
                     f1 = results["f1"]
                     if f1 > best_f1:
                         best_f1, best_global_step = f1, global_step
-                        wandb.run.summary["best_f1"] = best_f1
+                        self.wandb_runner.summary["best_f1"] = best_f1
 
                         # Save model
                         output_dir = os.path.join(self.args.output_dir, f'model')
                         save_all(tokenizer=self.tokenizer, model=self.model, output_dir=output_dir)
                     logger.info(f"best f1 is {best_f1} on global step {best_global_step}")
 
     def evaluate(self, test=False, prefix=''):
```

### Comparing `fastcoref-2.1.1/fastcoref/utilities/collate.py` & `fastcoref-2.1.3/fastcoref/utilities/collate.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/utilities/consts.py` & `fastcoref-2.1.3/fastcoref/utilities/consts.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/utilities/coref_dataset.py` & `fastcoref-2.1.3/fastcoref/utilities/coref_dataset.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/utilities/metrics.py` & `fastcoref-2.1.3/fastcoref/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref/utilities/util.py` & `fastcoref-2.1.3/fastcoref/utilities/util.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/fastcoref.egg-info/PKG-INFO` & `fastcoref-2.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-Metadata-Version: 2.1
-Name: fastcoref
-Version: 2.1.1
-Home-page: https://github.com/shon-otmazgin/fastcoref
-Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
-Author-email: shon711@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 This repository is the official implementation of the paper ["F-COREF: Fast, Accurate and Easy to Use Coreference Resolution"](https://arxiv.org/abs/2209.04280).
 
 The `fastcoref` Python package provides an easy and fast API for coreference information with only few lines of code without any prepossessing steps.
 
 - [Installation](#Installation)
 - [Demo](#demo)
 - [Quick start](#quick-start)
 - [Spacy component](#spacy-component)
 - [Training](#distil-your-own-coref-model)
 - [Citation](#citation)
 
 ## Installation
 
-```python
+```bash
 pip install fastcoref
+# or for training:
+pip install fastcoref[train]
 ```
 
 ## Demo
 
 **NEW** try out the FastCoref web demo
 
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/pythiccoder/FastCoref)
@@ -127,20 +119,20 @@
    config={'model_architecture': 'LingMessCoref', 'model_path': 'biu-nlp/lingmess-coref', 'device': 'cpu'}
 )
 ```
 
 By specifying `resolve_text=True` in the pipe call, you can get the resolved text for each cluster:
 
 ```python
-docs = nlp.pipe(
-   texts, 
+doc = nlp(      # for multiple texts use nlp.pipe
+   text, 
    component_cfg={"fastcoref": {'resolve_text': True}}
 )
 
-docs[0]._.resolved_text
+doc._.resolved_text
 > "Alice goes down the rabbit hole. Where Alice would discover a new reality beyond Alice's expectations."
 ```
 
 ## Distil your own coref model
 On top of the provided models, the package also provides the ability to train and distill coreference models on your own data, opening the possibility for fast and accurate coreference models for additional languages and domains.
 
 To be able to distil your own model you need:
@@ -200,7 +192,18 @@
    model_name_or_path='your-fast-coref-model-path',
    device='cuda:0'
 )
 ```
 
 
 ## Citation
+
+```
+@inproceedings{Otmazgin2022FcorefFA,
+  title={F-coref: Fast, Accurate and Easy to Use Coreference Resolution},
+  author={Shon Otmazgin and Arie Cattan and Yoav Goldberg},
+  booktitle={AACL},
+  year={2022}
+}
+```
+
+[F-coref: Fast, Accurate and Easy to Use Coreference Resolution](https://aclanthology.org/2022.aacl-demo.6) (Otmazgin et al., AACL-IJCNLP 2022)
```

### Comparing `fastcoref-2.1.1/fastcoref.egg-info/SOURCES.txt` & `fastcoref-2.1.3/fastcoref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.1/setup.py` & `fastcoref-2.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='fastcoref',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.1.1',
+    version='2.1.3',
     license='MIT',
     author="Shon Otmazgin, Arie Cattan, Yoav Goldberg",
     author_email='shon711@gmail.com',
     packages=['fastcoref', 'fastcoref.coref_models', 'fastcoref.utilities', 'fastcoref.spacy_component'],
     url='https://github.com/shon-otmazgin/fastcoref',
     install_requires=[
         'tqdm>=4.64.0',
         'numpy>=1.21.6',
         'scipy>=1.7.3',
         'spacy>=3.0.6',
         'torch>=1.10.0',
         'transformers>=4.11.3',
         'datasets>=2.5.2',
-        'wandb>=0.13.4'
-      ],
+    ],
+    extras_require={
+        'train': ['wandb>=0.13.4'],
+    },
 
 )
```

