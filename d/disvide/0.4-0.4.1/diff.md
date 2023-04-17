# Comparing `tmp/disvide-0.4.tar.gz` & `tmp/disvide-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disvide-0.4.tar", last modified: Mon Apr 17 14:38:02 2023, max compression
+gzip compressed data, was "disvide-0.4.1.tar", last modified: Mon Apr 17 14:44:05 2023, max compression
```

## Comparing `disvide-0.4.tar` & `disvide-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:38:02.517977 disvide-0.4/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4/LICENSE
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3081 2023-04-17 14:38:02.517977 disvide-0.4/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.4/README.rst
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:38:02.517977 disvide-0.4/disvide.egg-info/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3081 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       51 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/entry_points.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/requires.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/top_level.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:38:02.517977 disvide-0.4/setup.cfg
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      791 2023-04-17 14:37:57.000000 disvide-0.4/setup.py
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:44:05.057975 disvide-0.4.1/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4.1/LICENSE
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3083 2023-04-17 14:44:05.057975 disvide-0.4.1/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.4.1/README.rst
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:44:05.057975 disvide-0.4.1/disvide.egg-info/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3083 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       47 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/entry_points.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/requires.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:44:05.000000 disvide-0.4.1/disvide.egg-info/top_level.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:44:05.057975 disvide-0.4.1/setup.cfg
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      789 2023-04-17 14:44:00.000000 disvide-0.4.1/setup.py
```

### Comparing `disvide-0.4/LICENSE` & `disvide-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `disvide-0.4/PKG-INFO` & `disvide-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disvide
-Version: 0.4
+Version: 0.4.1
 Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
 Home-page: https://github.com/Cored-Inc/disvide
 Author: Cored Developments
 Author-email: skyblockmohammed@gmail.com
 License: MIT
 Keywords: discord bot generator beginner
 Description-Content-Type: text/markdown
```

### Comparing `disvide-0.4/README.rst` & `disvide-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `disvide-0.4/disvide.egg-info/PKG-INFO` & `disvide-0.4.1/disvide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disvide
-Version: 0.4
+Version: 0.4.1
 Summary: Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.
 Home-page: https://github.com/Cored-Inc/disvide
 Author: Cored Developments
 Author-email: skyblockmohammed@gmail.com
 License: MIT
 Keywords: discord bot generator beginner
 Description-Content-Type: text/markdown
```

### Comparing `disvide-0.4/setup.py` & `disvide-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name='disvide',
-    version='0.4',
+    version='0.4.1',
     license='MIT',
     author='Cored Developments',
     author_email='skyblockmohammed@gmail.com',
     packages=find_packages(),
     url='https://github.com/Cored-Inc/disvide',
     description='Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.',
     keywords='discord bot generator beginner',
     install_requires=[
         'questionary',
         'termcolor'
     ],
     entry_points={
         'console_scripts': [
-            'my_package=my_package.cli:main'
+            'disvide=disvide:create_bot'
         ]
     },
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

