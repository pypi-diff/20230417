# Comparing `tmp/poutils-0.8.0.tar.gz` & `tmp/poutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/poutils-0.8.0.tar", last modified: Tue Sep 15 12:46:06 2020, max compression
+gzip compressed data, was "dist/poutils-0.9.0.tar", last modified: Thu Oct 15 16:58:40 2020, max compression
```

## Comparing `poutils-0.8.0.tar` & `poutils-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 seluj78    (501) staff       (20)        0 2020-09-15 12:46:06.210388 poutils-0.8.0/
--rw-r--r--   0 seluj78    (501) staff       (20)     1979 2020-09-15 12:46:06.210701 poutils-0.8.0/PKG-INFO
--rw-r--r--   0 seluj78    (501) staff       (20)      990 2019-12-11 15:46:40.000000 poutils-0.8.0/README.rst
-drwxr-xr-x   0 seluj78    (501) staff       (20)        0 2020-09-15 12:46:06.209461 poutils-0.8.0/poutils.egg-info/
--rw-r--r--   0 seluj78    (501) staff       (20)     1979 2020-09-15 12:46:06.000000 poutils-0.8.0/poutils.egg-info/PKG-INFO
--rw-r--r--   0 seluj78    (501) staff       (20)      209 2020-09-15 12:46:06.000000 poutils-0.8.0/poutils.egg-info/SOURCES.txt
--rw-r--r--   0 seluj78    (501) staff       (20)        1 2020-09-15 12:46:06.000000 poutils-0.8.0/poutils.egg-info/dependency_links.txt
--rw-r--r--   0 seluj78    (501) staff       (20)       86 2020-09-15 12:46:06.000000 poutils-0.8.0/poutils.egg-info/requires.txt
--rw-r--r--   0 seluj78    (501) staff       (20)        1 2020-09-15 12:46:06.000000 poutils-0.8.0/poutils.egg-info/top_level.txt
--rw-r--r--   0 seluj78    (501) staff       (20)        1 2019-11-25 21:04:42.000000 poutils-0.8.0/poutils.egg-info/zip-safe
--rw-r--r--   0 seluj78    (501) staff       (20)      753 2020-09-15 12:46:06.211824 poutils-0.8.0/setup.cfg
--rw-r--r--   0 seluj78    (501) staff       (20)       38 2019-11-25 20:59:05.000000 poutils-0.8.0/setup.py
+drwxr-xr-x   0 seluj78    (501) staff       (20)        0 2020-10-15 16:58:40.345692 poutils-0.9.0/
+-rw-r--r--   0 seluj78    (501) staff       (20)     1979 2020-10-15 16:58:40.345832 poutils-0.9.0/PKG-INFO
+-rw-r--r--   0 seluj78    (501) staff       (20)      990 2019-12-11 15:46:40.000000 poutils-0.9.0/README.rst
+drwxr-xr-x   0 seluj78    (501) staff       (20)        0 2020-10-15 16:58:40.344990 poutils-0.9.0/poutils.egg-info/
+-rw-r--r--   0 seluj78    (501) staff       (20)     1979 2020-10-15 16:58:40.000000 poutils-0.9.0/poutils.egg-info/PKG-INFO
+-rw-r--r--   0 seluj78    (501) staff       (20)      209 2020-10-15 16:58:40.000000 poutils-0.9.0/poutils.egg-info/SOURCES.txt
+-rw-r--r--   0 seluj78    (501) staff       (20)        1 2020-10-15 16:58:40.000000 poutils-0.9.0/poutils.egg-info/dependency_links.txt
+-rw-r--r--   0 seluj78    (501) staff       (20)       87 2020-10-15 16:58:40.000000 poutils-0.9.0/poutils.egg-info/requires.txt
+-rw-r--r--   0 seluj78    (501) staff       (20)        1 2020-10-15 16:58:40.000000 poutils-0.9.0/poutils.egg-info/top_level.txt
+-rw-r--r--   0 seluj78    (501) staff       (20)        1 2019-11-25 21:04:42.000000 poutils-0.9.0/poutils.egg-info/zip-safe
+-rw-r--r--   0 seluj78    (501) staff       (20)      754 2020-10-15 16:58:40.346464 poutils-0.9.0/setup.cfg
+-rw-r--r--   0 seluj78    (501) staff       (20)       38 2019-11-25 20:59:05.000000 poutils-0.9.0/setup.py
```

### Comparing `poutils-0.8.0/PKG-INFO` & `poutils-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: poutils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Gettext related tools: spellcheck, line wrapping etc...
 Home-page: https://github.com/seluj78/poutils
 Author: Jules Lasne
 Author-email: jules.lasne@gmail.com
 License: MIT
 Description: poutils
         =======
```

### Comparing `poutils-0.8.0/README.rst` & `poutils-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `poutils-0.8.0/poutils.egg-info/PKG-INFO` & `poutils-0.9.0/poutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: poutils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Gettext related tools: spellcheck, line wrapping etc...
 Home-page: https://github.com/seluj78/poutils
 Author: Jules Lasne
 Author-email: jules.lasne@gmail.com
 License: MIT
 Description: poutils
         =======
```

### Comparing `poutils-0.8.0/setup.cfg` & `poutils-0.9.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = poutils
 url = https://github.com/seluj78/poutils
-version = 0.8.0
+version = 0.9.0
 description = Gettext related tools: spellcheck, line wrapping etc...
 long_description = file: README.rst
 keywords = poutils, gettext, powrap, pospell, pogrep, potodo, pomerge, padpo
 license = MIT
 author = Jules Lasne
 author_email = jules.lasne@gmail.com
 classifiers = 
@@ -15,18 +15,18 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 
 [options]
 zip_safe = True
 include_package_data = True
 install_requires = 
-	powrap==0.3.2
-	pospell==1.0.5
+	powrap==0.3.3
+	pospell==1.0.11
 	pogrep==0.1.2
-	potodo==0.10.0
+	potodo==0.17.3
 	pomerge==0.1.4
 	padpo==0.9.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

