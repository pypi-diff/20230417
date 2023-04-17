# Comparing `tmp/oarepo-vocabularies-1.0.8.tar.gz` & `tmp/oarepo-vocabularies-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-1.0.8.tar", last modified: Fri Mar 24 06:53:52 2023, max compression
+gzip compressed data, was "oarepo-vocabularies-1.0.9.tar", last modified: Sun Mar 26 07:43:56 2023, max compression
```

## Comparing `oarepo-vocabularies-1.0.8.tar` & `oarepo-vocabularies-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/ui_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.053284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.053284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/templates/oarepo_ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/oarepo_vocabularies/templates/oarepo_ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 06:53:52.057284 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-24 06:53:51.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-24 06:53:52.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 06:53:51.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-24 06:53:51.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-24 06:53:51.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-24 06:53:51.000000 oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-24 06:53:52.061284 oarepo-vocabularies-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-24 06:50:11.000000 oarepo-vocabularies-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/ui_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:43:56.202370 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-26 07:43:56.000000 oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-26 07:43:56.206369 oarepo-vocabularies-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 07:40:14.000000 oarepo-vocabularies-1.0.9/setup.py
```

### Comparing `oarepo-vocabularies-1.0.8/LICENSE` & `oarepo-vocabularies-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/PKG-INFO` & `oarepo-vocabularies-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 1.0.8
+Version: 1.0.9
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-1.0.8/README.md` & `oarepo-vocabularies-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/config.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/ext.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/fixtures.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/api.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/resources/config.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/config.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/schemas.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/schemas.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/search.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/services/ui_schemas.py` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/services/ui_schemas.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 00000000: 7b25 2d20 6d61 6372 6f20 7265 6e64 6572  {%- macro render
 00000010: 5f76 6f63 6162 756c 6172 795f 6974 656d  _vocabulary_item
-00000020: 2861 7267 2920 2d25 7d0a 3c73 7061 6e20  (arg) -%}.<span 
-00000030: 636c 6173 733d 2776 6f63 6162 756c 6172  class='vocabular
-00000040: 7927 3e7b 7b20 6172 672e 7469 746c 6520  y'>{{ arg.title 
-00000050: 7d7d 3c2f 7370 616e 3e0a 7b25 2d20 656e  }}</span>.{%- en
-00000060: 646d 6163 726f 202d 257d 0a0a 7b25 2d20  dmacro -%}..{%- 
-00000070: 6d61 6372 6f20 7265 6e64 6572 5f74 6178  macro render_tax
-00000080: 6f6e 6f6d 795f 6974 656d 2861 7267 2920  onomy_item(arg) 
-00000090: 2d25 7d0a 3c73 7061 6e20 636c 6173 733d  -%}.<span class=
-000000a0: 2774 6178 6f6e 6f6d 7927 3e0a 7b25 2d20  'taxonomy'>.{%- 
-000000b0: 666f 7220 7469 746c 6520 696e 2061 7267  for title in arg
-000000c0: 2e68 6965 7261 7263 6879 2e74 6974 6c65  .hierarchy.title
-000000d0: 202d 257d 0a20 2020 203c 7370 616e 2063   -%}.    <span c
-000000e0: 6c61 7373 3d27 766f 6361 6275 6c61 7279  lass='vocabulary
-000000f0: 273e 7b7b 2074 6974 6c65 207d 7d3c 2f73  '>{{ title }}</s
-00000100: 7061 6e3e 0a20 2020 207b 252d 2069 6620  pan>.    {%- if 
-00000110: 6e6f 7420 6c6f 6f70 2e6c 6173 7420 2d25  not loop.last -%
-00000120: 7d0a 2020 2020 2020 7b25 2d20 7661 6c75  }.      {%- valu
-00000130: 6520 7569 3d31 2063 6f6d 706f 6e65 6e74  e ui=1 component
-00000140: 3d22 7461 786f 6e6f 6d79 5f73 6570 6172  ="taxonomy_separ
-00000150: 6174 6f72 2220 2d25 7d0a 2020 2020 7b25  ator" -%}.    {%
-00000160: 2d20 656e 6469 6620 2d25 7d0a 7b25 2d20  - endif -%}.{%- 
-00000170: 656e 6466 6f72 202d 257d 0a3c 2f73 7061  endfor -%}.</spa
-00000180: 6e3e 0a7b 252d 2065 6e64 6d61 6372 6f20  n>.{%- endmacro 
-00000190: 2d25 7d0a 0a7b 252d 206d 6163 726f 2072  -%}..{%- macro r
-000001a0: 656e 6465 725f 7461 786f 6e6f 6d79 5f73  ender_taxonomy_s
-000001b0: 6570 6172 6174 6f72 2861 7267 2920 2d25  eparator(arg) -%
-000001c0: 7d0a 7b25 2d20 6966 2061 7267 202d 257d  }.{%- if arg -%}
-000001d0: 3c73 7061 6e20 636c 6173 733d 2774 6178  <span class='tax
-000001e0: 6f6e 6f6d 795f 7365 7061 7261 746f 7227  onomy_separator'
-000001f0: 3e20 2667 743b 203c 2f73 7061 6e3e 7b25  > &gt; </span>{%
-00000200: 2d20 656e 6469 6620 2d25 7d0a 7b25 2d20  - endif -%}.{%- 
-00000210: 656e 646d 6163 726f 202d 257d 0a0a       endmacro -%}..
+00000020: 2861 7267 2920 2d25 7d0a 3c61 2068 7265  (arg) -%}.<a hre
+00000030: 663d 222f 766f 6361 6275 6c61 7279 2f7b  f="/vocabulary/{
+00000040: 7b61 7267 2e74 7970 657d 7d2f 7b7b 6172  {arg.type}}/{{ar
+00000050: 672e 6964 7d7d 223e 3c69 2063 6c61 7373  g.id}}"><i class
+00000060: 3d22 6963 6f6e 2061 6c69 676e 206a 7573  ="icon align jus
+00000070: 7469 6679 223e 3c2f 693e 3c2f 613e 203c  tify"></i></a> <
+00000080: 7370 616e 2063 6c61 7373 3d27 766f 6361  span class='voca
+00000090: 6275 6c61 7279 273e 7b7b 2061 7267 2e74  bulary'>{{ arg.t
+000000a0: 6974 6c65 207d 7d3c 2f73 7061 6e3e 0a7b  itle }}</span>.{
+000000b0: 252d 2065 6e64 6d61 6372 6f20 2d25 7d0a  %- endmacro -%}.
+000000c0: 0a7b 252d 206d 6163 726f 2072 656e 6465  .{%- macro rende
+000000d0: 725f 7461 786f 6e6f 6d79 5f69 7465 6d28  r_taxonomy_item(
+000000e0: 6172 6729 202d 257d 0a3c 7370 616e 2063  arg) -%}.<span c
+000000f0: 6c61 7373 3d27 7461 786f 6e6f 6d79 273e  lass='taxonomy'>
+00000100: 0a7b 252d 2066 6f72 2074 6974 6c65 2069  .{%- for title i
+00000110: 6e20 6172 672e 6869 6572 6172 6368 792e  n arg.hierarchy.
+00000120: 7469 746c 6520 2d25 7d0a 3c61 2068 7265  title -%}.<a hre
+00000130: 663d 222f 766f 6361 6275 6c61 7279 2f7b  f="/vocabulary/{
+00000140: 7b61 7267 2e74 7970 657d 7d2f 7b7b 6172  {arg.type}}/{{ar
+00000150: 672e 6964 7d7d 223e 3c69 2063 6c61 7373  g.id}}"><i class
+00000160: 3d22 6963 6f6e 2061 6c69 676e 206a 7573  ="icon align jus
+00000170: 7469 6679 223e 3c2f 693e 3c2f 613e 203c  tify"></i></a> <
+00000180: 7370 616e 2063 6c61 7373 3d27 766f 6361  span class='voca
+00000190: 6275 6c61 7279 273e 7b7b 2074 6974 6c65  bulary'>{{ title
+000001a0: 207d 7d3c 2f73 7061 6e3e 0a20 2020 207b   }}</span>.    {
+000001b0: 252d 2069 6620 6e6f 7420 6c6f 6f70 2e6c  %- if not loop.l
+000001c0: 6173 7420 2d25 7d0a 2020 2020 2020 7b25  ast -%}.      {%
+000001d0: 2d20 7661 6c75 6520 7569 3d31 2c20 636f  - value ui=1, co
+000001e0: 6d70 6f6e 656e 743d 2274 6178 6f6e 6f6d  mponent="taxonom
+000001f0: 795f 7365 7061 7261 746f 7222 202d 257d  y_separator" -%}
+00000200: 0a20 2020 207b 252d 2065 6e64 6966 202d  .    {%- endif -
+00000210: 257d 0a7b 252d 2065 6e64 666f 7220 2d25  %}.{%- endfor -%
+00000220: 7d0a 3c2f 7370 616e 3e0a 7b25 2d20 656e  }.</span>.{%- en
+00000230: 646d 6163 726f 202d 257d 0a0a 7b25 2d20  dmacro -%}..{%- 
+00000240: 6d61 6372 6f20 7265 6e64 6572 5f74 6178  macro render_tax
+00000250: 6f6e 6f6d 795f 7365 7061 7261 746f 7228  onomy_separator(
+00000260: 6172 6729 202d 257d 0a7b 252d 2069 6620  arg) -%}.{%- if 
+00000270: 6172 6720 2d25 7d3c 7370 616e 2063 6c61  arg -%}<span cla
+00000280: 7373 3d27 7461 786f 6e6f 6d79 5f73 6570  ss='taxonomy_sep
+00000290: 6172 6174 6f72 273e 2026 6774 3b20 3c2f  arator'> &gt; </
+000002a0: 7370 616e 3e7b 252d 2065 6e64 6966 202d  span>{%- endif -
+000002b0: 257d 0a7b 252d 2065 6e64 6d61 6372 6f20  %}.{%- endmacro 
+000002c0: 2d25 7d0a                                -%}.
```

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 1.0.8
+Version: 1.0.9
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-1.0.8/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo-vocabularies-1.0.9/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-1.0.8/setup.cfg` & `oarepo-vocabularies-1.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 1.0.8
+version = 1.0.9
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

