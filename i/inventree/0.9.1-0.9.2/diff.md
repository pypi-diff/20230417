# Comparing `tmp/inventree-0.9.1.tar.gz` & `tmp/inventree-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventree-0.9.1.tar", last modified: Sun Dec  4 13:09:30 2022, max compression
+gzip compressed data, was "inventree-0.9.2.tar", last modified: Mon Dec 12 21:11:04 2022, max compression
```

## Comparing `inventree-0.9.1.tar` & `inventree-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 13:09:30.193139 inventree-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-04 13:09:14.000000 inventree-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-04 13:09:30.193139 inventree-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-04 13:09:14.000000 inventree-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 13:09:30.189139 inventree-0.9.1/inventree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17192 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/part.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2022-12-04 13:09:14.000000 inventree-0.9.1/inventree/stock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 13:09:30.189139 inventree-0.9.1/inventree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-04 13:09:30.000000 inventree-0.9.1/inventree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-04 13:09:30.000000 inventree-0.9.1/inventree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 13:09:30.000000 inventree-0.9.1/inventree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-04 13:09:30.000000 inventree-0.9.1/inventree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-04 13:09:30.000000 inventree-0.9.1/inventree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-04 13:09:30.193139 inventree-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-04 13:09:14.000000 inventree-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 13:09:30.193139 inventree-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_company.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_internal_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    22848 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_part.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2022-12-04 13:09:14.000000 inventree-0.9.1/test/test_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 21:11:04.028366 inventree-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-12 21:10:48.000000 inventree-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-12 21:11:04.028366 inventree-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-12 21:10:48.000000 inventree-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 21:11:04.028366 inventree-0.9.2/inventree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17192 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-12 21:10:48.000000 inventree-0.9.2/inventree/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 21:11:04.028366 inventree-0.9.2/inventree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2022-12-12 21:11:03.000000 inventree-0.9.2/inventree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2022-12-12 21:11:04.000000 inventree-0.9.2/inventree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 21:11:03.000000 inventree-0.9.2/inventree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-12 21:11:03.000000 inventree-0.9.2/inventree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-12 21:11:03.000000 inventree-0.9.2/inventree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-12 21:11:04.032366 inventree-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2022-12-12 21:10:48.000000 inventree-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 21:11:04.028366 inventree-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8779 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_internal_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2022-12-12 21:10:48.000000 inventree-0.9.2/test/test_stock.py
```

### Comparing `inventree-0.9.1/LICENSE` & `inventree-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/PKG-INFO` & `inventree-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python interface for InvenTree inventory management system
 Home-page: https://github.com/inventree/inventree-python/
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: bom,bill of materials,stock,inventory,management,barcode
 Requires-Python: >=3.8
```

### Comparing `inventree-0.9.1/README.md` & `inventree-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/api.py` & `inventree-0.9.2/inventree/api.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/base.py` & `inventree-0.9.2/inventree/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import logging
 import json
 
 from . import api as inventree_api
 
 
-INVENTREE_PYTHON_VERSION = "0.9.1"
+INVENTREE_PYTHON_VERSION = "0.9.2"
 
 
 logger = logging.getLogger('inventree')
 
 
 class InventreeObject(object):
     """ Base class for an InvenTree object """
```

### Comparing `inventree-0.9.1/inventree/build.py` & `inventree-0.9.2/inventree/build.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/company.py` & `inventree-0.9.2/inventree/company.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/label.py` & `inventree-0.9.2/inventree/label.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/order.py` & `inventree-0.9.2/inventree/order.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/part.py` & `inventree-0.9.2/inventree/part.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree/stock.py` & `inventree-0.9.2/inventree/stock.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/inventree.egg-info/PKG-INFO` & `inventree-0.9.2/inventree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python interface for InvenTree inventory management system
 Home-page: https://github.com/inventree/inventree-python/
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: bom,bill of materials,stock,inventory,management,barcode
 Requires-Python: >=3.8
```

### Comparing `inventree-0.9.1/inventree.egg-info/SOURCES.txt` & `inventree-0.9.2/inventree.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 inventree/base.py
 inventree/build.py
 inventree/company.py
 inventree/label.py
 inventree/order.py
 inventree/part.py
 inventree/stock.py
+inventree/user.py
 inventree.egg-info/PKG-INFO
 inventree.egg-info/SOURCES.txt
 inventree.egg-info/dependency_links.txt
 inventree.egg-info/requires.txt
 inventree.egg-info/top_level.txt
 test/test_api.py
 test/test_base.py
```

### Comparing `inventree-0.9.1/setup.py` & `inventree-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_api.py` & `inventree-0.9.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_base.py` & `inventree-0.9.2/test/test_base.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_build.py` & `inventree-0.9.2/test/test_build.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_company.py` & `inventree-0.9.2/test/test_company.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_internal_price.py` & `inventree-0.9.2/test/test_internal_price.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_label.py` & `inventree-0.9.2/test/test_label.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_order.py` & `inventree-0.9.2/test/test_order.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_part.py` & `inventree-0.9.2/test/test_part.py`

 * *Files identical despite different names*

### Comparing `inventree-0.9.1/test/test_stock.py` & `inventree-0.9.2/test/test_stock.py`

 * *Files identical despite different names*

