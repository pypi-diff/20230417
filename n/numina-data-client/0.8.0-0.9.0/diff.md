# Comparing `tmp/numina-data-client-0.8.0.tar.gz` & `tmp/numina-data-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numina-data-client-0.8.0.tar", max compression
+gzip compressed data, was "numina-data-client-0.9.0.tar", max compression
```

## Comparing `numina-data-client-0.8.0.tar` & `numina-data-client-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2022-08-04 20:27:50.512582 numina-data-client-0.8.0/numina_data_client/__init__.py
--rw-r--r--   0        0        0     6014 2022-09-07 20:54:39.874300 numina-data-client-0.8.0/numina_data_client/client.py
--rw-r--r--   0        0        0     2102 2022-09-07 20:54:39.874417 numina-data-client-0.8.0/numina_data_client/constants.py
--rw-r--r--   0        0        0     1974 2022-08-03 20:46:30.250035 numina-data-client-0.8.0/numina_data_client/mutations.py
--rw-r--r--   0        0        0     4983 2022-08-03 20:46:30.250243 numina-data-client-0.8.0/numina_data_client/queries.py
--rw-r--r--   0        0        0       73 2022-08-03 20:46:30.250460 numina-data-client-0.8.0/numina_data_client/utils/__init__.py
--rw-r--r--   0        0        0     3161 2022-09-07 20:54:39.874647 numina-data-client-0.8.0/numina_data_client/utils/athena.py
--rw-r--r--   0        0        0    30168 2022-08-03 20:46:30.251006 numina-data-client-0.8.0/numina_data_client/utils/db.py
--rw-r--r--   0        0        0     1640 2022-08-03 20:46:30.251224 numina-data-client-0.8.0/numina_data_client/utils/frame.py
--rw-r--r--   0        0        0    16929 2022-09-07 20:54:39.874808 numina-data-client-0.8.0/numina_data_client/utils/img.py
--rw-r--r--   0        0        0     6513 2022-08-03 20:46:30.251678 numina-data-client-0.8.0/numina_data_client/utils/metrics.py
--rw-r--r--   0        0        0      599 2022-09-29 18:21:04.170141 numina-data-client-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      928 2022-09-29 18:21:07.801933 numina-data-client-0.8.0/setup.py
--rw-r--r--   0        0        0      828 2022-09-29 18:21:07.802091 numina-data-client-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-08-04 20:27:50.512582 numina-data-client-0.9.0/numina_data_client/__init__.py
+-rw-r--r--   0        0        0     6212 2022-10-04 00:05:43.595969 numina-data-client-0.9.0/numina_data_client/client.py
+-rw-r--r--   0        0        0     2102 2022-09-07 20:54:39.874417 numina-data-client-0.9.0/numina_data_client/constants.py
+-rw-r--r--   0        0        0     1974 2022-08-03 20:46:30.250035 numina-data-client-0.9.0/numina_data_client/mutations.py
+-rw-r--r--   0        0        0     4983 2022-08-03 20:46:30.250243 numina-data-client-0.9.0/numina_data_client/queries.py
+-rw-r--r--   0        0        0       73 2022-08-03 20:46:30.250460 numina-data-client-0.9.0/numina_data_client/utils/__init__.py
+-rw-r--r--   0        0        0     3161 2022-09-07 20:54:39.874647 numina-data-client-0.9.0/numina_data_client/utils/athena.py
+-rw-r--r--   0        0        0    30168 2022-08-03 20:46:30.251006 numina-data-client-0.9.0/numina_data_client/utils/db.py
+-rw-r--r--   0        0        0     1640 2022-08-03 20:46:30.251224 numina-data-client-0.9.0/numina_data_client/utils/frame.py
+-rw-r--r--   0        0        0    16929 2022-09-07 20:54:39.874808 numina-data-client-0.9.0/numina_data_client/utils/img.py
+-rw-r--r--   0        0        0     6513 2022-08-03 20:46:30.251678 numina-data-client-0.9.0/numina_data_client/utils/metrics.py
+-rw-r--r--   0        0        0      601 2022-10-04 00:05:43.597027 numina-data-client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      928 2022-10-04 00:07:29.584055 numina-data-client-0.9.0/setup.py
+-rw-r--r--   0        0        0      828 2022-10-04 00:07:29.584210 numina-data-client-0.9.0/PKG-INFO
```

### Comparing `numina-data-client-0.8.0/numina_data_client/client.py` & `numina-data-client-0.9.0/numina_data_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from graphql.language.ast import DocumentNode
 
 from . import constants
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
+# Requests logs the payload of every http call at the INFO level.
+# This is too verbose for our purposes, so we set the log level to WARNING.
+logging.getLogger("requests").setLevel(logging.WARNING)
 
 ###############################################################################
 
 
 class Auth(NamedTuple):
     expiration_dt: datetime
     token: str
```

### Comparing `numina-data-client-0.8.0/numina_data_client/constants.py` & `numina-data-client-0.9.0/numina_data_client/constants.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/mutations.py` & `numina-data-client-0.9.0/numina_data_client/mutations.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/queries.py` & `numina-data-client-0.9.0/numina_data_client/queries.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/utils/athena.py` & `numina-data-client-0.9.0/numina_data_client/utils/athena.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/utils/db.py` & `numina-data-client-0.9.0/numina_data_client/utils/db.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/utils/frame.py` & `numina-data-client-0.9.0/numina_data_client/utils/frame.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/utils/img.py` & `numina-data-client-0.9.0/numina_data_client/utils/img.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/numina_data_client/utils/metrics.py` & `numina-data-client-0.9.0/numina_data_client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `numina-data-client-0.8.0/pyproject.toml` & `numina-data-client-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numina-data-client"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = ["Numina Engineering <inquiries@numina.co>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 gql = "^3.4.0"
 pandas = "^1.4.3"
@@ -15,14 +15,14 @@
 Pillow = "^9.2.0"
 opencv-python-headless = "^4.6.0"
 boto3 = "^1.24.46"
 requests = "^2.28.1"
 requests-toolbelt = "^0.9.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
 black = "^22.6.0"
 pytest-raises = "^0.11"
+pytest = "^7.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `numina-data-client-0.8.0/setup.py` & `numina-data-client-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pyathena>=2.13.0,<3.0.0',
  'requests-toolbelt>=0.9.1,<0.10.0',
  'requests>=2.28.1,<3.0.0',
  'shapely>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'numina-data-client',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '',
     'long_description': None,
     'author': 'Numina Engineering',
     'author_email': 'inquiries@numina.co',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `numina-data-client-0.8.0/PKG-INFO` & `numina-data-client-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numina-data-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 Author: Numina Engineering
 Author-email: inquiries@numina.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

