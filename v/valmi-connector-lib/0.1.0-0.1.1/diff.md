# Comparing `tmp/valmi_connector_lib-0.1.0.tar.gz` & `tmp/valmi_connector_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.0.tar", last modified: Mon Apr 17 10:37:03 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.1.tar", last modified: Mon Apr 17 11:14:05 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.0.tar` & `valmi_connector_lib-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.003559 valmi_connector_lib-0.1.0/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 10:37:03.003610 valmi_connector_lib-0.1.0/PKG-INFO
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.001297 valmi_connector_lib-0.1.0/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:23:53.000000 valmi_connector_lib-0.1.0/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6006 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.0/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-15 12:32:17.000000 valmi_connector_lib-0.1.0/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)     5403 2023-04-15 12:33:27.000000 valmi_connector_lib-0.1.0/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3556 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.0/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2448 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.0/destination_wrapper/read_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.0/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 10:37:03.003872 valmi_connector_lib-0.1.0/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      600 2023-04-17 10:36:49.000000 valmi_connector_lib-0.1.0/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.001603 valmi_connector_lib-0.1.0/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.0/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.0/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.002354 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 10:37:02.000000 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      721 2023-04-17 10:37:02.000000 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 10:37:02.000000 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       48 2023-04-17 10:37:02.000000 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       68 2023-04-17 10:37:02.000000 valmi_connector_lib-0.1.0/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.002682 valmi_connector_lib-0.1.0/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.0/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.0/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 10:37:03.003419 valmi_connector_lib-0.1.0/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.0/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.0/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.0/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.588518 valmi_connector_lib-0.1.1/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:14:05.588557 valmi_connector_lib-0.1.1/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.1/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:14:05.588788 valmi_connector_lib-0.1.1/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      600 2023-04-17 11:13:42.000000 valmi_connector_lib-0.1.1/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.585517 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:14:05.000000 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 11:14:05.000000 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:14:05.000000 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       48 2023-04-17 11:14:05.000000 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:14:05.000000 valmi_connector_lib-0.1.1/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.585615 valmi_connector_lib-0.1.1/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.1/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.586757 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:23:53.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6006 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-15 12:32:17.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5403 2023-04-15 12:33:27.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3556 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2448 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.587211 valmi_connector_lib-0.1.1/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.1/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.1/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.587712 valmi_connector_lib-0.1.1/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.1/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.1/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:14:05.588393 valmi_connector_lib-0.1.1/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.1/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.1/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.1/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.0/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.1/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/setup.py` & `valmi_connector_lib-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.0",
+    version="0.1.1",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.0/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.1/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.1/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.0/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.1/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files identical despite different names*

