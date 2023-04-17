# Comparing `tmp/huscy.projects-1.5.0.tar.gz` & `tmp/huscy.projects-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.projects-1.5.0.tar", last modified: Fri Dec  9 13:05:01 2022, max compression
+gzip compressed data, was "huscy.projects-1.5.1.tar", last modified: Mon Apr 17 12:33:44 2023, max compression
```

## Comparing `huscy.projects-1.5.0.tar` & `huscy.projects-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-09 13:05:01.534602 huscy.projects-1.5.0/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3763 2022-12-09 13:05:01.534602 huscy.projects-1.5.0/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1991 2022-12-01 10:43:26.000000 huscy.projects-1.5.0/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-09 13:05:01.486601 huscy.projects-1.5.0/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-09 13:05:01.514602 huscy.projects-1.5.0/huscy/projects/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2022-12-09 10:03:27.000000 huscy.projects-1.5.0/huscy/projects/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1727 2021-10-29 14:50:52.000000 huscy.projects-1.5.0/huscy/projects/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      527 2022-12-09 10:03:27.000000 huscy.projects-1.5.0/huscy/projects/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-23 09:54:31.000000 huscy.projects-1.5.0/huscy/projects/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-09 13:05:01.534602 huscy.projects-1.5.0/huscy/projects/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3042 2021-10-28 10:46:34.000000 huscy.projects-1.5.0/huscy/projects/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      369 2021-11-01 07:26:46.000000 huscy.projects-1.5.0/huscy/projects/migrations/0002_alter_membership_options.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 12:30:45.000000 huscy.projects-1.5.0/huscy/projects/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2823 2021-10-28 10:46:34.000000 huscy.projects-1.5.0/huscy/projects/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1764 2022-12-01 10:43:26.000000 huscy.projects-1.5.0/huscy/projects/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4101 2022-03-15 12:22:45.000000 huscy.projects-1.5.0/huscy/projects/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3031 2022-03-15 12:22:45.000000 huscy.projects-1.5.0/huscy/projects/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2022-12-09 10:03:27.000000 huscy.projects-1.5.0/huscy/projects/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5085 2022-12-01 10:43:26.000000 huscy.projects-1.5.0/huscy/projects/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-09 13:05:01.486601 huscy.projects-1.5.0/huscy.projects.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3763 2022-12-09 13:05:01.000000 huscy.projects-1.5.0/huscy.projects.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      606 2022-12-09 13:05:01.000000 huscy.projects-1.5.0/huscy.projects.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-09 13:05:01.000000 huscy.projects-1.5.0/huscy.projects.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      164 2022-12-09 13:05:01.000000 huscy.projects-1.5.0/huscy.projects.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-09 13:05:01.000000 huscy.projects-1.5.0/huscy.projects.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-09 13:05:01.534602 huscy.projects-1.5.0/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1745 2022-12-09 10:03:27.000000 huscy.projects-1.5.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1991 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/projects/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/huscy/projects/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1727 2021-10-29 14:50:52.000000 huscy.projects-1.5.1/huscy/projects/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      527 2022-12-09 10:03:27.000000 huscy.projects-1.5.1/huscy/projects/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-23 09:54:31.000000 huscy.projects-1.5.1/huscy/projects/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/projects/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3042 2021-10-28 10:46:34.000000 huscy.projects-1.5.1/huscy/projects/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      369 2021-11-01 07:26:46.000000 huscy.projects-1.5.1/huscy/projects/migrations/0002_alter_membership_options.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 12:30:45.000000 huscy.projects-1.5.1/huscy/projects/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2823 2021-10-28 10:46:34.000000 huscy.projects-1.5.1/huscy/projects/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1764 2022-12-01 10:43:26.000000 huscy.projects-1.5.1/huscy/projects/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4101 2022-03-15 12:22:45.000000 huscy.projects-1.5.1/huscy/projects/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3193 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/huscy/projects/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2022-12-09 10:03:27.000000 huscy.projects-1.5.1/huscy/projects/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5085 2022-12-01 10:43:26.000000 huscy.projects-1.5.1/huscy/projects/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy.projects.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      606 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      164 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1751 2023-04-17 11:26:50.000000 huscy.projects-1.5.1/setup.py
```

### Comparing `huscy.projects-1.5.0/PKG-INFO` & `huscy.projects-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.projects
-Version: 1.5.0
+Version: 1.5.1
 Summary: Managing projects in a research context.
 Home-page: https://bitbucket.org/huscy/projects/
 Author: Mathias Goldau, Stefan Bunde
 Author-email: goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.projects
         
@@ -16,18 +16,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-projects)
         [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/projects/badge.svg?branch=master)](https://coveralls.io/bitbucket/huscy/projects?branch=master)
         
         
         
         ## Requirements
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         ## Installation
         
         To install `husy.projects` simply run:
         
@@ -95,19 +95,19 @@
         
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

### Comparing `huscy.projects-1.5.0/README.md` & `huscy.projects-1.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-projects)
 [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/projects/badge.svg?branch=master)](https://coveralls.io/bitbucket/huscy/projects?branch=master)
 
 
 
 ## Requirements
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 ## Installation
 
 To install `husy.projects` simply run:
```

### Comparing `huscy.projects-1.5.0/huscy/projects/admin.py` & `huscy.projects-1.5.1/huscy/projects/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/api_urls.py` & `huscy.projects-1.5.1/huscy/projects/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/migrations/0001_initial.py` & `huscy.projects-1.5.1/huscy/projects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/models.py` & `huscy.projects-1.5.1/huscy/projects/models.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/permissions.py` & `huscy.projects-1.5.1/huscy/projects/permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/serializers.py` & `huscy.projects-1.5.1/huscy/projects/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/services.py` & `huscy.projects-1.5.1/huscy/projects/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,12 +86,19 @@
         remove_perm('change_project', membership.user, membership.project)
     membership.is_coordinator = is_coordinator
     membership.save()
     return membership
 
 
 def update_project(project, local_id=None, title=None, description=None):
-    project.description = description or project.description
-    project.local_id = local_id or project.local_id
-    project.title = title or project.title
-    project.save(update_fields=['description', 'local_id', 'title'])
+    update_fields = []
+    if local_id is not None:
+        project.local_id = local_id
+        update_fields.append('local_id')
+    if title is not None:
+        project.title = title
+        update_fields.append('title')
+    if description is not None:
+        project.description = description
+        update_fields.append('description')
+    project.save(update_fields=update_fields)
     return project
```

### Comparing `huscy.projects-1.5.0/huscy/projects/urls.py` & `huscy.projects-1.5.1/huscy/projects/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy/projects/views.py` & `huscy.projects-1.5.1/huscy/projects/views.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/huscy.projects.egg-info/PKG-INFO` & `huscy.projects-1.5.1/huscy.projects.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.projects
-Version: 1.5.0
+Version: 1.5.1
 Summary: Managing projects in a research context.
 Home-page: https://bitbucket.org/huscy/projects/
 Author: Mathias Goldau, Stefan Bunde
 Author-email: goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.projects
         
@@ -16,18 +16,18 @@
         ![Django Versions](https://img.shields.io/pypi/djversions/huscy-projects)
         [![Coverage Status](https://coveralls.io/repos/bitbucket/huscy/projects/badge.svg?branch=master)](https://coveralls.io/bitbucket/huscy/projects?branch=master)
         
         
         
         ## Requirements
         
-        - Python 3.7+
+        - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.0 and 4.1.
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
         
         
         
         ## Installation
         
         To install `husy.projects` simply run:
         
@@ -95,19 +95,19 @@
         
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

### Comparing `huscy.projects-1.5.0/huscy.projects.egg-info/SOURCES.txt` & `huscy.projects-1.5.1/huscy.projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.0/setup.py` & `huscy.projects-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 
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

