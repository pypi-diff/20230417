# Comparing `tmp/huscy.project_ethics-1.3.0.tar.gz` & `tmp/huscy.project_ethics-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_ethics-1.3.0.tar", last modified: Mon Feb  6 11:25:41 2023, max compression
+gzip compressed data, was "huscy.project_ethics-1.3.1.tar", last modified: Mon Apr 17 14:43:36 2023, max compression
```

## Comparing `huscy.project_ethics-1.3.0.tar` & `huscy.project_ethics-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-02-06 11:25:41.250080 huscy.project_ethics-1.3.0/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3450 2023-02-06 11:25:41.246080 huscy.project_ethics-1.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1728 2022-12-01 15:46:43.000000 huscy.project_ethics-1.3.0/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-02-06 11:25:41.246080 huscy.project_ethics-1.3.0/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-02-06 11:25:41.246080 huscy.project_ethics-1.3.0/huscy/project_ethics/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1311 2021-11-01 11:31:20.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      614 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 13:25:50.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-02-06 11:25:41.246080 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3136 2021-03-23 02:28:15.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1451 2021-11-01 11:31:20.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0002_auto_20211101_0600.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      598 2021-11-04 17:18:32.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0003_alter_ethicfile_filehandle.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      464 2021-11-11 12:12:27.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0004_alter_ethicfile_filetype.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-18 13:48:28.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2366 2021-11-11 12:12:27.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1341 2022-01-20 08:29:05.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2222 2022-01-31 14:41:33.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1259 2021-03-23 02:28:15.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      789 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3757 2022-01-14 11:02:20.000000 huscy.project_ethics-1.3.0/huscy/project_ethics/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-02-06 11:25:41.246080 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3450 2023-02-06 11:25:41.000000 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      839 2023-02-06 11:25:41.000000 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-02-06 11:25:41.000000 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-02-06 11:25:41.000000 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-02-06 11:25:41.000000 huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-02-06 11:25:41.250080 huscy.project_ethics-1.3.0/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1594 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 14:43:36.183953 huscy.project_ethics-1.3.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3456 2023-04-17 14:43:36.183953 huscy.project_ethics-1.3.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1728 2023-04-11 14:17:43.000000 huscy.project_ethics-1.3.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 14:43:36.179953 huscy.project_ethics-1.3.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 14:43:36.183953 huscy.project_ethics-1.3.1/huscy/project_ethics/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2023-04-11 14:17:43.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1311 2021-11-01 11:31:20.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      614 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 13:25:50.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 14:43:36.183953 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3136 2021-03-23 02:28:15.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1451 2021-11-01 11:31:20.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0002_auto_20211101_0600.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      598 2021-11-04 17:18:32.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0003_alter_ethicfile_filehandle.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      464 2021-11-11 12:12:27.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0004_alter_ethicfile_filetype.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-18 13:48:28.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2366 2021-11-11 12:12:27.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1341 2022-01-20 08:29:05.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2222 2022-01-31 14:41:33.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1259 2021-03-23 02:28:15.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      789 2023-02-06 08:42:45.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3757 2022-01-14 11:02:20.000000 huscy.project_ethics-1.3.1/huscy/project_ethics/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 14:43:36.179953 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3456 2023-04-17 14:43:36.000000 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      839 2023-04-17 14:43:36.000000 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 14:43:36.000000 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-04-17 14:43:36.000000 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 14:43:36.000000 huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 14:43:36.183953 huscy.project_ethics-1.3.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1600 2023-04-17 13:40:36.000000 huscy.project_ethics-1.3.1/setup.py
```

### Comparing `huscy.project_ethics-1.3.0/PKG-INFO` & `huscy.project_ethics-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_ethics
-Version: 1.3.0
+Version: 1.3.1
 Summary: Managing ethics and ethic files for projects in a human research context.
 Home-page: UNKNOWN
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.project-ethics
         ======
@@ -17,18 +17,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project-ethics)
         
         
         
         Requirements
         ------
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         Installation
         ------
         
         To install `husy.project-ethics` simply run:
@@ -92,19 +92,19 @@
         
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

### Comparing `huscy.project_ethics-1.3.0/README.md` & `huscy.project_ethics-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project-ethics)
 
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 Installation
 ------
 
 To install `husy.project-ethics` simply run:
```

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/admin.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/api_urls.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0001_initial.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0002_auto_20211101_0600.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0002_auto_20211101_0600.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/migrations/0003_alter_ethicfile_filehandle.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/migrations/0003_alter_ethicfile_filehandle.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/models.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/permissions.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/serializer.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/services.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/urls.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy/project_ethics/views.py` & `huscy.project_ethics-1.3.1/huscy/project_ethics/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/PKG-INFO` & `huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-ethics
-Version: 1.3.0
+Version: 1.3.1
 Summary: Managing ethics and ethic files for projects in a human research context.
 Home-page: UNKNOWN
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.project-ethics
         ======
@@ -17,18 +17,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-project-ethics)
         
         
         
         Requirements
         ------
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         Installation
         ------
         
         To install `husy.project-ethics` simply run:
@@ -92,19 +92,19 @@
         
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

### Comparing `huscy.project_ethics-1.3.0/huscy.project_ethics.egg-info/SOURCES.txt` & `huscy.project_ethics-1.3.1/huscy.project_ethics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.project_ethics-1.3.0/setup.py` & `huscy.project_ethics-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
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

