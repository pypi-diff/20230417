# Comparing `tmp/huscy.participations-0.3.0a7.tar.gz` & `tmp/huscy.participations-0.3.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.participations-0.3.0a7.tar", last modified: Fri Dec  2 09:29:06 2022, max compression
+gzip compressed data, was "huscy.participations-0.3.0a8.tar", last modified: Mon Apr 17 09:43:46 2023, max compression
```

## Comparing `huscy.participations-0.3.0a7.tar` & `huscy.participations-0.3.0a8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1061 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-05-06 09:48:24.000000 huscy.participations-0.3.0a7/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/huscy/participations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2022-12-02 09:02:58.000000 huscy.participations-0.3.0a7/huscy/participations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      962 2022-12-02 09:02:58.000000 huscy.participations-0.3.0a7/huscy/participations/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-24 09:40:30.000000 huscy.participations-0.3.0a7/huscy/participations/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/huscy/participations/migrations/
--rw-rw-r--   0 jenkins    (111) jenkins    (115)     2161 2021-05-06 11:02:22.000000 huscy.participations-0.3.0a7/huscy/participations/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      661 2022-03-28 13:20:29.000000 huscy.participations-0.3.0a7/huscy/participations/migrations/0002_auto_20220328_0820.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-05-06 11:06:28.000000 huscy.participations-0.3.0a7/huscy/participations/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1816 2021-05-06 09:48:24.000000 huscy.participations-0.3.0a7/huscy/participations/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2849 2021-05-11 08:32:57.000000 huscy.participations-0.3.0a7/huscy/participations/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2031 2022-03-28 13:20:10.000000 huscy.participations-0.3.0a7/huscy/participations/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1366 2022-03-28 13:20:10.000000 huscy.participations-0.3.0a7/huscy/participations/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/huscy.participations.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1061 2022-12-02 09:29:06.000000 huscy.participations-0.3.0a7/huscy.participations.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      612 2022-12-02 09:29:06.000000 huscy.participations-0.3.0a7/huscy.participations.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-02 09:29:06.000000 huscy.participations-0.3.0a7/huscy.participations.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       73 2022-12-02 09:29:06.000000 huscy.participations-0.3.0a7/huscy.participations.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-02 09:29:06.000000 huscy.participations-0.3.0a7/huscy.participations.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-02 09:29:06.396243 huscy.participations-0.3.0a7/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1524 2022-12-02 09:02:58.000000 huscy.participations-0.3.0a7/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:43:46.531752 huscy.participations-0.3.0a8/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1067 2023-04-17 09:43:46.531752 huscy.participations-0.3.0a8/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-05-06 09:48:24.000000 huscy.participations-0.3.0a8/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:43:46.527752 huscy.participations-0.3.0a8/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:43:46.531752 huscy.participations-0.3.0a8/huscy/participations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-14 09:13:05.000000 huscy.participations-0.3.0a8/huscy/participations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      962 2022-12-02 09:02:58.000000 huscy.participations-0.3.0a8/huscy/participations/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-24 09:40:30.000000 huscy.participations-0.3.0a8/huscy/participations/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:43:46.531752 huscy.participations-0.3.0a8/huscy/participations/migrations/
+-rw-rw-r--   0 jenkins    (111) jenkins    (115)     2161 2021-05-06 11:02:22.000000 huscy.participations-0.3.0a8/huscy/participations/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      661 2022-03-28 13:20:29.000000 huscy.participations-0.3.0a8/huscy/participations/migrations/0002_auto_20220328_0820.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-05-06 11:06:28.000000 huscy.participations-0.3.0a8/huscy/participations/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1816 2021-05-06 09:48:24.000000 huscy.participations-0.3.0a8/huscy/participations/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2849 2021-05-11 08:32:57.000000 huscy.participations-0.3.0a8/huscy/participations/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2031 2022-03-28 13:20:10.000000 huscy.participations-0.3.0a8/huscy/participations/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1366 2022-03-28 13:20:10.000000 huscy.participations-0.3.0a8/huscy/participations/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:43:46.527752 huscy.participations-0.3.0a8/huscy.participations.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1067 2023-04-17 09:43:46.000000 huscy.participations-0.3.0a8/huscy.participations.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      612 2023-04-17 09:43:46.000000 huscy.participations-0.3.0a8/huscy.participations.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 09:43:46.000000 huscy.participations-0.3.0a8/huscy.participations.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       73 2023-04-17 09:43:46.000000 huscy.participations-0.3.0a8/huscy.participations.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 09:43:46.000000 huscy.participations-0.3.0a8/huscy.participations.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 09:43:46.531752 huscy.participations-0.3.0a8/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1530 2023-04-17 09:27:34.000000 huscy.participations-0.3.0a8/setup.py
```

### Comparing `huscy.participations-0.3.0a7/PKG-INFO` & `huscy.participations-0.3.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.participations
-Version: 0.3.0a7
+Version: 0.3.0a8
 Summary: huscy.participations
 Home-page: https://bitbucket.org/huscy/participations
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.participations
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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

### Comparing `huscy.participations-0.3.0a7/huscy/participations/api_urls.py` & `huscy.participations-0.3.0a8/huscy/participations/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/migrations/0001_initial.py` & `huscy.participations-0.3.0a8/huscy/participations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/migrations/0002_auto_20220328_0820.py` & `huscy.participations-0.3.0a8/huscy/participations/migrations/0002_auto_20220328_0820.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/models.py` & `huscy.participations-0.3.0a8/huscy/participations/models.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/serializer.py` & `huscy.participations-0.3.0a8/huscy/participations/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/services.py` & `huscy.participations-0.3.0a8/huscy/participations/services.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy/participations/views.py` & `huscy.participations-0.3.0a8/huscy/participations/views.py`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/huscy.participations.egg-info/PKG-INFO` & `huscy.participations-0.3.0a8/huscy.participations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.participations
-Version: 0.3.0a7
+Version: 0.3.0a8
 Summary: huscy.participations
 Home-page: https://bitbucket.org/huscy/participations
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.participations
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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

### Comparing `huscy.participations-0.3.0a7/huscy.participations.egg-info/SOURCES.txt` & `huscy.participations-0.3.0a8/huscy.participations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.participations-0.3.0a7/setup.py` & `huscy.participations-0.3.0a8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
     classifiers=[
         'Development Status :: 3 - Alpha',
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

