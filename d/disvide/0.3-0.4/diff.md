# Comparing `tmp/disvide-0.3.tar.gz` & `tmp/disvide-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disvide-0.3.tar", last modified: Mon Apr 17 14:35:23 2023, max compression
+gzip compressed data, was "disvide-0.4.tar", last modified: Mon Apr 17 14:38:02 2023, max compression
```

## Comparing `disvide-0.3.tar` & `disvide-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:35:23.827973 disvide-0.3/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.3/LICENSE
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:35:23.827973 disvide-0.3/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.3/README.rst
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:35:23.827973 disvide-0.3/disvide.egg-info/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       51 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/entry_points.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/requires.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:35:23.000000 disvide-0.3/disvide.egg-info/top_level.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:35:23.827973 disvide-0.3/setup.cfg
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      633 2023-04-17 14:34:48.000000 disvide-0.3/setup.py
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:38:02.517977 disvide-0.4/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.4/LICENSE
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3081 2023-04-17 14:38:02.517977 disvide-0.4/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.4/README.rst
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:38:02.517977 disvide-0.4/disvide.egg-info/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     3081 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      225 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       51 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/entry_points.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)       22 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/requires.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:38:02.000000 disvide-0.4/disvide.egg-info/top_level.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:38:02.517977 disvide-0.4/setup.cfg
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      791 2023-04-17 14:37:57.000000 disvide-0.4/setup.py
```

### Comparing `disvide-0.3/LICENSE` & `disvide-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `disvide-0.3/README.rst` & `disvide-0.4/README.rst`

 * *Files identical despite different names*

### Comparing `disvide-0.3/setup.py` & `disvide-0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
 
+with open('README.rst', 'r') as f:
+    long_description = f.read()
+
 setup(
     name='disvide',
-    version='0.3',
+    version='0.4',
     license='MIT',
     author='Cored Developments',
     author_email='skyblockmohammed@gmail.com',
     packages=find_packages(),
     url='https://github.com/Cored-Inc/disvide',
     description='Disvide is a beginner-friendly Discord bot generator that allows you to create a bot by answering a few questions.',
     keywords='discord bot generator beginner',
@@ -14,9 +17,11 @@
         'questionary',
         'termcolor'
     ],
     entry_points={
         'console_scripts': [
             'my_package=my_package.cli:main'
         ]
-    }
+    },
+    long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

