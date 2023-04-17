# Comparing `tmp/huscy.data_protection-0.4.0a7.tar.gz` & `tmp/huscy.data_protection-0.4.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.data_protection-0.4.0a7.tar", last modified: Mon Dec  5 12:01:07 2022, max compression
+gzip compressed data, was "huscy.data_protection-0.4.0a8.tar", last modified: Mon Apr 17 09:50:10 2023, max compression
```

## Comparing `huscy.data_protection-0.4.0a7.tar` & `huscy.data_protection-0.4.0a8.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 12:01:07.049073 huscy.data_protection-0.4.0a7/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      950 2022-12-05 12:01:07.049073 huscy.data_protection-0.4.0a7/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 12:01:07.045072 huscy.data_protection-0.4.0a7/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 12:01:07.045072 huscy.data_protection-0.4.0a7/huscy/data_protection/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      293 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      193 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 12:01:07.049073 huscy.data_protection-0.4.0a7/huscy/data_protection/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2093 2022-12-05 12:01:06.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1182 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1597 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2186 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/huscy/data_protection/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 12:01:07.045072 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      950 2022-12-05 12:01:06.000000 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      533 2022-12-05 12:01:07.000000 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 12:01:06.000000 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2022-12-05 12:01:06.000000 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2022-12-05 12:01:06.000000 huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 12:01:07.049073 huscy.data_protection-0.4.0a7/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1189 2022-12-05 11:50:09.000000 huscy.data_protection-0.4.0a7/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      956 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.743735 huscy.data_protection-0.4.0a8/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/huscy/data_protection/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      293 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      193 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/huscy/data_protection/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2091 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1182 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1597 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2186 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/huscy/data_protection/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      956 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      617 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       72 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 09:50:10.000000 huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1195 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:50:10.747735 huscy.data_protection-0.4.0a8/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3248 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/tests/test_dataaccessrequest_viewset.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3574 2023-04-17 09:44:00.000000 huscy.data_protection-0.4.0a8/tests/test_datarevocationrequest_viewset.py
```

### Comparing `huscy.data_protection-0.4.0a7/PKG-INFO` & `huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
-Name: huscy.data_protection
-Version: 0.4.0a7
+Name: huscy.data-protection
+Version: 0.4.0a8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
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

### Comparing `huscy.data_protection-0.4.0a7/huscy/data_protection/migrations/0001_initial.py` & `huscy.data_protection-0.4.0a8/huscy/data_protection/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by Django 4.1.3 on 2022-12-05 06:01
+# Generated by Django 4.2 on 2023-04-17 04:50
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ('subjects', '0001_squashed_0009_delete_contactold'),
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
             name='DataRevocationRequest',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `huscy.data_protection-0.4.0a7/huscy/data_protection/models.py` & `huscy.data_protection-0.4.0a8/huscy/data_protection/models.py`

 * *Files identical despite different names*

### Comparing `huscy.data_protection-0.4.0a7/huscy/data_protection/serializer.py` & `huscy.data_protection-0.4.0a8/huscy/data_protection/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.data_protection-0.4.0a7/huscy/data_protection/views.py` & `huscy.data_protection-0.4.0a8/huscy/data_protection/views.py`

 * *Files identical despite different names*

### Comparing `huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/PKG-INFO` & `huscy.data_protection-0.4.0a8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
-Name: huscy.data-protection
-Version: 0.4.0a7
+Name: huscy.data_protection
+Version: 0.4.0a8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
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

### Comparing `huscy.data_protection-0.4.0a7/huscy.data_protection.egg-info/SOURCES.txt` & `huscy.data_protection-0.4.0a8/huscy.data_protection.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 huscy/data_protection/__init__.py
 huscy/data_protection/api_urls.py
 huscy/data_protection/apps.py
 huscy/data_protection/models.py
 huscy/data_protection/serializer.py
 huscy/data_protection/views.py
 huscy/data_protection/migrations/0001_initial.py
-huscy/data_protection/migrations/__init__.py
+huscy/data_protection/migrations/__init__.py
+tests/test_dataaccessrequest_viewset.py
+tests/test_datarevocationrequest_viewset.py
```

### Comparing `huscy.data_protection-0.4.0a7/setup.py` & `huscy.data_protection-0.4.0a8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
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

