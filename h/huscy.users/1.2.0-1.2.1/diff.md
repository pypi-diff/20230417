# Comparing `tmp/huscy.users-1.2.0.tar.gz` & `tmp/huscy.users-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.users-1.2.0.tar", last modified: Mon Dec  5 14:32:16 2022, max compression
+gzip compressed data, was "huscy.users-1.2.1.tar", last modified: Mon Apr 17 10:29:12 2023, max compression
```

## Comparing `huscy.users-1.2.0.tar` & `huscy.users-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:32:16.344931 huscy.users-1.2.0/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2919 2022-12-05 14:32:16.344931 huscy.users-1.2.0/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1382 2022-11-24 10:54:04.000000 huscy.users-1.2.0/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:32:16.340931 huscy.users-1.2.0/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:32:16.344931 huscy.users-1.2.0/huscy/users/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2022-12-05 14:25:06.000000 huscy.users-1.2.0/huscy/users/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      178 2022-12-05 14:25:06.000000 huscy.users-1.2.0/huscy/users/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      183 2022-06-24 10:00:38.000000 huscy.users-1.2.0/huscy/users/apps.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      649 2021-05-20 09:14:23.000000 huscy.users-1.2.0/huscy/users/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      353 2022-12-05 14:25:06.000000 huscy.users-1.2.0/huscy/users/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      711 2021-05-20 09:14:23.000000 huscy.users-1.2.0/huscy/users/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:32:16.340931 huscy.users-1.2.0/huscy.users.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2919 2022-12-05 14:32:16.000000 huscy.users-1.2.0/huscy.users.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      327 2022-12-05 14:32:16.000000 huscy.users-1.2.0/huscy.users.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 14:32:16.000000 huscy.users-1.2.0/huscy.users.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       93 2022-12-05 14:32:16.000000 huscy.users-1.2.0/huscy.users.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-05 14:32:16.000000 huscy.users-1.2.0/huscy.users.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 14:32:16.344931 huscy.users-1.2.0/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1559 2022-12-05 14:25:06.000000 huscy.users-1.2.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:29:12.074742 huscy.users-1.2.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2925 2023-04-17 10:29:12.074742 huscy.users-1.2.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1382 2023-04-13 08:46:50.000000 huscy.users-1.2.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:29:12.070742 huscy.users-1.2.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:29:12.074742 huscy.users-1.2.1/huscy/users/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-04-13 08:46:50.000000 huscy.users-1.2.1/huscy/users/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      178 2022-12-05 14:25:06.000000 huscy.users-1.2.1/huscy/users/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      183 2022-06-24 10:00:38.000000 huscy.users-1.2.1/huscy/users/apps.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      649 2021-05-20 09:14:23.000000 huscy.users-1.2.1/huscy/users/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      353 2022-12-05 14:25:06.000000 huscy.users-1.2.1/huscy/users/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      711 2021-05-20 09:14:23.000000 huscy.users-1.2.1/huscy/users/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:29:12.070742 huscy.users-1.2.1/huscy.users.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2925 2023-04-17 10:29:11.000000 huscy.users-1.2.1/huscy.users.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      327 2023-04-17 10:29:11.000000 huscy.users-1.2.1/huscy.users.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:29:11.000000 huscy.users-1.2.1/huscy.users.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       93 2023-04-17 10:29:11.000000 huscy.users-1.2.1/huscy.users.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:29:11.000000 huscy.users-1.2.1/huscy.users.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:29:12.074742 huscy.users-1.2.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1565 2023-04-17 10:26:09.000000 huscy.users-1.2.1/setup.py
```

### Comparing `huscy.users-1.2.0/PKG-INFO` & `huscy.users-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.users
-Version: 1.2.0
+Version: 1.2.1
 Summary: Listing and creating users via REST API
 Home-page: https://bitbucket.org/huscy/users
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.users
         
@@ -15,18 +15,18 @@
         ![Python Versions](https://img.shields.io/pypi/pyversions/huscy-users.svg)
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-users)
         
         
         
         ## Requirements
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         ## Installation
         
         To install `husy.users` simply run:
         
@@ -71,19 +71,19 @@
         
 Platform: UNKNOWN
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.users-1.2.0/README.md` & `huscy.users-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 ![Python Versions](https://img.shields.io/pypi/pyversions/huscy-users.svg)
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-users)
 
 
 
 ## Requirements
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 ## Installation
 
 To install `husy.users` simply run:
```

### Comparing `huscy.users-1.2.0/huscy/users/serializer.py` & `huscy.users-1.2.1/huscy/users/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.users-1.2.0/huscy/users/views.py` & `huscy.users-1.2.1/huscy/users/views.py`

 * *Files identical despite different names*

### Comparing `huscy.users-1.2.0/huscy.users.egg-info/PKG-INFO` & `huscy.users-1.2.1/huscy.users.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.users
-Version: 1.2.0
+Version: 1.2.1
 Summary: Listing and creating users via REST API
 Home-page: https://bitbucket.org/huscy/users
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.users
         
@@ -15,18 +15,18 @@
         ![Python Versions](https://img.shields.io/pypi/pyversions/huscy-users.svg)
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-users)
         
         
         
         ## Requirements
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         ## Installation
         
         To install `husy.users` simply run:
         
@@ -71,19 +71,19 @@
         
 Platform: UNKNOWN
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.users-1.2.0/setup.py` & `huscy.users-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 
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
         'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
 )
```

