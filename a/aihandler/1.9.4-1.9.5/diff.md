# Comparing `tmp/aihandler-1.9.4.tar.gz` & `tmp/aihandler-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.4.tar", last modified: Sun Apr 16 19:58:39 2023, max compression
+gzip compressed data, was "aihandler-1.9.5.tar", last modified: Mon Apr 17 00:49:33 2023, max compression
```

## Comparing `aihandler-1.9.4.tar` & `aihandler-1.9.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:58:39.695188 aihandler-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 19:58:28.000000 aihandler-1.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 19:58:39.695188 aihandler-1.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-16 19:58:28.000000 aihandler-1.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:58:39.695188 aihandler-1.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-16 19:58:28.000000 aihandler-1.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:58:39.691188 aihandler-1.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:58:39.691188 aihandler-1.9.4/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    53693 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-16 19:58:28.000000 aihandler-1.9.4/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:58:39.695188 aihandler-1.9.4/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 19:58:39.000000 aihandler-1.9.4/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 19:58:39.000000 aihandler-1.9.4/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:58:39.000000 aihandler-1.9.4/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-16 19:58:39.000000 aihandler-1.9.4/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 19:58:39.000000 aihandler-1.9.4/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:33.651667 aihandler-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 00:49:19.000000 aihandler-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-17 00:49:33.651667 aihandler-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 00:49:19.000000 aihandler-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 00:49:33.651667 aihandler-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 00:49:19.000000 aihandler-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:33.647667 aihandler-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:33.651667 aihandler-1.9.5/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53693 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-17 00:49:19.000000 aihandler-1.9.5/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:33.651667 aihandler-1.9.5/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-17 00:49:33.000000 aihandler-1.9.5/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 00:49:33.000000 aihandler-1.9.5/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:49:33.000000 aihandler-1.9.5/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-17 00:49:33.000000 aihandler-1.9.5/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 00:49:33.000000 aihandler-1.9.5/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.4/LICENSE` & `aihandler-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/PKG-INFO` & `aihandler-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.4
+Version: 1.9.5
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.4/README.md` & `aihandler-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/setup.py` & `aihandler-1.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # "torch==2.0.0",
     # "torchvision==0.15.1",
     # "torchaudio==2.0.1",
     # "bitsandbytes==0.38.0",
     "einops==0.6.0",
     "ninja==1.11.1",
     "JIT==0.2.7",
-    "triton==2.0.0",
+    #"triton==2.0.0",
     "tqdm==4.65.0",
     "xformers==0.0.18",
     "omegaconf==2.3.0",
     "accelerate==0.18.0",
     "controlnet_aux==0.0.1",
     "huggingface-hub==0.13.3",
     "numpy==1.23.5",
@@ -47,15 +47,15 @@
     "sympy==1.11.1",
     "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.4",
+    version="1.9.5",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.4/src/aihandler/base_runner.py` & `aihandler-1.9.5/src/aihandler/base_runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/controlnet_utils.py` & `aihandler-1.9.5/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/database.py` & `aihandler-1.9.5/src/aihandler/database.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/llmrunner.py` & `aihandler-1.9.5/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/logger.py` & `aihandler-1.9.5/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/offline_client.py` & `aihandler-1.9.5/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.5/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/qtvar.py` & `aihandler-1.9.5/src/aihandler/qtvar.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/runner.py` & `aihandler-1.9.5/src/aihandler/runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/settings.py` & `aihandler-1.9.5/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/settings_manager.py` & `aihandler-1.9.5/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/socket_server.py` & `aihandler-1.9.5/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler/util.py` & `aihandler-1.9.5/src/aihandler/util.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.5/src/aihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.4
+Version: 1.9.5
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.4/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.5/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.4/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.5/src/aihandler.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 einops==0.6.0
 ninja==1.11.1
 JIT==0.2.7
-triton==2.0.0
 tqdm==4.65.0
 xformers==0.0.18
 omegaconf==2.3.0
 accelerate==0.18.0
 controlnet_aux==0.0.1
 huggingface-hub==0.13.3
 numpy==1.23.5
```

