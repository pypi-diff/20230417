# Comparing `tmp/huscy.email-recruitment-0.4.0a5.tar.gz` & `tmp/huscy.email-recruitment-0.4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.email-recruitment-0.4.0a5.tar", last modified: Fri Dec  2 09:02:52 2022, max compression
+gzip compressed data, was "huscy.email-recruitment-0.4.0a6.tar", last modified: Mon Apr 17 10:24:52 2023, max compression
```

## Comparing `huscy.email-recruitment-0.4.0a5.tar` & `huscy.email-recruitment-0.4.0a6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1026 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       31 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/config/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2272 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/config/settings.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      191 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/config/urls.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      349 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      195 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1471 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      545 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1303 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1286 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1736 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1026 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1131 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       73 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2022-12-02 09:02:52.000000 huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1249 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/setup.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/tests/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      996 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/conftest.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/tests/services/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      570 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_create_invitation_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      558 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_create_reminder_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      373 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_delete_invitation_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      359 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_delete_reminder_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      694 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_get_invitation_emails.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      676 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_get_reminder_emails.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      838 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_update_invitation_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      800 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/services/test_update_reminder_email.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)       40 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/test_assert_true.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2022-12-02 09:02:52.563957 huscy.email-recruitment-0.4.0a5/tests/viewsets/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5708 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/viewsets/test_invitation_email_viewset.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5554 2022-12-02 08:53:52.000000 huscy.email-recruitment-0.4.0a5/tests/viewsets/test_reminder_email_viewset.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1032 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       31 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/config/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2272 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/config/settings.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      191 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/config/urls.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.329207 huscy.email-recruitment-0.4.0a6/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      349 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      195 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1469 2023-04-17 10:24:51.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      545 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1303 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1286 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1736 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1032 2023-04-17 10:24:52.000000 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1131 2023-04-17 10:24:52.000000 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 10:24:52.000000 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       73 2023-04-17 10:24:52.000000 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       24 2023-04-17 10:24:52.000000 huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1255 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/tests/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      996 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/conftest.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/tests/services/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      570 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_create_invitation_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      558 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_create_reminder_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      373 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_delete_invitation_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      359 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_delete_reminder_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      694 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_get_invitation_emails.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      676 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_get_reminder_emails.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      838 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_update_invitation_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      800 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/services/test_update_reminder_email.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       40 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/test_assert_true.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 10:24:52.333207 huscy.email-recruitment-0.4.0a6/tests/viewsets/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5708 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/viewsets/test_invitation_email_viewset.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5554 2023-04-17 10:19:56.000000 huscy.email-recruitment-0.4.0a6/tests/viewsets/test_reminder_email_viewset.py
```

### Comparing `huscy.email-recruitment-0.4.0a5/PKG-INFO` & `huscy.email-recruitment-0.4.0a6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.email-recruitment
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@cbs.mpg.de, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
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

### Comparing `huscy.email-recruitment-0.4.0a5/config/settings.py` & `huscy.email-recruitment-0.4.0a6/config/settings.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/migrations/0001_initial.py` & `huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/migrations/0001_initial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.3 on 2022-12-02 03:02
+# Generated by Django 4.2 on 2023-04-17 05:24
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/models.py` & `huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/models.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/serializer.py` & `huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/services.py` & `huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/services.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/huscy/email_recruitment/views.py` & `huscy.email-recruitment-0.4.0a6/huscy/email_recruitment/views.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/PKG-INFO` & `huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: huscy.email-recruitment
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
 Author-email: tyapkov@cbs.mpg.de, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
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

### Comparing `huscy.email-recruitment-0.4.0a5/huscy.email_recruitment.egg-info/SOURCES.txt` & `huscy.email-recruitment-0.4.0a6/huscy.email_recruitment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/setup.py` & `huscy.email-recruitment-0.4.0a6/setup.py`

 * *Files 9% similar despite different names*

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

### Comparing `huscy.email-recruitment-0.4.0a5/tests/conftest.py` & `huscy.email-recruitment-0.4.0a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_create_invitation_email.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_create_invitation_email.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_create_reminder_email.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_create_reminder_email.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_get_invitation_emails.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_get_invitation_emails.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_get_reminder_emails.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_get_reminder_emails.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_update_invitation_email.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_update_invitation_email.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/services/test_update_reminder_email.py` & `huscy.email-recruitment-0.4.0a6/tests/services/test_update_reminder_email.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/viewsets/test_invitation_email_viewset.py` & `huscy.email-recruitment-0.4.0a6/tests/viewsets/test_invitation_email_viewset.py`

 * *Files identical despite different names*

### Comparing `huscy.email-recruitment-0.4.0a5/tests/viewsets/test_reminder_email_viewset.py` & `huscy.email-recruitment-0.4.0a6/tests/viewsets/test_reminder_email_viewset.py`

 * *Files identical despite different names*

