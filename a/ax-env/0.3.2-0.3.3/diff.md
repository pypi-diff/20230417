# Comparing `tmp/ax_env-0.3.2.tar.gz` & `tmp/ax_env-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ax_env-0.3.2.tar", last modified: Fri Feb 17 14:25:41 2023, max compression
+gzip compressed data, was "ax_env-0.3.3.tar", last modified: Mon Apr 17 19:18:17 2023, max compression
```

## Comparing `ax_env-0.3.2.tar` & `ax_env-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:25:41.726645 ax_env-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-02-17 14:25:41.726645 ax_env-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-17 14:25:39.000000 ax_env-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:25:41.726645 ax_env-0.3.2/ax_env/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-17 14:25:39.000000 ax_env-0.3.2/ax_env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:25:41.726645 ax_env-0.3.2/ax_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-17 14:25:41.000000 ax_env-0.3.2/ax_env.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:25:41.726645 ax_env-0.3.2/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-17 14:25:39.000000 ax_env-0.3.2/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 14:25:41.726645 ax_env-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-17 14:25:39.000000 ax_env-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:17.921717 ax_env-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-04-17 19:18:17.921717 ax_env-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-17 19:18:15.000000 ax_env-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:17.921717 ax_env-0.3.3/ax_env/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 19:18:15.000000 ax_env-0.3.3/ax_env/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:17.921717 ax_env-0.3.3/ax_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 19:18:17.000000 ax_env-0.3.3/ax_env.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:18:17.921717 ax_env-0.3.3/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-17 19:18:15.000000 ax_env-0.3.3/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:18:17.921717 ax_env-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-17 19:18:15.000000 ax_env-0.3.3/setup.py
```

### Comparing `ax_env-0.3.2/PKG-INFO` & `ax_env-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax_env
-Version: 0.3.2
+Version: 0.3.3
 Summary: dependency manager for XENONnT package
 Home-page: https://github.com/XENONnT/ax_env
 Author: J. R. Angevaare
 License: UNKNOWN
 Description: # Ax env
         [![Test package](https://github.com/XENONnT/ax_env/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/ax_env/actions/workflows/pytest.yml) 
         [![PyPI version shields.io](https://img.shields.io/pypi/v/ax_env.svg)](https://pypi.python.org/pypi/ax_env/)
```

### Comparing `ax_env-0.3.2/README.md` & `ax_env-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ax_env-0.3.2/ax_env.egg-info/PKG-INFO` & `ax_env-0.3.3/ax_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax-env
-Version: 0.3.2
+Version: 0.3.3
 Summary: dependency manager for XENONnT package
 Home-page: https://github.com/XENONnT/ax_env
 Author: J. R. Angevaare
 License: UNKNOWN
 Description: # Ax env
         [![Test package](https://github.com/XENONnT/ax_env/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/ax_env/actions/workflows/pytest.yml) 
         [![PyPI version shields.io](https://img.shields.io/pypi/v/ax_env.svg)](https://pypi.python.org/pypi/ax_env/)
```

### Comparing `ax_env-0.3.2/ax_env.egg-info/requires.txt` & `ax_env-0.3.3/ax_env.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 fsspec==2022.11.0
 gitpython==3.1.30
 holoviews==1.15.4
 hypothesis==6.46.2
 immutabledict==2.2.3
 ipywidgets==8.0.4
 jinja2==3.1.2
-jupyter-client==8.0.2
+jupyter-client==8.0.3
 keras==2.11.0
 lz4==4.3.2
 matplotlib==3.5.3
 memory_profiler==0.61.0
 mongomock==4.1.2
 multihist==0.6.5
 nbmake==1.4.1
@@ -35,19 +35,19 @@
 panel==0.14.3
 pdmongo==0.3.4
 psutil==5.9.4
 pymongo==3.13.0
 pytest==7.2.1
 pytest-cov==4.0.0
 pytest-xdist==3.2.0
-rframe==0.2.5
+rframe==0.2.6
 scikit-learn==1.2.1
 scipy==1.10.0
 tensorflow==2.11.0
 typing_extensions==4.5.0
 tqdm==4.64.1
 uproot==4.3.7
 utilix==0.7.2
 xarray==2022.12.0
-xedocs==0.2.10
+xedocs==0.2.14
 zarr==2.14.1
 zstd==1.5.4.0
```

### Comparing `ax_env-0.3.2/extra_requirements/requirements-tests.txt` & `ax_env-0.3.3/extra_requirements/requirements-tests.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 fsspec==2022.11.0
 gitpython==3.1.30
 holoviews==1.15.4
 hypothesis==6.46.2
 immutabledict==2.2.3
 ipywidgets==8.0.4
 jinja2==3.1.2
-jupyter-client==8.0.2
+jupyter-client==8.0.3
 keras==2.11.0
 lz4==4.3.2
 matplotlib==3.5.3
 memory_profiler==0.61.0
 mongomock==4.1.2
 multihist==0.6.5
 nbmake==1.4.1
@@ -35,19 +35,19 @@
 panel==0.14.3
 pdmongo==0.3.4
 psutil==5.9.4
 pymongo==3.13.0
 pytest==7.2.1
 pytest-cov==4.0.0
 pytest-xdist==3.2.0
-rframe==0.2.5
+rframe==0.2.6
 scikit-learn==1.2.1
 scipy==1.10.0
 tensorflow== 2.11.0
 typing_extensions==4.5.0
 tqdm==4.64.1
 uproot==4.3.7
 utilix==0.7.2
 xarray==2022.12.0
-xedocs==0.2.10
+xedocs==0.2.14
 zarr==2.14.1
 zstd==1.5.4.0
```

### Comparing `ax_env-0.3.2/setup.py` & `ax_env-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 requires = open_requirements('extra_requirements/requirements-tests.txt')
 
 setuptools.setup(name='ax_env',
-                 version='0.3.2',
+                 version='0.3.3',
                  description='dependency manager for XENONnT package',
                  author='J. R. Angevaare',
                  url='https://github.com/XENONnT/ax_env',
                  long_description=readme + '\n\n' + history,
                  long_description_content_type="text/markdown",
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
```

