# Comparing `tmp/dknovautils-0.0.22.tar.gz` & `tmp/dknovautils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.0.22.tar", last modified: Sun Apr 16 15:50:17 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.0.3.tar", last modified: Thu Mar  9 05:00:48 2023, max compression
```

## Comparing `dknovautils-0.0.22.tar` & `dknovautils-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,18 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-16 15:50:17.000000 dknovautils-0.0.22/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1606 2023-04-16 15:49:57.000000 dknovautils-0.0.22/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1440 2023-04-16 15:50:16.000000 dknovautils-0.0.22/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1510 2023-04-13 12:40:40.000000 dknovautils-0.0.22/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      416 2023-04-16 14:11:46.000000 dknovautils-0.0.22/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      441 2023-04-16 15:50:16.000000 dknovautils-0.0.22/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.0.22/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.0.22/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.0.22/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      148 2023-04-13 15:12:35.000000 dknovautils-0.0.22/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       49 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-04-16 15:50:17.000000 dknovautils-0.0.22/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.22/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      881 2023-04-16 15:50:17.000000 dknovautils-0.0.22/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.0.22/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-04-16 15:50:17.000000 dknovautils-0.0.22/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1141 2023-04-16 15:50:16.000000 dknovautils-0.0.22/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      156 2023-03-09 04:55:58.000000 dknovautils-0.0.3/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-03-09 03:20:10.000000 dknovautils-0.0.3/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        2 2023-03-09 04:42:46.000000 dknovautils-0.0.3/dknovautils/files.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       49 2023-03-09 04:42:48.000000 dknovautils-0.0.3/dknovautils/test_a.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 02:42:43.000000 dknovautils-0.0.3/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      313 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-03-09 05:00:48.000000 dknovautils-0.0.3/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.0.3/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      678 2023-03-09 05:00:48.000000 dknovautils-0.0.3/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      271 2023-03-09 04:58:34.000000 dknovautils-0.0.3/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-03-09 05:00:48.000000 dknovautils-0.0.3/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1075 2023-03-09 05:00:42.000000 dknovautils-0.0.3/setup.py
```

### Comparing `dknovautils-0.0.22/setup.py` & `dknovautils-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.0.22'
+version = "0.0.03"
 
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
+with open("README.md", "r",encoding="utf-8") as f:
+  long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
-    version=DkAppVer,
+    version=version,
     author="dknova",
     author_email="dknova@example.com",
     description="This is the tools for dknova.",
     long_description=long_description,
     # long_description_content_type="text/markdown",
     url="http://example.com",
     install_requires=[
         'requests!=2.9.0',
         'lxml>=4.2.3',
         'monotonic>=1.5',
-        'numpy',
     ],
     packages=setuptools.find_packages(exclude=("test")),
     classifiers=(
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
 
         "Programming Language :: Python :: 3.7"
     ),
-    exclude_package_data={'': ["*.txt", "*.adoc", "*.sh", "dknovautils/test.py",
-                               "dknovautils/config.txt", "dknovautils/*.sh", "dknovautils/test*.py"]},
+    exclude_package_data={'': ["*.txt","*.adoc","dknovautils/test.py", "dknovautils/config.txt","dknovautils/*.sh","dknovautils/test*.py"]},
 )
```

