# Comparing `tmp/flexypy-0.0.1.tar.gz` & `tmp/flexypy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.1.tar", last modified: Mon Apr 17 08:03:28 2023, max compression
+gzip compressed data, was "flexypy-0.0.2.tar", last modified: Mon Apr 17 08:36:21 2023, max compression
```

## Comparing `flexypy-0.0.1.tar` & `flexypy-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:28.144674 flexypy-0.0.1/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:03:28.144674 flexypy-0.0.1/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.664673 flexypy-0.0.1/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.1/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.1/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.716673 flexypy-0.0.1/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.1/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.1/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.1/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.1/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.732673 flexypy-0.0.1/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.1/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.1/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.1/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.804673 flexypy-0.0.1/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.1/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.1/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.804673 flexypy-0.0.1/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.1/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.904673 flexypy-0.0.1/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.1/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.1/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.1/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      156 2023-04-16 08:47:03.000000 flexypy-0.0.1/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.936673 flexypy-0.0.1/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.1/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1168 2023-04-14 14:37:12.000000 flexypy-0.0.1/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2634 2023-04-15 08:50:25.000000 flexypy-0.0.1/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     8359 2023-04-16 08:44:00.000000 flexypy-0.0.1/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.952674 flexypy-0.0.1/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.1/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:28.124674 flexypy-0.0.1/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.1/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.1/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      431 2023-04-16 08:43:50.000000 flexypy-0.0.1/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3248 2023-04-16 08:44:00.000000 flexypy-0.0.1/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:28.136674 flexypy-0.0.1/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.1/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.1/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:03:27.684673 flexypy-0.0.1/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:03:27.000000 flexypy-0.0.1/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1139 2023-04-17 08:03:27.000000 flexypy-0.0.1/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-17 08:03:27.000000 flexypy-0.0.1/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-17 08:03:27.000000 flexypy-0.0.1/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-17 08:03:27.000000 flexypy-0.0.1/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-17 08:01:05.000000 flexypy-0.0.1/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-17 08:03:28.144674 flexypy-0.0.1/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:36:21.848876 flexypy-0.0.2/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.840876 flexypy-0.0.2/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.2/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.2/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.2/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.2/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.2/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.2/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.2/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.2/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.2/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.2/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.2/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.2/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      254 2023-04-17 08:31:23.000000 flexypy-0.0.2/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.2/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1168 2023-04-14 14:37:12.000000 flexypy-0.0.2/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2634 2023-04-15 08:50:25.000000 flexypy-0.0.2/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     8359 2023-04-16 08:44:00.000000 flexypy-0.0.2/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.2/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.2/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.2/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      431 2023-04-16 08:43:50.000000 flexypy-0.0.2/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3248 2023-04-16 08:44:00.000000 flexypy-0.0.2/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.2/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.2/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1139 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-17 08:36:14.000000 flexypy-0.0.2/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-17 08:36:21.848876 flexypy-0.0.2/setup.cfg
```

### Comparing `flexypy-0.0.1/flexypy/exceptions/web/server.py` & `flexypy-0.0.2/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/generate_templates/generator.py` & `flexypy-0.0.2/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/http/request.py` & `flexypy-0.0.2/flexypy/http/request.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/http/routing.py` & `flexypy-0.0.2/flexypy/http/routing.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/http/server.py` & `flexypy-0.0.2/flexypy/http/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.0.2/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy/http/template/render.py` & `flexypy-0.0.2/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.1/flexypy.egg-info/SOURCES.txt` & `flexypy-0.0.2/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

