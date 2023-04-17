# Comparing `tmp/customdbcred-0.2.tar.gz` & `tmp/customdbcred-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdbcred-0.2.tar", last modified: Mon Apr 17 10:26:57 2023, max compression
+gzip compressed data, was "customdbcred-0.3.tar", last modified: Mon Apr 17 13:37:14 2023, max compression
```

## Comparing `customdbcred-0.2.tar` & `customdbcred-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.588695 customdbcred-0.2/
--rw-rw-rw-   0        0        0       57 2023-04-17 10:26:57.588695 customdbcred-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.551450 customdbcred-0.2/customdbcred/
--rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customdbcred-0.2/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.571060 customdbcred-0.2/customdbcred.egg-info/
--rw-rw-rw-   0        0        0       57 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.578596 customdbcred-0.2/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customdbcred-0.2/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.586658 customdbcred-0.2/customvalidator/
--rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customdbcred-0.2/customvalidator/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-17 10:26:57.589674 customdbcred-0.2/setup.cfg
--rw-rw-rw-   0        0        0      201 2023-04-17 10:26:39.000000 customdbcred-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.588815 customdbcred-0.3/
+-rw-rw-rw-   0        0        0       57 2023-04-17 13:37:14.587814 customdbcred-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.562380 customdbcred-0.3/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customdbcred-0.3/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.582814 customdbcred-0.3/customdbcred.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.584807 customdbcred-0.3/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customdbcred-0.3/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.585822 customdbcred-0.3/customvalidator/
+-rw-rw-rw-   0        0        0     1387 2023-04-17 13:34:13.000000 customdbcred-0.3/customvalidator/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:37:14.588815 customdbcred-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      201 2023-04-17 13:37:06.000000 customdbcred-0.3/setup.py
```

### Comparing `customdbcred-0.2/customdbcred/__init__.py` & `customdbcred-0.3/customdbcred/__init__.py`

 * *Files identical despite different names*

### Comparing `customdbcred-0.2/customstatuscodes/__init__.py` & `customdbcred-0.3/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customdbcred-0.2/customvalidator/__init__.py` & `customdbcred-0.3/customvalidator/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 # Create your views here.
 import logging
 import json
 import jsonschema
 from pathlib import Path
 
 logger = logging.getLogger("info_logs")
+logger_error = logging.getLogger('error_logs')
 
 
 def schema_validation(data, path):
     """Function for validating Json Schema functionality."""
-    flag = 0
-    schema = load(path)
-    v = jsonschema.Draft4Validator(schema)
-    errors = sorted(v.iter_errors(data), key=lambda e: e.path)
-
-    for error in errors:
-        logger.info('json validation failed')
-        flag = 452
-        output_json = dict(zip(['Status', 'Message'], [flag, error.message]))
+    try:
+        flag = 0
+        schema = load(path)
+        logger.info(schema)
+        data = data.get_json()
+        v = jsonschema.Draft4Validator(schema)
+        logger.info(v)
+        errors = sorted(v.iter_errors(data), key=lambda e: e.path)
+        for error in errors:
+            logger.info('json validation failed')
+            flag = 452
+            output_json = dict(zip(['Status', 'Message'], [flag, error.message]))
+            return output_json
+        logger.info('schema validation done')
+        output_json = dict(zip(['Status', 'Message', 'Payload'], [flag, 'schema validation done', None]))
+        return output_json
+    except Exception as ex:
+        logger_error.error(f"Exception Encountered Exception is : {ex}", exc_info=1)
+        output_json = dict(zip(['Status', 'Message', 'Payload'], [500, f"Exception encountered: {ex}", None]))
         return output_json
-    logger.info('schema validation done')
-    output_json = dict(zip(['Status', 'Message'], [flag, 'schema validation done']))
-    return output_json
 
 
 def load(schema_path):
     """
     :param schema_path:
     :return:
     """
```

