# Comparing `tmp/huscy.bookings-0.4.1a11.tar.gz` & `tmp/huscy.bookings-0.4.1a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.bookings-0.4.1a11.tar", last modified: Tue Dec 20 11:02:28 2022, max compression
+gzip compressed data, was "huscy.bookings-0.4.1a12.tar", last modified: Mon Apr 17 09:25:57 2023, max compression
```

## Comparing `huscy.bookings-0.4.1a11.tar` & `huscy.bookings-0.4.1a12.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1017 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       11 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a11/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/config/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2147 2022-06-24 08:46:18.000000 huscy.bookings-0.4.1a11/config/settings.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      245 2022-12-05 13:16:05.000000 huscy.bookings-0.4.1a11/config/urls.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/huscy/bookings/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2022-12-20 10:52:32.000000 huscy.bookings-0.4.1a11/huscy/bookings/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      671 2022-12-20 10:52:32.000000 huscy.bookings-0.4.1a11/huscy/bookings/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-24 08:46:18.000000 huscy.bookings-0.4.1a11/huscy/bookings/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/huscy/bookings/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1297 2022-12-20 11:02:27.000000 huscy.bookings-0.4.1a11/huscy/bookings/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a11/huscy/bookings/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1984 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/huscy/bookings/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      851 2021-03-01 09:24:23.000000 huscy.bookings-0.4.1a11/huscy/bookings/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2950 2021-08-17 09:14:14.000000 huscy.bookings-0.4.1a11/huscy/bookings/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2583 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/huscy/bookings/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1017 2022-12-20 11:02:28.000000 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      852 2022-12-20 11:02:28.000000 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-20 11:02:28.000000 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       95 2022-12-20 11:02:28.000000 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2022-12-20 11:02:28.000000 huscy.bookings-0.4.1a11/huscy.bookings.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1263 2022-12-05 13:16:05.000000 huscy.bookings-0.4.1a11/setup.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/tests/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2729 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/tests/conftest.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/tests/serializer/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      261 2021-03-01 09:24:23.000000 huscy.bookings-0.4.1a11/tests/serializer/test_timeslot_serializer.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/tests/services/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2132 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/tests/services/test_get_timeslots.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4298 2020-11-06 14:37:55.000000 huscy.bookings-0.4.1a11/tests/test_book_timeslot.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2921 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a11/tests/test_create_timeslot.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2246 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a11/tests/test_delete_timeslot.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4351 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/tests/test_timeslot.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3639 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a11/tests/test_timeslot_manager.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4072 2020-11-06 14:37:55.000000 huscy.bookings-0.4.1a11/tests/test_unbook_timeslot.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3483 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a11/tests/test_update_timeslot.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-20 11:02:28.084083 huscy.bookings-0.4.1a11/tests/viewsets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1692 2021-08-17 09:14:14.000000 huscy.bookings-0.4.1a11/tests/viewsets/test_list_timeslots_viewset.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1023 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       11 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a12/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.270420 huscy.bookings-0.4.1a12/config/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2147 2022-06-24 08:46:18.000000 huscy.bookings-0.4.1a12/config/settings.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      245 2022-12-05 13:16:05.000000 huscy.bookings-0.4.1a12/config/urls.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.270420 huscy.bookings-0.4.1a12/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.270420 huscy.bookings-0.4.1a12/huscy/bookings/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2023-04-11 14:03:48.000000 huscy.bookings-0.4.1a12/huscy/bookings/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      671 2022-12-20 10:52:32.000000 huscy.bookings-0.4.1a12/huscy/bookings/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-24 08:46:18.000000 huscy.bookings-0.4.1a12/huscy/bookings/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.270420 huscy.bookings-0.4.1a12/huscy/bookings/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1295 2023-04-17 09:25:56.000000 huscy.bookings-0.4.1a12/huscy/bookings/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a12/huscy/bookings/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1984 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/huscy/bookings/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      851 2021-03-01 09:24:23.000000 huscy.bookings-0.4.1a12/huscy/bookings/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2950 2021-08-17 09:14:14.000000 huscy.bookings-0.4.1a12/huscy/bookings/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2583 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/huscy/bookings/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.270420 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1023 2023-04-17 09:25:57.000000 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      852 2023-04-17 09:25:57.000000 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 09:25:57.000000 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       95 2023-04-17 09:25:57.000000 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2023-04-17 09:25:57.000000 huscy.bookings-0.4.1a12/huscy.bookings.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1269 2023-04-17 09:17:24.000000 huscy.bookings-0.4.1a12/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2729 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/tests/conftest.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/tests/serializer/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      261 2021-03-01 09:24:23.000000 huscy.bookings-0.4.1a12/tests/serializer/test_timeslot_serializer.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/tests/services/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2132 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/tests/services/test_get_timeslots.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4298 2020-11-06 14:37:55.000000 huscy.bookings-0.4.1a12/tests/test_book_timeslot.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2921 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a12/tests/test_create_timeslot.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2246 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a12/tests/test_delete_timeslot.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4351 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/tests/test_timeslot.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3639 2021-10-26 13:00:18.000000 huscy.bookings-0.4.1a12/tests/test_timeslot_manager.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4072 2020-11-06 14:37:55.000000 huscy.bookings-0.4.1a12/tests/test_unbook_timeslot.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3483 2020-04-08 18:36:41.000000 huscy.bookings-0.4.1a12/tests/test_update_timeslot.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 09:25:57.274421 huscy.bookings-0.4.1a12/tests/viewsets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1692 2021-08-17 09:14:14.000000 huscy.bookings-0.4.1a12/tests/viewsets/test_list_timeslots_viewset.py
```

### Comparing `huscy.bookings-0.4.1a11/PKG-INFO` & `huscy.bookings-0.4.1a12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.bookings
-Version: 0.4.1a11
+Version: 0.4.1a12
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

### Comparing `huscy.bookings-0.4.1a11/config/settings.py` & `huscy.bookings-0.4.1a12/config/settings.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/api_urls.py` & `huscy.bookings-0.4.1a12/huscy/bookings/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/migrations/0001_initial.py` & `huscy.bookings-0.4.1a12/huscy/bookings/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Generated by Django 4.1.4 on 2022-12-20 05:02
+# Generated by Django 4.2 on 2023-04-17 04:25
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('appointments', '0004_auto_20211026_0424'),
         ('project_design', '0001_initial'),
+        ('appointments', '0004_auto_20211026_0424'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Timeslot',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/models.py` & `huscy.bookings-0.4.1a12/huscy/bookings/models.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/serializers.py` & `huscy.bookings-0.4.1a12/huscy/bookings/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/services.py` & `huscy.bookings-0.4.1a12/huscy/bookings/services.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy/bookings/views.py` & `huscy.bookings-0.4.1a12/huscy/bookings/views.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/huscy.bookings.egg-info/PKG-INFO` & `huscy.bookings-0.4.1a12/huscy.bookings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.bookings
-Version: 0.4.1a11
+Version: 0.4.1a12
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

### Comparing `huscy.bookings-0.4.1a11/huscy.bookings.egg-info/SOURCES.txt` & `huscy.bookings-0.4.1a12/huscy.bookings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/setup.py` & `huscy.bookings-0.4.1a12/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
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

### Comparing `huscy.bookings-0.4.1a11/tests/conftest.py` & `huscy.bookings-0.4.1a12/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/services/test_get_timeslots.py` & `huscy.bookings-0.4.1a12/tests/services/test_get_timeslots.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_book_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_book_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_create_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_create_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_delete_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_delete_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_timeslot_manager.py` & `huscy.bookings-0.4.1a12/tests/test_timeslot_manager.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_unbook_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_unbook_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/test_update_timeslot.py` & `huscy.bookings-0.4.1a12/tests/test_update_timeslot.py`

 * *Files identical despite different names*

### Comparing `huscy.bookings-0.4.1a11/tests/viewsets/test_list_timeslots_viewset.py` & `huscy.bookings-0.4.1a12/tests/viewsets/test_list_timeslots_viewset.py`

 * *Files identical despite different names*

