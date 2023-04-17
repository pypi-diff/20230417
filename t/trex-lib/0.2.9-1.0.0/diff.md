# Comparing `tmp/trex-lib-0.2.9.tar.gz` & `tmp/trex-lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trex-lib-0.2.9.tar", last modified: Thu Feb  4 01:33:21 2021, max compression
+gzip compressed data, was "trex-lib-1.0.0.tar", last modified: Mon Apr 17 03:27:42 2023, max compression
```

## Comparing `trex-lib-0.2.9.tar` & `trex-lib-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.275596 trex-lib-0.2.9/
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-0.2.9/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-04 01:33:21.275773 trex-lib-0.2.9/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-0.2.9/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2021-02-04 01:33:21.276412 trex-lib-0.2.9/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      877 2021-02-04 01:32:47.000000 trex-lib-0.2.9/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.259700 trex-lib-0.2.9/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)      957 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)      103 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2021-02-04 01:33:21.000000 trex-lib-0.2.9/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.260193 trex-lib-0.2.9/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-0.2.9/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4200 2021-01-21 09:42:37.000000 trex-lib-0.2.9/trexlib/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.261058 trex-lib-0.2.9/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-0.2.9/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.261673 trex-lib-0.2.9/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-0.2.9/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-0.2.9/trexlib/libs/flask_wtf/crsf_ext.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.266218 trex-lib-0.2.9/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-0.2.9/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.273120 trex-lib-0.2.9/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-0.2.9/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-0.2.9/trexlib/utils/common/cache_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3162 2021-02-03 09:11:17.000000 trex-lib-0.2.9/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-0.2.9/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-0.2.9/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2345 2020-09-01 10:20:51.000000 trex-lib-0.2.9/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-0.2.9/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-0.2.9/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1361 2020-09-04 07:32:41.000000 trex-lib-0.2.9/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      823 2020-09-04 07:16:17.000000 trex-lib-0.2.9/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      808 2020-11-09 09:40:17.000000 trex-lib-0.2.9/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2021-02-04 01:33:21.274738 trex-lib-0.2.9/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-0.2.9/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12742 2021-01-26 10:05:22.000000 trex-lib-0.2.9/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3477 2021-01-22 08:40:12.000000 trex-lib-0.2.9/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-0.2.9/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3140 2021-01-22 09:14:05.000000 trex-lib-0.2.9/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4739 2021-01-06 06:55:12.000000 trex-lib-0.2.9/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-0.2.9/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.552711 trex-lib-1.0.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.0/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.0/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-04-17 03:27:42.553095 trex-lib-1.0.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.0/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-17 03:27:42.554207 trex-lib-1.0.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      911 2023-04-17 03:26:54.000000 trex-lib-1.0.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.530294 trex-lib-1.0.0/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-04-17 03:27:42.000000 trex-lib-1.0.0/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1247 2023-04-17 03:27:42.000000 trex-lib-1.0.0/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-17 03:27:42.000000 trex-lib-1.0.0/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)      124 2023-04-17 03:27:42.000000 trex-lib-1.0.0/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-04-17 03:27:42.000000 trex-lib-1.0.0/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.530961 trex-lib-1.0.0/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.0/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5304 2023-03-08 04:35:45.000000 trex-lib-1.0.0/trexlib/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.531758 trex-lib-1.0.0/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.0/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.532171 trex-lib-1.0.0/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.0/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.0/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.533597 trex-lib-1.0.0/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.0/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.0/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.534717 trex-lib-1.0.0/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.0/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.0/trexlib/libs/flask_wtf/crsf_ext.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.539313 trex-lib-1.0.0/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.0/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.547789 trex-lib-1.0.0/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.0/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-1.0.0/trexlib/utils/common/cache_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.0/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.0/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.0/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.0/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2707 2021-09-16 10:19:23.000000 trex-lib-1.0.0/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.0/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.0/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.0/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.0/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.0/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.0/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:27:42.551863 trex-lib-1.0.0/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.0/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.0/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4051 2022-09-09 02:31:34.000000 trex-lib-1.0.0/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.0/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.0/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.0/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5535 2022-08-25 01:59:10.000000 trex-lib-1.0.0/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.0/trexlib/utils/url_util.py
```

### Comparing `trex-lib-0.2.9/setup.py` & `trex-lib-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='0.2.9',
+     version='1.0.0',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
@@ -22,10 +22,11 @@
           'cryptography',
           'urllib3',
           'phonenumbers',
           'email_validator',
           'Flask-Caching',
           'Flask-Script',
           'basicauth',
+          'flask-restful>=0.3.9',
       ],
  )
```

### Comparing `trex-lib-0.2.9/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.0.0/trex_lib.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 trex_lib.egg-info/PKG-INFO
 trex_lib.egg-info/SOURCES.txt
 trex_lib.egg-info/dependency_links.txt
 trex_lib.egg-info/requires.txt
 trex_lib.egg-info/top_level.txt
 trexlib/__init__.py
 trexlib/conf.py
 trexlib/libs/__init__.py
+trexlib/libs/controllers/__init__.py
+trexlib/libs/controllers/task_base_routes.py
+trexlib/libs/firebase/__init__.py
+trexlib/libs/firebase/firebase_helper.py
 trexlib/libs/flask_wtf/__init__.py
 trexlib/libs/flask_wtf/crsf_ext.py
 trexlib/utils/__init__.py
 trexlib/utils/crypto_util.py
 trexlib/utils/log_util.py
 trexlib/utils/security_util.py
 trexlib/utils/string_util.py
 trexlib/utils/url_util.py
 trexlib/utils/common/__init__.py
 trexlib/utils/common/cache_util.py
 trexlib/utils/common/common_util.py
 trexlib/utils/common/conftest.py
 trexlib/utils/common/crm_util.py
+trexlib/utils/common/currency_util.py
 trexlib/utils/common/date_util.py
 trexlib/utils/common/float_util.py
+trexlib/utils/common/format_util.py
 trexlib/utils/common/pagination_util.py
 trexlib/utils/common/phone_util.py
 trexlib/utils/common/user_util.py
 trexlib/utils/google/__init__.py
 trexlib/utils/google/bigquery_util.py
-trexlib/utils/google/cloud_tasks_util.py
+trexlib/utils/google/cloud_tasks_util.py
+trexlib/utils/google/gcloud_util.py
```

### Comparing `trex-lib-0.2.9/trexlib/utils/common/crm_util.py` & `trex-lib-1.0.0/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.9/trexlib/utils/common/date_util.py` & `trex-lib-1.0.0/trexlib/utils/common/date_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 @author: jacklok
 '''
  
 from datetime import datetime, timedelta
 from dateutil.relativedelta import relativedelta
 
+
 def parse_date(date_value, date_separator='/', full_year_date_format='%d/%m/%Y', short_year_date_format='%d/%m/%y'):
     if date_value is not None:
         #logging.info('parse_date: date_value=%s', date_value)
         _d_array = date_value.split(date_separator)
         if len(_d_array)==3:
             if len(_d_array[2])==4:
                 _datetime = datetime.strptime(date_value, full_year_date_format)
@@ -21,14 +22,17 @@
     return None
 
 def parse_datetime(date_value, parse_format='%d-%m-%Y %H:%M:%S'):
     if date_value:
         return datetime.strptime(date_value, parse_format)
     return None
 
+def convert_date_to_datetime(date_value):
+    return datetime.combine(date_value, datetime.min.time())
+
 def get_gmt_datetime_from_gmt(gmt):
     now = datetime.now()
     return now + timedelta(hours=gmt)
 
 def convert_datetime_from_gmt_hours(gmt_hours, datetime_value):
     return datetime_value + timedelta(hours=gmt_hours)
 
@@ -57,7 +61,19 @@
             origin_date = origin_date + timedelta(milliseconds=millisecond)
 
         #logging.info('increase_date after increased: origin_date=%s', origin_date)
 
         return origin_date
     else:
         return origin_date
+    
+def last_day_of_month(date):
+    if date.month == 12:
+        return date.replace(day=31)
+    return date.replace(month=date.month+1, day=1) - timedelta(days=1)
+
+def to_day_of_year(datetime_input):
+    return datetime_input.timetuple().tm_yday
+    
+
+
+
```

### Comparing `trex-lib-0.2.9/trexlib/utils/common/pagination_util.py` & `trex-lib-1.0.0/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-0.2.9/trexlib/utils/common/phone_util.py` & `trex-lib-1.0.0/trexlib/utils/common/phone_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 '''
 Created on 3 Sep 2020
 
 @author: jacklok
 '''
-from datetime import date
 import phonenumbers
 from phonenumbers import carrier
 from phonenumbers.phonenumberutil import number_type
-from trexlib import conf
 import logging 
-from six import string_types
+from trexlib.utils.log_util import get_tracelog
 
 logger = logging.getLogger('phone_util')
 
 def is_mobile_phone(phone_no):
     if phone_no:
-        is_valid = False
         try:
-            phone_no_obj = phonenumbers.parse(phone_no)
-            logging.info('phone_no_obj=%s', phone_no_obj)
+            phone_no_obj = phonenumbers.parse(phone_no, _check_region=False)
+            logger.debug('phone_no_obj=%s', phone_no_obj)
             ntype = number_type(phone_no_obj)
-            logging.info('ntype=%s', ntype)
+            logger.debug('ntype=%s', ntype)
             return carrier._is_mobile(ntype)
         except:
+            logger.error('Failed to parse phone no (%s) due to %s', phone_no, get_tracelog())
             return False
     else:
         return False
 
-def normalized_mobile_phone(phone_no, default_country_code=conf.DEFAULT_COUNTRY_CODE.upper()):
+def normalized_mobile_phone(phone_no):
     if is_mobile_phone(phone_no):
         try:
-            parsed_mobile_phone = phonenumbers.parse(phone_no, region=default_country_code)
+            parsed_mobile_phone = phonenumbers.parse(phone_no, _check_region=False)
             return '+%s%s' % (parsed_mobile_phone.country_code, parsed_mobile_phone.national_number)
         except:
             return None
     return None
 
-def format_mobile_phone(phone_no, default_country_code=conf.DEFAULT_COUNTRY_CODE.upper()):
-    parsed_mobile_phone = phonenumbers.parse(phone_no, region=default_country_code)
-    return '+%s%s' % (parsed_mobile_phone.country_code, parsed_mobile_phone.national_number)
```

### Comparing `trex-lib-0.2.9/trexlib/utils/common/user_util.py` & `trex-lib-1.0.0/trexlib/utils/common/user_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
 Created on 29 Apr 2020
 
 @author: jacklok
 '''
 import hashlib
 import logging
-from urllib.parse import urlencode, quote_plus 
+from six.moves.urllib.parse import urlencode, quote_plus
  
-logger = logging.getLogger('user_util') 
+logger = logging.getLogger('lib') 
  
 def get_gravatar_url(email):
     
     #default = "https://www.example.com/default.jpg"
     size = 40
     
     email = email.encode('utf-8')
     
-    logging.debug('email=%s', email)
+    logger.debug('email=%s', email)
     # construct the url
     hashed_email = hashlib.md5(email.lower()).hexdigest()
     logger.debug('hashed_email=%s', hashed_email)
     gravatar_url = "https://www.gravatar.com/avatar/" + hashlib.md5(email.lower()).hexdigest() + "?"
     #gravatar_url += urlencode({'d':default, 's':str(size)}, quote_via=quote_plus)
     gravatar_url += urlencode({'s':str(size)}, quote_via=quote_plus)
```

### Comparing `trex-lib-0.2.9/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.0.0/trexlib/utils/google/bigquery_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,37 +8,35 @@
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 import logging
 from datetime import datetime, date, time
 from google.cloud.bigquery.dataset import DatasetReference
 import uuid
 
-logger = logging.getLogger('debug')
+logger = logging.getLogger('import')
 
-def create_bigquery_client(info=None, credential_filepath=None):
+def create_bigquery_client(info=None, credential_filepath=None, project_id=None):
+    cred = None
+    
     if info:
         cred = service_account.Credentials.from_service_account_info(info)
         
     else:
         if credential_filepath:
             cred = service_account.Credentials.from_service_account_file(credential_filepath)
-        else:
-            cred = service_account.Credentials.from_service_account_file(
-                                                            lib_conf.BIGQUERY_SERVICE_CREDENTIAL_PATH,
-                                                            scopes=["https://www.googleapis.com/auth/cloud-platform", 
-                                                                    "https://www.googleapis.com/auth/bigquery.insertdata"
-                                                                    ]
-                                                            )
-
-    client = bigquery.Client(project=lib_conf.BIGQUERY_GCLOUD_PROJECT_ID, credentials=cred, location=lib_conf.BIGQUERY_GCLOUD_LOCATION)
-    
-    return client 
+        
+            
+    if cred:
+        client = bigquery.Client(project=project_id, credentials=cred)
+        
+        return client 
 
-def create_dataset_reference(dataset_name):
-    dataset_ref = DatasetReference(lib_conf.BIGQUERY_GCLOUD_PROJECT_ID, dataset_name)
+def create_dataset_reference(project_id, dataset_name):
+    #dataset_ref = DatasetReference(lib_conf.BIGQUERY_GCLOUD_PROJECT_ID, dataset_name)
+    dataset_ref = DatasetReference(project_id, dataset_name)
     return dataset_ref
 
 
 def if_dataset_exists(bigquery_client, dataset_ref):
     
     try:
         bigquery_client.get_dataset(dataset_ref)
@@ -55,15 +53,19 @@
 
 
 def create_table_from_template(dataset_name, table_name, table_scheme, table_name_surfix=None, 
                                partition_value=None, bigquery_client=None, final_table_name=None):
     if bigquery_client is None:
         bigquery_client   = create_bigquery_client()
     
-    dataset_ref = create_dataset_reference(dataset_name)
+    project_id = bigquery_client.project
+    
+    logger.debug('create_table_from_template: project_id=%s', project_id)
+    
+    dataset_ref = create_dataset_reference(project_id, dataset_name)
     
     if if_dataset_exists(bigquery_client, dataset_ref) is False:
         logger.debug('dataset(%s) is not exist, thus going to create it', dataset_name)
         bigquery_client.create_dataset(dataset_ref, timeout=30)
     
     
     logger.debug('dataset_ref=%s' , dataset_ref)
@@ -228,28 +230,34 @@
         serialized_dict = {}
         
         for k,v in data_dict.items():
             serialized_dict[k] = default_serializable(v)
             
         serialize_data_to_stream_list.append(serialized_dict)
         
+    logger.debug('serialize_data_to_stream_list=%s' , serialize_data_to_stream_list)
             
     __errors = bigquery_client.insert_rows_json(created_table, serialize_data_to_stream_list)
+    
+    logger.debug('==============================================')
+    logger.debug('__errors=%s' , __errors)
+    logger.debug('==============================================')
             
     if len(__errors)>0:
         errors.extend(__errors)
             
     return errors
 
 def stream_data_by_datetime_partition(bigquery_client, dataset_name, table_template_name, table_scheme, data_dict_to_stream, column_name_used_to_partition=None, 
                              partition_date=False, partition_month=False, partition_year=False):
     
     errors                      = []
     partition_date_formation    = None
     logger.debug('table_scheme=%s' , table_scheme)
+    logger.debug('column_name_used_to_partition=%s' , column_name_used_to_partition)
     
     if column_name_used_to_partition and (partition_date or partition_month or partition_year):
         logger.debug('partition_date=%s' , partition_date)
         logger.debug('partition_month=%s' , partition_month)
         logger.debug('partition_year=%s' , partition_year)
         
         if partition_date:
@@ -263,22 +271,25 @@
         
         logger.debug('partition_date_formation=%s', partition_date_formation)
     
     
     for table_name_suffix, data_list_to_stream in data_dict_to_stream.items():
     
         partition_dict              =  {}
-        
+        partition_value_str         = ''
         #partition data first
         for data_dict in data_list_to_stream:
             if partition_date_formation:
                 partition_value         = data_dict.get(column_name_used_to_partition)
-                partition_value_str     = partition_value.strftime(partition_date_formation)
-            else:
-                partition_value_str     = ''    
+                
+                logger.debug('partition_value=%s', partition_value)
+                
+                if partition_value:
+                    partition_value_str     = partition_value.strftime(partition_date_formation)
+                
             
             partition_list = partition_dict.get(partition_value_str)
             if partition_list is None:
                 partition_list = []
             
             serialized_dict = {}
             
@@ -324,18 +335,18 @@
             if job.error_result:
                 raise RuntimeError(job.errors)
             return
         time.sleep(1)  
 
 def execute_query(bigquery_client, query):
     job_id = str(uuid.uuid4())
-    
-    query_job = bigquery_client.query(query, job_id=job_id)
-    
-    return query_job.result()
+    if bigquery_client:
+        query_job = bigquery_client.query(query, job_id=job_id)
+        
+        return query_job.result()
         
 def process_job_result_into_category_and_count(job_result_rows):
     row_list = []
     for row in job_result_rows:
         #logger.debug(row)
         column_dict = {}
         category_value = row[0]
@@ -349,8 +360,7 @@
         column_dict['count']     = count
         
         row_list.append(column_dict)
     
     return row_list          
         
     
-
```

### Comparing `trex-lib-0.2.9/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.0.0/trexlib/utils/google/cloud_tasks_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,39 +7,48 @@
 from trexlib import conf as lib_conf
 import logging, json
 from datetime import datetime, timedelta
 from google.oauth2 import service_account 
 from google.protobuf import timestamp_pb2
 from trexlib.utils.security_util import create_basic_authentication, verfiy_basic_authentication
 from trexlib.utils.string_util import random_string
+#from trexlib.conf import SYSTEM_TASK_SERVICE_ACCOUNT_KEY, SYSTEM_TASK_GCLOUD_PROJECT_ID, SYSTEM_TASK_GCLOUD_LOCATION, SYSTEM_TASK_SERVICE_ACCOUNT_EMAIL
 
-logger = logging.getLogger('debug')
+logger = logging.getLogger('utils-debug')
 
-def create_task(task_url, queue_name, payload=None, in_seconds=None, http_method='get', headers=None): 
+def create_task(task_url, queue_name, payload=None, in_seconds=None, http_method='get', headers=None, 
+                credential_path=None, 
+                project_id=None, 
+                location=None, 
+                service_email=None): 
     
     cred = service_account.Credentials.from_service_account_file(
-                                                            lib_conf.TASK_SERVICE_CREDENTIAL_PATH,
+                                                            credential_path,
                                                             scopes=["https://www.googleapis.com/auth/cloud-platform", 
                                                                     "https://www.googleapis.com/auth/cloud-tasks"
                                                                     ]
                                                             )
     
     task_id = random_string(12)
     
     client = tasks_v2.CloudTasksClient(credentials=cred)
         
-    parent = client.queue_path(lib_conf.TASK_GCLOUD_PROJECT_ID, lib_conf.TASK_GCLOUD_LOCATION, queue_name)
+    parent = client.queue_path(project_id, location, queue_name)
     
-    logger.debug(">>>>>>>>>>>>>>>>create_task: task_url=%s", task_url)
+    logger.info(">>>>>>>>>>>>>>>>create_task: task_url=%s", task_url)
+    logger.info(">>>>>>>>>>>>>>>>create_task: credential_path=%s", credential_path)
+    logger.info(">>>>>>>>>>>>>>>>create_task: project_id=%s", project_id)
+    logger.info(">>>>>>>>>>>>>>>>create_task: location=%s", location)
+    logger.info(">>>>>>>>>>>>>>>>create_task: service_email=%s", service_email)
     
     task = {
         "http_request": {  # Specify the type of request.
-                         "http_method"  : tasks_v2.HttpMethod.POST if http_method=='post' else tasks_v2.HttpMethod.GET,
+                         "http_method"  : tasks_v2.HttpMethod.POST if http_method.lower()=='post' or payload is not None else tasks_v2.HttpMethod.GET,
                          "url"          : task_url,  
-                         "oidc_token"   : {"service_account_email": lib_conf.TASK_SERVICE_ACCOUNT_EMAIL},
+                         "oidc_token"   : {"service_account_email": service_email},
                         }
         }
     
     if payload is not None:
         if isinstance(payload, dict):
             # Convert dict to JSON string
             payload = json.dumps(payload)
@@ -50,34 +59,35 @@
         converted_payload = payload.encode()
         
         logger.debug('create_task: converted_payload=%s', converted_payload)
     
         # Add the payload to the request.
         task["http_request"]["body"] = converted_payload
     
+    
     if headers is not None:
         for k,v in headers.items():
             task["http_request"]["headers"][k]=v
             
     
-    task["http_request"]["headers"]['X-task-id']= task_id
-    task["http_request"]["headers"]['X-task-token']= create_task_authenticated_token(task_id)
+    task["http_request"]["headers"]['X-task-id']        = task_id
+    task["http_request"]["headers"]['X-task-token']     = create_task_authenticated_token(task_id)
         
     if in_seconds is not None:
         # Convert "seconds from now" into an rfc3339 datetime string.
         d = datetime.utcnow() + timedelta(seconds=in_seconds)
     
         # Create Timestamp protobuf.
         timestamp = timestamp_pb2.Timestamp()
         timestamp.FromDatetime(d)
     
         # Add the timestamp to the tasks.
         task["schedule_time"] = timestamp    
     
-    logger.debug('task["http_request"]["headers"]=%s', task["http_request"]["headers"])
+    logger.info('task["http_request"]["headers"]=%s', task["http_request"].get("headers"))
     
     response = client.create_task(request={"parent": parent, "task": task})
     
     return response
 
 
 def create_task_authenticated_token(id):
```

### Comparing `trex-lib-0.2.9/trexlib/utils/security_util.py` & `trex-lib-1.0.0/trexlib/utils/security_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import hashlib, hmac, time, uuid, json
 from trexlib import conf
 import logging
 from basicauth import encode as basic_encode, decode as basic_decode
 
-logger = logging.getLogger('debug')
+logger = logging.getLogger('lib')
 
 #-----------------------------------------------------------------
 # Password Hashing & Blending
 # DO NOT CHANGE AFTER DEPLOYED TO PRODUCTION
 #-----------------------------------------------------------------
 def hash_password(unique_id, password):
     # sha512 hashing with custom algorithm
     hashed_password = ""
     
     if password and unique_id:
         #password = password.decode('utf-8')
-        logging.debug('unique_id=%s', unique_id)
-        logging.debug('password=%s', password)
+        logger.debug('unique_id=%s', unique_id)
+        logger.debug('password=%s', password)
+        logger.debug('conf.MAX_PASSWORD_LENGTH=%s', conf.MAX_PASSWORD_LENGTH)
+        
         blended_password = blend_password(unique_id, password)
-        logging.debug('blended_password=%s', blended_password)
-        logging.debug('conf.MAX_PASSWORD_LENGTH=%s', conf.MAX_PASSWORD_LENGTH)
+        logger.debug('blended_password=%s', blended_password)
+        
         
         password_salt = conf.SECRET_KEY 
         
+        logger.debug('password_salt=%s', password_salt)
+        
         hash_512 = hashlib.sha512()
         hash_512.update(('%s%s' % (password_salt, password)).encode('utf-8'))
         hashed_password = hash_512.hexdigest()
         
-        logging.debug('hashed_password=%s', hashed_password)
+        logger.debug('hashed_password=%s', hashed_password)
         
         final_hashed_password =   hashed_password[0: int(conf.MAX_PASSWORD_LENGTH,10)]
         
-        logging.debug('final_hashed_password=%s', final_hashed_password)
+        logger.debug('final_hashed_password=%s', final_hashed_password)
         
         return final_hashed_password 
 
 def blend_password(unique_id, password):
     return unique_id + '!7' + password
 #-----------------------------------------------------------------
```

### Comparing `trex-lib-0.2.9/trexlib/utils/string_util.py` & `trex-lib-1.0.0/trexlib/utils/string_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 '''
 Created on Jul 3, 2012
 
 @author: sglok
 '''
 import random, re, string, logging
+import hmac
 
 WHITESPACE_PATTERN  = re.compile(r'\s')
 DASH_PATTERN        = re.compile(r'-')
 
 ALPHANUMERIC_CHARS  = string.ascii_lowercase + string.ascii_uppercase + string.digits
 NUMERIC_CHARS       = string.digits
 
 HUMAN_SAFE_ALPHANUMERIC_CHARS     = 'abcdefghijkmnpqrstuvwxyzABCDEFGHJKLMNPQRSTUVWXYZ123456789'
 
 
+
+def safe_str_cmp(a: str, b: str) -> bool:
+    """This function compares strings in somewhat constant time. This
+    requires that the length of at least one string is known in advance.
+
+    Returns `True` if the two strings are equal, or `False` if they are not.
+    """
+
+    if isinstance(a, str):
+        a = a.encode("utf-8")  # type: ignore
+
+    if isinstance(b, str):
+        b = b.encode("utf-8")  # type: ignore
+
+    return hmac.compare_digest(a, b)
+
 def random_string(number_character, is_human_mistake_safe=False):
     if is_human_mistake_safe:
         if number_character and type(number_character) is int and number_character>=0:
             return ''.join(random.sample(HUMAN_SAFE_ALPHANUMERIC_CHARS, number_character))
         else:
             return ''
 
@@ -127,20 +144,26 @@
     i = randint(range_from, range_to)
     if zero_padding:
         return str(i).zfill(zero_padding)
     else:
         return str(i)
 
 def is_empty(value):
-    if (isinstance(value, str)):
+    if isinstance(value, str):
         if value is None or value.strip()=='' or value.strip()=='null' or value.strip()=='None':
             return True
-        return False
+        
+    elif isinstance(value,(dict,list)):
+        if len(value)==0:
+            return True
+          
     else:
         return value is None
+    
+    return False
 
 def is_not_empty(value):
     return is_empty(value)==False
 
 def truncate_if_max_length(value, max_length):
     if value:
         return value[:max_length]
@@ -152,7 +175,14 @@
     else:
         return unicode_value
 
 
 def base64Encode(value):
     import base64
     return base64.b64encode(bytes(value, 'utf-8'))
+
+def split_by_length(str_value, length):
+    def _f(str_value, length):
+        while str_value:
+            yield str_value[:length]
+            str_value = str_value[length:]
+    return list(_f(str_value, length))
```

### Comparing `trex-lib-0.2.9/trexlib/utils/url_util.py` & `trex-lib-1.0.0/trexlib/utils/url_util.py`

 * *Files identical despite different names*

