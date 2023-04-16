# Comparing `tmp/marqo-0.9.2.tar.gz` & `tmp/marqo-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-0.9.2.tar", last modified: Fri Apr 14 06:08:25 2023, max compression
+gzip compressed data, was "marqo-0.9.3.tar", last modified: Sun Apr 16 23:54:06 2023, max compression
```

## Comparing `marqo-0.9.2.tar` & `marqo-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.529800 marqo-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-14 06:08:15.000000 marqo-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-14 06:08:25.529800 marqo-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-14 06:08:15.000000 marqo-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 06:08:15.000000 marqo-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:08:25.529800 marqo-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-14 06:08:15.000000 marqo-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.521799 marqo-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.525800 marqo-0.9.2/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.529800 marqo-0.9.2/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:54:06.419959 marqo-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-16 23:53:54.000000 marqo-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-16 23:54:06.419959 marqo-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-16 23:53:54.000000 marqo-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-16 23:53:54.000000 marqo-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 23:54:06.419959 marqo-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 23:53:54.000000 marqo-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:54:06.415959 marqo-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:54:06.419959 marqo-0.9.3/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-16 23:53:54.000000 marqo-0.9.3/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:54:06.419959 marqo-0.9.3/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-16 23:54:06.000000 marqo-0.9.3/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-16 23:54:06.000000 marqo-0.9.3/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:54:06.000000 marqo-0.9.3/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-16 23:54:06.000000 marqo-0.9.3/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 23:54:06.000000 marqo-0.9.3/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-0.9.2/LICENSE` & `marqo-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/PKG-INFO` & `marqo-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.2 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.3 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
                                     [Marqo]
```

### Comparing `marqo-0.9.2/README.md` & `marqo-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/setup.py` & `marqo-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "pydantic"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="0.9.2",
+    version="0.9.3",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-0.9.2/src/marqo/_httprequests.py` & `marqo-0.9.3/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/client.py` & `marqo-0.9.3/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/config.py` & `marqo-0.9.3/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/defaults.py` & `marqo-0.9.3/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/errors.py` & `marqo-0.9.3/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/index.py` & `marqo-0.9.3/src/marqo/index.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/models.py` & `marqo-0.9.3/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.2/src/marqo/utils.py` & `marqo-0.9.3/src/marqo/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Args:
         query_param: query parameter
         x: List of values for the query parameter. 
 
     Returns:
         A rendered query string for the given parameter and parameter value.
     """
-    return "&".join([f"{query_param}={str(xx)}" for xx in x])
+    return "&".join([f"{query_param}={urllib.parse.quote_plus(str(xx))}" for xx in x])
 
 
 def convert_dict_to_url_params(d: dict) -> str:
     """Converts a dict into a url-encoded string that can be appended as a query_param
     Args:
         d: dict to be converted
```

### Comparing `marqo-0.9.2/src/marqo.egg-info/PKG-INFO` & `marqo-0.9.3/src/marqo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.2 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.3 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
                                     [Marqo]
```

