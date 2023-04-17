# Comparing `tmp/c8connector-0.0.8.tar.gz` & `tmp/c8connector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c8connector-0.0.8.tar", last modified: Wed Nov  2 09:10:31 2022, max compression
+gzip compressed data, was "c8connector-0.0.9.tar", last modified: Thu Nov  3 04:37:50 2022, max compression
```

## Comparing `c8connector-0.0.8.tar` & `c8connector-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:10:31.221792 c8connector-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-11-02 09:10:08.000000 c8connector-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-11-02 09:10:31.221792 c8connector-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-11-02 09:10:08.000000 c8connector-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:10:31.217792 c8connector-0.0.8/c8connector/
--rw-r--r--   0 runner    (1001) docker     (121)     3595 2022-11-02 09:10:08.000000 c8connector-0.0.8/c8connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 09:10:31.221792 c8connector-0.0.8/c8connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-11-02 09:10:31.000000 c8connector-0.0.8/c8connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-02 09:10:31.000000 c8connector-0.0.8/c8connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 09:10:31.000000 c8connector-0.0.8/c8connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-02 09:10:31.000000 c8connector-0.0.8/c8connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-02 09:10:08.000000 c8connector-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-02 09:10:31.221792 c8connector-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 04:37:50.865917 c8connector-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-11-03 04:37:30.000000 c8connector-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-11-03 04:37:50.865917 c8connector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-11-03 04:37:30.000000 c8connector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 04:37:50.865917 c8connector-0.0.9/c8connector/
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2022-11-03 04:37:30.000000 c8connector-0.0.9/c8connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 04:37:50.865917 c8connector-0.0.9/c8connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14587 2022-11-03 04:37:50.000000 c8connector-0.0.9/c8connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-03 04:37:50.000000 c8connector-0.0.9/c8connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 04:37:50.000000 c8connector-0.0.9/c8connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-03 04:37:50.000000 c8connector-0.0.9/c8connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-03 04:37:31.000000 c8connector-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-03 04:37:50.865917 c8connector-0.0.9/setup.cfg
```

### Comparing `c8connector-0.0.8/LICENSE` & `c8connector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `c8connector-0.0.8/PKG-INFO` & `c8connector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: C8 Connector Interface
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `c8connector-0.0.8/README.md` & `c8connector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `c8connector-0.0.8/c8connector/__init__.py` & `c8connector-0.0.9/c8connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,14 @@
         self.type = type
         self.is_mandatory = is_mandatory
         self.is_dynamic = is_dynamic
         self.description = description
         self.example = example
 
 
-class Sample:
-    """C8Connector Sample"""
-
-    def __init__(self, stream: dict, data: list):
-        self.stream = stream
-        self.data = data
-
-
 class Attribute:
     """C8Connector Attribute"""
 
     def __init__(self, name: str, type: AttributeType):
         self.name = name
         self.type = type
 
@@ -46,14 +38,22 @@
     """C8Connector Schema"""
 
     def __init__(self, name: str, attributes: list[Attribute]):
         self.name = name
         self.attributes = attributes
 
 
+class Sample:
+    """C8Connector Sample"""
+
+    def __init__(self, schema: Schema, data: list[dict]):
+        self.schema = schema
+        self.data = data
+
+
 class C8ConnectorMeta(type):
     """C8Connector metaclass"""
 
     def __instancecheck__(cls, instance):
         return cls.__subclasscheck__(type(instance))
 
     def __subclasscheck__(cls, subclass):
```

### Comparing `c8connector-0.0.8/c8connector.egg-info/PKG-INFO` & `c8connector-0.0.9/c8connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: C8 Connector Interface
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `c8connector-0.0.8/pyproject.toml` & `c8connector-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "c8connector"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "C8 Connector Interface"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

