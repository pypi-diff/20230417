# Comparing `tmp/arrendatools_plantillas-1.0.3.tar.gz` & `tmp/arrendatools_plantillas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools_plantillas-1.0.3.tar", last modified: Sun Apr 16 11:28:46 2023, max compression
+gzip compressed data, was "arrendatools_plantillas-1.1.0.tar", last modified: Sun Apr 16 18:48:46 2023, max compression
```

## Comparing `arrendatools_plantillas-1.0.3.tar` & `arrendatools_plantillas-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1100 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/arrendatools_plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/arrendatools_plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas/filters/numero_a_palabras.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-16 11:28:43.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 11:28:46.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-04-16 11:28:46.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 11:28:46.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-16 11:28:46.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 11:28:46.000000 arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-16 11:28:46.203742 arrendatools_plantillas-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-16 11:28:44.000000 arrendatools_plantillas-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:48:46.799828 arrendatools_plantillas-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 18:48:46.799828 arrendatools_plantillas-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:48:46.795828 arrendatools_plantillas-1.1.0/arrendatools_plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:48:46.799828 arrendatools_plantillas-1.1.0/arrendatools_plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas/filters/formato_fecha.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas/filters/numero_a_palabras.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:48:46.799828 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      751 2023-04-16 18:48:46.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      489 2023-04-16 18:48:46.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:48:46.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-16 18:48:46.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 18:48:46.000000 arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-16 18:48:46.799828 arrendatools_plantillas-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-16 18:48:44.000000 arrendatools_plantillas-1.1.0/setup.py
```

### Comparing `arrendatools_plantillas-1.0.3/LICENSE` & `arrendatools_plantillas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-1.0.3/PKG-INFO` & `arrendatools_plantillas-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools_plantillas
-Version: 1.0.3
+Version: 1.1.0
 Summary: Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_plantillas-1.0.3/README.md` & `arrendatools_plantillas-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-1.0.3/arrendatools_plantillas/filters/numero_a_palabras.py` & `arrendatools_plantillas-1.1.0/arrendatools_plantillas/filters/numero_a_palabras.py`

 * *Files identical despite different names*

### Comparing `arrendatools_plantillas-1.0.3/arrendatools_plantillas.egg-info/PKG-INFO` & `arrendatools_plantillas-1.1.0/arrendatools_plantillas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools-plantillas
-Version: 1.0.3
+Version: 1.1.0
 Summary: Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `arrendatools_plantillas-1.0.3/setup.py` & `arrendatools_plantillas-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
-__version__ = "1.0.3"
+__version__ = "1.1.0"
 
 setup(
     name='arrendatools_plantillas',
     version=__version__,
     description='Módulo de Python que aplica plantillas usando jinja 2. Además incluye algunos filtros adicionales como el convertir un número a palabras.',
     url='https://github.com/hokus15/ArrendaToolsPlantillas',
     author='hokus15',
     author_email='hokus@hotmail.com',
     license='MIT',
     packages=['arrendatools_plantillas', 'arrendatools_plantillas.filters'],
-    install_requires=['num2words==0.5.12', 'jinja2==3.1.2'],
+    install_requires=['num2words==0.5.12', 'jinja2==3.1.2', 'python-dateutil==2.8.2'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

