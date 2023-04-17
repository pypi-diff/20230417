# Comparing `tmp/huscy.rooms-0.2.0a6.tar.gz` & `tmp/huscy.rooms-0.2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.rooms-0.2.0a6.tar", last modified: Mon Dec  5 16:04:04 2022, max compression
+gzip compressed data, was "huscy.rooms-0.2.0a7.tar", last modified: Mon Apr 17 10:18:16 2023, max compression
```

## Comparing `huscy.rooms-0.2.0a6.tar` & `huscy.rooms-0.2.0a7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.325676 huscy.rooms-0.2.0a6/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1017 2022-12-05 16:04:04.325676 huscy.rooms-0.2.0a6/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1405 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a6/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/config/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1912 2020-03-23 15:46:10.000000 huscy.rooms-0.2.0a6/config/settings.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      234 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a6/config/urls.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/huscy/rooms/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2022-12-05 15:47:50.000000 huscy.rooms-0.2.0a6/huscy/rooms/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      171 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      276 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a6/huscy/rooms/api_urls.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/huscy/rooms/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1299 2020-03-17 07:20:01.000000 huscy.rooms-0.2.0a6/huscy/rooms/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      563 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1029 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      425 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/huscy/rooms/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1017 2022-12-05 16:04:04.000000 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      785 2022-12-05 16:04:04.000000 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-05 16:04:04.000000 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       84 2022-12-05 16:04:04.000000 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2022-12-05 16:04:04.000000 huscy.rooms-0.2.0a6/huscy.rooms.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-05 16:04:04.325676 huscy.rooms-0.2.0a6/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1247 2022-12-05 15:47:50.000000 huscy.rooms-0.2.0a6/setup.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/tests/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      927 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/conftest.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-05 16:04:04.321676 huscy.rooms-0.2.0a6/tests/viewsets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1471 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_building_viewset_create_building.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1497 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_building_viewset_view_buildings.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1478 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_floor_viewset_create_floor.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1405 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_floor_viewset_view_floors.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1536 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_room_viewset_create_room.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1381 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a6/tests/viewsets/test_room_viewset_view_rooms.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1023 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1405 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a7/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/config/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1912 2020-03-23 15:46:10.000000 huscy.rooms-0.2.0a7/config/settings.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      234 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a7/config/urls.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.858793 huscy.rooms-0.2.0a7/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/huscy/rooms/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-14 08:48:59.000000 huscy.rooms-0.2.0a7/huscy/rooms/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      171 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      276 2022-12-01 21:18:24.000000 huscy.rooms-0.2.0a7/huscy/rooms/api_urls.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/huscy/rooms/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1299 2020-03-17 07:20:01.000000 huscy.rooms-0.2.0a7/huscy/rooms/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      563 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1029 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      425 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/huscy/rooms/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1023 2023-04-17 10:18:16.000000 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      785 2023-04-17 10:18:16.000000 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:18:16.000000 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       84 2023-04-17 10:18:16.000000 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2023-04-17 10:18:16.000000 huscy.rooms-0.2.0a7/huscy.rooms.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1253 2023-04-17 10:10:53.000000 huscy.rooms-0.2.0a7/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      927 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/conftest.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:18:16.862793 huscy.rooms-0.2.0a7/tests/viewsets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1471 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_building_viewset_create_building.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1497 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_building_viewset_view_buildings.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1478 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_floor_viewset_create_floor.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1405 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_floor_viewset_view_floors.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1536 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_room_viewset_create_room.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1381 2020-03-17 07:19:30.000000 huscy.rooms-0.2.0a7/tests/viewsets/test_room_viewset_view_rooms.py
```

### Comparing `huscy.rooms-0.2.0a6/PKG-INFO` & `huscy.rooms-0.2.0a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.rooms
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
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

### Comparing `huscy.rooms-0.2.0a6/README.md` & `huscy.rooms-0.2.0a7/README.md`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/config/settings.py` & `huscy.rooms-0.2.0a7/config/settings.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/huscy/rooms/migrations/0001_initial.py` & `huscy.rooms-0.2.0a7/huscy/rooms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/huscy/rooms/models.py` & `huscy.rooms-0.2.0a7/huscy/rooms/models.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/huscy/rooms/serializer.py` & `huscy.rooms-0.2.0a7/huscy/rooms/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/huscy/rooms/views.py` & `huscy.rooms-0.2.0a7/huscy/rooms/views.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/huscy.rooms.egg-info/PKG-INFO` & `huscy.rooms-0.2.0a7/huscy.rooms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.rooms
-Version: 0.2.0a6
+Version: 0.2.0a7
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
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

### Comparing `huscy.rooms-0.2.0a6/huscy.rooms.egg-info/SOURCES.txt` & `huscy.rooms-0.2.0a7/huscy.rooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/setup.py` & `huscy.rooms-0.2.0a7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
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

### Comparing `huscy.rooms-0.2.0a6/tests/conftest.py` & `huscy.rooms-0.2.0a7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_building_viewset_create_building.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_building_viewset_create_building.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_building_viewset_view_buildings.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_building_viewset_view_buildings.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_floor_viewset_create_floor.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_floor_viewset_create_floor.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_floor_viewset_view_floors.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_floor_viewset_view_floors.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_room_viewset_create_room.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_room_viewset_create_room.py`

 * *Files identical despite different names*

### Comparing `huscy.rooms-0.2.0a6/tests/viewsets/test_room_viewset_view_rooms.py` & `huscy.rooms-0.2.0a7/tests/viewsets/test_room_viewset_view_rooms.py`

 * *Files identical despite different names*

