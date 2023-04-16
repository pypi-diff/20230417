# Comparing `tmp/developergpt-0.1.7.tar.gz` & `tmp/developergpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.1.7.tar", last modified: Sat Apr 15 19:20:48 2023, max compression
+gzip compressed data, was "developergpt-0.2.1.tar", last modified: Sun Apr 16 22:05:10 2023, max compression
```

## Comparing `developergpt-0.1.7.tar` & `developergpt-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.444974 developergpt-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-15 19:20:35.000000 developergpt-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 19:20:35.000000 developergpt-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-15 19:20:48.440973 developergpt-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-15 19:20:35.000000 developergpt-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-15 19:20:35.000000 developergpt-0.1.7/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 19:20:48.000000 developergpt-0.1.7/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:20:48.444974 developergpt-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-15 19:20:35.000000 developergpt-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:48.440973 developergpt-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 19:20:35.000000 developergpt-0.1.7/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 22:04:59.000000 developergpt-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 22:04:59.000000 developergpt-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-16 22:05:10.465326 developergpt-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-16 22:04:59.000000 developergpt-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:05:10.465326 developergpt-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 22:04:59.000000 developergpt-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/test_cli.py
```

### Comparing `developergpt-0.1.7/LICENSE` & `developergpt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.7/PKG-INFO` & `developergpt-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,101 @@
-Metadata-Version: 2.1
-Name: developergpt
-Version: 0.1.7
-Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
-Home-page: https://github.com/luo-anthony/DeveloperGPT/
-Author: luo-anthony
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
+
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model (some features are currently not supported when using BLOOM). Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+
+In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** **GPT3.5 (default)**, BLOOM
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** Currently, command explanations are **not** supported when using BLOOM. Commands using BLOOM may also require more revision to get the desired output. 
+**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
+
+With both models, it is always good practice to manually verify the command output before running it.
 
-#### 2. Chat with GPT-3.5 Inside the Terminal
-**Supported Models:** **GPT3.5 (only)**
+#### 2. Chat inside the Terminal
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
-**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI terms of use. 
+**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-DeveloperGPT uses the GPT-3.5 model from OpenAI by default (with full feature support). 
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
 Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 
 ```bash
 # Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you just want to use the BLOOM model with **Feature 1 (Natural Language to Terminal Commands)** only, you don't need to setup an OpenAI key.
+If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+
+```bash
+# Do this once 
+# set Hugging Face API token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
-# chat with GPT-3.5 inside the terminal 
+# chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
-# natural langauge to terminal commands using BLOOM
+# chat with DeveloperGPT using BLOOM model instead
+$ developergpt --model bloom chat
+
+# natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face API Usage (BLOOM)
-Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
+### Hugging-Face Usage (BLOOM)
+Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
-
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
-- Thanks to Hugging Face and the NLP community for open-source models! 
+- Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
-- This project was written with assistance from ChatGPT and Github CoPilot.
+- This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.7/README.md` & `developergpt-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,112 @@
+Metadata-Version: 2.1
+Name: developergpt
+Version: 0.2.1
+Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
+Home-page: https://github.com/luo-anthony/DeveloperGPT/
+Author: luo-anthony
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
+
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model (some features are currently not supported when using BLOOM). Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+
+In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** **GPT3.5 (default)**, BLOOM
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** Currently, command explanations are **not** supported when using BLOOM. Commands using BLOOM may also require more revision to get the desired output. 
+**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
+
+With both models, it is always good practice to manually verify the command output before running it.
 
-#### 2. Chat with GPT-3.5 Inside the Terminal
-**Supported Models:** **GPT3.5 (only)**
+#### 2. Chat inside the Terminal
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
-**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI terms of use. 
+**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-DeveloperGPT uses the GPT-3.5 model from OpenAI by default (with full feature support). 
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
 Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 
 ```bash
 # Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you just want to use the BLOOM model with **Feature 1 (Natural Language to Terminal Commands)** only, you don't need to setup an OpenAI key.
+If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+
+```bash
+# Do this once 
+# set Hugging Face API token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
-# chat with GPT-3.5 inside the terminal 
+# chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
-# natural langauge to terminal commands using BLOOM
+# chat with DeveloperGPT using BLOOM model instead
+$ developergpt --model bloom chat
+
+# natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face API Usage (BLOOM)
-Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
+### Hugging-Face Usage (BLOOM)
+Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
-
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
-- Thanks to Hugging Face and the NLP community for open-source models! 
+- Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
-- This project was written with assistance from ChatGPT and Github CoPilot. 
+- This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.7/developergpt/cli.py` & `developergpt-0.2.1/developergpt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,68 +54,71 @@
     "--model",
     default="gpt-3.5",
     help="The language model to use. Options: gpt-3.5 (default), bloom",
 )
 @click.pass_context
 def main(ctx, temperature, model):
     model = model.lower().strip()
+    if not utils.check_connectivity():
+        console.print(
+            "[bold red]No internet connection. Please check your internet connection and try again.[/bold red]"
+        )
+        sys.exit(-1)
+
     if model not in config.SUPPORTED_MODELS:
         console.print(
             f"""[bold red]Model {model} is not supported. 
             Supported models: {",".join(config.SUPPORTED_MODELS)}[/bold red]"""
         )
         sys.exit(-1)
+
+    ctx.ensure_object(dict)
     if model == config.GPT35:
         openai.api_key = config.get_environ_key(config.OPEN_AI_API_KEY, console)
+        openai_adapter.check_open_ai_key(console)
     elif model == config.BLOOM:
+        ctx.obj["api_key"] = config.get_environ_key_optional(
+            config.HUGGING_FACE_API_KEY, console
+        )
         console.print(
-            "[bold yellow]Using Bloom 176B model: some features may not be supported and results may not be as good as using GPT-3.5.[/bold yellow]"
+            "[bold yellow]Using Bloom 176B model: some features may have unexpected behavior and results may not be as good as using GPT-3.5.[/bold yellow]"
         )
-        # we don't need the api key for bloom yet
 
-    ctx.ensure_object(dict)
     ctx.obj["temperature"] = temperature
     ctx.obj["model"] = model
 
 
 @click.command(help="Chat with DeveloperGPT")
 @click.pass_context
 @handle_api_error
 def chat(ctx):
-    # TODO save previous conversations like the web interface does?
-    if ctx.obj["model"] != config.GPT35:
-        console.print(
-            f"""[bold red]Model {ctx.obj["model"]} is not supported for chat. 
-            Supported models: {config.GPT35}[/bold red]"""
-        )
-        sys.exit(-1)
+    model = ctx.obj["model"]
 
-    MODEL = "gpt-3.5-turbo"
-    MAX_TOKENS = 4000
-    RESERVED_OUTPUT_TOKENS = 1024
-    MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
-    input_messages = [openai_adapter.INITIAL_CHAT_SYSTEM_MSG]
+    if model == config.GPT35:
+        input_messages = [openai_adapter.INITIAL_CHAT_SYSTEM_MSG]
+    elif model == config.BLOOM:
+        input_messages = huggingface_adapter.BASE_INPUT_CHAT_MSGS
     console.print("[gray]Type 'quit' to exit the chat[/gray]")
     while True:
         user_input = utils.prompt_user_input(
             "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
         )
 
         if len(user_input) == 0:
             continue
 
-        input_messages.append({"role": "user", "content": user_input})
-        input_messages, n_input_tokens = utils.check_reduce_context(
-            input_messages, MAX_INPUT_TOKENS, MODEL, ctx_removal_index=1
-        )
-        n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
-        full_response = openai_adapter.get_model_chat_response(
-            MODEL, console, input_messages, n_output_tokens, ctx.obj["temperature"]
-        )
-        input_messages.append({"role": "assistant", "content": full_response})
+        if model == config.GPT35:
+            input_messages = openai_adapter.get_model_chat_response(
+                user_input, console, input_messages, ctx.obj["temperature"]
+            )
+        elif model == config.BLOOM:
+            api_token = ctx.obj.get("api_key", None)
+            input_messages = huggingface_adapter.get_model_chat_response(
+                user_input, console, input_messages, api_token
+            )
 
 
 kb = KeyBindings()
 
 
 @kb.add(Keys.Enter, eager=True)
 def _(event: KeyPressEvent):
@@ -135,46 +138,52 @@
     input_request = "\nDesired Command Request: "
 
     model = ctx.obj["model"]
     input_messages = copy.deepcopy(openai_adapter.BASE_INPUT_CMD_MSGS)
 
     console.print("[gray]Type 'quit' to exit[/gray]")
 
+    if model == config.BLOOM:
+        console.print(
+            "[bold yellow]WARNING: Bloom 176B model command outputs are less accurate than GPT-3.5. Check all commands before running them.[/bold yellow]"
+        )
+
     while True:
         user_input = utils.prompt_user_input(
             input_request,
             session,
             console,
             completer=utils.PathCompleter(),
             complete_style=CompleteStyle.MULTI_COLUMN,
             key_bindings=kb,
         )
         if len(user_input) == 0:
             continue
 
         if model == config.GPT35:
-            commands = openai_adapter.model_command(user_input, console, input_messages)
+            model_output = openai_adapter.model_command(
+                user_input, console, input_messages
+            )
         elif model == config.BLOOM:
-            commands = huggingface_adapter.model_command(user_input, console)
+            model_output = huggingface_adapter.model_command(user_input, console)
 
+        commands = utils.print_command_response(model_output, console)
         if not commands:
             continue
 
-        # TODO: make this look nicer
         # Give user options to revise query, execute command(s), or quit
         options = [
             "Revise Query",
             "Execute Command(s)",
             "Copy Command(s) to Clipboard",
             "Quit",
         ]
         questions = [
             inquirer.List("Next", message="What would you like to do?", choices=options)
         ]
-
         selected_option = inquirer.prompt(questions)["Next"]
 
         if selected_option == "Revise Query":
             input_request = "Revised Command Request: "
             continue
         elif selected_option == "Execute Command(s)":
             console.print("[bold blue]Executing command(s)...\n[/bold blue]")
@@ -199,14 +208,21 @@
         sys.exit(0)
 
 
 @click.command()
 @click.pass_context
 def test(ctx):
     pass
+    # while True:
+    #     user_input = utils.prompt_user_input(
+    #         "Chat: ", session, console, auto_suggest=AutoSuggestFromHistory()
+    #     )
+
+    #     if len(user_input) == 0:
+    #         continue
 
 
 @click.command(help="Give feedback")
 def feedback():
     console.print(
         "Thanks for using DeveloperGPT! You can [bold blue][link=https://forms.gle/J36KbztsRAPHXnrKA]give feedback here[/link][/bold blue]!"
     )
```

### Comparing `developergpt-0.1.7/developergpt/openai_adapter.py` & `developergpt-0.2.1/developergpt/openai_adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 DeveloperGPT by luo-anthony
 """
-import json
 import platform
+import sys
 from datetime import datetime
 
 import openai
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from rich.panel import Panel
@@ -63,19 +63,19 @@
 search_output_example = """
     {
         "input": "search the ~/Documents/ directory for any .py file that begins with 'test'",
         "error" : 0,
         "commands": [
             {
                 "seq": 1,
-                "cmd_to_execute": "find ~/Documents/ -name "test*.py"",
+                "cmd_to_execute": "find ~/Documents/ -name 'test*.py'",
                 "cmd_explanations": ["`find` is used to list files."],
                 "arg_explanations": [
                                         "``~/Documents` specifies the folder to search in.",
-                                        "`-name "test.py"` specifies that we want to search for files starting with `test` and ending with `.py`."
+                                        "`-name 'test.py'` specifies that we want to search for files starting with `test` and ending with `.py`."
                                     ]
             }
         ]
     }
     """
 
 unknown_query_output_example_one = (
@@ -142,65 +142,74 @@
 )
 
 NEGATIVE_EXAMPLE_ONE = (
     format_user_request("the quick brown fox jumped over"),
     format_assistant_response(unknown_query_output_example_one),
 )
 
+BASE_INPUT_CMD_MSGS = [
+    INITIAL_CMD_SYSTEM_MSG,
+    INITIAL_USER_CMD_MSG,
+    *EXAMPLE_ONE,
+    *EXAMPLE_TWO,
+    *NEGATIVE_EXAMPLE_ONE,
+]
+
 
 def get_model_chat_response(
-    model: str, console: "Console", messages: list, max_tokens: int, temperature: float
-) -> str:
+    user_input: str, console: "Console", input_messages: list, temperature: float
+) -> list:
+    MODEL = "gpt-3.5-turbo"
+    MAX_TOKENS = 4000
+    RESERVED_OUTPUT_TOKENS = 1024
+    MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
+
+    input_messages.append({"role": "user", "content": user_input})
+    input_messages, n_input_tokens = utils.check_reduce_context(
+        input_messages, MAX_INPUT_TOKENS, MODEL, ctx_removal_index=1
+    )
+    n_output_tokens = max(RESERVED_OUTPUT_TOKENS, MAX_TOKENS - n_input_tokens)
+
     """Get the response from the model."""
     response = openai.ChatCompletion.create(
-        model=model,
-        messages=messages,
-        max_tokens=max_tokens,
+        model=MODEL,
+        messages=input_messages,
+        max_tokens=n_output_tokens,
         temperature=temperature,
         stream=True,
     )
 
     collected_messages = []
     panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
     output_panel = Panel(
         "",
         title="[bold blue]DeveloperGPT[/bold blue]",
         title_align="left",
         width=panel_width,
     )
 
-    # TODO prettify the output
     with Live(output_panel, refresh_per_second=4):
         for chunk in response:
             msg = chunk["choices"][0]["delta"].get("content", "")
             collected_messages.append(msg)
             output_panel.renderable = Markdown(
                 "".join(collected_messages), inline_code_theme="monokai"
             )
 
     full_response = "".join(collected_messages)
-    return full_response
-
-
-BASE_INPUT_CMD_MSGS = [
-    INITIAL_CMD_SYSTEM_MSG,
-    INITIAL_USER_CMD_MSG,
-    *EXAMPLE_ONE,
-    *EXAMPLE_TWO,
-    *NEGATIVE_EXAMPLE_ONE,
-]
+    input_messages.append({"role": "assistant", "content": full_response})
+    return input_messages
 
 
 def model_command(user_input: str, console: "Console", input_messages: list) -> list:
     MODEL = "gpt-3.5-turbo"
     MAX_TOKENS = 4000
     RESERVED_OUTPUT_TOKENS = 1024
     MAX_INPUT_TOKENS = MAX_TOKENS - RESERVED_OUTPUT_TOKENS
     TEMP = 0.05
-    panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
 
     input_messages.append(format_user_request(user_input))
 
     n_input_tokens = utils.count_msg_tokens(input_messages, MODEL)
 
     if n_input_tokens > MAX_INPUT_TOKENS:
         input_messages, n_input_tokens = utils.remove_old_contexts(
@@ -218,52 +227,27 @@
             model=MODEL,
             messages=input_messages,
             max_tokens=n_output_tokens,
             temperature=TEMP,
         )
 
     model_output = response["choices"][0]["message"]["content"].strip()
-    try:
-        output_data = json.loads(model_output)
-    except json.decoder.JSONDecodeError:
-        console.print(
-            "[bold red]Error: Could not parse model response properly[/bold red]"
-        )
-        console.log(model_output)
-        return []
-
-    if output_data.get("error", 0) or "commands" not in output_data:
-        console.print(
-            "[bold red]Error: Could not find commands for this request[/bold red]"
-        )
-        return []
 
-    commands = output_data.get("commands", {})
-    cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
+    return model_output
 
-    # print all the commands in a panel
-    utils.pretty_print_commands(cmd_strings, console, panel_width)
 
-    # print all the explanations in a panel
-    explanation_items = []
-    for cmd in commands:
-        explanation_items.extend([f"- {c}" for c in cmd.get("cmd_explanations", [])])
-        explanation_items.extend([f"\t- {c}" for c in cmd.get("arg_explanations", [])])
-
-    arg_out = Markdown("\n".join(explanation_items))
-
-    console.print(
-        Panel(
-            arg_out,
-            title="[bold blue]Explanation[/bold blue]",
-            title_align="left",
-            width=panel_width,
+def check_open_ai_key(console: "Console") -> None:
+    """Check if the OpenAI API key is valid."""
+    try:
+        _ = openai.Model.list()
+    except openai.error.AuthenticationError:
+        console.print(
+            f"[bold red]Error: Invalid OpenAI API key. Check your {config.OPEN_AI_API_KEY} environment variable.[/bold red]"
         )
-    )
-    return cmd_strings
+        sys.exit(-1)
 
 
 # def format_model_output(text: str) -> str:
 #     """Format the model output to be more readable."""
 #     text = re.sub(
 #         r"```(.+?)```", "[syntax]" + r"\1" + "[/syntax]", text, flags=re.DOTALL
 #     )
```

### Comparing `developergpt-0.1.7/developergpt/utils.py` & `developergpt-0.2.1/developergpt/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 DeveloperGPT by luo-anthony
 """
 
 
+import json
 import os
 import sys
 
 import pyperclip
+import requests
 import tiktoken
 from prompt_toolkit.completion import Completer, Completion
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.panel import Panel
 
 from developergpt import config
@@ -31,14 +33,60 @@
             title="[bold blue]Command(s)[/bold blue]",
             title_align="left",
             width=panel_width,
         )
     )
 
 
+def print_command_response(model_output: str, console: "Console"):
+    if not model_output:
+        return []
+
+    panel_width = min(console.width, config.DEFAULT_COLUMN_WIDTH)
+
+    try:
+        output_data = json.loads(model_output)
+    except json.decoder.JSONDecodeError:
+        console.print(
+            "[bold red]Error: Could not parse model response properly[/bold red]"
+        )
+        console.log(model_output)
+        return []
+
+    if output_data.get("error", 0) or "commands" not in output_data:
+        console.print(
+            "[bold red]Error: Could not find commands for this request[/bold red]"
+        )
+        return []
+
+    commands = output_data.get("commands", {})
+    cmd_strings = [cmd.get("cmd_to_execute", "") for cmd in commands]
+
+    # print all the commands in a panel
+    pretty_print_commands(cmd_strings, console, panel_width)
+
+    # print all the explanations in a panel
+    explanation_items = []
+    for cmd in commands:
+        explanation_items.extend([f"- {c}" for c in cmd.get("cmd_explanations", [])])
+        explanation_items.extend([f"\t- {c}" for c in cmd.get("arg_explanations", [])])
+
+    arg_out = Markdown("\n".join(explanation_items))
+
+    console.print(
+        Panel(
+            arg_out,
+            title="[bold blue]Explanation[/bold blue]",
+            title_align="left",
+            width=panel_width,
+        )
+    )
+    return cmd_strings
+
+
 def copy_comands_to_cliboard(commands: list):
     pyperclip.copy("\n".join(commands))
 
 
 def prompt_user_input(
     input_request,
     session,
@@ -178,7 +226,15 @@
 
                 # substitute for the full path but only display the basename of the file
                 yield Completion(
                     completion,
                     display=os.path.basename(completion),
                     start_position=-len(text),
                 )
+
+
+def check_connectivity(url="http://www.google.com", timeout=8):
+    try:
+        _ = requests.get(url, timeout=timeout)
+        return True
+    except requests.ConnectionError:
+        return False
```

### Comparing `developergpt-0.1.7/developergpt.egg-info/PKG-INFO` & `developergpt-0.2.1/developergpt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,112 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.1.7
-Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models
+Version: 0.2.1
+Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # DeveloperGPT
 [![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
 [![CI](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml/badge.svg)](https://github.com/luo-anthony/DeveloperGPT/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/developergpt)](https://pypi.org/project/developergpt/)
+[![LLMs](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)](https://img.shields.io/badge/Supported%20LLMs-GPT3.5,%20BLOOM-blue)
+
 
 <!-- [![codecov](https://codecov.io/gh/luo-anthony/DeveloperGPT/branch/main/graph/badge.svg?token=DeveloperGPT_token_here)](https://codecov.io/gh/luo-anthony/DeveloperGPT) -->
 
 DeveloperGPT is a terminal application that uses the latest LLMs to help developers be more productive. 
 
-By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model (some features are currently not supported when using BLOOM). Support for more models and features is coming soon! 
+By default, DeveloperGPT uses the [gpt-3.5-turbo](https://platform.openai.com/docs/models) model from OpenAI, but you can also use the open-source [BLOOM](https://bigscience.huggingface.co/blog/bloom) model. Support for more models and features is coming soon! 
+
+In our testing, we recommend GPT-3.5 (default) as it generally yields better results and is able to handle more complex requests. 
 
 DeveloperGPT has two main features:
 #### 1. Natural Language to Terminal Commands
-**Supported Models:** **GPT3.5 (default)**, BLOOM
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Natural Language Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/cmddemo.gif)
 
-**NOTE:** Currently, command explanations are **not** supported when using BLOOM. Commands using BLOOM may also require more revision to get the desired output. 
+**NOTE:** The BLOOM model command output may not be accurate, especially for more complex commands. Using the BLOOM model may also result in unexpected or undefined behavior. 
+
+With both models, it is always good practice to manually verify the command output before running it.
 
-#### 2. Chat with GPT-3.5 Inside the Terminal
-**Supported Models:** **GPT3.5 (only)**
+#### 2. Chat inside the Terminal
+**Supported Models:** GPT3.5 (default), BLOOM
 ![Chat Example](https://github.com/luo-anthony/DeveloperGPT/raw/main/samples/chatdemo.gif)
 
-**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI terms of use. 
+**NOTE:** Chat moderation is **NOT** implemented - all your chat messages should follow the OpenAI and BLOOM terms of use. 
 
 
 ## Install DeveloperGPT from PyPI
 ```bash
 pip install -U developergpt
 ```
 
 ### Setup
 
-DeveloperGPT uses the GPT-3.5 model from OpenAI by default (with full feature support). 
+By default, DeveloperGPT uses the GPT-3.5 model from OpenAI. From limited testing, the GPT-3.5 model has the best results. 
 
 Get your own OpenAI API Key: https://platform.openai.com/account/api-keys
 
 ```bash
 # Do this once 
 # set OpenAI API Key (using zsh for example)
 $ echo 'export OPENAI_API_KEY=[your_key_here]' >> ~/.zshenv
 
 # reload the environment (or just quit and open a new terminal)
 $ source ~/.zshenv
 ```
 
-If you just want to use the BLOOM model with **Feature 1 (Natural Language to Terminal Commands)** only, you don't need to setup an OpenAI key.
+If you want to use the BLOOM model instead, you can optionally set up a [Hugging Face User Access](https://huggingface.co/settings/tokens) or [Inference API](https://huggingface.co/docs/api-inference/index) token. Setting up a token is not required (BLOOM model will work without any token or key), but it will allow you to make more requests without being rate limited. 
+
+```bash
+# Do this once 
+# set Hugging Face API token (using zsh for example)
+$ echo 'export HUGGING_FACE_API_KEY=[your_key_here]' >> ~/.zshenv
+
+# reload the environment (or just quit and open a new terminal)
+$ source ~/.zshenv
+```
 
 ## Usage
 ```bash
 # see available commands
 $ developergpt 
 
-# chat with GPT-3.5 inside the terminal 
+# chat with DeveloperGPT using GPT-3.5 (default)
 $ developergpt chat
 
 # natural language to terminal commands using GPT-3.5 (default)
 $ developergpt cmd
 
-# natural langauge to terminal commands using BLOOM
+# chat with DeveloperGPT using BLOOM model instead
+$ developergpt --model bloom chat
+
+# natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
-### Hugging-Face API Usage (BLOOM)
-Currently, using the BLOOM model does not require a [Hugging Face Inference API](https://huggingface.co/docs/api-inference/index) token and is free (but rate limited). 
+### Hugging-Face Usage (BLOOM)
+Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above. 
 
 ## Contributing
-
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ### Future Roadmap
 - Add support for open-source models (Alpaca, Vicuna, Dolly, etc.)
 
 ## Credit
-- Thanks to Hugging Face and the NLP community for open-source models! 
+- Thanks to Hugging Face and the NLP community for open-source models and prompts! 
 - This project uses the Python project template from https://github.com/rochacbruno/python-project-template
 - This project was written with assistance from ChatGPT and Github CoPilot.
```

### Comparing `developergpt-0.1.7/developergpt.egg-info/SOURCES.txt` & `developergpt-0.2.1/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.1.7/setup.py` & `developergpt-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,20 +28,18 @@
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
 
 setup(
     name="developergpt",
     version=read("developergpt", "VERSION"),
-    python_requires='>=3.9',
-    description="developergpt is a command line tool that allows users to use natural language to execute commands and chat with GPT-3.5 models",
+    python_requires=">=3.9",
+    description="developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs",
     url="https://github.com/luo-anthony/DeveloperGPT/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="luo-anthony",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
-    entry_points={
-        "console_scripts": ["developergpt = developergpt.__main__:main"]
-    },
+    entry_points={"console_scripts": ["developergpt = developergpt.__main__:main"]},
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

