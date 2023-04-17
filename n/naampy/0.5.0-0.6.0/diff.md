# Comparing `tmp/naampy-0.5.0.tar.gz` & `tmp/naampy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naampy-0.5.0.tar", last modified: Mon Sep 19 16:01:38 2022, max compression
+gzip compressed data, was "naampy-0.6.0.tar", last modified: Mon Apr 17 17:06:09 2023, max compression
```

## Comparing `naampy-0.5.0.tar` & `naampy-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.576713 naampy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-19 16:01:23.000000 naampy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-19 16:01:23.000000 naampy-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13245 2022-09-19 16:01:38.576713 naampy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12455 2022-09-19 16:01:23.000000 naampy-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.568713 naampy-0.5.0/naampy/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8980 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/in_rolls_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.568713 naampy-0.5.0/naampy/model/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.572713 naampy-0.5.0/naampy/model/naampy_rmse/
--rw-r--r--   0 runner    (1001) docker     (121)    26485 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/model/naampy_rmse/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (121)   190672 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/model/naampy_rmse/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.572713 naampy-0.5.0/naampy/model/naampy_rmse/variables/
--rw-r--r--   0 runner    (1001) docker     (121)  2084065 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/model/naampy_rmse/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/model/naampy_rmse/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.576713 naampy-0.5.0/naampy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/tests/test_010_in_rolls_ln.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/tests/test_020_in_rolls_ln.py
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-09-19 16:01:23.000000 naampy-0.5.0/naampy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 16:01:38.568713 naampy-0.5.0/naampy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13245 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-19 16:01:38.000000 naampy-0.5.0/naampy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-19 16:01:38.576713 naampy-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-09-19 16:01:23.000000 naampy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.148146 naampy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-17 17:05:57.000000 naampy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 17:05:57.000000 naampy-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-17 17:06:09.148146 naampy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-17 17:05:57.000000 naampy-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.144146 naampy-0.6.0/naampy/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/in_rolls_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.144146 naampy-0.6.0/naampy/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.148146 naampy-0.6.0/naampy/model/naampy_rmse/
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/model/naampy_rmse/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (123)   190672 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/model/naampy_rmse/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.148146 naampy-0.6.0/naampy/model/naampy_rmse/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  2084065 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/model/naampy_rmse/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/model/naampy_rmse/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.148146 naampy-0.6.0/naampy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/tests/test_010_in_rolls_ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/tests/test_020_in_rolls_ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-17 17:05:57.000000 naampy-0.6.0/naampy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:06:09.148146 naampy-0.6.0/naampy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:06:09.000000 naampy-0.6.0/naampy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 17:06:09.148146 naampy-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-17 17:05:57.000000 naampy-0.6.0/setup.py
```

### Comparing `naampy-0.5.0/LICENSE` & `naampy-0.6.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2018 Gaurav Sood and Atul Dhingra
+Copyright (c) 2023 Rajashekar Chintalapati, Suriyam Laohaprapanon, and Gaurav Sood
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `naampy-0.5.0/PKG-INFO` & `naampy-0.6.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,25 @@
-Metadata-Version: 2.1
-Name: naampy
-Version: 0.5.0
-Summary: Infer Gender from Indian Names
-Home-page: https://github.com/appeler/naampy
-Author: Gaurav Sood, Suriyan Laohaprapanon, Rajashekar Chintalapati
-Author-email: gsood07@gmail.com, suriyant@gmail.com, rajshekar.ch@gmail.com
-License: MIT
-Keywords: gender names
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 naampy: Infer Sociodemographic Characteristics from Indian Names
 ----------------------------------------------------------------
 
-.. image:: https://travis-ci.org/appeler/naampy.svg?branch=master
-    :target: https://travis-ci.org/appeler/naampy
-.. image:: https://ci.appveyor.com/api/projects/status/q4wr4clilf4samlk?svg=true
-    :target: https://ci.appveyor.com/project/soodoku/naampy
+.. image:: https://github.com/appeler/naampy/workflows/test/badge.svg
+    :target: https://github.com/appeler/naampy/actions/workflows/test.yml
 .. image:: https://img.shields.io/pypi/v/naampy.svg
     :target: https://pypi.python.org/pypi/naampy
+.. image:: https://readthedocs.org/projects/naampy/badge/?version=latest
+    :target: http://naampy.readthedocs.io/en/latest/?badge=latest
 .. image:: https://pepy.tech/badge/naampy
     :target: https://pepy.tech/project/naampy
 
-
 The ability to programmatically reliably infer the social attributes of a person from their name can be useful for a broad set of tasks, from estimating bias in coverage of women in the media to estimating bias in lending against certain social groups. But unlike the American Census Bureau, which produces a list of last names and first names, which can (and are) used to infer the gender, race, ethnicity, etc., from names, the Indian government produces no such commensurate datasets. And hence inferring the relationship between gender, ethnicity, language group, etc., and names have generally been done with small datasets constructed in an ad-hoc manner.
 
 We fill this yawning gap. Using data from the `Indian Electoral Rolls <https://github.com/in-rolls/electoral_rolls>`__ (parsed data `here <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/MUEGDT>`__), we estimate the proportion female, male, and `third sex` (see `here <https://en.wikipedia.org/wiki/Third_gender>`__) for a particular `first name, year, and state.`
 
+Please also check out `pranaam <https://github.com/appeler/pranaam>`__ that uses land record data from Bihar to infer religion based on the name. The package uses `indicate <https://github.com/in-rolls/indicate>`__ to transliterate Hindi to English.
+
 Data
 ~~~~
 
 In all, we capitalize on information in the parsed electoral rolls from the following 31 states and union territories: 
 
 .. list-table:: States
    :widths: 30 30 30 30
@@ -97,15 +77,15 @@
 * Voting registration lists are, at best, a census of adult citizens. But to the extent there is prejudice against women, etc., that prevents them from reaching adulthood, the data bakes those biases in.
 
 * Indian names are complicated. We do not have good parsers for them yet. We have gone for the default arrangement. Please go through the notebook to look at the judgments we make. We plan to improve the underlying data over time.
 
 * For state electoral rolls that are neither in English and Hindi, we use libindic. The quality of transliterations is consistently bad.
 
 Gender Classifier
-~~~~~~~~~~~~~~~~~
+==============================
 
 We start by providing a base model for first\_name that gives the Bayes
 optimal solution---the proportion of people with that name who
 are women. We also provide a series of base models where the state of
 residence and year of birth is known.
 
 If the name does not exist in the database, we use `ML model <https://github.com/appeler/naampy/blob/master/naampy/data/ml_model/02_training_model.ipynb>`__ that uses the relationship between
@@ -135,25 +115,25 @@
 Below are the inference results using different models.
 
 .. figure:: images/infer_oos.png
    :alt: Inference on different models
    :align: center
 
 Installation
-~~~~~~~~~~~~~~
+==============================
 
 We strongly recommend installing `naampy` inside a Python virtual environment (see `venv documentation <https://docs.python.org/3/library/venv.html#creating-virtual-environments>`__)
 
 ::
 
     pip install naampy
 
 
 Usage
-~~~~~
+==============================
 
 ::
 
     usage: in_rolls_fn_gender [-h] -f FIRST_NAME
                             [-s {andaman,andhra,arunachal,assam,bihar,chandigarh,dadra,daman,delhi,goa,gujarat,haryana,himachal,jharkhand,jk,karnataka,kerala,maharashtra,manipur,meghalaya,mizoram,mp,nagaland,odisha,puducherry,punjab,rajasthan,sikkim,tripura,up,uttarakhand}]
                             [-y YEAR] [-o OUTPUT]
                             input
@@ -178,15 +158,15 @@
     -o OUTPUT, --output OUTPUT
                             Output file with Indian electoral rolls data columns
 
         choices=["v1", "v2", "v2_1k", "v2_native", "v2_en"],
 
 
 Using naampy
-~~~~~~~~~~~~
+==============================
 
 ::
 
     >>> import pandas as pd
     >>> from naampy import in_rolls_fn_gender
 
     >>> names = [{'name': 'gaurav'},
@@ -294,22 +274,22 @@
     23         rajkummar        male   0.845139
     24           sharman        male   0.858538
     25         ayushmann        male   0.964895
     26            irrfan        male   0.837053
     27           riteish        male   0.950755
 
 Functionality
-~~~~~~~~~~~~~
+==============================
 
 When you first run `in_rolls_fn_gender`, it downloads data from `Harvard Dataverse <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/WZGJBM>`__ to the local folder. Next time you run the function, it searches for local data and if it finds it, it uses it.
 Use `predict_fn_gender` to get gender predictions based on first name.
 
 Authors
-~~~~~~~
+==============================
 
 Suriyan Laohaprapanon, Gaurav Sood, and Rajashekar Chintalapati
 
 License
-~~~~~~~
+==============================
 
 The package is released under the `MIT
 License <https://opensource.org/licenses/MIT>`__.
```

### Comparing `naampy-0.5.0/README.rst` & `naampy-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,48 @@
+Metadata-Version: 2.1
+Name: naampy
+Version: 0.6.0
+Summary: Infer Gender from Indian Names
+Home-page: https://github.com/appeler/naampy
+Author: Gaurav Sood, Suriyan Laohaprapanon, Rajashekar Chintalapati
+Author-email: gsood07@gmail.com, suriyant@gmail.com, rajshekar.ch@gmail.com
+License: MIT
+Keywords: gender names
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
 naampy: Infer Sociodemographic Characteristics from Indian Names
 ----------------------------------------------------------------
 
-.. image:: https://travis-ci.org/appeler/naampy.svg?branch=master
-    :target: https://travis-ci.org/appeler/naampy
-.. image:: https://ci.appveyor.com/api/projects/status/q4wr4clilf4samlk?svg=true
-    :target: https://ci.appveyor.com/project/soodoku/naampy
+.. image:: https://github.com/appeler/naampy/workflows/test/badge.svg
+    :target: https://github.com/appeler/naampy/actions/workflows/test.yml
 .. image:: https://img.shields.io/pypi/v/naampy.svg
     :target: https://pypi.python.org/pypi/naampy
+.. image:: https://readthedocs.org/projects/naampy/badge/?version=latest
+    :target: http://naampy.readthedocs.io/en/latest/?badge=latest
 .. image:: https://pepy.tech/badge/naampy
     :target: https://pepy.tech/project/naampy
 
-
 The ability to programmatically reliably infer the social attributes of a person from their name can be useful for a broad set of tasks, from estimating bias in coverage of women in the media to estimating bias in lending against certain social groups. But unlike the American Census Bureau, which produces a list of last names and first names, which can (and are) used to infer the gender, race, ethnicity, etc., from names, the Indian government produces no such commensurate datasets. And hence inferring the relationship between gender, ethnicity, language group, etc., and names have generally been done with small datasets constructed in an ad-hoc manner.
 
 We fill this yawning gap. Using data from the `Indian Electoral Rolls <https://github.com/in-rolls/electoral_rolls>`__ (parsed data `here <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/MUEGDT>`__), we estimate the proportion female, male, and `third sex` (see `here <https://en.wikipedia.org/wiki/Third_gender>`__) for a particular `first name, year, and state.`
 
+Please also check out `pranaam <https://github.com/appeler/pranaam>`__ that uses land record data from Bihar to infer religion based on the name. The package uses `indicate <https://github.com/in-rolls/indicate>`__ to transliterate Hindi to English.
+
 Data
 ~~~~
 
 In all, we capitalize on information in the parsed electoral rolls from the following 31 states and union territories: 
 
 .. list-table:: States
    :widths: 30 30 30 30
@@ -76,15 +100,15 @@
 * Voting registration lists are, at best, a census of adult citizens. But to the extent there is prejudice against women, etc., that prevents them from reaching adulthood, the data bakes those biases in.
 
 * Indian names are complicated. We do not have good parsers for them yet. We have gone for the default arrangement. Please go through the notebook to look at the judgments we make. We plan to improve the underlying data over time.
 
 * For state electoral rolls that are neither in English and Hindi, we use libindic. The quality of transliterations is consistently bad.
 
 Gender Classifier
-~~~~~~~~~~~~~~~~~
+==============================
 
 We start by providing a base model for first\_name that gives the Bayes
 optimal solution---the proportion of people with that name who
 are women. We also provide a series of base models where the state of
 residence and year of birth is known.
 
 If the name does not exist in the database, we use `ML model <https://github.com/appeler/naampy/blob/master/naampy/data/ml_model/02_training_model.ipynb>`__ that uses the relationship between
@@ -114,25 +138,25 @@
 Below are the inference results using different models.
 
 .. figure:: images/infer_oos.png
    :alt: Inference on different models
    :align: center
 
 Installation
-~~~~~~~~~~~~~~
+==============================
 
 We strongly recommend installing `naampy` inside a Python virtual environment (see `venv documentation <https://docs.python.org/3/library/venv.html#creating-virtual-environments>`__)
 
 ::
 
     pip install naampy
 
 
 Usage
-~~~~~
+==============================
 
 ::
 
     usage: in_rolls_fn_gender [-h] -f FIRST_NAME
                             [-s {andaman,andhra,arunachal,assam,bihar,chandigarh,dadra,daman,delhi,goa,gujarat,haryana,himachal,jharkhand,jk,karnataka,kerala,maharashtra,manipur,meghalaya,mizoram,mp,nagaland,odisha,puducherry,punjab,rajasthan,sikkim,tripura,up,uttarakhand}]
                             [-y YEAR] [-o OUTPUT]
                             input
@@ -157,15 +181,15 @@
     -o OUTPUT, --output OUTPUT
                             Output file with Indian electoral rolls data columns
 
         choices=["v1", "v2", "v2_1k", "v2_native", "v2_en"],
 
 
 Using naampy
-~~~~~~~~~~~~
+==============================
 
 ::
 
     >>> import pandas as pd
     >>> from naampy import in_rolls_fn_gender
 
     >>> names = [{'name': 'gaurav'},
@@ -273,22 +297,22 @@
     23         rajkummar        male   0.845139
     24           sharman        male   0.858538
     25         ayushmann        male   0.964895
     26            irrfan        male   0.837053
     27           riteish        male   0.950755
 
 Functionality
-~~~~~~~~~~~~~
+==============================
 
 When you first run `in_rolls_fn_gender`, it downloads data from `Harvard Dataverse <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/WZGJBM>`__ to the local folder. Next time you run the function, it searches for local data and if it finds it, it uses it.
 Use `predict_fn_gender` to get gender predictions based on first name.
 
 Authors
-~~~~~~~
+==============================
 
 Suriyan Laohaprapanon, Gaurav Sood, and Rajashekar Chintalapati
 
 License
-~~~~~~~
+==============================
 
 The package is released under the `MIT
 License <https://opensource.org/licenses/MIT>`__.
```

### Comparing `naampy-0.5.0/naampy/in_rolls_fn.py` & `naampy-0.6.0/naampy/in_rolls_fn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,75 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+from __future__ import annotations
 import sys
 import os
 import argparse
 import pandas as pd
 import tensorflow as tf
-from keras.preprocessing.text import Tokenizer
-from keras.preprocessing.sequence import pad_sequences
+import numpy as np
+from typing import Optional
+from tensorflow.keras.preprocessing.text import Tokenizer
+from tensorflow.keras.preprocessing.sequence import pad_sequences
 
 from pkg_resources import resource_filename
 
-from .utils import column_exists, fixup_columns, get_app_file_path, download_file
+from .utils import get_app_file_path, download_file
 
 
 IN_ROLLS_DATA = {
     "v1": "https://dataverse.harvard.edu/api/v1/access/datafile/4967581",
     "v2": "https://dataverse.harvard.edu/api/v1/access/datafile/4965696",
     "v2_1k": "https://dataverse.harvard.edu/api/v1/access/datafile/4965695",
     "v2_native": "https://dataverse.harvard.edu/api/v1/access/datafile/6292042",
     "v2_en": "https://dataverse.harvard.edu/api/v1/access/datafile/6457224",
 }
 
 IN_ROLLS_COLS = ["n_male", "n_female", "n_third_gender", "prop_female", "prop_male", "prop_third_gender"]
 
 
 class InRollsFnData:
+    """
+    InRollsFnData class.
+    """
     __df = None
     __state = None
     __year = None
     __model = None
     __tk = None
     __dataset = None
 
     @staticmethod
-    def load_naampy_data(dataset):
-        data_fn = "naampy_{0:s}.csv.gz".format(dataset)
+    def load_naampy_data(dataset: str) -> str:
+        """
+
+        Args:
+            dataset (str): version of the dataset
+        Returns:
+            path to the data
+        """
+        data_fn = f"naampy_{dataset}.csv.gz"
         data_path = get_app_file_path("naampy", data_fn)
         if not os.path.exists(data_path):
-            print("Downloading naampy data from the server ({0!s})...".format(data_fn))
+            print(f"Downloading naampy data from the server ({data_fn})...")
             if not download_file(IN_ROLLS_DATA[dataset], data_path):
-                print("ERROR: Cannot download naampy data file")
-                return None
+                raise Exception("ERROR: Cannot download naampy data file")
         else:
-            print("Using cached naampy data from local ({0!s})...".format(data_path))
+            print(f"Using cached naampy data from local ({data_path})...")
         return data_path
 
     @classmethod
-    def predict_fn_gender(cls, input):
+    def predict_fn_gender(cls, first_names: list[str]) -> pd.DataFrame:
         """
         Predict gender based on name
         Args:
-            input (list of str): list of first name
+            first_names (list of str): list of first name
         Returns:
-            DataFrame: Pandas DataFrame with prediction and its probability
+            DataFrame: Pandas DataFrame with predicted labels and probability
         """
         # load model
         if cls.__model is None:
             model_fn = resource_filename(__name__, "model")
             cls.__model = tf.keras.models.load_model(f"{model_fn}/naampy_rmse")
         # create tokenizer
         if cls.__tk is None:
@@ -67,62 +79,54 @@
             for i, char in enumerate(alphabet):
                 char_dict[char] = i + 1
             # Use char_dict to replace the tk.word_index
             cls.__tk.word_index = char_dict.copy()
             # Add 'UNK' to the vocabulary
             cls.__tk.word_index[cls.__tk.oov_token] = max(char_dict.values()) + 1
 
-        input = [i.lower() for i in input]
-        sequences = cls.__tk.texts_to_sequences(input)
+        first_names = [i.lower() for i in first_names]
+        sequences = cls.__tk.texts_to_sequences(first_names)
         tokens = pad_sequences(sequences, maxlen=24, padding="post")
 
         results = cls.__model.predict(tokens)
-        gender = []
-        score = []
-        for i in range(len(input)):
-            pred = results[i].item()
-            if pred > 0.5:
-                gender.append("female")
-                score.append(pred)
-            else:
-                gender.append("male")
-                score.append(1 - pred)
-        return pd.DataFrame(data={"name": input, "pred_gender": gender, "pred_prob": score})
+        gender = np.where(results > 0.5, "female", "male")[:, 0]
+        score = np.where(results > 0.5, results, 1 - results)[:, 0]
+
+        return pd.DataFrame(data={"name": first_names, "pred_gender": gender, "pred_prob": score})
 
     @classmethod
-    def in_rolls_fn_gender(cls, df, namecol, state=None, year=None, dataset="v2_1k"):
-        """Appends additional columns from Female ratio data to the input DataFrame
+    def in_rolls_fn_gender(cls, df: pd.DataFrame, namecol: str, state: Optional[str]=None, year: Optional[int]=None, dataset: str="v2_1k") -> pd.DataFrame:
+        """
+        Appends additional columns from Female ratio data to the input DataFrame
         based on the first name.
 
         Removes extra space. Checks if the name is the Indian electoral rolls data.
         If it is, outputs data from that row.
 
         Args:
             df (:obj:`DataFrame`): Pandas DataFrame containing the first name
                 column.
-            namecol (str or int): Column's name or location of the name in
-                DataFrame.
-            state (str): The state name of Indian electoral rolls data to be used.
+            namecol (str): Columnn name containing the first name.
+            state (str or None): The state from which Indian electoral rolls data to be used.
                 (default is None for all states)
-            year (int): The year of Indian electoral rolls to be used.
+            year (int or None): The year of Indian electoral rolls to be used.
                 (default is None for all years)
 
         Returns:
             DataFrame: Pandas DataFrame with additional columns:-
                 'n_female', 'n_male', 'n_third_gender',
                 'prop_female', 'prop_male', 'prop_third_gender' by first name
 
         """
 
-        if namecol not in df.columns:
-            print("No column `{0!s}` in the DataFrame".format(namecol))
+        if namecol and namecol not in df.columns:
+            print(f"No column `{namecol}` in the DataFrame")
             return df
 
-        df["__first_name"] = df[namecol].str.strip()
-        df["__first_name"] = df["__first_name"].str.lower()
+        df["__first_name"] = df[namecol].str.strip().str.lower()
 
         if cls.__df is None or cls.__state != state or cls.__year != year or cls.__dataset != dataset:
             cls.__dataset = dataset
             data_path = InRollsFnData.load_naampy_data(dataset)
             adf = pd.read_csv(
                 data_path, usecols=["state", "birth_year", "first_name", "n_female", "n_male", "n_third_gender"]
             )
@@ -159,30 +163,40 @@
                 rdf.at[not_in_db_names.index, "pred_prob"] = mdf["pred_prob"].values
 
         del rdf["__first_name"]
 
         return rdf
 
     @staticmethod
-    def list_states(dataset="v2_1k"):
+    def list_states(dataset: str="v2_1k") -> np.ndarray:
+        """
+
+        Args:
+            dataset (str): version of the dataset
+        Returns:
+            list of states
+        """
         data_path = InRollsFnData.load_naampy_data(dataset)
         adf = pd.read_csv(data_path, usecols=["state"])
         return adf.state.unique()
 
 
 in_rolls_fn_gender = InRollsFnData.in_rolls_fn_gender
 predict_fn_gender = InRollsFnData.predict_fn_gender
 
 
 def main(argv=sys.argv[1:]):
-    title = "Appends Electoral roll columns for prop_female, n_female, " "n_male n_third_gender by first name"
+    """
+    Main method for shell support
+    """
+    title = "Appends Electoral roll columns prop_female, n_female, n_male n_third_gender"
     parser = argparse.ArgumentParser(description=title)
     parser.add_argument("input", default=None, help="Input file")
     parser.add_argument(
-        "-f", "--first-name", required=True, help="Name or index location of column contains " "the first name"
+        "-f", "--first-name", required=True, help="Name of column containing the first name"
     )
     parser.add_argument(
         "-s",
         "--state",
         default=None,
         choices=InRollsFnData.list_states(),
         help="State name of Indian electoral rolls data " "(default=all)",
@@ -194,40 +208,35 @@
         "-o", "--output", default="in-rolls-output.csv", help="Output file with Indian electoral rolls data columns"
     )
     parser.add_argument(
         "-d",
         "--dataset",
         default="v2_1k",
         choices=["v1", "v2", "v2_1k", "v2_native", "v2_en"],
-        help="Select the dataset v1 is 12 states,"
+        help="Select the dataset. v1 is 12 states,"
         + " v2 and v2_1k for 30 states with 100 and 1,000"
         + " first name occurrences respectively"
         + " v2_native is the native language dataset of"
         + " 16 states with 10 first name occurrences per state,"
         + " and v2_en is Hindi transliteration of v2_native dataset"
         + " (default=v2_1k)"
     )
 
     args = parser.parse_args(argv)
 
     print(args)
 
-    if not args.first_name.isdigit():
-        df = pd.read_csv(args.input)
-    else:
-        df = pd.read_csv(args.input, header=None)
-        args.first_name = int(args.first_name)
-
-    if not column_exists(df, args.first_name):
+    df = pd.read_csv(args.input)
+    
+    if args.first_name and (args.first_name not in df.columns):
+        print(f"Column `{args.first_name}` not found in the input file")
         return -1
 
     rdf = in_rolls_fn_gender(df, args.first_name, args.state, args.year, args.dataset)
 
-    print("Saving output to file: `{0:s}`".format(args.output))
-    rdf.columns = fixup_columns(rdf.columns)
+    print(f"Saving output to file: `{args.output}`")
     rdf.to_csv(args.output, index=False)
 
     return 0
 
-
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `naampy-0.5.0/naampy/model/naampy_rmse/keras_metadata.pb` & `naampy-0.6.0/naampy/model/naampy_rmse/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy/model/naampy_rmse/saved_model.pb` & `naampy-0.6.0/naampy/model/naampy_rmse/saved_model.pb`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy/model/naampy_rmse/variables/variables.data-00000-of-00001` & `naampy-0.6.0/naampy/model/naampy_rmse/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy/model/naampy_rmse/variables/variables.index` & `naampy-0.6.0/naampy/model/naampy_rmse/variables/variables.index`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy/tests/test_010_in_rolls_ln.py` & `naampy-0.6.0/naampy/tests/test_010_in_rolls_ln.py`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy/tests/test_020_in_rolls_ln.py` & `naampy-0.6.0/naampy/tests/test_020_in_rolls_ln.py`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/naampy.egg-info/PKG-INFO` & `naampy-0.6.0/naampy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: naampy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Infer Gender from Indian Names
 Home-page: https://github.com/appeler/naampy
 Author: Gaurav Sood, Suriyan Laohaprapanon, Rajashekar Chintalapati
 Author-email: gsood07@gmail.com, suriyant@gmail.com, rajshekar.ch@gmail.com
 License: MIT
 Keywords: gender names
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 naampy: Infer Sociodemographic Characteristics from Indian Names
 ----------------------------------------------------------------
 
-.. image:: https://travis-ci.org/appeler/naampy.svg?branch=master
-    :target: https://travis-ci.org/appeler/naampy
-.. image:: https://ci.appveyor.com/api/projects/status/q4wr4clilf4samlk?svg=true
-    :target: https://ci.appveyor.com/project/soodoku/naampy
+.. image:: https://github.com/appeler/naampy/workflows/test/badge.svg
+    :target: https://github.com/appeler/naampy/actions/workflows/test.yml
 .. image:: https://img.shields.io/pypi/v/naampy.svg
     :target: https://pypi.python.org/pypi/naampy
+.. image:: https://readthedocs.org/projects/naampy/badge/?version=latest
+    :target: http://naampy.readthedocs.io/en/latest/?badge=latest
 .. image:: https://pepy.tech/badge/naampy
     :target: https://pepy.tech/project/naampy
 
-
 The ability to programmatically reliably infer the social attributes of a person from their name can be useful for a broad set of tasks, from estimating bias in coverage of women in the media to estimating bias in lending against certain social groups. But unlike the American Census Bureau, which produces a list of last names and first names, which can (and are) used to infer the gender, race, ethnicity, etc., from names, the Indian government produces no such commensurate datasets. And hence inferring the relationship between gender, ethnicity, language group, etc., and names have generally been done with small datasets constructed in an ad-hoc manner.
 
 We fill this yawning gap. Using data from the `Indian Electoral Rolls <https://github.com/in-rolls/electoral_rolls>`__ (parsed data `here <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/MUEGDT>`__), we estimate the proportion female, male, and `third sex` (see `here <https://en.wikipedia.org/wiki/Third_gender>`__) for a particular `first name, year, and state.`
 
+Please also check out `pranaam <https://github.com/appeler/pranaam>`__ that uses land record data from Bihar to infer religion based on the name. The package uses `indicate <https://github.com/in-rolls/indicate>`__ to transliterate Hindi to English.
+
 Data
 ~~~~
 
 In all, we capitalize on information in the parsed electoral rolls from the following 31 states and union territories: 
 
 .. list-table:: States
    :widths: 30 30 30 30
@@ -97,15 +100,15 @@
 * Voting registration lists are, at best, a census of adult citizens. But to the extent there is prejudice against women, etc., that prevents them from reaching adulthood, the data bakes those biases in.
 
 * Indian names are complicated. We do not have good parsers for them yet. We have gone for the default arrangement. Please go through the notebook to look at the judgments we make. We plan to improve the underlying data over time.
 
 * For state electoral rolls that are neither in English and Hindi, we use libindic. The quality of transliterations is consistently bad.
 
 Gender Classifier
-~~~~~~~~~~~~~~~~~
+==============================
 
 We start by providing a base model for first\_name that gives the Bayes
 optimal solution---the proportion of people with that name who
 are women. We also provide a series of base models where the state of
 residence and year of birth is known.
 
 If the name does not exist in the database, we use `ML model <https://github.com/appeler/naampy/blob/master/naampy/data/ml_model/02_training_model.ipynb>`__ that uses the relationship between
@@ -135,25 +138,25 @@
 Below are the inference results using different models.
 
 .. figure:: images/infer_oos.png
    :alt: Inference on different models
    :align: center
 
 Installation
-~~~~~~~~~~~~~~
+==============================
 
 We strongly recommend installing `naampy` inside a Python virtual environment (see `venv documentation <https://docs.python.org/3/library/venv.html#creating-virtual-environments>`__)
 
 ::
 
     pip install naampy
 
 
 Usage
-~~~~~
+==============================
 
 ::
 
     usage: in_rolls_fn_gender [-h] -f FIRST_NAME
                             [-s {andaman,andhra,arunachal,assam,bihar,chandigarh,dadra,daman,delhi,goa,gujarat,haryana,himachal,jharkhand,jk,karnataka,kerala,maharashtra,manipur,meghalaya,mizoram,mp,nagaland,odisha,puducherry,punjab,rajasthan,sikkim,tripura,up,uttarakhand}]
                             [-y YEAR] [-o OUTPUT]
                             input
@@ -178,15 +181,15 @@
     -o OUTPUT, --output OUTPUT
                             Output file with Indian electoral rolls data columns
 
         choices=["v1", "v2", "v2_1k", "v2_native", "v2_en"],
 
 
 Using naampy
-~~~~~~~~~~~~
+==============================
 
 ::
 
     >>> import pandas as pd
     >>> from naampy import in_rolls_fn_gender
 
     >>> names = [{'name': 'gaurav'},
@@ -294,22 +297,22 @@
     23         rajkummar        male   0.845139
     24           sharman        male   0.858538
     25         ayushmann        male   0.964895
     26            irrfan        male   0.837053
     27           riteish        male   0.950755
 
 Functionality
-~~~~~~~~~~~~~
+==============================
 
 When you first run `in_rolls_fn_gender`, it downloads data from `Harvard Dataverse <https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/WZGJBM>`__ to the local folder. Next time you run the function, it searches for local data and if it finds it, it uses it.
 Use `predict_fn_gender` to get gender predictions based on first name.
 
 Authors
-~~~~~~~
+==============================
 
 Suriyan Laohaprapanon, Gaurav Sood, and Rajashekar Chintalapati
 
 License
-~~~~~~~
+==============================
 
 The package is released under the `MIT
 License <https://opensource.org/licenses/MIT>`__.
```

### Comparing `naampy-0.5.0/naampy.egg-info/SOURCES.txt` & `naampy-0.6.0/naampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naampy-0.5.0/setup.py` & `naampy-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 setup(
     name="naampy",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.5.0",
+    version="0.6.0",
     description="Infer Gender from Indian Names",
     long_description=long_description,
     # The project's main homepage.
     url="https://github.com/appeler/naampy",
     # Author details
     author="Gaurav Sood, Suriyan Laohaprapanon, Rajashekar Chintalapati",
     author_email="gsood07@gmail.com, suriyant@gmail.com, rajshekar.ch@gmail.com",
@@ -86,14 +86,16 @@
         "Intended Audience :: Developers",
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
     # What does your project relate to?
     keywords="gender names",
     # You can just specify the packages manually here if your project is
```

