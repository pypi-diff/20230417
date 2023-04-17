# Comparing `tmp/schnitsum-0.4.5.tar.gz` & `tmp/schnitsum-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schnitsum-0.4.5.tar", max compression
+gzip compressed data, was "schnitsum-0.4.6.tar", max compression
```

## Comparing `schnitsum-0.4.5.tar` & `schnitsum-0.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-09-29 19:29:08.745912 schnitsum-0.4.5/LICENSE
--rw-r--r--   0        0        0     2117 2022-10-02 07:50:48.157911 schnitsum-0.4.5/README.md
--rw-r--r--   0        0        0      548 2023-04-13 10:43:07.653564 schnitsum-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       37 2022-09-30 14:59:31.703238 schnitsum-0.4.5/schnitsum/__init__.py
--rw-r--r--   0        0        0      693 2022-10-01 09:02:23.109770 schnitsum-0.4.5/schnitsum/bin/summarize.py
--rw-r--r--   0        0        0     2112 2023-04-13 09:12:00.250419 schnitsum-0.4.5/schnitsum/main.py
--rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 schnitsum-0.4.5/setup.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 schnitsum-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-29 19:29:08.745912 schnitsum-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2388 2023-04-17 12:20:42.761272 schnitsum-0.4.6/README.md
+-rw-r--r--   0        0        0      548 2023-04-17 13:08:12.684287 schnitsum-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-09-30 14:59:31.703238 schnitsum-0.4.6/schnitsum/__init__.py
+-rw-r--r--   0        0        0      693 2022-10-01 09:02:23.109770 schnitsum-0.4.6/schnitsum/bin/summarize.py
+-rw-r--r--   0        0        0     2596 2023-04-17 13:01:21.888138 schnitsum-0.4.6/schnitsum/main.py
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 schnitsum-0.4.6/setup.py
+-rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 schnitsum-0.4.6/PKG-INFO
```

### Comparing `schnitsum-0.4.5/LICENSE` & `schnitsum-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schnitsum-0.4.5/README.md` & `schnitsum-0.4.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)).
   - Model name: `sobamchan/bart-large-scitldr`
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 65% parameters less.
   - Model name: `sobamchan/bart-large-scitldr-distilled-3-3`
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 37% parameters less.
   - Model name: `sobamchan/bart-large-scitldr-distilled-12-3`
+- [mBART (large, en-to-de)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers, English papers and German summaries (ref. [X-SciTLDR](https://dl.acm.org/doi/abs/10.1145/3529372.3530938)).
+  - Model name: `sobamchan/mbart-large-xscitldr-de`
 
 we are planning to expand coverage soon to other sizes, domains, languages, models soon.
 
 
 # Installation
 
 ```bash
```

### Comparing `schnitsum-0.4.5/pyproject.toml` & `schnitsum-0.4.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schnitsum"
-version = "0.4.5"
+version = "0.4.6"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 transformers = "4.22.2"
```

### Comparing `schnitsum-0.4.5/schnitsum/bin/summarize.py` & `schnitsum-0.4.6/schnitsum/bin/summarize.py`

 * *Files identical despite different names*

### Comparing `schnitsum-0.4.5/schnitsum/main.py` & `schnitsum-0.4.6/schnitsum/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,44 @@
 from tqdm import tqdm
 from transformers import AutoModelForSeq2SeqLM, AutoTokenizer
 
 MODEL_NAMES = [
     "sobamchan/bart-large-scitldr",
     "sobamchan/bart-large-scitldr-distilled-3-3",
     "sobamchan/bart-large-scitldr-distilled-12-3",
+    "sobamchan/mbart-large-xscitldr-de",
 ]
+LANG2CODE = {
+    "en": "en_XX",
+    "de": "de_DE",
+    "ja": "ja_XX",
+    "it": "it_IT",
+    "zh": "zh_CN",
+}
 
 
 class SchnitSum:
-    def __init__(self, model_name: str = None, use_gpu: bool = False):
+    def __init__(
+        self, model_name: str = None, tgt_lang: str = "en", use_gpu: bool = False
+    ):
 
         """Easy to use summarization package.
         model_name (str):
         use_gpu (bool): Whether use GPU for inference or not.
 
         Parameters
         ----------
         model_name : str
             Model name to use.
 
         use_gpu : bool
             If use GPU or not
+
+        tgt_lang : str
+            Language for output summary (default = `en`)
         """
         if model_name not in MODEL_NAMES:
             model_names_str = "\n".join([f"- {name}" for name in MODEL_NAMES])
             raise ValueError(
                 f"{model_name} is not currently supported. Pick one from\n"
                 f"{model_names_str}"
             )
@@ -39,26 +52,32 @@
 
         if use_gpu:
             model = model.to("cuda")
 
         self.use_gpu = use_gpu
         self.model = model
         self.model_name = model_name
+        self.tgt_lang = tgt_lang
         print("loaded!")
 
     def summarize_batch(self, texts: List[str]) -> List[str]:
         inputs = self.tokenizer(
             texts, padding="max_length", truncation=True, return_tensors="pt"
         )
         summary_ids = self.model.generate(
             inputs["input_ids"].to("cuda") if self.use_gpu else inputs["input_ids"],
             max_length=250,
             num_beams=1,
             repetition_penalty=1.0,
             early_stopping=True,
+            decoder_start_token_id=self.tokenizer.lang_code_to_id[
+                LANG2CODE[self.tgt_lang]
+            ]
+            if self.tgt_lang != "en"
+            else None,
         )
         return self.tokenizer.batch_decode(summary_ids, skip_special_tokens=True)
 
     def __call__(self, texts: List[str], batch_size: int = 4) -> List[str]:
         summaries = []
         for i in tqdm(range(0, len(texts), batch_size)):
             texts_batch = texts[i : i + batch_size]
```

### Comparing `schnitsum-0.4.5/setup.py` & `schnitsum-0.4.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fire>=0.4.0,<0.5.0', 'sienna>=0.2.0', 'torch>=2.0.0', 'transformers==4.22.2']
 
 entry_points = \
 {'console_scripts': ['schnitsum = schnitsum.bin.summarize:cli']}
 
 setup_kwargs = {
     'name': 'schnitsum',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': '',
-    'long_description': '# Schnitsum: Easy to use neural network based summarization models\n\nThis package enables to generate summaries of you documents of interests.\n\nCurrently, we support following models,\n\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)).\n  - Model name: `sobamchan/bart-large-scitldr`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 65% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-3-3`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 37% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-12-3`\n\nwe are planning to expand coverage soon to other sizes, domains, languages, models soon.\n\n\n# Installation\n\n```bash\npip install schnitsum  # or poetry add schnitsum\n```\n\nThis will let you generate summaries with CPUs only, if you want to utilize your GPUs, please follow the instruction by PyTorch, [here](https://pytorch.org/get-started/locally/).\n\n\n# Usage\n\n## From Command Line\nPass document as an argument and print the summary\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --text "Text to summarize"\n```\n\nPass documents as a file and save summaries in a file.\nInput file needs to contain documents line by line. [example](https://github.com/sobamchan/schnitsum/blob/main/examples/docs.txt)\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --file docs.txt --opath sums.txt\n```\n\n## From Python\n```py3\nfrom schnitsum import SchnitSum\n\nmodel = SchnitSum("sobamchan/bart-large-scitldr-distilled-3-3")\ndocs = [\n    "Document you want to summarize."\n]\nsummaries = model(docs)\nprint(summaries)\n```\n',
+    'long_description': '# Schnitsum: Easy to use neural network based summarization models\n\nThis package enables to generate summaries of you documents of interests.\n\nCurrently, we support following models,\n\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)).\n  - Model name: `sobamchan/bart-large-scitldr`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 65% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-3-3`\n- [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 37% parameters less.\n  - Model name: `sobamchan/bart-large-scitldr-distilled-12-3`\n- [mBART (large, en-to-de)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers, English papers and German summaries (ref. [X-SciTLDR](https://dl.acm.org/doi/abs/10.1145/3529372.3530938)).\n  - Model name: `sobamchan/mbart-large-xscitldr-de`\n\nwe are planning to expand coverage soon to other sizes, domains, languages, models soon.\n\n\n# Installation\n\n```bash\npip install schnitsum  # or poetry add schnitsum\n```\n\nThis will let you generate summaries with CPUs only, if you want to utilize your GPUs, please follow the instruction by PyTorch, [here](https://pytorch.org/get-started/locally/).\n\n\n# Usage\n\n## From Command Line\nPass document as an argument and print the summary\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --text "Text to summarize"\n```\n\nPass documents as a file and save summaries in a file.\nInput file needs to contain documents line by line. [example](https://github.com/sobamchan/schnitsum/blob/main/examples/docs.txt)\n```sh\n> schnitsum --model-name sobamchan/bart-large-scitldr-distilled-3-3 --file docs.txt --opath sums.txt\n```\n\n## From Python\n```py3\nfrom schnitsum import SchnitSum\n\nmodel = SchnitSum("sobamchan/bart-large-scitldr-distilled-3-3")\ndocs = [\n    "Document you want to summarize."\n]\nsummaries = model(docs)\nprint(summaries)\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `schnitsum-0.4.5/PKG-INFO` & `schnitsum-0.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schnitsum
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,16 @@
 
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)).
   - Model name: `sobamchan/bart-large-scitldr`
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 65% parameters less.
   - Model name: `sobamchan/bart-large-scitldr-distilled-3-3`
 - [BART (large)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers (ref. [SciTLDR](https://aclanthology.org/2020.findings-emnlp.428)). Then distilled (by [`shrink and fine-tune`](http://arxiv.org/abs/2010.13002)) to have 37% parameters less.
   - Model name: `sobamchan/bart-large-scitldr-distilled-12-3`
+- [mBART (large, en-to-de)](https://aclanthology.org/2020.acl-main.703) fine-tuned on computer science papers, English papers and German summaries (ref. [X-SciTLDR](https://dl.acm.org/doi/abs/10.1145/3529372.3530938)).
+  - Model name: `sobamchan/mbart-large-xscitldr-de`
 
 we are planning to expand coverage soon to other sizes, domains, languages, models soon.
 
 
 # Installation
 
 ```bash
```

