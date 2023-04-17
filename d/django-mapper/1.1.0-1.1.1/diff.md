# Comparing `tmp/django-mapper-1.1.0.tar.gz` & `tmp/django-mapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.0.tar", last modified: Mon Apr 17 06:31:34 2023, max compression
+gzip compressed data, was "django-mapper-1.1.1.tar", last modified: Mon Apr 17 09:20:31 2023, max compression
```

## Comparing `django-mapper-1.1.0.tar` & `django-mapper-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.367653 django-mapper-1.1.0/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 06:31:34.363653 django-mapper-1.1.0/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.0/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.363653 django-mapper-1.1.0/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.0/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2598 2023-04-17 06:18:02.000000 django-mapper-1.1.0/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.363653 django-mapper-1.1.0/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-17 06:31:34.367653 django-mapper-1.1.0/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-17 06:25:06.000000 django-mapper-1.1.0/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 09:20:31.658364 django-mapper-1.1.1/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.1/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.1/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     2808 2023-04-17 09:18:20.000000 django-mapper-1.1.1/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 09:20:31.658364 django-mapper-1.1.1/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-17 09:20:31.000000 django-mapper-1.1.1/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-17 09:20:31.658364 django-mapper-1.1.1/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-17 09:18:34.000000 django-mapper-1.1.1/setup.py
```

### Comparing `django-mapper-1.1.0/PKG-INFO` & `django-mapper-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.0/django_mapper/mapper.py` & `django-mapper-1.1.1/django_mapper/mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from django.db import models
 
 class DataMapper:
     def __init__(self, config, target_model=None, enable_logging=False):
         self.config = config
         self.target_model = target_model
         self.enable_logging = enable_logging
         self.logger = logging.getLogger(__name__)
@@ -38,17 +39,21 @@
             instance = self.create_instance(self.target_model, mapped_data)
             self.logger.info(f"Created instance of {self.target_model.__name__}")
             return instance
         else:
             return mapped_data
     
     def get_value(self, data, field):
+        current_data = data
         for f in field.split('__'):
-            data = data.get(f)
-        return data
+            if isinstance(data, models.Model):
+                current_data = getattr(current_data, field)
+            else:
+                current_data = current_data.get(f)
+        return current_data
     
     def set_value(self, data, field, value):
         fields = field.split('__')
         for f in fields[:-1]:
             if f not in data:
                 data[f] = {}
             data = data[f]
```

### Comparing `django-mapper-1.1.0/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.1/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.0/setup.py` & `django-mapper-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.0',
+    version='1.1.1',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

