# Comparing `tmp/huscy.pseudonyms-1.2.1.tar.gz` & `tmp/huscy.pseudonyms-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.pseudonyms-1.2.1.tar", last modified: Thu Dec  1 21:53:05 2022, max compression
+gzip compressed data, was "huscy.pseudonyms-1.2.2.tar", last modified: Mon Apr 17 10:10:44 2023, max compression
```

## Comparing `huscy.pseudonyms-1.2.1.tar` & `huscy.pseudonyms-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-01 21:53:05.372070 huscy.pseudonyms-1.2.1/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2020-03-19 11:06:18.000000 huscy.pseudonyms-1.2.1/LICENSE
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2815 2022-12-01 21:53:05.368070 huscy.pseudonyms-1.2.1/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1757 2022-12-01 21:49:45.000000 huscy.pseudonyms-1.2.1/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-01 21:53:05.368070 huscy.pseudonyms-1.2.1/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-01 21:53:05.368070 huscy.pseudonyms-1.2.1/huscy/pseudonyms/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2022-12-01 21:49:45.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      188 2022-06-23 11:42:27.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-01 21:53:05.368070 huscy.pseudonyms-1.2.1/huscy/pseudonyms/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      805 2021-01-19 12:45:42.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-19 20:40:47.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      423 2021-01-19 12:45:42.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1873 2021-04-29 12:20:21.000000 huscy.pseudonyms-1.2.1/huscy/pseudonyms/services.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-01 21:53:05.368070 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2815 2022-12-01 21:53:05.000000 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      419 2022-12-01 21:53:05.000000 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-01 21:53:05.000000 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       70 2022-12-01 21:53:05.000000 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-01 21:53:05.000000 huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-01 21:53:05.372070 huscy.pseudonyms-1.2.1/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1615 2022-12-01 21:49:45.000000 huscy.pseudonyms-1.2.1/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2020-03-19 11:06:18.000000 huscy.pseudonyms-1.2.2/LICENSE
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2877 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1762 2023-04-11 17:50:32.000000 huscy.pseudonyms-1.2.2/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/huscy/pseudonyms/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-04-11 17:50:32.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      188 2022-06-23 11:42:27.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/huscy/pseudonyms/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      805 2021-01-19 12:45:42.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-19 20:40:47.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      423 2021-01-19 12:45:42.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1873 2021-04-29 12:20:21.000000 huscy.pseudonyms-1.2.2/huscy/pseudonyms/services.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2877 2023-04-17 10:10:44.000000 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      419 2023-04-17 10:10:44.000000 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:10:44.000000 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       70 2023-04-17 10:10:44.000000 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:10:44.000000 huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:10:44.846784 huscy.pseudonyms-1.2.2/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1671 2023-04-17 10:07:51.000000 huscy.pseudonyms-1.2.2/setup.py
```

### Comparing `huscy.pseudonyms-1.2.1/LICENSE` & `huscy.pseudonyms-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.pseudonyms-1.2.1/PKG-INFO` & `huscy.pseudonyms-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: huscy.pseudonyms
-Version: 1.2.1
+Version: 1.2.2
 Summary: Managing pseudonyms for subjects.
 Home-page: https://bitbucket.org/huscy/pseudonyms
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
 License-File: LICENSE
 
 huscy.pseudonyms
 ======
@@ -35,18 +36,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-pseudonyms)
 [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/pseudonyms/badge.svg)](https://coveralls.io/bitbucket/huscy/pseudonyms)
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2 and 4.0.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 Installation
 ------
 
 To install `husy.pseudonyms` simply run:
 ```
```

### Comparing `huscy.pseudonyms-1.2.1/README.md` & `huscy.pseudonyms-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-pseudonyms)
 [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/pseudonyms/badge.svg)](https://coveralls.io/bitbucket/huscy/pseudonyms)
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2 and 4.0.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 Installation
 ------
 
 To install `husy.pseudonyms` simply run:
 ```
```

### Comparing `huscy.pseudonyms-1.2.1/huscy/pseudonyms/migrations/0001_initial.py` & `huscy.pseudonyms-1.2.2/huscy/pseudonyms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.pseudonyms-1.2.1/huscy/pseudonyms/services.py` & `huscy.pseudonyms-1.2.2/huscy/pseudonyms/services.py`

 * *Files identical despite different names*

### Comparing `huscy.pseudonyms-1.2.1/huscy.pseudonyms.egg-info/PKG-INFO` & `huscy.pseudonyms-1.2.2/huscy.pseudonyms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: huscy.pseudonyms
-Version: 1.2.1
+Version: 1.2.2
 Summary: Managing pseudonyms for subjects.
 Home-page: https://bitbucket.org/huscy/pseudonyms
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
 License-File: LICENSE
 
 huscy.pseudonyms
 ======
@@ -35,18 +36,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-pseudonyms)
 [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/pseudonyms/badge.svg)](https://coveralls.io/bitbucket/huscy/pseudonyms)
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2 and 4.0.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 Installation
 ------
 
 To install `husy.pseudonyms` simply run:
 ```
```

### Comparing `huscy.pseudonyms-1.2.1/setup.py` & `huscy.pseudonyms-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
 )
```

