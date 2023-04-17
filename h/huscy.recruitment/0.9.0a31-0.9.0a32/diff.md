# Comparing `tmp/huscy.recruitment-0.9.0a31.tar.gz` & `tmp/huscy.recruitment-0.9.0a32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.recruitment-0.9.0a31.tar", last modified: Mon Dec  5 14:16:32 2022, max compression
+gzip compressed data, was "huscy.recruitment-0.9.0a32.tar", last modified: Mon Apr 17 10:46:28 2023, max compression
```

## Comparing `huscy.recruitment-0.9.0a31.tar` & `huscy.recruitment-0.9.0a32.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       14 2020-05-04 12:19:33.000000 huscy.recruitment-0.9.0a31/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/huscy/recruitment/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2022-12-05 13:54:10.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1007 2022-12-01 21:31:35.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      189 2022-06-24 08:58:51.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/huscy/recruitment/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4036 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-04 12:19:33.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2958 2022-03-28 09:53:22.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4223 2021-05-04 08:38:35.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/serializer.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/huscy/recruitment/services/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1145 2021-08-13 09:30:14.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3638 2022-11-14 08:45:27.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/attribute_filtersets.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      487 2020-10-26 15:18:33.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/contact_history.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      970 2021-05-04 08:38:35.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/contact_history_items.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3089 2021-05-07 08:23:46.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/participation_requests.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1467 2021-08-13 09:30:14.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/services/subject_group.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4877 2022-03-28 09:53:22.000000 huscy.recruitment-0.9.0a31/huscy/recruitment/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1020 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      766 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      108 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-05 14:16:32.000000 huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 14:16:32.876323 huscy.recruitment-0.9.0a31/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1312 2022-12-05 13:54:10.000000 huscy.recruitment-0.9.0a31/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1026 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       14 2020-05-04 12:19:33.000000 huscy.recruitment-0.9.0a32/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.449046 huscy.recruitment-0.9.0a32/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/huscy/recruitment/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2023-04-13 08:36:50.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1007 2022-12-01 21:31:35.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      189 2022-06-24 08:58:51.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/huscy/recruitment/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4034 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-04 12:19:33.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2958 2022-03-28 09:53:22.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4223 2021-05-04 08:38:35.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/serializer.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/huscy/recruitment/services/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1145 2021-08-13 09:30:14.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3638 2022-11-14 08:45:27.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/attribute_filtersets.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      487 2020-10-26 15:18:33.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/contact_history.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      970 2021-05-04 08:38:35.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/contact_history_items.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3089 2021-05-07 08:23:46.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/participation_requests.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1467 2021-08-13 09:30:14.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/services/subject_group.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4877 2022-03-28 09:53:22.000000 huscy.recruitment-0.9.0a32/huscy/recruitment/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1026 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      766 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      108 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 10:46:28.000000 huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:46:28.453046 huscy.recruitment-0.9.0a32/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1318 2023-04-17 10:36:15.000000 huscy.recruitment-0.9.0a32/setup.py
```

### Comparing `huscy.recruitment-0.9.0a31/PKG-INFO` & `huscy.recruitment-0.9.0a32/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.recruitment
-Version: 0.9.0a31
+Version: 0.9.0a32
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
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
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/api_urls.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/migrations/0001_initial.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Generated by Django 4.1.3 on 2022-12-05 08:16
+# Generated by Django 4.2 on 2023-04-17 05:46
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('appointments', '0004_auto_20211026_0424'),
         ('project_design', '0001_initial'),
+        ('appointments', '0004_auto_20211026_0424'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ('projects', '0002_alter_membership_options'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='AttributeFilterSet',
             fields=[
```

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/models.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/models.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/serializer.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/services/__init__.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/services/__init__.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/services/attribute_filtersets.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/services/attribute_filtersets.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/services/contact_history_items.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/services/contact_history_items.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/services/participation_requests.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/services/participation_requests.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/services/subject_group.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/services/subject_group.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy/recruitment/views.py` & `huscy.recruitment-0.9.0a32/huscy/recruitment/views.py`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/PKG-INFO` & `huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.recruitment
-Version: 0.9.0a31
+Version: 0.9.0a32
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
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
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.recruitment-0.9.0a31/huscy.recruitment.egg-info/SOURCES.txt` & `huscy.recruitment-0.9.0a32/huscy.recruitment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.recruitment-0.9.0a31/setup.py` & `huscy.recruitment-0.9.0a32/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
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

