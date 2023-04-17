# Comparing `tmp/audiostack-0.0.4.tar.gz` & `tmp/audiostack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-0.0.4.tar", last modified: Thu Mar 16 15:15:47 2023, max compression
+gzip compressed data, was "audiostack-0.0.5.tar", last modified: Mon Apr 17 07:57:04 2023, max compression
```

## Comparing `audiostack-0.0.4.tar` & `audiostack-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.408275 audiostack-0.0.4/
--rw-r--r--   0 hackerman   (501) staff       (20)     1061 2022-12-06 15:30:00.000000 audiostack-0.0.4/LICENSE
--rw-r--r--   0 hackerman   (501) staff       (20)    27234 2023-03-16 15:15:47.408064 audiostack-0.0.4/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.4/README.md
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.396759 audiostack-0.0.4/audiostack/
--rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-03-16 15:15:40.000000 audiostack-0.0.4/audiostack/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.399376 audiostack-0.0.4/audiostack/content/
--rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.4/audiostack/content/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/content/media.py
--rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.4/audiostack/content/root_functions.py
--rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/content/script.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.399758 audiostack-0.0.4/audiostack/delivery/
--rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.4/audiostack/delivery/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1902 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/delivery/encoder.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.400359 audiostack-0.0.4/audiostack/docs/
--rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/docs/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/docs/docs.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.402556 audiostack-0.0.4/audiostack/helpers/
--rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.4/audiostack/helpers/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/helpers/api_item.py
--rw-r--r--   0 hackerman   (501) staff       (20)      811 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/helpers/api_list.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4300 2023-03-15 15:14:21.000000 audiostack-0.0.4/audiostack/helpers/request_interface.py
--rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/helpers/request_types.py
--rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/helpers/response.py
--rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/helpers/util.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.402794 audiostack-0.0.4/audiostack/orchestrator/
--rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.405359 audiostack-0.0.4/audiostack/production/
--rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/production/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4138 2023-03-16 15:15:23.000000 audiostack-0.0.4/audiostack/production/mix.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4394 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/production/sound.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.406245 audiostack-0.0.4/audiostack/speech/
--rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.4/audiostack/speech/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/speech/diction.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4502 2023-03-16 15:15:23.000000 audiostack-0.0.4/audiostack/speech/tts.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.4/audiostack/speech/voice.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.397440 audiostack-0.0.4/audiostack.egg-info/
--rw-r--r--   0 hackerman   (501) staff       (20)    27234 2023-03-16 15:15:47.000000 audiostack-0.0.4/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)      967 2023-03-16 15:15:47.000000 audiostack-0.0.4/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-03-16 15:15:47.000000 audiostack-0.0.4/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-03-16 15:15:47.000000 audiostack-0.0.4/audiostack.egg-info/requires.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-03-16 15:15:47.000000 audiostack-0.0.4/audiostack.egg-info/top_level.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-03-16 15:15:47.408334 audiostack-0.0.4/setup.cfg
--rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.4/setup.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-03-16 15:15:47.407276 audiostack-0.0.4/tests/
--rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.4/tests/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.4/tests/test_audience.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.080026 audiostack-0.0.5/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-04-17 07:57:04.079543 audiostack-0.0.5/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.5/README.md
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.069086 audiostack-0.0.5/audiostack/
+-rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-04-17 07:56:01.000000 audiostack-0.0.5/audiostack/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.071102 audiostack-0.0.5/audiostack/content/
+-rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/content/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/content/media.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/content/root_functions.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/content/script.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.072118 audiostack-0.0.5/audiostack/delivery/
+-rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.5/audiostack/delivery/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     1902 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/delivery/encoder.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.072863 audiostack-0.0.5/audiostack/docs/
+-rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/docs/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/docs/docs.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.074939 audiostack-0.0.5/audiostack/helpers/
+-rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.5/audiostack/helpers/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/api_item.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      811 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/api_list.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4301 2023-04-17 07:54:26.000000 audiostack-0.0.5/audiostack/helpers/request_interface.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/request_types.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/response.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/helpers/util.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.075194 audiostack-0.0.5/audiostack/orchestrator/
+-rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.076032 audiostack-0.0.5/audiostack/production/
+-rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/production/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4138 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/production/mix.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.5/audiostack/production/sound.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.077852 audiostack-0.0.5/audiostack/speech/
+-rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.5/audiostack/speech/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/speech/diction.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4502 2023-03-16 15:15:23.000000 audiostack-0.0.5/audiostack/speech/tts.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.5/audiostack/speech/voice.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.069855 audiostack-0.0.5/audiostack.egg-info/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/requires.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-04-17 07:57:04.000000 audiostack-0.0.5/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-04-17 07:57:04.080136 audiostack-0.0.5/setup.cfg
+-rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.5/setup.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-04-17 07:57:04.078871 audiostack-0.0.5/tests/
+-rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.5/tests/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.5/tests/test_audience.py
```

### Comparing `audiostack-0.0.4/PKG-INFO` & `audiostack-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: audiostack
-Version: 0.0.4
-Summary: Python SDK for Audiostack API
-Home-page: https://github.com/aflorithmic/audiostack-python
-Author: Aflorithmic
-Author-email: sam@aflorithmic.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 <a href="https://www.api.audio/" rel="noopener">
  <img src="https://uploads-ssl.webflow.com/60b89b300a9c71a64936aafd/60c1d07f4fd2c92916129788_logoAudio.svg" alt="api.audio logo"></a>
 </p>
 
 <h3 align="center">apiaudio - audiostack SDK</h3>
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: audiostack Version: 0.0.4 Summary: Python SDK for
-Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
-Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
                                [api.audio_logo]
                       **** apiaudio - audiostack SDK ****
 ---
    audiostack is the official api.audio Python 3 SDK. This SDK provides easy
        access to the api.audio API for applications written in python.
 ## Maintainers  - https://github.com/Sjhunt93 ## License  This project is
 licensed under the terms of the MIT license. # ð Table of Contents -
```

### Comparing `audiostack-0.0.4/audiostack/__init__.py` & `audiostack-0.0.5/audiostack/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-sdk_version = "0.0.4"
+sdk_version = "0.0.5"
 api_base = "https://v2.api.audio"
 api_key = None
 
-api_version = "0.0.4"
+api_version = "0.0.5"
 verify_ssl_certs = True
 proxy = None
 default_http_client = None
 app_info = None
 enable_telemetry = True
 max_network_retries = 0
```

### Comparing `audiostack-0.0.4/audiostack/content/media.py` & `audiostack-0.0.5/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/content/root_functions.py` & `audiostack-0.0.5/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/content/script.py` & `audiostack-0.0.5/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/delivery/encoder.py` & `audiostack-0.0.5/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/docs/docs.py` & `audiostack-0.0.5/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/helpers/api_item.py` & `audiostack-0.0.5/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/helpers/api_list.py` & `audiostack-0.0.5/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/helpers/request_interface.py` & `audiostack-0.0.5/audiostack/helpers/request_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             else:
                 final_dict[key] = val
     return final_dict
 
 
 class RequestInterface:
     # disable debug print
-    DEBUG_PRINT = True
+    DEBUG_PRINT = False
 
     def __init__(self, family: str) -> None:
         self.family = family
 
     def make_header(self):
         return {
             "x-api-key": audiostack.api_key,
```

### Comparing `audiostack-0.0.4/audiostack/production/mix.py` & `audiostack-0.0.5/audiostack/production/mix.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/production/sound.py` & `audiostack-0.0.5/audiostack/production/sound.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             return Sound.Template.List(r, list_type="templates")
 
         def create(templateName: str, description: str = ""):
             body = {"templateName": templateName, "description": description}
             r = Sound.interface.send_request(
                 rtype=RequestTypes.POST, route="template", json=body
             )
-            print(r)
             return Sound.Template.Item(r)
 
         def delete(templateName: str):
             r = Sound.interface.send_request(
                 rtype=RequestTypes.DELETE,
                 route="template",
                 path_parameters=templateName,
@@ -88,15 +87,14 @@
             body = {
                 "templateName": templateName,
                 "description": description,
                 "genre": genre,
                 "collections": collections,
                 "tags": tags,
             }
-            print(body)
             r = Sound.interface.send_request(
                 rtype=RequestTypes.PUT, route="template", json=body
             )
             return Sound.Template.Item(r)
 
     # ----------------------------------------- TEMPLATE SEGMENT -----------------------------------------
     class Segment:
```

### Comparing `audiostack-0.0.4/audiostack/speech/diction.py` & `audiostack-0.0.5/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/speech/tts.py` & `audiostack-0.0.5/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack/speech/voice.py` & `audiostack-0.0.5/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/audiostack.egg-info/SOURCES.txt` & `audiostack-0.0.5/audiostack.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 audiostack/__init__.py
 audiostack.egg-info/PKG-INFO
 audiostack.egg-info/SOURCES.txt
 audiostack.egg-info/dependency_links.txt
 audiostack.egg-info/requires.txt
```

### Comparing `audiostack-0.0.4/setup.py` & `audiostack-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.4/tests/test_audience.py` & `audiostack-0.0.5/tests/test_audience.py`

 * *Files identical despite different names*

