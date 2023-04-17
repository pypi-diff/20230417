# Comparing `tmp/ovos-vad-plugin-precise-0.0.1a4.tar.gz` & `tmp/ovos-vad-plugin-precise-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-vad-plugin-precise-0.0.1a4.tar", last modified: Mon Apr 17 21:29:26 2023, max compression
+gzip compressed data, was "ovos-vad-plugin-precise-0.0.1a5.tar", last modified: Mon Apr 17 21:29:49 2023, max compression
```

## Comparing `ovos-vad-plugin-precise-0.0.1a4.tar` & `ovos-vad-plugin-precise-0.0.1a5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:26.741860 ovos-vad-plugin-precise-0.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 21:29:26.741860 ovos-vad-plugin-precise-0.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:26.737860 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/vad.tflite
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 21:29:22.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:26.737860 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:29:26.000000 ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:29:26.741860 ovos-vad-plugin-precise-0.0.1a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-04-17 21:29:19.000000 ovos-vad-plugin-precise-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:49.475664 ovos-vad-plugin-precise-0.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 21:29:49.475664 ovos-vad-plugin-precise-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:49.475664 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/vad.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 21:29:45.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:29:49.475664 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:29:49.000000 ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:29:49.475664 ovos-vad-plugin-precise-0.0.1a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-04-17 21:29:40.000000 ovos-vad-plugin-precise-0.0.1a5/setup.py
```

### Comparing `ovos-vad-plugin-precise-0.0.1a4/LICENSE.md` & `ovos-vad-plugin-precise-0.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a4/PKG-INFO` & `ovos-vad-plugin-precise-0.0.1a5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-precise
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: precise VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-precise
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-precise-0.0.1a4/README.md` & `ovos-vad-plugin-precise-0.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/__init__.py` & `ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise/vad.tflite` & `ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise/vad.tflite`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-precise-0.0.1a4/ovos_vad_plugin_precise.egg-info/PKG-INFO` & `ovos-vad-plugin-precise-0.0.1a5/ovos_vad_plugin_precise.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-precise
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: precise VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-precise
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-precise-0.0.1a4/setup.py` & `ovos-vad-plugin-precise-0.0.1a5/setup.py`

 * *Files identical despite different names*

