# Comparing `tmp/hagis-0.2.3.tar.gz` & `tmp/hagis-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.2.3.tar", last modified: Mon Apr 17 13:03:42 2023, max compression
+gzip compressed data, was "hagis-0.2.4.tar", last modified: Mon Apr 17 13:06:02 2023, max compression
```

## Comparing `hagis-0.2.3.tar` & `hagis-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:03:42.981231 hagis-0.2.3/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:03:42.980236 hagis-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 13:03:42.969191 hagis-0.2.3/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.3/hagis/__init__.py
--rw-rw-rw-   0        0        0     9718 2023-04-17 13:01:15.000000 hagis-0.2.3/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:03:42.978231 hagis-0.2.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      941 2023-04-17 13:03:42.000000 hagis-0.2.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-17 13:03:42.000000 hagis-0.2.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:03:42.000000 hagis-0.2.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 13:03:42.000000 hagis-0.2.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-17 13:01:50.000000 hagis-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 13:03:42.982231 hagis-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.324439 hagis-0.2.4/
+-rw-rw-rw-   0        0        0      941 2023-04-17 13:06:02.322452 hagis-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-15 00:53:49.000000 hagis-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.309262 hagis-0.2.4/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.2.4/hagis/__init__.py
+-rw-rw-rw-   0        0        0     9714 2023-04-17 13:05:10.000000 hagis-0.2.4/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:06:02.318442 hagis-0.2.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      941 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 13:06:02.000000 hagis-0.2.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-17 13:05:17.000000 hagis-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:06:02.325441 hagis-0.2.4/setup.cfg
```

### Comparing `hagis-0.2.3/PKG-INFO` & `hagis-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.3/hagis/hagis.py` & `hagis-0.2.4/hagis/hagis.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         self._layer_url = layer_url
         self._model = model
         self._oid_field = oid_field
         self._shape_property_name = shape_property_name
         self._shape_property_type = None
         self._unknown_shape_types = [Any, object, SimpleNamespace]
         self._fields: Dict[str, str] = {}
-
         self.generate_token: Callable[[], str] = lambda: ""
-
         self._is_dynamic = model == SimpleNamespace
 
         if self._is_dynamic:
             return
         
         # List of custom mapping properties that have been handled.
         mapped: List[str] = []
```

### Comparing `hagis-0.2.3/hagis.egg-info/PKG-INFO` & `hagis-0.2.4/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.2.3/pyproject.toml` & `hagis-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

