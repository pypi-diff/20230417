# Comparing `tmp/digimat.bac0-0.0.3.tar.gz` & `tmp/digimat.bac0-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.3.tar", last modified: Sun Apr 16 10:41:01 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.4.tar", last modified: Mon Apr 17 14:31:17 2023, max compression
```

## Comparing `digimat.bac0-0.0.3.tar` & `digimat.bac0-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.780372 digimat.bac0-0.0.3/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.780089 digimat.bac0-0.0.3/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-16 10:41:01.780471 digimat.bac0-0.0.3/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      958 2023-04-16 10:40:57.000000 digimat.bac0-0.0.3/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.776996 digimat.bac0-0.0.3/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.777526 digimat.bac0-0.0.3/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.3/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.779708 digimat.bac0-0.0.3/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.3/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8287 2023-04-16 10:39:38.000000 digimat.bac0-0.0.3/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:41:01.779227 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      375 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 16:54:48.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       28 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:41:01.000000 digimat.bac0-0.0.3/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.906400 digimat.bac0-0.0.4/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 14:31:17.905951 digimat.bac0-0.0.4/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 14:31:17.906526 digimat.bac0-0.0.4/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 14:31:12.000000 digimat.bac0-0.0.4/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.901657 digimat.bac0-0.0.4/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.902345 digimat.bac0-0.0.4/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.4/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.905518 digimat.bac0-0.0.4/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.4/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     9243 2023-04-17 14:30:41.000000 digimat.bac0-0.0.4/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 14:31:17.905034 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 14:31:17.000000 digimat.bac0-0.0.4/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.3/setup.py` & `digimat.bac0-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.3',
+    version='0.0.4',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
+        'digimat.units',
         'ptable',
         'pytz',
         'BAC0',
         'setuptools'
     ],
     dependency_links=[
         ''
```

### Comparing `digimat.bac0-0.0.3/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.4/src/digimat/bac0/bacnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class BACBag(object):
     def __init__(self, device, key=None):
         self._device=device
         self._points=[]
         self._pointsByName={}
+        self._pointsIndexByName={}
         if key:
             self.add(key)
 
     def __repr__(self):
         return '<%s[%s](%d points)>' % (self.__class__.__name__, self.device.name,
             len(self._points))
 
@@ -24,16 +25,31 @@
     def logger(self):
         return self._device.logger
 
     @property
     def device(self):
         return self._device
 
-    def points(self):
-        return self._points
+    def points(self, key=None, objectType=None, outOfService=False):
+        items=[]
+        if key:
+            key=key.lower()
+        if key=='*':
+            key=None
+        for point in self._points:
+            if not outOfService and point.bacnet_properties['outOfService']:
+                continue
+            if objectType and objectType!=point.properties.type:
+                continue
+            if key:
+                if key not in point.properties.name.lower() and \
+                        key not in point.properties.description.lower():
+                    continue
+            items.append(point)
+        return items
 
     def point(self, name):
         try:
             return self._pointsByName[name]
         except:
             pass
         try:
@@ -55,32 +71,37 @@
             if type(key)==list:
                 points=key
             else:
                 points=self.device.points(key)
             if points:
                 for point in points:
                     if not self.point(point.properties.name):
-                        self._points.append(point)
                         self._pointsByName[point.properties.name]=point
+                        self._pointsIndexByName[point.properties.name]=len(self._points)
+                        self._points.append(point)
 
-    def dump(self):
-        if self._points:
+    def dump(self, key=None):
+        points=self.points(key)
+        if points:
             t=PrettyTable()
             t.field_names=['#', 'name', 'type', 'value', 'unit', 'description']
             t.align['#']='l'
             t.align['name']='l'
             t.align['type']='l'
             t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
-            for n in range(len(self._points)):
-                point=self._points[n]
-                t.add_row([n, point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
+            for point in points:
+                index=self._pointsIndexByName[point.properties.name]
+                t.add_row([index, point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
             print(t)
 
+    def __iter__(self):
+        return iter(self._points)
+
 
 class BACDevice(object):
     def __init__(self, parent, ip, did):
         self._parent=parent
         self._did=did
         self._ip=ip
         self.logger.info('Creating device %s:%d' % (ip, did))
@@ -195,14 +216,17 @@
             for point in points:
                 t.add_row([point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
             print(t)
 
     def bag(self, key=None):
         return BACBag(self, key)
 
+    def __iter__(self):
+        return iter(self._device.points)
+
 
 class BAC(object):
     def __init__(self, network, ipRouter=None, logServer='localhost', logLevel=logging.DEBUG):
         logger=logging.getLogger("BAC(%s)" % network)
         logger.setLevel(logLevel)
         socketHandler = logging.handlers.SocketHandler(logServer, logging.handlers.DEFAULT_TCP_LOGGING_PORT)
         logger.addHandler(socketHandler)
@@ -287,10 +311,13 @@
             for device in devices:
                 t.add_row([device.name, device.did, device.ip,
                            device.vendorName, device.modelName, device.systemStatus,
                            device.description,
                            device.count()])
             print(t)
 
+    def __iter__(self):
+        return iter(self._devices)
+
 
 if __name__=='__main__':
     pass
```

