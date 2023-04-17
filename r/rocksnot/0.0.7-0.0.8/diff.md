# Comparing `tmp/rocksnot-0.0.7.tar.gz` & `tmp/rocksnot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocksnot-0.0.7.tar", last modified: Mon Apr 10 17:48:24 2023, max compression
+gzip compressed data, was "rocksnot-0.0.8.tar", last modified: Mon Apr 17 20:40:17 2023, max compression
```

## Comparing `rocksnot-0.0.7.tar` & `rocksnot-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-10 17:48:16.000000 rocksnot-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 17:48:16.000000 rocksnot-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-10 17:48:24.229576 rocksnot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-10 17:48:16.000000 rocksnot-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-10 17:48:16.000000 rocksnot-0.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/rocksnot/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-10 17:48:16.000000 rocksnot-0.0.7/rocksnot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-10 17:48:16.000000 rocksnot-0.0.7/rocksnot/rocksnot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:48:24.225576 rocksnot-0.0.7/rocksnot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 17:48:24.000000 rocksnot-0.0.7/rocksnot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 17:48:24.229576 rocksnot-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-10 17:48:16.000000 rocksnot-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:40:17.022384 rocksnot-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 20:40:05.000000 rocksnot-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 20:40:05.000000 rocksnot-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-17 20:40:17.022384 rocksnot-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-17 20:40:05.000000 rocksnot-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 20:40:05.000000 rocksnot-0.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:40:17.022384 rocksnot-0.0.8/rocksnot/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 20:40:05.000000 rocksnot-0.0.8/rocksnot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-17 20:40:05.000000 rocksnot-0.0.8/rocksnot/foliumrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-17 20:40:05.000000 rocksnot-0.0.8/rocksnot/rocksnot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:40:17.022384 rocksnot-0.0.8/rocksnot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 20:40:16.000000 rocksnot-0.0.8/rocksnot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 20:40:17.026383 rocksnot-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 20:40:05.000000 rocksnot-0.0.8/setup.py
```

### Comparing `rocksnot-0.0.7/LICENSE` & `rocksnot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rocksnot-0.0.7/PKG-INFO` & `rocksnot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocksnot
-Version: 0.0.7
+Version: 0.0.8
 Summary: python package
 Home-page: https://github.com/rlape28/rocksnot
 Author: Robby Lape
 Author-email: robby.lape@gmail.com
 License: MIT license
 Keywords: rocksnot
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rocksnot-0.0.7/README.md` & `rocksnot-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rocksnot-0.0.7/rocksnot.egg-info/PKG-INFO` & `rocksnot-0.0.8/rocksnot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocksnot
-Version: 0.0.7
+Version: 0.0.8
 Summary: python package
 Home-page: https://github.com/rlape28/rocksnot
 Author: Robby Lape
 Author-email: robby.lape@gmail.com
 License: MIT license
 Keywords: rocksnot
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rocksnot-0.0.7/setup.py` & `rocksnot-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rocksnot',
     name='rocksnot',
     packages=find_packages(include=['rocksnot', 'rocksnot.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rlape28/rocksnot',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

