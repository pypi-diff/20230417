# Comparing `tmp/spleaf-2.1.3.tar.gz` & `tmp/spleaf-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spleaf-2.1.3.tar", last modified: Sat Apr 15 23:03:49 2023, max compression
+gzip compressed data, was "spleaf-2.1.4.tar", last modified: Mon Apr 17 15:17:13 2023, max compression
```

## Comparing `spleaf-2.1.3.tar` & `spleaf-2.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-15 23:02:33.000000 spleaf-2.1.3/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-15 23:02:33.000000 spleaf-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-15 23:03:49.022904 spleaf-2.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-15 23:02:33.000000 spleaf-2.1.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 23:03:49.022904 spleaf-2.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-15 23:02:33.000000 spleaf-2.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.021904 spleaf-2.1.3/spleaf/
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/__info__.py
--rw-rw-rw-   0 root         (0) root         (0)    29194 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16971 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/cov.py
--rw-rw-rw-   0 root         (0) root         (0)    49962 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/fenrir.py
--rw-rw-rw-   0 root         (0) root         (0)    30205 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/libspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)     4571 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/libspleaf.h
--rw-rw-rw-   0 root         (0) root         (0)    61577 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/pywrapspleaf.c
--rw-rw-rw-   0 root         (0) root         (0)    82399 2023-04-15 23:02:33.000000 spleaf-2.1.3/spleaf/term.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/spleaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      802 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-15 23:03:48.000000 spleaf-2.1.3/spleaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 23:03:49.022904 spleaf-2.1.3/test/
--rw-rw-rw-   0 root         (0) root         (0)    27167 2023-04-15 23:02:33.000000 spleaf-2.1.3/test/test_cov.py
--rw-rw-rw-   0 root         (0) root         (0)    11276 2023-04-15 23:02:33.000000 spleaf-2.1.3/test/test_spleaf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:17:13.362027 spleaf-2.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-17 15:15:56.000000 spleaf-2.1.4/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-17 15:15:56.000000 spleaf-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-17 15:17:13.362027 spleaf-2.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-17 15:15:56.000000 spleaf-2.1.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:17:13.363027 spleaf-2.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-04-17 15:15:56.000000 spleaf-2.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:17:13.361027 spleaf-2.1.4/spleaf/
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/__info__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29194 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16971 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    49962 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/fenrir.py
+-rw-rw-rw-   0 root         (0) root         (0)    30205 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/libspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)     4571 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/libspleaf.h
+-rw-rw-rw-   0 root         (0) root         (0)    61577 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/pywrapspleaf.c
+-rw-rw-rw-   0 root         (0) root         (0)    82399 2023-04-17 15:15:56.000000 spleaf-2.1.4/spleaf/term.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:17:13.362027 spleaf-2.1.4/spleaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-04-17 15:17:13.000000 spleaf-2.1.4/spleaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-17 15:17:13.000000 spleaf-2.1.4/spleaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:17:13.000000 spleaf-2.1.4/spleaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-17 15:17:13.000000 spleaf-2.1.4/spleaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-17 15:17:13.000000 spleaf-2.1.4/spleaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:17:13.362027 spleaf-2.1.4/test/
+-rw-rw-rw-   0 root         (0) root         (0)    27167 2023-04-17 15:15:56.000000 spleaf-2.1.4/test/test_cov.py
+-rw-rw-rw-   0 root         (0) root         (0)    11276 2023-04-17 15:15:56.000000 spleaf-2.1.4/test/test_spleaf.py
```

### Comparing `spleaf-2.1.3/COPYING` & `spleaf-2.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/PKG-INFO` & `spleaf-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.3
+Version: 2.1.4
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.3/README.rst` & `spleaf-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/setup.py` & `spleaf-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/__info__.py` & `spleaf-2.1.4/spleaf/__info__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 __title__ = 'spleaf'
 __description__ = 'Symmetric S+LEAF matrix.'
 __author__ = 'Jean-Baptiste Delisle'
 __author_email__ = 'jean-baptiste.delisle@unige.ch'
 __license__ = 'GPLv3'
 __url__ = 'https://gitlab.unige.ch/jean-baptiste.delisle/spleaf'
-__version__ = "2.1.3"
+__version__ = "2.1.4"
```

### Comparing `spleaf-2.1.3/spleaf/__init__.py` & `spleaf-2.1.4/spleaf/__init__.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/cov.py` & `spleaf-2.1.4/spleaf/cov.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/fenrir.py` & `spleaf-2.1.4/spleaf/fenrir.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/libspleaf.c` & `spleaf-2.1.4/spleaf/libspleaf.c`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/libspleaf.h` & `spleaf-2.1.4/spleaf/libspleaf.h`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/pywrapspleaf.c` & `spleaf-2.1.4/spleaf/pywrapspleaf.c`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf/term.py` & `spleaf-2.1.4/spleaf/term.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/spleaf.egg-info/PKG-INFO` & `spleaf-2.1.4/spleaf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spleaf
-Version: 2.1.3
+Version: 2.1.4
 Summary: Symmetric S+LEAF matrix.
 Home-page: https://gitlab.unige.ch/jean-baptiste.delisle/spleaf
 Author: Jean-Baptiste Delisle
 Author-email: jean-baptiste.delisle@unige.ch
 License: GPLv3
 Requires-Python: >=3.6
 License-File: COPYING
```

### Comparing `spleaf-2.1.3/test/test_cov.py` & `spleaf-2.1.4/test/test_cov.py`

 * *Files identical despite different names*

### Comparing `spleaf-2.1.3/test/test_spleaf.py` & `spleaf-2.1.4/test/test_spleaf.py`

 * *Files identical despite different names*

