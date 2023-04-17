# Comparing `tmp/quickgpt-0.6.tar.gz` & `tmp/quickgpt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgpt-0.6.tar", last modified: Mon Apr 17 00:33:44 2023, max compression
+gzip compressed data, was "quickgpt-0.6.1.tar", last modified: Mon Apr 17 02:41:32 2023, max compression
```

## Comparing `quickgpt-0.6.tar` & `quickgpt-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4168 2023-04-17 00:33:44.935318 quickgpt-0.6/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2843 2023-04-04 20:54:41.000000 quickgpt-0.6/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/bin/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6/bin/quickgpt
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-02 15:07:51.000000 quickgpt-0.6/quickgpt/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt/thread/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     5932 2023-04-17 00:33:22.000000 quickgpt-0.6/quickgpt/thread/__init__.py
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      643 2023-03-27 17:04:18.000000 quickgpt-0.6/quickgpt/thread/messagetypes.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2551 2023-04-17 00:27:35.000000 quickgpt-0.6/quickgpt/thread/response.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4168 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/top_level.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-17 00:33:44.935318 quickgpt-0.6/setup.cfg
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      803 2023-04-17 00:20:59.000000 quickgpt-0.6/setup.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.166690 quickgpt-0.6.1/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-17 02:41:32.166690 quickgpt-0.6.1/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2993 2023-04-17 02:41:07.000000 quickgpt-0.6.1/README.rst
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/bin/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6.1/bin/quickgpt
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-17 02:41:25.000000 quickgpt-0.6.1/quickgpt/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt/thread/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     5932 2023-04-17 00:33:22.000000 quickgpt-0.6.1/quickgpt/thread/__init__.py
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      643 2023-03-27 17:04:18.000000 quickgpt-0.6.1/quickgpt/thread/messagetypes.py
+-rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2552 2023-04-17 02:40:43.000000 quickgpt-0.6.1/quickgpt/thread/response.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 02:41:32.162690 quickgpt-0.6.1/quickgpt.egg-info/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4352 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/requires.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-17 02:41:32.000000 quickgpt-0.6.1/quickgpt.egg-info/top_level.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-17 02:41:32.166690 quickgpt-0.6.1/setup.cfg
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-04-17 02:41:18.000000 quickgpt-0.6.1/setup.py
```

### Comparing `quickgpt-0.6/PKG-INFO` & `quickgpt-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6
+Version: 0.6.1
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
@@ -21,14 +21,18 @@
         of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
         language responses to prompts and questions using state-of-the-art
         language models trained by OpenAI.
         
         For the record, this README was (mostly) generated with ChatGPT - hence
         the braggy tone.
         
+        Like fine wine and cheddar, this library pairs nicely with the
+        `ElevenLabs <https://github.com/benbaptist/elevenlabs>`__ text-to-speech
+        API library.
+        
         Installation
         ------------
         
         You can install **quickGPT** using pip:
         
         .. code:: sh
```

### Comparing `quickgpt-0.6/README.rst` & `quickgpt-0.6.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
 language responses to prompts and questions using state-of-the-art
 language models trained by OpenAI.
 
 For the record, this README was (mostly) generated with ChatGPT - hence
 the braggy tone.
 
+Like fine wine and cheddar, this library pairs nicely with the
+`ElevenLabs <https://github.com/benbaptist/elevenlabs>`__ text-to-speech
+API library.
+
 Installation
 ------------
 
 You can install **quickGPT** using pip:
 
 .. code:: sh
```

### Comparing `quickgpt-0.6/bin/quickgpt` & `quickgpt-0.6.1/bin/quickgpt`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6/quickgpt/__init__.py` & `quickgpt-0.6.1/quickgpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from quickgpt.thread import Thread
 
-__version__ = "0.5.2"
+__version__ = "0.6.1"
 
 import os
 
 class QuickGPT:
     def __init__(self, api_key=None, retry_count=3):
         """ Main QuickGPT object
```

### Comparing `quickgpt-0.6/quickgpt/thread/__init__.py` & `quickgpt-0.6.1/quickgpt/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6/quickgpt/thread/messagetypes.py` & `quickgpt-0.6.1/quickgpt/thread/messagetypes.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.6/quickgpt/thread/response.py` & `quickgpt-0.6.1/quickgpt/thread/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
             if "role" in delta:
                 self.gathered["choices"][0]["message"]["role"] = delta["role"]
 
             if "content" in delta:
                 segment = delta["content"]
 
-                self.gathered["choices"][0]["message"]["content"] = segment
+                self.gathered["choices"][0]["message"]["content"] += segment
 
                 yield segment
             else:
                 yield ""
 
             self.gathered["choices"][0]["finished_reason"] = \
                 resp["choices"][0]["finish_reason"]
```

### Comparing `quickgpt-0.6/quickgpt.egg-info/PKG-INFO` & `quickgpt-0.6.1/quickgpt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.6
+Version: 0.6.1
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
@@ -21,14 +21,18 @@
         of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
         language responses to prompts and questions using state-of-the-art
         language models trained by OpenAI.
         
         For the record, this README was (mostly) generated with ChatGPT - hence
         the braggy tone.
         
+        Like fine wine and cheddar, this library pairs nicely with the
+        `ElevenLabs <https://github.com/benbaptist/elevenlabs>`__ text-to-speech
+        API library.
+        
         Installation
         ------------
         
         You can install **quickGPT** using pip:
         
         .. code:: sh
```

### Comparing `quickgpt-0.6/setup.py` & `quickgpt-0.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='quickgpt',
-    version='0.6',
+    version='0.6.1',
     description='A barebones library to make interacting with OpenAI\'s ChatGPT API much simpler.',
     long_description=open("README.rst", "r").read(),
     author='Ben Baptist',
     author_email='me@benbaptist.com',
     url='https://github.com/benbaptist/quickgpt',
     packages=find_packages(),
     scripts=['bin/quickgpt'],
```

