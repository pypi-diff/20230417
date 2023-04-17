# Comparing `tmp/llama_inference-0.0.2.post1.tar.gz` & `tmp/llama_inference-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_inference-0.0.2.post1.tar", last modified: Sun Apr 16 21:02:24 2023, max compression
+gzip compressed data, was "llama_inference-0.0.3.tar", last modified: Mon Apr 17 10:34:22 2023, max compression
```

## Comparing `llama_inference-0.0.2.post1.tar` & `llama_inference-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.021332 llama_inference-0.0.2.post1/
--rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.2.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.2.post1/CONTRIBUTING.md
--rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.2.post1/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)      783 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)     1604 2023-04-16 21:02:24.021457 llama_inference-0.0.2.post1/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)     1243 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/README.md
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.017386 llama_inference-0.0.2.post1/assets/
--rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.2.post1/assets/llama-inference-api-min.png
--rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-16 21:02:24.021903 llama_inference-0.0.2.post1/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)      148 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/setup.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.019164 llama_inference-0.0.2.post1/src/
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.019899 llama_inference-0.0.2.post1/src/llama_inference/
--rw-r--r--   0 aniket     (501) staff       (20)      123 2023-04-16 21:01:53.000000 llama_inference-0.0.2.post1/src/llama_inference/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     4968 2023-04-16 21:01:50.000000 llama_inference-0.0.2.post1/src/llama_inference/model.py
--rw-r--r--   0 aniket     (501) staff       (20)      695 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/src/llama_inference/serve.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.021127 llama_inference-0.0.2.post1/src/llama_inference.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)     1604 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      443 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/requires.txt
--rw-r--r--   0 aniket     (501) staff       (20)       16 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/top_level.txt
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/src/requirements.txt
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.923315 llama_inference-0.0.3/
+-rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.3/LICENSE
+-rw-r--r--   0 aniket     (501) staff       (20)      834 2023-04-17 06:38:34.000000 llama_inference-0.0.3/MANIFEST.in
+-rw-r--r--   0 aniket     (501) staff       (20)     1934 2023-04-17 10:34:22.923465 llama_inference-0.0.3/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)     1579 2023-04-17 07:35:21.000000 llama_inference-0.0.3/README.md
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.916378 llama_inference-0.0.3/assets/
+-rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.3/assets/llama-inference-api-min.png
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.918709 llama_inference-0.0.3/requirements/
+-rw-r--r--   0 aniket     (501) staff       (20)      122 2023-04-17 06:38:34.000000 llama_inference-0.0.3/requirements/chatbot.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:22:06.000000 llama_inference-0.0.3/requirements/requirements.txt
+-rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-17 10:34:22.923949 llama_inference-0.0.3/setup.cfg
+-rw-r--r--   0 aniket     (501) staff       (20)      314 2023-04-17 06:38:34.000000 llama_inference-0.0.3/setup.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.914654 llama_inference-0.0.3/src/
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.919593 llama_inference-0.0.3/src/chatbot/
+-rw-r--r--   0 aniket     (501) staff       (20)       47 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1803 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/base.py
+-rw-r--r--   0 aniket     (501) staff       (20)     2296 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/chain.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.920292 llama_inference-0.0.3/src/chatbot/ui/
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1692 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/main.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1337 2023-04-17 07:35:21.000000 llama_inference-0.0.3/src/chatbot/ui/templates.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.921470 llama_inference-0.0.3/src/llama_inference/
+-rw-r--r--   0 aniket     (501) staff       (20)      118 2023-04-17 10:34:09.000000 llama_inference-0.0.3/src/llama_inference/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     4968 2023-04-17 06:38:34.000000 llama_inference-0.0.3/src/llama_inference/model.py
+-rw-r--r--   0 aniket     (501) staff       (20)     1136 2023-04-17 06:38:34.000000 llama_inference-0.0.3/src/llama_inference/serve.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-17 10:34:22.922861 llama_inference-0.0.3/src/llama_inference.egg-info/
+-rw-r--r--   0 aniket     (501) staff       (20)     1934 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      620 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       31 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/requires.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       35 2023-04-17 10:34:22.000000 llama_inference-0.0.3/src/llama_inference.egg-info/top_level.txt
```

### Comparing `llama_inference-0.0.2.post1/CODE_OF_CONDUCT.md` & `llama_inference-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2.post1/CONTRIBUTING.md` & `llama_inference-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2.post1/LICENSE` & `llama_inference-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2.post1/MANIFEST.in` & `llama_inference-0.0.3/MANIFEST.in`

 * *Files 24% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 exclude tests
 
 # Exclude the documentation files
 recursive-exclude docs *
 exclude docs
 
 # Include the Requirements
-include src/requirements.txt
-recursive-include src/requirements *.txt
+include requirements/requirements.txt
+include requirements/chatbot.txt
+recursive-include requirements/requirements *.txt
 
 # Exclude Makefile
 exclude Makefile
 
 prune .git
 prune .github
 prune scripts
```

### Comparing `llama_inference-0.0.2.post1/README.md` & `llama_inference-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -38,18 +38,33 @@
 
 ## For deploying as a REST API
 
 Create a Python file `app.py` and initialize the `ServeLLaMA` App.
 
 ```python
 # app.py
-from llama_inference.serve import ServeLLaMA, Response
+from llama_inference.serve import ServeLLaMA, Response, PromptRequest
 
 import lightning as L
 
 component = ServeLLaMA(input_type=PromptRequest, output_type=Response)
 app = L.LightningApp(component)
 ```
 
 ```bash
 lightning run app app.py
 ```
+
+## How to use the Chatbot
+
+```python
+from chatbot import LLaMAChatBot
+
+checkpoint_path = f"../../weights/state_dict.pth"
+tokenizer_path = f"../../weights/tokenizer.model"
+
+bot = LLaMAChatBot(
+    checkpoint_path=checkpoint_path, tokenizer_path=tokenizer_path
+)
+
+print(bot.send("hi, what is the capital of France?"))
+```
```

### Comparing `llama_inference-0.0.2.post1/assets/llama-inference-api-min.png` & `llama_inference-0.0.3/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2.post1/setup.cfg` & `llama_inference-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2.post1/src/llama_inference/model.py` & `llama_inference-0.0.3/src/llama_inference/model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 
     return idx
 
 
 class LLaMAInference:
     def __init__(
         self,
+        checkpoint_path: Optional[Path] = None,
+        tokenizer_path: Optional[Path] = None,
         model_size: str = "7B",
         dtype: Optional[str] = None,
         quantize: Optional[str] = None,
-        checkpoint_path: Optional[Path] = None,
-        tokenizer_path: Optional[Path] = None,
         accelerator: str = "auto",
         devices: int = 1,
     ) -> None:
         self.fabric = fabric = L.Fabric(accelerator=accelerator, devices=devices)
 
         if not checkpoint_path and WEIGHTS_PATH:
             checkpoint_path = f"{WEIGHTS_PATH}/{model_size}/state_dict.pth"
```

### Comparing `llama_inference-0.0.2.post1/src/llama_inference.egg-info/PKG-INFO` & `llama_inference-0.0.3/src/llama_inference.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-inference
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: Inference API for LLaMA
 Home-page: https://github.com/aniketmaurya/LLaMA-inference-api
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT
 Requires-Python: >=3.8
@@ -51,18 +51,33 @@
 
 ## For deploying as a REST API
 
 Create a Python file `app.py` and initialize the `ServeLLaMA` App.
 
 ```python
 # app.py
-from llama_inference.serve import ServeLLaMA, Response
+from llama_inference.serve import ServeLLaMA, Response, PromptRequest
 
 import lightning as L
 
 component = ServeLLaMA(input_type=PromptRequest, output_type=Response)
 app = L.LightningApp(component)
 ```
 
 ```bash
 lightning run app app.py
 ```
+
+## How to use the Chatbot
+
+```python
+from chatbot import LLaMAChatBot
+
+checkpoint_path = f"../../weights/state_dict.pth"
+tokenizer_path = f"../../weights/tokenizer.model"
+
+bot = LLaMAChatBot(
+    checkpoint_path=checkpoint_path, tokenizer_path=tokenizer_path
+)
+
+print(bot.send("hi, what is the capital of France?"))
+```
```

