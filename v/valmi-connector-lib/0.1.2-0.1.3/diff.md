# Comparing `tmp/valmi_connector_lib-0.1.2.tar.gz` & `tmp/valmi_connector_lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.2.tar", last modified: Mon Apr 17 11:26:19 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.3.tar", last modified: Mon Apr 17 11:33:33 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.2.tar` & `valmi_connector_lib-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.929086 valmi_connector_lib-0.1.2/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:26:19.929129 valmi_connector_lib-0.1.2/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.2/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:26:19.929353 valmi_connector_lib-0.1.2/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      600 2023-04-17 11:23:21.000000 valmi_connector_lib-0.1.2/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.925731 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:26:19.000000 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      911 2023-04-17 11:26:19.000000 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:26:19.000000 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       48 2023-04-17 11:26:19.000000 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:26:19.000000 valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.925833 valmi_connector_lib-0.1.2/valmi_lib/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.2/valmi_lib/__init__.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.927386 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6006 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-15 12:32:17.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)      110 2023-04-17 11:26:04.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/main.py
--rw-r--r--   0 raj        (501) staff       (20)     5403 2023-04-15 12:33:27.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3556 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2448 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/read_handlers.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.927661 valmi_connector_lib-0.1.2/valmi_lib/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.2/valmi_lib/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.2/valmi_lib/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.928117 valmi_connector_lib-0.1.2/valmi_lib/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.2/valmi_lib/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.2/valmi_lib/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:26:19.928962 valmi_connector_lib-0.1.2/valmi_lib/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.2/valmi_lib/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.2/valmi_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.2/valmi_lib/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.582954 valmi_connector_lib-0.1.3/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:33:33.583013 valmi_connector_lib-0.1.3/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.3/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:33:33.583299 valmi_connector_lib-0.1.3/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      600 2023-04-17 11:33:18.000000 valmi_connector_lib-0.1.3/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.579686 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       48 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:33:33.000000 valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.579790 valmi_connector_lib-0.1.3/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.3/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581070 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6006 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-15 12:32:17.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5403 2023-04-15 12:33:27.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3556 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2448 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581435 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.581932 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:33:33.582759 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.2/setup.py` & `valmi_connector_lib-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.2",
+    version="0.1.3",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.2/valmi_connector_lib.egg-info/SOURCES.txt` & `valmi_connector_lib-0.1.3/valmi_connector_lib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 valmi_connector_lib.egg-info/dependency_links.txt
 valmi_connector_lib.egg-info/requires.txt
 valmi_connector_lib.egg-info/top_level.txt
 valmi_lib/__init__.py
 valmi_lib/destination_wrapper/__init__.py
 valmi_lib/destination_wrapper/destination_container_wrapper.py
 valmi_lib/destination_wrapper/engine.py
-valmi_lib/destination_wrapper/main.py
 valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
 valmi_lib/destination_wrapper/proc_stdout_handler.py
 valmi_lib/destination_wrapper/read_handlers.py
 valmi_lib/source_wrapper/__init__.py
 valmi_lib/source_wrapper/source_container_wrapper.py
 valmi_lib/valmi_destination/__init__.py
 valmi_lib/valmi_destination/valmi_destination.py
```

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.3/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.3/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.3/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.2/valmi_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.3/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files identical despite different names*

