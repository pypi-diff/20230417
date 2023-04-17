# Comparing `tmp/icap_commons-0.2.0.tar.gz` & `tmp/icap_commons-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icap_commons-0.2.0.tar", last modified: Mon Apr 17 10:38:25 2023, max compression
+gzip compressed data, was "icap_commons-0.3.0.tar", last modified: Mon Apr 17 10:42:30 2023, max compression
```

## Comparing `icap_commons-0.2.0.tar` & `icap_commons-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:38:25.614405 icap_commons-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-17 10:38:25.613488 icap_commons-0.2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:38:25.611655 icap_commons-0.2.0/icap_commons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 10:38:09.000000 icap_commons-0.2.0/icap_commons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-17 10:38:09.000000 icap_commons-0.2.0/icap_commons/gcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:38:25.613488 icap_commons-0.2.0/icap_commons.egg-info/
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-17 10:38:25.000000 icap_commons-0.2.0/icap_commons.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-17 10:38:25.000000 icap_commons-0.2.0/icap_commons.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:38:25.000000 icap_commons-0.2.0/icap_commons.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 10:38:25.000000 icap_commons-0.2.0/icap_commons.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-17 10:38:09.000000 icap_commons-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:38:25.614405 icap_commons-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-04-17 10:38:09.000000 icap_commons-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:42:30.985393 icap_commons-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-17 10:42:30.985393 icap_commons-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:42:30.983562 icap_commons-0.3.0/icap_commons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 10:42:17.000000 icap_commons-0.3.0/icap_commons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-17 10:42:17.000000 icap_commons-0.3.0/icap_commons/gcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:42:30.984478 icap_commons-0.3.0/icap_commons.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-17 10:42:30.000000 icap_commons-0.3.0/icap_commons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-17 10:42:30.000000 icap_commons-0.3.0/icap_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:42:30.000000 icap_commons-0.3.0/icap_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 10:42:30.000000 icap_commons-0.3.0/icap_commons.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-17 10:42:17.000000 icap_commons-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:42:30.985393 icap_commons-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-04-17 10:42:17.000000 icap_commons-0.3.0/setup.py
```

### Comparing `icap_commons-0.2.0/PKG-INFO` & `icap_commons-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icap_commons
-Version: 0.2.0
+Version: 0.3.0
 Summary: Example Python library
 Author: Makrand Bhonde
 Author-email: makrand.bhonde@bluealtair.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `icap_commons-0.2.0/icap_commons/gcp.py` & `icap_commons-0.3.0/icap_commons/gcp.py`

 * *Files identical despite different names*

### Comparing `icap_commons-0.2.0/icap_commons.egg-info/PKG-INFO` & `icap_commons-0.3.0/icap_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icap-commons
-Version: 0.2.0
+Version: 0.3.0
 Summary: Example Python library
 Author: Makrand Bhonde
 Author-email: makrand.bhonde@bluealtair.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `icap_commons-0.2.0/setup.py` & `icap_commons-0.3.0/setup.py`

 * *Files identical despite different names*

