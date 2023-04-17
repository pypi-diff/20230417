# Comparing `tmp/openai_api_call-0.3.7.tar.gz` & `tmp/openai_api_call-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.7.tar", last modified: Thu Apr 13 08:30:29 2023, max compression
+gzip compressed data, was "openai_api_call-0.3.8.tar", last modified: Mon Apr 17 13:36:36 2023, max compression
```

## Comparing `openai_api_call-0.3.7.tar` & `openai_api_call-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 08:30:29.000000 openai_api_call-0.3.7/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:30:29.992414 openai_api_call-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:30:18.000000 openai_api_call-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.489138 openai_api_call-0.3.8/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:36:36.489138 openai_api_call-0.3.8/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 13:36:36.000000 openai_api_call-0.3.8/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:36:36.493137 openai_api_call-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-17 13:36:24.000000 openai_api_call-0.3.8/setup.py
```

### Comparing `openai_api_call-0.3.7/LICENSE` & `openai_api_call-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.7/PKG-INFO` & `openai_api_call-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.7
+Version: 0.3.8
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -130,14 +130,17 @@
         # fake response
         chat.user("What's your name?")
         chat.assistant("My name is GPT-3.5.")
         
         # get the last result
         print(chat[-1])
         
+        # save chat history
+        chat.save("chat_history.log", mode="w") # default to "a"
+        
         # print chat history
         chat.print_log()
         ```
         
         Moreover, you can check the usage status of the API key:
         
         ```py
```

### Comparing `openai_api_call-0.3.7/README.md` & `openai_api_call-0.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,17 @@
 # fake response
 chat.user("What's your name?")
 chat.assistant("My name is GPT-3.5.")
 
 # get the last result
 print(chat[-1])
 
+# save chat history
+chat.save("chat_history.log", mode="w") # default to "a"
+
 # print chat history
 chat.print_log()
 ```
 
 Moreover, you can check the usage status of the API key:
 
 ```py
```

### Comparing `openai_api_call-0.3.7/openai_api_call/__init__.py` & `openai_api_call-0.3.8/openai_api_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.7'
+__version__ = '0.3.8'
 
 import os
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
```

### Comparing `openai_api_call-0.3.7/openai_api_call/chattool.py` & `openai_api_call-0.3.8/openai_api_call/chattool.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import List, Dict, Union
 import openai_api_call
 from .response import Resp
 from .request import chat_completion, usage_status
 import signal, time, random
 import datetime
+import json
 
 # timeout handler
 def handler(signum, frame):
     raise Exception("API call timed out!")
 
 class Chat():
     def __init__( self
@@ -138,19 +139,20 @@
         Args:
             recent (int, optional): number of the usage of recent days. Defaults to 10.
             duration (int, optional): duration of the usage. Defaults to 99.
         """
         storage, usage, rem, recent_usage = self.get_usage_status(recent=recent, duration=duration)
         print(f"Total account: {storage:.4f}$")
         print(f"Total usage: {usage:.4f}$")
-        print(f"Total remaining: {storage-usage:.4f}$")
+        print(f"Total remaining: {rem:.4f}$")
         for date, cost in recent_usage.items():
             print(f"{date}: {cost:.4f}$")
 
     def add(self, role:str, msg:str):
+        """Add a message to the chat log"""
         assert role in ['user', 'assistant', 'system'], "role should be 'user', 'assistant' or 'system'"
         self._chat_log.append({"role": role, "content": msg})
         return self
 
     def user(self, msg:str):
         """User message"""
         return self.add('user', msg)
@@ -165,17 +167,33 @@
     
     def clear(self):
         """Clear the chat log"""
         self._chat_log = []
     
     def copy(self):
         """Copy the chat log"""
-        return Chat(self._chat_log.copy())
-    
+        return Chat(self._chat_log)
+
+    def save(self, path:str, mode:str='a', end:str='\n'):
+        """
+        Save the chat log to a file
+
+        Args:
+            path (str): path to the file
+            mode (str, optional): mode to open the file. Defaults to 'a'.
+            end (str, optional): end of each line. Defaults to '\n'.
+        """
+        assert mode in ['a', 'w'], "mode should be 'a' or 'w'"
+        data = self.chat_log
+        with open(path, mode, encoding='utf-8') as f:
+            f.write(json.dumps(data) + end)
+        return True
+        
     def print_log(self, sep: Union[str, None]=None):
+        """Print the chat log"""
         if sep is None:
             sep = '\n' + '-'*15 + '\n'
         for d in self._chat_log:
             print(sep, d['role'], sep, d['content'])
     
     @property
     def chat_log(self):
```

### Comparing `openai_api_call-0.3.7/openai_api_call/proxy.py` & `openai_api_call-0.3.8/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.7/openai_api_call/request.py` & `openai_api_call-0.3.8/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.7/openai_api_call/response.py` & `openai_api_call-0.3.8/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.7/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.3.8/openai_api_call.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.7
+Version: 0.3.8
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -130,14 +130,17 @@
         # fake response
         chat.user("What's your name?")
         chat.assistant("My name is GPT-3.5.")
         
         # get the last result
         print(chat[-1])
         
+        # save chat history
+        chat.save("chat_history.log", mode="w") # default to "a"
+        
         # print chat history
         chat.print_log()
         ```
         
         Moreover, you can check the usage status of the API key:
         
         ```py
```

### Comparing `openai_api_call-0.3.7/setup.py` & `openai_api_call-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.7'
+VERSION = '0.3.8'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

