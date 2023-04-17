# Comparing `tmp/je_api_testka_dev-0.0.8.tar.gz` & `tmp/je_api_testka_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\je_api_testka_dev-0.0.8.tar", last modified: Fri Mar 11 14:20:47 2022, max compression
+gzip compressed data, was "dist\je_api_testka_dev-0.0.9.tar", last modified: Sat Mar 12 10:59:14 2022, max compression
```

## Comparing `je_api_testka_dev-0.0.8.tar` & `je_api_testka_dev-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      930 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      307 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0      966 2022-03-11 14:20:44.000000 je_api_testka_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/
--rw-rw-rw-   0        0        0     2866 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.8/je_api_testka/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/record/
--rw-rw-rw-   0        0        0        0 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.8/je_api_testka/record/__init__.py
--rw-rw-rw-   0        0        0      258 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.8/je_api_testka/record/record.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0       46 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     3134 2022-03-11 09:34:19.000000 je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     1294 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/requests_data_structure.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/
--rw-rw-rw-   0        0        0       35 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0       45 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     2754 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/exception/api_test_eceptions_tag.py
--rw-rw-rw-   0        0        0     1906 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/exception/api_test_exceptions.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/execute_action/
--rw-rw-rw-   0        0        0       50 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/execute_action/__init__.py
--rw-rw-rw-   0        0        0     1155 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/execute_action/action_executor.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0       53 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1063 2022-03-11 13:13:40.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0       40 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0       50 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1324 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0       52 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1046 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_search/
--rw-rw-rw-   0        0        0       52 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_search/__init__.py
--rw-rw-rw-   0        0        0     1084 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_search/json_search.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0       39 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0       48 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2480 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.8/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0      930 2022-03-11 14:20:46.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1332 2022-03-11 14:20:46.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-11 14:20:46.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2022-03-11 14:20:46.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-03-11 14:20:46.000000 je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-11 14:20:47.000000 je_api_testka_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      958 2022-03-07 18:28:11.000000 je_api_testka_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      966 2022-03-12 10:59:10.000000 je_api_testka_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/
+-rw-rw-rw-   0        0        0     2866 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/record/
+-rw-rw-rw-   0        0        0        0 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/record.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     3134 2022-03-11 09:34:19.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     1294 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/requests_data_structure.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/
+-rw-rw-rw-   0        0        0       35 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:52:53.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2754 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_eceptions_tag.py
+-rw-rw-rw-   0        0        0     1906 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_exceptions.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/__init__.py
+-rw-rw-rw-   0        0        0     1159 2022-03-12 09:24:21.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1063 2022-03-11 13:13:40.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0       40 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1324 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1046 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/__init__.py
+-rw-rw-rw-   0        0        0     1084 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/json_search.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2480 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1378 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      958 2022-03-11 16:12:43.000000 je_api_testka_dev-0.0.9/setup.py
```

### Comparing `je_api_testka_dev-0.0.8/LICENSE` & `je_api_testka_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/PKG-INFO` & `je_api_testka_dev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: api testing
 Home-page: https://github.com/JE-Chen/APITestka
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_api_testka_dev-0.0.8/dev_setup.py` & `je_api_testka_dev-0.0.9/dev_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_api_testka_dev",
-    version="0.0.08",
+    version="0.0.09",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="api testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/APITestka",
     packages=setuptools.find_packages(),
```

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.9/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/request_method.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/requests_wrapper/requests_data_structure.py` & `je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/requests_data_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/exception/api_test_eceptions_tag.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_eceptions_tag.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/exception/api_test_exceptions.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/execute_action/action_executor.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/action_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from je_api_testka.requests_wrapper.request_method import test_api_method
 from je_api_testka.utils.exception.api_test_exceptions import APITesterExecuteException
 from je_api_testka.utils.exception.api_test_eceptions_tag import executor_data_error
 from je_api_testka.record.record import record
 
 event_dict = {
     # test api
-    "test_api_method": test_api_method,
+        "test_api_method": test_api_method,
 }
 
 
 def execute_event(action: list):
     event = event_dict.get(action[0])
     if len(action) == 2:
         return event(**action[1])
```

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/json/json_search/json_search.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/json_search.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: api testing
 Home-page: https://github.com/JE-Chen/APITestka
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_api_testka_dev-0.0.8/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 je_api_testka/__init__.py
 je_api_testka/record/__init__.py
 je_api_testka/record/record.py
 je_api_testka/requests_wrapper/__init__.py
 je_api_testka/requests_wrapper/request_method.py
 je_api_testka/requests_wrapper/requests_data_structure.py
 je_api_testka/utils/__init__.py
+je_api_testka/utils/assert_result/__init__.py
 je_api_testka/utils/exception/__init__.py
 je_api_testka/utils/exception/api_test_eceptions_tag.py
 je_api_testka/utils/exception/api_test_exceptions.py
 je_api_testka/utils/execute_action/__init__.py
 je_api_testka/utils/execute_action/action_executor.py
 je_api_testka/utils/get_data_strcture/__init__.py
 je_api_testka/utils/get_data_strcture/get_api_data.py
```

### Comparing `je_api_testka_dev-0.0.8/setup.py` & `je_api_testka_dev-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_api_testka",
-    version="0.0.49",
+    version="0.0.50",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="api testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/APITestka",
     packages=setuptools.find_packages(),
```

