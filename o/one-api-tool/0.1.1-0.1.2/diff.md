# Comparing `tmp/one-api-tool-0.1.1.tar.gz` & `tmp/one-api-tool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.1.1.tar", last modified: Mon Apr 17 12:25:35 2023, max compression
+gzip compressed data, was "one-api-tool-0.1.2.tar", last modified: Mon Apr 17 12:35:12 2023, max compression
```

## Comparing `one-api-tool-0.1.1.tar` & `one-api-tool-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:25:35.549615 one-api-tool-0.1.1/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.1/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     2128 2023-04-17 12:25:35.549448 one-api-tool-0.1.1/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     1572 2023-04-17 12:13:33.000000 one-api-tool-0.1.1/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:25:35.549009 one-api-tool-0.1.1/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     2128 2023-04-17 12:25:35.000000 one-api-tool-0.1.1/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-17 12:25:35.000000 one-api-tool-0.1.1/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-17 12:25:35.000000 one-api-tool-0.1.1/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-17 12:25:35.000000 one-api-tool-0.1.1/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-17 12:25:35.000000 one-api-tool-0.1.1/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:25:35.549256 one-api-tool-0.1.1/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.1/oneapi/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     9311 2023-04-17 12:12:03.000000 one-api-tool-0.1.1/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-17 12:25:35.549658 one-api-tool-0.1.1/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-17 12:25:19.000000 one-api-tool-0.1.1/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:35:12.027206 one-api-tool-0.1.2/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.1.2/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2152 2023-04-17 12:35:12.027052 one-api-tool-0.1.2/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1596 2023-04-17 12:32:42.000000 one-api-tool-0.1.2/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:35:12.026341 one-api-tool-0.1.2/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2152 2023-04-17 12:35:11.000000 one-api-tool-0.1.2/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      242 2023-04-17 12:35:12.000000 one-api-tool-0.1.2/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-04-17 12:35:11.000000 one-api-tool-0.1.2/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       60 2023-04-17 12:35:11.000000 one-api-tool-0.1.2/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-04-17 12:35:11.000000 one-api-tool-0.1.2/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-04-17 12:35:12.026778 one-api-tool-0.1.2/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       47 2023-04-17 12:21:51.000000 one-api-tool-0.1.2/oneapi/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     9311 2023-04-17 12:12:03.000000 one-api-tool-0.1.2/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-04-17 12:35:12.027253 one-api-tool-0.1.2/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      908 2023-04-17 12:34:23.000000 one-api-tool-0.1.2/setup.py
```

### Comparing `one-api-tool-0.1.1/LICENSE` & `one-api-tool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.1/PKG-INFO` & `one-api-tool-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OneAPI
 Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 ## Installation
 ```sh
-pip install -U oneapi
+pip install -U one-api-tool
 ```
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
@@ -46,17 +46,17 @@
 `api_key` OpenAI API key is availalle on the ![website](https://platform.openai.com/account/api-keys), Clade API key here ![website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
 `api_type` fixed value for "open_ai", "azure" or "anthropic"
 
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. derectly set the api_key in code
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
 print(res)
 ```
```

### Comparing `one-api-tool-0.1.1/README.md` & `one-api-tool-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # OneAPI
 Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 ## Installation
 ```sh
-pip install -U oneapi
+pip install -U one-api-tool
 ```
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
@@ -34,17 +34,17 @@
 `api_key` OpenAI API key is availalle on the ![website](https://platform.openai.com/account/api-keys), Clade API key here ![website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
 `api_type` fixed value for "open_ai", "azure" or "anthropic"
 
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. derectly set the api_key in code
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
 print(res)
 ```
```

### Comparing `one-api-tool-0.1.1/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.1.2/one_api_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OneAPI
 Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 ## Installation
 ```sh
-pip install -U oneapi
+pip install -U one-api-tool
 ```
 ## Usage
 ### 1. (Recommended method) Set your key information in the local configuration file.
 
 OpenAI config:
 ```json
 {
@@ -46,17 +46,17 @@
 `api_key` OpenAI API key is availalle on the ![website](https://platform.openai.com/account/api-keys), Clade API key here ![website](https://console.anthropic.com/account/keys)
 
 `api` The base api used to send requests, you may also specify to a proxy url like: "https://your_proxy_domain/v1". For Azure APIs, you can find relevant information on the Azure resource dashboard, the form of API is usually:  https://{your origization}.openai.azure.com/
 
 `api_type` fixed value for "open_ai", "azure" or "anthropic"
 
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config_file("your_config_file.json").simple_chat("Hello AI!")
 print(res)
 ```
 ### 2. derectly set the api_key in code
 ```python
-import oneapi
-res = oneapi.OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
+from oneapi import OneAPITool
+res = OneAPITool.from_config(api_key, api, api_type).simple_chat("Hello AI!")
 print(res)
 ```
```

### Comparing `one-api-tool-0.1.1/oneapi/one_api.py` & `one-api-tool-0.1.2/oneapi/one_api.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.1.1/setup.py` & `one-api-tool-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

