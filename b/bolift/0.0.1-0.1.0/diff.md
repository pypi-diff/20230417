# Comparing `tmp/bolift-0.0.1.tar.gz` & `tmp/bolift-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolift-0.0.1.tar", last modified: Wed Apr 12 00:11:28 2023, max compression
+gzip compressed data, was "bolift-0.1.0.tar", last modified: Mon Apr 17 07:33:47 2023, max compression
```

## Comparing `bolift-0.0.1.tar` & `bolift-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:11:28.229875 bolift-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 00:11:28.229875 bolift-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-12 00:08:11.000000 bolift-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:11:28.229875 bolift-0.0.1/bolift/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/aqfxns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/asktell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6739 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/asktellGPR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/asktellNearestNeighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/asktellRidgeRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/asktellfinetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/llm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 00:08:11.000000 bolift-0.0.1/bolift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:11:28.229875 bolift-0.0.1/bolift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 00:11:28.000000 bolift-0.0.1/bolift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-12 00:11:28.000000 bolift-0.0.1/bolift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:11:28.000000 bolift-0.0.1/bolift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 00:11:28.000000 bolift-0.0.1/bolift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 00:11:28.000000 bolift-0.0.1/bolift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:11:28.229875 bolift-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-04-12 00:08:11.000000 bolift-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:11:28.229875 bolift-0.0.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8031 2023-04-12 00:08:11.000000 bolift-0.0.1/tests/test_bolift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:33:47.298740 bolift-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-17 07:33:47.298740 bolift-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-17 07:31:15.000000 bolift-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:33:47.294740 bolift-0.1.0/bolift/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/aqfxns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/asktell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6739 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/asktellGPR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/asktellNearestNeighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/asktellRidgeRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/asktellfinetuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/llm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 07:31:15.000000 bolift-0.1.0/bolift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:33:47.294740 bolift-0.1.0/bolift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-17 07:33:47.000000 bolift-0.1.0/bolift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 07:33:47.000000 bolift-0.1.0/bolift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:33:47.000000 bolift-0.1.0/bolift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 07:33:47.000000 bolift-0.1.0/bolift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 07:33:47.000000 bolift-0.1.0/bolift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 07:33:47.298740 bolift-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-04-17 07:31:16.000000 bolift-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:33:47.294740 bolift-0.1.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8031 2023-04-17 07:31:16.000000 bolift-0.1.0/tests/test_bolift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-17 07:31:16.000000 bolift-0.1.0/tests/test_tool.py
```

### Comparing `bolift-0.0.1/PKG-INFO` & `bolift-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolift
-Version: 0.0.1
+Version: 0.1.0
 Summary: BayesOPT with LIFT
 Home-page: https://github.com/whitead/bolift
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,25 +12,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: gpr
 
 # 🤖 BO-LIFT: Bayesian Optimization using in-context learning
 
 
 ![version](https://img.shields.io/badge/version-0.0.1-brightgreen)
-[![paper](https://img.shields.io/badge/paper-arXiv-red)](#)
+[![paper](https://img.shields.io/badge/paper-arXiv-red)](https://arxiv.org/abs/2304.05341)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 
 BO-LIFT does regression with uncertainties using frozen Large Language Models by using token probabilities.
 It uses LangChain to select examples to create in-context learning prompts from training data.
 By selecting examples, it can consider more training data than it fits in the model's context window.
 Being able to predict uncertainty, allow the employment of interesting techniques such as Bayesian Optimization.
 
 ## Table of content
--[BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
+- [BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
   - [Install](#install-)
   - [Usage](#usage-)
     - [Quickstart](#quickstart-)
     - [Customising the model](#customising-the-model)
     - [Inverse design](#inverse-design)
   - [Citation](#citation)
 
@@ -38,14 +38,21 @@
 
 bolift can simply be installed using pip:
 
 ```bash
 pip install bolift
 ```
 
+Some additional requirements are needed to use the Gaussian Process Regressor (GPR) module.
+They can also be installed using pip:
+
+```bash
+pip install bolift[gpr]
+```
+
 ## Usage 💻
 
 You need to set up your OpenAI API key in order to use BO-LIFT.
 You can do that using the `os` Python library:
 
 ```py
 import os
@@ -117,15 +124,23 @@
   y_formatter=lambda y: f"{y:.2f}",
   model="gpt-4",
   selector_k=5,
   temperature=0.7,
 )
 ```
 Other arguments can be used to customize the prompt (`prefix`, `prompt_template`, `suffix`) and the in-context learning procedure (`use_quantiles`, `n_quantiles`).
-Refer to the notebooks available in the paper directory to see examples on how to use bolift.
+Additionally, we implemented other models. A brief list can be seen below:
+- AskTellFewShotMulti;
+- AskTellFewShotTopk;
+- AskTellFinetuning;
+- AskTellRidgeKernelRegression;
+- AskTellGPR;
+- AskTellNearestNeighbor.
+
+Refer to the [notebooks](https://github.com/ur-whitelab/BO-LIFT/tree/main/paper) available in the paper directory to see examples of how to use bolift and the [paper](https://arxiv.org/abs/2304.05341) for a detailed description of the classes.
 
 ### Inverse design
 
 Aiming to propose new data, `bolift` implements another approach to generate data.
 After following a similar procedure to `tell` datapoints to the model, the `inv_predict` can be used to do an inverse prediction.
 For carrying an inverse design out, we query the label we want and the model should generate a data that corresponds to that label:
 
@@ -152,16 +167,18 @@
 This generated the following procedure:
 ```
 the synthesis procedure:"A 30 wt% tungsten carbide catalyst was prepared with Cu dopant metal at 5 wt% and carburized at 835 C. The reaction was run at 350 ºC"
 ```
 
 ### Citation
 
-Please, cite [Ramos et al.](#):
+Please, cite [Ramos et al.](https://arxiv.org/abs/2304.05341):
 ```
-@article{ramos2023bolift,
-  title={Bayesian Optimization of Catalysts With In-context Learning},
-  author={Ramos, Mayk and Michtavy, Shane and Porosoff, Marc and White, Andrew D},
-  journal={arXiv preprint arXiv:submit/4836185},
-  year={2023},
+@misc{ramos2023bayesian,
+      title={Bayesian Optimization of Catalysts With In-context Learning}, 
+      author={Mayk Caldas Ramos and Shane S. Michtavy and Marc D. Porosoff and Andrew D. White},
+      year={2023},
+      eprint={2304.05341},
+      archivePrefix={arXiv},
+      primaryClass={physics.chem-ph}
 }
 ```
```

### Comparing `bolift-0.0.1/README.md` & `bolift-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # 🤖 BO-LIFT: Bayesian Optimization using in-context learning
 
 
 ![version](https://img.shields.io/badge/version-0.0.1-brightgreen)
-[![paper](https://img.shields.io/badge/paper-arXiv-red)](#)
+[![paper](https://img.shields.io/badge/paper-arXiv-red)](https://arxiv.org/abs/2304.05341)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 
 BO-LIFT does regression with uncertainties using frozen Large Language Models by using token probabilities.
 It uses LangChain to select examples to create in-context learning prompts from training data.
 By selecting examples, it can consider more training data than it fits in the model's context window.
 Being able to predict uncertainty, allow the employment of interesting techniques such as Bayesian Optimization.
 
 ## Table of content
--[BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
+- [BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
   - [Install](#install-)
   - [Usage](#usage-)
     - [Quickstart](#quickstart-)
     - [Customising the model](#customising-the-model)
     - [Inverse design](#inverse-design)
   - [Citation](#citation)
 
@@ -24,14 +24,21 @@
 
 bolift can simply be installed using pip:
 
 ```bash
 pip install bolift
 ```
 
+Some additional requirements are needed to use the Gaussian Process Regressor (GPR) module.
+They can also be installed using pip:
+
+```bash
+pip install bolift[gpr]
+```
+
 ## Usage 💻
 
 You need to set up your OpenAI API key in order to use BO-LIFT.
 You can do that using the `os` Python library:
 
 ```py
 import os
@@ -103,15 +110,23 @@
   y_formatter=lambda y: f"{y:.2f}",
   model="gpt-4",
   selector_k=5,
   temperature=0.7,
 )
 ```
 Other arguments can be used to customize the prompt (`prefix`, `prompt_template`, `suffix`) and the in-context learning procedure (`use_quantiles`, `n_quantiles`).
-Refer to the notebooks available in the paper directory to see examples on how to use bolift.
+Additionally, we implemented other models. A brief list can be seen below:
+- AskTellFewShotMulti;
+- AskTellFewShotTopk;
+- AskTellFinetuning;
+- AskTellRidgeKernelRegression;
+- AskTellGPR;
+- AskTellNearestNeighbor.
+
+Refer to the [notebooks](https://github.com/ur-whitelab/BO-LIFT/tree/main/paper) available in the paper directory to see examples of how to use bolift and the [paper](https://arxiv.org/abs/2304.05341) for a detailed description of the classes.
 
 ### Inverse design
 
 Aiming to propose new data, `bolift` implements another approach to generate data.
 After following a similar procedure to `tell` datapoints to the model, the `inv_predict` can be used to do an inverse prediction.
 For carrying an inverse design out, we query the label we want and the model should generate a data that corresponds to that label:
 
@@ -138,16 +153,18 @@
 This generated the following procedure:
 ```
 the synthesis procedure:"A 30 wt% tungsten carbide catalyst was prepared with Cu dopant metal at 5 wt% and carburized at 835 C. The reaction was run at 350 ºC"
 ```
 
 ### Citation
 
-Please, cite [Ramos et al.](#):
+Please, cite [Ramos et al.](https://arxiv.org/abs/2304.05341):
 ```
-@article{ramos2023bolift,
-  title={Bayesian Optimization of Catalysts With In-context Learning},
-  author={Ramos, Mayk and Michtavy, Shane and Porosoff, Marc and White, Andrew D},
-  journal={arXiv preprint arXiv:submit/4836185},
-  year={2023},
+@misc{ramos2023bayesian,
+      title={Bayesian Optimization of Catalysts With In-context Learning}, 
+      author={Mayk Caldas Ramos and Shane S. Michtavy and Marc D. Porosoff and Andrew D. White},
+      year={2023},
+      eprint={2304.05341},
+      archivePrefix={arXiv},
+      primaryClass={physics.chem-ph}
 }
 ```
```

### Comparing `bolift-0.0.1/bolift/aqfxns.py` & `bolift-0.1.0/bolift/aqfxns.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/asktell.py` & `bolift-0.1.0/bolift/asktell.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/asktellGPR.py` & `bolift-0.1.0/bolift/asktellGPR.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/asktellNearestNeighbor.py` & `bolift-0.1.0/bolift/asktellNearestNeighbor.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/asktellRidgeRegression.py` & `bolift-0.1.0/bolift/asktellRidgeRegression.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/asktellfinetuning.py` & `bolift-0.1.0/bolift/asktellfinetuning.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/llm_model.py` & `bolift-0.1.0/bolift/llm_model.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift/pool.py` & `bolift-0.1.0/bolift/pool.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/bolift.egg-info/PKG-INFO` & `bolift-0.1.0/bolift.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolift
-Version: 0.0.1
+Version: 0.1.0
 Summary: BayesOPT with LIFT
 Home-page: https://github.com/whitead/bolift
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,25 +12,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: gpr
 
 # 🤖 BO-LIFT: Bayesian Optimization using in-context learning
 
 
 ![version](https://img.shields.io/badge/version-0.0.1-brightgreen)
-[![paper](https://img.shields.io/badge/paper-arXiv-red)](#)
+[![paper](https://img.shields.io/badge/paper-arXiv-red)](https://arxiv.org/abs/2304.05341)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 
 BO-LIFT does regression with uncertainties using frozen Large Language Models by using token probabilities.
 It uses LangChain to select examples to create in-context learning prompts from training data.
 By selecting examples, it can consider more training data than it fits in the model's context window.
 Being able to predict uncertainty, allow the employment of interesting techniques such as Bayesian Optimization.
 
 ## Table of content
--[BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
+- [BO-LIFT](#-bo-lift-bayesian-optimization-using-in-context-learning)
   - [Install](#install-)
   - [Usage](#usage-)
     - [Quickstart](#quickstart-)
     - [Customising the model](#customising-the-model)
     - [Inverse design](#inverse-design)
   - [Citation](#citation)
 
@@ -38,14 +38,21 @@
 
 bolift can simply be installed using pip:
 
 ```bash
 pip install bolift
 ```
 
+Some additional requirements are needed to use the Gaussian Process Regressor (GPR) module.
+They can also be installed using pip:
+
+```bash
+pip install bolift[gpr]
+```
+
 ## Usage 💻
 
 You need to set up your OpenAI API key in order to use BO-LIFT.
 You can do that using the `os` Python library:
 
 ```py
 import os
@@ -117,15 +124,23 @@
   y_formatter=lambda y: f"{y:.2f}",
   model="gpt-4",
   selector_k=5,
   temperature=0.7,
 )
 ```
 Other arguments can be used to customize the prompt (`prefix`, `prompt_template`, `suffix`) and the in-context learning procedure (`use_quantiles`, `n_quantiles`).
-Refer to the notebooks available in the paper directory to see examples on how to use bolift.
+Additionally, we implemented other models. A brief list can be seen below:
+- AskTellFewShotMulti;
+- AskTellFewShotTopk;
+- AskTellFinetuning;
+- AskTellRidgeKernelRegression;
+- AskTellGPR;
+- AskTellNearestNeighbor.
+
+Refer to the [notebooks](https://github.com/ur-whitelab/BO-LIFT/tree/main/paper) available in the paper directory to see examples of how to use bolift and the [paper](https://arxiv.org/abs/2304.05341) for a detailed description of the classes.
 
 ### Inverse design
 
 Aiming to propose new data, `bolift` implements another approach to generate data.
 After following a similar procedure to `tell` datapoints to the model, the `inv_predict` can be used to do an inverse prediction.
 For carrying an inverse design out, we query the label we want and the model should generate a data that corresponds to that label:
 
@@ -152,16 +167,18 @@
 This generated the following procedure:
 ```
 the synthesis procedure:"A 30 wt% tungsten carbide catalyst was prepared with Cu dopant metal at 5 wt% and carburized at 835 C. The reaction was run at 350 ºC"
 ```
 
 ### Citation
 
-Please, cite [Ramos et al.](#):
+Please, cite [Ramos et al.](https://arxiv.org/abs/2304.05341):
 ```
-@article{ramos2023bolift,
-  title={Bayesian Optimization of Catalysts With In-context Learning},
-  author={Ramos, Mayk and Michtavy, Shane and Porosoff, Marc and White, Andrew D},
-  journal={arXiv preprint arXiv:submit/4836185},
-  year={2023},
+@misc{ramos2023bayesian,
+      title={Bayesian Optimization of Catalysts With In-context Learning}, 
+      author={Mayk Caldas Ramos and Shane S. Michtavy and Marc D. Porosoff and Andrew D. White},
+      year={2023},
+      eprint={2304.05341},
+      archivePrefix={arXiv},
+      primaryClass={physics.chem-ph}
 }
 ```
```

### Comparing `bolift-0.0.1/setup.py` & `bolift-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bolift-0.0.1/tests/test_bolift.py` & `bolift-0.1.0/tests/test_bolift.py`

 * *Files identical despite different names*

