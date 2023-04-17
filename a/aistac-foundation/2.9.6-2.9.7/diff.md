# Comparing `tmp/aistac-foundation-2.9.6.tar.gz` & `tmp/aistac-foundation-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aistac-foundation-2.9.6.tar", last modified: Mon Jul 20 15:38:28 2020, max compression
+gzip compressed data, was "dist/aistac-foundation-2.9.7.tar", last modified: Tue Jul 21 22:23:59 2020, max compression
```

## Comparing `aistac-foundation-2.9.6.tar` & `aistac-foundation-2.9.7.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/
--rwxr-xr-x   0 doatridge (920500908) 1887692788     1507 2018-04-18 17:23:53.000000 aistac-foundation-2.9.6/LICENSE.txt
--rwxr-xr-x   0 doatridge (920500908) 1887692788       65 2018-04-18 17:23:53.000000 aistac-foundation-2.9.6/MANIFEST.in
--rw-r--r--   0 doatridge (920500908) 1887692788    22188 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/PKG-INFO
--rwxr-xr-x   0 doatridge (920500908) 1887692788    18337 2020-06-09 16:47:28.000000 aistac-foundation-2.9.6/README.rst
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac/
--rwxrwxrwx   0 doatridge (920500908) 1887692788      114 2020-07-20 14:31:54.000000 aistac-foundation-2.9.6/aistac/__init__.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac/components/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-14 18:31:57.000000 aistac-foundation-2.9.6/aistac/components/__init__.py
--rw-r--r--   0 doatridge (920500908) 1887692788    44302 2020-07-20 15:24:34.000000 aistac-foundation-2.9.6/aistac/components/abstract_component.py
--rw-r--r--   0 doatridge (920500908) 1887692788     4240 2020-06-09 16:33:47.000000 aistac-foundation-2.9.6/aistac/components/abstract_ledger_component.py
--rw-r--r--   0 doatridge (920500908) 1887692788    13381 2020-07-19 21:15:26.000000 aistac-foundation-2.9.6/aistac/components/aistac_commons.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac/handlers/
--rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.6/aistac/handlers/__init__.py
--rw-r--r--   0 doatridge (920500908) 1887692788     4952 2020-03-15 18:30:58.000000 aistac-foundation-2.9.6/aistac/handlers/abstract_event_book.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788    14913 2020-04-15 23:08:25.000000 aistac-foundation-2.9.6/aistac/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge (920500908) 1887692788     6512 2020-02-09 23:42:24.000000 aistac-foundation-2.9.6/aistac/handlers/parsers.py
--rw-r--r--   0 doatridge (920500908) 1887692788    11638 2020-07-13 16:14:10.000000 aistac-foundation-2.9.6/aistac/handlers/python_handlers.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac/intent/
--rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.6/aistac/intent/__init__.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788    10824 2020-05-10 17:12:39.000000 aistac-foundation-2.9.6/aistac/intent/abstract_intent.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788    39219 2020-05-10 18:09:41.000000 aistac-foundation-2.9.6/aistac/intent/python_cleaners_intent.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac/properties/
--rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.6/aistac/properties/__init__.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788    61754 2020-06-19 13:25:11.000000 aistac-foundation-2.9.6/aistac/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788     2996 2019-08-08 09:17:15.000000 aistac-foundation-2.9.6/aistac/properties/decorator_patterns.py
--rw-r--r--   0 doatridge (920500908) 1887692788     5427 2020-06-10 16:01:16.000000 aistac-foundation-2.9.6/aistac/properties/ledger_property_manager.py
--rw-r--r--   0 doatridge (920500908) 1887692788    11116 2020-05-19 18:31:03.000000 aistac-foundation-2.9.6/aistac/properties/property_manager.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac_foundation.egg-info/
--rw-r--r--   0 doatridge (920500908) 1887692788    22188 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac_foundation.egg-info/PKG-INFO
--rw-r--r--   0 doatridge (920500908) 1887692788     1441 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac_foundation.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge (920500908) 1887692788        1 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac_foundation.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge (920500908) 1887692788       13 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/aistac_foundation.egg-info/top_level.txt
--rwxr-xr-x   0 doatridge (920500908) 1887692788      110 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/setup.cfg
--rwxr-xr-x   0 doatridge (920500908) 1887692788     2157 2020-04-20 00:16:15.000000 aistac-foundation-2.9.6/setup.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/components/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-16 22:33:39.000000 aistac-foundation-2.9.6/tests/components/__init__.py
--rw-r--r--   0 doatridge (920500908) 1887692788    21921 2020-07-09 14:32:52.000000 aistac-foundation-2.9.6/tests/components/abstract_component_test.py
--rw-r--r--   0 doatridge (920500908) 1887692788     7464 2020-07-19 21:13:21.000000 aistac-foundation-2.9.6/tests/components/commons_test.py
--rw-r--r--   0 doatridge (920500908) 1887692788     1410 2020-06-09 16:33:47.000000 aistac-foundation-2.9.6/tests/components/master_ledget_test.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/handlers/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2019-06-14 06:59:54.000000 aistac-foundation-2.9.6/tests/handlers/__init__.py
--rw-r--r--   0 doatridge (920500908) 1887692788    10775 2020-06-10 16:37:11.000000 aistac-foundation-2.9.6/tests/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge (920500908) 1887692788     1806 2020-03-02 00:35:34.000000 aistac-foundation-2.9.6/tests/handlers/handler_factory_test.py
--rw-r--r--   0 doatridge (920500908) 1887692788    11308 2020-04-20 00:26:37.000000 aistac-foundation-2.9.6/tests/handlers/test_handlers.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/intent/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-19 15:08:28.000000 aistac-foundation-2.9.6/tests/intent/__init__.py
--rw-r--r--   0 doatridge (920500908) 1887692788     3034 2020-05-10 18:33:22.000000 aistac-foundation-2.9.6/tests/intent/abstract_intent_test.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/properties/
--rw-rw-r--   0 doatridge (920500908) 1887692788        0 2020-03-17 15:16:07.000000 aistac-foundation-2.9.6/tests/properties/__init__.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788    34712 2020-07-09 13:41:16.000000 aistac-foundation-2.9.6/tests/properties/abstract_properties_manager_test.py
--rw-rw-r--   0 doatridge (920500908) 1887692788     4103 2020-04-27 15:42:14.000000 aistac-foundation-2.9.6/tests/properties/master_ledger_property_manager_test.py
--rwxr-xr-x   0 doatridge (920500908) 1887692788     9484 2020-05-19 18:44:01.000000 aistac-foundation-2.9.6/tests/properties/property_manager_test.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/test_data/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-30 13:17:53.000000 aistac-foundation-2.9.6/tests/test_data/__init__.py
-drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-20 15:38:28.000000 aistac-foundation-2.9.6/tests/test_data/contracts/
--rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-30 13:18:16.000000 aistac-foundation-2.9.6/tests/test_data/contracts/__init__.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/
+-rwxr-xr-x   0 doatridge (920500908) 1887692788     1507 2018-04-18 17:23:53.000000 aistac-foundation-2.9.7/LICENSE.txt
+-rwxr-xr-x   0 doatridge (920500908) 1887692788       65 2018-04-18 17:23:53.000000 aistac-foundation-2.9.7/MANIFEST.in
+-rw-r--r--   0 doatridge (920500908) 1887692788    22188 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/PKG-INFO
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    18337 2020-06-09 16:47:28.000000 aistac-foundation-2.9.7/README.rst
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac/
+-rwxrwxrwx   0 doatridge (920500908) 1887692788      114 2020-07-20 16:04:17.000000 aistac-foundation-2.9.7/aistac/__init__.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac/components/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-14 18:31:57.000000 aistac-foundation-2.9.7/aistac/components/__init__.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    44302 2020-07-20 15:24:34.000000 aistac-foundation-2.9.7/aistac/components/abstract_component.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    13381 2020-07-19 21:15:26.000000 aistac-foundation-2.9.7/aistac/components/aistac_commons.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac/handlers/
+-rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.7/aistac/handlers/__init__.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     4952 2020-03-15 18:30:58.000000 aistac-foundation-2.9.7/aistac/handlers/abstract_event_book.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    14913 2020-04-15 23:08:25.000000 aistac-foundation-2.9.7/aistac/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     6512 2020-02-09 23:42:24.000000 aistac-foundation-2.9.7/aistac/handlers/parsers.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    11638 2020-07-13 16:14:10.000000 aistac-foundation-2.9.7/aistac/handlers/python_handlers.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac/intent/
+-rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.7/aistac/intent/__init__.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    10824 2020-05-10 17:12:39.000000 aistac-foundation-2.9.7/aistac/intent/abstract_intent.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    39219 2020-05-10 18:09:41.000000 aistac-foundation-2.9.7/aistac/intent/python_cleaners_intent.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac/properties/
+-rwxr-xr-x   0 doatridge (920500908) 1887692788        0 2018-04-20 15:32:45.000000 aistac-foundation-2.9.7/aistac/properties/__init__.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    62107 2020-07-21 21:31:43.000000 aistac-foundation-2.9.7/aistac/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788     2996 2019-08-08 09:17:15.000000 aistac-foundation-2.9.7/aistac/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    11116 2020-05-19 18:31:03.000000 aistac-foundation-2.9.7/aistac/properties/property_manager.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac_foundation.egg-info/
+-rw-r--r--   0 doatridge (920500908) 1887692788    22188 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac_foundation.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge (920500908) 1887692788     1349 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac_foundation.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge (920500908) 1887692788        1 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac_foundation.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge (920500908) 1887692788       13 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/aistac_foundation.egg-info/top_level.txt
+-rwxr-xr-x   0 doatridge (920500908) 1887692788      110 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/setup.cfg
+-rwxr-xr-x   0 doatridge (920500908) 1887692788     2157 2020-04-20 00:16:15.000000 aistac-foundation-2.9.7/setup.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/components/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-16 22:33:39.000000 aistac-foundation-2.9.7/tests/components/__init__.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    21921 2020-07-09 14:32:52.000000 aistac-foundation-2.9.7/tests/components/abstract_component_test.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     7464 2020-07-19 21:13:21.000000 aistac-foundation-2.9.7/tests/components/commons_test.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     1410 2020-06-09 16:33:47.000000 aistac-foundation-2.9.7/tests/components/master_ledget_test.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/handlers/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2019-06-14 06:59:54.000000 aistac-foundation-2.9.7/tests/handlers/__init__.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    10775 2020-06-10 16:37:11.000000 aistac-foundation-2.9.7/tests/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     1806 2020-03-02 00:35:34.000000 aistac-foundation-2.9.7/tests/handlers/handler_factory_test.py
+-rw-r--r--   0 doatridge (920500908) 1887692788    11308 2020-04-20 00:26:37.000000 aistac-foundation-2.9.7/tests/handlers/test_handlers.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/intent/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-19 15:08:28.000000 aistac-foundation-2.9.7/tests/intent/__init__.py
+-rw-r--r--   0 doatridge (920500908) 1887692788     3034 2020-05-10 18:33:22.000000 aistac-foundation-2.9.7/tests/intent/abstract_intent_test.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/properties/
+-rw-rw-r--   0 doatridge (920500908) 1887692788        0 2020-03-17 15:16:07.000000 aistac-foundation-2.9.7/tests/properties/__init__.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788    35052 2020-07-21 22:22:49.000000 aistac-foundation-2.9.7/tests/properties/abstract_properties_manager_test.py
+-rw-rw-r--   0 doatridge (920500908) 1887692788     4103 2020-04-27 15:42:14.000000 aistac-foundation-2.9.7/tests/properties/master_ledger_property_manager_test.py
+-rwxr-xr-x   0 doatridge (920500908) 1887692788     9484 2020-05-19 18:44:01.000000 aistac-foundation-2.9.7/tests/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/test_data/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-30 13:17:53.000000 aistac-foundation-2.9.7/tests/test_data/__init__.py
+drwxr-xr-x   0 doatridge (920500908) 1887692788        0 2020-07-21 22:23:59.000000 aistac-foundation-2.9.7/tests/test_data/contracts/
+-rw-r--r--   0 doatridge (920500908) 1887692788        0 2020-01-30 13:18:16.000000 aistac-foundation-2.9.7/tests/test_data/contracts/__init__.py
```

### Comparing `aistac-foundation-2.9.6/LICENSE.txt` & `aistac-foundation-2.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/PKG-INFO` & `aistac-foundation-2.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aistac-foundation
-Version: 2.9.6
+Version: 2.9.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/aistac-foundation
 Author: Gigas64
 Author-email: gigas64@aistac.com
 License: BSD
 Description: AI-STAC Foundation Package
         ##########################
```

### Comparing `aistac-foundation-2.9.6/README.rst` & `aistac-foundation-2.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/components/abstract_component.py` & `aistac-foundation-2.9.7/aistac/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/components/aistac_commons.py` & `aistac-foundation-2.9.7/aistac/components/aistac_commons.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/handlers/abstract_event_book.py` & `aistac-foundation-2.9.7/aistac/handlers/abstract_event_book.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/handlers/abstract_handlers.py` & `aistac-foundation-2.9.7/aistac/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/handlers/parsers.py` & `aistac-foundation-2.9.7/aistac/handlers/parsers.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/handlers/python_handlers.py` & `aistac-foundation-2.9.7/aistac/handlers/python_handlers.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/intent/abstract_intent.py` & `aistac-foundation-2.9.7/aistac/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/intent/python_cleaners_intent.py` & `aistac-foundation-2.9.7/aistac/intent/python_cleaners_intent.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/properties/abstract_properties.py` & `aistac-foundation-2.9.7/aistac/properties/abstract_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         if isinstance(knowledge_keys, list) and len(knowledge_keys):
             self._knowledge_catalog = knowledge_keys
             self._knowledge_catalog.append('intent')
             self._knowledge_catalog.append('schema')
         else:
             self._knowledge_catalog = ['intent', 'schema']
         root_keys += ['description', 'version', 'status', 'connectors', 'intent', 'snapshot', 'run_book',
-                      {self._KNOWLEDGE_ROOT: self._knowledge_catalog}]
+                      {'meta': ['module', 'class']}, {self._KNOWLEDGE_ROOT: self._knowledge_catalog}]
         self._keys = AbstractProperty(root_keys, manager=self.manager_name(), contract=self._task_name)
         if not self.is_key(self.KEY.contract_key):
             self.reset_all()
         self._connection_handler = {}
         self._create_abstract_properties()
         self._restricted_key = []
         for key in self.KEY.keys():
@@ -1177,14 +1177,19 @@
         return rtn_dict
 
     """
         PRIVATE & UTILITIES SECTION
     """
     def _create_abstract_properties(self):
         for method in self.KEY.__dir__():
+            if method == 'meta_key':
+                if not self.is_key(self.KEY.meta.module_key):
+                    self.set(self.KEY.meta.module_key, self.__module__.split("."))
+                if not self.is_key(self.KEY.meta.class_key):
+                    self.set(self.KEY.meta.class_key, self.__class__.__name__)
             if method == 'version_key':
                 if not self.is_key(self.KEY.version_key):
                     self.set(self.KEY.version_key, 'v0.00')
             if method == 'status_key':
                 if not self.is_key(self.KEY.status_key):
                     self.set(self.KEY.status_key, 'discovery')
             if method == 'description_key':
```

### Comparing `aistac-foundation-2.9.6/aistac/properties/decorator_patterns.py` & `aistac-foundation-2.9.7/aistac/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac/properties/property_manager.py` & `aistac-foundation-2.9.7/aistac/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/aistac_foundation.egg-info/PKG-INFO` & `aistac-foundation-2.9.7/aistac_foundation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aistac-foundation
-Version: 2.9.6
+Version: 2.9.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/aistac-foundation
 Author: Gigas64
 Author-email: gigas64@aistac.com
 License: BSD
 Description: AI-STAC Foundation Package
         ##########################
```

### Comparing `aistac-foundation-2.9.6/aistac_foundation.egg-info/SOURCES.txt` & `aistac-foundation-2.9.7/aistac_foundation.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 aistac/__init__.py
 aistac/components/__init__.py
 aistac/components/abstract_component.py
-aistac/components/abstract_ledger_component.py
 aistac/components/aistac_commons.py
 aistac/handlers/__init__.py
 aistac/handlers/abstract_event_book.py
 aistac/handlers/abstract_handlers.py
 aistac/handlers/parsers.py
 aistac/handlers/python_handlers.py
 aistac/intent/__init__.py
 aistac/intent/abstract_intent.py
 aistac/intent/python_cleaners_intent.py
 aistac/properties/__init__.py
 aistac/properties/abstract_properties.py
 aistac/properties/decorator_patterns.py
-aistac/properties/ledger_property_manager.py
 aistac/properties/property_manager.py
 aistac_foundation.egg-info/PKG-INFO
 aistac_foundation.egg-info/SOURCES.txt
 aistac_foundation.egg-info/dependency_links.txt
 aistac_foundation.egg-info/top_level.txt
 tests/components/__init__.py
 tests/components/abstract_component_test.py
```

### Comparing `aistac-foundation-2.9.6/setup.py` & `aistac-foundation-2.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/components/abstract_component_test.py` & `aistac-foundation-2.9.7/tests/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/components/commons_test.py` & `aistac-foundation-2.9.7/tests/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/components/master_ledget_test.py` & `aistac-foundation-2.9.7/tests/components/master_ledget_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/handlers/connector_contract_test.py` & `aistac-foundation-2.9.7/tests/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/handlers/handler_factory_test.py` & `aistac-foundation-2.9.7/tests/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/handlers/test_handlers.py` & `aistac-foundation-2.9.7/tests/handlers/test_handlers.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/intent/abstract_intent_test.py` & `aistac-foundation-2.9.7/tests/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/properties/abstract_properties_manager_test.py` & `aistac-foundation-2.9.7/tests/properties/abstract_properties_manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,19 @@
 
     def test_reset_abstract_properties(self):
         keys = ['connectors', 'intent', 'overview']
         pm = ControlPropertyManager(task_name='contract', root_keys=keys, knowledge_keys=[])
         pm.set(pm.KEY.intent_key, 'some value')
         pm.set_version('v1')
         control = {'description': "", 'status': 'discovery', 'cleaners': {}, 'connectors': {}, 'intent': 'some value', 'overview': {}, 'run_book': {},'snapshot': {}, 'version': 'v1',
-                   'knowledge': {'intent': {}, 'schema': {}}}
+                   'meta': {'class': 'ControlPropertyManager', 'module': pm.__module__.split(".")}, 'knowledge': {'intent': {}, 'schema': {}}}
         self.assertEqual(control, pm.get(pm.KEY.contract_key))
         pm.reset_all()
         control = {'description': "", 'status': 'discovery', 'cleaners': {}, 'connectors': {}, 'intent': {}, 'overview': {}, 'run_book': {},'snapshot': {}, 'version': 'v0.00',
-                   'knowledge': {'intent': {}, 'schema': {}}}
+                   'meta': {'class': 'ControlPropertyManager', 'module': pm.__module__.split(".")}, 'knowledge': {'intent': {}, 'schema': {}}}
         self.assertEqual(control, pm.get(pm.KEY.contract_key))
 
     def test_connection_handler(self):
         pm = ControlPropertyManager('test_abstract_properties', root_keys=[], knowledge_keys=[])
         control_connector = self.connector
         pm.set_connector_contract(connector_name='control', connector_contract=self.connector)
         result = pm.get_connector_contract(connector_name='control')
@@ -133,15 +133,15 @@
         # connections should be empty as not requested a handler
         self.assertEqual([], pm.connector_handler_list)
         self.assertEqual(['control'], pm.connector_contract_list)
         pm.get_connector_handler(connector_name='control')
         self.assertEqual(['control'], pm.connector_handler_list)
         pm.remove_connector_contract(connector_name='control')
         control = {'description': '', 'status': 'discovery', 'cleaners': {}, 'connectors': {},  'intent': {}, 'run_book': {}, 'snapshot': {}, 'version': 'v0.00',
-                   'knowledge': {'intent': {}, 'schema': {}}}
+                   'meta': {'class': 'ControlPropertyManager', 'module': pm.__module__.split(".")}, 'knowledge': {'intent': {}, 'schema': {}}}
         self.assertEqual(control, pm.get(pm.KEY.contract_key))
 
     def test_set_property(self):
         pm = ControlPropertyManager('test_abstract_properties')
         pm.set_property_connector(self.connector)
         result = pm.get_connector_contract(pm.CONNECTOR_PM_CONTRACT)
         self.assertEqual('works/config_contract.pkl?sep=.&encoding=Latin1', result.raw_uri)
@@ -242,22 +242,22 @@
         result = dpm.report_info()
         control = {'contract': 'control', 'task': 'test', 'desciption': '', 'status': 'discovery', 'version': 'v0.00'}
         self.assertEqual(control, result)
 
     def test_set_snapshot(self):
         dpm = ControlPropertyManager('test_abstract_properties')
         dpm.set_snapshot('3.00.001')
-        control = ['description', 'status', 'cleaners', 'snapshot', 'intent', 'version', 'run_book','connectors', 'knowledge']
+        control = ['description', 'status', 'cleaners', 'snapshot', 'intent', 'version', 'run_book','connectors', 'knowledge', 'meta']
         self.assertCountEqual(control, list(dpm.get(dpm.KEY.contract_key).keys()))
         result = list(dpm.get(dpm.KEY.snapshot_key).keys())
         control = ['test_abstract_properties_#3_00_001']
         self.assertCountEqual(control, result)
         result = list(dpm.get(dpm.KEY.snapshot_key).get('test_abstract_properties_#3_00_001').keys())
         # check the snapshot hasn't been copied to the snapshot
-        control = ['description', 'status', 'cleaners', 'intent', 'version', 'run_book','connectors', 'knowledge']
+        control = ['description', 'status', 'cleaners', 'intent', 'version', 'run_book','connectors', 'knowledge', 'meta']
         self.assertCountEqual(control, result)
 
     def test_recover_snapshot(self):
         dpm = ControlPropertyManager('test_abstract_properties')
         version = '1.00.000'
         dpm.set(dpm.KEY.version_key, version)
         self.assertEqual(version, dpm.version)
@@ -604,15 +604,15 @@
         pm.reset_connector_contracts()
         pm.reset_intents()
         pm.reset_knowledge()
         pm.reset_run_books()
         pm.reset_snapshots()
         result = pm.get(pm.KEY.contract_key)
         control = {'cleaners': {}, 'description': '', 'status': 'discovery', 'version': 'v0.00', 'connectors': {}, 'intent': {},
-                   'knowledge': {'schema': {}}, 'run_book': {}, 'snapshot': {}}
+                   'meta': {'class': 'ControlPropertyManager', 'module': pm.__module__.split(".")}, 'knowledge': {'schema': {}}, 'run_book': {}, 'snapshot': {}}
         self.assertDictEqual(control, result)
 
     def test_report_connectors_align(self):
         pm = ControlPropertyManager('task')
         connector_name = 'connector'
         uri = "s3://bucket/path/hadron_control_task_connector.pickle?name=fred&value=45"
         cc = ConnectorContract(uri=uri, module_name='module.package', handler='Handler')
```

### Comparing `aistac-foundation-2.9.6/tests/properties/master_ledger_property_manager_test.py` & `aistac-foundation-2.9.7/tests/properties/master_ledger_property_manager_test.py`

 * *Files identical despite different names*

### Comparing `aistac-foundation-2.9.6/tests/properties/property_manager_test.py` & `aistac-foundation-2.9.7/tests/properties/property_manager_test.py`

 * *Files identical despite different names*

