# Comparing `tmp/pycpep-1.0.5.tar.gz` & `tmp/pycpep-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycpep-1.0.5.tar", last modified: Tue Jan 10 21:03:47 2023, max compression
+gzip compressed data, was "pycpep-1.1.1.tar", last modified: Mon Apr 17 13:39:12 2023, max compression
```

## Comparing `pycpep-1.0.5.tar` & `pycpep-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-01-10 21:03:47.662380 pycpep-1.0.5/
--rw-r--r--   0 nirmal     (501) staff       (20)      275 2023-01-10 21:03:47.661650 pycpep-1.0.5/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)     3289 2023-01-10 21:01:27.000000 pycpep-1.0.5/README.md
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-01-10 21:03:47.643006 pycpep-1.0.5/pycpep/
--rw-r--r--   0 nirmal     (501) staff       (20)       23 2023-01-08 19:04:25.000000 pycpep-1.0.5/pycpep/__init__.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-01-10 21:03:47.658559 pycpep-1.0.5/pycpep/mdl/
--rw-r--r--   0 nirmal     (501) staff       (20)    54392 2023-01-10 18:58:30.000000 pycpep-1.0.5/pycpep/mdl/model.h5
--rw-r--r--   0 nirmal     (501) staff       (20)    54392 2023-01-10 18:58:30.000000 pycpep-1.0.5/pycpep/mdl/model.hdf5
--rw-r--r--   0 nirmal     (501) staff       (20)      630 2023-01-07 16:18:03.000000 pycpep-1.0.5/pycpep/mdl/scaler.pkl
--rw-r--r--   0 nirmal     (501) staff       (20)     5805 2023-01-10 21:01:55.000000 pycpep-1.0.5/pycpep/pycpep.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-01-10 21:03:47.648219 pycpep-1.0.5/pycpep.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)      275 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      296 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       58 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        7 2023-01-10 21:03:47.000000 pycpep-1.0.5/pycpep.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-01-10 21:03:47.662836 pycpep-1.0.5/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      653 2023-01-10 21:02:18.000000 pycpep-1.0.5/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-17 13:39:12.258272 pycpep-1.1.1/
+-rw-r--r--   0 nirmal     (501) staff       (20)      193 2023-04-16 16:16:58.000000 pycpep-1.1.1/LICENSE.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)      301 2023-04-17 13:39:12.258152 pycpep-1.1.1/PKG-INFO
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-17 13:39:12.255410 pycpep-1.1.1/PyCpep/
+-rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-17 12:31:32.000000 pycpep-1.1.1/PyCpep/__init__.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-17 13:39:12.257570 pycpep-1.1.1/PyCpep/mdl/
+-rw-r--r--   0 nirmal     (501) staff       (20)    54392 2023-04-16 16:16:58.000000 pycpep-1.1.1/PyCpep/mdl/model.h5
+-rw-r--r--   0 nirmal     (501) staff       (20)    54392 2023-04-16 16:16:58.000000 pycpep-1.1.1/PyCpep/mdl/model.hdf5
+-rw-r--r--   0 nirmal     (501) staff       (20)      630 2023-04-16 16:16:58.000000 pycpep-1.1.1/PyCpep/mdl/scaler.pkl
+-rw-r--r--   0 nirmal     (501) staff       (20)     5994 2023-04-17 13:03:48.000000 pycpep-1.1.1/PyCpep/pycpep.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-17 13:39:12.256454 pycpep-1.1.1/PyCpep.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)      301 2023-04-17 13:39:12.000000 pycpep-1.1.1/PyCpep.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      486 2023-04-17 13:39:12.000000 pycpep-1.1.1/PyCpep.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-17 13:39:12.000000 pycpep-1.1.1/PyCpep.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-16 20:50:56.000000 pycpep-1.1.1/PyCpep.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       52 2023-04-17 13:39:12.000000 pycpep-1.1.1/PyCpep.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        7 2023-04-17 13:39:12.000000 pycpep-1.1.1/PyCpep.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)     2039 2023-04-17 13:08:56.000000 pycpep-1.1.1/README.md
+-rw-r--r--   0 nirmal     (501) staff       (20)       38 2023-04-17 13:39:12.258312 pycpep-1.1.1/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      645 2023-04-17 13:38:53.000000 pycpep-1.1.1/setup.py
```

### Comparing `pycpep-1.0.5/pycpep/mdl/model.h5` & `pycpep-1.1.1/PyCpep/mdl/model.h5`

 * *Files identical despite different names*

### Comparing `pycpep-1.0.5/pycpep/mdl/model.hdf5` & `pycpep-1.1.1/PyCpep/mdl/model.hdf5`

 * *Files identical despite different names*

### Comparing `pycpep-1.0.5/pycpep/mdl/scaler.pkl` & `pycpep-1.1.1/PyCpep/mdl/scaler.pkl`

 * *Files identical despite different names*

### Comparing `pycpep-1.0.5/setup.py` & `pycpep-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(name='pycpep',
-        version='1.0.5',
+        version='1.1.1',
         license='MIT',
         url='https://github.com/nirmalparmarphd/PyCpep',
         description='Predicts deviation in the heat capacity measurement for microDSC Tian-Calvet', 
-        long_description=('README.md'),
+        long_description='README.md',
         author='Nirmal Parmar',
         author_email='nirmalparmarphd@gmail.com',
         packages=setuptools.find_packages(),
         include_package_data=True,
         package_data={'': ['mdl/*.h5', 'mdl/*.pkl','mdl/*.hdf5']},
-        install_requires=['scikit-learn','tensorflow','numpy', 'h5py','keras', 'gitpython', 'pandas'],
+        install_requires=['scikit-learn','numpy', 'h5py','keras', 'gitpython', 'pandas','h5py'],
         zip_safe=False)
```

