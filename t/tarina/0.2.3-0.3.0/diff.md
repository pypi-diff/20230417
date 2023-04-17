# Comparing `tmp/tarina-0.2.3.tar.gz` & `tmp/tarina-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.2.3.tar", last modified: Wed Apr 12 14:50:05 2023, max compression
+gzip compressed data, was "tarina-0.3.0.tar", last modified: Mon Apr 17 05:31:24 2023, max compression
```

## Comparing `tarina-0.2.3.tar` & `tarina-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 14:49:48.000000 tarina-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 14:49:48.000000 tarina-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:50:05.516930 tarina-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 14:49:48.000000 tarina-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 14:49:48.000000 tarina-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:50:05.516930 tarina-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-12 14:49:48.000000 tarina-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.512930 tarina-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (123)   200403 2023-04-12 14:49:56.000000 tarina-0.2.3/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 14:49:48.000000 tarina-0.2.3/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:50:05.516930 tarina-0.2.3/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 14:50:05.000000 tarina-0.2.3/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-17 05:31:07.000000 tarina-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 05:31:07.000000 tarina-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:31:24.729679 tarina-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 05:31:07.000000 tarina-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 05:31:07.000000 tarina-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:31:24.729679 tarina-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-17 05:31:07.000000 tarina-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.725679 tarina-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (123)   200403 2023-04-17 05:31:16.000000 tarina-0.3.0/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/guard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/en-US.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/i18n/zh-CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-17 05:31:07.000000 tarina-0.3.0/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:31:24.729679 tarina-0.3.0/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 05:31:24.000000 tarina-0.3.0/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.2.3/LICENSE` & `tarina-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/PKG-INFO` & `tarina-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.3
+Version: 0.3.0
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.3/pyproject.toml` & `tarina-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.2.3"
+version = "0.3.0"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.2.3/setup.py` & `tarina-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_lru_c.c` & `tarina-0.3.0/src/tarina/_lru_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_lru_c.pyi` & `tarina-0.3.0/src/tarina/_lru_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_lru_py.py` & `tarina-0.3.0/src/tarina/_lru_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_op.h` & `tarina-0.3.0/src/tarina/_op.h`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_string_c.c` & `tarina-0.3.0/src/tarina/_string_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_string_c.pyi` & `tarina-0.3.0/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_string_c.pyx` & `tarina-0.3.0/src/tarina/_string_c.pyx`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/_string_py.py` & `tarina-0.3.0/src/tarina/_string_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/context.py` & `tarina-0.3.0/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/generic.py` & `tarina-0.3.0/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/guard.py` & `tarina-0.3.0/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/lru.pyi` & `tarina-0.3.0/src/tarina/lru.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/signature.py` & `tarina-0.3.0/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/string.py` & `tarina-0.3.0/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina/tools.py` & `tarina-0.3.0/src/tarina/tools.py`

 * *Files identical despite different names*

### Comparing `tarina-0.2.3/src/tarina.egg-info/PKG-INFO` & `tarina-0.3.0/src/tarina.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.2.3
+Version: 0.3.0
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tarina-0.2.3/src/tarina.egg-info/SOURCES.txt` & `tarina-0.3.0/src/tarina.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 src/tarina/_string_c.pyi
 src/tarina/_string_c.pyx
 src/tarina/_string_py.py
 src/tarina/const.py
 src/tarina/context.py
 src/tarina/generic.py
 src/tarina/guard.py
+src/tarina/lang.py
 src/tarina/lru.py
 src/tarina/lru.pyi
 src/tarina/signature.py
 src/tarina/string.py
 src/tarina/tools.py
 src/tarina.egg-info/PKG-INFO
 src/tarina.egg-info/SOURCES.txt
 src/tarina.egg-info/dependency_links.txt
 src/tarina.egg-info/requires.txt
-src/tarina.egg-info/top_level.txt
+src/tarina.egg-info/top_level.txt
+src/tarina/i18n/.config.json
+src/tarina/i18n/en-US.json
+src/tarina/i18n/zh-CN.json
```

