# Comparing `tmp/streamlit-chat-animated-0.0.2.8.tar.gz` & `tmp/streamlit-chat-animated-0.0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-animated-0.0.2.8.tar", last modified: Thu Apr 13 04:48:48 2023, max compression
+gzip compressed data, was "streamlit-chat-animated-0.0.2.9.tar", last modified: Mon Apr 17 05:13:29 2023, max compression
```

## Comparing `streamlit-chat-animated-0.0.2.8.tar` & `streamlit-chat-animated-0.0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:48.002704 streamlit-chat-animated-0.0.2.8/
--rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.2.8/LICENSE
--rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.2.8/MANIFEST.in
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-13 04:48:48.002416 streamlit-chat-animated-0.0.2.8/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.2.8/README.md
--rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-13 04:48:48.002806 streamlit-chat-animated-0.0.2.8/setup.cfg
--rw-r--r--   0 systemd    (501) staff       (20)      945 2023-04-13 04:45:10.000000 streamlit-chat-animated-0.0.2.8/setup.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:47.992174 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/
--rw-r--r--   0 systemd    (501) staff       (20)     7053 2023-04-13 04:42:49.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/__init__.py
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:47.990124 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:47.996821 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/
--rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/asset-manifest.json
--rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-13 04:44:03.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/bootstrap.min.css
--rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-13 04:44:03.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/index.html
--rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/precache-manifest.3b0a591d4a4841e4c5b66ac197cf38fa.js
--rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/service-worker.js
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:47.990373 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:48.001992 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/
--rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
--rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     3497 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js
--rw-r--r--   0 systemd    (501) staff       (20)    10331 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js.map
--rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-13 04:44:12.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-13 04:48:47.993607 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/
--rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-13 04:48:47.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/PKG-INFO
--rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-13 04:48:47.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/SOURCES.txt
--rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-13 04:48:47.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/dependency_links.txt
--rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-13 04:48:47.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/requires.txt
--rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-13 04:48:47.000000 streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/top_level.txt
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.425569 streamlit-chat-animated-0.0.2.9/
+-rw-r--r--   0 systemd    (501) staff       (20)     1064 2023-04-05 09:19:37.000000 streamlit-chat-animated-0.0.2.9/LICENSE
+-rw-r--r--   0 systemd    (501) staff       (20)       59 2023-04-05 18:23:33.000000 streamlit-chat-animated-0.0.2.9/MANIFEST.in
+-rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-17 05:13:29.425282 streamlit-chat-animated-0.0.2.9/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)      729 2023-04-05 21:42:26.000000 streamlit-chat-animated-0.0.2.9/README.md
+-rw-r--r--   0 systemd    (501) staff       (20)       38 2023-04-17 05:13:29.425661 streamlit-chat-animated-0.0.2.9/setup.cfg
+-rw-r--r--   0 systemd    (501) staff       (20)      945 2023-04-17 05:12:05.000000 streamlit-chat-animated-0.0.2.9/setup.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.415865 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/
+-rw-r--r--   0 systemd    (501) staff       (20)     7120 2023-04-17 05:11:57.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/__init__.py
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.413543 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.420287 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/
+-rw-r--r--   0 systemd    (501) staff       (20)      859 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/asset-manifest.json
+-rw-r--r--   0 systemd    (501) staff       (20)   197459 2023-04-17 05:12:58.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/bootstrap.min.css
+-rw-r--r--   0 systemd    (501) staff       (20)   646432 2023-04-17 05:12:58.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 systemd    (501) staff       (20)     2101 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/index.html
+-rw-r--r--   0 systemd    (501) staff       (20)      564 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/precache-manifest.8824ed4ecf5825cb344cf9d35e20ccfa.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1183 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/service-worker.js
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.413842 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.424877 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/
+-rw-r--r--   0 systemd    (501) staff       (20)   490881 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)     1653 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
+-rw-r--r--   0 systemd    (501) staff       (20)  1704293 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     3559 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js
+-rw-r--r--   0 systemd    (501) staff       (20)    10083 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js.map
+-rw-r--r--   0 systemd    (501) staff       (20)     1598 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 systemd    (501) staff       (20)     8317 2023-04-17 05:13:03.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 systemd    (501) staff       (20)        0 2023-04-17 05:13:29.417354 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/
+-rw-r--r--   0 systemd    (501) staff       (20)     1261 2023-04-17 05:13:29.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/PKG-INFO
+-rw-r--r--   0 systemd    (501) staff       (20)     1208 2023-04-17 05:13:29.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/SOURCES.txt
+-rw-r--r--   0 systemd    (501) staff       (20)        1 2023-04-17 05:13:29.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/dependency_links.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       16 2023-04-17 05:13:29.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/requires.txt
+-rw-r--r--   0 systemd    (501) staff       (20)       24 2023-04-17 05:13:29.000000 streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/top_level.txt
```

### Comparing `streamlit-chat-animated-0.0.2.8/LICENSE` & `streamlit-chat-animated-0.0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/PKG-INFO` & `streamlit-chat-animated-0.0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.2.8
+Version: 0.0.2.9
 Summary: A streamlit component, to make chatbots with animated text
 Home-page: UNKNOWN
 Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.2.8/README.md` & `streamlit-chat-animated-0.0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/setup.py` & `streamlit-chat-animated-0.0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-animated",
-    version="0.0.2.8",
+    version="0.0.2.9",
     author="Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley",
     author_email="darin.j.manley@gmail.com",
     description="A streamlit component, to make chatbots with animated text",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/__init__.py` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import streamlit.components.v1 as components
-import os
+import os, random, time
 from typing import Optional, Union
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
@@ -53,53 +53,50 @@
     "shapes",
     "thumbs",
 ]
 
 def message(message: str, 
             is_user: Optional[bool] = False, 
             animated: Optional[bool] = False,
+            key: Optional[str] = None 
             ):
     """
     Creates a new instance of streamlit-chat component
 
     Parameters
     ----------
     message: str
         The message to be displayed in the component
     is_user: bool 
         if the sender of the message is user, if `True` will align the 
         message to right, default is False.
-    avatar_style: Literal or None
+    avatar_style: Literal or False
         The style for the avatar of the sender of message, default is bottts
         for not user, and pixel-art-neutral for user.
         st-chat uses https://www.dicebear.com/styles for the avatar
     seed: int or str
         The seed for choosing the avatar to be used, default is 42.
-    key: str or None
+    key: str or False
         An optional key that uniquely identifies this component. If this is
-        None, and the component's arguments are changed, the component will
+     False, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
 
-    Returns: None
+    Returns: False
     """
 
-    for index, mess in enumerate(message):
-            if index == len(message)-1:
-                 mess['animated'] = False
-            else:
-                 mess['animated'] = True
 
-            _streamlit_chat(message=mess['message'], isUser=mess['isUser'], animated=mess['animated'])
+
+    _streamlit_chat(message=str(mess['message']).replace("\n", ""), isUser=mess['isUser'], animated=mess['animated'])
 
 
 if not _RELEASE:
     import streamlit as st  
     # testing
     long_message = """A chatbot or chatterbot is a software application used to conduct an on-line chat conversation via text or text-to-speech, in lieu of providing direct contact with a live human agent. 
-    Designed to convincingly simulate the way a human would behave as a conversational partner, chatbot systems 
+    Designed to convincingly simulate the way a human would behave as a conversational partner, chatbot systems. 
     """
     longer_message = """Where does it come from?
 Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. Richard McClintock,
  a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word 
  in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by
    Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes
  from a line in section 1.10.32. The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus
@@ -114,24 +111,19 @@
  a Latin professor at Hampden-Sydney College in Virginia, looked up one of the more obscure Latin words, consectetur, from a Lorem Ipsum passage, and going through the cites of the word 
  in classical literature, discovered the undoubtable source. Lorem Ipsum comes from sections 1.10.32 and 1.10.33 of "de Finibus Bonorum et Malorum" (The Extremes of Good and Evil) by
    Cicero, written in 45 BC. This book is a treatise on the theory of ethics, very popular during the Renaissance. The first line of Lorem Ipsum, "Lorem ipsum dolor sit amet..", comes
  from a line in section 1.10.32. The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested. Sections 1.10.32 and 1.10.33 from "de Finibus
    Bonorum et Malorum" by Cicero are also reproduced in their exact original form, accompanied by English versions from the 1914 translation by H. Rackham.
     """
 
-
-    user, bot = [],[]
-    messages = [{'message':"Hello", 'isUser':True, 'animated': None}, 
-                {'message':"Hi", 'isUser': False, 'animated': None}, 
-                {'message':"How are you?", 'isUser':True, 'animated': None},
-                {'message':"I'm great!, and you", 'isUser': False, 'animated': None}, 
-                {'message':"I'm good, thanks!", 'isUser':True, 'animated': None},
-                {'message':"Give me a history lesson", 'isUser':True, 'animated': None},
-                {'message':long_message, 'isUser':False, 'animated': None}
+    messages = [{'message':"Hello", 'isUser':True, 'animated': False, 'key': time.time() + random.randint(1,100)}, 
+                {'message':"Hi", 'isUser': False, 'animated': False, 'key': time.time() + random.randint(1,100)}, 
+                {'message':"How are you?", 'isUser':True, 'animated': False, 'key': time.time() + random.randint(1,100)},
+                {'message':"I'm great!, and you", 'isUser': False, 'animated': False, 'key': time.time() + random.randint(1,100)}, 
+                {'message':"I'm good, thanks!", 'isUser':True, 'animated': False, 'key': time.time() + random.randint(1,100)},
+                {'message':"Give me a history lesson", 'isUser':True, 'animated': False, 'key': time.time() + random.randint(1,100)},
+                {'message':long_message, 'isUser':False, 'animated': False, 'key': time.time() + random.randint(1,100)}
                 ]
     for index, mess in enumerate(messages):
-            if index == len(messages)-1:
-                 mess['animated'] = False
-            else:
-                 mess['animated'] = True
-            message(mess['message'], is_user=mess['isUser'], animated=mess['animated'])
+            
+            message(mess['message'], is_user=mess['isUser'], animated=mess['animated'], key=mess['key'])
     st.text_input("Message:")
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/bootstrap.min.css` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/bootstrap.min.css.map` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/index.html` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.c8026899.chunk.js"></script><script src="./static/js/main.073104d6.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.c8026899.chunk.js"></script><script src="./static/js/main.7a3454f9.chunk.js"></script></body></html>
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/precache-manifest.3b0a591d4a4841e4c5b66ac197cf38fa.js` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/precache-manifest.8824ed4ecf5825cb344cf9d35e20ccfa.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "14a51ce8775419601ea0a7b8752416d4",
+    "revision": "cd8354f238ebd2cf4e186c4b2065f123",
     "url": "./index.html"
 }, {
     "revision": "8bc589e1d7b1ffa912d7",
     "url": "./static/js/2.c8026899.chunk.js"
 }, {
     "revision": "3fc7fb5bfeeec1534560a2c962e360a7",
     "url": "./static/js/2.c8026899.chunk.js.LICENSE.txt"
 }, {
-    "revision": "0cb9268843634ebdf5b1",
-    "url": "./static/js/main.073104d6.chunk.js"
+    "revision": "ece8e983825a9275cdbc",
+    "url": "./static/js/main.7a3454f9.chunk.js"
 }, {
     "revision": "7c26bca7e16783d14d15",
     "url": "./static/js/runtime-main.11ec9aca.js"
 }]);
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/service-worker.js` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/service-worker.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.3b0a591d4a4841e4c5b66ac197cf38fa.js"
+    "./precache-manifest.8824ed4ecf5825cb344cf9d35e20ccfa.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -7,36 +7,36 @@
             "use strict";
             a.r(t);
             var r, n, i, c, o = a(5),
                 s = a.n(o),
                 l = a(30),
                 d = a.n(l),
                 u = a(0),
-                m = a(1),
-                p = a(2),
+                p = a(1),
+                m = a(2),
                 g = a(3),
                 h = a(14),
                 b = a(15),
                 f = a(22),
-                x = a(7),
-                v = a(12),
+                v = a(7),
+                x = a(12),
                 j = function(e) {
                     var t = e.text,
                         a = e.onComplete,
                         r = e.onHeightChange,
                         n = e.args,
                         i = Object(o.useState)(""),
-                        c = Object(x.a)(i, 2),
+                        c = Object(v.a)(i, 2),
                         l = c[0],
                         d = c[1],
                         u = Object(o.useRef)(null),
-                        m = Object(o.useState)(!1),
-                        p = Object(x.a)(m, 2),
-                        g = p[0],
-                        h = p[1];
+                        p = Object(o.useState)(!1),
+                        m = Object(v.a)(p, 2),
+                        g = m[0],
+                        h = m[1];
                     return Object(o.useEffect)((function() {
                         if (!g) {
                             var e = 0,
                                 n = setInterval((function() {
                                     if (e < t.length) {
                                         if (d((function(a) {
                                                 return a + t[e]
@@ -54,120 +54,122 @@
                     }), [t, a, r, g]), s.a.createElement("div", {
                         style: {
                             background: n.theme.secondaryBackgroundColor,
                             border: "1px solid transparent",
                             borderRadius: "10px",
                             padding: "10px 14px",
                             margin: "5px 20px",
-                            maxWidth: "70%",
+                            maxWidth: "80%",
                             fontSize: "1rem",
-                            overflow: "scroll",
                             flex: 1,
-                            whiteSpace: "pre-line",
-                            flexDirection: "column",
                             display: "flex"
                         },
                         ref: u
                     }, l)
                 },
                 O = function(e) {
                     var t = e.args,
                         a = t.isUser,
                         l = t.message,
                         d = t.animated,
-                        u = Object(o.useState)(!1),
-                        m = Object(x.a)(u, 2),
-                        p = m[0],
-                        g = m[1],
+                        u = (t.key, Object(o.useState)(!1)),
+                        p = Object(v.a)(u, 2),
+                        m = p[0],
+                        g = p[1],
                         O = Object(o.useRef)(0),
                         y = "";
                     y = a ? "https://api.dicebear.com/6.x/shapes/svg?backgroundType=gradientLinear,solid" : "https://api.dicebear.com/6.x/avataaars/svg?seed=Felix&facialHair=beardMajestic&facialHairColor=2c1b18&eyes=happy&hairColor=4a312c&skinColor=d08b5b&style=circle&clothing=shirtVNeck&clothesColor=ffffff&top=curvy";
                     var k = Object(b.a)(j)({
                             background: t.theme.secondaryBackgroundColor
                         }),
                         E = b.a.img({
                             border: "1px solid transparent",
                             borderRadius: "50%",
                             height: "5rem",
                             width: "5rem",
                             margin: 0
                         }, (function(e) {
-                            return e.isUser ? Object(v.a)(r || (r = Object(f.a)(["\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        "]))) : Object(v.a)(n || (n = Object(f.a)([""])))
+                            return e.isUser ? Object(x.a)(r || (r = Object(f.a)(["\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        "]))) : Object(x.a)(n || (n = Object(f.a)([""])))
                         })),
-                        w = b.a.div({
+                        C = b.a.div({
                             display: "inline-block",
                             background: t.theme.secondaryBackgroundColor,
                             border: "1px solid transparent",
                             borderRadius: "10px",
                             padding: "10px 14px",
                             margin: "5px 20px",
                             height: "auto",
                             maxWidth: "70%",
                             whiteSpace: "pre-line"
                         }),
-                        C = b.a.div({
+                        w = b.a.div({
                             display: "flex",
                             flex: 1,
                             maxWidth: "100vw",
                             height: "auto",
                             overflow: "auto"
                         }, (function(e) {
-                            return e.isUser ? Object(v.a)(i || (i = Object(f.a)(["\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      "]))) : Object(v.a)(c || (c = Object(f.a)([""])))
+                            return e.isUser ? Object(x.a)(i || (i = Object(f.a)(["\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      "]))) : Object(x.a)(c || (c = Object(f.a)([""])))
                         }));
                     return s.a.createElement("div", {
                         style: {
                             height: "".concat(O.current, "px")
                         }
-                    }, s.a.createElement(C, {
+                    }, s.a.createElement(w, {
                         isUser: a
                     }, s.a.createElement(E, {
                         isUser: a,
                         src: y,
                         alt: "profile",
                         draggable: "false"
-                    }), a || d || p ? s.a.createElement(w, null, l) : s.a.createElement("div", null, s.a.createElement(k, {
+                    }), a || d || m ? s.a.createElement(C, null, l) : s.a.createElement("div", null, s.a.createElement(k, {
                         text: l,
                         onComplete: function() {
-                            g(!0), console.log(p), t.animated = !0
+                            g(!0), t.animated = !0
                         },
                         onHeightChange: function(e) {
                             O.current = e, e < 80 ? h.a.setFrameHeight(80) : h.a.setFrameHeight(e)
                         },
                         args: t
                     }))))
                 },
                 y = function(e) {
-                    Object(p.a)(a, e);
+                    Object(m.a)(a, e);
                     var t = Object(g.a)(a);
 
-                    function a(e) {
-                        var r;
-                        return Object(m.a)(this, a), (r = t.call(this, e)).render = function() {
+                    function a() {
+                        var e;
+                        Object(p.a)(this, a);
+                        for (var r = arguments.length, n = new Array(r), i = 0; i < r; i++) n[i] = arguments[i];
+                        return (e = t.call.apply(t, [this].concat(n))).render = function() {
                             h.a.setFrameHeight(window.innerHeight);
-                            var e = r.props.args,
-                                t = e.isUser,
-                                a = e.message,
-                                n = e.animated,
-                                i = r.props.theme;
-                            if (!i) return s.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
-                            var c = Object(b.a)(O)({});
-                            return s.a.createElement(c, {
+                            var t = e.props.args,
+                                a = t.isUser,
+                                r = t.message,
+                                n = t.animated,
+                                i = t.key;
+                            console.log(e.props.args);
+                            var c = e.props.theme;
+                            if (!c) return s.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
+                            var o = Object(b.a)(O)({});
+                            return s.a.createElement(o, {
                                 args: {
-                                    isUser: t,
-                                    message: a,
-                                    theme: i,
-                                    animated: n
+                                    isUser: a,
+                                    message: r,
+                                    theme: c,
+                                    animated: n,
+                                    key: i
                                 }
                             })
-                        }, r
+                        }, e
                     }
                     return Object(u.a)(a)
                 }(h.b),
                 k = Object(h.c)(y);
             d.a.render(s.a.createElement(s.a.StrictMode, null, s.a.createElement(k, null)), document.getElementById("root"))
         }
     },
     [
         [31, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.073104d6.chunk.js.map
+//# sourceMappingURL=main.7a3454f9.chunk.js.map
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js.map` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7867608581894296%*

 * *Differences: {"'file'": "'static/js/main.7a3454f9.chunk.js'",*

 * * "'mappings'": "'wSA2DeA,EAlDmC,SAAC,GAAgD,IAA9CC,EAA6C,EAA7CA,KAAMC,EAAuC,EAAvCA,WAAYC,EAA2B,EAA3BA,eAAgBC,EAAW,EAAXA,KACrF,EAAsCC,mBAAS,IAA/C,mBAAOC,EAAP,KAAoBC,EAApB,KACMC,EAAUC,iBAAuB,MACvC,EAAkCJ,oBAAS,GAA3C,mBAAOK,EAAP,KAAkBC,EAAlB,KA2BA,OAzBAC,qBAAU,WACR,IAAIF,EAAJ,CAEA,IAAIG,EAAQ,EAENC,EAAWC,aAAY,WAC3B,GAAIF,EAAQZ,EAAKe,OAAQ,CAGvB,GAFAT,GAAe,SAACU,GAAD,OAAcA,EAAWhB,EAAKY,MAEzCL,EAAQU,QAAS,CACnB,IAAQC,EAAWX,EAAQU,QAAQE,wBAA3BD,OACRhB,EAAegB,GAGjBN,SAEA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.073104d6.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.7a3454f9.chunk.js",
+    "mappings": "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",
     "names": [
         "AnimatedText",
         "text",
         "onComplete",
         "onHeightChange",
         "args",
         "useState",
@@ -30,48 +30,48 @@
         "secondaryBackgroundColor",
         "border",
         "borderRadius",
         "padding",
         "margin",
         "maxWidth",
         "fontSize",
-        "overflow",
         "flex",
-        "whiteSpace",
-        "flexDirection",
         "display",
         "ref",
         "ChatContainer",
         "isUser",
         "message",
         "animated",
+        "key",
         "isAnimationCompleted",
         "setAnimationCompleted",
         "containerHeightRef",
         "avatarUrl",
         "TypingStyle",
         "styled",
         "Avatar",
         "img",
         "width",
         "props",
         "css",
         "Message",
         "div",
+        "whiteSpace",
         "Chat",
+        "overflow",
         "src",
         "alt",
         "draggable",
-        "console",
-        "log",
         "Streamlit",
         "setFrameHeight",
         "render",
         "window",
         "innerHeight",
+        "console",
+        "log",
         "StyledChatContainer",
         "StreamlitComponentBase",
         "withStreamlitConnection",
         "ReactDOM",
         "StrictMode",
         "document",
         "getElementById"
@@ -80,14 +80,14 @@
     "sources": [
         "AnimatedText.tsx",
         "chatContainer.tsx",
         "stChat.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import React, { useState, useEffect, useRef } from 'react';\n\ninterface AnimatedTextProps {\n    text: string;\n    onComplete: () => void;\n    onHeightChange: (height: number) => void;\n    args: any;\n}\n\nconst AnimatedText: React.FC<AnimatedTextProps> = ({ text, onComplete, onHeightChange, args }) => {\n  const [visibleText, setVisibleText] = useState('');\n  const textRef = useRef<HTMLDivElement>(null);\n  const [completed, setCompleted] = useState(false);\n\n  useEffect(() => {\n    if (completed) return;\n\n    let index = 0;\n\n    const interval = setInterval(() => {\n      if (index < text.length) {\n        setVisibleText((prevText) => prevText + text[index]);\n\n        if (textRef.current) {\n          const { height } = textRef.current.getBoundingClientRect();\n          onHeightChange(height);\n        }\n\n        index++;\n      } else {\n        clearInterval(interval);\n        onComplete();\n        setCompleted(true);\n      }\n    }, 10); // Adjust the typing speed here\n\n    return () => clearInterval(interval);\n  }, [text, onComplete, onHeightChange, completed]);\n\n  return (\n    <div\n      style={{\n        background: args.theme.secondaryBackgroundColor,\n        border: '1px solid transparent',\n        borderRadius: '10px',\n        padding: '10px 14px',\n        margin: '5px 20px',\n        maxWidth: '70%',\n        fontSize: '1rem',\n        overflow: 'scroll',\n        flex: 1,\n        whiteSpace: 'pre-line',\n        flexDirection: 'column',\n        display: 'flex',\n      }}\n      ref={textRef}\n    >\n      {visibleText}\n    </div>\n  );\n};\n\nexport default AnimatedText;\n",
-        "import React, { useRef, useState, useEffect } from \"react\";\nimport styled from \"@emotion/styled\";\nimport { css } from \"@emotion/react\";\nimport AnimatedText from './AnimatedText'; // Assuming both files are in the same folder\nimport { Streamlit } from \"streamlit-component-lib\";\n\n\n// import Typing, { TypingProps } from 'react-typing-animation';\n\ninterface ChatProps {\n  args: {\n    isUser: boolean;\n    message: string;\n    animated: boolean;\n    theme: any;\n  \n  };\n}\n\ninterface AvatarProps {\n  isUser: boolean;\n}\n\ninterface ChatContainerProps {\n  isUser: boolean;\n}\n\nconst ChatContainer: React.FC<ChatProps> = ({ args }) => {\n  const { isUser, message, animated } = args;\n  const [isAnimationCompleted, setAnimationCompleted] = useState(false);\n  const containerHeightRef = useRef(0);\n\n  let avatarUrl = \"\";\n  if (!isUser) {\n    avatarUrl = `https://api.dicebear.com/6.x/avataaars/svg?seed=Felix&facialHair=beardMajestic&facialHairColor=2c1b18&eyes=happy&hairColor=4a312c&skinColor=d08b5b&style=circle&clothing=shirtVNeck&clothesColor=ffffff&top=curvy`;\n  } else {\n    avatarUrl = `https://api.dicebear.com/6.x/shapes/svg?backgroundType=gradientLinear,solid`;\n  }\n\n  // Styles for the Typing component\n  const TypingStyle = styled(AnimatedText)({\n    background: args.theme.secondaryBackgroundColor,\n   \n    // etc.\n  });\n\n  // styles for the avatar image\n  const Avatar = styled.img<AvatarProps>(\n    {\n      border: `1px solid transparent`,\n      borderRadius: \"50%\",\n      height: \"5rem\",\n      width: \"5rem\",\n      margin: 0,\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        `;\n      }\n      return css``;\n    }\n  );\n\n  // styles for the message box\n  const Message = styled.div({\n    display: \"inline-block\",\n    background: args.theme.secondaryBackgroundColor,\n    border: \"1px solid transparent\",\n    borderRadius: \"10px\",\n    padding: \"10px 14px\",\n    margin: \"5px 20px\",\n    height: \"auto\",\n    maxWidth: \"70%\",\n    whiteSpace: \"pre-line\",\n  });\n\n  // styles for the container\n  const Chat = styled.div<ChatContainerProps>(\n    {\n      display: \"flex\",\n      flex: 1,\n      maxWidth: \"100vw\",\n      height: \"auto\",\n      overflow: \"auto\",\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      `;\n      }\n      return css``;\n    }\n  );\n\n  const handleAnimationComplete = () => {\n    setAnimationCompleted(true);\n    console.log(isAnimationCompleted)\n    args.animated=true\n    //Streamlit.setComponentValue(args); // Send the value back to Streamlit\n  };\n\n  const updateHeight = (height: number) => {\n    containerHeightRef.current = height;\n    //console.log(containerHeightRef.current)\n    if (height < 80){\n      Streamlit.setFrameHeight(80);\n    }else{\n      Streamlit.setFrameHeight(height);\n    }\n      \n\n  };\n\n\n\n  return (\n    <div style={{ height: `${containerHeightRef.current}px` }}>\n      <Chat isUser={isUser}>\n        <Avatar isUser={isUser} src={avatarUrl} alt=\"profile\" draggable=\"false\" />\n        {!isUser && !animated && !isAnimationCompleted? (\n          <div>\n            <TypingStyle\n              text={message}\n              onComplete={handleAnimationComplete}\n              onHeightChange={updateHeight} // Pass the handler here\n              args={args}\n            />\n          </div>\n        ) : (\n          <Message>{message}</Message>\n        )}\n      </Chat>\n    </div>\n  );\n}\n\nexport default ChatContainer",
-        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode, useEffect, useState } from \"react\"\nimport styled from \"@emotion/styled\";\nimport ChatContainer from './chatContainer'\n\nclass Chat extends StreamlitComponentBase {\n\n  constructor(props:any) {\n    super(props);\n\n  }\n\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, message, animated } = this.props.args;\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    // Styles for the Typing component\n  const StyledChatContainer = styled(ChatContainer)({\n  });\n    return (\n        <StyledChatContainer args={{ isUser: isUser, message: message, theme: theme, animated: animated}}/>\n\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
+        "import React, { useState, useEffect, useRef } from 'react';\n\ninterface AnimatedTextProps {\n    text: string;\n    onComplete: () => void;\n    onHeightChange: (height: number) => void;\n    args: any;\n}\n\nconst AnimatedText: React.FC<AnimatedTextProps> = ({ text, onComplete, onHeightChange, args }) => {\n  const [visibleText, setVisibleText] = useState('');\n  const textRef = useRef<HTMLDivElement>(null);\n  const [completed, setCompleted] = useState(false);\n\n  useEffect(() => {\n    if (completed) return;\n\n    let index = 0;\n\n    const interval = setInterval(() => {\n      if (index < text.length) {\n        setVisibleText((prevText) => prevText + text[index]);\n\n        if (textRef.current) {\n          const { height } = textRef.current.getBoundingClientRect();\n          onHeightChange(height);\n        }\n\n        index++;\n      } else {\n        clearInterval(interval);\n        onComplete();\n        setCompleted(true);\n      }\n    }, 10); // Adjust the typing speed here\n\n    return () => clearInterval(interval);\n  }, [text, onComplete, onHeightChange, completed]);\n\n  return (\n    <div\n      style={{\n        background: args.theme.secondaryBackgroundColor,\n        border: '1px solid transparent',\n        borderRadius: '10px',\n        padding: '10px 14px',\n        margin: '5px 20px',\n        maxWidth: '80%',\n        fontSize: '1rem',\n        flex: 1,\n        display: 'flex',\n      }}\n      ref={textRef}\n    >\n      {visibleText}\n    </div>\n  );\n};\n\nexport default AnimatedText;\n",
+        "import React, { useEffect, useRef, useState } from \"react\";\nimport styled from \"@emotion/styled\";\nimport { css } from \"@emotion/react\";\nimport AnimatedText from './AnimatedText'; // Assuming both files are in the same folder\nimport { Streamlit } from \"streamlit-component-lib\";\n\ninterface ChatProps {\n  args: {\n    isUser: boolean;\n    message: string;\n    animated: boolean;\n    key: any;\n    theme: any;\n  \n  };\n}\n\ninterface AvatarProps {\n  isUser: boolean;\n}\n\ninterface ChatContainerProps {\n  isUser: boolean;\n}\n\nconst ChatContainer: React.FC<ChatProps> = ({ args }) => {\n  const { isUser, message, animated, key } = args;\n  const [isAnimationCompleted, setAnimationCompleted] = useState(false);\n  const containerHeightRef = useRef(0);\n\n  // Streamlit.setComponentValue(args); // Send the value back to Streamlit\n \n  \n\n\n  let avatarUrl = \"\";\n  if (!isUser) {\n    avatarUrl = `https://api.dicebear.com/6.x/avataaars/svg?seed=Felix&facialHair=beardMajestic&facialHairColor=2c1b18&eyes=happy&hairColor=4a312c&skinColor=d08b5b&style=circle&clothing=shirtVNeck&clothesColor=ffffff&top=curvy`;\n  } else {\n    avatarUrl = `https://api.dicebear.com/6.x/shapes/svg?backgroundType=gradientLinear,solid`;\n  }\n\n  // Styles for the Typing component\n  const TypingStyle = styled(AnimatedText)({\n    background: args.theme.secondaryBackgroundColor,\n  });\n\n  // styles for the avatar image\n  const Avatar = styled.img<AvatarProps>(\n    {\n      border: `1px solid transparent`,\n      borderRadius: \"50%\",\n      height: \"5rem\",\n      width: \"5rem\",\n      margin: 0,\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n          height: 4rem;\n          width: 4rem;\n          margin: 0;\n        `;\n      }\n      return css``;\n    }\n  );\n\n  // styles for the message box\n  const Message = styled.div({\n    display: \"inline-block\",\n    background: args.theme.secondaryBackgroundColor,\n    border: \"1px solid transparent\",\n    borderRadius: \"10px\",\n    padding: \"10px 14px\",\n    margin: \"5px 20px\",\n    height: \"auto\",\n    maxWidth: \"70%\",\n    whiteSpace: \"pre-line\",\n  });\n\n  // styles for the container\n  const Chat = styled.div<ChatContainerProps>(\n    {\n      display: \"flex\",\n      flex: 1,\n      maxWidth: \"100vw\",\n      height: \"auto\",\n      overflow: \"auto\",\n    },\n    (props: { isUser: boolean }) => {\n      // specific styles\n      if (props.isUser) {\n        return css`\n        flex-direction: row-reverse;\n        & > div {/\n          text-align: right;\n        }\n      `;\n      }\n      return css``;\n    }\n  );\n\n  const handleAnimationComplete = () => {\n    setAnimationCompleted(true);\n    args.animated=true\n  };\n\n  const updateHeight = (height: number) => {\n    containerHeightRef.current = height;\n    //console.log(containerHeightRef.current)\n    if (height < 80){\n      Streamlit.setFrameHeight(80);\n    }else{\n      Streamlit.setFrameHeight(height);\n    }\n      \n\n  };\n\n  return (\n    <div style={{ height: `${containerHeightRef.current}px` }}>\n      <Chat isUser={isUser}>\n        <Avatar isUser={isUser} src={avatarUrl} alt=\"profile\" draggable=\"false\" />\n        {!isUser && !animated && !isAnimationCompleted ? (\n          <div>\n            <TypingStyle\n              text={message}\n              onComplete={handleAnimationComplete}\n              onHeightChange={updateHeight} // Pass the handler here\n              args={args}\n            />\n          </div>\n        ) : (\n          <Message>{message}</Message>\n        )}\n      </Chat>\n    </div>\n  );\n}\n\nexport default ChatContainer",
+        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from \"@emotion/styled\";\nimport ChatContainer from './chatContainer'\n\nclass Chat extends StreamlitComponentBase {\n\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, message, animated, key } = this.props.args;\n    console.log(this.props.args)\n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    // Styles for the Typing component\n  const StyledChatContainer = styled(ChatContainer)({\n  });\n    return (\n        <StyledChatContainer args={{ isUser: isUser, message: message, theme: theme, animated: animated, key: key}}/>\n\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Chat from \"./stChat\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Chat />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/PKG-INFO` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-animated
-Version: 0.0.2.8
+Version: 0.0.2.9
 Summary: A streamlit component, to make chatbots with animated text
 Home-page: UNKNOWN
 Author: Yash Pravin Pawar, Yash Vardhan Kapil, Darin Manley
 Author-email: darin.j.manley@gmail.com
 License: UNKNOWN
 Keywords: chat streamlit streamlit-component animated text
 Platform: UNKNOWN
```

### Comparing `streamlit-chat-animated-0.0.2.8/streamlit_chat_animated.egg-info/SOURCES.txt` & `streamlit-chat-animated-0.0.2.9/streamlit_chat_animated.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 streamlit_chat_animated.egg-info/dependency_links.txt
 streamlit_chat_animated.egg-info/requires.txt
 streamlit_chat_animated.egg-info/top_level.txt
 streamlit_chat_animated/frontend/build/asset-manifest.json
 streamlit_chat_animated/frontend/build/bootstrap.min.css
 streamlit_chat_animated/frontend/build/bootstrap.min.css.map
 streamlit_chat_animated/frontend/build/index.html
-streamlit_chat_animated/frontend/build/precache-manifest.3b0a591d4a4841e4c5b66ac197cf38fa.js
+streamlit_chat_animated/frontend/build/precache-manifest.8824ed4ecf5825cb344cf9d35e20ccfa.js
 streamlit_chat_animated/frontend/build/service-worker.js
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.LICENSE.txt
 streamlit_chat_animated/frontend/build/static/js/2.c8026899.chunk.js.map
-streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js
-streamlit_chat_animated/frontend/build/static/js/main.073104d6.chunk.js.map
+streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js
+streamlit_chat_animated/frontend/build/static/js/main.7a3454f9.chunk.js.map
 streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js
 streamlit_chat_animated/frontend/build/static/js/runtime-main.11ec9aca.js.map
```

