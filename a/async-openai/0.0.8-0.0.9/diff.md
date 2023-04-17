# Comparing `tmp/async_openai-0.0.8.tar.gz` & `tmp/async_openai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_openai-0.0.8.tar", last modified: Thu Feb  2 19:51:19 2023, max compression
+gzip compressed data, was "async_openai-0.0.9.tar", last modified: Wed Feb  8 06:26:55 2023, max compression
```

## Comparing `async_openai-0.0.8.tar` & `async_openai-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.075037 async_openai-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-02 19:51:08.000000 async_openai-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-02 19:51:08.000000 async_openai-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-02-02 19:51:19.075037 async_openai-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-02 19:51:08.000000 async_openai-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.071037 async_openai-0.0.8/async_openai/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.075037 async_openai-0.0.8/async_openai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/completions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/schemas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.075037 async_openai-0.0.8/async_openai/types/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    29120 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/types/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.075037 async_openai-0.0.8/async_openai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-02 19:51:08.000000 async_openai-0.0.8/async_openai/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 19:51:19.075037 async_openai-0.0.8/async_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-02-02 19:51:19.000000 async_openai-0.0.8/async_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-02 19:51:19.000000 async_openai-0.0.8/async_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 19:51:19.000000 async_openai-0.0.8/async_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 19:51:19.000000 async_openai-0.0.8/async_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-02 19:51:19.000000 async_openai-0.0.8/async_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 19:51:19.075037 async_openai-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-02-02 19:51:08.000000 async_openai-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.763907 async_openai-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-08 06:26:39.000000 async_openai-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-08 06:26:39.000000 async_openai-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-02-08 06:26:55.763907 async_openai-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-08 06:26:39.000000 async_openai-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.759907 async_openai-0.0.9/async_openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.763907 async_openai-0.0.9/async_openai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/completions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/schemas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.763907 async_openai-0.0.9/async_openai/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29120 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/types/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.763907 async_openai-0.0.9/async_openai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-08 06:26:39.000000 async_openai-0.0.9/async_openai/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 06:26:55.763907 async_openai-0.0.9/async_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-02-08 06:26:55.000000 async_openai-0.0.9/async_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-08 06:26:55.000000 async_openai-0.0.9/async_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 06:26:55.000000 async_openai-0.0.9/async_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-08 06:26:55.000000 async_openai-0.0.9/async_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-08 06:26:55.000000 async_openai-0.0.9/async_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 06:26:55.763907 async_openai-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-02-08 06:26:39.000000 async_openai-0.0.9/setup.py
```

### Comparing `async_openai-0.0.8/LICENSE` & `async_openai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/PKG-INFO` & `async_openai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_openai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Async Python client library for the OpenAI API
 Home-page: https://github.com/GrowthEngineAI/async-openai
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `async_openai-0.0.8/README.md` & `async_openai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/__init__.py` & `async_openai-0.0.9/async_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/client.py` & `async_openai-0.0.9/async_openai/client.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/routes.py` & `async_openai-0.0.9/async_openai/routes.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/schemas/__init__.py` & `async_openai-0.0.9/async_openai/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/schemas/completions.py` & `async_openai-0.0.9/async_openai/schemas/completions.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,20 @@
     presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
     best_of: Optional[int] = 1
     logit_bias: Optional[Dict[str, float]] = None
     user: Optional[str] = None
 
     @validator('model', pre=True, always=True)
-    def validate_model(cls, v) -> OpenAIModel:
+    def validate_model(cls, v, values: Dict[str, Any]) -> OpenAIModel:
         """
         Validate the model
         """
+        if not v and values.get('engine'):
+            v = values.get('engine')
         if isinstance(v, OpenAIModel):
             return v
         if isinstance(v, dict):
             return OpenAIModel(**v)
         return OpenAIModel(value = v, mode = 'completion')
 
     @validator('max_tokens')
```

### Comparing `async_openai-0.0.8/async_openai/schemas/edits.py` & `async_openai-0.0.9/async_openai/schemas/edits.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/schemas/embeddings.py` & `async_openai-0.0.9/async_openai/schemas/embeddings.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/schemas/images.py` & `async_openai-0.0.9/async_openai/schemas/images.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/schemas/models.py` & `async_openai-0.0.9/async_openai/schemas/models.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/__init__.py` & `async_openai-0.0.9/async_openai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/errors.py` & `async_openai-0.0.9/async_openai/types/errors.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/options.py` & `async_openai-0.0.9/async_openai/types/options.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/resources.py` & `async_openai-0.0.9/async_openai/types/resources.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/responses.py` & `async_openai-0.0.9/async_openai/types/responses.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/types/routes.py` & `async_openai-0.0.9/async_openai/types/routes.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/utils/config.py` & `async_openai-0.0.9/async_openai/utils/config.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai/utils/helpers.py` & `async_openai-0.0.9/async_openai/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/async_openai.egg-info/PKG-INFO` & `async_openai-0.0.9/async_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-openai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unofficial Async Python client library for the OpenAI API
 Home-page: https://github.com/GrowthEngineAI/async-openai
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `async_openai-0.0.8/async_openai.egg-info/SOURCES.txt` & `async_openai-0.0.9/async_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async_openai-0.0.8/setup.py` & `async_openai-0.0.9/setup.py`

 * *Files identical despite different names*

