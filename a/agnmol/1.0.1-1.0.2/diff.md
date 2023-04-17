# Comparing `tmp/agnmol-1.0.1.tar.gz` & `tmp/agnmol-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnmol-1.0.1.tar", last modified: Sun Apr 16 15:14:37 2023, max compression
+gzip compressed data, was "agnmol-1.0.2.tar", last modified: Mon Apr 17 14:53:23 2023, max compression
```

## Comparing `agnmol-1.0.1.tar` & `agnmol-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.690675 agnmol-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1367 2023-04-16 15:14:37.689674 agnmol-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      978 2023-04-16 15:09:05.000000 agnmol-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.664683 agnmol-1.0.1/agnmol/
--rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.1/agnmol/__init__.py
--rw-rw-rw-   0        0        0      823 2023-04-16 15:13:05.000000 agnmol-1.0.1/agnmol/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:14:37.688673 agnmol-1.0.1/agnmol.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 15:14:37.000000 agnmol-1.0.1/agnmol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-16 15:13:35.000000 agnmol-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 15:14:37.690675 agnmol-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 14:53:23.141500 agnmol-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1394 2023-04-17 14:53:23.139503 agnmol-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-04-17 14:53:02.000000 agnmol-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:53:23.104498 agnmol-1.0.2/agnmol/
+-rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.2/agnmol/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-04-17 14:50:23.000000 agnmol-1.0.2/agnmol/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:53:23.137500 agnmol-1.0.2/agnmol.egg-info/
+-rw-rw-rw-   0        0        0     1394 2023-04-17 14:53:23.000000 agnmol-1.0.2/agnmol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-17 14:53:23.000000 agnmol-1.0.2/agnmol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:53:23.000000 agnmol-1.0.2/agnmol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 14:53:23.000000 agnmol-1.0.2/agnmol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-17 14:53:02.000000 agnmol-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:53:23.141500 agnmol-1.0.2/setup.cfg
```

### Comparing `agnmol-1.0.1/LICENSE.txt` & `agnmol-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.1/PKG-INFO` & `agnmol-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -39,18 +39,19 @@
 from agnmol.motion import change_in_position
 
 change_in_position(1, 3, 2) #output: 12.0
 # or use named variables
 change_in_position(a=2, t=3, vi=1) #output: 12.0
 ```
 ###Final velocity
-Final velocity is calculated using formula: 
+Final velocity is calculated using one of formulas: 
 ```math
-x = vi*t+1/2*a*t^2
+vf = (vi^2+2a*x)^1/2
+vf = vi+a*t
 ```
 ```python
-from agnmol.motion import change_in_position
-
-change_in_position(1, 3, 2) #output: 12.0
-# or use named variables
-change_in_position(a=2, t=3, vi=1) #output: 12.0
+from agnmol.motion import v_final
+# using first equation
+v_final(vi=1, a=3, x_delta=1.5) #output: 10.0
+# using second equation
+v_final(vi=1, a=2.3, t=2) #output: 5.6
 ```
```

### Comparing `agnmol-1.0.1/agnmol/motion.py` & `agnmol-1.0.2/agnmol/motion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import math
 
 
-def acceleration(v_delta, t, vf, vi):
-    if v_delta and t:
+def acceleration(v_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
+    if v_delta != math.inf and t != math.inf:
         return v_delta / t
-    elif vi and vf and t:
+    elif vi != math.inf and vf != math.inf and t != math.inf:
         return (vf - vi) / t
     else:
         return 0
 
-def v_average(x_delta, t, vf, vi):
-    if x_delta and t:
+def v_average(x_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
+    if x_delta != math.inf and t != math.inf:
         return x_delta / t
-    elif vi and vf:
+    elif vi != math.inf and vf != math.inf:
         return (vf - vi) / 2
     else:
         return 0
 
 def v_final(vi, a, t=math.inf, x_delta=math.inf):
     if not vi or not a:
         return 0
@@ -26,15 +26,11 @@
 
     if x_delta != math.inf:
         return vi ** 2 + 2 * a * x_delta
 
     return 0
 
 def change_in_position(vi, t, a):
-    if vi and t and a:
-        return vi * t + 0.5 * a * (t ** 2)
-    return 0
+    return vi * t + 0.5 * a * (t ** 2)
 
 def displacement(t, vf, vi):
-    if vi and vf and t:
-        return 0.5 * (vi + vf) * t
-    return 0
+    return 0.5 * (vi + vf) * t
```

### Comparing `agnmol-1.0.1/agnmol.egg-info/PKG-INFO` & `agnmol-1.0.2/agnmol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -39,18 +39,19 @@
 from agnmol.motion import change_in_position
 
 change_in_position(1, 3, 2) #output: 12.0
 # or use named variables
 change_in_position(a=2, t=3, vi=1) #output: 12.0
 ```
 ###Final velocity
-Final velocity is calculated using formula: 
+Final velocity is calculated using one of formulas: 
 ```math
-x = vi*t+1/2*a*t^2
+vf = (vi^2+2a*x)^1/2
+vf = vi+a*t
 ```
 ```python
-from agnmol.motion import change_in_position
-
-change_in_position(1, 3, 2) #output: 12.0
-# or use named variables
-change_in_position(a=2, t=3, vi=1) #output: 12.0
+from agnmol.motion import v_final
+# using first equation
+v_final(vi=1, a=3, x_delta=1.5) #output: 10.0
+# using second equation
+v_final(vi=1, a=2.3, t=2) #output: 5.6
 ```
```

