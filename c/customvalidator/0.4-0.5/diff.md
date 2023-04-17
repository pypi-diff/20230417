# Comparing `tmp/customvalidator-0.4.tar.gz` & `tmp/customvalidator-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customvalidator-0.4.tar", last modified: Mon Apr 17 11:34:01 2023, max compression
+gzip compressed data, was "customvalidator-0.5.tar", last modified: Mon Apr 17 11:45:30 2023, max compression
```

## Comparing `customvalidator-0.4.tar` & `customvalidator-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.503602 customvalidator-0.4/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:34:01.502602 customvalidator-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.484307 customvalidator-0.4/customdbcred/
--rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.4/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.486358 customvalidator-0.4/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.4/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.487307 customvalidator-0.4/customvalidator/
--rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customvalidator-0.4/customvalidator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:34:01.501588 customvalidator-0.4/customvalidator.egg-info/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 11:34:01.000000 customvalidator-0.4/customvalidator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 11:34:01.503602 customvalidator-0.4/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-04-17 11:33:48.000000 customvalidator-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.989221 customvalidator-0.5/
+-rw-rw-rw-   0        0        0       60 2023-04-17 11:45:30.988219 customvalidator-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.966874 customvalidator-0.5/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.5/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.968876 customvalidator-0.5/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.5/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.969877 customvalidator-0.5/customvalidator/
+-rw-rw-rw-   0        0        0     1353 2023-04-17 11:45:07.000000 customvalidator-0.5/customvalidator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.986221 customvalidator-0.5/customvalidator.egg-info/
+-rw-rw-rw-   0        0        0       60 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:45:30.989221 customvalidator-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-17 11:45:22.000000 customvalidator-0.5/setup.py
```

### Comparing `customvalidator-0.4/customdbcred/__init__.py` & `customvalidator-0.5/customdbcred/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.4/customstatuscodes/__init__.py` & `customvalidator-0.5/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.4/customvalidator/__init__.py` & `customvalidator-0.5/customvalidator/__init__.py`

 * *Files 20% similar despite different names*

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
+        output_json = dict(zip(['Status', 'Message'], [flag, 'schema validation done']))
+        return output_json
+    except Exception as ex:
+        logger_error.error(f"Exception Encountered Exception is : {ex}", exc_info=1)
+        output_json = dict(zip(['Status', 'Message'], [500, f"Exception encountered: {ex}"]))
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

