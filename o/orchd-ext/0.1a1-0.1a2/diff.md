# Comparing `tmp/orchd-ext-0.1a1.tar.gz` & `tmp/orchd-ext-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchd-ext-0.1a1.tar", last modified: Thu Apr  6 13:30:34 2023, max compression
+gzip compressed data, was "orchd-ext-0.1a2.tar", last modified: Mon Apr 17 13:19:54 2023, max compression
```

## Comparing `orchd-ext-0.1a1.tar` & `orchd-ext-0.1a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.995079 orchd-ext-0.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.995079 orchd-ext-0.1a1/src/orchd_ext/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/src/orchd_ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/src/orchd_ext/reactions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/src/orchd_ext/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/src/orchd_ext/reactions/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/src/orchd_ext/sensors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/src/orchd_ext/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/src/orchd_ext/sinks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/src/orchd_ext/sinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/src/orchd_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-06 13:30:33.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-04-06 13:30:33.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 13:30:33.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 13:30:29.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-06 13:30:33.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-06 13:30:33.000000 orchd-ext-0.1a1/src/orchd_ext.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 13:30:33.999079 orchd-ext-0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/tests/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-06 13:30:18.000000 orchd-ext-0.1a1/tests/test_sinks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/orchd_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/src/orchd_ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/orchd_ext/reactions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/src/orchd_ext/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/src/orchd_ext/reactions/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/orchd_ext/sensors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/src/orchd_ext/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/orchd_ext/sinks/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/src/orchd_ext/sinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/src/orchd_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-17 13:19:54.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-04-17 13:19:54.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 13:19:54.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 13:19:49.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-17 13:19:54.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 13:19:54.000000 orchd-ext-0.1a2/src/orchd_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:19:54.732503 orchd-ext-0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/tests/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-17 13:19:38.000000 orchd-ext-0.1a2/tests/test_sinks.py
```

### Comparing `orchd-ext-0.1a1/PKG-INFO` & `orchd-ext-0.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchd-ext
-Version: 0.1a1
+Version: 0.1a2
 Summary: Official orchd Extensions
 Home-page: UNKNOWN
 License: MIT
 Description: # Orchd Project 
         
         This is a Orchd project created with Orchd SDK. It contains custom reactions
         and sensors that can be deployed in to the Orchd Agent.
```

### Comparing `orchd-ext-0.1a1/setup.cfg` & `orchd-ext-0.1a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchd-ext-0.1a1/src/orchd_ext/reactions/core.py` & `orchd-ext-0.1a2/src/orchd_ext/reactions/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 from orchd_sdk.reaction import ReactionHandler
 from orchd_sdk.models import ReactionTemplate, Event
 
 from reactivex.subject import Subject
 
-
 logger = logging.getLogger(__name__)
 
 
 class HttpEventStreamerReactionHandler(ReactionHandler):
     """
     Capture all events and publishes on a Singleton subject.
 
@@ -20,15 +19,15 @@
     """
     events = Subject()
 
     template = ReactionTemplate(
         id='4d3aba04-a303-4793-b35a-afcf60668d58',
         name='io.orchd.reactions.templates.core.HttpEventStreamer',
         version='1.0',
-        handler='orchd_extensions.core_reactions.HttpEventStreamerReactionHandler',
+        handler='orchd_ext.core.reactions.HttpEventStreamerReactionHandler',
         triggered_on=[''],
         sinks=[],
         handler_parameters=dict(),
         active=True
     )
 
     def handle(self, event: Event, reaction: ReactionTemplate) -> None:
```

### Comparing `orchd-ext-0.1a1/src/orchd_ext.egg-info/PKG-INFO` & `orchd-ext-0.1a2/src/orchd_ext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchd-ext
-Version: 0.1a1
+Version: 0.1a2
 Summary: Official orchd Extensions
 Home-page: UNKNOWN
 License: MIT
 Description: # Orchd Project 
         
         This is a Orchd project created with Orchd SDK. It contains custom reactions
         and sensors that can be deployed in to the Orchd Agent.
```

