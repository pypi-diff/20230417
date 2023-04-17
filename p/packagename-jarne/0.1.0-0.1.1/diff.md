# Comparing `tmp/packagename_jarne-0.1.0.tar.gz` & `tmp/packagename_jarne-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagename_jarne-0.1.0.tar", last modified: Mon Apr 17 08:24:52 2023, max compression
+gzip compressed data, was "packagename_jarne-0.1.1.tar", last modified: Mon Apr 17 08:48:34 2023, max compression
```

## Comparing `packagename_jarne-0.1.0.tar` & `packagename_jarne-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxr-x   0 eragon    (1000) eragon    (1000)        0 2023-04-17 08:24:52.404591 packagename_jarne-0.1.0/
--rw-rw-r--   0 eragon    (1000) eragon    (1000)     1419 2023-04-17 08:24:52.404591 packagename_jarne-0.1.0/PKG-INFO
--rwxr--r--   0 eragon    (1000) eragon    (1000)      744 2023-04-17 08:02:35.000000 packagename_jarne-0.1.0/README.md
-drwxrwxr-x   0 eragon    (1000) eragon    (1000)        0 2023-04-17 08:24:52.404591 packagename_jarne-0.1.0/packagename_jarne.egg-info/
--rw-rw-r--   0 eragon    (1000) eragon    (1000)     1419 2023-04-17 08:24:52.000000 packagename_jarne-0.1.0/packagename_jarne.egg-info/PKG-INFO
--rw-rw-r--   0 eragon    (1000) eragon    (1000)      237 2023-04-17 08:24:52.000000 packagename_jarne-0.1.0/packagename_jarne.egg-info/SOURCES.txt
--rw-rw-r--   0 eragon    (1000) eragon    (1000)        1 2023-04-17 08:24:52.000000 packagename_jarne-0.1.0/packagename_jarne.egg-info/dependency_links.txt
--rw-rw-r--   0 eragon    (1000) eragon    (1000)       85 2023-04-17 08:24:52.000000 packagename_jarne-0.1.0/packagename_jarne.egg-info/requires.txt
--rw-rw-r--   0 eragon    (1000) eragon    (1000)       30 2023-04-17 08:24:52.000000 packagename_jarne-0.1.0/packagename_jarne.egg-info/top_level.txt
--rw-rw-r--   0 eragon    (1000) eragon    (1000)       86 2023-04-17 07:52:35.000000 packagename_jarne-0.1.0/pyproject.toml
--rw-rw-r--   0 eragon    (1000) eragon    (1000)       38 2023-04-17 08:24:52.404591 packagename_jarne-0.1.0/setup.cfg
--rwxr-xr-x   0 eragon    (1000) eragon    (1000)     3591 2023-04-17 08:21:29.000000 packagename_jarne-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-17 08:45:42.000000 packagename_jarne-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/packagename_jarne.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 08:48:33.000000 packagename_jarne-0.1.1/packagename_jarne.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:48:34.012822 packagename_jarne-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-17 08:45:42.000000 packagename_jarne-0.1.1/setup.py
```

### Comparing `packagename_jarne-0.1.0/PKG-INFO` & `packagename_jarne-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagename_jarne
-Version: 0.1.0
+Version: 0.1.1
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -15,37 +15,41 @@
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 
 # Python-sphinx-documentation
 
-Template to document code with sphinx
+Template to document code with sphinx.
+install package ```pip install packagename_jarne```
 
 ## Create documentation
 
 1. Update files to fit the new package
 
-- Change ```packagename_jarne``` to the new packagename_jarne
-- Change version in ```packagename_jarne/version``` and ```setup.py```
+- Change ```packagename_jarne``` to the new packagename
+- Change version in ```packagename_jarne/version```
 - Update ```setup.py```
 - Update sources for Sphinx
   - ```docs/source/conf.py```
   - rst files
 
 
-2. Install package with conda
+1. Install package with conda
 
 ```conda env create -f environment.yml```
 
-3. Make documentation
+2. Make documentation
 
-- ```cd docs```
+- ```conda env create -f environment_build.yml; conda activate conda-env-name-build;cd docs;make html;cd ..```
 - ```make html```
   - alternatives ```make help```
 
 ## Add new python files
 
 1. Add files in package folder ```packagename_jarne``` (or the new name)
 2. Add links to the python files in ```docs/source/```
 3. Make [Documentation](#create-documentation) (see above)
 
+## Upload to pipy requirements
+
+- add ```PYPI_TOKEN``` to github secrets
```

### Comparing `packagename_jarne-0.1.0/README.md` & `packagename_jarne-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # Python-sphinx-documentation
 
-Template to document code with sphinx
+Template to document code with sphinx.
+install package ```pip install packagename_jarne```
 
 ## Create documentation
 
 1. Update files to fit the new package
 
-- Change ```packagename_jarne``` to the new packagename_jarne
-- Change version in ```packagename_jarne/version``` and ```setup.py```
+- Change ```packagename_jarne``` to the new packagename
+- Change version in ```packagename_jarne/version```
 - Update ```setup.py```
 - Update sources for Sphinx
   - ```docs/source/conf.py```
   - rst files
 
 
-2. Install package with conda
+1. Install package with conda
 
 ```conda env create -f environment.yml```
 
-3. Make documentation
+2. Make documentation
 
-- ```cd docs```
+- ```conda env create -f environment_build.yml; conda activate conda-env-name-build;cd docs;make html;cd ..```
 - ```make html```
   - alternatives ```make help```
 
 ## Add new python files
 
 1. Add files in package folder ```packagename_jarne``` (or the new name)
 2. Add links to the python files in ```docs/source/```
 3. Make [Documentation](#create-documentation) (see above)
 
+## Upload to pipy requirements
+
+- add ```PYPI_TOKEN``` to github secrets
```

### Comparing `packagename_jarne-0.1.0/packagename_jarne.egg-info/PKG-INFO` & `packagename_jarne-0.1.1/packagename_jarne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagename-jarne
-Version: 0.1.0
+Version: 0.1.1
 Summary: Example project for sphinx python.
 Home-page: https://github.com/jarneamerlinck/python-sphinx-documentation
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -15,37 +15,41 @@
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 
 # Python-sphinx-documentation
 
-Template to document code with sphinx
+Template to document code with sphinx.
+install package ```pip install packagename_jarne```
 
 ## Create documentation
 
 1. Update files to fit the new package
 
-- Change ```packagename_jarne``` to the new packagename_jarne
-- Change version in ```packagename_jarne/version``` and ```setup.py```
+- Change ```packagename_jarne``` to the new packagename
+- Change version in ```packagename_jarne/version```
 - Update ```setup.py```
 - Update sources for Sphinx
   - ```docs/source/conf.py```
   - rst files
 
 
-2. Install package with conda
+1. Install package with conda
 
 ```conda env create -f environment.yml```
 
-3. Make documentation
+2. Make documentation
 
-- ```cd docs```
+- ```conda env create -f environment_build.yml; conda activate conda-env-name-build;cd docs;make html;cd ..```
 - ```make html```
   - alternatives ```make help```
 
 ## Add new python files
 
 1. Add files in package folder ```packagename_jarne``` (or the new name)
 2. Add links to the python files in ```docs/source/```
 3. Make [Documentation](#create-documentation) (see above)
 
+## Upload to pipy requirements
+
+- add ```PYPI_TOKEN``` to github secrets
```

### Comparing `packagename_jarne-0.1.0/setup.py` & `packagename_jarne-0.1.1/setup.py`

 * *Files identical despite different names*

