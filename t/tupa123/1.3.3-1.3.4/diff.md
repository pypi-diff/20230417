# Comparing `tmp/tupa123-1.3.3.tar.gz` & `tmp/tupa123-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.3.tar", last modified: Mon Apr 17 14:28:02 2023, max compression
+gzip compressed data, was "tupa123-1.3.4.tar", last modified: Mon Apr 17 19:23:23 2023, max compression
```

## Comparing `tupa123-1.3.3.tar` & `tupa123-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.907846 tupa123-1.3.3/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     7810 2023-04-17 14:28:02.906850 tupa123-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     7334 2023-04-17 14:18:59.000000 tupa123-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 14:28:02.907846 tupa123-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 14:09:16.000000 tupa123-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.894943 tupa123-1.3.3/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.3/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 13:58:16.000000 tupa123-1.3.3/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:28:02.904859 tupa123-1.3.3/tupa123.egg-info/
--rw-rw-rw-   0        0        0     7810 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 14:28:02.000000 tupa123-1.3.3/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 19:23:23.588434 tupa123-1.3.4/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     7905 2023-04-17 19:23:23.587465 tupa123-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7429 2023-04-17 19:22:38.000000 tupa123-1.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 19:23:23.588434 tupa123-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 19:21:03.000000 tupa123-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:23:23.575507 tupa123-1.3.4/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.4/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 13:58:16.000000 tupa123-1.3.4/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-17 19:23:23.585440 tupa123-1.3.4/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     7905 2023-04-17 19:23:23.000000 tupa123-1.3.4/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-17 19:23:23.000000 tupa123-1.3.4/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 19:23:23.000000 tupa123-1.3.4/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 19:23:23.000000 tupa123-1.3.4/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 19:23:23.000000 tupa123-1.3.4/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.3/LICENSE.txt` & `tupa123-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.3/PKG-INFO` & `tupa123-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.3
+Version: 1.3.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,14 +14,16 @@
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+<br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

### Comparing `tupa123-1.3.3/README.md` & `tupa123-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+<br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

### Comparing `tupa123-1.3.3/setup.py` & `tupa123-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.3',
+    version='1.3.4',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.3/tupa123/tupa123.py` & `tupa123-1.3.4/tupa123/tupa123.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.3/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.4/tupa123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.3
+Version: 1.3.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,14 +14,16 @@
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
 <br>
 #Manual = https://www.mediafire.com/file/xygt3o9zf7iw3id/Manual_Tupa123.pdf <br>
 <br>
+#Quick Guide = https://www.mediafire.com/file/a0db7fb3lfsxvaj/Guia_Rapido.pdf/file <br>
+<br>
 #Excel example data = https://www.mediafire.com/file/o2nzsmnvweh8w1a/ALETAS.xlsx<br>
 #Excel example (old version) = https://www.mediafire.com/file/0xmx5quakd21txu/ALETAS.xls <br>
 <br>
 <br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
```

