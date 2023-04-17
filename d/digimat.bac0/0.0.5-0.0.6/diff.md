# Comparing `tmp/digimat.bac0-0.0.5.tar.gz` & `tmp/digimat.bac0-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.5.tar", last modified: Mon Apr 17 17:16:40 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.6.tar", last modified: Mon Apr 17 21:38:55 2023, max compression
```

## Comparing `digimat.bac0-0.0.5.tar` & `digimat.bac0-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.469035 digimat.bac0-0.0.5/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 17:16:40.468691 digimat.bac0-0.0.5/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 17:16:40.469287 digimat.bac0-0.0.5/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 17:16:34.000000 digimat.bac0-0.0.5/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.463932 digimat.bac0-0.0.5/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.464724 digimat.bac0-0.0.5/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.5/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.468109 digimat.bac0-0.0.5/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.5/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9772 2023-04-17 17:15:25.000000 digimat.bac0-0.0.5/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 17:16:40.467307 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 17:16:40.000000 digimat.bac0-0.0.5/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.419969 digimat.bac0-0.0.6/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:38:55.419604 digimat.bac0-0.0.6/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 21:38:55.420071 digimat.bac0-0.0.6/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 21:38:49.000000 digimat.bac0-0.0.6/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.413529 digimat.bac0-0.0.6/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.414215 digimat.bac0-0.0.6/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.6/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.419068 digimat.bac0-0.0.6/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.6/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9994 2023-04-17 21:36:52.000000 digimat.bac0-0.0.6/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:38:55.418442 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:38:55.000000 digimat.bac0-0.0.6/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.5/setup.py` & `digimat.bac0-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.5',
+    version='0.0.6',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.5/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.6/src/digimat/bac0/bacnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,24 @@
             if points:
                 for point in points:
                     if not self.point(point.properties.name):
                         self._pointsByName[point.properties.name]=point
                         self._pointsIndexByName[point.properties.name]=len(self._points)
                         self._points.append(point)
 
-    def cov(self, key=None):
-        points=self.points(key)
+    def cov(self, enable=True):
+        points=self.points()
         if points:
             for point in points:
-                if not point.cov_registered:
-                    point.subscribe_cov()
+                if enable:
+                    if not point.cov_registered:
+                        point.subscribe_cov()
+                else:
+                    if point.cov_registered:
+                        point.cancel_cov()
 
     def properties(self, index):
         point=self.point(index)
         if point:
             return point.properties
 
     def dump(self, key=None):
@@ -111,20 +115,20 @@
             print(t)
 
     def __iter__(self):
         return iter(self._points)
 
 
 class BACDevice(object):
-    def __init__(self, parent, ip, did):
+    def __init__(self, parent, ip, did, poll=60):
         self._parent=parent
         self._did=did
         self._ip=ip
         self.logger.info('Creating device %s:%d' % (ip, did))
-        self._device=BAC0.device(ip, did, parent.bac0)
+        self._device=BAC0.device(ip, did, parent.bac0, poll=poll)
 
     def __repr__(self):
         return '<%s:%d(%s:%s, %s, %d points)>' % (self.__class__.__name__, self._did,
             self.vendorName, self.modelName, self.systemStatus,
             len(self._device.points))
 
     @property
@@ -249,14 +253,16 @@
         socketHandler = logging.handlers.SocketHandler(logServer, logging.handlers.DEFAULT_TCP_LOGGING_PORT)
         logger.addHandler(socketHandler)
         self._logger=logger
 
         self._network=network
         self._bac0=None
 
+        # BAC0.log_level('silence')
+
         if ipRouter:
             self.logger.info('Starting BAC0 with network %s@%s' % (self._network, ipRouter))
             self._bac0=BAC0.lite(ip=network, bbmdAddress=ipRouter, bbmdTTL=900)
         else:
             self.logger.info('Starting BAC0 with network %s' % self._network)
             self._bac0=BAC0.lite(ip=self._network)
 
@@ -303,17 +309,17 @@
                 for item in items:
                     self.declare(item[0], item[1])
             return items
 
     def discover(self):
         return self.whois(True)
 
-    def declare(self, ip, did):
+    def declare(self, ip, did, poll=60):
         if not self.device(did):
-            device=BACDevice(self, ip, did)
+            device=BACDevice(self, ip, did, poll=poll)
             self._devices[did]=device
             return device
 
     def __getitem__(self, key):
         return self.device(key)
 
     def dump(self):
```

