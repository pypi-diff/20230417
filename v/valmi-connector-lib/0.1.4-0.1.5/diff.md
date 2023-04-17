# Comparing `tmp/valmi_connector_lib-0.1.4.tar.gz` & `tmp/valmi_connector_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.4.tar", last modified: Mon Apr 17 11:39:16 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.5.tar", last modified: Mon Apr 17 12:11:44 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.4.tar` & `valmi_connector_lib-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.929419 valmi_connector_lib-0.1.4/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:39:16.929462 valmi_connector_lib-0.1.4/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.4/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 11:39:16.929690 valmi_connector_lib-0.1.4/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-17 11:39:11.000000 valmi_connector_lib-0.1.4/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.926445 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 11:39:16.000000 valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.926546 valmi_connector_lib-0.1.4/valmi_lib/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.4/valmi_lib/__init__.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.927717 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/read_handlers.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.928029 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.928577 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 11:39:16.929294 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      369 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.353321 valmi_connector_lib-0.1.5/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 12:11:44.353372 valmi_connector_lib-0.1.5/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.5/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-17 12:11:44.353621 valmi_connector_lib-0.1.5/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-17 12:11:25.000000 valmi_connector_lib-0.1.5/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.350037 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-17 12:11:44.000000 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-17 12:11:44.000000 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-17 12:11:44.000000 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-17 12:11:44.000000 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-17 12:11:44.000000 valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.350135 valmi_connector_lib-0.1.5/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.5/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.351307 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.351704 valmi_connector_lib-0.1.5/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.5/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.5/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.352365 valmi_connector_lib-0.1.5/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.5/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     6887 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.5/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-17 12:11:44.353108 valmi_connector_lib-0.1.5/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      548 2023-04-17 12:11:09.000000 valmi_connector_lib-0.1.5/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.5/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     3944 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.5/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.4/setup.py` & `valmi_connector_lib-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.4",
+    version="0.1.5",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.4/valmi_connector_lib.egg-info/SOURCES.txt` & `valmi_connector_lib-0.1.5/valmi_connector_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.5/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.5/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.5/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.4/valmi_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.5/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files identical despite different names*

