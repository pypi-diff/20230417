# Comparing `tmp/garpix_profitbase-1.9.1.tar.gz` & `tmp/garpix_profitbase-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_profitbase-1.9.1.tar", last modified: Thu Aug 25 13:35:12 2022, max compression
+gzip compressed data, was "garpix_profitbase-1.9.2.tar", last modified: Mon Sep 12 12:32:41 2022, max compression
```

## Comparing `garpix_profitbase-1.9.1.tar` & `garpix_profitbase-1.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.472447 garpix_profitbase-1.9.1/
--rw-r--r--   0 crusat     (501) staff       (20)       37 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     2620 2022-08-25 13:35:12.472336 garpix_profitbase-1.9.1/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.470364 garpix_profitbase-1.9.1/garpix_profitbase/
--rw-r--r--   0 crusat     (501) staff       (20)       37 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)       69 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.471131 garpix_profitbase-1.9.1/garpix_profitbase/admin/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/admin/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)      146 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/apps.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.469567 garpix_profitbase-1.9.1/garpix_profitbase/management/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.471208 garpix_profitbase-1.9.1/garpix_profitbase/management/commands/
--rw-r--r--   0 crusat     (501) staff       (20)     1537 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/management/commands/profitbase_update.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.472191 garpix_profitbase-1.9.1/garpix_profitbase/models/
--rw-r--r--   0 crusat     (501) staff       (20)      313 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/__init__.py
--rw-r--r--   0 crusat     (501) staff       (20)      686 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/city.py
--rw-r--r--   0 crusat     (501) staff       (20)       72 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/empty_mixin.py
--rw-r--r--   0 crusat     (501) staff       (20)      814 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/house.py
--rw-r--r--   0 crusat     (501) staff       (20)      810 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/house_floor.py
--rw-r--r--   0 crusat     (501) staff       (20)      695 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/house_section.py
--rw-r--r--   0 crusat     (501) staff       (20)     1233 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/layout_plan.py
--rw-r--r--   0 crusat     (501) staff       (20)      720 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/project.py
--rw-r--r--   0 crusat     (501) staff       (20)     3362 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/property.py
--rw-r--r--   0 crusat     (501) staff       (20)     1887 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.1/garpix_profitbase/models/property_special_offer.py
--rw-r--r--   0 crusat     (501) staff       (20)    20760 2022-08-25 13:34:42.000000 garpix_profitbase-1.9.1/garpix_profitbase/profitbase.py
--rw-r--r--   0 crusat     (501) staff       (20)     1120 2022-08-25 13:34:32.000000 garpix_profitbase-1.9.1/garpix_profitbase/setup.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-08-25 13:35:12.471027 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     2620 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)      894 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)       56 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       18 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/garpix_profitbase.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2022-08-25 13:35:12.472483 garpix_profitbase-1.9.1/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1120 2022-08-25 13:35:12.000000 garpix_profitbase-1.9.1/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.288251 garpix_profitbase-1.9.2/
+-rw-r--r--   0 crusat     (501) staff       (20)       37 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     2620 2022-09-12 12:32:41.288125 garpix_profitbase-1.9.2/PKG-INFO
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.286015 garpix_profitbase-1.9.2/garpix_profitbase/
+-rw-r--r--   0 crusat     (501) staff       (20)       37 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)       69 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.286817 garpix_profitbase-1.9.2/garpix_profitbase/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/admin/__init__.py
+-rw-r--r--   0 crusat     (501) staff       (20)      146 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/apps.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.285132 garpix_profitbase-1.9.2/garpix_profitbase/management/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.286899 garpix_profitbase-1.9.2/garpix_profitbase/management/commands/
+-rw-r--r--   0 crusat     (501) staff       (20)     1537 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/management/commands/profitbase_update.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.287957 garpix_profitbase-1.9.2/garpix_profitbase/models/
+-rw-r--r--   0 crusat     (501) staff       (20)      313 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/__init__.py
+-rw-r--r--   0 crusat     (501) staff       (20)      686 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/city.py
+-rw-r--r--   0 crusat     (501) staff       (20)       72 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/empty_mixin.py
+-rw-r--r--   0 crusat     (501) staff       (20)      814 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/house.py
+-rw-r--r--   0 crusat     (501) staff       (20)      810 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/house_floor.py
+-rw-r--r--   0 crusat     (501) staff       (20)      695 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/house_section.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1233 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/layout_plan.py
+-rw-r--r--   0 crusat     (501) staff       (20)      720 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/project.py
+-rw-r--r--   0 crusat     (501) staff       (20)     3362 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/property.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1887 2022-08-25 10:08:27.000000 garpix_profitbase-1.9.2/garpix_profitbase/models/property_special_offer.py
+-rw-r--r--   0 crusat     (501) staff       (20)    20809 2022-09-12 12:32:29.000000 garpix_profitbase-1.9.2/garpix_profitbase/profitbase.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1120 2022-09-12 12:32:29.000000 garpix_profitbase-1.9.2/garpix_profitbase/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2022-09-12 12:32:41.286711 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/
+-rw-r--r--   0 crusat     (501) staff       (20)     2620 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/PKG-INFO
+-rw-r--r--   0 crusat     (501) staff       (20)      894 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/SOURCES.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/dependency_links.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/not-zip-safe
+-rw-r--r--   0 crusat     (501) staff       (20)       56 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/requires.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       18 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/garpix_profitbase.egg-info/top_level.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       38 2022-09-12 12:32:41.288290 garpix_profitbase-1.9.2/setup.cfg
+-rw-r--r--   0 crusat     (501) staff       (20)     1120 2022-09-12 12:32:41.000000 garpix_profitbase-1.9.2/setup.py
```

### Comparing `garpix_profitbase-1.9.1/PKG-INFO` & `garpix_profitbase-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_profitbase
-Version: 1.9.1
+Version: 1.9.2
 Home-page: https://github.com/garpixcms/garpix_profitbase
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/management/commands/profitbase_update.py` & `garpix_profitbase-1.9.2/garpix_profitbase/management/commands/profitbase_update.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/city.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/city.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/house.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/house.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/house_floor.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/house_floor.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/house_section.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/house_section.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/layout_plan.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/layout_plan.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/project.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/project.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/property.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/property.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/models/property_special_offer.py` & `garpix_profitbase-1.9.2/garpix_profitbase/models/property_special_offer.py`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/profitbase.py` & `garpix_profitbase-1.9.2/garpix_profitbase/profitbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         for item in response.json()['data']:
             if not isinstance(item, dict):
                 break
             house = House.objects.filter(profitbase_id=item['id']).first()
             data = {
                 'name': item['title'],
                 'title': item['title'],
+                'material': item.get('material')
             }
             try:
                 if house is None:
                     House.objects.create(
                         profitbase_id=item['id'],
                         **data,
                     )
```

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase/setup.py` & `garpix_profitbase-1.9.2/garpix_profitbase/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.conf import settings
 
 with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
     long_description = convert(f.read())
 
 setup(
     name='garpix_profitbase',
-    version='1.9.1',
+    version='1.9.2',
     description='',
     long_description=long_description,
     url='https://github.com/garpixcms/garpix_profitbase',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
```

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase.egg-info/PKG-INFO` & `garpix_profitbase-1.9.2/garpix_profitbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-profitbase
-Version: 1.9.1
+Version: 1.9.2
 Home-page: https://github.com/garpixcms/garpix_profitbase
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_profitbase-1.9.1/garpix_profitbase.egg-info/SOURCES.txt` & `garpix_profitbase-1.9.2/garpix_profitbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_profitbase-1.9.1/setup.py` & `garpix_profitbase-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.conf import settings
 
 with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
     long_description = convert(f.read())
 
 setup(
     name='garpix_profitbase',
-    version='1.9.1',
+    version='1.9.2',
     description='',
     long_description=long_description,
     url='https://github.com/garpixcms/garpix_profitbase',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
```

