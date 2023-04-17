# Comparing `tmp/huscy.subjects-2.1.0.tar.gz` & `tmp/huscy.subjects-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/huscy.subjects-2.1.0.tar", last modified: Mon Dec 12 11:05:26 2022, max compression
+gzip compressed data, was "huscy.subjects-2.1.1.tar", last modified: Mon Apr 17 17:36:32 2023, max compression
```

## Comparing `huscy.subjects-2.1.0.tar` & `huscy.subjects-2.1.1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 bunde     (1000) bunde     (1000)        0 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/
--rw-r--r--   0 bunde     (1000) bunde     (1000)    34523 2020-05-14 12:27:34.000000 huscy.subjects-2.1.0/LICENSE
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     3213 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/PKG-INFO
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     2095 2022-11-10 12:30:24.000000 huscy.subjects-2.1.0/README.md
-drwxrwxr-x   0 bunde     (1000) bunde     (1000)        0 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/huscy/
-drwxrwxr-x   0 bunde     (1000) bunde     (1000)        0 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/huscy/subjects/
--rw-rw-r--   0 bunde     (1000) bunde     (1000)       89 2022-12-09 12:44:24.000000 huscy.subjects-2.1.0/huscy/subjects/__init__.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     2496 2022-10-18 15:42:37.000000 huscy.subjects-2.1.0/huscy/subjects/admin.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      459 2022-12-09 12:44:24.000000 huscy.subjects-2.1.0/huscy/subjects/api_urls.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      186 2022-10-17 14:20:40.000000 huscy.subjects-2.1.0/huscy/subjects/apps.py
-drwxrwxr-x   0 bunde     (1000) bunde     (1000)        0 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/
--rw-r--r--   0 bunde     (1000) bunde     (1000)     4491 2020-11-23 17:38:19.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0001_initial.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     5418 2022-11-10 12:30:24.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     7787 2022-10-17 09:49:42.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0002_auto_20210810_0124.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     1498 2022-10-17 14:20:40.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0003_auto_20211028_1133.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      245 2022-10-17 14:20:40.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0004_delete_note.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     1834 2022-10-17 14:20:40.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0005_auto_20221011_0432.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      287 2022-10-20 08:34:00.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0006_rename_contact_contactold.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     3841 2022-10-20 08:34:00.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0007_contact.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      714 2022-10-20 08:34:00.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0008_auto_20221018_0935.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      251 2022-10-20 08:34:00.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/0009_delete_contactold.py
--rw-r--r--   0 bunde     (1000) bunde     (1000)        0 2020-11-18 13:07:47.000000 huscy.subjects-2.1.0/huscy/subjects/migrations/__init__.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     4388 2022-12-05 15:39:49.000000 huscy.subjects-2.1.0/huscy/subjects/models.py
--rw-r--r--   0 bunde     (1000) bunde     (1000)      187 2020-11-18 13:07:47.000000 huscy.subjects-2.1.0/huscy/subjects/pagination.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      494 2022-10-17 14:20:40.000000 huscy.subjects-2.1.0/huscy/subjects/permissions.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     3796 2022-12-05 15:39:49.000000 huscy.subjects-2.1.0/huscy/subjects/serializers.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     4293 2022-12-05 15:39:49.000000 huscy.subjects-2.1.0/huscy/subjects/services.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      634 2022-12-09 12:44:24.000000 huscy.subjects-2.1.0/huscy/subjects/urls.py
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     4467 2022-12-05 15:39:49.000000 huscy.subjects-2.1.0/huscy/subjects/views.py
-drwxrwxr-x   0 bunde     (1000) bunde     (1000)        0 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     3213 2022-12-12 11:05:25.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/PKG-INFO
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     1062 2022-12-12 11:05:25.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/SOURCES.txt
--rw-rw-r--   0 bunde     (1000) bunde     (1000)        1 2022-12-12 11:05:25.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/dependency_links.txt
--rw-rw-r--   0 bunde     (1000) bunde     (1000)      253 2022-12-12 11:05:25.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/requires.txt
--rw-rw-r--   0 bunde     (1000) bunde     (1000)        6 2022-12-12 11:05:25.000000 huscy.subjects-2.1.0/huscy.subjects.egg-info/top_level.txt
--rw-rw-r--   0 bunde     (1000) bunde     (1000)       38 2022-12-12 11:05:26.000000 huscy.subjects-2.1.0/setup.cfg
--rw-rw-r--   0 bunde     (1000) bunde     (1000)     1931 2022-12-09 12:44:24.000000 huscy.subjects-2.1.0/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 17:36:32.655211 huscy.subjects-2.1.1/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3980 2023-04-17 17:36:32.655211 huscy.subjects-2.1.1/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2095 2023-04-11 15:22:54.000000 huscy.subjects-2.1.1/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 17:36:32.647210 huscy.subjects-2.1.1/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 17:36:32.651210 huscy.subjects-2.1.1/huscy/subjects/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-04-11 15:22:54.000000 huscy.subjects-2.1.1/huscy/subjects/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2496 2022-10-17 12:29:15.000000 huscy.subjects-2.1.1/huscy/subjects/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      459 2022-12-09 13:23:52.000000 huscy.subjects-2.1.1/huscy/subjects/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-21 19:01:54.000000 huscy.subjects-2.1.1/huscy/subjects/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 17:36:32.655211 huscy.subjects-2.1.1/huscy/subjects/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4491 2020-11-23 17:38:26.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5418 2022-11-10 10:58:50.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     7787 2021-10-28 16:39:39.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0002_auto_20210810_0124.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1498 2021-10-28 16:39:39.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0003_auto_20211028_1133.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      245 2022-10-11 07:31:35.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0004_delete_note.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1834 2022-10-11 14:39:42.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0005_auto_20221011_0432.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      287 2022-10-20 08:32:27.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0006_rename_contact_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3841 2022-10-20 08:32:27.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0007_contact.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      714 2022-10-20 08:32:27.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0008_auto_20221018_0935.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      251 2022-10-20 08:32:27.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/0009_delete_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-14 14:27:02.000000 huscy.subjects-2.1.1/huscy/subjects/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4388 2022-10-20 08:32:27.000000 huscy.subjects-2.1.1/huscy/subjects/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      187 2020-05-14 14:27:02.000000 huscy.subjects-2.1.1/huscy/subjects/pagination.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      494 2022-10-11 07:31:35.000000 huscy.subjects-2.1.1/huscy/subjects/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3796 2022-10-17 12:29:15.000000 huscy.subjects-2.1.1/huscy/subjects/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4293 2022-11-10 10:58:50.000000 huscy.subjects-2.1.1/huscy/subjects/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      634 2022-12-09 13:23:52.000000 huscy.subjects-2.1.1/huscy/subjects/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4467 2022-11-10 10:58:50.000000 huscy.subjects-2.1.1/huscy/subjects/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 17:36:32.651210 huscy.subjects-2.1.1/huscy.subjects.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3980 2023-04-17 17:36:32.000000 huscy.subjects-2.1.1/huscy.subjects.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1054 2023-04-17 17:36:32.000000 huscy.subjects-2.1.1/huscy.subjects.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 17:36:32.000000 huscy.subjects-2.1.1/huscy.subjects.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      253 2023-04-17 17:36:32.000000 huscy.subjects-2.1.1/huscy.subjects.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 17:36:32.000000 huscy.subjects-2.1.1/huscy.subjects.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 17:36:32.655211 huscy.subjects-2.1.1/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1937 2023-04-17 15:12:04.000000 huscy.subjects-2.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `huscy.subjects-2.1.0/PKG-INFO` & `huscy.subjects-2.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 Metadata-Version: 2.1
 Name: huscy.subjects
-Version: 2.1.0
+Version: 2.1.1
 Summary: Managing subjects in a human research context.
 Home-page: https://bitbucket.org/huscy/subjects
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: huscy.subjects
+        ======
+        
+        ![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
+        ![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
+        ![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
+        ![PyPI License](https://img.shields.io/pypi/l/huscy-subjects?color=yellow)
+        ![Python Versions](https://img.shields.io/pypi/pyversions/huscy-subjects.svg)
+        ![Django Versions](https://img.shields.io/pypi/djversions/huscy-subjects)
+        
+        
+        
+        Requirements
+        ------
+        
+        - Python 3.8+
+        - A supported version of Django
+        
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
+        
+        
+        
+        Installation
+        ------
+        
+        To install `husy.subjects` simply run:
+        
+            pip install huscy.subjects
+        
+        Add `huscy.subjects` and further required apps to `INSTALLED_APPS` in your `settings.py`:
+        
+        ```python
+        INSTALLED_APPS = (
+        	...
+        	'django_countries',
+        	'guardian',
+        	'phonenumber_field',
+        	'rest_framework',
+        
+        	'huscy.subjects',
+        )
+        ```
+        
+        Hook the urls from `huscy.subjects` into your `urls.py`:
+        
+        ```python
+        urlpatterns = [
+        	...
+        	path('api/', include('huscy.subjects.urls')),
+        ]
+        ```
+        
+        Create `huscy.subjects` database tables by running:
+        
+            python manage.py migrate
+        
+        
+        
+        Configuration
+        ------
+        
+        There are some settings to configure the service. These settings have be added to `settings.py`.
+        
+        
+        | Name | Default value | Description |
+        | -------- | -------- | -------- |
+        | HUSCY_SUBJECTS_AGE_OF_MAJORITY | 18 | Specifies the age of majority. |
+        | HUSCY_SUBJECTS_SUBJECT_VIEWSET_MAX_RESULT_COUNT | 500 | Specifies the maximum number of subjects returned by the queryset in the SubjectViewSet. |
+        
+        
+        
+        Development
+        ------
+        
+        Install PostgreSQL and create a database user called `huscy` and a database called `huscy`.
+        
+            sudo -u postgres createdb huscy
+            sudo -u postgres createuser -d huscy
+            sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE huscy TO huscy;"
+            sudo -u postgres psql -c "ALTER USER huscy WITH PASSWORD '123';"
+        
+        Check out the repository and start your virtual environment (if necessary).
+        
+        Install dependencies:
+        
+            make install
+        
+        Create database tables:
+        
+            make migrate
+        
+        Run tests to see if everything works fine:
+        
+            make test
+        
+Platform: UNKNOWN
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
-License-File: LICENSE
-
-huscy.subjects
-======
-
-![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
-![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
-![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
-![PyPI License](https://img.shields.io/pypi/l/huscy-subjects?color=yellow)
-![Python Versions](https://img.shields.io/pypi/pyversions/huscy-subjects.svg)
-![Django Versions](https://img.shields.io/pypi/djversions/huscy-subjects)
-
-
-
-Requirements
-------
-
-- Python 3.7+
-- A supported version of Django
-
-Tox tests on Django versions 3.2, 4.0 and 4.1.
-
-
-
-Installation
-------
-
-To install `husy.subjects` simply run:
-
-    pip install huscy.subjects
-
-Add `huscy.subjects` and further required apps to `INSTALLED_APPS` in your `settings.py`:
-
-```python
-INSTALLED_APPS = (
-	...
-	'django_countries',
-	'guardian',
-	'phonenumber_field',
-	'rest_framework',
-
-	'huscy.subjects',
-)
-```
-
-Hook the urls from `huscy.subjects` into your `urls.py`:
-
-```python
-urlpatterns = [
-	...
-	path('api/', include('huscy.subjects.urls')),
-]
-```
-
-Create `huscy.subjects` database tables by running:
-
-    python manage.py migrate
-
-
-
-Configuration
-------
-
-There are some settings to configure the service. These settings have be added to `settings.py`.
-
-
-| Name | Default value | Description |
-| -------- | -------- | -------- |
-| HUSCY_SUBJECTS_AGE_OF_MAJORITY | 18 | Specifies the age of majority. |
-| HUSCY_SUBJECTS_SUBJECT_VIEWSET_MAX_RESULT_COUNT | 500 | Specifies the maximum number of subjects returned by the queryset in the SubjectViewSet. |
-
-
-
-Development
-------
-
-Install PostgreSQL and create a database user called `huscy` and a database called `huscy`.
-
-    sudo -u postgres createdb huscy
-    sudo -u postgres createuser -d huscy
-    sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE huscy TO huscy;"
-    sudo -u postgres psql -c "ALTER USER huscy WITH PASSWORD '123';"
-
-Check out the repository and start your virtual environment (if necessary).
-
-Install dependencies:
-
-    make install
-
-Create database tables:
-
-    make migrate
-
-Run tests to see if everything works fine:
-
-    make test
```

### Comparing `huscy.subjects-2.1.0/README.md` & `huscy.subjects-2.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ![Django Versions](https://img.shields.io/pypi/djversions/huscy-subjects)
 
 
 
 Requirements
 ------
 
-- Python 3.7+
+- Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.0 and 4.1.
+Tox tests on Django versions 3.2, 4.1 and 4.2.
 
 
 
 Installation
 ------
 
 To install `husy.subjects` simply run:
```

### Comparing `huscy.subjects-2.1.0/huscy/subjects/admin.py` & `huscy.subjects-2.1.1/huscy/subjects/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0001_initial.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0002_auto_20210810_0124.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0002_auto_20210810_0124.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0003_auto_20211028_1133.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0003_auto_20211028_1133.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0005_auto_20221011_0432.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0005_auto_20221011_0432.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0007_contact.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0007_contact.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/migrations/0008_auto_20221018_0935.py` & `huscy.subjects-2.1.1/huscy/subjects/migrations/0008_auto_20221018_0935.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/models.py` & `huscy.subjects-2.1.1/huscy/subjects/models.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/serializers.py` & `huscy.subjects-2.1.1/huscy/subjects/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/services.py` & `huscy.subjects-2.1.1/huscy/subjects/services.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/urls.py` & `huscy.subjects-2.1.1/huscy/subjects/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy/subjects/views.py` & `huscy.subjects-2.1.1/huscy/subjects/views.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.0/huscy.subjects.egg-info/PKG-INFO` & `huscy.subjects-2.1.1/huscy.subjects.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 Metadata-Version: 2.1
 Name: huscy.subjects
-Version: 2.1.0
+Version: 2.1.1
 Summary: Managing subjects in a human research context.
 Home-page: https://bitbucket.org/huscy/subjects
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
+Description: huscy.subjects
+        ======
+        
+        ![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
+        ![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
+        ![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
+        ![PyPI License](https://img.shields.io/pypi/l/huscy-subjects?color=yellow)
+        ![Python Versions](https://img.shields.io/pypi/pyversions/huscy-subjects.svg)
+        ![Django Versions](https://img.shields.io/pypi/djversions/huscy-subjects)
+        
+        
+        
+        Requirements
+        ------
+        
+        - Python 3.8+
+        - A supported version of Django
+        
+        Tox tests on Django versions 3.2, 4.1 and 4.2.
+        
+        
+        
+        Installation
+        ------
+        
+        To install `husy.subjects` simply run:
+        
+            pip install huscy.subjects
+        
+        Add `huscy.subjects` and further required apps to `INSTALLED_APPS` in your `settings.py`:
+        
+        ```python
+        INSTALLED_APPS = (
+        	...
+        	'django_countries',
+        	'guardian',
+        	'phonenumber_field',
+        	'rest_framework',
+        
+        	'huscy.subjects',
+        )
+        ```
+        
+        Hook the urls from `huscy.subjects` into your `urls.py`:
+        
+        ```python
+        urlpatterns = [
+        	...
+        	path('api/', include('huscy.subjects.urls')),
+        ]
+        ```
+        
+        Create `huscy.subjects` database tables by running:
+        
+            python manage.py migrate
+        
+        
+        
+        Configuration
+        ------
+        
+        There are some settings to configure the service. These settings have be added to `settings.py`.
+        
+        
+        | Name | Default value | Description |
+        | -------- | -------- | -------- |
+        | HUSCY_SUBJECTS_AGE_OF_MAJORITY | 18 | Specifies the age of majority. |
+        | HUSCY_SUBJECTS_SUBJECT_VIEWSET_MAX_RESULT_COUNT | 500 | Specifies the maximum number of subjects returned by the queryset in the SubjectViewSet. |
+        
+        
+        
+        Development
+        ------
+        
+        Install PostgreSQL and create a database user called `huscy` and a database called `huscy`.
+        
+            sudo -u postgres createdb huscy
+            sudo -u postgres createuser -d huscy
+            sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE huscy TO huscy;"
+            sudo -u postgres psql -c "ALTER USER huscy WITH PASSWORD '123';"
+        
+        Check out the repository and start your virtual environment (if necessary).
+        
+        Install dependencies:
+        
+            make install
+        
+        Create database tables:
+        
+            make migrate
+        
+        Run tests to see if everything works fine:
+        
+            make test
+        
+Platform: UNKNOWN
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
-License-File: LICENSE
-
-huscy.subjects
-======
-
-![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
-![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
-![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
-![PyPI License](https://img.shields.io/pypi/l/huscy-subjects?color=yellow)
-![Python Versions](https://img.shields.io/pypi/pyversions/huscy-subjects.svg)
-![Django Versions](https://img.shields.io/pypi/djversions/huscy-subjects)
-
-
-
-Requirements
-------
-
-- Python 3.7+
-- A supported version of Django
-
-Tox tests on Django versions 3.2, 4.0 and 4.1.
-
-
-
-Installation
-------
-
-To install `husy.subjects` simply run:
-
-    pip install huscy.subjects
-
-Add `huscy.subjects` and further required apps to `INSTALLED_APPS` in your `settings.py`:
-
-```python
-INSTALLED_APPS = (
-	...
-	'django_countries',
-	'guardian',
-	'phonenumber_field',
-	'rest_framework',
-
-	'huscy.subjects',
-)
-```
-
-Hook the urls from `huscy.subjects` into your `urls.py`:
-
-```python
-urlpatterns = [
-	...
-	path('api/', include('huscy.subjects.urls')),
-]
-```
-
-Create `huscy.subjects` database tables by running:
-
-    python manage.py migrate
-
-
-
-Configuration
-------
-
-There are some settings to configure the service. These settings have be added to `settings.py`.
-
-
-| Name | Default value | Description |
-| -------- | -------- | -------- |
-| HUSCY_SUBJECTS_AGE_OF_MAJORITY | 18 | Specifies the age of majority. |
-| HUSCY_SUBJECTS_SUBJECT_VIEWSET_MAX_RESULT_COUNT | 500 | Specifies the maximum number of subjects returned by the queryset in the SubjectViewSet. |
-
-
-
-Development
-------
-
-Install PostgreSQL and create a database user called `huscy` and a database called `huscy`.
-
-    sudo -u postgres createdb huscy
-    sudo -u postgres createuser -d huscy
-    sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE huscy TO huscy;"
-    sudo -u postgres psql -c "ALTER USER huscy WITH PASSWORD '123';"
-
-Check out the repository and start your virtual environment (if necessary).
-
-Install dependencies:
-
-    make install
-
-Create database tables:
-
-    make migrate
-
-Run tests to see if everything works fine:
-
-    make test
```

### Comparing `huscy.subjects-2.1.0/huscy.subjects.egg-info/SOURCES.txt` & `huscy.subjects-2.1.1/huscy.subjects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 huscy.subjects.egg-info/PKG-INFO
 huscy.subjects.egg-info/SOURCES.txt
 huscy.subjects.egg-info/dependency_links.txt
 huscy.subjects.egg-info/requires.txt
 huscy.subjects.egg-info/top_level.txt
```

### Comparing `huscy.subjects-2.1.0/setup.py` & `huscy.subjects-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
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

