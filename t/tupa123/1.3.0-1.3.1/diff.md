# Comparing `tmp/tupa123-1.3.0.tar.gz` & `tmp/tupa123-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.0.tar", last modified: Fri Apr 14 21:02:26 2023, max compression
+gzip compressed data, was "tupa123-1.3.1.tar", last modified: Mon Apr 17 11:29:17 2023, max compression
```

## Comparing `tupa123-1.3.0.tar` & `tupa123-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.448205 tupa123-1.3.0/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     7490 2023-04-14 21:02:26.448205 tupa123-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7127 2023-04-14 21:01:08.000000 tupa123-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 21:02:26.448205 tupa123-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-04-14 21:01:41.000000 tupa123-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.438202 tupa123-1.3.0/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.0/tupa123/__init__.py
--rw-rw-rw-   0        0        0    60174 2023-04-14 13:18:14.000000 tupa123-1.3.0/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.448205 tupa123-1.3.0/tupa123.egg-info/
--rw-rw-rw-   0        0        0     7490 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 11:29:17.563049 tupa123-1.3.1/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     7490 2023-04-17 11:29:17.563049 tupa123-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7127 2023-04-14 21:01:08.000000 tupa123-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:29:17.563049 tupa123-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-04-17 11:27:47.000000 tupa123-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:29:17.547431 tupa123-1.3.1/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.1/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    60186 2023-04-17 11:17:01.000000 tupa123-1.3.1/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:29:17.563049 tupa123-1.3.1/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     7490 2023-04-17 11:29:17.000000 tupa123-1.3.1/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-17 11:29:17.000000 tupa123-1.3.1/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:29:17.000000 tupa123-1.3.1/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 11:29:17.000000 tupa123-1.3.1/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 11:29:17.000000 tupa123-1.3.1/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.0/LICENSE.txt` & `tupa123-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.0/PKG-INFO` & `tupa123-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.0
+Version: 1.3.1
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.3.0/README.md` & `tupa123-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.0/setup.py` & `tupa123-1.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.0',
+    version='1.3.1',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
-    install_requires=['numpy>=1.23.5','matplotlib>=3.6.3','pandas>=1.5.3'],    
+    install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='artificial-intelligence neural-networks four-layers regression classification tupa123'
 )
```

### Comparing `tupa123-1.3.0/tupa123/tupa123.py` & `tupa123-1.3.1/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
             return y
 
         if (typee==3): #gaussinana (0,1)
             y = np.exp(-1*(x**2)) 
             return y
 
         if (typee==4): #ReLU (0,inf)
-            y=np.where(x < 0, 0, x)       
+            y=np.where(x < 1e-8, 1e-8, x)       
             return y
 
         if (typee==5): #tanh (-1,1)
             y = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             return y
 
         if (typee==6): #LReLU (-inf,inf)
@@ -603,15 +603,15 @@
             return y
     
         if (typee==3): #gaussinana (0,1)
             y = -2*x*np.exp(-1*(x**2)) 
             return y
 
         if (typee==4): #ReLU (0,inf)
-            y=np.where(x < 0, 0, 1)       
+            y=np.where(x < 1e-8, 1e-8, 1)       
             return y    
 
         if (typee==5): #tanh (-1,1)
             w = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             y = 1 - w**2
             return y
```

### Comparing `tupa123-1.3.0/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.1/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.0
+Version: 1.3.1
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

