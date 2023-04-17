# Comparing `tmp/tmpeco-1.2.tar.gz` & `tmp/tmpeco-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmpeco-1.2.tar", last modified: Mon Apr 17 03:13:05 2023, max compression
+gzip compressed data, was "tmpeco-1.3.tar", last modified: Mon Apr 17 03:18:20 2023, max compression
```

## Comparing `tmpeco-1.2.tar` & `tmpeco-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:13:05.979684 tmpeco-1.2/
--rw-rw-rw-   0        0        0     1715 2023-04-17 03:13:05.978687 tmpeco-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1299 2023-04-16 16:55:22.000000 tmpeco-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 03:13:05.979684 tmpeco-1.2/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-04-17 03:11:28.000000 tmpeco-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:13:05.947770 tmpeco-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:13:05.976693 tmpeco-1.2/src/tmpeco/
--rw-rw-rw-   0        0        0     6350 2023-04-15 23:34:29.000000 tmpeco-1.2/src/tmpeco/BCRP.py
--rw-rw-rw-   0        0        0     2820 2023-04-14 08:10:41.000000 tmpeco-1.2/src/tmpeco/BM.py
--rw-rw-rw-   0        0        0     3554 2023-04-14 08:10:41.000000 tmpeco-1.2/src/tmpeco/FRED.py
--rw-rw-rw-   0        0        0     2112 2023-04-15 23:34:08.000000 tmpeco-1.2/src/tmpeco/OECD.py
--rw-rw-rw-   0        0        0     3583 2023-04-16 17:04:40.000000 tmpeco-1.2/src/tmpeco/YFinance.py
--rw-rw-rw-   0        0        0       63 2023-04-16 17:41:14.000000 tmpeco-1.2/src/tmpeco/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:13:05.971706 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/
--rw-rw-rw-   0        0        0     1715 2023-04-17 03:13:05.000000 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-04-17 03:13:05.000000 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:13:05.000000 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-17 03:13:05.000000 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2023-04-17 03:13:05.000000 tmpeco-1.2/src/tmpeco/tmpeco.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 03:18:20.467984 tmpeco-1.3/
+-rw-rw-rw-   0        0        0     1715 2023-04-17 03:18:20.467984 tmpeco-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1299 2023-04-16 16:55:22.000000 tmpeco-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:18:20.468981 tmpeco-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-04-17 03:16:35.000000 tmpeco-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:18:20.439981 tmpeco-1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 03:18:20.465989 tmpeco-1.3/src/tmpeco/
+-rw-rw-rw-   0        0        0     6350 2023-04-15 23:34:29.000000 tmpeco-1.3/src/tmpeco/BCRP.py
+-rw-rw-rw-   0        0        0     2820 2023-04-14 08:10:41.000000 tmpeco-1.3/src/tmpeco/BM.py
+-rw-rw-rw-   0        0        0     3554 2023-04-14 08:10:41.000000 tmpeco-1.3/src/tmpeco/FRED.py
+-rw-rw-rw-   0        0        0     2112 2023-04-15 23:34:08.000000 tmpeco-1.3/src/tmpeco/OECD.py
+-rw-rw-rw-   0        0        0     3583 2023-04-16 17:04:40.000000 tmpeco-1.3/src/tmpeco/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 03:16:12.000000 tmpeco-1.3/src/tmpeco/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:18:20.460005 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/
+-rw-rw-rw-   0        0        0     1715 2023-04-17 03:18:20.000000 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-04-17 03:18:20.000000 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:18:20.000000 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-17 03:18:20.000000 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2023-04-17 03:18:20.000000 tmpeco-1.3/src/tmpeco/tmpeco.egg-info/top_level.txt
```

### Comparing `tmpeco-1.2/PKG-INFO` & `tmpeco-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmpeco
-Version: 1.2
+Version: 1.3
 Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tmpeco-1.2/README.md` & `tmpeco-1.3/README.md`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/setup.py` & `tmpeco-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='tmpeco',
-    version = '1.2',
+    version = '1.3',
     author = 'Mauricio Alvarado, Andrei Romero',
     description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     # url='https://github.com/mauricioalvaradoo/econdata',
     classifiers = [
         'Programming Language :: Python :: 3',
```

### Comparing `tmpeco-1.2/src/tmpeco/BCRP.py` & `tmpeco-1.3/src/tmpeco/BCRP.py`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/src/tmpeco/BM.py` & `tmpeco-1.3/src/tmpeco/BM.py`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/src/tmpeco/FRED.py` & `tmpeco-1.3/src/tmpeco/FRED.py`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/src/tmpeco/OECD.py` & `tmpeco-1.3/src/tmpeco/OECD.py`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/src/tmpeco/YFinance.py` & `tmpeco-1.3/src/tmpeco/YFinance.py`

 * *Files identical despite different names*

### Comparing `tmpeco-1.2/src/tmpeco/tmpeco.egg-info/PKG-INFO` & `tmpeco-1.3/src/tmpeco/tmpeco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmpeco
-Version: 1.2
+Version: 1.3
 Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tmpeco-1.2/src/tmpeco/tmpeco.egg-info/SOURCES.txt` & `tmpeco-1.3/src/tmpeco/tmpeco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

