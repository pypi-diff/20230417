# Comparing `tmp/huscy.project_design-0.3.0a4.tar.gz` & `tmp/huscy.project_design-0.3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_design-0.3.0a4.tar", last modified: Mon Dec  5 13:53:42 2022, max compression
+gzip compressed data, was "huscy.project_design-0.3.0a5.tar", last modified: Mon Apr 17 10:53:51 2023, max compression
```

## Comparing `huscy.project_design-0.3.0a4.tar` & `huscy.project_design-0.3.0a5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/
--rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2021-10-25 14:36:31.000000 huscy.project_design-0.3.0a4/LICENSE
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1014 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.3.0a4/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/huscy/project_design/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2022-12-05 13:36:14.000000 huscy.project_design-0.3.0a4/huscy/project_design/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a4/huscy/project_design/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      466 2022-12-05 13:36:14.000000 huscy.project_design-0.3.0a4/huscy/project_design/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.3.0a4/huscy/project_design/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/huscy/project_design/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     8578 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy/project_design/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.3.0a4/huscy/project_design/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4677 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a4/huscy/project_design/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2017 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a4/huscy/project_design/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1669 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a4/huscy/project_design/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1393 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a4/huscy/project_design/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1014 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      591 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-05 13:53:42.000000 huscy.project_design-0.3.0a4/huscy.project_design.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 13:53:42.919950 huscy.project_design-0.3.0a4/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1542 2022-12-05 13:36:14.000000 huscy.project_design-0.3.0a4/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)    34523 2021-10-25 14:36:31.000000 huscy.project_design-0.3.0a5/LICENSE
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.3.0a5/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/project_design/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-14 09:00:23.000000 huscy.project_design-0.3.0a5/huscy/project_design/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      466 2022-12-05 13:36:14.000000 huscy.project_design-0.3.0a5/huscy/project_design/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.3.0a5/huscy/project_design/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy/project_design/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     8576 2023-04-17 10:53:50.000000 huscy.project_design-0.3.0a5/huscy/project_design/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.3.0a5/huscy/project_design/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4677 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2017 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1669 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1393 2021-10-25 14:42:47.000000 huscy.project_design-0.3.0a5/huscy/project_design/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:53:51.393515 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      591 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:53:51.000000 huscy.project_design-0.3.0a5/huscy.project_design.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:53:51.397515 huscy.project_design-0.3.0a5/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1548 2023-04-17 10:46:38.000000 huscy.project_design-0.3.0a5/setup.py
```

### Comparing `huscy.project_design-0.3.0a4/LICENSE` & `huscy.project_design-0.3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/PKG-INFO` & `huscy.project_design-0.3.0a5/huscy.project_design.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: huscy.project_design
-Version: 0.3.0a4
+Name: huscy.project-design
+Version: 0.3.0a5
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
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
 License-File: LICENSE
 
 # huscy.project_design
```

### Comparing `huscy.project_design-0.3.0a4/huscy/project_design/migrations/0001_initial.py` & `huscy.project_design-0.3.0a5/huscy/project_design/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Generated by Django 4.1.3 on 2022-12-05 07:53
+# Generated by Django 4.2 on 2023-04-17 05:53
 
 import datetime
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 import huscy.project_design.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('projects', '0002_alter_membership_options'),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('projects', '0002_alter_membership_options'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='DataAcquisitionMethod',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `huscy.project_design-0.3.0a4/huscy/project_design/models.py` & `huscy.project_design-0.3.0a5/huscy/project_design/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/huscy/project_design/serializer.py` & `huscy.project_design-0.3.0a5/huscy/project_design/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/huscy/project_design/services.py` & `huscy.project_design-0.3.0a5/huscy/project_design/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/huscy/project_design/views.py` & `huscy.project_design-0.3.0a5/huscy/project_design/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/huscy.project_design.egg-info/PKG-INFO` & `huscy.project_design-0.3.0a5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
-Name: huscy.project-design
-Version: 0.3.0a4
+Name: huscy.project_design
+Version: 0.3.0a5
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
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
 License-File: LICENSE
 
 # huscy.project_design
```

### Comparing `huscy.project_design-0.3.0a4/huscy.project_design.egg-info/SOURCES.txt` & `huscy.project_design-0.3.0a5/huscy.project_design.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.0a4/setup.py` & `huscy.project_design-0.3.0a5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 
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

