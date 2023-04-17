# Comparing `tmp/huscy.subject_notes-0.1.0a1.tar.gz` & `tmp/huscy.subject_notes-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.subject_notes-0.1.0a1.tar", last modified: Mon Dec  5 14:24:53 2022, max compression
+gzip compressed data, was "huscy.subject_notes-0.1.0a2.tar", last modified: Mon Apr 17 10:36:07 2023, max compression
```

## Comparing `huscy.subject_notes-0.1.0a1.tar` & `huscy.subject_notes-0.1.0a2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1045 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       22 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/huscy/subject_notes/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      101 2022-12-05 14:17:07.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      754 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      429 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      191 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/huscy/subject_notes/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1966 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1233 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      739 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      991 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      703 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1238 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a1/huscy/subject_notes/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1045 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      603 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-05 14:24:53.000000 huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 14:24:53.909153 huscy.subject_notes-0.1.0a1/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1537 2022-12-05 14:17:07.000000 huscy.subject_notes-0.1.0a1/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1051 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       22 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/huscy/subject_notes/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      101 2023-04-14 08:55:53.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      754 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      429 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      191 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/huscy/subject_notes/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1966 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1233 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      739 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      991 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      703 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1238 2022-11-24 16:46:54.000000 huscy.subject_notes-0.1.0a2/huscy/subject_notes/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1051 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      603 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:36:07.000000 huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:36:07.806529 huscy.subject_notes-0.1.0a2/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1543 2023-04-17 10:29:20.000000 huscy.subject_notes-0.1.0a2/setup.py
```

### Comparing `huscy.subject_notes-0.1.0a1/PKG-INFO` & `huscy.subject_notes-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.subject_notes
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/subject_notes
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.subject_notes
         
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

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/admin.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/migrations/0001_initial.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/models.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/models.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/permissions.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/serializer.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/services.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/services.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy/subject_notes/views.py` & `huscy.subject_notes-0.1.0a2/huscy/subject_notes/views.py`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/PKG-INFO` & `huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: huscy.subject-notes
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/subject_notes
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.subject_notes
         
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

### Comparing `huscy.subject_notes-0.1.0a1/huscy.subject_notes.egg-info/SOURCES.txt` & `huscy.subject_notes-0.1.0a2/huscy.subject_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.subject_notes-0.1.0a1/setup.py` & `huscy.subject_notes-0.1.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
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

