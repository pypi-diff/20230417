# Comparing `tmp/agnmol-1.0.6.tar.gz` & `tmp/agnmol-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnmol-1.0.6.tar", last modified: Mon Apr 17 16:29:45 2023, max compression
+gzip compressed data, was "agnmol-1.0.7.tar", last modified: Mon Apr 17 16:32:05 2023, max compression
```

## Comparing `agnmol-1.0.6.tar` & `agnmol-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:29:45.652785 agnmol-1.0.6/
--rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2049 2023-04-17 16:29:45.649785 agnmol-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-04-17 16:29:23.000000 agnmol-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 16:29:45.635788 agnmol-1.0.6/agnmol/
--rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.6/agnmol/__init__.py
--rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.6/agnmol/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:29:45.648788 agnmol-1.0.6/agnmol.egg-info/
--rw-rw-rw-   0        0        0     2049 2023-04-17 16:29:45.000000 agnmol-1.0.6/agnmol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-17 16:29:45.000000 agnmol-1.0.6/agnmol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:29:45.000000 agnmol-1.0.6/agnmol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 16:29:45.000000 agnmol-1.0.6/agnmol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-17 16:29:23.000000 agnmol-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 16:29:45.652785 agnmol-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.355975 agnmol-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2040 2023-04-17 16:32:05.352966 agnmol-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-04-17 16:31:46.000000 agnmol-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.338967 agnmol-1.0.7/agnmol/
+-rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.7/agnmol/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.7/agnmol/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.351966 agnmol-1.0.7/agnmol.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-17 16:31:46.000000 agnmol-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 16:32:05.355975 agnmol-1.0.7/setup.cfg
```

### Comparing `agnmol-1.0.6/LICENSE.txt` & `agnmol-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.6/PKG-INFO` & `agnmol-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,89 +1,81 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Physics equations of motion solver
-
 This is a package for physics motion calculations.
 
-#Installation
-
+# Installation
 ```pip install agnmol```
 
-#Usage
-
-###Displacement
-
+# Usage
+### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
 ```python
 from agnmol.motion import displacement
 
 displacement(1, 2.3, 3) #output: 2.65
 # or use named variables
 displacement(vf=2.3, t=1, vi=3) #output: 2.65
 ```
 
-###Change in position
-
+### Change in position
 Change in position is calculated using formula: 
 ```math
 x = vi*t+1/2*a*t^2
 ```
 ```python
 from agnmol.motion import change_in_position
 
 change_in_position(1, 3, 2) #output: 12.0
 # or use named variables
 change_in_position(a=2, t=3, vi=1) #output: 12.0
 ```
 
-###Final velocity
-
+### Final velocity
 Final velocity is calculated using one of formulas: 
 ```math
 vf = (vi^2+2a*x)^1/2
 vf = vi+a*t
 ```
 ```python
 from agnmol.motion import v_final
 # using first equation
 v_final(vi=1, a=3, x_delta=1.5) #output: 10.0
 # using second equation
 v_final(vi=1, a=2.3, t=2) #output: 5.6
 ```
 
-###Average velocity
-
+### Average velocity
 Average velocity is calculated using one of formulas: 
 ```math
 va = x/t
 va = (vi+vf)/2
 ```
 ```python
 from agnmol.motion import v_average
 # using first equation
 v_average(x_delta=1, t=3) #output: 0.3333333333333333
 # using second equation
 v_average(vi=1, vf=2.6) #output: 0.8
 ```
 
-###Acceleration velocity
-
+### Acceleration velocity
 Acceleration velocity is calculated using one of formulas: 
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
```

### Comparing `agnmol-1.0.6/README.md` & `agnmol-1.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,69 @@
 # Physics equations of motion solver
-
 This is a package for physics motion calculations.
 
-#Installation
-
+# Installation
 ```pip install agnmol```
 
-#Usage
-
-###Displacement
-
+# Usage
+### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
 ```python
 from agnmol.motion import displacement
 
 displacement(1, 2.3, 3) #output: 2.65
 # or use named variables
 displacement(vf=2.3, t=1, vi=3) #output: 2.65
 ```
 
-###Change in position
-
+### Change in position
 Change in position is calculated using formula: 
 ```math
 x = vi*t+1/2*a*t^2
 ```
 ```python
 from agnmol.motion import change_in_position
 
 change_in_position(1, 3, 2) #output: 12.0
 # or use named variables
 change_in_position(a=2, t=3, vi=1) #output: 12.0
 ```
 
-###Final velocity
-
+### Final velocity
 Final velocity is calculated using one of formulas: 
 ```math
 vf = (vi^2+2a*x)^1/2
 vf = vi+a*t
 ```
 ```python
 from agnmol.motion import v_final
 # using first equation
 v_final(vi=1, a=3, x_delta=1.5) #output: 10.0
 # using second equation
 v_final(vi=1, a=2.3, t=2) #output: 5.6
 ```
 
-###Average velocity
-
+### Average velocity
 Average velocity is calculated using one of formulas: 
 ```math
 va = x/t
 va = (vi+vf)/2
 ```
 ```python
 from agnmol.motion import v_average
 # using first equation
 v_average(x_delta=1, t=3) #output: 0.3333333333333333
 # using second equation
 v_average(vi=1, vf=2.6) #output: 0.8
 ```
 
-###Acceleration velocity
-
+### Acceleration velocity
 Acceleration velocity is calculated using one of formulas: 
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
```

### Comparing `agnmol-1.0.6/agnmol/motion.py` & `agnmol-1.0.7/agnmol/motion.py`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.6/agnmol.egg-info/PKG-INFO` & `agnmol-1.0.7/agnmol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,89 +1,81 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Physics equations of motion solver
-
 This is a package for physics motion calculations.
 
-#Installation
-
+# Installation
 ```pip install agnmol```
 
-#Usage
-
-###Displacement
-
+# Usage
+### Displacement
 Displacement is calculated using formula: 
 ```math
 x = (vi-vf)/2*t 
 ```
 ```python
 from agnmol.motion import displacement
 
 displacement(1, 2.3, 3) #output: 2.65
 # or use named variables
 displacement(vf=2.3, t=1, vi=3) #output: 2.65
 ```
 
-###Change in position
-
+### Change in position
 Change in position is calculated using formula: 
 ```math
 x = vi*t+1/2*a*t^2
 ```
 ```python
 from agnmol.motion import change_in_position
 
 change_in_position(1, 3, 2) #output: 12.0
 # or use named variables
 change_in_position(a=2, t=3, vi=1) #output: 12.0
 ```
 
-###Final velocity
-
+### Final velocity
 Final velocity is calculated using one of formulas: 
 ```math
 vf = (vi^2+2a*x)^1/2
 vf = vi+a*t
 ```
 ```python
 from agnmol.motion import v_final
 # using first equation
 v_final(vi=1, a=3, x_delta=1.5) #output: 10.0
 # using second equation
 v_final(vi=1, a=2.3, t=2) #output: 5.6
 ```
 
-###Average velocity
-
+### Average velocity
 Average velocity is calculated using one of formulas: 
 ```math
 va = x/t
 va = (vi+vf)/2
 ```
 ```python
 from agnmol.motion import v_average
 # using first equation
 v_average(x_delta=1, t=3) #output: 0.3333333333333333
 # using second equation
 v_average(vi=1, vf=2.6) #output: 0.8
 ```
 
-###Acceleration velocity
-
+### Acceleration velocity
 Acceleration velocity is calculated using one of formulas: 
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
```

