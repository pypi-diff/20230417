# Comparing `tmp/qasem-0.1.9.tar.gz` & `tmp/qasem-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qasem-0.1.9.tar", last modified: Thu Dec 15 13:07:31 2022, max compression
+gzip compressed data, was "dist/qasem-0.2.0.tar", last modified: Mon Apr 17 06:11:34 2023, max compression
```

## Comparing `qasem-0.1.9.tar` & `qasem-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 kleinay   (3219) nlp       (1301)        0 2022-12-15 13:07:31.000000 qasem-0.1.9/
--rw-r--r--   0 kleinay   (3219) nlp       (1301)       88 2022-11-21 07:43:16.000000 qasem-0.1.9/MANIFEST.in
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     7636 2022-12-15 13:07:31.000000 qasem-0.1.9/PKG-INFO
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     7147 2022-11-30 12:57:20.000000 qasem-0.1.9/README.md
-drwxr-xr-x   0 kleinay   (3219) nlp       (1301)        0 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem/
--rw-r--r--   0 kleinay   (3219) nlp       (1301)      200 2022-11-21 07:43:16.000000 qasem-0.1.9/qasem/__init__.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     7432 2022-11-21 07:43:16.000000 qasem-0.1.9/qasem/candidates_finder.py
-drwxr-xr-x   0 kleinay   (3219) nlp       (1301)        0 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem/data/
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     5934 2022-11-21 07:43:16.000000 qasem-0.1.9/qasem/data/connectives_small_set.txt
--rw-r--r--   0 kleinay   (3219) nlp       (1301)    17436 2022-12-15 13:04:27.000000 qasem-0.1.9/qasem/end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     5039 2022-11-30 13:40:12.000000 qasem-0.1.9/qasem/openie_converter.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     4616 2022-11-21 13:09:51.000000 qasem-0.1.9/qasem/qa_discourse_pipeline.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     2181 2022-12-01 08:58:36.000000 qasem-0.1.9/qasem/test_end_to_end_pipeline.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)      276 2022-11-21 09:56:37.000000 qasem-0.1.9/qasem/utils.py
--rw-r--r--   0 kleinay   (3219) nlp       (1301)        5 2022-12-15 13:06:35.000000 qasem-0.1.9/qasem/version.txt
-drwxr-xr-x   0 kleinay   (3219) nlp       (1301)        0 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     7636 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/PKG-INFO
--rw-r--r--   0 kleinay   (3219) nlp       (1301)      419 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/SOURCES.txt
--rw-r--r--   0 kleinay   (3219) nlp       (1301)        1 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/dependency_links.txt
--rw-r--r--   0 kleinay   (3219) nlp       (1301)       67 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/requires.txt
--rw-r--r--   0 kleinay   (3219) nlp       (1301)        6 2022-12-15 13:07:31.000000 qasem-0.1.9/qasem.egg-info/top_level.txt
--rw-r--r--   0 kleinay   (3219) nlp       (1301)       79 2022-12-15 13:07:31.000000 qasem-0.1.9/setup.cfg
--rw-r--r--   0 kleinay   (3219) nlp       (1301)     1206 2022-11-23 11:22:38.000000 qasem-0.1.9/setup.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       88 2022-07-17 10:30:16.000000 qasem-0.2.0/MANIFEST.in
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-04-17 06:11:34.000000 qasem-0.2.0/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     8708 2023-04-17 06:10:03.000000 qasem-0.2.0/README.md
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      200 2022-07-17 11:03:06.000000 qasem-0.2.0/qasem/__init__.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     7443 2023-03-16 08:20:42.000000 qasem-0.2.0/qasem/candidates_finder.py
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem/data/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5934 2023-01-31 18:04:55.000000 qasem-0.2.0/qasem/data/connectives_small_set.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)    17746 2023-03-16 08:12:00.000000 qasem-0.2.0/qasem/end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5039 2023-01-04 13:57:20.000000 qasem-0.2.0/qasem/openie_converter.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     5041 2023-03-16 08:22:36.000000 qasem-0.2.0/qasem/qa_adj_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     4616 2023-01-04 13:57:20.000000 qasem-0.2.0/qasem/qa_discourse_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     3232 2023-01-31 14:13:37.000000 qasem-0.2.0/qasem/question_contextualizer.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      845 2023-03-16 08:20:10.000000 qasem-0.2.0/qasem/spacy_loader.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     2364 2023-02-05 09:41:21.000000 qasem-0.2.0/qasem/test_end_to_end_pipeline.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      271 2023-02-05 09:41:21.000000 qasem-0.2.0/qasem/utils.py
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        5 2023-04-17 06:09:51.000000 qasem-0.2.0/qasem/version.txt
+drwxr-xr-x   0 kleinay   (1000) kleinay   (1000)        0 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     9234 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/PKG-INFO
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)      499 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/SOURCES.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        1 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/dependency_links.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       53 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/requires.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)        6 2023-04-17 06:11:34.000000 qasem-0.2.0/qasem.egg-info/top_level.txt
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)       79 2023-04-17 06:11:34.000000 qasem-0.2.0/setup.cfg
+-rw-r--r--   0 kleinay   (1000) kleinay   (1000)     1235 2023-03-16 08:23:45.000000 qasem-0.2.0/setup.py
```

### Comparing `qasem-0.1.9/PKG-INFO` & `qasem-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: qasem
-Version: 0.1.9
-Summary: package for QA-based Semantics - representing textual information via question-answer pairs
-Home-page: https://github.com/kleinay/QASem
-Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
-Author-email: ayal.s.klein@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # QASem - Question-Answer based Semantics 
 
 This repository includes software for parsing natural language sentence with various layers of QA-based semantic annotations. 
 We currently support three layers of semantic annotations - QASRL, QANom, and QADiscourse. 
 See an overview of our approach at our paper on [QASem Parsing](https://arxiv.org/abs/2205.11413). 
 
 [QASRL (Question Answer driven Semantic Role Labeling)](https://aclanthology.org/D15-1076/) is a lightweight semantic framework for annotating "who did what to whom, how, when and where". 
@@ -35,15 +22,15 @@
 Check out the [live QASem demo](https://huggingface.co/spaces/kleinay/qasem-demo) on Huggingface.
 
 
 
 
 ## Installation
 
-**Pre-requisite**: Python 3.7
+**Pre-requisite**: Python 3.8 (as of version 0.2.0; before that - Python 3.7)
 
 Installation is available via pip:
 ```bash
 pip install qasem
 ```
 
 ### Installation from source
@@ -68,21 +55,28 @@
 
 ## Usage 
 
 The `QASemEndToEndPipeline` class would, by demand, parse sentences with any of the QASem semantic annotation layers --- currenlty including 'qasrl', 'qanom' and 'qadiscourse'.  
 
 ### Features
 
+**Run on GPU:**
+Use `device=d` in initialization to put models and tensors on a GPU device, where `d` is the CUDA device ID. We currently do not support parallelization on multiple GPUs. Defaults to `device=-1`, i.e. CPU.  
+
 **Annotation layers:**
 By default, the pipeline would parse all layers.
 To specify a subset of desired layers, e.g. QASRL and QADiscourse alone, use `annotation_layers=('qasrl', 'qadiscourse')` in initialization.
 
 **QA-SRL contextualization:**
 For the sake of generality, QA-SRL and QANom generate ``abstractive'' questions, that replace arguments with placeholders, e.g. "Why was *someone* interested in *something*?". However, in some use-cases you might want to have a more natural question with contextualized arguments, e.g. "Why was *the doctor* interested in *Luke 's treatment*?". Utilizing the model from [Pyatkin et. al., 2021](https://aclanthology.org/2021.emnlp-main.108/), one can additionally get contextualized questions for QA-SRL and QANom by setting `QASemEndToEndPipeline(contextualize=True)` (see example below).     
 
+**QA-SRL Discrete Roles:** In QA-SRL, semantic roles are captured in a rich but soft manner within the questions. For some applications, a reduced discrete account of semantic roles may be desired. By default (`return_qasrl_discrete_role=True` in initialization), we provide a discrete "question-role" label per question in the output, based on a heuristic mapping from the question syntactical structure. For the core arguments, "R0" corresponds to asking about the subject position (commonly equivalent to proto-agent semantic roles), "R1" to direct object (proto-patient), "R2" to a second direct object, and "R2_<preposition>" to an indirect object (e.g. "R2_on" <-> "what did someone put something *on*?"). For modifiers ("where", "when", "how", "why", "how long", "how much") the WH-word (plus, optionally, the preposition) is defining the "question-role". See Table 7 at the [QA-SRL 2015 paper](https://dada.cs.washington.edu/qasrl/docs/emnlp2015_hlz.pdf) for more details about the set of Roles and the heuristic mapping.  
+
+**QA-SRL Question slots:** Set `return_qasrl_slots=True` in initialization to get detailed information about each QA-SRL question. This includes the 7 slots comprising the question, the verb inflection, voice ("is_passive") and negation ("is_negated"). 
+
 **Nominal predicate detection:**
 `nominalization_detection_threshold` --- which can be set globally in initialization and per `__call__` --- is the threshold for the nominalization detection model.
 A higher threshold (e.g. `0.8`) means capturing less nominal predicates with higher confidence of them being, in context, verb-derived event markers. Default threshold is `0.7`. 
 
 **OpenIE converter:**
 Set `output_openie=True` (in `__call__`) in order to get a reduction of output QAs into Open Information Extraction's tuples format. This option uses the `qasem.openie_converter.OpenIEConverter` class to linearize the arguments along with the predicate by the order of occurrence in the source sentence. 
 The pipeline's output would then be in the form `{"qasem": <regular QA outputs>, "openie": <OpenIE tuple outputs>}`.
```

### Comparing `qasem-0.1.9/README.md` & `qasem-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: qasem
+Version: 0.2.0
+Summary: package for QA-based Semantics - representing textual information via question-answer pairs
+Home-page: https://github.com/kleinay/QASem
+Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
+Author-email: ayal.s.klein@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # QASem - Question-Answer based Semantics 
 
 This repository includes software for parsing natural language sentence with various layers of QA-based semantic annotations. 
 We currently support three layers of semantic annotations - QASRL, QANom, and QADiscourse. 
 See an overview of our approach at our paper on [QASem Parsing](https://arxiv.org/abs/2205.11413). 
 
 [QASRL (Question Answer driven Semantic Role Labeling)](https://aclanthology.org/D15-1076/) is a lightweight semantic framework for annotating "who did what to whom, how, when and where". 
@@ -22,15 +37,15 @@
 Check out the [live QASem demo](https://huggingface.co/spaces/kleinay/qasem-demo) on Huggingface.
 
 
 
 
 ## Installation
 
-**Pre-requisite**: Python 3.7
+**Pre-requisite**: Python 3.8 (as of version 0.2.0; before that - Python 3.7)
 
 Installation is available via pip:
 ```bash
 pip install qasem
 ```
 
 ### Installation from source
@@ -55,21 +70,28 @@
 
 ## Usage 
 
 The `QASemEndToEndPipeline` class would, by demand, parse sentences with any of the QASem semantic annotation layers --- currenlty including 'qasrl', 'qanom' and 'qadiscourse'.  
 
 ### Features
 
+**Run on GPU:**
+Use `device=d` in initialization to put models and tensors on a GPU device, where `d` is the CUDA device ID. We currently do not support parallelization on multiple GPUs. Defaults to `device=-1`, i.e. CPU.  
+
 **Annotation layers:**
 By default, the pipeline would parse all layers.
 To specify a subset of desired layers, e.g. QASRL and QADiscourse alone, use `annotation_layers=('qasrl', 'qadiscourse')` in initialization.
 
 **QA-SRL contextualization:**
 For the sake of generality, QA-SRL and QANom generate ``abstractive'' questions, that replace arguments with placeholders, e.g. "Why was *someone* interested in *something*?". However, in some use-cases you might want to have a more natural question with contextualized arguments, e.g. "Why was *the doctor* interested in *Luke 's treatment*?". Utilizing the model from [Pyatkin et. al., 2021](https://aclanthology.org/2021.emnlp-main.108/), one can additionally get contextualized questions for QA-SRL and QANom by setting `QASemEndToEndPipeline(contextualize=True)` (see example below).     
 
+**QA-SRL Discrete Roles:** In QA-SRL, semantic roles are captured in a rich but soft manner within the questions. For some applications, a reduced discrete account of semantic roles may be desired. By default (`return_qasrl_discrete_role=True` in initialization), we provide a discrete "question-role" label per question in the output, based on a heuristic mapping from the question syntactical structure. For the core arguments, "R0" corresponds to asking about the subject position (commonly equivalent to proto-agent semantic roles), "R1" to direct object (proto-patient), "R2" to a second direct object, and "R2_<preposition>" to an indirect object (e.g. "R2_on" <-> "what did someone put something *on*?"). For modifiers ("where", "when", "how", "why", "how long", "how much") the WH-word (plus, optionally, the preposition) is defining the "question-role". See Table 7 at the [QA-SRL 2015 paper](https://dada.cs.washington.edu/qasrl/docs/emnlp2015_hlz.pdf) for more details about the set of Roles and the heuristic mapping.  
+
+**QA-SRL Question slots:** Set `return_qasrl_slots=True` in initialization to get detailed information about each QA-SRL question. This includes the 7 slots comprising the question, the verb inflection, voice ("is_passive") and negation ("is_negated"). 
+
 **Nominal predicate detection:**
 `nominalization_detection_threshold` --- which can be set globally in initialization and per `__call__` --- is the threshold for the nominalization detection model.
 A higher threshold (e.g. `0.8`) means capturing less nominal predicates with higher confidence of them being, in context, verb-derived event markers. Default threshold is `0.7`. 
 
 **OpenIE converter:**
 Set `output_openie=True` (in `__call__`) in order to get a reduction of output QAs into Open Information Extraction's tuples format. This option uses the `qasem.openie_converter.OpenIEConverter` class to linearize the arguments along with the predicate by the order of occurrence in the source sentence. 
 The pipeline's output would then be in the form `{"qasem": <regular QA outputs>, "openie": <OpenIE tuple outputs>}`.
@@ -141,7 +163,9 @@
 @article{klein2022qasem,
   title={QASem Parsing: Text-to-text Modeling of QA-based Semantics},
   author={Klein, Ayal and Hirsch, Eran and Eliav, Ron and Pyatkin, Valentina and Caciularu, Avi and Dagan, Ido},
   journal={arXiv preprint arXiv:2205.11413},
   year={2022}
 }
 ```
+
+
```

### Comparing `qasem-0.1.9/qasem/candidates_finder.py` & `qasem-0.2.0/qasem/candidates_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional 
-import spacy
 import codecs
 from nltk.tokenize.treebank import TreebankWordDetokenizer
 from collections import defaultdict
 from qasem import data_dir
+from qasem.spacy_loader import get_spacy
 
 connective_file_default_path = data_dir / "connectives_small_set.txt"
 
 def get_connectives(conn_file):
     conns = defaultdict(lambda : '')
     infile = codecs.open(conn_file, 'r')
     for line in infile.readlines():
@@ -71,15 +71,15 @@
     
 class CandidateFinder():
 
     def __init__(self, conn_file: Optional[str] = None):
         conn_file = conn_file or connective_file_default_path
         self.connectives = get_connectives(conn_file)
         self.detokenizer = TreebankWordDetokenizer()
-        self.nlp = spacy.load("en_core_web_sm")
+        self.nlp = get_spacy()
         self.covered = defaultdict(lambda : '')
         
         
     def num_candidates(self, sentence):
         sentence = sentence.strip().split('\t')
         text = sentence[0]
         text = text.replace(' -LRB- ', ' ')
```

### Comparing `qasem-0.1.9/qasem/data/connectives_small_set.txt` & `qasem-0.2.0/qasem/data/connectives_small_set.txt`

 * *Files identical despite different names*

### Comparing `qasem-0.1.9/qasem/end_to_end_pipeline.py` & `qasem-0.2.0/qasem/end_to_end_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
-# sys.path.append('/Users/rubenwol/PycharmProjects/QANom/')
-
 from typing import Iterable, Optional, Tuple, List, Any, Dict
 from qanom.nominalization_detector import NominalizationDetector
 from qanom.qasrl_seq2seq_pipeline import QASRL_Pipeline
-import spacy
+
 import nltk
 from tqdm import tqdm
 from nltk.downloader import Downloader
-from roleqgen.question_translation import QuestionTranslator
+from qasem.question_contextualizer import QuestionContextualizer
 from spacy.tokenizer import Tokenizer
+from qasem.spacy_loader import get_spacy
 from qasem.qa_discourse_pipeline import QADiscourse_Pipeline
 from qasem.openie_converter import OpenIEConverter
 from qasem.utils import ListDataset
 
 qasrl_models = {"baseline": "kleinay/qasrl-seq2seq-model",
                 "joint": "kleinay/qanom-seq2seq-model-joint"}
 qanom_models = {"baseline": "kleinay/qanom-seq2seq-model-baseline",
@@ -24,74 +23,86 @@
 qadiscourse_model_name = "RonEliav/QA_discourse_v2"
 question_contextualization_model_name = "biu-nlp/contextualizer_qasrl"
 
 # Defaults
 default_annotation_layers = ['qanom', 'qasrl', 'qadiscourse']
 default_nominalization_detection_threshold = 0.7
 NO_REPEAT = True
+DEFAULT_SPACY_MODEL = 'en_core_web_trf'
 
 class QASemEndToEndPipeline():
     """
     This pipeline currently wraps QA-SRL, QANom and QADiscourse pipelines.
     """
     def __init__(self,
                  annotation_layers: Optional[List[str]] = None,
                  device: int = -1, 
                  qasrl_model: Optional[str] = None,  # for verbal predicates
                  qanom_model: Optional[str] = None,  # for nominal predicates
                  nominalization_detection_threshold: Optional[float] = None,
                  contextualize: bool = False,
+                 return_qasrl_slots: bool = False,
+                 return_qasrl_discrete_role: bool = True,
+                 spacy_model: Optional[str] = None,
+                 qasrl_pipeline_kwargs = dict(),
                  openie_converter_kwargs: Dict[str, Any] = dict(),
                  ):
         """
 
         Args:
             annotation_layers (Optional[List[str]], optional): which QA-based semantic tasks should the output include. 
                 Default includes all available layers (currently "qasrl", "qanom", "qadiscourse").
             device (int, optional): -1 for CPU (default), >=0 refers to CUDA device ordinal. Defaults to -1.
             qasrl_model (Optional[str], optional): Underlying verbal QASRL model. Can be a key for `qasrl_models` or a Huggingface Hub URL. 
                 Defaults to "joint".
-            qanom_model (Optional[str], optional): Underlying nominal QASRL (=QANom) model. Can be a key for `qanom_models` or a Huggingface Hub URL. 
+            qanom_model (Optional[str], optional): Underlying nominal QASRL (=QANom) model. Can be a key for `qanom_models` or a Huggingface Hub URL.
                 Defaults to "joint".
             contextualize (bool, optional): . 
             openie_converter_kwargs (Dict[str, Any], optional): key-word args to pass to `OpenIEConverter` constructor. Defaults to empty dict().
         """
         self.device_int = device # represent device in HF convention
-        self.device_str = f"cuda:{device}" if device>=0 else "cpu" # represent device in pytorch convention
+        self.device_str = f"cuda:{device}" if device >= 0 else "cpu"# represent device in pytorch convention
         self.annotation_layers = annotation_layers or default_annotation_layers
         qasrl_model = qasrl_model or default_qasrl_model
         qanom_model = qanom_model or default_qanom_model
         # Either a name from dict or the actual model name in HF
         qasrl_model_url = qasrl_models[qasrl_model] if qasrl_model in qasrl_models else qasrl_model
         qanom_model_url = qanom_models[qanom_model] if qanom_model in qanom_models else qanom_model
         # Init QANom predicate detection model
         if 'qanom' in self.annotation_layers:
             self.nominal_predicate_detector = NominalizationDetector(device=device)
             self.nominalization_detection_threshold = nominalization_detection_threshold or default_nominalization_detection_threshold
 
         # Set `self.qasrl_pipelines` for verbal and/or nominal QASRL
+        qasrl_pipeline_kwargs = dict(return_question_slots=return_qasrl_slots,
+                                     return_question_role=return_qasrl_discrete_role,
+                                     device=device,
+                                     **qasrl_pipeline_kwargs)
+        
         if 'qasrl' in self.annotation_layers and 'qanom' in self.annotation_layers \
                 and qasrl_model_url == qanom_model_url:
             # Default is using the same joint model for verbs and nominalizations (memory efficency)
-            joint_pipe = QASRL_Pipeline(qasrl_model_url, device=device)
+            joint_pipe = QASRL_Pipeline(qasrl_model_url, **qasrl_pipeline_kwargs)
             self.qasrl_pipelines = {"verbal": joint_pipe, "nominal": joint_pipe}
         else:
             if 'qasrl' in self.annotation_layers:
-                self.qasrl_pipelines = {"verbal": QASRL_Pipeline(qasrl_model_url, device=device)}
+                self.qasrl_pipelines = {"verbal": QASRL_Pipeline(qasrl_model_url, **qasrl_pipeline_kwargs)}
             if 'qanom' in self.annotation_layers:
-                self.qasrl_pipelines = {"nominal": QASRL_Pipeline(qasrl_model_url, device=device)}
-
+                self.qasrl_pipelines = {"nominal": QASRL_Pipeline(qasrl_model_url, **qasrl_pipeline_kwargs)}
 
         if 'qadiscourse' in self.annotation_layers:
             self.qa_discourse_pipeline = QADiscourse_Pipeline(qadiscourse_model_name, device=device)
 
         self.contextualize = contextualize
+        self.return_qasrl_slots = return_qasrl_slots
+        self.return_qasrl_discrete_role = return_qasrl_discrete_role
+        self.spacy_model_name = spacy_model or DEFAULT_SPACY_MODEL
 
         if self.contextualize:
-            self.q_translator = QuestionTranslator.from_pretrained(question_contextualization_model_name)
+            self.q_translator = QuestionContextualizer.from_pretrained(question_contextualization_model_name, device_id=device)
 
         self.openie_converter = OpenIEConverter(**openie_converter_kwargs)
 
 
     def __call__(self, sentences: Iterable[str], 
                  nominalization_detection_threshold: Optional[float] = None,
                  output_openie: bool = False,
@@ -170,19 +181,19 @@
     def get_qasrl_qa(self, sentences, predicate_lists, predicate_type, **generate_kwargs):
         
         outputs_qa = [[] for k in range(len(sentences))]
         inputs_to_qa_model, input_sentence_index, inputs_verb_forms, inputs_pred_infos = self._prepare_input_sentences(
             sentences, predicate_lists)
         # Run QA-generation pipeline (invoke inside tqdm to show progress bar)
         model_output = list(tqdm(self.qasrl_pipelines[predicate_type](ListDataset(inputs_to_qa_model),
-                                        # verb_form=inputs_verb_forms,
-                                        verb_form='',
+                                        verb_form=inputs_verb_forms,
                                         predicate_type=predicate_type, 
                                         **generate_kwargs)))
 
+
         if len(inputs_to_qa_model) > 0:
             if self.contextualize:
                 # for contextualization
                 model_output = self.contextual_qa(model_output, inputs_pred_infos, sentences, input_sentence_index)
 
         # collect QAs for all predicates in sentence
         for model_pred_output, pred_info, sent_index in zip(model_output, inputs_pred_infos, input_sentence_index):
@@ -217,15 +228,15 @@
             pred_infos_flatten.extend(pred_infos)
             input_sentence_index.extend([index_sentence]*len(model_input))
             index_sentence += 1
         return sentences_input, input_sentence_index, input_verbs_form, pred_infos_flatten
 
 
     def pos_tag_tokens(self, sentences):
-        nlp = get_spacy('en_core_web_sm')
+        nlp = get_spacy(self.spacy_model_name)
         tokenizer = Tokenizer(nlp.vocab)
         nlp.tokenizer = tokenizer
         spacy_parsed_sentences = list(nlp.pipe(sentences))
         sentences_tokens_tags = []
         sentences_pos = []
         sentences_lemma = []
         for sentence_nlp in spacy_parsed_sentences:
@@ -242,14 +253,16 @@
         for i, sent_tokens_and_poses in enumerate(sentences_pos):
             target_idxs = []
             verb_forms = []
             sent_tokens, sent_pos = zip(*sent_tokens_and_poses)
             lemmas = sentences_lemma[i]
             for j, token in enumerate(sent_pos):
                 if token == 'VERB':
+                    if lemmas[j] == 'be':
+                        continue
                     target_idxs.append(j)
                     verb_forms.append(lemmas[j])
                 # elif j != 0 and token == 'ADJ':
                 #     k = 1
                 #     while sent_pos[j - k] == 'ADV' and j - k > 0: k += 1
                 #     if sent_pos[j-k] == 'AUX':
                 #         target_idxs.append(j)
@@ -279,26 +292,14 @@
         i = 0
         for pred_output, sentence_index in zip(model_output, sentences_index):
             for qa in pred_output['QAs']:
                 qa['contextual_question'] = contextualized_questions[i]
                 i += 1
         return model_output
 
-# Keep spacy model a global singleton
-spacy_models = {}
-def get_spacy(lang_model):
-    if lang_model not in spacy_models:
-        try:
-            nlp = spacy.load(lang_model)
-        except OSError:
-            print(f'Downloading SpaCy model {lang_model} for POS tagging (one-time)...\n', file=sys.stderr)
-            spacy.cli.download(lang_model)
-            nlp = spacy.load(lang_model)
-        spacy_models[lang_model] = nlp
-    return spacy_models[lang_model]
 
 def nltk_pos_tag(*inputs):
     """
     In the QASRL/QANom annotation process, they used nltk's pos_tagger ('averaged_perceptron_tagger'),
     So one should use this pos-tagger if concerned with maximum compatability with these datasets.
     Otherwise, SpaCy POS-tagger should work fine.
     """
@@ -322,15 +323,15 @@
 if __name__ == "__main__":
     open_ie_kwargs = {
         "layers_included": ["qasrl", "qanom"],
         "labeled_adjuncts": True,
     }
     pipe = QASemEndToEndPipeline(nominalization_detection_threshold=0.8, openie_converter_kwargs=open_ie_kwargs)
     import sys
-    if len(sys.argv)==1:
+    if len(sys.argv) == 1:
         sentences = [s.strip() for s in """
         He did not return to military life until the outbreak of the revolution in 1775 .
         Very little further erosion takes place after the formation of a pavement , and the ground becomes stable .
         Moreover , Russia does not want a division of Ukraine , which could lead NATO to become established within the borders of the ex-USSR , so it is more likely it is seeking to change the facts on the ground so to be able to negotiate from a position of strength .
         The king was , at first , put off by her strict religious practice , but he warmed to her through her care for his children .
         An unexpected series of experimental results for the rate of decay of heavy highly charged radioactive ions circulating in a storage ring has provoked theoretical activity in an effort to find a convincing explanation .
         The President said that he views the achievements of the Paralympics above that of the Olympics , that the Paralympics play a vital role in the lives of the athletes .
```

### Comparing `qasem-0.1.9/qasem/openie_converter.py` & `qasem-0.2.0/qasem/openie_converter.py`

 * *Files identical despite different names*

### Comparing `qasem-0.1.9/qasem/qa_discourse_pipeline.py` & `qasem-0.2.0/qasem/qa_discourse_pipeline.py`

 * *Files identical despite different names*

### Comparing `qasem-0.1.9/qasem/test_end_to_end_pipeline.py` & `qasem-0.2.0/qasem/test_end_to_end_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,20 @@
         "qadiscourse",
     ]
     open_ie_kwargs = {
         "layers_included": ["qasrl", "qanom"],
         "labeled_adjuncts": True,
     }
     pipe = QASemEndToEndPipeline(layers, 
-                                 device=-1, 
-                                 nominalization_detection_threshold=0.75, 
-                                 contextualize = True,
+                                 device=-1,
+                                 nominalization_detection_threshold=0.5,
+                                 contextualize=True,
                                  openie_converter_kwargs=open_ie_kwargs)
-    sentences = ["The doctor was very interested in Luke 's treatment as he was not feeling well .", "Tom brings the dog to the park.", "I hate cats."]
+    sentences = ["We made a very clear commitment : if there is any proposal in the next parliament for a transfer of powers to Brussels ( the EU ) we will have an in/out referendum ."]
+    # sentences = ["The doctor was very interested in Luke 's treatment as he was not feeling well .", "Tom brings the dog to the park.", "I hate cats."]
     outputs = pipe(sentences, verbose=True, output_openie=True)
     pprint(outputs)
     # print()
     # sentences = ["the ball is red ."]
     # sentences = ["the construction of the officer 's building finished right after the beginning of the destruction of the previous construction ."]
     # sentences = ["The Veterinary student was interested in Luke 's treatment of sea animals .", "John ate an apple because he was hungry ."]
     # outputs = pipe(sentences)
```

### Comparing `qasem-0.1.9/qasem.egg-info/PKG-INFO` & `qasem-0.2.0/qasem.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: qasem
-Version: 0.1.9
+Version: 0.2.0
 Summary: package for QA-based Semantics - representing textual information via question-answer pairs
 Home-page: https://github.com/kleinay/QASem
 Author: Ayal Klein, Ruben Wolhandler, Ron Eliav
 Author-email: ayal.s.klein@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # QASem - Question-Answer based Semantics 
@@ -35,15 +37,15 @@
 Check out the [live QASem demo](https://huggingface.co/spaces/kleinay/qasem-demo) on Huggingface.
 
 
 
 
 ## Installation
 
-**Pre-requisite**: Python 3.7
+**Pre-requisite**: Python 3.8 (as of version 0.2.0; before that - Python 3.7)
 
 Installation is available via pip:
 ```bash
 pip install qasem
 ```
 
 ### Installation from source
@@ -68,21 +70,28 @@
 
 ## Usage 
 
 The `QASemEndToEndPipeline` class would, by demand, parse sentences with any of the QASem semantic annotation layers --- currenlty including 'qasrl', 'qanom' and 'qadiscourse'.  
 
 ### Features
 
+**Run on GPU:**
+Use `device=d` in initialization to put models and tensors on a GPU device, where `d` is the CUDA device ID. We currently do not support parallelization on multiple GPUs. Defaults to `device=-1`, i.e. CPU.  
+
 **Annotation layers:**
 By default, the pipeline would parse all layers.
 To specify a subset of desired layers, e.g. QASRL and QADiscourse alone, use `annotation_layers=('qasrl', 'qadiscourse')` in initialization.
 
 **QA-SRL contextualization:**
 For the sake of generality, QA-SRL and QANom generate ``abstractive'' questions, that replace arguments with placeholders, e.g. "Why was *someone* interested in *something*?". However, in some use-cases you might want to have a more natural question with contextualized arguments, e.g. "Why was *the doctor* interested in *Luke 's treatment*?". Utilizing the model from [Pyatkin et. al., 2021](https://aclanthology.org/2021.emnlp-main.108/), one can additionally get contextualized questions for QA-SRL and QANom by setting `QASemEndToEndPipeline(contextualize=True)` (see example below).     
 
+**QA-SRL Discrete Roles:** In QA-SRL, semantic roles are captured in a rich but soft manner within the questions. For some applications, a reduced discrete account of semantic roles may be desired. By default (`return_qasrl_discrete_role=True` in initialization), we provide a discrete "question-role" label per question in the output, based on a heuristic mapping from the question syntactical structure. For the core arguments, "R0" corresponds to asking about the subject position (commonly equivalent to proto-agent semantic roles), "R1" to direct object (proto-patient), "R2" to a second direct object, and "R2_<preposition>" to an indirect object (e.g. "R2_on" <-> "what did someone put something *on*?"). For modifiers ("where", "when", "how", "why", "how long", "how much") the WH-word (plus, optionally, the preposition) is defining the "question-role". See Table 7 at the [QA-SRL 2015 paper](https://dada.cs.washington.edu/qasrl/docs/emnlp2015_hlz.pdf) for more details about the set of Roles and the heuristic mapping.  
+
+**QA-SRL Question slots:** Set `return_qasrl_slots=True` in initialization to get detailed information about each QA-SRL question. This includes the 7 slots comprising the question, the verb inflection, voice ("is_passive") and negation ("is_negated"). 
+
 **Nominal predicate detection:**
 `nominalization_detection_threshold` --- which can be set globally in initialization and per `__call__` --- is the threshold for the nominalization detection model.
 A higher threshold (e.g. `0.8`) means capturing less nominal predicates with higher confidence of them being, in context, verb-derived event markers. Default threshold is `0.7`. 
 
 **OpenIE converter:**
 Set `output_openie=True` (in `__call__`) in order to get a reduction of output QAs into Open Information Extraction's tuples format. This option uses the `qasem.openie_converter.OpenIEConverter` class to linearize the arguments along with the predicate by the order of occurrence in the source sentence. 
 The pipeline's output would then be in the form `{"qasem": <regular QA outputs>, "openie": <OpenIE tuple outputs>}`.
@@ -154,7 +163,9 @@
 @article{klein2022qasem,
   title={QASem Parsing: Text-to-text Modeling of QA-based Semantics},
   author={Klein, Ayal and Hirsch, Eran and Eliav, Ron and Pyatkin, Valentina and Caciularu, Avi and Dagan, Ido},
   journal={arXiv preprint arXiv:2205.11413},
   year={2022}
 }
 ```
+
+
```

### Comparing `qasem-0.1.9/setup.py` & `qasem-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     author_email="ayal.s.klein@gmail.com",
     description="package for QA-based Semantics - representing textual information via question-answer pairs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kleinay/QASem",
     packages=setuptools.find_packages(),
     install_requires=[
-        'transformers==4.15.0',
-        'spacy>=3.0.0',
-        'qanom',
-        'roleqgen',
-        'markupsafe==2.0.1', # downgrade because of bug in 2.1.1, https://stackoverflow.com/questions/72191560/importerror-cannot-import-name-soft-unicode-from-markupsafe
+        'qanom>=0.0.31',
+        'transformers>=4.15.0',
+        'spacy>=3.0.0,<4.0',
+        # 'constrained_decoding',
+        # 'markupsafe==2.1.2', # downgrade because of bug in 2.1.1, https://stackoverflow.com/questions/72191560/importerror-cannot-import-name-soft-unicode-from-markupsafe
     ],
     package_data={
         "": ["qasem/data/connectives_small_set.txt"],
     },
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```

