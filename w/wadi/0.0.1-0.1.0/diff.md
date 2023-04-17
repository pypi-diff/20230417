# Comparing `tmp/WADI-0.0.1.tar.gz` & `tmp/wadi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\WADI-0.0.1.tar", last modified: Mon Aug 29 14:47:34 2022, max compression
+gzip compressed data, was "wadi-0.1.0.tar", last modified: Mon Apr 17 10:48:16 2023, max compression
```

## Comparing `WADI-0.0.1.tar` & `wadi-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-08-29 14:47:34.000000 WADI-0.0.1/
--rw-rw-rw-   0        0        0     2290 2022-08-29 14:47:34.000000 WADI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      973 2022-08-29 14:40:53.000000 WADI-0.0.1/README.rst
--rw-rw-rw-   0        0        0       87 2022-08-29 14:47:34.000000 WADI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1542 2022-08-29 14:46:23.000000 WADI-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-29 14:47:34.000000 WADI-0.0.1/testing/
--rw-rw-rw-   0        0        0     8836 2022-08-29 14:47:16.000000 WADI-0.0.1/testing/test_removal_functions.py
--rw-rw-rw-   0        0        0        0 2022-08-29 14:34:21.000000 WADI-0.0.1/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI/
--rw-rw-rw-   0        0        0    18474 2022-08-29 14:34:21.000000 WADI-0.0.1/WADI/removal_functions.py
--rw-rw-rw-   0        0        0        0 2022-08-29 14:34:21.000000 WADI-0.0.1/WADI/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/
--rw-rw-rw-   0        0        0        1 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2290 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/requires.txt
--rw-rw-rw-   0        0        0      265 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2022-08-29 14:47:34.000000 WADI-0.0.1/WADI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.219895 wadi-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 10:48:05.000000 wadi-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 10:48:16.219895 wadi-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 10:48:05.000000 wadi-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:48:16.219895 wadi-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-17 10:48:05.000000 wadi-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.215895 wadi-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 10:48:05.000000 wadi-0.1.0/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.215895 wadi-0.1.0/wadi/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/harmonizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28719 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.219895 wadi-0.1.0/wadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `WADI-0.0.1/setup.py` & `wadi-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-import os
-from setuptools import setup, find_packages
-
-def read(fname):
-    with open(os.path.join(os.path.dirname(__file__), fname)) as f:
-        return f.read()
-
-setup(
-    name='WADI',
-    version='0.0.1',
-    packages=find_packages(exclude=['tests*']),
-    license='MIT',
-    description='A python package for calculating the removal of microbial organisms in the subsurface',
-    long_description=read('README.rst'),
-    long_description_content_type="text/x-rst",
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'Intended Audience :: Other Audience',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Topic :: Scientific/Engineering :: Hydrology',
-    ],
-    python_requires='>=3.7',
-    project_urls={
-    'Source': 'https://github.com/steven-ros/WADI',
-    'Documentation': 'http://WADI.readthedocs.io/en/latest/',
-    'Tracker': 'https://github.com/steven-ros/WADI/issues',
-    'Help': 'https://github.com/steven-ros/WADI/issues',
-    # 'Help': 'https://stackoverflow.com/questions/tagged/WADI'
-    },
-    install_requires=[
-        'pandas>=0.23',
-
-        ],
-    include_package_data=True,
-    url='https://github.com/steven-ros/WADI',
-    author='KWR Water Research Institute',
-    author_email='vincent.post@kwrwater.nl, martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl, steven.ros@kwrwater.nl'
-)
+import os
+from setuptools import setup, find_packages
+
+def read(fname):
+    with open(os.path.join(os.path.dirname(__file__), fname)) as f:
+        return f.read()
+
+setup(
+    name='wadi',
+    version='0.1.0',
+    packages=find_packages(exclude=['tests*']),
+    license='MIT',
+    description='Generic importer for water quality data of the (Dutch) water laboratory',
+    long_description=read('README.md'),
+    long_description_content_type="text/x-rst",
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Science/Research',
+        'Intended Audience :: Other Audience',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Scientific/Engineering :: Hydrology',
+    ],
+    python_requires='>=3.9',
+    project_urls={
+    'Source': 'https://github.com/KWR-Water/wadi',
+    'Documentation': 'http://wadi.readthedocs.io/en/latest/',
+    'Tracker': 'https://github.com/KWR-Water/wadi/issues',
+    'Help': 'https://github.com/KWR-Water/wadi/issues'
+    },
+    install_requires=[
+        'pandas>=0.23',
+        'pint',
+        'requests',
+        'molmass',
+        'openpyxl>=3.0.0',
+        'googletrans',
+        'fuzzywuzzy'
+        ],
+    include_package_data=True,
+    url='https://github.com/KWR-Water/wadi',
+    author='KWR Water Research Institute',
+    author_email='martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl',
+)
```

