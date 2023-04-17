# Comparing `tmp/jeff_api-1.2.0.tar.gz` & `tmp/jeff_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.2.0.tar", last modified: Mon Apr 17 00:39:12 2023, max compression
+gzip compressed data, was "jeff_api-1.2.1.tar", last modified: Mon Apr 17 00:44:01 2023, max compression
```

## Comparing `jeff_api-1.2.0.tar` & `jeff_api-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:39:12.666577 jeff_api-1.2.0/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.0/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 00:39:12.666577 jeff_api-1.2.0/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.0/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 00:38:36.000000 jeff_api-1.2.0/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 00:39:12.666577 jeff_api-1.2.0/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:39:12.626577 jeff_api-1.2.0/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:39:12.660577 jeff_api-1.2.0/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)      120 2023-04-16 22:46:34.000000 jeff_api-1.2.0/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7665 2023-04-17 00:37:26.000000 jeff_api-1.2.0/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1766 2023-04-16 23:09:48.000000 jeff_api-1.2.0/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.0/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.0/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:39:12.664577 jeff_api-1.2.0/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 00:39:12.000000 jeff_api-1.2.0/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 00:39:12.000000 jeff_api-1.2.0/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 00:39:12.000000 jeff_api-1.2.0/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 00:39:12.000000 jeff_api-1.2.0/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:44:01.921537 jeff_api-1.2.1/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.1/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 00:44:01.919537 jeff_api-1.2.1/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.1/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 00:43:29.000000 jeff_api-1.2.1/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 00:44:01.921537 jeff_api-1.2.1/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:44:01.911537 jeff_api-1.2.1/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:44:01.917537 jeff_api-1.2.1/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.1/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7665 2023-04-17 00:37:26.000000 jeff_api-1.2.1/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1766 2023-04-16 23:09:48.000000 jeff_api-1.2.1/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.1/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.1/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 00:44:01.919537 jeff_api-1.2.1/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 00:44:01.000000 jeff_api-1.2.1/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 00:44:01.000000 jeff_api-1.2.1/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 00:44:01.000000 jeff_api-1.2.1/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 00:44:01.000000 jeff_api-1.2.1/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.2.0/LICENSE` & `jeff_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.0/PKG-INFO` & `jeff_api-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.2.0/src/jeff_api/bridge.py` & `jeff_api-1.2.1/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.0/src/jeff_api/extension.py` & `jeff_api-1.2.1/src/jeff_api/extension.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.0/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.2.1/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

