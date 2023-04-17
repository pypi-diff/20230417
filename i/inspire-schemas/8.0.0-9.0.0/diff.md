# Comparing `tmp/inspire-schemas-8.0.0.tar.gz` & `tmp/inspire-schemas-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspire-schemas-8.0.0.tar", last modified: Mon Jan 23 09:30:47 2017, max compression
+gzip compressed data, was "dist/inspire-schemas-9.0.0.tar", last modified: Mon Jan 23 09:31:35 2017, max compression
```

## Comparing `inspire-schemas-8.0.0.tar` & `inspire-schemas-9.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas/records/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/
--rw-r--r--   0 travis    (1000) travis    (1000)     1081 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      408 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/acquisition_source.json
--rw-r--r--   0 travis    (1000) travis    (1000)      894 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/address.json
--rw-r--r--   0 travis    (1000) travis    (1000)     3373 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/arxiv_categories.json
--rw-r--r--   0 travis    (1000) travis    (1000)      398 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/contact.json
--rw-r--r--   0 travis    (1000) travis    (1000)     3897 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/country_code.json
--rw-r--r--   0 travis    (1000) travis    (1000)     5616 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/id.json
--rw-r--r--   0 travis    (1000) travis    (1000)      937 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/inspire_field.json
--rw-r--r--   0 travis    (1000) travis    (1000)      288 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/json_reference.json
--rw-r--r--   0 travis    (1000) travis    (1000)      301 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/rank.json
--rw-r--r--   0 travis    (1000) travis    (1000)     4345 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/reference.json
--rw-r--r--   0 travis    (1000) travis    (1000)      281 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/title.json
--rw-r--r--   0 travis    (1000) travis    (1000)      253 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/elements/url.json
--rw-r--r--   0 travis    (1000) travis    (1000)     1030 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9712 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/authors.json
--rw-r--r--   0 travis    (1000) travis    (1000)     4098 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/conferences.json
--rw-r--r--   0 travis    (1000) travis    (1000)     7371 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/experiments.json
--rw-r--r--   0 travis    (1000) travis    (1000)    30617 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/hep.json
--rw-r--r--   0 travis    (1000) travis    (1000)     7789 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/institutions.json
--rw-r--r--   0 travis    (1000) travis    (1000)     4096 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/jobs.json
--rw-r--r--   0 travis    (1000) travis    (1000)     4736 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/records/journals.json
--rw-r--r--   0 travis    (1000) travis    (1000)     1052 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2304 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/api.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2030 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/errors.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2724 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/inspire_schemas/utils.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1002 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1318 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)       22 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       16 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/inspire_schemas.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      491 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/AUTHORS
--rw-r--r--   0 travis    (1000) travis    (1000)     7278 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/CHANGELOG
--rw-r--r--   0 travis    (1000) travis    (1000)       34 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     1919 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      966 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1692 2017-01-23 09:30:08.000000 inspire-schemas-8.0.0/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1002 2017-01-23 09:30:47.000000 inspire-schemas-8.0.0/PKG-INFO
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas/records/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1081 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      408 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/acquisition_source.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      894 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/address.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     3373 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/arxiv_categories.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      398 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/contact.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     3897 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/country_code.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     5616 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/id.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      937 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/inspire_field.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      288 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/json_reference.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      301 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/rank.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     4345 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/reference.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      281 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/title.json
+-rw-r--r--   0 travis    (1000) travis    (1000)      253 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/elements/url.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     1030 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9712 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/authors.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     4098 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/conferences.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     7371 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/experiments.json
+-rw-r--r--   0 travis    (1000) travis    (1000)    29502 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/hep.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     7789 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/institutions.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     4096 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/jobs.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     4736 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/records/journals.json
+-rw-r--r--   0 travis    (1000) travis    (1000)     1052 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2304 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/api.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2030 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/errors.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2724 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/inspire_schemas/utils.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1002 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1318 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (1000) travis    (1000)       22 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       16 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/inspire_schemas.egg-info/top_level.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      491 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/AUTHORS
+-rw-r--r--   0 travis    (1000) travis    (1000)     7471 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/CHANGELOG
+-rw-r--r--   0 travis    (1000) travis    (1000)       34 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     1919 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)      966 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1692 2017-01-23 09:30:39.000000 inspire-schemas-9.0.0/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1002 2017-01-23 09:31:35.000000 inspire-schemas-9.0.0/PKG-INFO
```

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/__init__.py` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/address.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/address.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/arxiv_categories.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/arxiv_categories.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/country_code.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/country_code.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/id.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/id.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/inspire_field.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/inspire_field.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/elements/reference.json` & `inspire-schemas-9.0.0/inspire_schemas/records/elements/reference.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/__init__.py` & `inspire-schemas-9.0.0/inspire_schemas/records/__init__.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/authors.json` & `inspire-schemas-9.0.0/inspire_schemas/records/authors.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/conferences.json` & `inspire-schemas-9.0.0/inspire_schemas/records/conferences.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/experiments.json` & `inspire-schemas-9.0.0/inspire_schemas/records/experiments.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/hep.json` & `inspire-schemas-9.0.0/inspire_schemas/records/hep.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977272727272727%*

 * *Differences: {"'properties'": "{delete: ['thesis_supervisors']}"}*

```diff
@@ -800,46 +800,14 @@
                         "type": "object"
                     },
                     "type": "array"
                 }
             },
             "type": "object"
         },
-        "thesis_supervisors": {
-            "items": {
-                "properties": {
-                    "affiliations": {
-                        "items": {
-                            "properties": {
-                                "curated_relation": {
-                                    "type": "boolean"
-                                },
-                                "record": {
-                                    "$ref": "elements/json_reference.json"
-                                },
-                                "value": {
-                                    "type": "string"
-                                }
-                            },
-                            "type": "object"
-                        },
-                        "type": "array"
-                    },
-                    "full_name": {
-                        "type": "string"
-                    }
-                },
-                "required": [
-                    "full_name"
-                ],
-                "type": "object"
-            },
-            "type": "array",
-            "uniqueItems": true
-        },
         "title_translations": {
             "items": {
                 "properties": {
                     "language": {
                         "format": "ISO 639-1",
                         "pattern": "\\w{2}",
                         "type": "string"
```

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/institutions.json` & `inspire-schemas-9.0.0/inspire_schemas/records/institutions.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/jobs.json` & `inspire-schemas-9.0.0/inspire_schemas/records/jobs.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/records/journals.json` & `inspire-schemas-9.0.0/inspire_schemas/records/journals.json`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/__init__.py` & `inspire-schemas-9.0.0/inspire_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/api.py` & `inspire-schemas-9.0.0/inspire_schemas/api.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/errors.py` & `inspire-schemas-9.0.0/inspire_schemas/errors.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas/utils.py` & `inspire-schemas-9.0.0/inspire_schemas/utils.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/inspire_schemas.egg-info/PKG-INFO` & `inspire-schemas-9.0.0/inspire_schemas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspire-schemas
-Version: 8.0.0
+Version: 9.0.0
 Summary: Inspire JSON schemas and utilities to use them.
 Home-page: https://github.com/inspirehep/inspire-schemas
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv2
 Description: UNKNOWN
 Platform: any
```

### Comparing `inspire-schemas-8.0.0/inspire_schemas.egg-info/SOURCES.txt` & `inspire-schemas-9.0.0/inspire_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/CHANGELOG` & `inspire-schemas-9.0.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+* 9.0.0 "Micha Moskovic <michamos@gmail.com>"
+    MAJOR f9169f0b: hep: thesis_supervisors superseded by inspire_roles
+    FIXED ISSUES: https://github.com/inspirehep/inspire-schemas/issues/60
+
 * 8.0.0 "Samuele Kaplun <Samuele.Kaplun@cern.ch>"
     MAJOR ec1cb438: Merge pull request #66 from kaplun/keywords
     MINOR 55b4397d: hep: merge classification_number into keywords
     FIXED ISSUES: https://github.com/inspirehep/inspire-schemas/issues/52
 
 * 7.0.1 "Samuele Kaplun <samuele.kaplun@cern.ch>"
     MINOR ee9f3b4d: .gitignore: add backup files
```

### Comparing `inspire-schemas-8.0.0/README.rst` & `inspire-schemas-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/setup.cfg` & `inspire-schemas-9.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/setup.py` & `inspire-schemas-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `inspire-schemas-8.0.0/PKG-INFO` & `inspire-schemas-9.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspire-schemas
-Version: 8.0.0
+Version: 9.0.0
 Summary: Inspire JSON schemas and utilities to use them.
 Home-page: https://github.com/inspirehep/inspire-schemas
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv2
 Description: UNKNOWN
 Platform: any
```

