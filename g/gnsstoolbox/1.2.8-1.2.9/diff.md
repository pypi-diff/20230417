# Comparing `tmp/gnsstoolbox-1.2.8.tar.gz` & `tmp/gnsstoolbox-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnsstoolbox-1.2.8.tar", last modified: Tue Apr  4 11:30:48 2023, max compression
+gzip compressed data, was "gnsstoolbox-1.2.9.tar", last modified: Mon Apr 17 10:59:24 2023, max compression
```

## Comparing `gnsstoolbox-1.2.8.tar` & `gnsstoolbox-1.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-04 11:30:48.931805 gnsstoolbox-1.2.8/
--rw-r--r--   0 beilin    (1000) beilin    (1000)    22118 2018-11-27 11:39:26.000000 gnsstoolbox-1.2.8/LICENCE.txt
--rw-r--r--   0 beilin    (1000) beilin    (1000)       76 2021-02-27 15:24:26.000000 gnsstoolbox-1.2.8/MANIFEST.in
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     1665 2023-04-04 11:30:48.931805 gnsstoolbox-1.2.8/PKG-INFO
--rw-r--r--   0 beilin    (1000) beilin    (1000)      858 2023-03-31 07:22:13.000000 gnsstoolbox-1.2.8/README.md
--rw-r--r--   0 beilin    (1000) beilin    (1000)      556 2023-03-31 06:55:30.000000 gnsstoolbox-1.2.8/__init__.py
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-04 11:30:48.931805 gnsstoolbox-1.2.8/gnsstoolbox/
--rw-r--r--   0 beilin    (1000) beilin    (1000)       45 2018-11-27 11:39:26.000000 gnsstoolbox-1.2.8/gnsstoolbox/__init__.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    35836 2023-03-31 08:21:38.000000 gnsstoolbox-1.2.8/gnsstoolbox/antex.py
--rw-r--r--   0 beilin    (1000) beilin    (1000)     2302 2023-03-31 08:21:56.000000 gnsstoolbox-1.2.8/gnsstoolbox/gnss_const.py
--rw-r--r--   0 beilin    (1000) beilin    (1000)     3065 2023-03-31 08:18:28.000000 gnsstoolbox-1.2.8/gnsstoolbox/gnss_corr.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    29066 2023-03-31 08:22:09.000000 gnsstoolbox-1.2.8/gnsstoolbox/gnss_process.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    10571 2023-03-31 08:18:21.000000 gnsstoolbox-1.2.8/gnsstoolbox/gnsstools.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    62481 2023-03-31 08:17:55.000000 gnsstoolbox-1.2.8/gnsstoolbox/orbits.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    53540 2023-04-01 20:36:54.000000 gnsstoolbox-1.2.8/gnsstoolbox/rinex_o.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)    11688 2023-03-31 08:18:40.000000 gnsstoolbox-1.2.8/gnsstoolbox/skyplot.py
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-04 11:30:48.931805 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     1665 2023-04-04 11:30:48.000000 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 beilin    (1000) beilin    (1000)      455 2023-04-04 11:30:48.000000 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)        1 2023-04-04 11:30:48.000000 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)       12 2023-04-04 11:30:48.000000 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/requires.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)       94 2023-04-04 11:30:48.000000 gnsstoolbox-1.2.8/gnsstoolbox.egg-info/top_level.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)       79 2023-04-04 11:30:48.931805 gnsstoolbox-1.2.8/setup.cfg
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     2610 2023-04-04 11:23:58.000000 gnsstoolbox-1.2.8/setup.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-17 10:59:24.328658 gnsstoolbox-1.2.9/
+-rw-r--r--   0 beilin    (1000) beilin    (1000)    22118 2018-11-27 11:39:26.000000 gnsstoolbox-1.2.9/LICENCE.txt
+-rw-r--r--   0 beilin    (1000) beilin    (1000)       76 2021-02-27 15:24:26.000000 gnsstoolbox-1.2.9/MANIFEST.in
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)     1665 2023-04-17 10:59:24.328658 gnsstoolbox-1.2.9/PKG-INFO
+-rw-r--r--   0 beilin    (1000) beilin    (1000)      858 2023-03-31 07:22:13.000000 gnsstoolbox-1.2.9/README.md
+-rw-r--r--   0 beilin    (1000) beilin    (1000)      556 2023-03-31 06:55:30.000000 gnsstoolbox-1.2.9/__init__.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-17 10:59:24.324658 gnsstoolbox-1.2.9/gnsstoolbox/
+-rw-r--r--   0 beilin    (1000) beilin    (1000)       45 2018-11-27 11:39:26.000000 gnsstoolbox-1.2.9/gnsstoolbox/__init__.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    35836 2023-03-31 08:21:38.000000 gnsstoolbox-1.2.9/gnsstoolbox/antex.py
+-rw-r--r--   0 beilin    (1000) beilin    (1000)     2302 2023-03-31 08:21:56.000000 gnsstoolbox-1.2.9/gnsstoolbox/gnss_const.py
+-rw-r--r--   0 beilin    (1000) beilin    (1000)     3065 2023-03-31 08:18:28.000000 gnsstoolbox-1.2.9/gnsstoolbox/gnss_corr.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    29066 2023-03-31 08:22:09.000000 gnsstoolbox-1.2.9/gnsstoolbox/gnss_process.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    11330 2023-04-17 10:56:51.000000 gnsstoolbox-1.2.9/gnsstoolbox/gnsstools.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    62481 2023-03-31 08:17:55.000000 gnsstoolbox-1.2.9/gnsstoolbox/orbits.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    53540 2023-04-01 20:36:54.000000 gnsstoolbox-1.2.9/gnsstoolbox/rinex_o.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)    11688 2023-03-31 08:18:40.000000 gnsstoolbox-1.2.9/gnsstoolbox/skyplot.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-04-17 10:59:24.328658 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)     1665 2023-04-17 10:59:24.000000 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)      455 2023-04-17 10:59:24.000000 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)        1 2023-04-17 10:59:24.000000 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)       12 2023-04-17 10:59:24.000000 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/requires.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)       94 2023-04-17 10:59:24.000000 gnsstoolbox-1.2.9/gnsstoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)       79 2023-04-17 10:59:24.328658 gnsstoolbox-1.2.9/setup.cfg
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)     2610 2023-04-17 10:57:20.000000 gnsstoolbox-1.2.9/setup.py
```

### Comparing `gnsstoolbox-1.2.8/LICENCE.txt` & `gnsstoolbox-1.2.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/PKG-INFO` & `gnsstoolbox-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnsstoolbox
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python GNSS processing package
 Home-page: https://gitlab.com/jbeilin/pygnsstoolbox
 Download-URL: 
 Author: Jacques Beilin
 Author-email: jacques.beilin@gmail.com
 License: gpl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gnsstoolbox-1.2.8/README.md` & `gnsstoolbox-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/__init__.py` & `gnsstoolbox-1.2.9/__init__.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/antex.py` & `gnsstoolbox-1.2.9/gnsstoolbox/antex.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/gnss_const.py` & `gnsstoolbox-1.2.9/gnsstoolbox/gnss_const.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/gnss_corr.py` & `gnsstoolbox-1.2.9/gnsstoolbox/gnss_corr.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/gnss_process.py` & `gnsstoolbox-1.2.9/gnsstoolbox/gnss_process.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/gnsstools.py` & `gnsstoolbox-1.2.9/gnsstoolbox/gnsstools.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,80 +45,92 @@
     Input :
     - X, Y, Z : cartesian coordinates (m) or vector of coordinates
 
     Output :
     - lon : vector of longitude (rad)
     - lat : vector of latitude (rad)
     - h : vector of heights (m)
+    or vector of coordinates
 
 
     Function call :
     [lamb,phi,h] = tool_cartgeo_GRS80_2([4201575.762;4201575.762],[189856.033;189856.033],[4779066.058;4779066.058])"""
 
     # IAG GRS80 constants
     a = 6378137.0
     f = 1/298.257222101
     e2 = 2 * f - f**2
-
-    rxy = np.sqrt(X**2 + Y**2)
-    r = np.sqrt( X**2 + Y**2 + Z**2)
     
-    if r < const.Rmin:
-        return 0.0, 0.0, 0.0
+    if not re.search('ndarray', str(type(X))):
+        X = np.array([X])
+        Y = np.array([Y])
+        Z = np.array([Z])
+    
+    rxy = (X**2 + Y**2)**0.5
+    
+    """ detect all points located exactly at north or south poles 
+    Those points are arbitrary shifted by 1e-6m in X coordinate """
+    X += np.where(rxy <= 0, 1e-6, 0) 
+    rxy = (X**2 + Y**2)**0.5
+    
+    lon = 2 * np.arctan(Y / (X + rxy));
+
+    r = ( X**2 + Y**2 + Z**2)**0.5
     
     mu = np.arctan((Z / rxy) * ((1 - f) + a * e2 / r))
 
     num = Z * (1 - f) + e2 * a * (np.sin(mu))**3;
     denum = (1 - f) * (rxy - a * e2 * (np.cos(mu))**3);
     lat = np.arctan(num / denum);
 
-    lon = 2 * np.arctan(Y / (X + rxy));
-
     w = (1 - e2 * np.sin(lat)**2)**0.5;
     h = rxy * np.cos(lat) + Z * np.sin(lat) - a * w;
     
     try:
-        lon = float(lon)
-        lat = float(lat)
-        h = float(h)
+        if len(lon) == 1:
+            lon = float(lon)
+            lat = float(lat)
+            h = float(h)
     except:
         pass
 
     return lon,lat,h
 
 def toolGeoCartGRS80(lon,lat,h):
     """[X,Y,Z] = tool_geocart_GRS80(lon,lat,h)
     Geographic to cartesian coordinates transformation
     Jacques BEILIN - 2014-06-10
 
     Input :
     - lon : longitude (rad)
     - lat : latitude (rad)
     - h : height (m)
+    or vector of coordinates
     Output :
-    - X, Y, Z : cartesian coordinates (m)
+    - X, Y, Z : cartesian coordinates (m) or vector of coordinates
 
     Function call :
         [X,Y,Z] = tool_geocart_GRS80(2.351412386,48.502786872,160.519)"""
 
     # IAG GRS80 constants
     a = 6378137.0
     f = 1/298.257222101
     e2 = 2 * f - f**2
 
     # angles in rad
     N = a / np.sqrt(1.0 - e2 * (np.sin(lat))**2);
     X = (N + h) * (np.cos(lon)) * (np.cos(lat));
     Y = (N + h) * (np.sin(lon)) * (np.cos(lat));
-    Z=(N * (1 - e2) + h) * (np.sin(lat));
+    Z = (N * (1 - e2) + h) * (np.sin(lat));
     
     try:
-        X = float(X)
-        Y = float(Y)
-        Z = float(Z)
+        if len(X) == 1:
+            X = float(X)
+            Y = float(Y)
+            Z = float(Z)
     except:
         pass
     
     return X,Y,Z
 
 def toolCartLocGRS80(X0,Y0,Z0,X,Y,Z):
     """function [E,N,U]=  tool_cartloc_GRS80(X0,Y0,Z0,X,Y,Z)
@@ -389,9 +401,22 @@
     print( Xr,Yr,Zr)
     [Xr,Yr,Zr] = toolRotY(X,Y,Z,alpha)
     print( Xr,Yr,Zr)
     [Xr,Yr,Zr] = toolRotZ(X,Y,Z,alpha)
     print( Xr,Yr,Zr)
     
 # if __name__ == "__main__":
-#     test()
+    # test()
+    
+    # M = np.array([[4201694.144, 177888.837, 4779371.767], [0, 0, 6378000], [0.001, 0, 6378000]])
+    # X = M[:, 0]
+    # Y = M[:, 1]
+    # Z = M[:, 2]
+    # print(M)
+
+
+    # M2 = toolCartGeoGRS80(X, Y, Z)
+    # print(M2)
+    
+    # M2 = toolCartGeoGRS80(4201694.144, 177888.837, 4779371.767)
+    # print(M2)
```

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/orbits.py` & `gnsstoolbox-1.2.9/gnsstoolbox/orbits.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/rinex_o.py` & `gnsstoolbox-1.2.9/gnsstoolbox/rinex_o.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox/skyplot.py` & `gnsstoolbox-1.2.9/gnsstoolbox/skyplot.py`

 * *Files identical despite different names*

### Comparing `gnsstoolbox-1.2.8/gnsstoolbox.egg-info/PKG-INFO` & `gnsstoolbox-1.2.9/gnsstoolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnsstoolbox
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python GNSS processing package
 Home-page: https://gitlab.com/jbeilin/pygnsstoolbox
 Download-URL: 
 Author: Jacques Beilin
 Author-email: jacques.beilin@gmail.com
 License: gpl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gnsstoolbox-1.2.8/setup.py` & `gnsstoolbox-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='gnsstoolbox',
-    version="1.2.8",
+    version="1.2.9",
     description='Python GNSS processing package',
     long_description=long_description,
     author='Jacques Beilin',
     author_email='jacques.beilin@gmail.com',
     packages = find_packages(exclude=["test","docs"]),
 
     install_requires = install_reqs,
```

