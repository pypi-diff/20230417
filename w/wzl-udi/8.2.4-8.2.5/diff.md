# Comparing `tmp/wzl-udi-8.2.4.tar.gz` & `tmp/wzl-udi-8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wzl-udi-8.2.4.tar", last modified: Thu Apr 13 11:49:52 2023, max compression
+gzip compressed data, was "wzl-udi-8.2.5.tar", last modified: Mon Apr 17 20:03:49 2023, max compression
```

## Comparing `wzl-udi-8.2.4.tar` & `wzl-udi-8.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.389940 wzl-udi-8.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10314 2023-04-13 11:49:52.388940 wzl-udi-8.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9659 2023-04-13 11:49:22.000000 wzl-udi-8.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 11:49:52.389940 wzl-udi-8.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-13 11:49:22.000000 wzl-udi-8.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.248940 wzl-udi-8.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.276940 wzl-udi-8.2.4/src/http/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/http/error.py
--rw-rw-rw-   0 root         (0) root         (0)    14897 2023-03-29 04:36:06.000000 wzl-udi-8.2.4/src/http/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.372940 wzl-udi-8.2.4/src/soil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:49:23.000000 wzl-udi-8.2.4/src/soil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19111 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/component.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-02-27 08:41:39.000000 wzl-udi-8.2.4/src/soil/datatype.py
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/element.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/soil/error.py
--rw-rw-rw-   0 root         (0) root         (0)     4965 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/soil/event.py
--rw-rw-rw-   0 root         (0) root         (0)    14273 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/figure.py
--rw-rw-rw-   0 root         (0) root         (0)     9108 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/function.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-03-29 07:22:00.000000 wzl-udi-8.2.4/src/soil/measurement.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/soil/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.387940 wzl-udi-8.2.4/src/utils/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/utils/error.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-25 10:32:29.000000 wzl-udi-8.2.4/src/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2023-02-24 13:15:09.000000 wzl-udi-8.2.4/src/utils/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:49:52.388940 wzl-udi-8.2.4/wzl_udi.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10314 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      627 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 11:49:52.000000 wzl-udi-8.2.4/wzl_udi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.656274 wzl-udi-8.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10403 2023-04-17 20:03:49.656274 wzl-udi-8.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9748 2023-04-17 20:03:41.000000 wzl-udi-8.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 20:03:49.656274 wzl-udi-8.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-17 20:03:41.000000 wzl-udi-8.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.091274 wzl-udi-8.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.162274 wzl-udi-8.2.5/src/http/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/http/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    14897 2023-03-29 04:36:06.000000 wzl-udi-8.2.5/src/http/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.433274 wzl-udi-8.2.5/src/soil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 20:03:41.000000 wzl-udi-8.2.5/src/soil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19111 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/component.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-02-27 08:41:39.000000 wzl-udi-8.2.5/src/soil/datatype.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/element.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/soil/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4965 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/soil/event.py
+-rw-rw-rw-   0 root         (0) root         (0)    14273 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/figure.py
+-rw-rw-rw-   0 root         (0) root         (0)     9108 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-03-29 07:22:00.000000 wzl-udi-8.2.5/src/soil/measurement.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9386 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/soil/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.620274 wzl-udi-8.2.5/src/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/utils/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-25 10:32:29.000000 wzl-udi-8.2.5/src/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-02-24 13:15:09.000000 wzl-udi-8.2.5/src/utils/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:03:49.656274 wzl-udi-8.2.5/wzl_udi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10403 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-17 20:03:49.000000 wzl-udi-8.2.5/wzl_udi.egg-info/top_level.txt
```

### Comparing `wzl-udi-8.2.4/LICENSE` & `wzl-udi-8.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/PKG-INFO` & `wzl-udi-8.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-udi
-Version: 8.2.4
+Version: 8.2.5
 Summary: Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python
 Author: Matthias Bodenbenner
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 8.2.4
+Current stable version: 8.2.5
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -61,14 +61,17 @@
 
 The authors acknowledge funding from the LaVA project (Large Volume Applications, contract 17IND03 of the European Metrology Programme for Innovation and Research EMPIR). The EMPIR initiative is co-funded by the European Union’s Horizon 2020 research and innovation programme and the EMPIR Participating States.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 ## Recent changes
 
+**8.2.5** - 2023-04-17
+  - relaxed required versions of dependencies to avoid conflicts
+
 **8.2.4** - 2023-04-13
   - updated dependency, so that wzl-udi is also compatible with Python 3.11
 
 **8.2.3** - 2023-03-29
   - removed legacy attributes from serialization and streaming
 
 **8.2.2** - 2023-03-29
```

### Comparing `wzl-udi-8.2.4/README.md` & `wzl-udi-8.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 8.2.4
+Current stable version: 8.2.5
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -47,14 +47,17 @@
 
 The authors acknowledge funding from the LaVA project (Large Volume Applications, contract 17IND03 of the European Metrology Programme for Innovation and Research EMPIR). The EMPIR initiative is co-funded by the European Union’s Horizon 2020 research and innovation programme and the EMPIR Participating States.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 ## Recent changes
 
+**8.2.5** - 2023-04-17
+  - relaxed required versions of dependencies to avoid conflicts
+
 **8.2.4** - 2023-04-13
   - updated dependency, so that wzl-udi is also compatible with Python 3.11
 
 **8.2.3** - 2023-03-29
   - removed legacy attributes from serialization and streaming
 
 **8.2.2** - 2023-03-29
```

### Comparing `wzl-udi-8.2.4/setup.py` & `wzl-udi-8.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='wzl-udi',
-      version='8.2.4',
+      version='8.2.5',
       url='https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python',
       project_urls={
           "Bug Tracker": "https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues",
       },
       author='Matthias Bodenbenner',
       author_email='m.bodenbenner@wzl-mq.rwth-aachen.de',
       description='Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).',
@@ -18,13 +18,13 @@
       long_description_content_type="text/markdown",
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
       install_requires=['aiohttp~=3.8.4',
-                        'Deprecated==1.2.13',
-                        'nest-asyncio==1.5.6',
+                        'Deprecated~=1.2.13',
+                        'nest-asyncio~=1.5.6',
                         'strict-rfc3339==0.7',
-                        'wzl-mqtt==2.5.1'
+                        'wzl-mqtt~=2.5.3'
                         ],
       zip_safe=False)
```

### Comparing `wzl-udi-8.2.4/src/http/server.py` & `wzl-udi-8.2.5/src/http/server.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/component.py` & `wzl-udi-8.2.5/src/soil/component.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/datatype.py` & `wzl-udi-8.2.5/src/soil/datatype.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/element.py` & `wzl-udi-8.2.5/src/soil/element.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/error.py` & `wzl-udi-8.2.5/src/soil/error.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/event.py` & `wzl-udi-8.2.5/src/soil/event.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/figure.py` & `wzl-udi-8.2.5/src/soil/figure.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/function.py` & `wzl-udi-8.2.5/src/soil/function.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/measurement.py` & `wzl-udi-8.2.5/src/soil/measurement.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/parameter.py` & `wzl-udi-8.2.5/src/soil/parameter.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/soil/stream.py` & `wzl-udi-8.2.5/src/soil/stream.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/utils/error.py` & `wzl-udi-8.2.5/src/utils/error.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/utils/logger.py` & `wzl-udi-8.2.5/src/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/src/utils/serialize.py` & `wzl-udi-8.2.5/src/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-8.2.4/wzl_udi.egg-info/PKG-INFO` & `wzl-udi-8.2.5/wzl_udi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-udi
-Version: 8.2.4
+Version: 8.2.5
 Summary: Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python
 Author: Matthias Bodenbenner
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 8.2.4
+Current stable version: 8.2.5
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -61,14 +61,17 @@
 
 The authors acknowledge funding from the LaVA project (Large Volume Applications, contract 17IND03 of the European Metrology Programme for Innovation and Research EMPIR). The EMPIR initiative is co-funded by the European Union’s Horizon 2020 research and innovation programme and the EMPIR Participating States.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 ## Recent changes
 
+**8.2.5** - 2023-04-17
+  - relaxed required versions of dependencies to avoid conflicts
+
 **8.2.4** - 2023-04-13
   - updated dependency, so that wzl-udi is also compatible with Python 3.11
 
 **8.2.3** - 2023-03-29
   - removed legacy attributes from serialization and streaming
 
 **8.2.2** - 2023-03-29
```

### Comparing `wzl-udi-8.2.4/wzl_udi.egg-info/SOURCES.txt` & `wzl-udi-8.2.5/wzl_udi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

