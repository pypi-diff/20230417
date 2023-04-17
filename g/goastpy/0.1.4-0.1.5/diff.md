# Comparing `tmp/goastpy-0.1.4.tar.gz` & `tmp/goastpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.4.tar", last modified: Mon Apr 17 08:15:52 2023, max compression
+gzip compressed data, was "goastpy-0.1.5.tar", last modified: Mon Apr 17 08:31:28 2023, max compression
```

## Comparing `goastpy-0.1.4.tar` & `goastpy-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:15:52.117272 goastpy-0.1.4/
--rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.4/LICENSE
--rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 08:15:52.117355 goastpy-0.1.4/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.4/README.md
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:15:52.116426 goastpy-0.1.4/goastpy/
--rw-r--r--   0 monolite   (502) staff       (20)       27 2023-04-16 13:44:10.000000 goastpy-0.1.4/goastpy/__init__.py
--rw-r--r--   0 monolite   (502) staff       (20)     3298 2023-04-17 07:48:55.000000 goastpy-0.1.4/goastpy/goastparser_wrapper.py
--rw-r--r--   0 monolite   (502) staff       (20)      687 2023-04-16 13:44:59.000000 goastpy-0.1.4/goastpy/goastpy.py
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:15:52.117142 goastpy-0.1.4/goastpy.egg-info/
--rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 08:15:52.000000 goastpy-0.1.4/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)      236 2023-04-17 08:15:52.000000 goastpy-0.1.4/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-17 08:15:52.000000 goastpy-0.1.4/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 monolite   (502) staff       (20)        8 2023-04-17 08:15:52.000000 goastpy-0.1.4/goastpy.egg-info/top_level.txt
--rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-17 08:15:52.117709 goastpy-0.1.4/setup.cfg
--rw-r--r--   0 monolite   (502) staff       (20)     1078 2023-04-17 08:15:46.000000 goastpy-0.1.4/setup.py
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:31:28.954026 goastpy-0.1.5/
+-rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.5/LICENSE
+-rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 08:31:28.954114 goastpy-0.1.5/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.5/README.md
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:31:28.952368 goastpy-0.1.5/goastpy/
+-rw-r--r--   0 monolite   (502) staff       (20)       27 2023-04-16 13:44:10.000000 goastpy-0.1.5/goastpy/__init__.py
+-rw-r--r--   0 monolite   (502) staff       (20)     1688 2023-04-16 11:49:12.000000 goastpy-0.1.5/goastpy/goastparser.h
+-rw-r--r--   0 monolite   (502) staff       (20)  2831794 2023-04-16 11:49:12.000000 goastpy-0.1.5/goastpy/goastparser.so
+-rw-r--r--   0 monolite   (502) staff       (20)     3298 2023-04-17 07:48:55.000000 goastpy-0.1.5/goastpy/goastparser_wrapper.py
+-rw-r--r--   0 monolite   (502) staff       (20)      687 2023-04-16 13:44:59.000000 goastpy-0.1.5/goastpy/goastpy.py
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 08:31:28.953904 goastpy-0.1.5/goastpy.egg-info/
+-rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 08:31:28.000000 goastpy-0.1.5/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)      285 2023-04-17 08:31:28.000000 goastpy-0.1.5/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-17 08:31:28.000000 goastpy-0.1.5/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        8 2023-04-17 08:31:28.000000 goastpy-0.1.5/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-17 08:31:28.954501 goastpy-0.1.5/setup.cfg
+-rw-r--r--   0 monolite   (502) staff       (20)     1179 2023-04-17 08:31:02.000000 goastpy-0.1.5/setup.py
```

### Comparing `goastpy-0.1.4/LICENSE` & `goastpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.4/PKG-INFO` & `goastpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `goastpy-0.1.4/goastpy/goastparser_wrapper.py` & `goastpy-0.1.5/goastpy/goastparser_wrapper.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.4/goastpy/goastpy.py` & `goastpy-0.1.5/goastpy/goastpy.py`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.4/goastpy.egg-info/PKG-INFO` & `goastpy-0.1.5/goastpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

