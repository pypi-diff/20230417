# Comparing `tmp/huscy.project_documents-1.3.0.tar.gz` & `tmp/huscy.project_documents-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_documents-1.3.0.tar", last modified: Tue Dec 13 10:39:12 2022, max compression
+gzip compressed data, was "huscy.project_documents-1.3.1.tar", last modified: Mon Apr 17 13:38:38 2023, max compression
```

## Comparing `huscy.project_documents-1.3.0.tar` & `huscy.project_documents-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3701 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1885 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.0/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/huscy/project_documents/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.0/huscy/project_documents/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      758 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.0/huscy/project_documents/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      370 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.0/huscy/project_documents/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      195 2022-06-23 13:24:50.000000 huscy.project_documents-1.3.0/huscy/project_documents/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/huscy/project_documents/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2021-02-24 14:29:50.000000 huscy.project_documents-1.3.0/huscy/project_documents/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      876 2021-10-28 12:45:20.000000 huscy.project_documents-1.3.0/huscy/project_documents/migrations/0002_auto_20211028_0738.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-18 12:08:52.000000 huscy.project_documents-1.3.0/huscy/project_documents/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1282 2021-10-28 12:45:20.000000 huscy.project_documents-1.3.0/huscy/project_documents/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      570 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.0/huscy/project_documents/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1372 2022-02-21 11:10:23.000000 huscy.project_documents-1.3.0/huscy/project_documents/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      915 2021-08-02 08:37:11.000000 huscy.project_documents-1.3.0/huscy/project_documents/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      545 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.0/huscy/project_documents/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2075 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.0/huscy/project_documents/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3701 2022-12-13 10:39:11.000000 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      761 2022-12-13 10:39:12.000000 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-13 10:39:11.000000 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2022-12-13 10:39:11.000000 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-13 10:39:11.000000 huscy.project_documents-1.3.0/huscy.project_documents.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-13 10:39:12.026828 huscy.project_documents-1.3.0/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1695 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3707 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1885 2023-04-13 11:18:39.000000 huscy.project_documents-1.3.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/huscy/project_documents/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-04-13 11:18:39.000000 huscy.project_documents-1.3.1/huscy/project_documents/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      758 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.1/huscy/project_documents/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      370 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.1/huscy/project_documents/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      195 2022-06-23 13:24:50.000000 huscy.project_documents-1.3.1/huscy/project_documents/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/huscy/project_documents/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1519 2021-02-24 14:29:50.000000 huscy.project_documents-1.3.1/huscy/project_documents/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      876 2021-10-28 12:45:20.000000 huscy.project_documents-1.3.1/huscy/project_documents/migrations/0002_auto_20211028_0738.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-18 12:08:52.000000 huscy.project_documents-1.3.1/huscy/project_documents/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1282 2021-10-28 12:45:20.000000 huscy.project_documents-1.3.1/huscy/project_documents/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      570 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.1/huscy/project_documents/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1372 2022-02-21 11:10:23.000000 huscy.project_documents-1.3.1/huscy/project_documents/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      915 2021-08-02 08:37:11.000000 huscy.project_documents-1.3.1/huscy/project_documents/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      545 2022-12-13 09:26:45.000000 huscy.project_documents-1.3.1/huscy/project_documents/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2075 2021-11-01 09:35:12.000000 huscy.project_documents-1.3.1/huscy/project_documents/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3707 2023-04-17 13:38:38.000000 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      761 2023-04-17 13:38:38.000000 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 13:38:38.000000 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-04-17 13:38:38.000000 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 13:38:38.000000 huscy.project_documents-1.3.1/huscy.project_documents.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 13:38:38.205565 huscy.project_documents-1.3.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1643 2023-04-17 12:36:40.000000 huscy.project_documents-1.3.1/setup.py
```

### Comparing `huscy.project_documents-1.3.0/PKG-INFO` & `huscy.project_documents-1.3.1/huscy.project_documents.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: huscy.project_documents
-Version: 1.3.0
+Name: huscy.project-documents
+Version: 1.3.1
 Summary: Managing document files for projects.
 Home-page: https://bitbucket.org/huscy/project_documents
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.project_documents
         ======
@@ -17,18 +17,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project_documents)
         
         
         
         Requirements
         ------
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         Installation
         ------
         
         To install `husy.project_documents` simply run:
@@ -94,19 +94,19 @@
         
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

### Comparing `huscy.project_documents-1.3.0/README.md` & `huscy.project_documents-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project_documents)
 
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 Installation
 ------
 
 To install `husy.project_documents` simply run:
```

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/admin.py` & `huscy.project_documents-1.3.1/huscy/project_documents/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/migrations/0001_initial.py` & `huscy.project_documents-1.3.1/huscy/project_documents/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/migrations/0002_auto_20211028_0738.py` & `huscy.project_documents-1.3.1/huscy/project_documents/migrations/0002_auto_20211028_0738.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/models.py` & `huscy.project_documents-1.3.1/huscy/project_documents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/permissions.py` & `huscy.project_documents-1.3.1/huscy/project_documents/permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/serializer.py` & `huscy.project_documents-1.3.1/huscy/project_documents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/services.py` & `huscy.project_documents-1.3.1/huscy/project_documents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/urls.py` & `huscy.project_documents-1.3.1/huscy/project_documents/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy/project_documents/views.py` & `huscy.project_documents-1.3.1/huscy/project_documents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_documents-1.3.0/huscy.project_documents.egg-info/PKG-INFO` & `huscy.project_documents-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: huscy.project-documents
-Version: 1.3.0
+Name: huscy.project_documents
+Version: 1.3.1
 Summary: Managing document files for projects.
 Home-page: https://bitbucket.org/huscy/project_documents
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.project_documents
         ======
@@ -17,18 +17,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project_documents)
         
         
         
         Requirements
         ------
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         Installation
         ------
         
         To install `husy.project_documents` simply run:
@@ -94,19 +94,19 @@
         
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

### Comparing `huscy.project_documents-1.3.0/huscy.project_documents.egg-info/SOURCES.txt` & `huscy.project_documents-1.3.1/huscy.project_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

