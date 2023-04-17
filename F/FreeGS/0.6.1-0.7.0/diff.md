# Comparing `tmp/FreeGS-0.6.1.tar.gz` & `tmp/FreeGS-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeGS-0.6.1.tar", last modified: Thu Feb 11 11:48:17 2021, max compression
+gzip compressed data, was "FreeGS-0.7.0.tar", last modified: Mon Apr 17 16:12:39 2023, max compression
```

## Comparing `FreeGS-0.6.1.tar` & `FreeGS-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 bd512     (1000) bd512     (1000)        0 2021-02-11 11:48:17.912994 FreeGS-0.6.1/
-drwxr-xr-x   0 bd512     (1000) bd512     (1000)        0 2021-02-11 11:48:17.906327 FreeGS-0.6.1/FreeGS.egg-info/
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8273 2021-02-11 11:48:17.000000 FreeGS-0.6.1/FreeGS.egg-info/PKG-INFO
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1027 2021-02-11 11:48:17.000000 FreeGS-0.6.1/FreeGS.egg-info/SOURCES.txt
--rw-r--r--   0 bd512     (1000) bd512     (1000)        1 2021-02-11 11:48:17.000000 FreeGS-0.6.1/FreeGS.egg-info/dependency_links.txt
--rw-r--r--   0 bd512     (1000) bd512     (1000)       52 2021-02-11 11:48:17.000000 FreeGS-0.6.1/FreeGS.egg-info/requires.txt
--rw-r--r--   0 bd512     (1000) bd512     (1000)        7 2021-02-11 11:48:17.000000 FreeGS-0.6.1/FreeGS.egg-info/top_level.txt
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8273 2021-02-11 11:48:17.912994 FreeGS-0.6.1/PKG-INFO
--rw-r--r--   0 bd512     (1000) bd512     (1000)     6133 2021-02-11 11:47:27.000000 FreeGS-0.6.1/README.md
-drwxr-xr-x   0 bd512     (1000) bd512     (1000)        0 2021-02-11 11:48:17.909660 FreeGS-0.6.1/freegs/
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1073 2021-02-11 11:47:27.000000 FreeGS-0.6.1/freegs/__init__.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    12250 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/_aeqdsk.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     3218 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/_divgeo.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     3023 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/_fileutils.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     7807 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/_geqdsk.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     6183 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/boundary.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8383 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/coil.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     7776 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/control.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    16611 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/critical.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)      287 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/divgeo.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8840 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/dump.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    27847 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/equilibrium.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     7103 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/fieldtracer.py
--rwxr-xr-x   0 bd512     (1000) bd512     (1000)    15345 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/geqdsk.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8512 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/gradshafranov.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    15015 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/jtor.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    58812 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/machine.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     8984 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/multi_coil.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)    11049 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/multigrid.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     6443 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/optimise.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     5144 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/optimiser.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     3999 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/picard.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     3390 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/plotting.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     5126 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/polygons.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     3818 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/quadrature.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     7126 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/shaped_coil.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     2963 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_aeqdsk.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     2758 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_critical.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1455 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_equilibrium.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)      685 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_fileutils.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)      996 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_geqdsk.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)      918 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_jtor.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1649 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/test_linearsolve.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1940 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_machine.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     2755 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_multi_coil.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1474 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_optimise.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     4036 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/test_optimiser.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1574 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/test_polygons.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1251 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_quadrature.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1306 2021-02-11 11:36:11.000000 FreeGS-0.6.1/freegs/test_readwrite.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1535 2021-01-29 16:14:39.000000 FreeGS-0.6.1/freegs/test_shaped_coil.py
--rw-r--r--   0 bd512     (1000) bd512     (1000)       38 2021-02-11 11:48:17.912994 FreeGS-0.6.1/setup.cfg
--rw-r--r--   0 bd512     (1000) bd512     (1000)     1191 2021-02-11 11:36:11.000000 FreeGS-0.6.1/setup.py
+drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.166091 FreeGS-0.7.0/
+drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.162091 FreeGS-0.7.0/FreeGS.egg-info/
+-rw-r--r--   0 peter     (1000) users      (100)     7552 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) users      (100)     1081 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) users      (100)        1 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) users      (100)       52 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) users      (100)        7 2023-04-17 16:12:39.000000 FreeGS-0.7.0/FreeGS.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) users      (100)     7651 2022-10-10 08:00:46.000000 FreeGS-0.7.0/LICENSE
+-rw-r--r--   0 peter     (1000) users      (100)     7552 2023-04-17 16:12:39.166091 FreeGS-0.7.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) users      (100)     6739 2023-04-17 16:11:10.000000 FreeGS-0.7.0/README.md
+drwxr-xr-x   0 peter     (1000) users      (100)        0 2023-04-17 16:12:39.166091 FreeGS-0.7.0/freegs/
+-rw-r--r--   0 peter     (1000) users      (100)     1073 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/__init__.py
+-rw-r--r--   0 peter     (1000) users      (100)    12250 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_aeqdsk.py
+-rw-r--r--   0 peter     (1000) users      (100)     3218 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_divgeo.py
+-rw-r--r--   0 peter     (1000) users      (100)     3023 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_fileutils.py
+-rw-r--r--   0 peter     (1000) users      (100)     7807 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/_geqdsk.py
+-rw-r--r--   0 peter     (1000) users      (100)      198 2023-03-17 16:15:33.000000 FreeGS-0.7.0/freegs/_version.py
+-rw-r--r--   0 peter     (1000) users      (100)     6183 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/boundary.py
+-rw-r--r--   0 peter     (1000) users      (100)     8386 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/coil.py
+-rw-r--r--   0 peter     (1000) users      (100)     9985 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/control.py
+-rw-r--r--   0 peter     (1000) users      (100)    16601 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/critical.py
+-rw-r--r--   0 peter     (1000) users      (100)      287 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/divgeo.py
+-rw-r--r--   0 peter     (1000) users      (100)     8858 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/dump.py
+-rw-r--r--   0 peter     (1000) users      (100)    42373 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/equilibrium.py
+-rw-r--r--   0 peter     (1000) users      (100)     7117 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/fieldtracer.py
+-rw-r--r--   0 peter     (1000) users      (100)    10087 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/filament_coil.py
+-rwxr-xr-x   0 peter     (1000) users      (100)    15345 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/geqdsk.py
+-rw-r--r--   0 peter     (1000) users      (100)     8512 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/gradshafranov.py
+-rw-r--r--   0 peter     (1000) users      (100)    15798 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/jtor.py
+-rw-r--r--   0 peter     (1000) users      (100)    60565 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/machine.py
+-rw-r--r--   0 peter     (1000) users      (100)    11049 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/multigrid.py
+-rw-r--r--   0 peter     (1000) users      (100)     6443 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/optimise.py
+-rw-r--r--   0 peter     (1000) users      (100)     5144 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/optimiser.py
+-rw-r--r--   0 peter     (1000) users      (100)     7244 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/picard.py
+-rw-r--r--   0 peter     (1000) users      (100)     3402 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/plotting.py
+-rw-r--r--   0 peter     (1000) users      (100)     5126 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/polygons.py
+-rw-r--r--   0 peter     (1000) users      (100)     7276 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/pre_calc_coil.py
+-rw-r--r--   0 peter     (1000) users      (100)     3818 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/quadrature.py
+-rw-r--r--   0 peter     (1000) users      (100)     7165 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/shaped_coil.py
+-rw-r--r--   0 peter     (1000) users      (100)     2963 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_aeqdsk.py
+-rw-r--r--   0 peter     (1000) users      (100)     2758 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_critical.py
+-rw-r--r--   0 peter     (1000) users      (100)     1455 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_equilibrium.py
+-rw-r--r--   0 peter     (1000) users      (100)      685 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_fileutils.py
+-rw-r--r--   0 peter     (1000) users      (100)      996 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_geqdsk.py
+-rw-r--r--   0 peter     (1000) users      (100)      918 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_jtor.py
+-rw-r--r--   0 peter     (1000) users      (100)     1649 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_linearsolve.py
+-rw-r--r--   0 peter     (1000) users      (100)     1940 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_machine.py
+-rw-r--r--   0 peter     (1000) users      (100)     2755 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_multi_coil.py
+-rw-r--r--   0 peter     (1000) users      (100)     1474 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_optimise.py
+-rw-r--r--   0 peter     (1000) users      (100)     4036 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_optimiser.py
+-rw-r--r--   0 peter     (1000) users      (100)     1574 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_polygons.py
+-rw-r--r--   0 peter     (1000) users      (100)     1251 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_quadrature.py
+-rw-r--r--   0 peter     (1000) users      (100)     1306 2023-04-17 16:06:31.000000 FreeGS-0.7.0/freegs/test_readwrite.py
+-rw-r--r--   0 peter     (1000) users      (100)     1535 2022-10-10 08:00:46.000000 FreeGS-0.7.0/freegs/test_shaped_coil.py
+-rw-r--r--   0 peter     (1000) users      (100)       38 2023-04-17 16:12:39.166091 FreeGS-0.7.0/setup.cfg
+-rw-r--r--   0 peter     (1000) users      (100)     1242 2023-04-17 16:12:30.000000 FreeGS-0.7.0/setup.py
```

### Comparing `FreeGS-0.6.1/FreeGS.egg-info/PKG-INFO` & `FreeGS-0.7.0/FreeGS.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,204 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: FreeGS
-Version: 0.6.1
+Version: 0.7.0
 Summary: Free boundary Grad-Shafranov solver for tokamak plasma equilibria
 Home-page: https://github.com/bendudson/freegs
 Author: Ben Dudson
 Author-email: benjamin.dudson@york.ac.uk
 License: LGPL
-Description: FreeGS: Free boundary Grad-Shafranov solver
-        ===========================================
-        
-        [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
-        [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-        [![Build Status](https://travis-ci.org/bendudson/freegs.svg?branch=master)](https://travis-ci.org/bendudson/freegs)
-        
-        This Python module calculates plasma equilibria for tokamak fusion experiments,
-        by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
-        plasma profiles and shape, FreeGS finds the currents in the coils which produce
-        a steady-state solution in force balance.
-        
-        **Note** This is a work in progress, and probably contains bugs. 
-        There is a feature wishlist in issues, suggestions and contributions welcome!
-        
-        Installing
-        ----------
-        
-        FreeGS is available on PyPI 
-        
-            $ pip install --user freegs
-        
-        or clone/download this repository and run setup:
-        
-            $ git clone https://github.com/bendudson/freegs.git
-            $ cd freegs
-            $ python setup.py install --user
-        
-        Documentation
-        -------------
-        
-        The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
-        
-        Testing
-        -------
-        
-        Unit tests use [pytest](https://docs.pytest.org/en/latest/) so after installing, run with:
-        
-            $ pytest
-        
-        The tests are in the `src/` subdirectory.
-        
-        A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
-        
-            $ python test-convergence.py
-        
-        Examples
-        --------
-        
-        The Jupyter notebooks contain examples wuth additional notes
-        
-        * MAST-example.ipynb 
-        
-        There are also some Python scripts to run short tests
-        and examples
-        
-            $ python 01-freeboundary.py
-        
-        This solves a free boundary problem, specifying the desired location of two X-points.
-        Writes the equilibrium to a G-EQDSK file "lsn.geqdsk"
-        
-            $ python 02-read-geqdsk.py
-        
-        Reads in the file "lsn.geqdsk", inferring the coil currents from the plasma boundary
-        and profiles in the G-EQDSK file.
-        
-            $ python 03-mast.py
-        
-        Calculates a double-null (CDND) equilibrium for MAST from scratch. Writes solution to
-        G-EQDSK file "mast.geqdsk"
-        
-            $ python 04-read-mast-geqdsk.py
-        
-        Reads the file "mast.geqdsk", inferring the coil currents.
-        
-            $ python 05-fixed-boundary.py 
-        
-        This example solves a fixed boundary problem, in which the square edges of the domain
-        are fixed. The plasma pressure on axis and plasma current are fixed.
-        
-            $ python 06-xpoints.py
-        
-        This demonstrates the coil current control code, finding X-points, and marking core region
-        These routines are used inside the free boundary solver
-        
-        Files
-        -----
-        
-        The "freegs" module consists of the following files:
-        
-        * **boundary.py**        - Operators for applying boundary conditions to plasma psi
-        * **control.py**         - Routines for controlling coil currents based on constraints
-        * **critical.py**        - Finds critical points (O- and X-points)
-        * **equilibrium.py**     - Represents the plasma equilibrium state
-        * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
-        * **jtor.py**            - Routines for calculating toroidal current density (profiles)
-        * **machine.py**         - Represents the coils and power supply circuits
-        * **multigrid.py**       - The multigrid solver for the linear elliptic operator
-        * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
-        * **plotting.py**        - Plotting routines using matplotlib
-        
-        License
-        -------
-        
-            Copyright 2016-2021 Ben Dudson, University of York, and other contributors.
-            Email: benjamin.dudson@york.ac.uk
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Lesser General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Lesser General Public License for more details.
-        
-            You should have received a copy of the GNU Lesser General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>.
-        
-        References
-        ----------
-        
-        * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
-        * S.Jardin "Computational Methods in Plasma Physics" CRC Press
-        
-        
-        Versions
-        --------
-        
-        0.6.1  11th February 2021
-          - Fixes for HDF5 reading and writing
-          - Fix Numpy deprecations
-          - Catch errors in optimisation measures, making that more robust
-          - Fix core mask in geqdsk file reading
-          - Flake8 fixes
-          - Move to Github actions
-        
-        0.6.0  29th January 2021
-          - Improve separatrix finding (Pablo Rodriguez-Fernandez)
-          - Update MAST-U machine description (James Harrison)
-          - Updated documentation
-          - Add tests for critical point finding
-          - Black format all library code
-          - Fix wall intersection calculation in optimisation
-          - Fix factor of pi in effectiveElongation (Chris Winnard)
-          - Miscellaneous fixes and tidying (Chris Winnard)
-          - Fix psi_bndry test in critical.core_mask
-          - Fix comments in Greens functions (James Morris)
-        
-        0.5.0  25th March 2020
-          - More tests, thanks to @ZedThree.
-          - Added more flexible coil types, thanks to Chris Marsden.
-            Includes support for shaped coils, multi-strand coils,
-            and up-down mirrored coils.
-          - Basic support for reading and writing AEQDSK files
-          - Added h5py to requirements, fixes for latest NumPy
-        
-        0.4.0  10th November 2019
-          - Add optimisation with Differential Evolution
-          - More unit testing, documentation
-        
-        0.3.0  28th July 2019
-          - Add 4th-order solver for potential
-          - Add convergence test
-        
-        0.2.0  12th March 2019
-          - Add field line tracer, `freegs.fieldtracer`
-          - Add Equilibrium.Btor toroidal field calculation
-          - Add Equilibrium.plasmaVolume
-          - Fix rlim, zlim saved into GEQDSK files
-        
-        
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+FreeGS: Free boundary Grad-Shafranov solver
+===========================================
+
+[![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
+[![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
+[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
+
+This Python module calculates plasma equilibria for tokamak fusion experiments,
+by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
+plasma profiles and shape, FreeGS finds the currents in the coils which produce
+a steady-state solution in force balance.
+
+**Note** This is a work in progress, and probably contains bugs. 
+There is a feature wishlist in issues, suggestions and contributions welcome!
+
+Installing
+----------
+
+A public vesion of FreeGS is available on PyPI 
+
+    $ pip install --user freegs
+
+or clone/download the internal TE version and run setup:
+
+    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
+    $ cd freegs
+    $ python setup.py install --user
+
+Documentation
+-------------
+
+The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
+
+Testing
+-------
+
+Unit tests use [pytest](https://docs.pytest.org/en/latest/) so after installing, run with:
+
+    $ pytest
+
+The tests are in the `src/` subdirectory.
+
+A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
+
+    $ python test-convergence.py
+
+To-do list
+----------
+See the 'issues' board on the left hand toolbar.
+
+Examples
+--------
+(Note: some of these may no longer be working with changes to
+coil classes. Not exactly a priority to fix these at present.)
+
+The Jupyter notebooks contain examples wuth additional notes
+
+* MAST-example.ipynb 
+
+There are also some Python scripts to run short tests
+and examples
+
+    $ python 01-freeboundary.py
+
+This solves a free boundary problem, specifying the desired location of two X-points.
+Writes the equilibrium to a G-EQDSK file "lsn.geqdsk"
+
+    $ python 02-read-geqdsk.py
+
+Reads in the file "lsn.geqdsk", inferring the coil currents from the plasma boundary
+and profiles in the G-EQDSK file.
+
+    $ python 03-mast.py
+
+Calculates a double-null (CDND) equilibrium for MAST from scratch. Writes solution to
+G-EQDSK file "mast.geqdsk"
+
+    $ python 04-read-mast-geqdsk.py
+
+Reads the file "mast.geqdsk", inferring the coil currents.
+
+    $ python 05-fixed-boundary.py 
+
+This example solves a fixed boundary problem, in which the square edges of the domain
+are fixed. The plasma pressure on axis and plasma current are fixed.
+
+    $ python 06-xpoints.py
+
+This demonstrates the coil current control code, finding X-points, and marking core region
+These routines are used inside the free boundary solver
+
+Files
+-----
+
+The "freegs" module consists of the following files:
+
+* **boundary.py**        - Operators for applying boundary conditions to plasma psi
+* **control.py**         - Routines for controlling coil currents based on constraints
+* **critical.py**        - Finds critical points (O- and X-points)
+* **equilibrium.py**     - Represents the plasma equilibrium state
+* **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
+* **jtor.py**            - Routines for calculating toroidal current density (profiles)
+* **machine.py**         - Represents the coils and power supply circuits
+* **multigrid.py**       - The multigrid solver for the linear elliptic operator
+* **picard.py**          - Nonlinear solver, iterating the profiles and constraints
+* **plotting.py**        - Plotting routines using matplotlib
+
+- more files have since been added! Check the repo.
+
+License
+-------
+
+    Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
+    Email: benjamin.dudson@york.ac.uk
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Lesser General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+References
+----------
+
+* YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
+* S.Jardin "Computational Methods in Plasma Physics" CRC Press
+
+Longer-term the intent is to move FreeGS development back to a public repo and to
+develop bespoke TE scripts in the eqtools python module.
+
+Public Versions
+---------------
+
+0.6.1  11th February 2021
+  - Fixes for HDF5 reading and writing
+  - Fix Numpy deprecations
+  - Catch errors in optimisation measures, making that more robust
+  - Fix core mask in geqdsk file reading
+  - Flake8 fixes
+  - Move to Github actions
+
+0.6.0  29th January 2021
+  - Improve separatrix finding (Pablo Rodriguez-Fernandez)
+  - Update MAST-U machine description (James Harrison)
+  - Updated documentation
+  - Add tests for critical point finding
+  - Black format all library code
+  - Fix wall intersection calculation in optimisation
+  - Fix factor of pi in effectiveElongation (Chris Winnard)
+  - Miscellaneous fixes and tidying (Chris Winnard)
+  - Fix psi_bndry test in critical.core_mask
+  - Fix comments in Greens functions (James Morris)
+
+0.5.0  25th March 2020
+  - More tests, thanks to @ZedThree.
+  - Added more flexible coil types, thanks to Chris Marsden.
+    Includes support for shaped coils, multi-strand coils,
+    and up-down mirrored coils.
+  - Basic support for reading and writing AEQDSK files
+  - Added h5py to requirements, fixes for latest NumPy
+
+0.4.0  10th November 2019
+  - Add optimisation with Differential Evolution
+  - More unit testing, documentation
+
+0.3.0  28th July 2019
+  - Add 4th-order solver for potential
+  - Add convergence test
+
+0.2.0  12th March 2019
+  - Add field line tracer, `freegs.fieldtracer`
+  - Add Equilibrium.Btor toroidal field calculation
+  - Add Equilibrium.plasmaVolume
+  - Fix rlim, zlim saved into GEQDSK files
+
```

### Comparing `FreeGS-0.6.1/FreeGS.egg-info/SOURCES.txt` & `FreeGS-0.7.0/FreeGS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+LICENSE
 README.md
 setup.py
 FreeGS.egg-info/PKG-INFO
 FreeGS.egg-info/SOURCES.txt
 FreeGS.egg-info/dependency_links.txt
 FreeGS.egg-info/requires.txt
 FreeGS.egg-info/top_level.txt
 freegs/__init__.py
 freegs/_aeqdsk.py
 freegs/_divgeo.py
 freegs/_fileutils.py
 freegs/_geqdsk.py
+freegs/_version.py
 freegs/boundary.py
 freegs/coil.py
 freegs/control.py
 freegs/critical.py
 freegs/divgeo.py
 freegs/dump.py
 freegs/equilibrium.py
 freegs/fieldtracer.py
+freegs/filament_coil.py
 freegs/geqdsk.py
 freegs/gradshafranov.py
 freegs/jtor.py
 freegs/machine.py
-freegs/multi_coil.py
 freegs/multigrid.py
 freegs/optimise.py
 freegs/optimiser.py
 freegs/picard.py
 freegs/plotting.py
 freegs/polygons.py
+freegs/pre_calc_coil.py
 freegs/quadrature.py
 freegs/shaped_coil.py
 freegs/test_aeqdsk.py
 freegs/test_critical.py
 freegs/test_equilibrium.py
 freegs/test_fileutils.py
 freegs/test_geqdsk.py
```

### Comparing `FreeGS-0.6.1/PKG-INFO` & `FreeGS-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,191 +1,204 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: FreeGS
-Version: 0.6.1
+Version: 0.7.0
 Summary: Free boundary Grad-Shafranov solver for tokamak plasma equilibria
 Home-page: https://github.com/bendudson/freegs
 Author: Ben Dudson
 Author-email: benjamin.dudson@york.ac.uk
 License: LGPL
-Description: FreeGS: Free boundary Grad-Shafranov solver
-        ===========================================
-        
-        [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
-        [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-        [![Build Status](https://travis-ci.org/bendudson/freegs.svg?branch=master)](https://travis-ci.org/bendudson/freegs)
-        
-        This Python module calculates plasma equilibria for tokamak fusion experiments,
-        by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
-        plasma profiles and shape, FreeGS finds the currents in the coils which produce
-        a steady-state solution in force balance.
-        
-        **Note** This is a work in progress, and probably contains bugs. 
-        There is a feature wishlist in issues, suggestions and contributions welcome!
-        
-        Installing
-        ----------
-        
-        FreeGS is available on PyPI 
-        
-            $ pip install --user freegs
-        
-        or clone/download this repository and run setup:
-        
-            $ git clone https://github.com/bendudson/freegs.git
-            $ cd freegs
-            $ python setup.py install --user
-        
-        Documentation
-        -------------
-        
-        The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
-        
-        Testing
-        -------
-        
-        Unit tests use [pytest](https://docs.pytest.org/en/latest/) so after installing, run with:
-        
-            $ pytest
-        
-        The tests are in the `src/` subdirectory.
-        
-        A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
-        
-            $ python test-convergence.py
-        
-        Examples
-        --------
-        
-        The Jupyter notebooks contain examples wuth additional notes
-        
-        * MAST-example.ipynb 
-        
-        There are also some Python scripts to run short tests
-        and examples
-        
-            $ python 01-freeboundary.py
-        
-        This solves a free boundary problem, specifying the desired location of two X-points.
-        Writes the equilibrium to a G-EQDSK file "lsn.geqdsk"
-        
-            $ python 02-read-geqdsk.py
-        
-        Reads in the file "lsn.geqdsk", inferring the coil currents from the plasma boundary
-        and profiles in the G-EQDSK file.
-        
-            $ python 03-mast.py
-        
-        Calculates a double-null (CDND) equilibrium for MAST from scratch. Writes solution to
-        G-EQDSK file "mast.geqdsk"
-        
-            $ python 04-read-mast-geqdsk.py
-        
-        Reads the file "mast.geqdsk", inferring the coil currents.
-        
-            $ python 05-fixed-boundary.py 
-        
-        This example solves a fixed boundary problem, in which the square edges of the domain
-        are fixed. The plasma pressure on axis and plasma current are fixed.
-        
-            $ python 06-xpoints.py
-        
-        This demonstrates the coil current control code, finding X-points, and marking core region
-        These routines are used inside the free boundary solver
-        
-        Files
-        -----
-        
-        The "freegs" module consists of the following files:
-        
-        * **boundary.py**        - Operators for applying boundary conditions to plasma psi
-        * **control.py**         - Routines for controlling coil currents based on constraints
-        * **critical.py**        - Finds critical points (O- and X-points)
-        * **equilibrium.py**     - Represents the plasma equilibrium state
-        * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
-        * **jtor.py**            - Routines for calculating toroidal current density (profiles)
-        * **machine.py**         - Represents the coils and power supply circuits
-        * **multigrid.py**       - The multigrid solver for the linear elliptic operator
-        * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
-        * **plotting.py**        - Plotting routines using matplotlib
-        
-        License
-        -------
-        
-            Copyright 2016-2021 Ben Dudson, University of York, and other contributors.
-            Email: benjamin.dudson@york.ac.uk
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Lesser General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Lesser General Public License for more details.
-        
-            You should have received a copy of the GNU Lesser General Public License
-            along with this program.  If not, see <http://www.gnu.org/licenses/>.
-        
-        References
-        ----------
-        
-        * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
-        * S.Jardin "Computational Methods in Plasma Physics" CRC Press
-        
-        
-        Versions
-        --------
-        
-        0.6.1  11th February 2021
-          - Fixes for HDF5 reading and writing
-          - Fix Numpy deprecations
-          - Catch errors in optimisation measures, making that more robust
-          - Fix core mask in geqdsk file reading
-          - Flake8 fixes
-          - Move to Github actions
-        
-        0.6.0  29th January 2021
-          - Improve separatrix finding (Pablo Rodriguez-Fernandez)
-          - Update MAST-U machine description (James Harrison)
-          - Updated documentation
-          - Add tests for critical point finding
-          - Black format all library code
-          - Fix wall intersection calculation in optimisation
-          - Fix factor of pi in effectiveElongation (Chris Winnard)
-          - Miscellaneous fixes and tidying (Chris Winnard)
-          - Fix psi_bndry test in critical.core_mask
-          - Fix comments in Greens functions (James Morris)
-        
-        0.5.0  25th March 2020
-          - More tests, thanks to @ZedThree.
-          - Added more flexible coil types, thanks to Chris Marsden.
-            Includes support for shaped coils, multi-strand coils,
-            and up-down mirrored coils.
-          - Basic support for reading and writing AEQDSK files
-          - Added h5py to requirements, fixes for latest NumPy
-        
-        0.4.0  10th November 2019
-          - Add optimisation with Differential Evolution
-          - More unit testing, documentation
-        
-        0.3.0  28th July 2019
-          - Add 4th-order solver for potential
-          - Add convergence test
-        
-        0.2.0  12th March 2019
-          - Add field line tracer, `freegs.fieldtracer`
-          - Add Equilibrium.Btor toroidal field calculation
-          - Add Equilibrium.plasmaVolume
-          - Fix rlim, zlim saved into GEQDSK files
-        
-        
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+FreeGS: Free boundary Grad-Shafranov solver
+===========================================
+
+[![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
+[![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
+[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
+
+This Python module calculates plasma equilibria for tokamak fusion experiments,
+by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
+plasma profiles and shape, FreeGS finds the currents in the coils which produce
+a steady-state solution in force balance.
+
+**Note** This is a work in progress, and probably contains bugs. 
+There is a feature wishlist in issues, suggestions and contributions welcome!
+
+Installing
+----------
+
+A public vesion of FreeGS is available on PyPI 
+
+    $ pip install --user freegs
+
+or clone/download the internal TE version and run setup:
+
+    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
+    $ cd freegs
+    $ python setup.py install --user
+
+Documentation
+-------------
+
+The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
+
+Testing
+-------
+
+Unit tests use [pytest](https://docs.pytest.org/en/latest/) so after installing, run with:
+
+    $ pytest
+
+The tests are in the `src/` subdirectory.
+
+A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
+
+    $ python test-convergence.py
+
+To-do list
+----------
+See the 'issues' board on the left hand toolbar.
+
+Examples
+--------
+(Note: some of these may no longer be working with changes to
+coil classes. Not exactly a priority to fix these at present.)
+
+The Jupyter notebooks contain examples wuth additional notes
+
+* MAST-example.ipynb 
+
+There are also some Python scripts to run short tests
+and examples
+
+    $ python 01-freeboundary.py
+
+This solves a free boundary problem, specifying the desired location of two X-points.
+Writes the equilibrium to a G-EQDSK file "lsn.geqdsk"
+
+    $ python 02-read-geqdsk.py
+
+Reads in the file "lsn.geqdsk", inferring the coil currents from the plasma boundary
+and profiles in the G-EQDSK file.
+
+    $ python 03-mast.py
+
+Calculates a double-null (CDND) equilibrium for MAST from scratch. Writes solution to
+G-EQDSK file "mast.geqdsk"
+
+    $ python 04-read-mast-geqdsk.py
+
+Reads the file "mast.geqdsk", inferring the coil currents.
+
+    $ python 05-fixed-boundary.py 
+
+This example solves a fixed boundary problem, in which the square edges of the domain
+are fixed. The plasma pressure on axis and plasma current are fixed.
+
+    $ python 06-xpoints.py
+
+This demonstrates the coil current control code, finding X-points, and marking core region
+These routines are used inside the free boundary solver
+
+Files
+-----
+
+The "freegs" module consists of the following files:
+
+* **boundary.py**        - Operators for applying boundary conditions to plasma psi
+* **control.py**         - Routines for controlling coil currents based on constraints
+* **critical.py**        - Finds critical points (O- and X-points)
+* **equilibrium.py**     - Represents the plasma equilibrium state
+* **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
+* **jtor.py**            - Routines for calculating toroidal current density (profiles)
+* **machine.py**         - Represents the coils and power supply circuits
+* **multigrid.py**       - The multigrid solver for the linear elliptic operator
+* **picard.py**          - Nonlinear solver, iterating the profiles and constraints
+* **plotting.py**        - Plotting routines using matplotlib
+
+- more files have since been added! Check the repo.
+
+License
+-------
+
+    Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
+    Email: benjamin.dudson@york.ac.uk
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Lesser General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+References
+----------
+
+* YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
+* S.Jardin "Computational Methods in Plasma Physics" CRC Press
+
+Longer-term the intent is to move FreeGS development back to a public repo and to
+develop bespoke TE scripts in the eqtools python module.
+
+Public Versions
+---------------
+
+0.6.1  11th February 2021
+  - Fixes for HDF5 reading and writing
+  - Fix Numpy deprecations
+  - Catch errors in optimisation measures, making that more robust
+  - Fix core mask in geqdsk file reading
+  - Flake8 fixes
+  - Move to Github actions
+
+0.6.0  29th January 2021
+  - Improve separatrix finding (Pablo Rodriguez-Fernandez)
+  - Update MAST-U machine description (James Harrison)
+  - Updated documentation
+  - Add tests for critical point finding
+  - Black format all library code
+  - Fix wall intersection calculation in optimisation
+  - Fix factor of pi in effectiveElongation (Chris Winnard)
+  - Miscellaneous fixes and tidying (Chris Winnard)
+  - Fix psi_bndry test in critical.core_mask
+  - Fix comments in Greens functions (James Morris)
+
+0.5.0  25th March 2020
+  - More tests, thanks to @ZedThree.
+  - Added more flexible coil types, thanks to Chris Marsden.
+    Includes support for shaped coils, multi-strand coils,
+    and up-down mirrored coils.
+  - Basic support for reading and writing AEQDSK files
+  - Added h5py to requirements, fixes for latest NumPy
+
+0.4.0  10th November 2019
+  - Add optimisation with Differential Evolution
+  - More unit testing, documentation
+
+0.3.0  28th July 2019
+  - Add 4th-order solver for potential
+  - Add convergence test
+
+0.2.0  12th March 2019
+  - Add field line tracer, `freegs.fieldtracer`
+  - Add Equilibrium.Btor toroidal field calculation
+  - Add Equilibrium.plasmaVolume
+  - Fix rlim, zlim saved into GEQDSK files
+
```

### Comparing `FreeGS-0.6.1/README.md` & `FreeGS-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 FreeGS: Free boundary Grad-Shafranov solver
 ===========================================
 
 [![License](https://img.shields.io/badge/license-GPL-blue.svg)](https://img.shields.io/badge/license-GPL-blue.svg)
 [![py3comp](https://img.shields.io/badge/py3-compatible-brightgreen.svg)](https://img.shields.io/badge/py3-compatible-brightgreen.svg)
-[![Build Status](https://travis-ci.org/bendudson/freegs.svg?branch=master)](https://travis-ci.org/bendudson/freegs)
+[![Build Status](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)](https://github.com/bendudson/freegs/workflows/Tests/badge.svg)
+[![codecov](https://codecov.io/gh/bendudson/freegs/branch/master/graph/badge.svg?token=4dc6aHbu7K)](https://codecov.io/gh/bendudson/freegs)
 
 This Python module calculates plasma equilibria for tokamak fusion experiments,
 by solving the Grad-Shafranov equation with free boundaries. Given a set of coils,
 plasma profiles and shape, FreeGS finds the currents in the coils which produce
 a steady-state solution in force balance.
 
 **Note** This is a work in progress, and probably contains bugs. 
 There is a feature wishlist in issues, suggestions and contributions welcome!
 
 Installing
 ----------
 
-FreeGS is available on PyPI 
+A public vesion of FreeGS is available on PyPI 
 
     $ pip install --user freegs
 
-or clone/download this repository and run setup:
+or clone/download the internal TE version and run setup:
 
-    $ git clone https://github.com/bendudson/freegs.git
+    $ git clone http://tokamak-devlin/gitlab/physics/freegs.git
     $ cd freegs
     $ python setup.py install --user
 
 Documentation
 -------------
 
 The manual is in the `docs` subdirectory, and [hosted here on readthedocs](http://freegs.readthedocs.io/en/latest/).
@@ -40,16 +41,22 @@
 
 The tests are in the `src/` subdirectory.
 
 A convergence test is [described in the manual](https://freegs.readthedocs.io/en/latest/tests.html#convergence-test). To run:
 
     $ python test-convergence.py
 
+To-do list
+----------
+See the 'issues' board on the left hand toolbar.
+
 Examples
 --------
+(Note: some of these may no longer be working with changes to
+coil classes. Not exactly a priority to fix these at present.)
 
 The Jupyter notebooks contain examples wuth additional notes
 
 * MAST-example.ipynb 
 
 There are also some Python scripts to run short tests
 and examples
@@ -95,18 +102,20 @@
 * **gradshafranov.py**   - Greens functions and operators for the Grad-Shafranov equation
 * **jtor.py**            - Routines for calculating toroidal current density (profiles)
 * **machine.py**         - Represents the coils and power supply circuits
 * **multigrid.py**       - The multigrid solver for the linear elliptic operator
 * **picard.py**          - Nonlinear solver, iterating the profiles and constraints
 * **plotting.py**        - Plotting routines using matplotlib
 
+- more files have since been added! Check the repo.
+
 License
 -------
 
-    Copyright 2016-2021 Ben Dudson, University of York, and other contributors.
+    Copyright 2016-2022 Ben Dudson, University of York, and other contributors.
     Email: benjamin.dudson@york.ac.uk
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU Lesser General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
@@ -120,17 +129,19 @@
 
 References
 ----------
 
 * YoungMu Jeon, [Development of a free boundary Tokamak Equlibrium Solver](http://link.springer.com/article/10.3938/jkps.67.843)  [arXiv:1503.03135](https://arxiv.org/abs/1503.03135)
 * S.Jardin "Computational Methods in Plasma Physics" CRC Press
 
+Longer-term the intent is to move FreeGS development back to a public repo and to
+develop bespoke TE scripts in the eqtools python module.
 
-Versions
---------
+Public Versions
+---------------
 
 0.6.1  11th February 2021
   - Fixes for HDF5 reading and writing
   - Fix Numpy deprecations
   - Catch errors in optimisation measures, making that more robust
   - Fix core mask in geqdsk file reading
   - Flake8 fixes
```

### Comparing `FreeGS-0.6.1/freegs/__init__.py` & `FreeGS-0.7.0/freegs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 from .equilibrium import Equilibrium
 
 from . import jtor
 
 from . import machine
```

### Comparing `FreeGS-0.6.1/freegs/_aeqdsk.py` & `FreeGS-0.7.0/freegs/_aeqdsk.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/_divgeo.py` & `FreeGS-0.7.0/freegs/_divgeo.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/_fileutils.py` & `FreeGS-0.7.0/freegs/_fileutils.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/_geqdsk.py` & `FreeGS-0.7.0/freegs/_geqdsk.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/boundary.py` & `FreeGS-0.7.0/freegs/boundary.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/coil.py` & `FreeGS-0.7.0/freegs/coil.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,10 +267,10 @@
 
         import matplotlib.pyplot as plt
 
         if axis is None:
             fig = plt.figure()
             axis = fig.add_subplot(111)
 
-        circle = plt.Circle((self.R, self.Z), minor_radius, color="b")
+        circle = plt.Circle((self.R, self.Z), minor_radius, color="gray")
         axis.add_artist(circle)
         return axis
```

### Comparing `FreeGS-0.6.1/freegs/control.py` & `FreeGS-0.7.0/freegs/control.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Plasma control system
 
 Use constraints to adjust coil currents
 """
 
-from numpy import dot, transpose, eye, array
-from numpy.linalg import inv
+from numpy import dot, transpose, eye, array, inf
+from numpy.linalg import inv, norm
 import numpy as np
-
 from scipy import optimize
-
 from . import critical
 
 
 class constrain(object):
     """
     Adjust coil currents using constraints. To use this class,
     first create an instance by specifying the constraints
@@ -32,27 +30,36 @@
 
     xpoints - A list of X-point (R,Z) locations
 
     isoflux - A list of tuples (R1,Z1, R2,Z2)
 
     psivals - A list of (R,Z,psi) values
 
-    At least one constraint must be included
+    At least one of the above constraints must be included.
 
     gamma - A scalar, minimises the magnitude of the coil currents
+
+    The following constraitns are entirely optional:
+
+    current_lims - A list of tuples [(l1,u1),(l2,u2)...(lN,uN)] for the upper
+    and lower bounds on the currents in each coil.
+
+    max_total_current - The maximum total current through the coilset.
     """
 
-    def __init__(self, xpoints=[], gamma=1e-12, isoflux=[], psivals=[]):
+    def __init__(self, xpoints=[], gamma=1e-12, isoflux=[], psivals=[], current_lims=None, max_total_current=None):
         """
         Create an instance, specifying the constraints to apply
         """
-        self.xpoints = xpoints
-        self.gamma = gamma
-        self.isoflux = isoflux
-        self.psivals = psivals
+        self.xpoints           = xpoints
+        self.gamma             = gamma
+        self.isoflux           = isoflux
+        self.psivals           = psivals
+        self.current_lims      = current_lims
+        self.max_total_current = max_total_current
 
     def __call__(self, eq):
         """
         Apply constraints to Equilibrium eq
         """
 
         tokamak = eq.getMachine()
@@ -103,29 +110,76 @@
         if not constraint_rhs:
             raise ValueError("No constraints given")
 
         # Constraint matrix
         A = array(constraint_matrix)
         b = np.reshape(array(constraint_rhs), (-1,))
 
-        # Solve by Tikhonov regularisation
-        # minimise || Ax - b ||^2 + ||gamma x ||^2
-        #
-        # x = (A^T A + gamma^2 I)^{-1}A^T b
-
         # Number of controls (length of x)
         ncontrols = A.shape[1]
+        
+        # First solve analytically by Tikhonov regularisation
+        # minimise || Ax - b ||^2 + ||gamma x ||^2
 
         # Calculate the change in coil current
-        current_change = dot(
+        self.current_change = dot(
             inv(dot(transpose(A), A) + self.gamma ** 2 * eye(ncontrols)),
             dot(transpose(A), b),
         )
-        # print("Current changes: " + str(current_change))
-        tokamak.controlAdjust(current_change)
+
+        # Now use the initial analytical soln to guide constrained solve
+        
+        # Establish constraints on changes in coil currents from the present
+        # and max/min coil current constraints
+
+        current_change_bounds = []
+
+        if self.current_lims is None:
+            for i in range(ncontrols):
+                current_change_bounds.append((-inf,inf))
+        else:
+            for i in range(ncontrols):
+                cur = tokamak.controlCurrents()[i]
+                lower_lim = self.current_lims[i][0]-cur
+                upper_lim = self.current_lims[i][1]-cur
+                current_change_bounds.append((lower_lim,upper_lim))
+
+        current_change_bnds = array(current_change_bounds)
+
+        # Reform the constraint matrices to include Tikhonov regularisation
+        A2 = np.concatenate([A, self.gamma*eye(ncontrols)])
+        b2 = np.concatenate([b, np.zeros(ncontrols)])
+
+        # The objetive function to minimize
+        # || A2x - b2 ||^2
+        def objective(x):
+            return (norm((A2@x)-b2))**2
+        
+        # Additional constraints on the optimisation
+        cons = []
+
+        def max_total_currents(x):
+            sum = 0.0
+            for delta,i in zip(x,tokamak.controlCurrents()):
+                sum+= abs(delta+i)
+            return -(sum-self.max_total_current)
+
+        if self.max_total_current is not None:
+            con1 = {'type': 'ineq', 'fun': max_total_currents}
+            cons.append(con1)
+
+        # Use the analytical current change as the initial guess
+        x0 = self.current_change
+        sol = optimize.minimize(objective,x0,method='SLSQP',bounds=current_change_bnds,constraints=cons)
+
+        self.current_change=sol.x
+        tokamak.controlAdjust(self.current_change)
+
+        # Store info for user
+        self.current_change = self.current_change
 
         # Ensure that the last constraint used is set in the Equilibrium
         eq._constraints = self
 
     def plot(self, axis=None, show=True):
         """
         Plots constraints used for coil current control
@@ -245,19 +299,22 @@
         if not opt:
             print("No O-points found!")
             print(opt, xpt)
             eq.plot()
             raise ValueError("No O-points found!")
         psi_axis = opt[0][2]
 
+        '''
         if not xpt:
             print("No X-points found!")
             eq.plot()
             raise ValueError("No X-points found")
-        psi_bndry = xpt[0][2]
+        '''
+
+        psi_bndry = eq.psi_bndry
 
         # Calculate normalised psi.
         # 0 = magnetic axis
         # 1 = plasma boundary
         psi_norm = (psi - psi_axis) / (psi_bndry - psi_axis)
 
         return (
```

### Comparing `FreeGS-0.6.1/freegs/critical.py` & `FreeGS-0.7.0/freegs/critical.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     sqrt,
     sum,
 )
 import numpy as np
 from warnings import warn
 
 
-def find_critical(R, Z, psi, discard_xpoints=False):
+def find_critical(R, Z, psi, discard_xpoints=True):
     """
     Find critical points
 
     Inputs
     ------
 
     R - R(nr, nz) 2D array of major radii
@@ -189,15 +189,15 @@
     Rmid = 0.5 * (R[-1, 0] + R[0, 0])
     Zmid = 0.5 * (Z[0, -1] + Z[0, 0])
     opoint.sort(key=lambda x: (x[0] - Rmid) ** 2 + (x[1] - Zmid) ** 2)
 
     # Draw a line from the O-point to each X-point. Psi should be
     # monotonic; discard those which are not
 
-    if True:  # discard_xpoints:
+    if discard_xpoints:
         Ro, Zo, Po = opoint[0]  # The primary O-point
         xpt_keep = []
         for xpt in xpoint:
             Rx, Zx, Px = xpt
 
             rline = linspace(Ro, Rx, num=50)
             zline = linspace(Zo, Zx, num=50)
@@ -391,15 +391,15 @@
     """
     if psi is None:
         psi = eq.psi()
 
     if (opoint is None) or (xpoint is None):
         opoint, xpoint = find_critical(eq.R, eq.Z, psi)
 
-    psinorm = (psi - opoint[0][2]) / (xpoint[0][2] - opoint[0][2])
+    psinorm = (psi - opoint[0][2]) / (eq.psi_bndry - opoint[0][2])
 
     psifunc = interpolate.RectBivariateSpline(eq.R[:, 0], eq.Z[0, :], psinorm)
 
     r0, z0 = opoint[0][0:2]
 
     theta_grid = linspace(0, 2 * pi, ntheta, endpoint=False)
     dtheta = theta_grid[1] - theta_grid[0]
```

### Comparing `FreeGS-0.6.1/freegs/dump.py` & `FreeGS-0.7.0/freegs/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     has_hdf5 = False
 
 import numpy as np
 
 from .equilibrium import Equilibrium
 from .machine import Coil, Circuit, Solenoid, Wall, Machine
 from .shaped_coil import ShapedCoil
-from .multi_coil import MultiCoil
+from .filament_coil import FilamentCoil
 from . import boundary
 from . import machine
 
 
 class OutputFormatNotAvailableError(Exception):
     """Raised when we couldn't import HDF5 (or some other library)
     required for this OutputFile format
@@ -111,22 +111,22 @@
     def write_equilibrium(self, equilibrium):
         """
         Write `equilbrium` to file
         """
 
         self.handle["coil_dtype"] = Coil.dtype
         self.handle["shapedcoil_dtype"] = ShapedCoil.dtype
-        self.handle["multicoil_dtype"] = MultiCoil.dtype
+        self.handle["filamentcoil_dtype"] = FilamentCoil.dtype
         self.handle["circuit_dtype"] = Circuit.dtype
         self.handle["solenoid_dtype"] = Solenoid.dtype
 
         type_to_dtype = {
             Coil.dtype: self.handle["coil_dtype"],
             ShapedCoil.dtype: self.handle["shapedcoil_dtype"],
-            MultiCoil.dtype: self.handle["multicoil_dtype"],
+            FilamentCoil.dtype: self.handle["filamentcoil_dtype"],
             Circuit.dtype: self.handle["circuit_dtype"],
             Solenoid.dtype: self.handle["solenoid_dtype"],
         }
 
         equilibrium_group = self.handle.require_group(self.EQUILIBRIUM_GROUP_NAME)
 
         equilibrium_group.create_dataset("Rmin", data=equilibrium.Rmin)
```

### Comparing `FreeGS-0.6.1/freegs/equilibrium.py` & `FreeGS-0.7.0/freegs/equilibrium.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 Defines class to represent the equilibrium
 state, including plasma and coil currents
 """
 
 from numpy import pi, meshgrid, linspace, exp, array
 import numpy as np
 from scipy import interpolate
-from scipy.integrate import romb  # Romberg integration
+from scipy.integrate import romb, cumtrapz  # Romberg integration
 
 from .boundary import fixedBoundary, freeBoundary
 from . import critical
 
 from . import polygons
 
 # Operators which define the G-S equation
 from .gradshafranov import mu0, GSsparse, GSsparse4thOrder
 
 # Multigrid solver
 from . import multigrid
 
 from . import machine
 
+import matplotlib.pyplot as plt
+
 
 class Equilibrium:
     """
     Represents the equilibrium state, including
     plasma and coil currents
 
     Data members
@@ -57,15 +59,15 @@
         Zmin=-1.0,
         Zmax=1.0,
         nx=65,
         ny=65,
         boundary=freeBoundary,
         psi=None,
         current=0.0,
-        order=4,
+        order=4
     ):
         """Initialises a plasma equilibrium
 
         Rmin, Rmax  - Range of major radius R [m]
         Zmin, Zmax  - Range of height Z [m]
 
         nx - Resolution in R. This must be 2^n + 1
@@ -76,14 +78,16 @@
         psi - Magnetic flux. If None, use concentric circular flux
               surfaces as starting guess
 
         current - Plasma current (default = 0.0)
 
         order - The order of the differential operators to use.
                 Valid values are 2 or 4.
+
+        check_limited - Boolean, checks if the plasma is limited.
         """
 
         self.tokamak = tokamak
 
         self._applyBoundary = boundary
 
         self.Rmin = Rmin
@@ -91,14 +95,19 @@
         self.Zmin = Zmin
         self.Zmax = Zmax
 
         self.R_1D = linspace(Rmin, Rmax, nx)
         self.Z_1D = linspace(Zmin, Zmax, ny)
         self.R, self.Z = meshgrid(self.R_1D, self.Z_1D, indexing="ij")
 
+        self.check_limited = False
+        self.is_limited = False
+        self.Rlim = None
+        self.Zlim = None
+
         if psi is None:
             # Starting guess for psi
             xx, yy = meshgrid(linspace(0, 1, nx), linspace(0, 1, ny), indexing="ij")
             psi = exp(-((xx - 0.5) ** 2 + (yy - 0.5) ** 2) / 0.4 ** 2)
 
             psi[0, :] = 0.0
             psi[:, 0] = 0.0
@@ -186,41 +195,14 @@
 
     def plasmaCurrent(self):
         """
         Plasma current [Amps]
         """
         return self._current
 
-    def poloidalBeta(self):
-        """
-        Return the poloidal beta
-        betap = (8pi/mu0) * int(p)dRdZ / Ip^2
-        """
-
-        dR = self.R[1, 0] - self.R[0, 0]
-        dZ = self.Z[0, 1] - self.Z[0, 0]
-
-        # Normalised psi
-        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
-
-        # Plasma pressure
-        pressure = self.pressure(psi_norm)
-        if self.mask is not None:
-            # If there is a masking function (X-points, limiters)
-            pressure *= self.mask
-
-        # Integrate pressure in 2D
-        return (
-            ((8.0 * pi) / mu0)
-            * romb(romb(pressure))
-            * dR
-            * dZ
-            / (self.plasmaCurrent() ** 2)
-        )
-
     def plasmaVolume(self):
         """Calculate the volume of the plasma in m^3"""
 
         dR = self.R[1, 0] - self.R[0, 0]
         dZ = self.Z[0, 1] - self.Z[0, 0]
 
         # Volume element
@@ -254,14 +236,22 @@
 
     def Bz(self, R, Z):
         """
         Total vertical magnetic field
         """
         return self.plasmaBz(R, Z) + self.tokamak.Bz(R, Z)
 
+    def Bpol(self, R, Z):
+        """
+        Total poloidal magnetic field
+        """
+        Br = self.Br(R,Z)
+        Bz = self.Bz(R,Z)
+        return np.sqrt(Br*Br + Bz*Bz)
+
     def Btor(self, R, Z):
         """
         Toroidal magnetic field
         """
         # Normalised psi
         psi_norm = (self.psiRZ(R, Z) - self.psi_axis) / (self.psi_bndry - self.psi_axis)
 
@@ -272,28 +262,53 @@
             # Get the values of the core mask at the requested R,Z locations
             # This is 1 in the core, 0 outside
             mask = self.mask_func(R, Z, grid=False)
             fpol = fpol * mask + (1.0 - mask) * self.fvac()
 
         return fpol / R
 
+    def Btot(self, R, Z):
+        """
+        Total magnetic field
+        """
+        Br = self.Br(R,Z)
+        Bz = self.Bz(R,Z)
+        Btor = self. Btor(R,Z)
+        return np.sqrt(Br*Br + Bz*Bz + Btor*Btor)       
+
     def psi(self):
         """
-        Total poloidal flux ψ (psi), including contribution from
+        Total poloidal flux (psi), including contribution from
         plasma and external coils.
         """
         # return self.plasma_psi + self.tokamak.psi(self.R, self.Z)
         return self.plasma_psi + self.tokamak.calcPsiFromGreens(self._pgreen)
 
+    def psiN(self):
+        """
+        Total poloidal flux (psi), including contribution from
+        plasma and external coils. Normalised such that psiN = 0 on
+        the magnetic axis and 1 on the LCFS.
+        """
+        # return self.plasma_psi + self.tokamak.psi(self.R, self.Z)
+        return (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+
     def psiRZ(self, R, Z):
         """
         Return poloidal flux psi at given (R,Z) location
         """
         return self.psi_func(R, Z, grid=False) + self.tokamak.psi(R, Z)
 
+    def psiNRZ(self, R, Z):
+        """
+        Return poloidal flux psi at given (R,Z) location. Normalised such
+        that psiN = 0 on the magnetic axis and 1 on the LCFS.
+        """
+        return (self.psiRZ(R, Z) - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+
     def fpol(self, psinorm):
         """
         Return f = R*Bt at specified values of normalised psi
         """
         return self._profiles.fpol(psinorm)
 
     def fvac(self):
@@ -326,69 +341,108 @@
 
         result = critical.find_safety(self, psinorm=psinorm)
         # Convert to a scalar if only one result
         if len(result) == 1:
             return np.asscalar(result)
         return result
 
+    def tor_flux(self, psi = None):
+        """
+        Calculates toroidal flux at specified values of poloidal flux.
+        >>> q = drho/dpsi
+        """
+        psiN = (psi - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+        # Get safety factor of these flux surfaces
+        qvals = self.q(psiN)
+
+        # Integrate q wrt psi to get rho. rho = 0 @ psiN = 0
+        result = cumtrapz(qvals,psi,initial=0.0)*(-1./(2.*np.pi))
+
+        # Convert to a scalar if only one result
+        if len(result) == 1:
+            return np.asscalar(result)
+        return result
+
+    def rhotor(self, psi = None):
+        """
+        Calculates normalised toroidal flux at specified values of
+        poloidal flux.
+         >>> rhotor = sqrt ( tor_flux/max(tor_flux)).
+        
+        Maximum toroidal flux shoud be at LCFS.
+        """
+
+        torflux = self.tor_flux(psi)
+
+        psi = np.linspace(self.psi_axis,self.psi_bndry,101,endpoint=True)
+        torflux_for_LCFS = self.tor_flux(psi)
+
+        max_torflux = np.max(torflux_for_LCFS)
+
+        result = np.sqrt(torflux/max_torflux)
+
+        if len(result) == 1:
+            return np.asscalar(result)
+        return result
+
     def pprime(self, psinorm):
         """
         Return p' at given normalised psi
         """
         return self._profiles.pprime(psinorm)
 
     def ffprime(self, psinorm):
         """
         Return ff' at given normalised psi
         """
         return self._profiles.ffprime(psinorm)
 
-    def pressure(self, psinorm, out=None):
+    def pressure(self, psinorm):
         """
         Returns plasma pressure at specified values of normalised psi
         """
         return self._profiles.pressure(psinorm)
 
-    def separatrix(self, ntheta=20):
+    def separatrix(self, npoints=360):
         """
-        Returns an array of ntheta (R, Z) coordinates of the separatrix,
+        Returns an array of npoints (R, Z) coordinates of the separatrix,
         equally spaced in geometric poloidal angle.
         """
-        return array(critical.find_separatrix(self, ntheta=ntheta, psi=self.psi()))[
+        return array(critical.find_separatrix(self, ntheta=npoints, psi=self.psi()))[
             :, 0:2
         ]
 
     def solve(self, profiles, Jtor=None, psi=None, psi_bndry=None):
         """
         Calculate the plasma equilibrium given new profiles
         replacing the current equilibrium.
 
         This performs the linear Grad-Shafranov solve
 
         profiles  - An object describing the plasma profiles.
                     At minimum this must have methods:
-             .Jtor(R, Z, psi)   -> [nx, ny]
+             .Jtor(R, Z, psi, psi_bndry)   -> [nx, ny]
              .pprime(psinorm)
              .ffprime(psinorm)
              .pressure(psinorm)
              .fpol(psinorm)
 
         Jtor : 2D array
             If supplied, specifies the toroidal current at each (R,Z) point
             If not supplied, Jtor is calculated from profiles by finding O,X-points
 
         psi_bndry  - Poloidal flux to use as the separatrix (plasma boundary)
                      If not given then X-point locations are used.
         """
 
         self._profiles = profiles
+        self._updateBoundaryPsi()
 
         if Jtor is None:
             # Calculate toroidal current density
-
             if psi is None:
                 psi = self.psi()
             Jtor = profiles.Jtor(self.R, self.Z, psi, psi_bndry=psi_bndry)
 
         # Set plasma boundary
         # Note that the Equilibrium is passed to the boundary function
         # since the boundary may need to run the G-S solver (von Hagenow's method)
@@ -409,14 +463,139 @@
         self._updatePlasmaPsi(plasma_psi)
 
         # Update plasma current
         dR = self.R[1, 0] - self.R[0, 0]
         dZ = self.Z[0, 1] - self.Z[0, 0]
         self._current = romb(romb(Jtor)) * dR * dZ
 
+    def _updateBoundaryPsi(self,psi=None):
+        """
+        For an input psi the magnetic axis and boundary psi are identified along
+        with the core mask.
+
+        Various logical checks occur, depending on whether or not the user
+        wishes to check if the plasma is limited or not, as well as whether
+        or not any xpoints are present.
+        """
+
+        if psi is None:
+            psi = self.psi()
+
+        opt, xpt = critical.find_critical(self.R, self.Z, psi)
+
+        psi = psi
+
+        if opt:
+        # Magnetic axis flux taken as primary o-point flux
+            self.psi_axis = opt[0][2]
+
+            '''
+            Several options depending on if user wishes to check
+            if the plasma becomes limited.
+            '''
+
+            # The user wishes to check if the plasma is limited
+            if(self.check_limited and self.tokamak.wall):
+
+                # A wall has actually been provided, proceed with checking
+
+                # Obtain flux on machine limit points
+                Rlimit = self.tokamak.limit_points_R
+                Zlimit = self.tokamak.limit_points_Z
+
+                '''
+                If an xpoint is present (plasma is potentianlly diverted)
+                then we must remove any limit points above/below the
+                primary xpoint as the PFR may land on these points,
+                which would break the algorithm (at present) for extracting the boundary
+                flux if the plasma were to infact be limited. There is a more advanced
+                version of this alogorithm that is more robust that will be
+                added in the future.
+                '''
+
+                if xpt:
+                    limit_args = np.ravel(np.argwhere(abs(Zlimit)<abs(0.75*xpt[0][1])))
+                    Rlimit = Rlimit[limit_args]
+                    Zlimit = Zlimit[limit_args]
+
+                # Obtain the flux psi at these limiter points
+                R = np.asarray(self.R[:, 0])
+                Z = np.asarray(self.Z[0, :])
+
+                # psi is transposed due to how FreeGS meshgrids R,Z
+                psi_2d = interpolate.interp2d(x=R,y=Z,z=psi.T)
+                
+                # Get psi at the limit points
+                psi_limit_points = np.zeros(len(Rlimit))
+                for i in range(len(Rlimit)):
+                    psi_limit_points[i] = psi_2d(Rlimit[i],Zlimit[i])[0]
+
+                # Get index of maximum psi value
+                indMax = np.argmax(psi_limit_points)
+                
+                # Extract R,Z of the contact point
+                self.Rlim = Rlimit[indMax]
+                self.Zlim = Zlimit[indMax]
+
+                # Obtain maximum psi
+                self.psi_limit = psi_limit_points[indMax]
+
+                # Check if any xpoints are present
+                if xpt:
+
+                    # Get flux from the primary xpoint
+                    self.psi_xpt = xpt[0][2]
+
+                    # Choose between diverted or limited flux
+                    self.psi_bndry = max(self.psi_xpt,self.psi_limit)
+
+                    if self.psi_bndry == self.psi_limit:
+                        self.is_limited = True
+
+                    else:
+                        self.is_limited = False
+
+                    # Mask the core
+                    self.mask = critical.core_mask(self.R, self.Z, psi, opt, xpt, self.psi_bndry)
+
+                    # Use interpolation to find if a point is in the core.
+                    self.mask_func = interpolate.RectBivariateSpline(
+                        self.R[:, 0], self.Z[0, :], self.mask
+                    )
+
+                else:
+
+                    # No xpoints, therefore psi_bndry = psi_limit
+                    self.psi_bndry = self.psi_limit
+                    self.is_limited = True
+                    self.mask = None
+
+            else:
+                # Either a wall was not provided or the user did not wish to
+                # check if the plasma was limited
+
+                if xpt:
+                    self.psi_xpt = xpt[0][2]
+                    self.psi_bndry = self.psi_xpt
+                    self.mask = critical.core_mask(self.R, self.Z, psi, opt, xpt)
+
+                    # Use interpolation to find if a point is in the core.
+                    self.mask_func = interpolate.RectBivariateSpline(
+                        self.R[:, 0], self.Z[0, :], self.mask
+                    )
+                elif self._applyBoundary is fixedBoundary:
+                    # No X-points, but using fixed boundary
+                    self.psi_bndry = psi[0, 0]  # Value of psi on the boundary
+                    self.mask = None  # All points are in the core region
+                else:
+                    self.psi_bndry = None
+                    self.mask = None
+
+                self.is_limited = False
+
     def _updatePlasmaPsi(self, plasma_psi):
         """
         Sets the plasma psi data, updates spline interpolation coefficients.
         Also updates:
 
         self.mask        2D (R,Z) array which is 1 in the core, 0 outside
         self.psi_axis    Value of psi on the magnetic axis
@@ -425,37 +604,16 @@
         self.plasma_psi = plasma_psi
 
         # Update spline interpolation
         self.psi_func = interpolate.RectBivariateSpline(
             self.R[:, 0], self.Z[0, :], plasma_psi
         )
 
-        # Update the locations of the X-points, core mask, psi ranges.
-        # Note that this may fail if there are no X-points, so it should not raise an error
-        # Analyse the equilibrium, finding O- and X-points
-        psi = self.psi()
-        opt, xpt = critical.find_critical(self.R, self.Z, psi)
-        if opt:
-            self.psi_axis = opt[0][2]
-
-            if xpt:
-                self.psi_bndry = xpt[0][2]
-                self.mask = critical.core_mask(self.R, self.Z, psi, opt, xpt)
-
-                # Use interpolation to find if a point is in the core.
-                self.mask_func = interpolate.RectBivariateSpline(
-                    self.R[:, 0], self.Z[0, :], self.mask
-                )
-            elif self._applyBoundary is fixedBoundary:
-                # No X-points, but using fixed boundary
-                self.psi_bndry = psi[0, 0]  # Value of psi on the boundary
-                self.mask = None  # All points are in the core region
-            else:
-                self.psi_bndry = None
-                self.mask = None
+        # Update the plasma axis and boundary flux as well as mask
+        self._updateBoundaryPsi()
 
     def plot(self, axis=None, show=True, oxpoints=True):
         """
         Plot the equilibrium flux surfaces
 
         axis     - Specify the axis on which to plot
         show     - Call matplotlib.pyplot.show() before returning
@@ -564,71 +722,237 @@
         opt, xpt = critical.find_critical(self.R, self.Z, self.psi())
         return opt[0]
 
     def Rmagnetic(self):
         """The major radius R of magnetic major radius"""
         return self.magneticAxis()[0]
 
-    def geometricAxis(self, npoints=20):
-        """Locates geometric axis, returning [R,Z]. Calculated as the centre
-        of a large number of points on the separatrix equally
-        distributed in angle from the magnetic axis.
-        """
-        separatrix = self.separatrix(ntheta=npoints)  # Array [:,2]
-        return np.mean(separatrix, axis=0)
-
-    def Rgeometric(self, npoints=20):
-        """Locates major radius R of the geometric major radius. Calculated
-        as the centre of a large number of points on the separatrix
-        equally distributed in angle from the magnetic axis.
+    def Zmagnetic(self):
+        """The height Z of magnetic axis"""
+        return self.magneticAxis()[1]
+
+    def geometricAxis(self, npoints=360):
+        """Locates geometric axis, returning [R,Z]. First locates the
+        extrema points in R of the LCFS, wherein P3 is at the IMP and
+        P1 is at the OMP.
+
+        R0 = R(P3) + 0.5*(R(P1)-R(P3))
+        z0 = 0.5*(Z(P1)+Z(P3))
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        
+        Rlcfs = np.array([i[0] for i in separatrix])
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        ind_P1 = np.argmax(Rlcfs)
+        ind_P3 = np.argmin(Rlcfs)
+
+        P1 = np.array([Rlcfs[ind_P1],Zlcfs[ind_P1]])
+        P3 = np.array([Rlcfs[ind_P3],Zlcfs[ind_P3]])
+
+        R0 = P3[0] + 0.5*(P1[0]-P3[0])
+        z0 = 0.5*(P1[1]+P3[1])
+
+        C = np.array([R0,z0])
+
+        return C
+
+    def Rgeometric(self, npoints=360):
+        """Locates major radius R of the geometric major radius.
         """
         return self.geometricAxis(npoints=npoints)[0]
 
-    def minorRadius(self, npoints=20):
-        """Calculates minor radius of plasma as the average distance from the
-        geometric major radius to a number of points along the
-        separatrix
-        """
-        separatrix = self.separatrix(ntheta=npoints)  # [:,2]
-        axis = np.mean(separatrix, axis=0)  # Geometric axis [R,Z]
-
-        # Calculate average distance from the geometric axis
-        return np.mean(
-            np.sqrt(
-                (separatrix[:, 0] - axis[0]) ** 2
-                + (separatrix[:, 1] - axis[1]) ** 2  # dR^2
-            )
-        )  # dZ^2
+    def Zgeometric(self, npoints=360):
+        """Locates the height z of the geometric axis.
+        """
+        return self.geometricAxis(npoints=npoints)[1]
 
-    def geometricElongation(self, npoints=20):
-        """Calculates the elongation of a plasma using the range of R and Z of
-        the separatrix
+    def minorRadius(self, npoints=360):
+        """Calculates minor radius of the plasma, a. First locates the
+        extrema points in R of the LCFS, wherein P3 is at the IMP and
+        P1 is at the OMP.
 
+        a = 0.5*(R(P1) - R(P3))
         """
-        separatrix = self.separatrix(ntheta=npoints)  # [:,2]
-        # Range in Z / range in R
-        return (max(separatrix[:, 1]) - min(separatrix[:, 1])) / (
-            max(separatrix[:, 0]) - min(separatrix[:, 0])
-        )
 
-    def aspectRatio(self, npoints=20):
-        """Calculates the plasma aspect ratio"""
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        
+        Rlcfs = np.array([i[0] for i in separatrix])
+
+        R_P1 = np.max(Rlcfs)
+        R_P3 = np.min(Rlcfs)
+
+        return 0.5*(R_P1 - R_P3)
+
+    def aspectRatio(self, npoints=360):
+        """Calculates the plasma aspect ratio.
+
+        A = R0/a where R0 = major radius, a = minor radius.
+        """
         return self.Rgeometric(npoints=npoints) / self.minorRadius(npoints=npoints)
 
-    def effectiveElongation(self, R_wall_inner, R_wall_outer, npoints=300):
+    def inverseAspectRatio(self, npoints=360):
+        """Calculates inverse of the plasma aspect ratio.
+
+        epsilon = 1/A
+        A = R0/a where R0 = major radius, a = minor radius.
+        """
+        return self.minorRadius(npoints=npoints) / self.Rgeometric(npoints=npoints)
+
+    def elongation(self, npoints=360):
+        """Calculates the elongation, kappa, of the plasma. A large number
+        of points should be supplied such that any primary xpoint(s) on
+        the LCFS are captured. The R,Z of the primary x-point is NOT
+        itself included in the R,Z of the LCFS as the plasma may be limited.
+        P2 is the point at the upper extent of the plasma, and P4 is the point
+        at the lower extent of the plasma.
+
+        kappa = (Z(P2) - Z(P4))/a
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        Z_P2 = np.max(Zlcfs)
+        Z_P4 = np.min(Zlcfs)
+
+        a = self.minorRadius(npoints=npoints)
+
+        return 0.5*(Z_P2 - Z_P4)/a
+
+    def elongationUpper(self, npoints=360):
+        """Calculates the upper elongation, kappa_u, of the plasma. A large number
+        of points should be supplied such that any primary xpoint(s) on
+        the LCFS are captured. The R,Z of the primary x-point is NOT
+        itself included in the R,Z of the LCFS as the plasma may be limited.
+        P2 is the point at the upper extent of the plasma.
+
+        kappa_u = (Z(P2) - z0)/a
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        Z_P2 = np.max(Zlcfs)
+
+        z0 = self.Zgeometric(npoints=npoints)
+        a = self.minorRadius(npoints=npoints)
+
+        return (Z_P2 - z0)/a
+
+    def elongationLower(self, npoints=360):
+        """Calculates the lower elongation, kappa_l, of the plasma. A large number
+        of points should be supplied such that any primary xpoint(s) on
+        the LCFS are captured. The R,Z of the primary x-point is NOT
+        itself included in the R,Z of the LCFS as the plasma may be limited.
+        P2 is the point at the upper extent of the plasma.
+
+        kappa_u = (z0 - Z(P4))/a
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        Z_P4 = np.min(Zlcfs)
+
+        z0 = self.Zgeometric(npoints=npoints)
+        a = self.minorRadius(npoints=npoints)
+
+        return (z0 - Z_P4)/a
+
+    def effectiveElongation(self, npoints=360):
         """Calculates plasma effective elongation using the plasma volume"""
         return self.plasmaVolume() / (
             2.0
             * np.pi
             * self.Rgeometric(npoints=npoints)
             * np.pi
             * self.minorRadius(npoints=npoints) ** 2
         )
 
-    def internalInductance1(self, npoints=300):
+    def triangularityUpper(self, npoints=360):
+        """Calculates plasma upper triangularity, delta_u.
+        P2 is the point at the upper extent of the plasma.
+
+        tri_u = (R0 - R(P2))/a
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        Rlcfs = np.array([i[0] for i in separatrix])
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        ind_P2 = np.argmax(Zlcfs)
+
+        R_P2 = Rlcfs[ind_P2]
+
+        R0 = self.Rgeometric(npoints=npoints)
+        a = self.minorRadius(npoints=npoints)
+
+        return (R0 - R_P2)/a
+
+    def triangularityLower(self, npoints=360):
+        """Calculates plasma upper triangularity, delta_u.
+        P4 is the point at the lower extent of the plasma.
+
+        tri_l = (R0 - R(P4))/a
+        """
+
+        # Get points along the LCFS
+        separatrix = self.separatrix(npoints=npoints)  # Array [:,2]
+        Rlcfs = np.array([i[0] for i in separatrix])
+        Zlcfs = np.array([i[1] for i in separatrix])
+
+        ind_P2 = np.argmax(Zlcfs)
+
+        R_P2 = Rlcfs[ind_P2]
+
+        R0 = self.Rgeometric(npoints=npoints)
+        a = self.minorRadius(npoints=npoints)
+
+        return (R0 - R_P2)/a
+
+    def triangularity(self, npoints=360):
+        """Calculates plasma triangularity, delta.
+
+        Here delta is defined as the average of the upper
+        and lower triangularities.
+        """
+
+        tri_u = self.triangularityUpper(npoints=npoints)
+        tri_l = self.triangularityLower(npoints=npoints)
+
+        return 0.5*(tri_u + tri_l)
+
+    def shafranovShift(self, npoints=360):
+        """Calculates the plasma shafranov shift
+        [delta_shafR,delta_shafZ] where
+
+        delta_shafR = Rmagnetic - Rgeo
+        delta_shafR = Zmagnetic - z0
+        """
+
+        Rmag = self.Rmagnetic()
+        Zmag = self.Zmagnetic()
+
+        Rgeo = self.Rgeometric()
+        z0 = self.Zgeometric()
+
+        return np.array([Rmag-Rgeo,Zmag-z0])
+
+    def internalInductance1(self, npoints=360):
         """Calculates li1 plasma internal inductance"""
 
         R = self.R
         Z = self.Z
         # Produce array of Bpol^2 in (R,Z)
         B_polvals_2 = self.Bz(R, Z) ** 2 + self.Br(R, Z) ** 2
 
@@ -637,15 +961,15 @@
         dV = 2.0 * np.pi * R * dR * dZ
 
         if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         Ip = self.plasmaCurrent()
         R_geo = self.Rgeometric(npoints=npoints)
-        elon = self.geometricElongation(npoints=npoints)
+        elon = self.elongation(npoints=npoints)
         effective_elon = self.effectiveElongation(npoints=npoints)
 
         integral = romb(romb(B_polvals_2 * dV))
         return ((2 * integral) / ((mu0 * Ip) ** 2 * R_geo)) * (
             (1 + elon * elon) / (2.0 * effective_elon)
         )
 
@@ -665,15 +989,15 @@
 
         Ip = self.plasmaCurrent()
         R_mag = self.Rmagnetic()
 
         integral = romb(romb(B_polvals_2 * dV))
         return 2 * integral / ((mu0 * Ip) ** 2 * R_mag)
 
-    def internalInductance3(self, R_wall_inner, R_wall_outer, npoints=300):
+    def internalInductance3(self, npoints=360):
         """Calculates li3 plasma internal inductance"""
 
         R = self.R
         Z = self.Z
         # Produce array of Bpol in (R,Z)
         B_polvals_2 = self.Br(R, Z) ** 2 + self.Bz(R, Z) ** 2
 
@@ -686,52 +1010,125 @@
 
         Ip = self.plasmaCurrent()
         R_geo = self.Rgeometric(npoints=npoints)
 
         integral = romb(romb(B_polvals_2 * dV))
         return 2 * integral / ((mu0 * Ip) ** 2 * R_geo)
 
-    def poloidalBeta2(self):
-        """Calculate plasma poloidal beta by integrating the thermal pressure
-        and poloidal magnetic field pressure over the plasma volume.
+    def internalInductance(self, npoints=360):
+        """Calculates plasma internal inductance li
 
+        li = 4/(mu0*R0*Ip^2) * int(2piR*(Bp^2/2mu0)*dR*dZ)
+           = 2/(mu0^2*R0*Ip^2)*int(2piR*Bp^2*dR*dZ)
         """
 
         R = self.R
         Z = self.Z
+        # Produce array of Bpol in (R,Z)
+        B_polvals_2 = self.Br(R, Z) ** 2 + self.Bz(R, Z) ** 2
+
+        dR = R[1, 0] - R[0, 0]
+        dZ = Z[0, 1] - Z[0, 0]
+        dV = 2.0 * np.pi * R * dR * dZ
+
+        if self.mask is not None:  # Only include points in the core
+            dV *= self.mask
+
+        Ip = self.plasmaCurrent()
+        R_geo = self.Rgeometric(npoints=npoints)
+
+        integral = romb(romb(B_polvals_2 * dV))
+        return 2 * integral / (mu0*mu0*R_geo*Ip*Ip)
+        
+    def poloidalBeta(self):
+        """Calculate plasma poloidal beta by integrating the thermal pressure
+        and poloidal magnetic field pressure over the plasma volume."""
+
+        R = self.R
+        Z = self.Z
 
         # Produce array of Bpol in (R,Z)
         B_polvals_2 = self.Br(R, Z) ** 2 + self.Bz(R, Z) ** 2
 
         dR = R[1, 0] - R[0, 0]
         dZ = Z[0, 1] - Z[0, 0]
         dV = 2.0 * np.pi * R * dR * dZ
 
         # Normalised psi
-        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+        psi_norm = self.psiN()
 
         # Plasma pressure
         pressure = self.pressure(psi_norm)
 
         if self.mask is not None:  # Only include points in the core
             dV *= self.mask
 
         pressure_integral = romb(romb(pressure * dV))
         field_integral_pol = romb(romb(B_polvals_2 * dV))
         return 2 * mu0 * pressure_integral / field_integral_pol
 
-    def toroidalBeta(self):
-        """Calculate plasma toroidal beta by integrating the thermal pressure
-        and toroidal magnetic field pressure over the plasma volume.
+    def poloidalBeta2(self):
+        """ Return the poloidal beta
+        betap = (8pi/mu0) * int(p)dRdZ / Ip^2
+        """
+
+        dR = self.R[1, 0] - self.R[0, 0]
+        dZ = self.Z[0, 1] - self.Z[0, 0]
+
+        # Normalised psi
+        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+
+        # Plasma pressure
+        pressure = self.pressure(psi_norm)
+        if self.mask is not None:
+            # If there is a masking function (X-points, limiters)
+            pressure *= self.mask
+
+        # Integrate pressure in 2D
+        return (
+            ((8.0 * pi) / mu0)
+            * romb(romb(pressure))
+            * dR
+            * dZ
+            / (self.plasmaCurrent() ** 2)
+        )
 
+    def poloidalBeta3(self):
+        """Calculates alterantive poloidal beta definition.
         """
 
         R = self.R
         Z = self.Z
 
+        dR = R[1,0] - R[0,0]
+        dZ = Z[0,1] - Z[0,0]
+        dV = 2.*np.pi * R * dR * dZ
+        
+        # Normalised psi
+        psi_norm = (self.psi() - self.psi_axis)  / (self.psi_bndry - self.psi_axis)
+
+        # Plasma pressure
+        pressure = self.pressure(psi_norm)
+        
+        if self.mask is not None: # Only include points in the core
+            dV *= self.mask
+
+        pressure_integral = romb(romb(pressure * dV))
+        Ip = self.plasmaCurrent()
+        vol = self.plasmaVolume()
+        r0 = self.Rgeometric()
+        return 4 * vol * pressure_integral / (mu0 * Ip * Ip * r0 )
+
+    def toroidalBeta(self):
+        """Calculate plasma toroidal beta by integrating the thermal pressure
+        and toroidal magnetic field pressure over the plasma volume."""
+
+        R = self.R
+        Z = self.Z
+
         # Produce array of Btor in (R,Z)
         B_torvals_2 = self.Btor(R, Z) ** 2
 
         dR = R[1, 0] - R[0, 0]
         dZ = Z[0, 1] - Z[0, 0]
         dV = 2.0 * np.pi * R * dR * dZ
 
@@ -750,15 +1147,92 @@
         np.nan_to_num(B_torvals_2, copy=False)
 
         field_integral_tor = romb(romb(B_torvals_2 * dV))
         return 2 * mu0 * pressure_integral / field_integral_tor
 
     def totalBeta(self):
         """Calculate plasma total beta"""
-        return 1.0 / ((1.0 / self.poloidalBeta2()) + (1.0 / self.toroidalBeta()))
+        return 1.0 / ((1.0 / self.poloidalBeta()) + (1.0 / self.toroidalBeta()))
+
+    def betaN(self, npoints=360):
+        """Calculate normalised plasma beta"""
+        geo = self.geometricAxis()
+        Bt = self.Btor(geo[0],geo[1])
+        return 100.0*1.0e+06*self.toroidalBeta()*( (self.minorRadius()*Bt) / (self.plasmaCurrent()) )
+
+    def pressure_ave(self):
+        """Calculate average pressure, Pa.
+        """
+
+        R = self.R
+        Z = self.Z
+
+        # Produce array of Btor in (R,Z)
+        B_torvals_2 = self.Btor(R, Z) ** 2
+
+        dR = R[1, 0] - R[0, 0]
+        dZ = Z[0, 1] - Z[0, 0]
+        dV = 2.0 * np.pi * R * dR * dZ
+
+        # Normalised psi
+        psi_norm = (self.psi() - self.psi_axis) / (self.psi_bndry - self.psi_axis)
+
+        # Plasma pressure
+        pressure = self.pressure(psi_norm)
+
+        if self.mask is not None:  # Only include points in the core
+            dV *= self.mask
+
+        pressure_integral = romb(romb(pressure * dV))
+        plasmaVolume      = romb(romb(dV))
+
+        return pressure_integral/plasmaVolume
+
+    def w_th(self):
+        """
+        Stored thermal energy in plasma, J.
+        """
+
+        R = self.R
+        Z = self.Z
+
+        dR = R[1,0] - R[0,0]
+        dZ = Z[0,1] - Z[0,0]
+        dV = 2.*np.pi * R * dR * dZ
+        
+        # Normalised psi
+        psi_norm = (self.psi() - self.psi_axis)  / (self.psi_bndry - self.psi_axis)
+        
+        # Plasma pressure
+        pressure = self.pressure(psi_norm)
+
+        if self.mask is not None: # Only include points in the core
+            dV *= self.mask
+
+        pressure_integral = romb(romb(pressure * dV))
+        thermal_energy = (3./2.)*pressure_integral
+
+        return thermal_energy
+
+    def qcyl(self):
+        """
+        Cylindrical safety factor.
+        """
+
+        eps = self.inverseAspectRatio()
+        a = self.minorRadius()
+
+        btor = self.fvac()/self.Rgeometric()
+        Ip = self.plasmaCurrent()
+
+        kappa = self.elongation()
+
+        val = 0.5 * (1 + kappa * kappa) * ((2. * np.pi * a * eps * btor) / (mu0 * Ip))
+
+        return val
 
 
 def refine(eq, nx=None, ny=None):
     """
     Double grid resolution, returning a new equilibrium
 
 
@@ -847,15 +1321,15 @@
     # Create a new equilibrium with the new domain
     result = Equilibrium(
         tokamak=eq.tokamak, Rmin=Rmin, Rmax=Rmax, Zmin=Zmin, Zmax=Zmax, nx=nx, ny=ny
     )
 
     # Calculate the current on the old grid
     profiles = eq._profiles
-    Jtor = profiles.Jtor(eq.R, eq.Z, eq.psi())
+    Jtor = profiles.Jtor(eq.R, eq.Z, eq.psi(), eq.psi_bndry)
 
     # Interpolate Jtor onto new grid
     Jtor_func = interpolate.RectBivariateSpline(eq.R[:, 0], eq.Z[0, :], Jtor)
     Jtor_new = Jtor_func(result.R, result.Z, grid=False)
 
     result._applyBoundary(result, Jtor_new, result.plasma_psi)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `FreeGS-0.6.1/freegs/fieldtracer.py` & `FreeGS-0.7.0/freegs/fieldtracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     ft = FieldTracer(eq)
 
     # Find the edge of the plasma
     psi = eq.psi()
     opoint, xpoint = critical.find_critical(eq.R, eq.Z, psi)
 
     r0, z0, psi_axis = opoint[0]
-    psi_bndry = xpoint[0][2]
+    psi_bndry = eq.psi_bndry #xpoint[0][2]
 
     # Find outboard midplane
     psifunc = interpolate.RectBivariateSpline(
         eq.R[:, 0], eq.Z[0, :], (psi - psi_axis) / (psi_bndry - psi_axis)
     )
 
     rmid, zmid = critical.find_psisurface(
```

### Comparing `FreeGS-0.6.1/freegs/geqdsk.py` & `FreeGS-0.7.0/freegs/geqdsk.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         "rleft": rmin,  # Minimum R in meter of rectangular computational box
         "zmid": 0.5 * (zmin + zmax),
     }  # Z of center of computational box in meter
 
     data["rmagx"], data["zmagx"], data["simagx"] = opoint[0]  # magnetic axis
 
     # Remove Psi magi axis to set it to zero at mag x
-    data["sibdry"] = xpoint[0][2] - data["simagx"]  # Psi at boundary
+    data["sibdry"] = eq.psi_bndry - data["simagx"]  # Psi at boundary
 
     data["cpasma"] = eq.plasmaCurrent()  # Plasma current [A]
 
     psinorm = linspace(0.0, 1.0, nx, endpoint=False)  # Does not include separatrix
 
     data["fpol"] = eq.fpol(psinorm)
     data["pres"] = eq.pressure(psinorm)
```

### Comparing `FreeGS-0.6.1/freegs/gradshafranov.py` & `FreeGS-0.7.0/freegs/gradshafranov.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/jtor.py` & `FreeGS-0.7.0/freegs/jtor.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
-
+import matplotlib.pyplot as plt
 from scipy.integrate import romb, quad  # Romberg integration
 from . import critical
 from .gradshafranov import mu0
 
 from numpy import clip, zeros, reshape, sqrt, pi
 import numpy as np
 
@@ -131,15 +131,15 @@
     Constrain poloidal Beta and plasma current
 
     This is the constraint used in
     YoungMu Jeon arXiv:1503.03135
 
     """
 
-    def __init__(self, betap, Ip, fvac, alpha_m=1.0, alpha_n=2.0, Raxis=1.0):
+    def __init__(self, eq, betap, Ip, fvac, alpha_m=1.0, alpha_n=2.0, Raxis=1.0):
         """
         betap - Poloidal beta
         Ip    - Plasma current [Amps]
         fvac  - Vacuum f = R*Bt
 
         Raxis - R used in p' and ff' components
         """
@@ -153,24 +153,30 @@
         # Set parameters for later use
         self.betap = betap
         self.Ip = Ip
         self._fvac = fvac
         self.alpha_m = alpha_m
         self.alpha_n = alpha_n
         self.Raxis = Raxis
+        self.eq = eq
 
     def Jtor(self, R, Z, psi, psi_bndry=None):
         """Calculate toroidal plasma current
 
         Jtor = L * (Beta0*R/Raxis + (1-Beta0)*Raxis/R)*jtorshape
 
         where jtorshape is a shape function
         L and Beta0 are parameters which are set by constraints
         """
 
+        # Intermediary update of the plasma
+        # boundary and axis flux
+        self.eq._updateBoundaryPsi(psi)
+        psi_bndry = self.eq.psi_bndry
+
         # Analyse the equilibrium, finding O- and X-points
         opt, xpt = critical.find_critical(R, Z, psi)
         if not opt:
             raise ValueError("No O-points found!")
         psi_axis = opt[0][2]
 
         if psi_bndry is not None:
@@ -220,32 +226,40 @@
             for j in range(1, ny - 1):
                 if (psi_norm[i, j] >= 0.0) and (psi_norm[i, j] < 1.0):
                     pfunc[i, j] = pshape(psi_norm[i, j])
         if mask is not None:
             pfunc *= mask
 
         # Integrate over plasma
-        # betap = (8pi/mu0) * int(p)dRdZ / Ip^2
-        #       = - (8pi/mu0) * (L*Beta0/Raxis) * intp / Ip^2
+        # betap = (2mu0) * (int(p)RdRdZ)/(int(B_poloidal**2)RdRdZ)
+        #       = - (2L*Beta0*mu0/Raxis) * (pfunc*RdRdZ)/((int(B_poloidal**2)RdRdZ))
 
-        intp = romb(romb(pfunc)) * dR * dZ
+        # Produce array of Bpol in (R,Z) for core plasma
+        B_polvals_2 = self.eq.Br(R,Z)**2 + self.eq.Bz(R,Z)**2
+        if mask is not None:
+            B_polvals_2 *= mask
 
-        LBeta0 = -self.betap * (mu0 / (8.0 * pi)) * self.Raxis * self.Ip ** 2 / intp
+        p_int = romb(romb(pfunc * R)) * dR*dZ
+        b_int = romb(romb(B_polvals_2 *R)) * dR*dZ
+        
+        #self.betap = - (2*LBeta0*mu0/ self.Raxis) * (p_int/b_int)
+        LBeta0 = (b_int/p_int) * (- self.betap * self.Raxis)/(2*mu0)
 
         # Integrate current components
-        IR = romb(romb(jtorshape * R / self.Raxis)) * dR * dZ
-        I_R = romb(romb(jtorshape * self.Raxis / R)) * dR * dZ
-
+        IR = romb(romb(jtorshape * R/self.Raxis)) * dR*dZ
+        I_R = romb(romb(jtorshape * self.Raxis/R)) * dR*dZ
+        
         # Toroidal plasma current Ip is
         #
         # Ip = L * (Beta0 * IR + (1-Beta0)*I_R)
         #    = L*Beta0*(IR - I_R) + L*I_R
         #
+        #L = self.Ip / ( (Beta0*IR) + ((1.0-Beta0)*(I_R)) )
 
-        L = self.Ip / I_R - LBeta0 * (IR / I_R - 1)
+        L = self.Ip/I_R - LBeta0*(IR/I_R - 1)
         Beta0 = LBeta0 / L
 
         # print("Constraints: L = %e, Beta0 = %e" % (L, Beta0))
 
         # Toroidal current
         Jtor = L * (Beta0 * R / self.Raxis + (1 - Beta0) * self.Raxis / R) * jtorshape
 
@@ -279,15 +293,15 @@
 
 class ConstrainPaxisIp(Profile):
     """
     Constrain pressure on axis and plasma current
 
     """
 
-    def __init__(self, paxis, Ip, fvac, alpha_m=1.0, alpha_n=2.0, Raxis=1.0):
+    def __init__(self, eq, paxis, Ip, fvac, alpha_m=1.0, alpha_n=2.0, Raxis=1.0):
         """
         paxis - Pressure at magnetic axis [Pa]
         Ip    - Plasma current [Amps]
         fvac  - Vacuum f = R*Bt
 
         Raxis - R used in p' and ff' components
         """
@@ -301,24 +315,30 @@
         # Set parameters for later use
         self.paxis = paxis
         self.Ip = Ip
         self._fvac = fvac
         self.alpha_m = alpha_m
         self.alpha_n = alpha_n
         self.Raxis = Raxis
+        self.eq = eq
 
     def Jtor(self, R, Z, psi, psi_bndry=None):
         """Calculate toroidal plasma current
 
         Jtor = L * (Beta0*R/Raxis + (1-Beta0)*Raxis/R)*jtorshape
 
         where jtorshape is a shape function
         L and Beta0 are parameters which are set by constraints
         """
 
+        # Intermediary update of the plasma
+        # boundary and axis flux
+        self.eq._updateBoundaryPsi(psi)
+        psi_bndry = self.eq.psi_bndry
+
         # Analyse the equilibrium, finding O- and X-points
         opt, xpt = critical.find_critical(R, Z, psi)
         if not opt:
             raise ValueError("No O-points found!")
         psi_axis = opt[0][2]
 
         if psi_bndry is not None:
```

### Comparing `FreeGS-0.6.1/freegs/machine.py` & `FreeGS-0.7.0/freegs/machine.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .gradshafranov import Greens, GreensBr, GreensBz
 
 from numpy import linspace
 import numpy as np
+from scipy.interpolate import interp1d
 
 from .coil import Coil, AreaCurrentLimit
 from .shaped_coil import ShapedCoil
-from .multi_coil import MultiCoil
+from .pre_calc_coil import PreCalcCoil
+from .filament_coil import FilamentCoil
 
 # We need this for the `label` part of the Circuit dtype for writing
 # to HDF5 files. See the following for information:
 # http://docs.h5py.org/en/latest/strings.html#how-to-store-text-strings
 try:
     import h5py
 
@@ -456,14 +458,19 @@
     def __init__(self, coils, wall=None):
         """
         coils - A list of coils [(label, Coil|Circuit|Solenoid)]
         """
 
         self.coils = coils
         self.wall = wall
+        self.limit_points_R = None
+        self.limit_points_Z = None
+
+        if self.wall is not None:
+            self.limit_points_R, self.limit_points_Z = self.generate_limit_points()
 
     def __repr__(self):
         return "Machine(coils={coils}, wall={wall})".format(
             coils=self.coils, wall=self.wall
         )
 
     def __eq__(self, other):
@@ -476,14 +483,36 @@
 
     def __getitem__(self, name):
         for label, coil in self.coils:
             if label == name:
                 return coil
         raise KeyError("Machine does not contain coil with label '{0}'".format(name))
 
+    def generate_limit_points(self):
+        '''
+        Generate points along the machine wall that may be used to check
+        if the plasma is limited or not.
+        '''
+
+        # Interpolate wall limit points (get_divcoords typically only return 8 or so points)
+        # Make an interpolator for point location as function of normalised distance
+        # along the wall
+        points = np.array([self.wall.R,self.wall.Z]).T
+        distance = np.cumsum(np.sqrt(np.sum(np.diff(points,axis=0)**2,axis=1)))
+        distance = np.insert(distance,0,0)/distance[-1]
+
+        interpolator = interp1d(distance,points,kind='linear',axis=0)
+        new_distances = np.linspace(0,1,500,endpoint=True)
+        interpolated_points = interpolator(new_distances)
+
+        R = np.asarray(interpolated_points[:,0])
+        Z = np.asarray(interpolated_points[:,1])
+
+        return R, Z
+
     def psi(self, R, Z):
         """
         Poloidal flux due to coils
         """
         psi_coils = 0.0
         for label, coil in self.coils:
             psi_coils += coil.psi(R, Z)
@@ -650,14 +679,35 @@
 
     wall = Wall(
         [0.75, 0.75, 1.5, 1.8, 1.8, 1.5], [-0.85, 0.85, 0.85, 0.25, -0.25, -0.85]  # R
     )  # Z
 
     return Machine(coils, wall)
 
+def TestTokamakLimited():
+    """
+    Create a simple tokamak
+    """
+
+    coils = [
+        (
+            "P1L",
+            ShapedCoil([(0.95, -1.15), (0.95, -1.05), (1.05, -1.05), (1.05, -1.15)]),
+        ),
+        ("P1U", ShapedCoil([(0.95, 1.15), (0.95, 1.05), (1.05, 1.05), (1.05, 1.15)])),
+        ("P2L", Coil(1.75, -0.6)),
+        ("P2U", Coil(1.75, 0.6)),
+    ]
+
+    wall = Wall(
+        [0.93, 0.93, 1.5, 1.8, 1.8, 1.5], [-0.85, 0.85, 0.85, 0.25, -0.25, -0.85]  # R
+    )  # Z
+
+    return Machine(coils, wall)
+
 
 def DIIID():
     """
     PF coil set from ef20030203.d3d
     Taken from Corsica
     """
 
@@ -787,15 +837,15 @@
     return Machine(coils)
 
 
 def MASTU_simple():
     """This is an older version of the MAST-U coilset.
     A simplified set of coils, with one strand per coil.
     This may be easier to use for initial development of scenarios,
-    but less detailed than the MultiCoil description (MASTU).
+    but less detailed than the FilamentCoil description (MASTU).
     """
     coils = [
         ("Solenoid", Solenoid(0.19475, -1.581, 1.581, 324)),
         # ("Pc", Coil(0.067, 0.0, turns=142)),
         ("Pc", Solenoid(0.067, -0.6, 0.6, 142)),
         (
             "Px",
@@ -1036,19 +1086,19 @@
     rwall = rwall + rwall[::-1]
     zwall = zwall + [-z for z in zwall[::-1]]
 
     return Machine(coils, Wall(rwall, zwall))
 
 
 #########################################
-# MAST-U, using MultiCoil to represent multiple strands
+# MAST-U, using FilamentCoil to represent multiple strands
 
 
 def MASTU():
-    """MAST-Upgrade, using MultiCoil to represent coils with different locations
+    """MAST-Upgrade, using FilamentCoil to represent coils with different locations
     for each strand.
     """
     d1_upper_r = [
         0.35275,
         0.36745015,
         0.38215014,
         0.39685005,
@@ -2259,111 +2309,111 @@
         7.25515604e-01,
         7.47515619e-01,
         7.69516051e-01,
     ]
 
     coils = [
         ("Solenoid", Solenoid(0.19475, -1.581, 1.581, 324, control=False)),
-        ("Pc", MultiCoil(pc_r, pc_z)),
+        ("Pc", FilamentCoil(pc_r, pc_z)),
         (
             "Px",
             Circuit(
                 [
-                    ("PxU", MultiCoil(px_upper_r, px_upper_z), 1.0),
-                    ("PxL", MultiCoil(px_upper_r, px_lower_z), 1.0),
+                    ("PxU", FilamentCoil(px_upper_r, px_upper_z), 1.0),
+                    ("PxL", FilamentCoil(px_upper_r, px_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D1",
             Circuit(
                 [
-                    ("D1U", MultiCoil(d1_upper_r, d1_upper_z), 1.0),
-                    ("D1L", MultiCoil(d1_upper_r, d1_lower_z), 1.0),
+                    ("D1U", FilamentCoil(d1_upper_r, d1_upper_z), 1.0),
+                    ("D1L", FilamentCoil(d1_upper_r, d1_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D2",
             Circuit(
                 [
-                    ("D2U", MultiCoil(d2_upper_r, d2_upper_z), 1.0),
-                    ("D2L", MultiCoil(d2_upper_r, d2_lower_z), 1.0),
+                    ("D2U", FilamentCoil(d2_upper_r, d2_upper_z), 1.0),
+                    ("D2L", FilamentCoil(d2_upper_r, d2_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D3",
             Circuit(
                 [
-                    ("D3U", MultiCoil(d3_upper_r, d3_upper_z), 1.0),
-                    ("D3L", MultiCoil(d3_upper_r, d3_lower_z), 1.0),
+                    ("D3U", FilamentCoil(d3_upper_r, d3_upper_z), 1.0),
+                    ("D3L", FilamentCoil(d3_upper_r, d3_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "Dp",
             Circuit(
                 [
-                    ("DPU", MultiCoil(dp_upper_r, dp_upper_z), 1.0),
-                    ("DPL", MultiCoil(dp_upper_r, dp_lower_z), 1.0),
+                    ("DPU", FilamentCoil(dp_upper_r, dp_upper_z), 1.0),
+                    ("DPL", FilamentCoil(dp_upper_r, dp_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D5",
             Circuit(
                 [
-                    ("D5U", MultiCoil(d5_upper_r, d5_upper_z), 1.0),
-                    ("D5L", MultiCoil(d5_upper_r, d5_lower_z), 1.0),
+                    ("D5U", FilamentCoil(d5_upper_r, d5_upper_z), 1.0),
+                    ("D5L", FilamentCoil(d5_upper_r, d5_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D6",
             Circuit(
                 [
-                    ("D6U", MultiCoil(d6_upper_r, d6_upper_z), 1.0),
-                    ("D6L", MultiCoil(d6_upper_r, d6_lower_z), 1.0),
+                    ("D6U", FilamentCoil(d6_upper_r, d6_upper_z), 1.0),
+                    ("D6L", FilamentCoil(d6_upper_r, d6_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "D7",
             Circuit(
                 [
-                    ("D7U", MultiCoil(d7_upper_r, d7_upper_z), 1.0),
-                    ("D7L", MultiCoil(d7_upper_r, d7_lower_z), 1.0),
+                    ("D7U", FilamentCoil(d7_upper_r, d7_upper_z), 1.0),
+                    ("D7L", FilamentCoil(d7_upper_r, d7_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "P4",
             Circuit(
                 [
-                    ("P4U", MultiCoil(p4_upper_r, p4_upper_z), 1.0),
-                    ("P4L", MultiCoil(p4_upper_r, p4_lower_z), 1.0),
+                    ("P4U", FilamentCoil(p4_upper_r, p4_upper_z), 1.0),
+                    ("P4L", FilamentCoil(p4_upper_r, p4_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "P5",
             Circuit(
                 [
-                    ("P5U", MultiCoil(p5_upper_r, p5_upper_z), 1.0),
-                    ("P5L", MultiCoil(p5_upper_r, p5_lower_z), 1.0),
+                    ("P5U", FilamentCoil(p5_upper_r, p5_upper_z), 1.0),
+                    ("P5L", FilamentCoil(p5_upper_r, p5_lower_z), 1.0),
                 ]
             ),
         ),
         (
             "P6",
             Circuit(
                 [
-                    ("P6U", MultiCoil(p6_upper_r, p6_upper_z), 1.0),
-                    ("P6L", MultiCoil(p6_upper_r, p6_lower_z), -1.0),
+                    ("P6U", FilamentCoil(p6_upper_r, p6_upper_z), 1.0),
+                    ("P6L", FilamentCoil(p6_upper_r, p6_lower_z), -1.0),
                 ]
             ),
         ),
     ]
 
     rwall = [
         1.6,
```

### Comparing `FreeGS-0.6.1/freegs/multi_coil.py` & `FreeGS-0.7.0/freegs/shaped_coil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
-Classes and routines to represent coils and circuits
+Define a class of coil which contains a uniform current density
+over a shaped region.
 
 License
 -------
 
-Copyright 2019 Chris Marsden, Tokamak Energy. Email: Chris.Marsden@tokamakenergy.co.uk
+Copyright 2019 Ben Dudson, University of York. Email: benjamin.dudson@york.ac.uk
 
 This file is part of FreeGS.
 
 FreeGS is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -18,204 +19,190 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import numpy as np
-from .coil import Coil, AreaCurrentLimit
+from . import quadrature
+from . import polygons
 from .gradshafranov import Greens, GreensBr, GreensBz
 
+import numpy as np
+
+from .coil import Coil
+
 
-class MultiCoil(Coil):
+class ShapedCoil(Coil):
     """
-    This class is multifunctional and can model several coil arrangements:
-    1. A single PF coil
-    2. A block of several PF coil filaments, modelled as
-        a) a single point in (R,Z)
-        b) a list of (R,Z) points for each filament in the block
-
-    In both cases, the specified coil(s) can also be mirrored in Z=0 and
-    connected in a circuit sharing the same power supply. In such a case,
-    there is also the option to specify the polarity of the currents in
-    the upper and lower coil blocks, enabling the wiring of these blocks
-    in opposite directions.
+    Represents a coil with a specified shape
 
     public members
     --------------
 
     R, Z - Location of the point coil/Locations of coil filaments
     current - current in the coil(s) in Amps
     turns   - Number of turns if using point coils
     control - enable or disable control system
-    mirror - enable or disable mirroring of coil block in Z=0
-    polarity - wiring of coil blocks in circuit
     area    - Cross-section area in m^2
 
-    For multiple point coils, the total toroidal current carried by the
-    point coil block is current * turns
+    The total toroidal current carried by the coil block is current * turns
     """
 
     # A dtype for converting to Numpy array and storing in HDF5 files
     dtype = np.dtype(
         [
-            (str("RZlen"), int),  # Length of R and Z arrays
-            (str("R"), "500f8"),  # Up to 100 points
-            (str("Z"), "500f8"),
+            (str("RZlen"), int),  # Length of the R and Z arrays
+            (str("R"), "10f8"),  # Note: Up to 10 points
+            (str("Z"), "10f8"),  # Note: Up to 10 points
             (str("current"), np.float64),
             (str("turns"), int),
             (str("control"), bool),
-            (str("mirror"), bool),
-            (str("polarity"), "2f8"),
+            (str("npoints"), int),
         ]
     )
 
-    def __init__(
-        self,
-        R,
-        Z,
-        current=0.0,
-        turns=1,
-        control=True,
-        mirror=False,
-        polarity=[1.0, 1.0],
-        area=AreaCurrentLimit(),
-    ):
-        """
-        R, Z       - Location of the coil centre. If modified moves all filaments
-        Rfil, Zfil - Locations of coil filaments (lists)
-
-        current - current in each turn of the coil in Amps
-        turns   - Number of turns in point coil(s) block. Total block current is current * turns
-                  This is only used if R,Z are a single point
-        control - enable or disable control system
-        mirror - mirror the point/detailed coil block in Z=0, creating a circuit
-        polarity - Wiring of the circuit: same or opposite direction, [Block 1, Block 2]
-        area    - Cross-section area of block in m^2
-
-        Area can be a fixed value (e.g. 0.025 for 5x5cm coil), or can be specified
-        using a function which takes a coil as an input argument.
-        To specify a current density limit, use:
-
-        area = AreaCurrentLimit(current_density)
-
-        where current_density is in A/m^2. The area of the coil will be recalculated
-        as the coil current is changed.
-
-        The most important effect of the area is on the coil self-force:
-        The smaller the area the larger the hoop force for a given current.
-        """
-        # Store locations as an internal list
-        if hasattr(R, "__len__"):
-            assert len(R) == len(Z)
-            self.Rfil = R
-            self.Zfil = Z
-            self.turns = len(R)
-        else:
-            # Assume a single R, Z. Turn into a list
-            self.Rfil = [R]
-            self.Zfil = [Z]
-            self.turns = turns
+    def __init__(self, shape, current=0.0, turns=1, control=True, npoints=6):
+        """
+        Inputs
+        ------
+        shape     outline of the coil shape as a list of points [(r1,z1), (r2,z2), ...]
+                  Must have more than two points
+        current   The current in the circuit. The total current is current * turns
+        turns     Number of turns in point coil(s) block. Total block current is current * turns
+        control   enable or disable control system
+        npoints   Number of quadrature points per triangle. Valid choices: 1, 3, 6
+
+        """
+        assert len(shape) > 2
+
+        # Find the geometric middle of the coil
+        # The R,Z properties have accessor functions to handle modifications
+        self._R_centre = sum(r for r, z in shape) / len(shape)
+        self._Z_centre = sum(z for r, z in shape) / len(shape)
 
         self.current = current
+        self.turns = turns
         self.control = control
-        self.mirror = mirror
-        self.polarity = polarity
-        self.area = area
-
-        # Internal (R,Z) value, should not be modified directly
-        self._R_centre = np.mean(self.Rfil)
-        self._Z_centre = np.mean(self.Zfil)
+        self._area = abs(polygons.area(shape))
+        self.shape = shape
+
+        # The quadrature points to be used
+        self.npoints_per_triangle = npoints
+        self._points = quadrature.polygon_quad(shape, n=npoints)
 
     def controlPsi(self, R, Z):
         """
         Calculate poloidal flux at (R,Z) due to a unit current
         """
-
         result = 0.0
-        for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-            result += Greens(R_fil, Z_fil, R, Z) * self.polarity[0]
-
-        if self.mirror:
-            for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-                result += Greens(R_fil, -Z_fil, R, Z) * self.polarity[1]
+        for R_fil, Z_fil, weight in self._points:
+            result += Greens(R_fil, Z_fil, R, Z) * weight
         return result
 
     def controlBr(self, R, Z):
         """
         Calculate radial magnetic field Br at (R,Z) due to a unit current
         """
         result = 0.0
-        for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-            result += GreensBr(R_fil, Z_fil, R, Z) * self.polarity[0]
-
-        if self.mirror:  # Mirror coil(s) in Z, creating circuit
-            for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-                result += GreensBr(R_fil, -Z_fil, R, Z) * self.polarity[1]
+        for R_fil, Z_fil, weight in self._points:
+            result += GreensBr(R_fil, Z_fil, R, Z) * weight
         return result
 
     def controlBz(self, R, Z):
         """
         Calculate vertical magnetic field Bz at (R,Z) due to a unit current
         """
         result = 0.0
-        for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-            result += GreensBz(R_fil, Z_fil, R, Z) * self.polarity[0]
-
-        if self.mirror:  # Mirror coil(s) in Z, creating circuit
-            for R_fil, Z_fil in zip(self.Rfil, self.Zfil):
-                result += GreensBz(R_fil, -Z_fil, R, Z) * self.polarity[1]
+        for R_fil, Z_fil, weight in self._points:
+            result += GreensBz(R_fil, Z_fil, R, Z) * weight
         return result
 
     def __repr__(self):
-        return "MultiCoil(R={0}, Z={1}, current={2:.1f}, turns={3}, control={4}, mirror={5}, polarity={6})".format(
-            self.Rfil,
-            self.Zfil,
-            self.current,
-            self.turns,
-            self.control,
-            self.mirror,
-            self.polarity,
+        return "ShapedCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
+            self.shape, self.current, self.turns, self.control
         )
 
-    def __eq__(self, other):
-        return (
-            self.R == other.R
-            and self.Z == other.Z
-            and self.current == other.current
-            and self.turns == other.turns
-            and self.control == other.control
-        )
+    @property
+    def R(self):
+        """
+        Major radius of the coil in m
+        """
+        return self._R_centre
 
-    def __ne__(self, other):
-        return not self == other
+    @R.setter
+    def R(self, Rnew):
+        # Need to shift all points
+        Rshift = Rnew - self._R_centre
+        self._points = [(r + Rshift, z, w) for r, z, w in self._points]
+        self._R_centre = Rnew
+
+    @property
+    def Z(self):
+        """
+        Height of the coil in m
+        """
+        return self._Z_centre
+
+    @Z.setter
+    def Z(self, Znew):
+        # Need to shift all points
+        Zshift = Znew - self._Z_centre
+        self._points = [(r, z + Zshift, w) for r, z, w in self._points]
+        self._Z_centre = Znew
+
+    @property
+    def area(self):
+        return self._area
+
+    @area.setter
+    def area(self, area):
+        raise ValueError("Area of a ShapedCoil is fixed")
+
+    def plot(self, axis=None, show=False):
+        """
+        Plot the coil shape, using axis if given
+        """
+        import matplotlib.pyplot as plt
+
+        if axis is None:
+            fig = plt.figure()
+            axis = fig.add_subplot(111)
+
+        r = [r for r, z in self.shape]
+        z = [z for r, z in self.shape]
+        axis.fill(r, z, color="gray")
+        axis.plot(r, z, color="black")
+
+        # Quadrature points
+        # rquad = [r for r,z,w in self._points]
+        # zquad = [z for r,z,w in self._points]
+        # axis.plot(rquad, zquad, 'ro')
+
+        return axis
 
     def to_numpy_array(self):
         """
         Helper method for writing output
         """
-
-        RZlen = len(self.Rfil)
-        assert RZlen <= 500
-        R = np.zeros(500)
-        Z = np.zeros(500)
-        R[:RZlen] = self.Rfil
-        Z[:RZlen] = self.Zfil
+        RZlen = len(self.shape)
+        R = np.zeros(10)
+        Z = np.zeros(10)
+        R[:RZlen] = [R for R, Z in self.shape]
+        Z[:RZlen] = [Z for R, Z in self.shape]
 
         return np.array(
             (
                 RZlen,
                 R,
                 Z,
                 self.current,
                 self.turns,
                 self.control,
-                self.mirror,
-                self.polarity,
+                self.npoints_per_triangle,
             ),
             dtype=self.dtype,
         )
 
     @classmethod
     def from_numpy_array(cls, value):
         if value.dtype != cls.dtype:
@@ -226,63 +213,28 @@
             )
         RZlen = value["RZlen"]
         R = value["R"][:RZlen]
         Z = value["Z"][:RZlen]
         current = value["current"]
         turns = value["turns"]
         control = value["control"]
-        mirror = value["npoints"]
-        polarity = value["polarity"]
+        npoints = value["npoints"]
 
-        return MultiCoil(
-            R,
-            Z,
+        return ShapedCoil(
+            list(zip(R, Z)),
             current=current,
             turns=turns,
             control=control,
-            mirror=mirror,
-            polarity=polarity,
+            npoints=npoints,
         )
 
-    def plot(self, axis=None, show=False):
-        """
-        Plot the coil including turn locations
-        """
-        import matplotlib.pyplot as plt
-
-        if axis is None:
-            fig = plt.figure()
-            axis = fig.add_subplot(111)
-
-        plt.plot(self.Rfil, self.Zfil, "bo")
-
-        return axis
-
-    @property
-    def R(self):
-        """
-        Major radius of the coil in m
-        """
-        return self._R_centre
-
-    @R.setter
-    def R(self, Rnew):
-        # Need to shift all points
-        Rshift = Rnew - self._R_centre
-        for i in range(len(self.Rfil)):
-            self.Rfil[i] += Rshift
-        self._R_centre = Rnew
-
-    @property
-    def Z(self):
-        """
-        Height of the coil in m
-        """
-        return self._Z_centre
+    def __eq__(self, other):
+        return (
+            np.allclose(self.shape, other.shape)
+            and self.current == other.current
+            and self.turns == other.turns
+            and self.control == other.control
+            and self.npoints_per_triangle == other.npoints_per_triangle
+        )
 
-    @Z.setter
-    def Z(self, Znew):
-        # Need to shift all points
-        Zshift = Znew - self._Z_centre
-        for i in range(len(self.Zfil)):
-            self.Zfil[i] += Zshift
-        self._Z_centre = Znew
+    def __ne__(self, other):
+        return not self == other
```

### Comparing `FreeGS-0.6.1/freegs/multigrid.py` & `FreeGS-0.7.0/freegs/multigrid.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/optimise.py` & `FreeGS-0.7.0/freegs/optimise.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/optimiser.py` & `FreeGS-0.7.0/freegs/optimiser.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/plotting.py` & `FreeGS-0.7.0/freegs/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     if axis is None:
         fig = plt.figure()
         axis = fig.add_subplot(111)
 
     return axis
 
-
 def plotConstraints(control, axis=None, show=True):
     """
     Plots constraints used for coil current control
 
     axis     - Specify the axis on which to plot
     show     - Call matplotlib.pyplot.show() before returning
 
@@ -65,15 +64,14 @@
 
     if show:
         plt.legend()
         plt.show()
 
     return axis
 
-
 def plotEquilibrium(eq, axis=None, show=True, oxpoints=True, wall=True):
     """
     Plot the equilibrium flux surfaces
 
     axis     - Specify the axis on which to plot
     show     - Call matplotlib.pyplot.show() before returning
     oxpoints - Plot X points as red circles, O points as green circles
@@ -104,15 +102,15 @@
 
         for r, z, _ in xpt:
             axis.plot(r, z, "ro")
         for r, z, _ in opt:
             axis.plot(r, z, "go")
 
         if xpt:
-            psi_bndry = xpt[0][2]
+            psi_bndry = eq.psi_bndry #xpt[0][2]
             axis.contour(eq.R, eq.Z, psi, levels=[psi_bndry], colors="r")
 
             # Add legend
             axis.plot([], [], "ro", label="X-points")
             axis.plot([], [], "r", label="Separatrix")
         if opt:
             axis.plot([], [], "go", label="O-points")
```

### Comparing `FreeGS-0.6.1/freegs/polygons.py` & `FreeGS-0.7.0/freegs/polygons.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/quadrature.py` & `FreeGS-0.7.0/freegs/quadrature.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/shaped_coil.py` & `FreeGS-0.7.0/freegs/pre_calc_coil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-Define a class of coil which contains a uniform current density
-over a shaped region.
+Classes and routines to represent coils and circuits
 
 License
 -------
 
-Copyright 2019 Ben Dudson, University of York. Email: benjamin.dudson@york.ac.uk
+Copyright 2022 Chris Marsden, Tokamak Energy. Email: chris.marsden@tokamakenergy.co.uk
 
 This file is part of FreeGS.
 
 FreeGS is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -19,162 +18,188 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with FreeGS.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-from . import quadrature
-from . import polygons
-from .gradshafranov import Greens, GreensBr, GreensBz
-
 import numpy as np
-
-from .coil import Coil
+from .coil import Coil, AreaCurrentLimit
+from .gradshafranov import Greens, GreensBr, GreensBz
 
 
-class ShapedCoil(Coil):
+class PreCalcCoil(Coil):
     """
-    Represents a coil with a specified shape
+    This class represents a coil whose Green's functions have
+    already been calculate by some external code. This is useful
+    in modelling coils whose internal structure may be complex and
+    whose current distribution may be highly non-uniform.
+
+    The user needs to supply information on the R,Z grids that the
+    Green's functions have been pre-calculated on, as well as the
+    Br, Bz and psi data on said R,Z grid.
 
     public members
     --------------
 
-    R, Z - Location of the point coil/Locations of coil filaments
-    current - current in the coil(s) in Amps
-    turns   - Number of turns if using point coils
+    R, Z    - Location of the coil
+    current - current in the coil in Amps
+    turns   - Number of turns
     control - enable or disable control system
     area    - Cross-section area in m^2
 
-    The total toroidal current carried by the coil block is current * turns
+    The total toroidal current carried by the coil is current * turns
     """
 
     # A dtype for converting to Numpy array and storing in HDF5 files
     dtype = np.dtype(
         [
             (str("RZlen"), int),  # Length of the R and Z arrays
             (str("R"), "10f8"),  # Note: Up to 10 points
             (str("Z"), "10f8"),  # Note: Up to 10 points
             (str("current"), np.float64),
             (str("turns"), int),
             (str("control"), bool),
-            (str("npoints"), int),
         ]
     )
 
-    def __init__(self, shape, current=0.0, turns=1, control=True, npoints=6):
+    def __init__(self, shape, Rgrid, Zgrid, mapBr, mapBz, mapPsi, current=0.0, turns=1, control=True):
         """
         Inputs
         ------
-        shape     outline of the coil shape as a list of points [(r1,z1), (r2,z2), ...]
-                  Must have more than two points
-        current   The current in the circuit. The total current is current * turns
-        turns     Number of turns in point coil(s) block. Total block current is current * turns
-        control   enable or disable control system
-        npoints   Number of quadrature points per triangle. Valid choices: 1, 3, 6
+        shape  - outline of the coil shape as a list of points [(r1,z1), (r2,z2), ...]
+                 Must have more than two points
+
+        Rgrid   - 1D array of R coords that maps are calculated on.
+        Zgrid   - 1D array of Z coords that maps are calculated on.
+        mapBr   - 1D array of Br calculated on Rgrid,Zgrid for the coil @ 1A-turn.
+        mapBz   - 1D array of Bz calculated on Rgrid,Zgrid for the coil @ 1A-turn.
+        mapPsi  - 1D array of Psi calculated on Rgrid,Zgrid for the coil @ 1A-turn.
+        current - The current in the circuit. The total current is current * turns.
+        turns   - Number of turns in point coil(s) block. Total block current is current * turns.
+        control - Enable or disable control system.
 
         """
         assert len(shape) > 2
 
         # Find the geometric middle of the coil
         # The R,Z properties have accessor functions to handle modifications
         self._R_centre = sum(r for r, z in shape) / len(shape)
         self._Z_centre = sum(z for r, z in shape) / len(shape)
 
         self.current = current
-        self.turns = turns
+        self.turns   = turns
         self.control = control
-        self._area = abs(polygons.area(shape))
-        self.shape = shape
-
-        # The quadrature points to be used
-        self.npoints_per_triangle = npoints
-        self._points = quadrature.polygon_quad(shape, n=npoints)
+        self._area   = abs(polygons.area(shape))
+        self.shape   = shape
+        self._points = np.array([(r,z) for r, z in self.shape])
+
+        # Data for the pre-calculated Green's functions
+        self.Rgrid   = np.transpose(Rgrid)[:,0]
+        self.Zgrid   = np.transpose(Zgrid)[0,:]
+        self.map_psi = np.transpose(np.asarray(map_psi))
+        self.map_Br  = np.transpose(np.asarray(map_Br))
+        self.map_Bz  = np.transpose(np.asarray(map_Bz))
+
+        # Interpolators for the pre-calculated Green's functions
+        self.cPsi = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapPsi)
+        self.cBr  = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapBr)
+        self.cBz  = RectBivariateSpline(self.Rgrid,self.Zgrid,self.mapBz)
 
     def controlPsi(self, R, Z):
         """
-        Calculate poloidal flux at (R,Z) due to a unit current
+        Calculate poloidal flux at (R,Z) due to a unit current.
         """
-        result = 0.0
-        for R_fil, Z_fil, weight in self._points:
-            result += Greens(R_fil, Z_fil, R, Z) * weight
+        
+        if isinstance(R,float) or isinstance(R,int):
+            result = self.cPsi(R,Z)[0][0]
+        else:
+            result = self.cPsi(R,Z,grid=False)
+
         return result
 
     def controlBr(self, R, Z):
         """
-        Calculate radial magnetic field Br at (R,Z) due to a unit current
+        Calculate radial magnetic field Br at (R,Z) due to a unit current.
         """
-        result = 0.0
-        for R_fil, Z_fil, weight in self._points:
-            result += GreensBr(R_fil, Z_fil, R, Z) * weight
+        
+        if isinstance(R,float) or isinstance(R,int):
+            result = self.cBr(R,Z)[0][0]
+        else:
+            result = self.cBr(R,Z,grid=False)
+
         return result
 
     def controlBz(self, R, Z):
         """
-        Calculate vertical magnetic field Bz at (R,Z) due to a unit current
+        Calculate vertical magnetic field Br at (R,Z) due to a unit current.
         """
-        result = 0.0
-        for R_fil, Z_fil, weight in self._points:
-            result += GreensBz(R_fil, Z_fil, R, Z) * weight
+        
+        if isinstance(R,float) or isinstance(R,int):
+            result = self.cBz(R,Z)[0][0]
+        else:
+            result = self.cBz(R,Z,grid=False)
+
         return result
 
     def __repr__(self):
-        return "ShapedCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
+        return "PreCalcCoil({0}, current={1:.1f}, turns={2}, control={3})".format(
             self.shape, self.current, self.turns, self.control
         )
 
     @property
     def R(self):
         """
         Major radius of the coil in m
         """
         return self._R_centre
 
     @R.setter
     def R(self, Rnew):
         # Need to shift all points
         Rshift = Rnew - self._R_centre
-        self._points = [(r + Rshift, z, w) for r, z, w in self._points]
+        self._points = [(r + Rshift, z) for r, z in self._points]
         self._R_centre = Rnew
 
     @property
     def Z(self):
         """
         Height of the coil in m
         """
         return self._Z_centre
 
     @Z.setter
     def Z(self, Znew):
         # Need to shift all points
         Zshift = Znew - self._Z_centre
-        self._points = [(r, z + Zshift, w) for r, z, w in self._points]
+        self._points = [(r, z + Zshift) for r, z in self._points]
         self._Z_centre = Znew
 
     @property
     def area(self):
         return self._area
 
     @area.setter
     def area(self, area):
-        raise ValueError("Area of a ShapedCoil is fixed")
+        raise ValueError("Area of a PreCalcCoil is fixed")
 
     def plot(self, axis=None, show=False):
         """
         Plot the coil shape, using axis if given
         """
         import matplotlib.pyplot as plt
 
         if axis is None:
             fig = plt.figure()
             axis = fig.add_subplot(111)
 
         r = [r for r, z in self.shape]
         z = [z for r, z in self.shape]
-        axis.fill(r, z, color="blue")
+        axis.fill(r, z, color="gray")
+        axis.plot(r, z, color="black")
 
         # Quadrature points
         # rquad = [r for r,z,w in self._points]
         # zquad = [z for r,z,w in self._points]
         # axis.plot(rquad, zquad, 'ro')
 
         return axis
@@ -192,48 +217,14 @@
         return np.array(
             (
                 RZlen,
                 R,
                 Z,
                 self.current,
                 self.turns,
-                self.control,
-                self.npoints_per_triangle,
+                self.control
             ),
             dtype=self.dtype,
         )
 
-    @classmethod
-    def from_numpy_array(cls, value):
-        if value.dtype != cls.dtype:
-            raise ValueError(
-                "Can't create {this} from dtype: {got} (expected: {dtype})".format(
-                    this=type(cls), got=value.dtype, dtype=cls.dtype
-                )
-            )
-        RZlen = value["RZlen"]
-        R = value["R"][:RZlen]
-        Z = value["Z"][:RZlen]
-        current = value["current"]
-        turns = value["turns"]
-        control = value["control"]
-        npoints = value["npoints"]
-
-        return ShapedCoil(
-            list(zip(R, Z)),
-            current=current,
-            turns=turns,
-            control=control,
-            npoints=npoints,
-        )
-
-    def __eq__(self, other):
-        return (
-            np.allclose(self.shape, other.shape)
-            and self.current == other.current
-            and self.turns == other.turns
-            and self.control == other.control
-            and self.npoints_per_triangle == other.npoints_per_triangle
-        )
-
     def __ne__(self, other):
         return not self == other
```

### Comparing `FreeGS-0.6.1/freegs/test_aeqdsk.py` & `FreeGS-0.7.0/freegs/test_aeqdsk.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_critical.py` & `FreeGS-0.7.0/freegs/test_critical.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_equilibrium.py` & `FreeGS-0.7.0/freegs/test_equilibrium.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_fileutils.py` & `FreeGS-0.7.0/freegs/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_geqdsk.py` & `FreeGS-0.7.0/freegs/test_geqdsk.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_jtor.py` & `FreeGS-0.7.0/freegs/test_jtor.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_linearsolve.py` & `FreeGS-0.7.0/freegs/test_linearsolve.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_machine.py` & `FreeGS-0.7.0/freegs/test_machine.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_multi_coil.py` & `FreeGS-0.7.0/freegs/test_multi_coil.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_optimise.py` & `FreeGS-0.7.0/freegs/test_optimise.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_optimiser.py` & `FreeGS-0.7.0/freegs/test_optimiser.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_polygons.py` & `FreeGS-0.7.0/freegs/test_polygons.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_quadrature.py` & `FreeGS-0.7.0/freegs/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_readwrite.py` & `FreeGS-0.7.0/freegs/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/freegs/test_shaped_coil.py` & `FreeGS-0.7.0/freegs/test_shaped_coil.py`

 * *Files identical despite different names*

### Comparing `FreeGS-0.6.1/setup.py` & `FreeGS-0.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     license="LGPL",
     author="Ben Dudson",
     author_email='benjamin.dudson@york.ac.uk',
     url="https://github.com/bendudson/freegs",
     description="Free boundary Grad-Shafranov solver for tokamak plasma equilibria",
 
     long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     
     install_requires=['numpy>=1.8',
                       'scipy>=0.14',
                       'matplotlib>=1.3',
                       'h5py>=2.10.0'],
     
     platforms='any',
```

