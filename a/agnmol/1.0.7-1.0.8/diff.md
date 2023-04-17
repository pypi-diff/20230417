# Comparing `tmp/agnmol-1.0.7.tar.gz` & `tmp/agnmol-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnmol-1.0.7.tar", last modified: Mon Apr 17 16:32:05 2023, max compression
+gzip compressed data, was "agnmol-1.0.8.tar", last modified: Mon Apr 17 16:34:28 2023, max compression
```

## Comparing `agnmol-1.0.7.tar` & `agnmol-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.355975 agnmol-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2040 2023-04-17 16:32:05.352966 agnmol-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-04-17 16:31:46.000000 agnmol-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.338967 agnmol-1.0.7/agnmol/
--rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.7/agnmol/__init__.py
--rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.7/agnmol/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:32:05.351966 agnmol-1.0.7/agnmol.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 16:32:05.000000 agnmol-1.0.7/agnmol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      461 2023-04-17 16:31:46.000000 agnmol-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 16:32:05.355975 agnmol-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.490082 agnmol-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 15:33:58.000000 agnmol-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2298 2023-04-17 16:34:28.477081 agnmol-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-04-17 16:34:05.000000 agnmol-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.448081 agnmol-1.0.8/agnmol/
+-rw-rw-rw-   0        0        0        0 2023-04-15 14:55:12.000000 agnmol-1.0.8/agnmol/__init__.py
+-rw-rw-rw-   0        0        0      916 2023-04-17 16:10:44.000000 agnmol-1.0.8/agnmol/motion.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:34:28.475084 agnmol-1.0.8/agnmol.egg-info/
+-rw-rw-rw-   0        0        0     2298 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 16:34:28.000000 agnmol-1.0.8/agnmol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      461 2023-04-17 16:34:08.000000 agnmol-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 16:34:28.491079 agnmol-1.0.8/setup.cfg
```

### Comparing `agnmol-1.0.7/LICENSE.txt` & `agnmol-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.7/PKG-INFO` & `agnmol-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -76,11 +76,27 @@
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
 # using first equation
-acceleration(v_delta=5, t=2.5) #output: 2.0
+acceleration(v_delta=5, t=2.5) 
+#output: 2.0
 # using second equation
-acceleration(vi=1, vf=6, t=2.5) #output: 2.0
+acceleration(vi=1, vf=6, t=2.5) 
+#output: 2.0
+```
+
+### Acceleration velocity
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+```python
+from agnmol.motion import acceleration
+
+acceleration(v_delta=5, t=2.5) 
+
+acceleration(vi=1, vf=6, t=2.5)
 ```
```

### Comparing `agnmol-1.0.7/README.md` & `agnmol-1.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -64,11 +64,27 @@
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
 # using first equation
-acceleration(v_delta=5, t=2.5) #output: 2.0
+acceleration(v_delta=5, t=2.5) 
+#output: 2.0
 # using second equation
-acceleration(vi=1, vf=6, t=2.5) #output: 2.0
+acceleration(vi=1, vf=6, t=2.5) 
+#output: 2.0
+```
+
+### Acceleration velocity
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+```python
+from agnmol.motion import acceleration
+
+acceleration(v_delta=5, t=2.5) 
+
+acceleration(vi=1, vf=6, t=2.5)
 ```
```

### Comparing `agnmol-1.0.7/agnmol/motion.py` & `agnmol-1.0.8/agnmol/motion.py`

 * *Files identical despite different names*

### Comparing `agnmol-1.0.7/agnmol.egg-info/PKG-INFO` & `agnmol-1.0.8/agnmol.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agnmol
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for physics motion calculations
 Author-email: agnmol <agnmol@ktu.lt>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -76,11 +76,27 @@
 ```math
 a = v/t
 a = (vf+vi)/t
 ```
 ```python
 from agnmol.motion import acceleration
 # using first equation
-acceleration(v_delta=5, t=2.5) #output: 2.0
+acceleration(v_delta=5, t=2.5) 
+#output: 2.0
 # using second equation
-acceleration(vi=1, vf=6, t=2.5) #output: 2.0
+acceleration(vi=1, vf=6, t=2.5) 
+#output: 2.0
+```
+
+### Acceleration velocity
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+```python
+from agnmol.motion import acceleration
+
+acceleration(v_delta=5, t=2.5) 
+
+acceleration(vi=1, vf=6, t=2.5)
 ```
```

