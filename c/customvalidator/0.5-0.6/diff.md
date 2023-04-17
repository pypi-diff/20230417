# Comparing `tmp/customvalidator-0.5.tar.gz` & `tmp/customvalidator-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customvalidator-0.5.tar", last modified: Mon Apr 17 11:45:30 2023, max compression
+gzip compressed data, was "customvalidator-0.6.tar", last modified: Mon Apr 17 13:38:21 2023, max compression
```

## Comparing `customvalidator-0.5.tar` & `customvalidator-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.989221 customvalidator-0.5/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:45:30.988219 customvalidator-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.966874 customvalidator-0.5/customdbcred/
--rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.5/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.968876 customvalidator-0.5/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.5/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.969877 customvalidator-0.5/customvalidator/
--rw-rw-rw-   0        0        0     1353 2023-04-17 11:45:07.000000 customvalidator-0.5/customvalidator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:45:30.986221 customvalidator-0.5/customvalidator.egg-info/
--rw-rw-rw-   0        0        0       60 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 11:45:30.000000 customvalidator-0.5/customvalidator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 11:45:30.989221 customvalidator-0.5/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-04-17 11:45:22.000000 customvalidator-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:38:21.210830 customvalidator-0.6/
+-rw-rw-rw-   0        0        0       60 2023-04-17 13:38:21.209829 customvalidator-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 13:38:21.190258 customvalidator-0.6/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.6/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:38:21.192250 customvalidator-0.6/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.6/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:38:21.193250 customvalidator-0.6/customvalidator/
+-rw-rw-rw-   0        0        0     1387 2023-04-17 13:34:13.000000 customvalidator-0.6/customvalidator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:38:21.208830 customvalidator-0.6/customvalidator.egg-info/
+-rw-rw-rw-   0        0        0       60 2023-04-17 13:38:21.000000 customvalidator-0.6/customvalidator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 13:38:21.000000 customvalidator-0.6/customvalidator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:38:21.000000 customvalidator-0.6/customvalidator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 13:38:21.000000 customvalidator-0.6/customvalidator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:38:21.210830 customvalidator-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-17 13:38:16.000000 customvalidator-0.6/setup.py
```

### Comparing `customvalidator-0.5/customdbcred/__init__.py` & `customvalidator-0.6/customdbcred/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.5/customstatuscodes/__init__.py` & `customvalidator-0.6/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.5/customvalidator/__init__.py` & `customvalidator-0.6/customvalidator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         errors = sorted(v.iter_errors(data), key=lambda e: e.path)
         for error in errors:
             logger.info('json validation failed')
             flag = 452
             output_json = dict(zip(['Status', 'Message'], [flag, error.message]))
             return output_json
         logger.info('schema validation done')
-        output_json = dict(zip(['Status', 'Message'], [flag, 'schema validation done']))
+        output_json = dict(zip(['Status', 'Message', 'Payload'], [flag, 'schema validation done', None]))
         return output_json
     except Exception as ex:
         logger_error.error(f"Exception Encountered Exception is : {ex}", exc_info=1)
-        output_json = dict(zip(['Status', 'Message'], [500, f"Exception encountered: {ex}"]))
+        output_json = dict(zip(['Status', 'Message', 'Payload'], [500, f"Exception encountered: {ex}", None]))
         return output_json
 
 
 def load(schema_path):
     """
     :param schema_path:
     :return:
```

