# Comparing `tmp/fenjing-0.1.4.tar.gz` & `tmp/fenjing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.1.4.tar", last modified: Sun Apr 16 06:07:07 2023, max compression
+gzip compressed data, was "fenjing-0.1.5.tar", last modified: Mon Apr 17 05:46:04 2023, max compression
```

## Comparing `fenjing-0.1.4.tar` & `fenjing-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 06:07:07.382000 fenjing-0.1.4/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-16 06:07:07.381000 fenjing-0.1.4/PKG-INFO
--rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.1.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 06:07:07.380000 fenjing-0.1.4/fenjing/
--rwxr-x---   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 fenjing-0.1.4/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.4/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 fenjing-0.1.4/fenjing/cli.py
--rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.1.4/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.4/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2043 2023-04-02 06:07:31.000000 fenjing-0.1.4/fenjing/form.py
--rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.4/fenjing/int_vars.py
--rwxr-x---   0 user      (1000) user      (1000)    37000 2023-03-31 08:46:50.000000 fenjing-0.1.4/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 fenjing-0.1.4/fenjing/request.py
--rw-r--r--   0 user      (1000) user      (1000)      861 2023-04-16 05:52:32.000000 fenjing-0.1.4/fenjing/scan_url.py
--rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.4/fenjing/shell_cmd.py
--rw-r--r--   0 user      (1000) user      (1000)     3864 2023-04-16 05:52:36.000000 fenjing-0.1.4/fenjing/test_form.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-16 06:07:07.381000 fenjing-0.1.4/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-16 06:07:07.000000 fenjing-0.1.4/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-16 06:07:07.000000 fenjing-0.1.4/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-16 06:07:07.000000 fenjing-0.1.4/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-16 06:07:07.000000 fenjing-0.1.4/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-16 06:07:07.000000 fenjing-0.1.4/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-16 06:07:07.382000 fenjing-0.1.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.311000 fenjing-0.1.5/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.5/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:46:04.311000 fenjing-0.1.5/PKG-INFO
+-rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.1.5/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.307000 fenjing-0.1.5/fenjing/
+-rwxr-x---   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 fenjing-0.1.5/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.5/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 fenjing-0.1.5/fenjing/cli.py
+-rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.1.5/fenjing/example.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.5/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2043 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/form.py
+-rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.5/fenjing/int_vars.py
+-rwxr-x---   0 user      (1000) user      (1000)    37000 2023-03-31 08:46:50.000000 fenjing-0.1.5/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 fenjing-0.1.5/fenjing/request.py
+-rw-r--r--   0 user      (1000) user      (1000)      861 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/scan_url.py
+-rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.5/fenjing/shell_cmd.py
+-rw-r--r--   0 user      (1000) user      (1000)     3864 2023-04-17 05:43:42.000000 fenjing-0.1.5/fenjing/test_form.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 05:46:04.310000 fenjing-0.1.5/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-17 05:46:04.000000 fenjing-0.1.5/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-17 05:46:04.311000 fenjing-0.1.5/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.5/setup.py
```

### Comparing `fenjing-0.1.4/LICENSE` & `fenjing-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/PKG-INFO` & `fenjing-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.4/README.md` & `fenjing-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/cli.py` & `fenjing-0.1.5/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/example.py` & `fenjing-0.1.5/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/form.py` & `fenjing-0.1.5/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/int_vars.py` & `fenjing-0.1.5/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/pattern.py` & `fenjing-0.1.5/fenjing/pattern.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/request.py` & `fenjing-0.1.5/fenjing/request.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/scan_url.py` & `fenjing-0.1.5/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/shell_cmd.py` & `fenjing-0.1.5/fenjing/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing/test_form.py` & `fenjing-0.1.5/fenjing/test_form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.4/fenjing.egg-info/PKG-INFO` & `fenjing-0.1.5/fenjing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.4/setup.py` & `fenjing-0.1.5/setup.py`

 * *Files identical despite different names*

