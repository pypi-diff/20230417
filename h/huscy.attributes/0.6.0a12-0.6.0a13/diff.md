# Comparing `tmp/huscy.attributes-0.6.0a12.tar.gz` & `tmp/huscy.attributes-0.6.0a13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.attributes-0.6.0a12.tar", last modified: Mon Dec  5 13:14:08 2022, max compression
+gzip compressed data, was "huscy.attributes-0.6.0a13.tar", last modified: Mon Apr 17 11:26:10 2023, max compression
```

## Comparing `huscy.attributes-0.6.0a12.tar` & `huscy.attributes-0.6.0a13.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.830423 huscy.attributes-0.6.0a12/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1069 2022-12-05 13:14:08.830423 huscy.attributes-0.6.0a12/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2020-04-08 19:17:07.000000 huscy.attributes-0.6.0a12/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/config/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2151 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a12/config/settings.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      239 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a12/config/urls.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.822423 huscy.attributes-0.6.0a12/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/huscy/attributes/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a12/huscy/attributes/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1191 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a12/huscy/attributes/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      364 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a12/huscy/attributes/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      188 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a12/huscy/attributes/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/huscy/attributes/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1210 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a12/huscy/attributes/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      611 2022-03-21 16:42:06.000000 huscy.attributes-0.6.0a12/huscy/attributes/migrations/0002_auto_20220321_1142.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-08 19:17:07.000000 huscy.attributes-0.6.0a12/huscy/attributes/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      722 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a12/huscy/attributes/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      445 2021-04-29 14:06:51.000000 huscy.attributes-0.6.0a12/huscy/attributes/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1064 2021-08-30 07:43:59.000000 huscy.attributes-0.6.0a12/huscy/attributes/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2976 2022-03-21 16:41:39.000000 huscy.attributes-0.6.0a12/huscy/attributes/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2134 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a12/huscy/attributes/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1069 2022-12-05 13:14:08.000000 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1187 2022-12-05 13:14:08.000000 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 13:14:08.000000 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       88 2022-12-05 13:14:08.000000 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2022-12-05 13:14:08.000000 huscy.attributes-0.6.0a12/huscy.attributes.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 13:14:08.830423 huscy.attributes-0.6.0a12/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1309 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a12/setup.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/tests/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/tests/admin/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      610 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a12/tests/admin/test_attribute_schema_admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      874 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a12/tests/admin/test_attribute_set_admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3601 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a12/tests/conftest.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/tests/models/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      359 2021-04-29 14:06:51.000000 huscy.attributes-0.6.0a12/tests/models/test_attribute_set.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/tests/serializer/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      518 2020-09-02 17:39:23.000000 huscy.attributes-0.6.0a12/tests/serializer/test_attributeset_serializer.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 13:14:08.826424 huscy.attributes-0.6.0a12/tests/services/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1726 2021-08-02 10:01:58.000000 huscy.attributes-0.6.0a12/tests/services/test_create_attribute_schema.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1721 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a12/tests/services/test_dict_merge.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2191 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a12/tests/services/test_filter_attributes_by_category_permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1064 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a12/tests/services/test_get_attribute_schema.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      635 2020-06-15 12:35:12.000000 huscy.attributes-0.6.0a12/tests/services/test_get_or_create_attribute_set.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2440 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a12/tests/services/test_update_attribute_set.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1936 2021-08-02 10:01:58.000000 huscy.attributes-0.6.0a12/tests/test_attributeschema_apiview.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5469 2022-03-21 16:41:39.000000 huscy.attributes-0.6.0a12/tests/test_attributeset_viewset.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1025 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2020-04-08 19:17:07.000000 huscy.attributes-0.6.0a13/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.909226 huscy.attributes-0.6.0a13/config/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2151 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a13/config/settings.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      239 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a13/config/urls.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.909226 huscy.attributes-0.6.0a13/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.909226 huscy.attributes-0.6.0a13/huscy/attributes/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2023-04-11 12:04:49.000000 huscy.attributes-0.6.0a13/huscy/attributes/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1191 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a13/huscy/attributes/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      364 2022-12-05 12:01:33.000000 huscy.attributes-0.6.0a13/huscy/attributes/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      188 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a13/huscy/attributes/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.909226 huscy.attributes-0.6.0a13/huscy/attributes/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1210 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a13/huscy/attributes/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      611 2022-03-21 16:42:06.000000 huscy.attributes-0.6.0a13/huscy/attributes/migrations/0002_auto_20220321_1142.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-04-08 19:17:07.000000 huscy.attributes-0.6.0a13/huscy/attributes/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      722 2022-06-23 11:43:15.000000 huscy.attributes-0.6.0a13/huscy/attributes/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      445 2021-04-29 14:06:51.000000 huscy.attributes-0.6.0a13/huscy/attributes/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1064 2021-08-30 07:43:59.000000 huscy.attributes-0.6.0a13/huscy/attributes/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2976 2022-03-21 16:41:39.000000 huscy.attributes-0.6.0a13/huscy/attributes/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2134 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a13/huscy/attributes/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.909226 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1025 2023-04-17 11:26:10.000000 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1187 2023-04-17 11:26:10.000000 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 11:26:10.000000 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       88 2023-04-17 11:26:10.000000 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2023-04-17 11:26:10.000000 huscy.attributes-0.6.0a13/huscy.attributes.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1266 2023-04-17 10:57:50.000000 huscy.attributes-0.6.0a13/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/tests/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/tests/admin/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      610 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a13/tests/admin/test_attribute_schema_admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      874 2021-08-20 10:06:22.000000 huscy.attributes-0.6.0a13/tests/admin/test_attribute_set_admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3601 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a13/tests/conftest.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/tests/models/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      359 2021-04-29 14:06:51.000000 huscy.attributes-0.6.0a13/tests/models/test_attribute_set.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/tests/serializer/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      518 2020-09-02 17:39:23.000000 huscy.attributes-0.6.0a13/tests/serializer/test_attributeset_serializer.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 11:26:10.913226 huscy.attributes-0.6.0a13/tests/services/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1726 2021-08-02 10:01:58.000000 huscy.attributes-0.6.0a13/tests/services/test_create_attribute_schema.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1721 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a13/tests/services/test_dict_merge.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2191 2021-08-04 11:18:51.000000 huscy.attributes-0.6.0a13/tests/services/test_filter_attributes_by_category_permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1064 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a13/tests/services/test_get_attribute_schema.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      635 2020-06-15 12:35:12.000000 huscy.attributes-0.6.0a13/tests/services/test_get_or_create_attribute_set.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2440 2021-08-20 12:21:37.000000 huscy.attributes-0.6.0a13/tests/services/test_update_attribute_set.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1936 2021-08-02 10:01:58.000000 huscy.attributes-0.6.0a13/tests/test_attributeschema_apiview.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5469 2022-03-21 16:41:39.000000 huscy.attributes-0.6.0a13/tests/test_attributeset_viewset.py
```

### Comparing `huscy.attributes-0.6.0a12/PKG-INFO` & `huscy.attributes-0.6.0a13/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.attributes
-Version: 0.6.0a12
+Version: 0.6.0a13
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
-Classifier: Programming Language :: Python :: 3.6
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

### Comparing `huscy.attributes-0.6.0a12/config/settings.py` & `huscy.attributes-0.6.0a13/config/settings.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/admin.py` & `huscy.attributes-0.6.0a13/huscy/attributes/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/migrations/0001_initial.py` & `huscy.attributes-0.6.0a13/huscy/attributes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/migrations/0002_auto_20220321_1142.py` & `huscy.attributes-0.6.0a13/huscy/attributes/migrations/0002_auto_20220321_1142.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/models.py` & `huscy.attributes-0.6.0a13/huscy/attributes/models.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/serializer.py` & `huscy.attributes-0.6.0a13/huscy/attributes/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/services.py` & `huscy.attributes-0.6.0a13/huscy/attributes/services.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy/attributes/views.py` & `huscy.attributes-0.6.0a13/huscy/attributes/views.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/huscy.attributes.egg-info/PKG-INFO` & `huscy.attributes-0.6.0a13/huscy.attributes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.attributes
-Version: 0.6.0a12
+Version: 0.6.0a13
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
-Classifier: Programming Language :: Python :: 3.6
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

### Comparing `huscy.attributes-0.6.0a12/huscy.attributes.egg-info/SOURCES.txt` & `huscy.attributes-0.6.0a13/huscy.attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/setup.py` & `huscy.attributes-0.6.0a13/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,18 @@
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
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

### Comparing `huscy.attributes-0.6.0a12/tests/admin/test_attribute_schema_admin.py` & `huscy.attributes-0.6.0a13/tests/admin/test_attribute_schema_admin.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/admin/test_attribute_set_admin.py` & `huscy.attributes-0.6.0a13/tests/admin/test_attribute_set_admin.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/conftest.py` & `huscy.attributes-0.6.0a13/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/serializer/test_attributeset_serializer.py` & `huscy.attributes-0.6.0a13/tests/serializer/test_attributeset_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_create_attribute_schema.py` & `huscy.attributes-0.6.0a13/tests/services/test_create_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_dict_merge.py` & `huscy.attributes-0.6.0a13/tests/services/test_dict_merge.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_filter_attributes_by_category_permissions.py` & `huscy.attributes-0.6.0a13/tests/services/test_filter_attributes_by_category_permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_get_attribute_schema.py` & `huscy.attributes-0.6.0a13/tests/services/test_get_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_get_or_create_attribute_set.py` & `huscy.attributes-0.6.0a13/tests/services/test_get_or_create_attribute_set.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/services/test_update_attribute_set.py` & `huscy.attributes-0.6.0a13/tests/services/test_update_attribute_set.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/test_attributeschema_apiview.py` & `huscy.attributes-0.6.0a13/tests/test_attributeschema_apiview.py`

 * *Files identical despite different names*

### Comparing `huscy.attributes-0.6.0a12/tests/test_attributeset_viewset.py` & `huscy.attributes-0.6.0a13/tests/test_attributeset_viewset.py`

 * *Files identical despite different names*

