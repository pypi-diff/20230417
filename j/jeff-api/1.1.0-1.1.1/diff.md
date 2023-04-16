# Comparing `tmp/jeff_api-1.1.0.tar.gz` & `tmp/jeff_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.1.0.tar", last modified: Sun Apr 16 22:44:01 2023, max compression
+gzip compressed data, was "jeff_api-1.1.1.tar", last modified: Sun Apr 16 22:47:11 2023, max compression
```

## Comparing `jeff_api-1.1.0.tar` & `jeff_api-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:44:01.269208 jeff_api-1.1.0/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.1.0/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-16 22:44:01.265208 jeff_api-1.1.0/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.1.0/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 22:43:14.000000 jeff_api-1.1.0/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 22:44:01.269208 jeff_api-1.1.0/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:44:01.155211 jeff_api-1.1.0/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:44:01.259209 jeff_api-1.1.0/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)       37 2023-04-16 21:52:39.000000 jeff_api-1.1.0/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     3852 2023-04-16 22:14:07.000000 jeff_api-1.1.0/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1760 2023-04-16 22:42:49.000000 jeff_api-1.1.0/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.1.0/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     3718 2023-04-16 22:35:08.000000 jeff_api-1.1.0/src/jeff_api/scenario.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:44:01.265208 jeff_api-1.1.0/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-16 22:44:01.000000 jeff_api-1.1.0/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      299 2023-04-16 22:44:01.000000 jeff_api-1.1.0/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 22:44:01.000000 jeff_api-1.1.0/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 22:44:01.000000 jeff_api-1.1.0/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:47:11.335435 jeff_api-1.1.1/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.1.1/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-16 22:47:11.335435 jeff_api-1.1.1/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.1.1/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 22:46:43.000000 jeff_api-1.1.1/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 22:47:11.337435 jeff_api-1.1.1/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:47:11.323435 jeff_api-1.1.1/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:47:11.331435 jeff_api-1.1.1/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      120 2023-04-16 22:46:34.000000 jeff_api-1.1.1/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     3852 2023-04-16 22:14:07.000000 jeff_api-1.1.1/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1760 2023-04-16 22:42:49.000000 jeff_api-1.1.1/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.1.1/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     3718 2023-04-16 22:35:08.000000 jeff_api-1.1.1/src/jeff_api/scenario.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 22:47:11.333435 jeff_api-1.1.1/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-16 22:47:11.000000 jeff_api-1.1.1/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      299 2023-04-16 22:47:11.000000 jeff_api-1.1.1/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 22:47:11.000000 jeff_api-1.1.1/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 22:47:11.000000 jeff_api-1.1.1/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.1.0/LICENSE` & `jeff_api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.0/PKG-INFO` & `jeff_api-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.1.0/src/jeff_api/bridge.py` & `jeff_api-1.1.1/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.0/src/jeff_api/extension.py` & `jeff_api-1.1.1/src/jeff_api/extension.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.0/src/jeff_api/scenario.py` & `jeff_api-1.1.1/src/jeff_api/scenario.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.0/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.1.1/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

