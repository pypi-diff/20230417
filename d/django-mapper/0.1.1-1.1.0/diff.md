# Comparing `tmp/django-mapper-0.1.1.tar.gz` & `tmp/django-mapper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-0.1.1.tar", last modified: Thu Apr 13 21:45:42 2023, max compression
+gzip compressed data, was "django-mapper-1.1.0.tar", last modified: Mon Apr 17 06:31:34 2023, max compression
```

## Comparing `django-mapper-0.1.1.tar` & `django-mapper-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-13 21:45:42.964242 django-mapper-0.1.1/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-0.1.1/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-0.1.1/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     2481 2023-04-13 20:17:57.000000 django-mapper-0.1.1/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-13 21:45:42.964242 django-mapper-0.1.1/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-13 21:45:42.000000 django-mapper-0.1.1/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-13 21:45:42.964242 django-mapper-0.1.1/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-13 21:43:57.000000 django-mapper-0.1.1/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.367653 django-mapper-1.1.0/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 06:31:34.363653 django-mapper-1.1.0/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.0/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.363653 django-mapper-1.1.0/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       45 2023-04-13 20:25:08.000000 django-mapper-1.1.0/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     2598 2023-04-17 06:18:02.000000 django-mapper-1.1.0/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-17 06:31:34.363653 django-mapper-1.1.0/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-17 06:31:34.000000 django-mapper-1.1.0/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-17 06:31:34.367653 django-mapper-1.1.0/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-17 06:25:06.000000 django-mapper-1.1.0/setup.py
```

### Comparing `django-mapper-0.1.1/PKG-INFO` & `django-mapper-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 0.1.1
+Version: 1.1.0
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-0.1.1/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.0/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 0.1.1
+Version: 1.1.0
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-0.1.1/setup.py` & `django-mapper-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='0.1.1',
+    version='1.1.0',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

