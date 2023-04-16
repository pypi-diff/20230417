# Comparing `tmp/geomapdemo-0.1.1.tar.gz` & `tmp/geomapdemo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.1.1.tar", last modified: Sat Apr 15 18:57:58 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.2.tar", last modified: Sun Apr 16 22:55:22 2023, max compression
```

## Comparing `geomapdemo-0.1.1.tar` & `geomapdemo-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:57:58.685623 geomapdemo-0.1.1/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 18:57:58.000000 geomapdemo-0.1.1/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 18:57:58.689623 geomapdemo-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-15 18:57:45.000000 geomapdemo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/setup.py
```

### Comparing `geomapdemo-0.1.1/LICENSE` & `geomapdemo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.1/PKG-INFO` & `geomapdemo-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -33,12 +33,13 @@
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
     
 
 ## Features
 
 -   Create random numbers and random text
+-   Basic Mapping and drawing
 -   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.1.1/README.md` & `geomapdemo-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
     
 
 ## Features
 
 -   Create random numbers and random text
+-   Basic Mapping and drawing
 -   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.1.1/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.2/geomapdemo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -33,12 +33,13 @@
 -   Free software: MIT license
 - Documentation: https://zyang91.github.io/geomapdemo
     
 
 ## Features
 
 -   Create random numbers and random text
+-   Basic Mapping and drawing
 -   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.1.1/setup.py` & `geomapdemo-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

