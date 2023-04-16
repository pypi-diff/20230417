# Comparing `tmp/developergpt-0.2.1.tar.gz` & `tmp/developergpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developergpt-0.2.1.tar", last modified: Sun Apr 16 22:05:10 2023, max compression
+gzip compressed data, was "developergpt-0.2.2.tar", last modified: Sun Apr 16 22:53:15 2023, max compression
```

## Comparing `developergpt-0.2.1.tar` & `developergpt-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 22:04:59.000000 developergpt-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 22:04:59.000000 developergpt-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-16 22:05:10.465326 developergpt-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-16 22:04:59.000000 developergpt-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/developergpt/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/huggingface_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/openai_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-16 22:04:59.000000 developergpt-0.2.1/developergpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/developergpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 22:05:10.000000 developergpt-0.2.1/developergpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:05:10.465326 developergpt-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 22:04:59.000000 developergpt-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:05:10.465326 developergpt-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 22:04:59.000000 developergpt-0.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:15.500965 developergpt-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 22:53:05.000000 developergpt-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 22:53:05.000000 developergpt-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-16 22:53:15.500965 developergpt-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 22:53:05.000000 developergpt-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:15.500965 developergpt-0.2.2/developergpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/huggingface_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/openai_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-16 22:53:05.000000 developergpt-0.2.2/developergpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:15.500965 developergpt-0.2.2/developergpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 22:53:15.000000 developergpt-0.2.2/developergpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:53:15.500965 developergpt-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 22:53:05.000000 developergpt-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:15.500965 developergpt-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:53:05.000000 developergpt-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 22:53:05.000000 developergpt-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 22:53:05.000000 developergpt-0.2.2/tests/test_cli.py
```

### Comparing `developergpt-0.2.1/LICENSE` & `developergpt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/PKG-INFO` & `developergpt-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -88,14 +88,16 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
+**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above.
```

### Comparing `developergpt-0.2.1/README.md` & `developergpt-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
+**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above.
```

### Comparing `developergpt-0.2.1/developergpt/cli.py` & `developergpt-0.2.2/developergpt/cli.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/developergpt/config.py` & `developergpt-0.2.2/developergpt/config.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/developergpt/huggingface_adapter.py` & `developergpt-0.2.2/developergpt/huggingface_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
 
 BLOOM_CHAT_PROMPT = """The following is a conversation with a software development expert chatbot. 
     The chatbot should be able to understand and respond to questions and statements about a variety of topics related to Computer Science and Software Development. 
     The chatbot is conversational, flexible, and should be able to engage in casual, friendly conversation to assist the user.
     The chatbot should also be able to maintain context across multiple turns of conversation.\n"""
 
-# examples created using ChatGPT output
 raw_chat_msgs = [
     "User: What is the difference between x86 and ARM architecture?",
     """Assistant: x86 and ARM are two different processor architectures used in modern computing devices. They have different instruction sets, 
     with x86 using a CISC instruction set and ARM using a RISC instruction set. x86 processors typically have higher clock speeds and can execute more instructions per clock cycle, while ARM processors are more power-efficient.
     x86 processors are compatible with a wide range of operating systems, while ARM processors are commonly used in mobile devices and are generally less expensive than x86 processors.""",
     "User: What are LDFLAGS in a Makefile?",
     """Assistant, LDFLAGS is a variable used in Makefiles that contains linker flags or options to pass to the linker program.
```

### Comparing `developergpt-0.2.1/developergpt/openai_adapter.py` & `developergpt-0.2.2/developergpt/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/developergpt/utils.py` & `developergpt-0.2.2/developergpt/utils.py`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/developergpt.egg-info/PKG-INFO` & `developergpt-0.2.2/developergpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developergpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: developergpt is a command line tool that allows users to use natural language to execute commands and chat with the latest LLMs
 Home-page: https://github.com/luo-anthony/DeveloperGPT/
 Author: luo-anthony
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -88,14 +88,16 @@
 # natural langauge to terminal commands using BLOOM model instead
 $ developergpt --model bloom cmd
 
 # give feedback
 $ developergpt feedback
 ```
 
+**NOTE:**: DeveloperGPT is **NOT** to be used for any purposes forbidden by the terms of use of the LLMs used (GPT-3.5, BLOOM). Additionally, DeveloperGPT itself (apart from the LLMs) is a proof of concept tool and is not intended to be used for any serious or commerical work. 
+
 ### OpenAI API Usage (GPT-3.5)
 You can monitor your OpenAI API usage here: https://platform.openai.com/account/usage
 
 DeveloperGPT uses the `gpt-3.5-turbo` model which is very cost efficient (1/10 the cost of models such as `text-davinci-003`). Based on preliminary testing, using DeveloperGPT should cost no more than 10 cents per day (assuming ~100 requests/day). 
 
 ### Hugging-Face Usage (BLOOM)
 Currently, using the BLOOM model does not require a token and is free but rate limited. To avoid rate limit, you can set a token using the instructions above.
```

### Comparing `developergpt-0.2.1/developergpt.egg-info/SOURCES.txt` & `developergpt-0.2.2/developergpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `developergpt-0.2.1/setup.py` & `developergpt-0.2.2/setup.py`

 * *Files identical despite different names*

