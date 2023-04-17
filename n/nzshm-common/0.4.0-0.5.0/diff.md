# Comparing `tmp/nzshm-common-0.4.0.tar.gz` & `tmp/nzshm_common-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzshm-common-0.4.0.tar", max compression
+gzip compressed data, was "nzshm_common-0.5.0.tar", max compression
```

## Comparing `nzshm-common-0.4.0.tar` & `nzshm_common-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0    34523 2022-09-27 00:13:05.000238 nzshm-common-0.4.0/LICENSE
--rw-r--r--   0        0        0      418 2022-09-27 00:13:05.000238 nzshm-common-0.4.0/README.md
--rw-r--r--   0        0        0      121 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/__init__.py
--rw-r--r--   0        0        0     1100 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/geometry/geometry.py
--rw-r--r--   0        0        0       47 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/__init__.py
--rw-r--r--   0        0        0      477 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/io.py
--rw-r--r--   0        0        0     2831 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/nz_0_1_nb_1_v0.py
--rw-r--r--   0        0        0     3524 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/nz_0_1_nb_1_v1.py
--rw-r--r--   0        0        0    47971 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/nz_0_2_nb_1_1.py
--rw-r--r--   0        0        0     1511 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/region_grid.py
--rw-r--r--   0        0        0    38248 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/wlg_0_01_nb_1_1.py
--rw-r--r--   0        0        0     3260 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/grids/wlg_0_05_nb_1_1.py
--rw-r--r--   0        0        0       41 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/location/__init__.py
--rw-r--r--   0        0        0     1411 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/location/code_location.py
--rw-r--r--   0        0        0     3630 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/location/location.py
--rw-r--r--   0        0        0       75 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/util/__init__.py
--rw-r--r--   0        0        0     1440 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/nzshm_common/util/compression.py
--rw-r--r--   0        0        0     2121 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3565 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/tests/test_coded_location.py
--rw-r--r--   0        0        0     2317 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/tests/test_compression.py
--rw-r--r--   0        0        0     4500 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/tests/test_geometry.py
--rw-r--r--   0        0        0      262 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/tests/test_location.py
--rw-r--r--   0        0        0     1018 2022-09-27 00:13:05.004238 nzshm-common-0.4.0/tests/test_region_grid.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 nzshm-common-0.4.0/setup.py
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 nzshm-common-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-17 04:07:36.289452 nzshm_common-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1109 2023-04-17 04:07:36.289452 nzshm_common-0.5.0/README.md
+-rw-r--r--   0        0        0      111 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/geometry/backarc_polygon.json
+-rw-r--r--   0        0        0     1489 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/geometry/geometry.py
+-rw-r--r--   0        0        0       47 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/io.py
+-rw-r--r--   0        0        0     2831 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v0.py
+-rw-r--r--   0        0        0     3524 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v1.py
+-rw-r--r--   0        0        0    47971 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/nz_0_2_nb_1_1.py
+-rw-r--r--   0        0        0     1511 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/region_grid.py
+-rw-r--r--   0        0        0    38248 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/wlg_0_01_nb_1_1.py
+-rw-r--r--   0        0        0     3260 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/grids/wlg_0_05_nb_1_1.py
+-rw-r--r--   0        0        0       41 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/code_location.py
+-rw-r--r--   0        0        0     1631 2023-04-17 04:07:36.293452 nzshm_common-0.5.0/nzshm_common/location/location.py
+-rw-r--r--   0        0        0  3218277 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/location/locations.json
+-rw-r--r--   0        0        0      252 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/location/nz_ids.json
+-rw-r--r--   0        0        0       75 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/util/__init__.py
+-rw-r--r--   0        0        0     1440 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/nzshm_common/util/compression.py
+-rw-r--r--   0        0        0     2049 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1760 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_backarc.py
+-rw-r--r--   0        0        0     3565 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_coded_location.py
+-rw-r--r--   0        0        0     2317 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_compression.py
+-rw-r--r--   0        0        0     4500 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_geometry.py
+-rw-r--r--   0        0        0     1662 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_location.py
+-rw-r--r--   0        0        0     1018 2023-04-17 04:07:36.301452 nzshm_common-0.5.0/tests/test_region_grid.py
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 nzshm_common-0.5.0/PKG-INFO
```

### Comparing `nzshm-common-0.4.0/LICENSE` & `nzshm_common-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/nz_0_1_nb_1_v0.py` & `nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v0.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/nz_0_1_nb_1_v1.py` & `nzshm_common-0.5.0/nzshm_common/grids/nz_0_1_nb_1_v1.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/nz_0_2_nb_1_1.py` & `nzshm_common-0.5.0/nzshm_common/grids/nz_0_2_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/region_grid.py` & `nzshm_common-0.5.0/nzshm_common/grids/region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/wlg_0_01_nb_1_1.py` & `nzshm_common-0.5.0/nzshm_common/grids/wlg_0_01_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/grids/wlg_0_05_nb_1_1.py` & `nzshm_common-0.5.0/nzshm_common/grids/wlg_0_05_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/location/code_location.py` & `nzshm_common-0.5.0/nzshm_common/location/code_location.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/nzshm_common/util/compression.py` & `nzshm_common-0.5.0/nzshm_common/util/compression.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/pyproject.toml` & `nzshm_common-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "nzshm-common"
-version = "0.4.0"
+version = "0.5.0"
 homepage = "https://github.com/GNS-Science/nzshm-common-py"
 description = "A small pure python library for shared NZ NSHM data like locations."
 authors = ["GNS Science <chrisbc@artisan.co.nz>"]
 readme = "README.md"
 license = "GNU Affero V3"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
 ]
 packages = [
 	{ include = "nzshm_common" },
 	{ include = "tests", format = "sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-geopandas = {version = "^0.11.1", optional = true, extras = ["geometry"]}
-Shapely = {version = "^1.8.3", optional = true, extras = ["geometry"]}
+geopandas = {version = "^0.12.2", optional = true}
 
 [tool.poetry.extras]
 
-geometry = ["geopandas", "Shapely"]
+geometry = ["geopandas"]
 
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
     "flake8",
@@ -45,23 +45,23 @@
 pytest = "^7.1.2"
 black = "^22.3.0"
 isort = "^5.10.1"
 flake8  = { version = "^3.9.2"}
 flake8-docstrings = { version = "^1.6.0", optional = true }
 mypy = {version = "^0.900"}
 pytest-cov  = { version = "^2.12.0"}
-tox = { version = "^3.20.1"}
+tox = "^4.2.8"
 virtualenv  = { version = "^20.2.2", optional = true}
 pip  = { version = "^20.3.1", optional = true}
 bump2version = "^1.0.1"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ['py38', 'py39']
+target-version = ['py310', 'py39']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `nzshm-common-0.4.0/tests/test_coded_location.py` & `nzshm_common-0.5.0/tests/test_coded_location.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/tests/test_compression.py` & `nzshm_common-0.5.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/tests/test_geometry.py` & `nzshm_common-0.5.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/tests/test_region_grid.py` & `nzshm_common-0.5.0/tests/test_region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm-common-0.4.0/PKG-INFO` & `nzshm_common-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzshm-common
-Version: 0.4.0
+Version: 0.5.0
 Summary: A small pure python library for shared NZ NSHM data like locations.
 Home-page: https://github.com/GNS-Science/nzshm-common-py
 License: GNU Affero V3
 Author: GNS Science
 Author-email: chrisbc@artisan.co.nz
 Requires-Python: >=3.8,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,32 +12,44 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: geometry
 Provides-Extra: test
-Requires-Dist: Shapely[geometry] (>=1.8.3,<2.0.0); extra == "geometry"
-Requires-Dist: geopandas[geometry] (>=0.11.1,<0.12.0); extra == "geometry"
+Requires-Dist: geopandas (>=0.12.2,<0.13.0) ; extra == "geometry"
 Description-Content-Type: text/markdown
 
 # nzshm-common
 
 A pure python library of shared objects used in nzshm projects
 
+[![pypi](https://img.shields.io/pypi/v/nzshm-common.svg)](https://pypi.org/project/nzshm-common/)
+[![python](https://img.shields.io/pypi/pyversions/nzshm-common.svg)](https://pypi.org/project/nzshm-common/)
+[![Build Status](https://github.com/GNS-Science/nzshm-common-py/actions/workflows/dev.yml/badge.svg)](https://github.com/GNS-Science/nzshm-common-py/actions/workflows/dev.yml)
+[![codecov](https://codecov.io/gh/GNS-Science/nzshm-common-py/branch/main/graphs/badge.svg)](https://codecov.io/github/GNS-Science/nzshm-common-py)
+
+
+* Documentation: <https://GNS-Science.github.io/nzshm-common-py>
+* GitHub: <https://github.com/GNS-Science/nzshm-common-py>
+* PyPI: <https://pypi.org/project/nzshm-common/>
+* Free software: GPL-3.0-only
+
 ## Installation
 
 ```
-pip install git+https://github.com/GNS-Science/nzshm-common-py>=1.0.0b
+pip install nzshm-common
 ```
 
 ## Use
 
 ```
 >>> from nzshm_common.location import location
 >>> dir(location)
```

