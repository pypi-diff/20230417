# Comparing `tmp/pymetdecoder-0.1.2.tar.gz` & `tmp/pymetdecoder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetdecoder-0.1.2.tar", last modified: Thu Jan 26 09:42:32 2023, max compression
+gzip compressed data, was "pymetdecoder-0.1.3.tar", last modified: Mon Apr 17 09:03:06 2023, max compression
```

## Comparing `pymetdecoder-0.1.2.tar` & `pymetdecoder-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-01-26 09:42:32.350116 pymetdecoder-0.1.2/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      356 2022-08-30 11:15:11.000000 pymetdecoder-0.1.2/LICENSE.md
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-01-26 09:42:32.350116 pymetdecoder-0.1.2/PKG-INFO
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     6625 2023-01-26 09:28:17.000000 pymetdecoder-0.1.2/README.md
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-01-26 09:42:32.346116 pymetdecoder-0.1.2/pymetdecoder/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    14534 2023-01-26 09:28:17.000000 pymetdecoder-0.1.2/pymetdecoder/__init__.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    39868 2023-01-26 09:28:17.000000 pymetdecoder-0.1.2/pymetdecoder/code_tables.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     5429 2022-08-30 11:15:11.000000 pymetdecoder-0.1.2/pymetdecoder/conversion.py
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-01-26 09:42:32.350116 pymetdecoder-0.1.2/pymetdecoder/synop/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    59831 2023-01-26 09:28:17.000000 pymetdecoder-0.1.2/pymetdecoder/synop/__init__.py
--rw-rw-r--   0 tdba      (1001) tdba      (1001)    57239 2023-01-26 09:28:17.000000 pymetdecoder-0.1.2/pymetdecoder/synop/observations.py
-drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-01-26 09:42:32.346116 pymetdecoder-0.1.2/pymetdecoder.egg-info/
--rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-01-26 09:42:32.000000 pymetdecoder-0.1.2/pymetdecoder.egg-info/PKG-INFO
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      319 2023-01-26 09:42:32.000000 pymetdecoder-0.1.2/pymetdecoder.egg-info/SOURCES.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)        1 2023-01-26 09:42:32.000000 pymetdecoder-0.1.2/pymetdecoder.egg-info/dependency_links.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)       13 2023-01-26 09:42:32.000000 pymetdecoder-0.1.2/pymetdecoder.egg-info/top_level.txt
--rw-rw-r--   0 tdba      (1001) tdba      (1001)       38 2023-01-26 09:42:32.350116 pymetdecoder-0.1.2/setup.cfg
--rw-rw-r--   0 tdba      (1001) tdba      (1001)      865 2023-01-26 09:30:31.000000 pymetdecoder-0.1.2/setup.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      356 2022-08-30 11:15:11.000000 pymetdecoder-0.1.3/LICENSE.md
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/PKG-INFO
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     6625 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/README.md
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    14250 2023-04-17 08:57:16.000000 pymetdecoder-0.1.3/pymetdecoder/__init__.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    39868 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/code_tables.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     5429 2022-08-30 11:15:11.000000 pymetdecoder-0.1.3/pymetdecoder/conversion.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder/synop/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    59831 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/synop/__init__.py
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)    57239 2023-01-26 09:28:17.000000 pymetdecoder-0.1.3/pymetdecoder/synop/observations.py
+drwxrwxr-x   0 tdba      (1001) tdba      (1001)        0 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/pymetdecoder.egg-info/
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)     7154 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/PKG-INFO
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      319 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)        1 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)       13 2023-04-17 09:03:06.000000 pymetdecoder-0.1.3/pymetdecoder.egg-info/top_level.txt
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)       38 2023-04-17 09:03:06.464609 pymetdecoder-0.1.3/setup.cfg
+-rw-rw-r--   0 tdba      (1001) tdba      (1001)      865 2023-04-17 08:57:16.000000 pymetdecoder-0.1.3/setup.py
```

### Comparing `pymetdecoder-0.1.2/PKG-INFO` & `pymetdecoder-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetdecoder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to decode/encode met reports e.g. SYNOPs
 Home-page: https://github.com/antarctica/pymetdecoder
 Author: Tim Barnes
 Author-email: tdba@bas.ac.uk
 License: Open Government License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymetdecoder-0.1.2/README.md` & `pymetdecoder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.2/pymetdecoder/__init__.py` & `pymetdecoder-0.1.3/pymetdecoder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 ################################################################################
 # pymetdecoder/__init__.py
 #
 # Main __init__ script for pymetdecoder
 #
 # TDBA 2019-01-16:
 #   * First version
+# TDBA 2023-04-14:
+#   * Removed logging configuration (#8)
 ################################################################################
 # IMPORTS
 ################################################################################
 import sys, json, logging, re
 from . import conversion
 ################################################################################
-# LOGGING
-################################################################################
-logging.basicConfig(
-    format   = "%(asctime)s [%(levelname)s] %(message)s",
-    level    = logging.INFO,
-    datefmt  = "%Y-%m-%d %H:%M:%S",
-    stream   = sys.stdout
-)
-################################################################################
 # EXCEPTION CLASSES
 ################################################################################
 class DecodeError(Exception):
     def __init__(self, msg):
         self.msg = msg
     def __str__(self):
         result = self.msg
```

### Comparing `pymetdecoder-0.1.2/pymetdecoder/code_tables.py` & `pymetdecoder-0.1.3/pymetdecoder/code_tables.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.2/pymetdecoder/conversion.py` & `pymetdecoder-0.1.3/pymetdecoder/conversion.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.2/pymetdecoder/synop/__init__.py` & `pymetdecoder-0.1.3/pymetdecoder/synop/__init__.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.2/pymetdecoder/synop/observations.py` & `pymetdecoder-0.1.3/pymetdecoder/synop/observations.py`

 * *Files identical despite different names*

### Comparing `pymetdecoder-0.1.2/pymetdecoder.egg-info/PKG-INFO` & `pymetdecoder-0.1.3/pymetdecoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetdecoder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to decode/encode met reports e.g. SYNOPs
 Home-page: https://github.com/antarctica/pymetdecoder
 Author: Tim Barnes
 Author-email: tdba@bas.ac.uk
 License: Open Government License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pymetdecoder-0.1.2/setup.py` & `pymetdecoder-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name             = "pymetdecoder",
-    version          = "0.1.2",
+    version          = "0.1.3",
     author           = "Tim Barnes",
     author_email     = "tdba@bas.ac.uk",
     description      = "Python module to decode/encode met reports e.g. SYNOPs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url              = "https://github.com/antarctica/pymetdecoder",
     license          = "Open Government License v3.0",
```

