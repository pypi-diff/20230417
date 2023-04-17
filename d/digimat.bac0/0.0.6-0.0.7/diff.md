# Comparing `tmp/digimat.bac0-0.0.6.tar.gz` & `tmp/digimat.bac0-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.6.tar", last modified: Mon Apr 17 21:38:55 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.7.tar", last modified: Mon Apr 17 21:47:27 2023, max compression
```

## Comparing `digimat.bac0-0.0.6.tar` & `digimat.bac0-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.419969 digimat.bac0-0.0.6/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:38:55.419604 digimat.bac0-0.0.6/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 21:38:55.420071 digimat.bac0-0.0.6/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 21:38:49.000000 digimat.bac0-0.0.6/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.413529 digimat.bac0-0.0.6/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.414215 digimat.bac0-0.0.6/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.6/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.419068 digimat.bac0-0.0.6/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.6/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9994 2023-04-17 21:36:52.000000 digimat.bac0-0.0.6/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.418442 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.247465 digimat.bac0-0.0.7/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:47:27.247112 digimat.bac0-0.0.7/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 21:47:27.247560 digimat.bac0-0.0.7/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 21:47:22.000000 digimat.bac0-0.0.7/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.239590 digimat.bac0-0.0.7/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.240342 digimat.bac0-0.0.7/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.7/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.246605 digimat.bac0-0.0.7/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.7/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    10140 2023-04-17 21:45:15.000000 digimat.bac0-0.0.7/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.245673 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.6/setup.py` & `digimat.bac0-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.6',
+    version='0.0.7',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.6/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.7/src/digimat/bac0/bacnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,20 @@
                 index=self._pointsIndexByName[point.properties.name]
                 cov=''
                 if point.cov_registered:
                     cov='X'
                 t.add_row([index, point.properties.name, point.properties.type, point.value, cov, point.units, point.properties.description])
             print(t)
 
+    def refresh(self, key=None):
+        points=self.points(key)
+        if points:
+            for point in points:
+                point.value
+
     def __iter__(self):
         return iter(self._points)
 
 
 class BACDevice(object):
     def __init__(self, parent, ip, did, poll=60):
         self._parent=parent
```

