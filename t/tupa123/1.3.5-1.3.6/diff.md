# Comparing `tmp/tupa123-1.3.5.tar.gz` & `tmp/tupa123-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.5.tar", last modified: Mon Apr 17 20:58:36 2023, max compression
+gzip compressed data, was "tupa123-1.3.6.tar", last modified: Mon Apr 17 21:01:09 2023, max compression
```

## Comparing `tupa123-1.3.5.tar` & `tupa123-1.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:58:36.551152 tupa123-1.3.5/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0     7905 2023-04-17 20:58:36.550184 tupa123-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     7429 2023-04-17 19:22:38.000000 tupa123-1.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 20:58:36.551152 tupa123-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 20:51:50.000000 tupa123-1.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:58:36.538214 tupa123-1.3.5/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.5/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.5/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:58:36.548161 tupa123-1.3.5/tupa123.egg-info/
--rw-rw-rw-   0        0        0     7905 2023-04-17 20:58:36.000000 tupa123-1.3.5/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-17 20:58:36.000000 tupa123-1.3.5/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:58:36.000000 tupa123-1.3.5/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-17 20:58:36.000000 tupa123-1.3.5/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 20:58:36.000000 tupa123-1.3.5/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.546476 tupa123-1.3.6/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     7904 2023-04-17 21:01:09.545507 tupa123-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7428 2023-04-17 21:00:27.000000 tupa123-1.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:01:09.546476 tupa123-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 21:00:39.000000 tupa123-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.534536 tupa123-1.3.6/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.6/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.6/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:01:09.543513 tupa123-1.3.6/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     7904 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 21:01:09.000000 tupa123-1.3.6/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.5/LICENSE.txt` & `tupa123-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.5/PKG-INFO` & `tupa123-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.5
+Version: 1.3.6
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -69,18 +69,18 @@
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
-#norma = type of data normalization: (default=2)<br>
+#norma = type of data normalization: <br>
 #=-1, standardization <br>
 #=0, do anything <br>
-#=1, between 0 and 1 <br>
+#=1, between 0 and 1 (default) <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
```

### Comparing `tupa123-1.3.5/README.md` & `tupa123-1.3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,18 +58,18 @@
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
-#norma = type of data normalization: (default=2)<br>
+#norma = type of data normalization: <br>
 #=-1, standardization <br>
 #=0, do anything <br>
-#=1, between 0 and 1 <br>
+#=1, between 0 and 1 (default) <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
```

### Comparing `tupa123-1.3.5/setup.py` & `tupa123-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.5',
+    version='1.3.6',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.5/tupa123/tupa123.py` & `tupa123-1.3.6/tupa123/tupa123.py`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.5/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.6/tupa123.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.5
+Version: 1.3.6
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -69,18 +69,18 @@
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1)</b> <br>
 #creates the Neural Network model <br>
 <br>
-#norma = type of data normalization: (default=2)<br>
+#norma = type of data normalization: <br>
 #=-1, standardization <br>
 #=0, do anything <br>
-#=1, between 0 and 1 <br>
+#=1, between 0 and 1 (default) <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
 #normout = if 1 normalizes the output (default=1), 0 dont <br>
```

