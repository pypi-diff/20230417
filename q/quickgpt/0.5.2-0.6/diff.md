# Comparing `tmp/quickgpt-0.5.2.tar.gz` & `tmp/quickgpt-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickgpt-0.5.2.tar", last modified: Tue Apr  4 20:54:41 2023, max compression
+gzip compressed data, was "quickgpt-0.6.tar", last modified: Mon Apr 17 00:33:44 2023, max compression
```

## Comparing `quickgpt-0.5.2.tar` & `quickgpt-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-04 20:54:41.511991 quickgpt-0.5.2/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4186 2023-04-04 20:54:41.511991 quickgpt-0.5.2/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2859 2023-03-27 22:13:26.000000 quickgpt-0.5.2/README.rst
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-04 20:54:41.511991 quickgpt-0.5.2/bin/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.5.2/bin/quickgpt
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-04 20:54:41.511991 quickgpt-0.5.2/quickgpt/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-02 15:07:51.000000 quickgpt-0.5.2/quickgpt/__init__.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-04 20:54:41.511991 quickgpt-0.5.2/quickgpt/thread/
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     5912 2023-04-02 22:15:01.000000 quickgpt-0.5.2/quickgpt/thread/__init__.py
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      643 2023-03-27 17:04:18.000000 quickgpt-0.5.2/quickgpt/thread/messagetypes.py
--rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)      961 2023-03-27 17:03:57.000000 quickgpt-0.5.2/quickgpt/thread/response.py
-drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-04 20:54:41.511991 quickgpt-0.5.2/quickgpt.egg-info/
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4186 2023-04-04 20:54:41.000000 quickgpt-0.5.2/quickgpt.egg-info/PKG-INFO
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-04 20:54:41.000000 quickgpt-0.5.2/quickgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-04 20:54:41.000000 quickgpt-0.5.2/quickgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-04 20:54:41.000000 quickgpt-0.5.2/quickgpt.egg-info/requires.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-04 20:54:41.000000 quickgpt-0.5.2/quickgpt.egg-info/top_level.txt
--rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-04 20:54:41.511991 quickgpt-0.5.2/setup.cfg
--rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      805 2023-04-02 14:56:14.000000 quickgpt-0.5.2/setup.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4168 2023-04-17 00:33:44.935318 quickgpt-0.6/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     2843 2023-04-04 20:54:41.000000 quickgpt-0.6/README.rst
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/bin/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     3766 2023-03-20 02:38:15.000000 quickgpt-0.6/bin/quickgpt
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     1660 2023-04-02 15:07:51.000000 quickgpt-0.6/quickgpt/__init__.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt/thread/
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)     5932 2023-04-17 00:33:22.000000 quickgpt-0.6/quickgpt/thread/__init__.py
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      643 2023-03-27 17:04:18.000000 quickgpt-0.6/quickgpt/thread/messagetypes.py
+-rwxr--r--   0 benbaptist  (1000) benbaptist  (1000)     2551 2023-04-17 00:27:35.000000 quickgpt-0.6/quickgpt/thread/response.py
+drwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)        0 2023-04-17 00:33:44.935318 quickgpt-0.6/quickgpt.egg-info/
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)     4168 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)      300 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        1 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        7 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/requires.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)        9 2023-04-17 00:33:44.000000 quickgpt-0.6/quickgpt.egg-info/top_level.txt
+-rw-rw-r--   0 benbaptist  (1000) benbaptist  (1000)       38 2023-04-17 00:33:44.935318 quickgpt-0.6/setup.cfg
+-rwxrwxr-x   0 benbaptist  (1000) benbaptist  (1000)      803 2023-04-17 00:20:59.000000 quickgpt-0.6/setup.py
```

### Comparing `quickgpt-0.5.2/PKG-INFO` & `quickgpt-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.5.2
+Version: 0.6
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
@@ -18,16 +18,16 @@
         
         **quickGPT** is a lightweight and easy-to-use Python library that
         provides a simplified interface for working with the new API interface
         of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
         language responses to prompts and questions using state-of-the-art
         language models trained by OpenAI.
         
-        For the record, this README.md was (mostly) generated with ChatGPT.
-        That’s why it’s a little braggy.
+        For the record, this README was (mostly) generated with ChatGPT - hence
+        the braggy tone.
         
         Installation
         ------------
         
         You can install **quickGPT** using pip:
         
         .. code:: sh
```

### Comparing `quickgpt-0.5.2/README.rst` & `quickgpt-0.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 **quickGPT** is a lightweight and easy-to-use Python library that
 provides a simplified interface for working with the new API interface
 of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
 language responses to prompts and questions using state-of-the-art
 language models trained by OpenAI.
 
-For the record, this README.md was (mostly) generated with ChatGPT.
-That’s why it’s a little braggy.
+For the record, this README was (mostly) generated with ChatGPT - hence
+the braggy tone.
 
 Installation
 ------------
 
 You can install **quickGPT** using pip:
 
 .. code:: sh
```

### Comparing `quickgpt-0.5.2/bin/quickgpt` & `quickgpt-0.6/bin/quickgpt`

 * *Files identical despite different names*

### Comparing `quickgpt-0.5.2/quickgpt/__init__.py` & `quickgpt-0.6/quickgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.5.2/quickgpt/thread/__init__.py` & `quickgpt-0.6/quickgpt/thread/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,14 @@
         except TypeError:
             pass
 
         for msg in messages:
             assert type(msg) in (System, Assistant, User, Response, dict), \
                 "Must be of type System, Assistant, User, Response, or dict"
 
-            if type(msg) == Response:
-                msg = Assistant(msg.message)
-
             # Convert a boring old dict message to a pretty object message
             if type(msg) == dict:
                 role = msg["role"]
                 content = msg["content"]
 
                 if role == "system":
                     msg = System(content)
@@ -110,15 +107,16 @@
                 self.thread.insert(insert, msg)
             else:
                 self.thread.append(msg)
 
     def insert(self, index, *messages):
         """ Inserts messages at a given index in the Thread
 
-        Unfinished method?"""
+        This method is currently not implemented.
+        """
 
         self.feed(
             insert=True,
             *messages
         )
 
     @property
@@ -127,15 +125,15 @@
 
         Returns:
             list: JSON-safe list of all messages
         """
 
         return [ msg.obj for msg in self.thread ]
 
-    def run(self, *append_messages, feed=True):
+    def run(self, *append_messages, feed=True, stream=False):
         """ Executes the current Thread and get a response. If ``feed`` is
         True, it will automatically save the response to the Thread.
 
         You can provide *append_messages that will only apply to this run(),
         and won't be permanently stored in the Thread.
 
         Returns:
@@ -145,15 +143,16 @@
         messages = self.messages
         append_messages = [ msg.obj for msg in append_messages ]
 
         for i in range(self.quickgpt.retry_count):
             try:
                 response_obj = openai.ChatCompletion.create(
                     model=self.model,
-                    messages=messages + append_messages
+                    messages=messages + append_messages,
+                    stream=stream
                 )
 
                 break
             except openai.error.RateLimitError as e:
                 if self.quickgpt.retry_count == i - 1:
                     print("Failed after %s tries" % self.quickgpt.retry_count)
                     raise e
@@ -168,16 +167,15 @@
                     }, indent=2)
                 )
 
                 print("Please see failed request encoded as JSON above.")
 
                 raise e
 
-
-        response = Response(response_obj)
+        response = Response(response_obj, stream=stream)
 
         if feed:
             self.feed(response)
 
         return response
 
     def moderate(self, prompt):
@@ -190,10 +188,10 @@
             bool: True if it's flagged as a violation, False if it's safe
         """
 
         response = openai.Moderation.create(
             input=prompt
         )
 
-        output = response["results"][0]
+        output = response["results"][0]["flagged"]
 
         return output
```

### Comparing `quickgpt-0.5.2/quickgpt/thread/messagetypes.py` & `quickgpt-0.6/quickgpt/thread/messagetypes.py`

 * *Files identical despite different names*

### Comparing `quickgpt-0.5.2/quickgpt.egg-info/PKG-INFO` & `quickgpt-0.6/quickgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: quickgpt
-Version: 0.5.2
+Version: 0.6
 Summary: A barebones library to make interacting with OpenAI's ChatGPT API much simpler.
 Home-page: https://github.com/benbaptist/quickgpt
 Author: Ben Baptist
 Author-email: me@benbaptist.com
 License: UNKNOWN
 Description: quickGPT
         ========
@@ -18,16 +18,16 @@
         
         **quickGPT** is a lightweight and easy-to-use Python library that
         provides a simplified interface for working with the new API interface
         of OpenAI’s ChatGPT. With quickGPT, you can easily generate natural
         language responses to prompts and questions using state-of-the-art
         language models trained by OpenAI.
         
-        For the record, this README.md was (mostly) generated with ChatGPT.
-        That’s why it’s a little braggy.
+        For the record, this README was (mostly) generated with ChatGPT - hence
+        the braggy tone.
         
         Installation
         ------------
         
         You can install **quickGPT** using pip:
         
         .. code:: sh
```

### Comparing `quickgpt-0.5.2/setup.py` & `quickgpt-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='quickgpt',
-    version='0.5.2',
+    version='0.6',
     description='A barebones library to make interacting with OpenAI\'s ChatGPT API much simpler.',
     long_description=open("README.rst", "r").read(),
     author='Ben Baptist',
     author_email='me@benbaptist.com',
     url='https://github.com/benbaptist/quickgpt',
     packages=find_packages(),
     scripts=['bin/quickgpt'],
```

