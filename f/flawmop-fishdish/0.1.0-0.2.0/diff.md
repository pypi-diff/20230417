# Comparing `tmp/flawmop-fishdish-0.1.0.tar.gz` & `tmp/flawmop-fishdish-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flawmop-fishdish-0.1.0.tar", last modified: Fri Apr 14 18:48:05 2023, max compression
+gzip compressed data, was "flawmop-fishdish-0.2.0.tar", last modified: Sun Apr 16 22:37:47 2023, max compression
```

## Comparing `flawmop-fishdish-0.1.0.tar` & `flawmop-fishdish-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:48:05.000000 flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/src/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/src/sample/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:48:05.512655 flawmop-fishdish-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 18:47:55.000000 flawmop-fishdish-0.1.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 22:37:47.000000 flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:37:47.437191 flawmop-fishdish-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-16 22:37:37.000000 flawmop-fishdish-0.2.0/tests/test_simple.py
```

### Comparing `flawmop-fishdish-0.1.0/LICENSE.txt` & `flawmop-fishdish-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flawmop-fishdish-0.1.0/PKG-INFO` & `flawmop-fishdish-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flawmop-fishdish
-Version: 0.1.0
+Version: 0.2.0
 Summary: A sample fish dish project
 Author-email: flawmop <author@example.com>
 Maintainer-email: flawmop <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `flawmop-fishdish-0.1.0/README.md` & `flawmop-fishdish-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flawmop-fishdish-0.1.0/pyproject.toml` & `flawmop-fishdish-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "flawmop-fishdish"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.1.0"  # Required
+version = "0.2.0"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A sample fish dish project"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `flawmop-fishdish-0.1.0/src/flawmop_fishdish.egg-info/PKG-INFO` & `flawmop-fishdish-0.2.0/src/flawmop_fishdish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flawmop-fishdish
-Version: 0.1.0
+Version: 0.2.0
 Summary: A sample fish dish project
 Author-email: flawmop <author@example.com>
 Maintainer-email: flawmop <maintainer@example.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

