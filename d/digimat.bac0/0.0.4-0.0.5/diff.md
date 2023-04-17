# Comparing `tmp/digimat.bac0-0.0.4.tar.gz` & `tmp/digimat.bac0-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.4.tar", last modified: Mon Apr 17 14:31:17 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.5.tar", last modified: Mon Apr 17 17:16:40 2023, max compression
```

## Comparing `digimat.bac0-0.0.4.tar` & `digimat.bac0-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.906400 digimat.bac0-0.0.4/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 14:31:17.905951 digimat.bac0-0.0.4/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 14:31:17.906526 digimat.bac0-0.0.4/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 14:31:12.000000 digimat.bac0-0.0.4/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.901657 digimat.bac0-0.0.4/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.902345 digimat.bac0-0.0.4/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.4/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.905518 digimat.bac0-0.0.4/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.4/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9243 2023-04-17 14:30:41.000000 digimat.bac0-0.0.4/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.905034 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.469035 digimat.bac0-0.0.5/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 17:16:40.468691 digimat.bac0-0.0.5/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 17:16:40.469287 digimat.bac0-0.0.5/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 17:16:34.000000 digimat.bac0-0.0.5/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.463932 digimat.bac0-0.0.5/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.464724 digimat.bac0-0.0.5/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.5/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.468109 digimat.bac0-0.0.5/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.5/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9772 2023-04-17 17:15:25.000000 digimat.bac0-0.0.5/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.467307 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.4/setup.py` & `digimat.bac0-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.4',
+    version='0.0.5',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.4/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.5/src/digimat/bac0/bacnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,43 @@
             if points:
                 for point in points:
                     if not self.point(point.properties.name):
                         self._pointsByName[point.properties.name]=point
                         self._pointsIndexByName[point.properties.name]=len(self._points)
                         self._points.append(point)
 
+    def cov(self, key=None):
+        points=self.points(key)
+        if points:
+            for point in points:
+                if not point.cov_registered:
+                    point.subscribe_cov()
+
+    def properties(self, index):
+        point=self.point(index)
+        if point:
+            return point.properties
+
     def dump(self, key=None):
         points=self.points(key)
         if points:
             t=PrettyTable()
-            t.field_names=['#', 'name', 'type', 'value', 'unit', 'description']
+            t.field_names=['#', 'name', 'type', 'value', 'COV', 'unit', 'description']
             t.align['#']='l'
             t.align['name']='l'
             t.align['type']='l'
             t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
             for point in points:
                 index=self._pointsIndexByName[point.properties.name]
-                t.add_row([index, point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
+                cov=''
+                if point.cov_registered:
+                    cov='X'
+                t.add_row([index, point.properties.name, point.properties.type, point.value, cov, point.units, point.properties.description])
             print(t)
 
     def __iter__(self):
         return iter(self._points)
 
 
 class BACDevice(object):
@@ -203,22 +218,25 @@
             pass
 
     def dump(self, points=None, outOfService=False):
         if type(points) is not list:
             points=self.points(points, outOfService=outOfService)
         if points:
             t=PrettyTable()
-            t.field_names=['name', 'type', 'value', 'unit', 'description']
+            t.field_names=['name', 'type', 'value', 'COV', 'unit', 'description']
             t.align['name']='l'
             t.align['type']='l'
             t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
             for point in points:
-                t.add_row([point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
+                cov=''
+                if point.cov_registered:
+                    cov='X'
+                t.add_row([point.properties.name, point.properties.type, point.value, cov, point.units, point.properties.description])
             print(t)
 
     def bag(self, key=None):
         return BACBag(self, key)
 
     def __iter__(self):
         return iter(self._device.points)
```

