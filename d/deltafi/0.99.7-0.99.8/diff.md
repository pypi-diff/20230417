# Comparing `tmp/deltafi-0.99.7.tar.gz` & `tmp/deltafi-0.99.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-0.99.7.tar", max compression
+gzip compressed data, was "deltafi-0.99.8.tar", max compression
```

## Comparing `deltafi-0.99.7.tar` & `deltafi-0.99.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      189 2023-01-05 23:22:04.560397 deltafi-0.99.7/README.md
--rw-r--r--   0        0        0      680 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/__init__.py
--rw-r--r--   0        0        0     8833 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/action.py
--rw-r--r--   0        0        0     1689 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      957 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/actiontype.py
--rw-r--r--   0        0        0     6329 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/domain.py
--rw-r--r--   0        0        0     1247 2023-01-05 23:22:04.560397 deltafi-0.99.7/deltafi/exception.py
--rw-r--r--   0        0        0     9389 2023-01-05 23:22:04.568397 deltafi-0.99.7/deltafi/input.py
--rw-r--r--   0        0        0     2078 2023-01-05 23:22:04.568397 deltafi-0.99.7/deltafi/logger.py
--rw-r--r--   0        0        0     1063 2023-01-05 23:22:04.568397 deltafi-0.99.7/deltafi/metric.py
--rw-r--r--   0        0        0     7659 2023-01-05 23:22:04.569397 deltafi-0.99.7/deltafi/plugin.py
--rw-r--r--   0        0        0     7018 2023-01-05 23:22:04.569397 deltafi-0.99.7/deltafi/result.py
--rw-r--r--   0        0        0     3480 2023-01-05 23:22:04.569397 deltafi-0.99.7/deltafi/storage.py
--rw-r--r--   0        0        0     1270 2023-01-05 23:27:26.560356 deltafi-0.99.7/pyproject.toml
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 deltafi-0.99.7/setup.py
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-0.99.7/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-01-09 19:04:11.248680 deltafi-0.99.8/README.md
+-rw-r--r--   0        0        0      680 2023-01-09 19:04:11.248680 deltafi-0.99.8/deltafi/__init__.py
+-rw-r--r--   0        0        0     8833 2023-01-09 19:04:11.248680 deltafi-0.99.8/deltafi/action.py
+-rw-r--r--   0        0        0     1689 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      957 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/actiontype.py
+-rw-r--r--   0        0        0     6329 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/domain.py
+-rw-r--r--   0        0        0     1247 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/exception.py
+-rw-r--r--   0        0        0     9389 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/input.py
+-rw-r--r--   0        0        0     2078 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/logger.py
+-rw-r--r--   0        0        0     1063 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/metric.py
+-rw-r--r--   0        0        0     7699 2023-01-09 19:04:11.249680 deltafi-0.99.8/deltafi/plugin.py
+-rw-r--r--   0        0        0     7018 2023-01-09 19:04:11.250680 deltafi-0.99.8/deltafi/result.py
+-rw-r--r--   0        0        0     3480 2023-01-09 19:04:11.250680 deltafi-0.99.8/deltafi/storage.py
+-rw-r--r--   0        0        0     1270 2023-01-09 19:09:25.496651 deltafi-0.99.8/pyproject.toml
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 deltafi-0.99.8/setup.py
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 deltafi-0.99.8/PKG-INFO
```

### Comparing `deltafi-0.99.7/deltafi/__init__.py` & `deltafi-0.99.8/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/action.py` & `deltafi-0.99.8/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/actioneventqueue.py` & `deltafi-0.99.8/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/actiontype.py` & `deltafi-0.99.8/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/domain.py` & `deltafi-0.99.8/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/exception.py` & `deltafi-0.99.8/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/input.py` & `deltafi-0.99.8/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/logger.py` & `deltafi-0.99.8/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/metric.py` & `deltafi-0.99.8/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/plugin.py` & `deltafi-0.99.8/deltafi/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         action_logger = get_logger(self.action_name(action))
 
         action_logger.info(f"Listening on {self.action_name(action)}")
         while True:
             try:
                 event_string = self.queue.take(self.action_name(action))
                 event = Event.create(json.loads(event_string), self.hostname, self.content_service, action_logger)
+                start_time = time.time()
                 action_logger.debug(f"Processing event for did {event.context.did}")
 
                 try:
                     result = action.execute(event)
                 except ExpectedContentException as e:
                     result = ErrorResult(f"Action attempted to look up element {e.index + 1} (index {e.index}) from "
                                          f"content list of size {e.size}",
@@ -165,15 +166,15 @@
                                          f"{str(e)}\n{traceback.format_exc()}")
                 except BaseException as e:
                     result = ErrorResult(f"Action execution {type(e)} exception", f"{str(e)}\n{traceback.format_exc()}")
 
                 response = {
                     'did': event.context.did,
                     'action': event.context.action_name,
-                    'start': time.time(),
+                    'start': start_time,
                     'stop': time.time(),
                     'type': result.result_type,
                     'metrics': [metric.json() for metric in result.metrics]
                 }
                 if result.result_key is not None:
                     response[result.result_key] = result.response()
```

### Comparing `deltafi-0.99.7/deltafi/result.py` & `deltafi-0.99.8/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/deltafi/storage.py` & `deltafi-0.99.8/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-0.99.7/pyproject.toml` & `deltafi-0.99.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "0.99.7"
+version = "0.99.8"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-0.99.7/setup.py` & `deltafi-0.99.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pydantic==1.10.2',
  'redis==4.3.4',
  'requests==2.28.1',
  'urllib3==1.26.12']
 
 setup_kwargs = {
     'name': 'deltafi',
-    'version': '0.99.7',
+    'version': '0.99.8',
     'description': 'SDK for DeltaFi plugins and actions',
     'long_description': '# DeltaFi Action Kit\n\nThis project provides a Python implementation of the DeltaFi Action Kit. The DeltaFi Action Kit is a setup of modules which simplify the creation of a DeltaFi Plugin.\n',
     'author': 'DeltaFi',
     'author_email': 'deltafi@systolic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deltafi-0.99.7/PKG-INFO` & `deltafi-0.99.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 0.99.7
+Version: 0.99.8
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

