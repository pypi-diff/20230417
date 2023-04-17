# Comparing `tmp/esi-acme-2022.8.tar.gz` & `tmp/esi-acme-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi-acme-2022.8.tar", last modified: Mon Aug  8 07:51:00 2022, max compression
+gzip compressed data, was "esi-acme-2023.4.tar", last modified: Mon Apr 17 08:59:17 2023, max compression
```

## Comparing `esi-acme-2022.8.tar` & `esi-acme-2023.4.tar`

### file list

```diff
@@ -1,31 +1,43 @@
-drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2022-08-08 07:51:00.801596 esi-acme-2022.8/
--rw-r--r--   0 fuertingers (70137) it       (70000)      224 2022-08-01 09:44:15.000000 esi-acme-2022.8/.coveragerc
--rw-r--r--   0 fuertingers (70137) it       (70000)     7687 2022-08-04 14:04:33.000000 esi-acme-2022.8/CHANGELOG.md
--rw-r--r--   0 fuertingers (70137) it       (70000)     1100 2022-08-08 07:50:59.000000 esi-acme-2022.8/CITATION.cff
--rw-r--r--   0 fuertingers (70137) it       (70000)     1597 2022-08-01 09:44:15.000000 esi-acme-2022.8/LICENSE
--rw-r--r--   0 fuertingers (70137) it       (70000)     6130 2022-08-08 07:51:00.801596 esi-acme-2022.8/PKG-INFO
--rw-r--r--   0 fuertingers (70137) it       (70000)     4935 2022-08-04 14:04:33.000000 esi-acme-2022.8/README.md
-drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2022-08-08 07:51:00.801596 esi-acme-2022.8/acme/
--rw-r--r--   0 fuertingers (70137) it       (70000)     1987 2022-08-01 09:44:15.000000 esi-acme-2022.8/acme/__init__.py
--rw-r--r--   0 fuertingers (70137) it       (70000)    36919 2022-08-05 11:16:24.000000 esi-acme-2022.8/acme/backend.py
--rw-r--r--   0 fuertingers (70137) it       (70000)    37463 2022-08-04 14:04:33.000000 esi-acme-2022.8/acme/dask_helpers.py
--rw-r--r--   0 fuertingers (70137) it       (70000)    18111 2022-08-04 14:04:33.000000 esi-acme-2022.8/acme/frontend.py
--rw-r--r--   0 fuertingers (70137) it       (70000)    12958 2022-08-04 14:04:33.000000 esi-acme-2022.8/acme/shared.py
-drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2022-08-08 07:51:00.801596 esi-acme-2022.8/acme/tests/
--rw-r--r--   0 fuertingers (70137) it       (70000)      936 2022-08-04 14:04:33.000000 esi-acme-2022.8/acme/tests/local_acme.py
--rwxr-xr-x   0 fuertingers (70137) it       (70000)      195 2022-08-01 09:44:15.000000 esi-acme-2022.8/acme/tests/no_slurm.sh
--rw-r--r--   0 fuertingers (70137) it       (70000)      643 2022-08-01 09:44:15.000000 esi-acme-2022.8/acme/tests/run_tests.cmd
--rwxr-xr-x   0 fuertingers (70137) it       (70000)     1943 2022-08-01 09:44:15.000000 esi-acme-2022.8/acme/tests/run_tests.sh
--rw-r--r--   0 fuertingers (70137) it       (70000)    38477 2022-08-08 07:46:35.000000 esi-acme-2022.8/acme/tests/test_pmap.py
--rw-r--r--   0 fuertingers (70137) it       (70000)      501 2022-08-08 07:50:59.000000 esi-acme-2022.8/acme.yml
-drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2022-08-08 07:51:00.801596 esi-acme-2022.8/esi_acme.egg-info/
--rw-r--r--   0 fuertingers (70137) it       (70000)     6130 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/PKG-INFO
--rw-r--r--   0 fuertingers (70137) it       (70000)      503 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/SOURCES.txt
--rw-r--r--   0 fuertingers (70137) it       (70000)        1 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/dependency_links.txt
--rw-r--r--   0 fuertingers (70137) it       (70000)        1 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/not-zip-safe
--rw-r--r--   0 fuertingers (70137) it       (70000)      182 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/requires.txt
--rw-r--r--   0 fuertingers (70137) it       (70000)        5 2022-08-08 07:51:00.000000 esi-acme-2022.8/esi_acme.egg-info/top_level.txt
--rw-r--r--   0 fuertingers (70137) it       (70000)      126 2022-08-04 14:08:12.000000 esi-acme-2022.8/pyproject.toml
--rw-r--r--   0 fuertingers (70137) it       (70000)     1518 2022-08-08 07:51:00.801596 esi-acme-2022.8/setup.cfg
--rw-r--r--   0 fuertingers (70137) it       (70000)     2379 2022-08-04 14:04:33.000000 esi-acme-2022.8/setup.py
--rw-r--r--   0 fuertingers (70137) it       (70000)      861 2022-08-04 14:04:33.000000 esi-acme-2022.8/tox.ini
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.215675 esi-acme-2023.4/
+-rw-r--r--   0 fuertingers (70137) it       (70000)      379 2023-04-17 08:55:10.000000 esi-acme-2023.4/.coveragerc
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.211675 esi-acme-2023.4/.reuse/
+-rw-r--r--   0 fuertingers (70137) it       (70000)      317 2023-04-17 08:55:10.000000 esi-acme-2023.4/.reuse/dep5
+-rw-r--r--   0 fuertingers (70137) it       (70000)    14915 2023-04-17 08:55:10.000000 esi-acme-2023.4/CHANGELOG.md
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1107 2023-04-17 08:59:16.000000 esi-acme-2023.4/CITATION.cff
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1601 2023-04-17 08:55:10.000000 esi-acme-2023.4/LICENSE
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.215675 esi-acme-2023.4/LICENSES/
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1543 2023-04-17 08:55:10.000000 esi-acme-2023.4/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)    11032 2023-04-17 08:55:10.000000 esi-acme-2023.4/LICENSES/CC-BY-NC-ND-1.0.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)    13065 2023-04-17 08:55:10.000000 esi-acme-2023.4/LICENSES/CC-BY-NC-SA-1.0.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)     7048 2023-04-17 08:55:10.000000 esi-acme-2023.4/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)     8579 2023-04-17 08:59:17.215675 esi-acme-2023.4/PKG-INFO
+-rw-r--r--   0 fuertingers (70137) it       (70000)     7355 2023-04-17 08:55:10.000000 esi-acme-2023.4/README.md
+-rw-r--r--   0 fuertingers (70137) it       (70000)      272 2023-04-17 08:55:10.000000 esi-acme-2023.4/SECURITY.md
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.215675 esi-acme-2023.4/acme/
+-rw-r--r--   0 fuertingers (70137) it       (70000)     2692 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/__init__.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)    57769 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/backend.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)    37549 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/dask_helpers.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)    22927 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/frontend.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)     6402 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/logger.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)     9431 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/shared.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)      833 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/spy_interface.py
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.215675 esi-acme-2023.4/acme/tests/
+-rw-r--r--   0 fuertingers (70137) it       (70000)      750 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/conftest.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1309 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/local_acme.py
+-rwxr-xr-x   0 fuertingers (70137) it       (70000)      351 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/no_slurm.sh
+-rw-r--r--   0 fuertingers (70137) it       (70000)      809 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/run_tests.cmd
+-rwxr-xr-x   0 fuertingers (70137) it       (70000)     2346 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/run_tests.sh
+-rw-r--r--   0 fuertingers (70137) it       (70000)     5688 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/test_dask.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)    65536 2023-04-17 08:55:10.000000 esi-acme-2023.4/acme/tests/test_pmap.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)      691 2023-04-17 08:59:16.000000 esi-acme-2023.4/acme.yml
+drwxr-xr-x   0 fuertingers (70137) it       (70000)        0 2023-04-17 08:59:17.215675 esi-acme-2023.4/esi_acme.egg-info/
+-rw-r--r--   0 fuertingers (70137) it       (70000)     8579 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/PKG-INFO
+-rw-r--r--   0 fuertingers (70137) it       (70000)      716 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/SOURCES.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)        1 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/dependency_links.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)        1 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/not-zip-safe
+-rw-r--r--   0 fuertingers (70137) it       (70000)      213 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/requires.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)        5 2023-04-17 08:59:17.000000 esi-acme-2023.4/esi_acme.egg-info/top_level.txt
+-rw-r--r--   0 fuertingers (70137) it       (70000)      285 2023-04-17 08:55:10.000000 esi-acme-2023.4/pyproject.toml
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1594 2023-04-17 08:59:17.219675 esi-acme-2023.4/setup.cfg
+-rw-r--r--   0 fuertingers (70137) it       (70000)     2792 2023-04-17 08:55:10.000000 esi-acme-2023.4/setup.py
+-rw-r--r--   0 fuertingers (70137) it       (70000)     1026 2023-04-17 08:55:10.000000 esi-acme-2023.4/tox.ini
```

### Comparing `esi-acme-2022.8/CITATION.cff` & `esi-acme-2023.4/CITATION.cff`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     \ Max Planck Society"
   family-names: Shapcott
   given-names: Katharine
   orcid: https://orcid.org/0000-0001-8618-5779
 - affiliation: "Ernst Str\xFCngmann Institute for Neuroscience in Cooperation with\
     \ Max Planck Society"
   family-names: Schmiedt
-  given-names: Joscha
+  given-names: Joscha Tapani
   orcid: https://orcid.org/0000-0001-6233-1866
 cff-version: 1.1.0
-date-released: '2022-08-08'
+date-released: '2023-04-17'
 keywords:
 - high-performance computing
 - parallel computing
 license: BSD-3-Clause
 message: If you use this software, please cite it based on metadata found in this
   file. ACME provides functionality to execute Python functions concurrently and is
   itself used as the parallelization engine of SyNCoPy.
 repository-code: https://github.com/esi-neuroscience/acme
 title: 'ACME: Asynchronous Computing Made ESI'
-version: '2022.8'
+version: '2023.4'
```

### Comparing `esi-acme-2022.8/LICENSE` & `esi-acme-2023.4/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, Ernst Strüngmann Institute (ESI) for Neuroscience in Cooperation with Max Planck Society
+Copyright (c) 2020-2023 Ernst Strüngmann Institute (ESI) for Neuroscience in Cooperation with Max Planck Society
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `esi-acme-2022.8/PKG-INFO` & `esi-acme-2023.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,38 @@
-Metadata-Version: 2.1
-Name: esi-acme
-Version: 2022.8
-Summary: Asynchronous Computing Made ESI
-Home-page: https://esi-acme.readthedocs.io/en/latest/
-Author: Ernst Strüngmann Institute (ESI) for Neuroscience in Cooperation with Max Planck Society
-Author-email: acme@esi-frankfurt.de
-License: BSD-3
-Project-URL: Bug Tracker, https://github.com/esi-neuroscience/acme/issues
-Project-URL: Documentation, https://esi-acme.readthedocs.io/en/latest/
-Project-URL: Source Code, https://github.com/esi-neuroscience/acme
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: <3.10,>=3.7
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: dev
-License-File: LICENSE
+<!--
+Copyright (c) 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+in Cooperation with Max Planck Society
+SPDX-License-Identifier: CC-BY-NC-SA-1.0
+-->
 
 ![ACME_logo](https://raw.githubusercontent.com/esi-neuroscience/acme/master/doc/source/_static/acme_logo.png)
 
 # ACME: Asynchronous Computing Made ESI
 
-main: [![tests+codecov](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml/badge.svg?branch=main)](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml)
-[![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/main/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
+[![conda](https://img.shields.io/conda/vn/conda-forge/esi-acme.svg)](https://anaconda.org/conda-forge/esi-acme)
+[![pypi](https://badge.fury.io/py/esi-acme.svg)](https://badge.fury.io/py/esi-acme)
+[![license](https://img.shields.io/github/license/esi-neuroscience/acme)](https://github.com/esi-neuroscience/acme/blob/main/LICENSE)
+[![Open in Visual Studio Code](https://img.shields.io/badge/-Open_in_VS_Code-007ACC?logo=visual%20studio%20code&logoColor=ffffff)](https://github.dev/esi-neuroscience/acme)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7144/badge)](https://bestpractices.coreinfrastructure.org/projects/7144)
 
+main: [![tests](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml/badge.svg?branch=main)](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml)
+[![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/main/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
 
-dev: [![tests+codecov](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml/badge.svg?branch=dev)](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml)
+dev: [![tests](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml/badge.svg?branch=dev)](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml)
 [![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/dev/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
 
 ## Summary
 
 The objective of ACME (pronounced *"ak-mee"*) is to provide easy-to-use
 wrappers for calling Python functions concurrently ("embarassingly parallel workloads").
 ACME is developed at the
 [Ernst Strüngmann Institute (ESI) gGmbH for Neuroscience in Cooperation with Max Planck Society](https://www.esi-frankfurt.de/>)
 and released free of charge under the
 [BSD 3-Clause "New" or "Revised" License](https://en.wikipedia.org/wiki/BSD_licenses#3-clause_license_(%22BSD_License_2.0%22,_%22Revised_BSD_License%22,_%22New_BSD_License%22,_or_%22Modified_BSD_License%22)).
-ACME relies on the concurrent processing library [Dask](https://docs.dask.org/en/latest/>)
+ACME relies heavily on the concurrent processing library [dask](https://docs.dask.org/en/latest/>)
 and was primarily designed to facilitate the use of [SLURM](https://slurm.schedmd.com/documentation.html)
 on the ESI HPC cluster (although other HPC infrastructure running SLURM can be
 leveraged as well). Local multi-processing hardware (i.e., multi-core CPUs)
 is fully supported too. ACME is itself used as the parallelization engine of [SyNCoPy](http://www.syncopy.org/).
 
 ![](https://github.com/esi-neuroscience/acme/blob/main/doc/source/_static/acme_demo.gif)
 
@@ -87,14 +70,16 @@
 def f(x, y, z=3):
   return (x + y) * z
 
 with ParallelMap(f, [2, 4, 6, 8], 4) as pmap:
   pmap.compute()
 ```
 
+See also our [Quickstart Guide](https://esi-acme.readthedocs.io/en/latest/quickstart.html).
+
 ### Intermediate Examples
 
 Set number of function calls via `n_inputs`
 
 ```python
 import numpy as np
 from acme import ParallelMap
@@ -104,14 +89,17 @@
 
 pmap = ParallelMap(f, [2, 4, 6, 8], [2, 2], z=np.array([1, 2]), w=np.ones((8, 1)), n_inputs=2)
 
 with pmap as p:
   p.compute()
 ```
 
+More details in
+[Override Automatic Input Argument Distribution](https://esi-acme.readthedocs.io/en/latest/userguide.html#override-automatic-input-argument-distribution)
+
 ### Advanced Use
 
 Allocate custom `client` object and recycle it for several computations
 (use `slurm_cluster_setup` on non-ESI HPC infrastructure or `local_cluster_setup`
 when working on your local machine)
 
 ```python
@@ -120,73 +108,119 @@
 
 def f(x, y, z=3, w=np.zeros((3, 1)), **kwargs):
     return (sum(x) + y) * z * w.max()
 
 def g(x, y, z=3, w=np.zeros((3, 1)), **kwargs):
     return (max(x) + y) * z * w.sum()
 
-n_jobs = 200
-client = esi_cluster_setup(partition="8GBXS", n_jobs=n_jobs)
+n_workers = 200
+client = esi_cluster_setup(partition="8GBXS", n_workers=n_workers)
 
 x = [2, 4, 6, 8]
-z = range(n_jobs)
+z = range(n_workers)
 w = np.ones((8, 1))
 
-pmap = ParallelMap(f, x, np.random.rand(n_jobs), z=z, w=w, n_inputs=n_jobs)
+pmap = ParallelMap(f, x, np.random.rand(n_workers), z=z, w=w, n_inputs=n_workers)
 with pmap as p:
     p.compute()
 
-pmap = ParallelMap(g, x, np.random.rand(n_jobs), z=z, w=w, n_inputs=n_jobs)
+pmap = ParallelMap(g, x, np.random.rand(n_workers), z=z, w=w, n_inputs=n_workers)
 with pmap as p:
     p.compute()
 ```
 
+For more information see [Reuse Worker Clients](https://esi-acme.readthedocs.io/en/latest/userguide.html#reuse-worker-clients)
+
 ## Handling results
 
 ### Load results from files
 
-The results are saved to disk in HDF5 format and the filenames are returned as a list of strings.
+By default, results are saved to disk in HDF5 format and can be accessed using
+the `results_container` attribute of `ParallelMap`:
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4) as pmap:
   filenames = pmap.compute()
 ```
 
 Example loading code:
 
 ```python
-out = np.zeros((4))
 import h5py
-for ii, fname in enumerate(filenames):
-    with h5py.File(fname, 'r') as f:
-        out[ii] = np.array(f['result_0'])
+import numpy as np
+out = np.zeros((4,))
+
+with h5py.File(pmap.results_container, "r") as h5f:
+  for k, key in enumerate(h5f.keys()):
+    out[k] = h5f[key]["result_0"][()]
+```
+
+See also [Where Are My Results?](https://esi-acme.readthedocs.io/en/latest/userguide.html#where-are-my-results)
+
+### Collect results in single HDF5 dataset
+
+If possible, results can be slotted into a single HDF5 dataset:
+
+```python
+def f(x, y, z=3):
+  return (x + y) * z
+
+with ParallelMap(f, [2, 4, 6, 8], 4, result_shape=(None,)) as pmap:
+  pmap.compute()
+```
+
+Example loading code:
+
+```python
+import h5py
+
+with h5py.File(pmap.results_container, "r") as h5f:
+  out = h5f["result_0"][()] # returns a NumPy array of shape (4,)
 ```
 
+More examples can be found in
+[Collect Results in Single Dataset](https://esi-acme.readthedocs.io/en/latest/userguide.html#collect-results-in-single-dataset)
+
 ### Collect results in local memory
 
 This is possible but not recommended.
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4, write_worker_results=False) as pmap:
-  results = pmap.compute() # returns a list of outputs
+  result = pmap.compute() # returns a 4-element list
+```
+
+Alternatively, create an in-memory NumPy array
+
+```python
+with ParallelMap(f, [2, 4, 6, 8], 4, write_worker_results=False, result_shape=(None,)) as pmap:
+  result = pmap.compute() # returns a NumPy array of shape (4,)
 ```
 
 ## Debugging
 
 Use the `debug` keyword to perform all function calls in the local thread of
 the active Python interpreter
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4, z=None) as pmap:
     results = pmap.compute(debug=True)
 ```
 
 This way tools like `pdb` or ``%debug`` IPython magics can be used.
+More information can be found in the `FAQ`[https://esi-acme.readthedocs.io/en/latest/troubleshooting_faq.html]
 
 ## Documentation and Contact
 
 To report bugs or ask questions please use our
 [GitHub issue tracker](https://github.com/esi-neuroscience/acme/issues).
 More usage details and background information is available in our
 [online documentation](https://esi-acme.readthedocs.io).
-
-
```

### Comparing `esi-acme-2022.8/acme/__init__.py` & `esi-acme-2023.4/acme/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# -*- coding: utf-8 -*-
 #
 # Main package initializer
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import subprocess
 import warnings
 import inspect
 import sys
 from pkg_resources import get_distribution, DistributionNotFound
@@ -26,20 +30,33 @@
         if proc.returncode != 0:
             msg = "<ACME> Package is not installed in site-packages nor cloned via git. " +\
                 "Please consider obtaining ACME sources from supported channels. "
             warnings.showwarning(msg, ImportWarning, __file__, inspect.currentframe().f_lineno)
             out = "-999"
     __version__ = out.rstrip("\n")
 
+# Central collection of deprecated keywords/canonical warning message
+__deprecated__ = ["n_jobs", "mem_per_job", "n_jobs_startup" "workers_per_job"]
+__deprecation_wrng__ = \
+    "The keywords `n_jobs`, `mem_per_job`, `n_jobs_startup` and " +\
+    "`workers_per_job` are DEPRECATED. Please use `n_workers`, `mem_per_worker`, " +\
+    "`n_workers_startup` and `processes_per_worker`, respectively."
+
+# Remove dask-jobqueue's FutureWarnings about tmpfile (which we don't use)
+warnings.simplefilter(action='ignore', category=FutureWarning)
+
 # Import local modules
-from . import frontend, backend, shared, dask_helpers
 from .frontend import *
 from .backend import *
 from .shared import *
 from .dask_helpers import *
+from .logger import prepare_log
+
+# Set up module-wide logging
+prepare_log(logname="ACME")
 
 # Override default exception handler (take care of Jupyter's Exception handling)
 from .shared import ctrlc_catcher
 try:
     ipy = get_ipython()
     import IPython
     ipy.ipyTBshower = IPython.core.interactiveshell.InteractiveShell.showtraceback
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/dask_helpers.py` & `esi-acme-2023.4/acme/dask_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# -*- coding: utf-8 -*-
 #
 # Helper routines for working w/dask
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import os
 import sys
 import socket
 import subprocess
 import getpass
@@ -15,89 +19,74 @@
 import numpy as np
 from tqdm import tqdm
 if sys.platform == "win32":
     # tqdm breaks term colors on Windows - fix that (tqdm issue #446)
     import colorama
     colorama.deinit()
     colorama.init(strip=False)
-
-# Local imports: differentiate b/w being imported as Syncopy sub-package or
-# standalone ACME module: if imported by Syncopy, use some lambda magic to avoid
-# circular imports due to (at import-time) only partially initialized Syncopy
-from .shared import user_input, user_yesno
-if "syncopy" in sys.modules:
-    isSpyModule = True
-    import syncopy as spy
-    customIOError = lambda msg : spy.shared.errors.SPYIOError(msg)
-    customValueError = lambda legal=None, varname=None, actual=None : \
-        spy.shared.errors.SPYValueError(legal=legal, varname=varname, actual=actual)
-    customTypeError = lambda val, varname=None, expected=None : \
-        spy.shared.errors.SPYTypeError(val, varname=varname, expected=expected)
-    scalar_parser = lambda var, varname="", ntype=None, lims=None : \
-        spy.shared.parsers.scalar_parser(var, varname=varname, ntype=ntype, lims=lims)
-else:
-    isSpyModule = False
-    from warnings import showwarning
-    import logging
-    from .shared import _scalar_parser as scalar_parser
-    customIOError = IOError
-    customValueError = lambda legal=None, varname=None, actual=None : ValueError(legal)
-    customTypeError = lambda msg, varname=None, expected=None : TypeError(msg)
-
 from dask_jobqueue import SLURMCluster
-from dask.distributed import Client, get_client
+from dask.distributed import Client, get_client, LocalCluster
 from datetime import datetime, timedelta
 
-# Be optimistic: prepare success message to be used throughout this module
-_successMsg = "{name:s} Cluster dashboard accessible at {dash:s}"
+# Local imports
+from acme import __deprecated__, __deprecation_wrng__
+from .shared import user_input, user_yesno
+from .spy_interface import scalar_parser, log
 
 __all__ = ["esi_cluster_setup", "local_cluster_setup", "cluster_cleanup", "slurm_cluster_setup"]
 
 
-# Setup SLURM jobs on the ESI HPC cluster
-def esi_cluster_setup(partition="8GBXS", n_jobs=2, mem_per_job="auto", n_jobs_startup=100,
-                      timeout=60, interactive=True, interactive_wait=120, start_client=True,
-                      job_extra=[], **kwargs):
+# Setup SLURM workers on the ESI HPC cluster
+def esi_cluster_setup(partition="8GBXS",
+                      n_workers=2,
+                      mem_per_worker="auto",
+                      n_workers_startup=1,
+                      timeout=60,
+                      interactive=True,
+                      interactive_wait=120,
+                      start_client=True,
+                      job_extra=[],
+                      **kwargs):
     """
     Start a Dask distributed SLURM worker cluster on the ESI HPC infrastructure
     (or local multi-processing)
 
     Parameters
     ----------
     partition : str
         Name of SLURM partition/queue to start workers in. Use the command `sinfo`
         in the terminal to see a list of available SLURM partitions on the ESI HPC
         cluster.
-    n_jobs : int
-        Number of SLURM jobs (=workers) to spawn
-    mem_per_job : None or str
-        Memory booking for each job. Can be specified either in megabytes
-        (e.g., ``mem_per_job = 1500MB``) or gigabytes (e.g., ``mem_per_job = "2GB"``).
-        If `mem_per_job` is `None`, or `"auto"` it is attempted to infer a sane default value
-        from the chosen partition, e.g., for ``partition = "8GBS"`` `mem_per_job` is
+    n_workers : int
+        Number of SLURM workers (=jobs) to spawn
+    mem_per_worker : None or str
+        Memory booking for each worker. Can be specified either in megabytes
+        (e.g., ``mem_per_worker = 1500MB``) or gigabytes (e.g., ``mem_per_worker = "2GB"``).
+        If `mem_per_worker` is `None`, or `"auto"` it is attempted to infer a sane default value
+        from the chosen partition, e.g., for ``partition = "8GBS"`` `mem_per_worker` is
         automatically set to the allowed maximum of `'8GB'`. However, even in
         queues with guaranteed memory bookings, it is possible to allocate less
-        memory than the allowed maximum per job to spawn numerous low-memory
-        jobs. See Examples for details.
-    n_jobs_startup : int
-        Number of spawned jobs to wait for. If `n_jobs_startup` is `100` (default),
+        memory than the allowed maximum per worker to spawn numerous low-memory
+        workers. See Examples for details.
+    n_workers_startup : int
+        Number of spawned workers to wait for. If `n_workers_startup` is `100` (default),
         the code does not proceed until either 100 SLURM jobs are running or the
         `timeout` interval has been exceeded.
     timeout : int
-        Number of seconds to wait for requested jobs to start (see `n_jobs_startup`).
+        Number of seconds to wait for requested workers to start (see `n_workers_startup`).
     interactive : bool
-        If `True`, user input is queried in case not enough jobs (set by `n_jobs_startup`)
+        If `True`, user input is queried in case not enough workers (set by `n_workers_startup`)
         could be started in the provided waiting period (determined by `timeout`).
         The code waits `interactive_wait` seconds for a user choice - if none is
-        provided, it continues with the current number of running jobs (if greater
-        than zero). If `interactive` is `False` and no job could not be started
+        provided, it continues with the current number of running workers (if greater
+        than zero). If `interactive` is `False` and no worker could not be started
         within `timeout` seconds, a `TimeoutError` is raised.
     interactive_wait : int
         Countdown interval (seconds) to wait for a user response in case fewer than
-        `n_jobs_startup` jobs could be started. If no choice is provided within
+        `n_workers_startup` workers could be started. If no choice is provided within
         the given time, the code automatically proceeds with the current number of
         active dask workers.
     start_client : bool
         If `True`, a distributed computing client is launched and attached to
         the dask worker cluster. If `start_client` is `False`, only a distributed
         computing cluster is started to which compute-clients can connect.
     job_extra : list
@@ -109,18 +98,18 @@
     -------
     proc : object
         A distributed computing client (if ``start_client = True``) or
         a distributed computing cluster (otherwise).
 
     Examples
     --------
-    The following command launches 10 SLURM jobs with 2 gigabytes memory each
+    The following command launches 10 SLURM workers with 2 gigabytes memory each
     in the `8GBS` partition
 
-    >>> client = esi_cluster_setup(n_jobs=10, partition="8GBS", mem_per_job="2GB")
+    >>> client = esi_cluster_setup(n_workers=10, partition="8GBS", mem_per_worker="2GB")
 
     The underlying distributed computing cluster can be accessed using
 
     >>> client.cluster
 
     Notes
     -----
@@ -130,28 +119,50 @@
     This function specifically acts  as a wrapper for :class:`dask_jobqueue.SLURMCluster`.
     Users familiar with Dask in general and its distributed scheduler and cluster
     objects in particular, may leverage Dask's entire API to fine-tune parallel
     processing jobs to their liking (if wanted).
 
     See also
     --------
+    dask_jobqueue.SLURMCluster : launch a dask cluster of SLURM workers
     slurm_cluster_setup : start a distributed Dask cluster of parallel processing workers using SLURM
     local_cluster_setup : start a local Dask multi-processing cluster on the host machine
-    cluster_cleanup : remove dangling parallel processing job-clusters
+    cluster_cleanup : remove dangling parallel processing worker-clusters
     """
 
-    # Re-direct printing/warnings to ACME logger outside of SyNCoPy
-    customPrint, customWarning = _logging_setup()
-
     # For later reference: dynamically fetch name of current function
-    funcName = "{pre:s}<{pkg:s}{name:s}>".format(pre="Syncopy " if isSpyModule else "",
-                                                 pkg="ACME: " if isSpyModule else "",
-                                                 name=inspect.currentframe().f_code.co_name)
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
+
+    # Backwards compatibility: legacy keywords are converted to new nomenclature
+    if any(kw in kwargs for kw in __deprecated__):
+        log.warning(__deprecation_wrng__)
+        n_workers = kwargs.pop("n_jobs", n_workers)
+        mem_per_worker = kwargs.pop("mem_per_job", mem_per_worker)
+        n_workers_startup = kwargs.pop("n_jobs_startup", n_workers_startup)
+        log.debug("Set `n_workers = n_jobs`, `mem_per_worker = mem_per_job`\
+                  and `n_workers_startup = n_jobs_startup`")
+
+    # Don't start a new cluster on top of an existing one
+    try:
+        client = get_client()
+        log.debug("Found existing client")
+        if count_online_workers(client.cluster) == 0:
+            log.debug("No active workers detected in %s", str(client))
+            cluster_cleanup(client)
+        else:
+            log.info("Found existing parallel computing client %s. \
+                     Not starting new cluster.", str(client))
+            if start_client:
+                return client
+            return client.cluster
+    except ValueError:
+        log.debug("No existing clients detected")
 
     # Check if SLURM's `sinfo` can be accessed
+    log.debug("Test if `sinfo` is available")
     proc = subprocess.Popen("sinfo",
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                             text=True, shell=True)
     _, err = proc.communicate()
 
     # Any non-zero return-code means SLURM is not ready to use
     if proc.returncode != 0:
@@ -166,125 +177,138 @@
                                         default="no")
             else:
                 startLocal = True
             if startLocal:
                 return local_cluster_setup(interactive=interactive, start_client=start_client)
 
         # SLURM is installed, but something's wrong
-        msg = "{preamble:s}SLURM queuing system from node {node:s}. " +\
-              "Original error message below:\n{error:s}"
-        raise customIOError(msg.format(preamble=funcName + " Cannot access " if not isSpyModule else "",
-                                       node=socket.gethostname(),
-                                       error=err))
-
-    # Use default by-job worker count or extract it from anonymous keyword args (if provided)
-    workers_per_job = 1
-    if kwargs.get("workers_per_job") is not None:
-        workers_per_job = kwargs.pop("workers_per_job")
+        msg = "Cannot access SLURM queuing system from node %s: %s "
+        log.error(msg, socket.gethostname(), err)
+        raise IOError("%s %s"%(funcName, msg%(socket.gethostname(), err)))
+
+    # Use default by-worker process count or extract it from anonymous keyword args (if provided)
+    processes_per_worker = kwargs.pop("processes_per_worker", 1)
+    log.debug("Found `sinfo`, set `processes_per_worker` to %d", processes_per_worker)
 
-    # If partition is "auto" use `mem_per_job` to pick pseudo-optimal partition
+    # If partition is "auto" use `mem_per_worker` to pick pseudo-optimal partition
     # Note: the `np.where` gymnastic below is necessary since `argmin` refuses
-    # to return multiple matches; if `mem_per_job` is 12, then ``memDiff = [4, 4, ...]``,
-    # however, 8GB won't fit a 12GB job, so we have to pick the second match 16GB
+    # to return multiple matches; if `mem_per_worker` is 12, then ``memDiff = [4, 4, ...]``,
+    # however, 8GB won't fit a 12GB worker, so we have to pick the second match 16GB
     if isinstance(partition, str) and partition == "auto":
-        if not isinstance(mem_per_job, str) or mem_per_job.find("estimate_memuse:") < 0:
-            msg = "{preamble:s}automatic partition selector without first invoking `ParallelMap`. "
-            raise customIOError(msg.format(preamble=funcName + " Cannot access " if not isSpyModule else ""))
-        memEstimate = int(mem_per_job.replace("estimate_memuse:" ,""))
-        mem_per_job = "auto"
-        customPrint("{}Automatically selecting SLURM partition...".format(funcName))
-        availPartitions = _get_slurm_partitions(funcName)
+        if not isinstance(mem_per_worker, str) or mem_per_worker.find("estimate_memuse:") < 0:
+            msg = "Cannot auto-select partition without first invoking memory estimation in `ParallelMap`. "
+            log.error(msg)
+            raise IOError("%s %s"%(funcName, msg))
+        memEstimate = int(mem_per_worker.replace("estimate_memuse:" ,""))
+        mem_per_worker = "auto"
+        log.info("Automatically selecting SLURM partition...")
+        availPartitions = _get_slurm_partitions()
         gbQueues = np.unique([int(queue.split("GB")[0]) for queue in availPartitions if queue[0].isdigit()])
         memDiff = np.abs(gbQueues - memEstimate)
         queueIdx = np.where(memDiff == memDiff.min())[0][-1]
         partition = "{}GBXS".format(gbQueues[queueIdx])
-        msg = "{preamble:s}Picked partition {p:s} based on estimated memory consumption of {m:d} GB"
-        customPrint(msg.format(preamble=funcName, p=partition, m=memEstimate))
+        msg = "Picked partition %s based on estimated memory consumption of %d GB"
+        log.info(msg, partition, memEstimate)
 
-    # Extract by-job CPU core count from anonymous keyword args or...
+    # Extract by-worker CPU core count from anonymous keyword args or...
     if kwargs.get("n_cores") is not None:
         n_cores = kwargs.pop("n_cores")
+        log.debug("Set `n_cores = %d` from kwargs", n_cores)
     else:
         # ...get memory limit (*in MB*) of chosen partition and set core count
         # accordingly (multiple of 8 wrt to GB RAM)
         try:
+            log.debug("Using `scontrol` to get partition info")
             pc = subprocess.run("scontrol -o show partition {}".format(partition),
                                 capture_output=True, check=True, shell=True, text=True)
             defMem = int(pc.stdout.strip().partition("DefMemPerCPU=")[-1].split()[0])
+            log.debug("Found DefMemPerCPU=%d", defMem)
         except Exception as exc:
-            msg = "{preamble:s}available memory per CPU in chosen SLURM partition. " +\
-                "Original error message below:\n{error:s}"
-            raise customIOError(msg.format(preamble=funcName + " Cannot access " if not isSpyModule else "",
-                                           error=str(exc)))
+            msg = "Cannot fetch available memory per CPU in SLURM: %s"
+            log.error(msg, str(exc))
+            raise IOError("%s %s"%(funcName, msg%(str(exc))))
         n_cores = int(defMem / 8000)
+        log.debug("Using `n_cores=%d`", n_cores)
 
     # Determine if `job_extra`` is a list (this is also checked in `slurm_cluster_setup`,
     # but we may need to append to it, so ensure that's possible)
     if not isinstance(job_extra, list):
-        msg = "{} `job_extra` has to be List, not {}"
-        raise customTypeError(job_extra if isSpyModule else msg.format(funcName, str(job_extra)),
-                              varname="job_extra",
-                              expected="list")
+        msg = "`job_extra` has to be a list, not %s"
+        log.error(msg, str(type(job_extra)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(job_extra)))))
 
     # If '--output' was not provided, append default output folder to `job_extra`
     if not any(option.startswith("--output") or option.startswith("-o") for option in job_extra):
+        log.debug("Auto-populating `--output` setting for sbatch")
         usr = getpass.getuser()
         slurm_wdir = "/cs/slurm/{usr:s}/{usr:s}_{date:s}"
         slurm_wdir = slurm_wdir.format(usr=usr,
                                        date=datetime.now().strftime('%Y%m%d-%H%M%S'))
         os.makedirs(slurm_wdir, exist_ok=True)
+        log.debug("Using %s for slurm logs", slurm_wdir)
         out_files = os.path.join(slurm_wdir, "slurm-%j.out")
         job_extra.append("--output={}".format(out_files))
+        log.debug("Setting `--output=%s`", out_files)
 
     # Let the SLURM-specific setup function do the rest (returns client or cluster)
-    return slurm_cluster_setup(partition, n_cores, n_jobs, workers_per_job, mem_per_job,
-                               n_jobs_startup, timeout, interactive, interactive_wait,
+    return slurm_cluster_setup(partition, n_cores, n_workers, processes_per_worker, mem_per_worker,
+                               n_workers_startup, timeout, interactive, interactive_wait,
                                start_client, job_extra, invalid_partitions=["DEV", "PPC"], **kwargs)
 
 
 # Setup SLURM cluster
-def slurm_cluster_setup(partition, n_cores, n_jobs, workers_per_job, mem_per_job,
-                        n_jobs_startup, timeout, interactive, interactive_wait,
-                        start_client, job_extra, invalid_partitions=[]):
+def slurm_cluster_setup(partition="partition_name",
+                        n_cores=1,
+                        n_workers=1,
+                        processes_per_worker=1,
+                        mem_per_worker="1GB",
+                        n_workers_startup=1,
+                        timeout=60,
+                        interactive=True,
+                        interactive_wait=10,
+                        start_client=True,
+                        job_extra=[],
+                        invalid_partitions=[],
+                        **kwargs):
     """
     Start a distributed Dask cluster of parallel processing workers using SLURM
 
     **NOTE** If you are working on the ESI HPC cluster, please use
     :func:`~acme.esi_cluster_setup` instead!
 
     Parameters
     ----------
     partition : str
         Name of SLURM partition/queue to use
     n_cores : int
-        Number of CPU cores per SLURM job
-    n_jobs : int
-        Number of SLURM jobs to spawn
-    workers_per_job : int
-        Number of processess (=dask workers) to use per job. Should be greater
+        Number of CPU cores per SLURM worker
+    n_workers : int
+        Number of SLURM workers (=jobs) to spawn
+    processes_per_worker : int
+        Number of processes to use per SLURM job (=worker). Should be greater
         than one only if the chosen partition contains nodes that expose multiple
         cores per job.
-    mem_per_job : str
-        Memory allocation for each job
-    n_jobs_startup : int
-        Number of spawned jobs to wait for. The code does not return until either
-        `n_jobs_startup` SLURM jobs are running or the `timeout` interval (see
+    mem_per_worker : str
+        Memory allocation for each worker
+    n_workers_startup : int
+        Number of spawned SLURM workers to wait for. The code does not return until either
+        `n_workers_startup` SLURM jobs are running or the `timeout` interval (see
         below) has been exceeded.
     timeout : int
-        Number of seconds to wait for requested jobs to start (see `n_jobs_startup`).
+        Number of seconds to wait for requested workers to start (see `n_workers_startup`).
     interactive : bool
-        If `True`, user input is queried in case not enough jobs (set by `n_jobs_startup`)
+        If `True`, user input is queried in case not enough workers (set by `n_workers_startup`)
         could be started in the provided waiting period (determined by `timeout`).
         The code waits `interactive_wait` seconds for a user choice - if none is
-        provided, it continues with the current number of running jobs (if greater
-        than zero). If `interactive` is `False` and no job could not be started
+        provided, it continues with the current number of running workers (if greater
+        than zero). If `interactive` is `False` and no worker could not be started
         within `timeout` seconds, a `TimeoutError` is raised.
     interactive_wait : int
         Countdown interval (seconds) to wait for a user response in case fewer than
-        `n_jobs_startup` jobs could be started. If no choice is provided within
+        `n_workers_startup` workers could be started. If no choice is provided within
         the given time, the code automatically proceeds with the current number of
         active dask workers.
     start_client : bool
         If `True`, a distributed computing client is launched and attached to
         the dask worker cluster. If `start_client` is `False`, only a distributed
         computing cluster is started to which compute-clients can connect.
     job_extra : list
@@ -297,312 +321,333 @@
     -------
     proc : object
         A distributed computing client (if ``start_client = True``) or
         a distributed computing cluster (otherwise).
 
     See also
     --------
+    dask_jobqueue.SLURMCluster : launch a dask cluster of SLURM workers
     esi_cluster_setup : start a SLURM worker cluster on the ESI HPC infrastructure
     local_cluster_setup : start a local Dask multi-processing cluster on the host machine
-    cluster_cleanup : remove dangling parallel processing job-clusters
+    cluster_cleanup : remove dangling parallel processing worker-clusters
     """
 
-    # Re-direct printing/warnings to ACME logger outside of SyNCoPy
-    customPrint, customWarning = _logging_setup()
-
     # For later reference: dynamically fetch name of current function
-    funcName = "{pre:s}<{pkg:s}{name:s}>".format(pre="Syncopy " if isSpyModule else "",
-                                                 pkg="ACME: " if isSpyModule else "",
-                                                 name=inspect.currentframe().f_code.co_name)
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
+
+    # Backwards compatibility: legacy keywords are converted to new nomenclature
+    if any(kw in kwargs for kw in __deprecated__):
+        log.warning(__deprecation_wrng__)
+        n_workers = kwargs.pop("n_jobs", n_workers)
+        processes_per_worker = kwargs.pop("workers_per_job", processes_per_worker)
+        mem_per_worker = kwargs.pop("mem_per_job", mem_per_worker)
+        n_workers_startup = kwargs.pop("n_jobs_startup", n_workers_startup)
+        log.debug("Set `n_workers = n_jobs`, `processes_per_worker = workers_per_job`, \
+                  `mem_per_worker = mem_per_job` \
+                  and `n_workers_startup = n_jobs_startup`")
 
     # Retrieve all partitions currently available in SLURM
-    availPartitions = _get_slurm_partitions(funcName)
+    availPartitions = _get_slurm_partitions()
 
     # Make sure we're in a valid partition
     if partition not in availPartitions:
         valid = list(set(availPartitions).difference(invalid_partitions))
         lgl = "'" + "or '".join(opt + "' " for opt in valid)
-        msg = "{} Invalid partition selection {}, available SLURM partitions are {}"
-        raise customValueError(legal=lgl if isSpyModule else msg.format(funcName, str(partition), lgl),
-                               varname="partition",
-                               actual=partition)
+        msg = "Invalid partition selection %s, available SLURM partitions are %s"
+        log.error(msg, str(partition), lgl)
+        raise ValueError("%s %s"%(funcName, msg%(str(partition), lgl)))
+    log.debug("Found `partition = %s`", partition)
 
-    # Parse job count
+    # Parse worker count
     try:
-        scalar_parser(n_jobs, varname="n_jobs", ntype="int_like", lims=[1, np.inf])
+        scalar_parser(n_workers, varname="n_workers", ntype="int_like", lims=[1, np.inf])
     except Exception as exc:
+        log.error("Error parsing `n_workers`")
         raise exc
+    log.debug("Using `n_workers = %d`", n_workers)
 
-    # Get requested memory per job
-    if isinstance(mem_per_job, str):
-        if mem_per_job == "auto":
-            mem_per_job = None
-    if mem_per_job is not None:
-        msg = "{} `mem_per_job` has to be a valid memory specifier (e.g., '8GB', '12000MB'), not {}"
-        lgl = "string representation of requested memory (e.g., '8GB', '12000MB')"
-        if not isinstance(mem_per_job, str):
-            raise customTypeError(mem_per_job if isSpyModule else msg.format(funcName, str(mem_per_job)),
-                                  varname="mem_per_job",
-                                  expected="string")
-        if not any(szstr in mem_per_job for szstr in ["MB", "GB"]):
-            raise customValueError(legal=lgl if isSpyModule else msg.format(funcName, str(mem_per_job)),
-                                   varname="mem_per_job",
-                                   actual=mem_per_job)
-        memNumeric = mem_per_job.replace("MB","").replace("GB","")
+    # Get requested memory per worker
+    if isinstance(mem_per_worker, str):
+        if mem_per_worker == "auto":
+            mem_per_worker = None
+            log.debug("Using auto-memory selection")
+    if mem_per_worker is not None:
+        msg = "`mem_per_worker` has to be a valid memory specifier (e.g., '8GB', '12000MB'), not %s"
+        if not isinstance(mem_per_worker, str):
+            log.error(msg, str(type(mem_per_worker)))
+            raise TypeError("%s %s"%(funcName, msg%(str(type(mem_per_worker)))))
+        if not any(szstr in mem_per_worker for szstr in ["MB", "GB"]):
+            log.error(msg, mem_per_worker)
+            raise ValueError("%s %s"%(funcName, msg%(mem_per_worker)))
+        memNumeric = mem_per_worker.replace("MB","").replace("GB","")
+        log.debug("Found `mem_per_worker = %s` in input args", mem_per_worker)
         try:
             memVal = float(memNumeric)
         except:
-            raise customValueError(legal=lgl if isSpyModule else msg.format(funcName, str(mem_per_job)),
-                                   varname="mem_per_job",
-                                   actual=mem_per_job)
+            log.error(msg, mem_per_worker)
+            raise ValueError("%s %s"%(funcName, msg%(mem_per_worker)))
         if memVal <= 0:
-            raise customValueError(legal=lgl if isSpyModule else msg.format(funcName, str(mem_per_job)),
-                                   varname="mem_per_job",
-                                   actual=mem_per_job)
+            log.error(msg, mem_per_worker)
+            raise ValueError("%s %s"%(funcName, msg%(mem_per_worker)))
 
-    # Parse job-waiter count
+    # Parse worker-waiter count
     try:
-        scalar_parser(n_jobs_startup, varname="n_jobs_startup", ntype="int_like", lims=[0, np.inf])
+        scalar_parser(n_workers_startup, varname="n_workers_startup", ntype="int_like", lims=[0, np.inf])
     except Exception as exc:
+        log.error("Error parsing `n_workers_startup`")
         raise exc
+    log.debug("Using `n_workers_startup = %d`", n_workers_startup)
 
     # Get memory limit (*in MB*) of chosen partition (guaranteed to exist, cf. above)
+    log.debug("Use `scontrol` to fetch partition's memory limit")
     pc = subprocess.run("scontrol -o show partition {}".format(partition),
                         capture_output=True, check=True, shell=True, text=True)
     try:
         mem_lim = int(pc.stdout.strip().partition("MaxMemPerCPU=")[-1].split()[0])
     except IndexError:
         try:
             mem_lim = int(pc.stdout.strip().partition("DefMemPerCPU=")[-1].split()[0])
         except IndexError:
             mem_lim = np.inf
+    log.debug("Found a limit of  %s MB", str(mem_lim))
 
     # Consolidate requested memory with chosen partition (or assign default memory)
-    if mem_per_job is None:
-        mem_per_job = str(mem_lim) + "MB"
+    if mem_per_worker is None:
+        mem_per_worker = str(mem_lim) + "MB"
+        log.debug("Using partition limit of %s MB", str(mem_lim))
     else:
-        if "MB" in mem_per_job:
-            mem_req = int(mem_per_job[:mem_per_job.find("MB")])
+        if "MB" in mem_per_worker:
+            mem_req = int(mem_per_worker[:mem_per_worker.find("MB")])
         else:
-            mem_req = int(round(float(mem_per_job[:mem_per_job.find("GB")]) * 1000))
+            mem_req = int(round(float(mem_per_worker[:mem_per_worker.find("GB")]) * 1000))
         if mem_req > mem_lim:
-            msg = "{name:s}`mem_per_job` exceeds limit of {lim:d}GB for partition {par:s}. " +\
+            msg = "`mem_per_worker` exceeds limit of %d MB for partition %s. " +\
                 "Capping memory at partition limit. "
-            customWarning(msg.format(name=funcName + " " if not isSpyModule else "", lim=mem_lim, par=partition),
-                          RuntimeWarning, __file__, inspect.currentframe().f_lineno)
-            mem_per_job = str(int(mem_lim)) + "GB"
+            log.warning(msg, mem_lim, partition)
+            mem_per_worker = str(int(mem_lim)) + "MB"
 
     # Parse requested timeout period
     try:
         scalar_parser(timeout, varname="timeout", ntype="int_like", lims=[1, np.inf])
     except Exception as exc:
+        log.error("Error parsing `timeout`")
         raise exc
+    log.debug("Using `timeout = %d`", timeout)
 
     # Parse requested interactive waiting period
     try:
         scalar_parser(interactive_wait, varname="interactive_wait", ntype="int_like",
                       lims=[0, np.inf])
     except Exception as exc:
+        log.error("Error parsing `interactive_wait`")
         raise exc
+    log.debug("Using `interactive_wait = %d`", interactive_wait)
 
     # Determine if cluster allocation is happening interactively
     if not isinstance(interactive, bool):
-        msg = "{} `interactive` has to be Boolean, not {}"
-        raise customTypeError(interactive if isSpyModule else msg.format(funcName, str(interactive)),
-                              varname="interactive",
-                              expected="bool")
+        msg = "`interactive` has to be Boolean, not %s"
+        log.error(msg, str(type(interactive)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(interactive)))))
+    log.debug("Using `interactive = %s`", str(interactive))
 
     # Determine if a dask client was requested
     if not isinstance(start_client, bool):
-        msg = "{} `start_client` has to be Boolean, not {}"
-        raise customTypeError(start_client if isSpyModule else msg.format(funcName, str(start_client)),
-                              varname="start_client",
-                              expected="bool")
+        msg = "`start_client` has to be Boolean, not %s"
+        log.error(msg, str(type(start_client)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(start_client)))))
+    log.debug("Using `start_client = %s`", str(start_client))
 
     # Determine if job_extra is a list
     if not isinstance(job_extra, list):
-        msg = "{} `job_extra` has to be List, not {}"
-        raise customTypeError(job_extra if isSpyModule else msg.format(funcName, str(job_extra)),
-                              varname="job_extra",
-                              expected="list")
+        msg = "`job_extra` has to be List, not %s"
+        log.error(msg, str(type(job_extra)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(job_extra)))))
 
     # Determine if job_extra options are valid
     for option in job_extra:
-        msg = "{} `job_extra` has to be a valid sbatch option, not {}"
+        msg = "`job_extra` has to be a valid sbatch option, not %s"
         if not isinstance(option, str):
-            raise customTypeError(option if isSpyModule else msg.format(funcName, str(option)),
-                                  varname="option",
-                                  expected="string")
+            log.error(msg, str(type(option)))
+            raise TypeError("%s %s"%(funcName, msg%(str(type(option)))))
         if not option[0] == "-":
-            lgl = "job_extra options should be flagged with - or --"
-            raise customValueError(legal=lgl, varname="option", actual=option)
+            msg = "`job_extra` options must be flagged with - or --"
+            log.error(msg)
+            raise ValueError("%s %s"%(funcName, msg))
+    log.debug("Using `job_extra = %s`", str(job_extra))
 
-    # Ensure validity of requested worker threads
+    # Ensure validity of requested worker processes
     try:
-        scalar_parser(workers_per_job, varname="workers_per_job",
+        scalar_parser(processes_per_worker, varname="processes_per_worker",
                       ntype="int_like", lims=[1, 16])
     except Exception as exc:
+        log.error("Error parsing `processes_per_worker`")
         raise exc
+    log.debug("Using `processes_per_worker = %d`", processes_per_worker)
 
     # Check for sanity of requested core count
     try:
         scalar_parser(n_cores, varname="n_cores",
                       ntype="int_like", lims=[1, np.inf])
     except Exception as exc:
+        log.error("Error parsing `n_cores`")
         raise exc
+    log.debug("Using `n_cores = %d`", n_cores)
 
     # Check validity of '--output' option if provided
     userOutSpec = [option.startswith("--output") or option.startswith("-o") for option in job_extra]
     if any(userOutSpec):
         userOut = job_extra[userOutSpec.index(True)]
         outSpec = userOut.split("=")
         if len(outSpec) != 2:
-            lgl = "the SLURM output directory must be specified using -o/--output=/path/to/file"
-            raise customValueError(legal=lgl if isSpyModule else "{} {}, not {}".format(funcName, lgl, userOut),
-                                   varname="job_extra",
-                                   actual=userOut)
+            msg = "SLURM output directory must be specified using -o/--output=/path/to/file, not %s"
+            log.error(msg, userOut)
+            raise ValueError("%s %s"%(funcName, msg%(userOut)))
         slurm_wdir = os.path.split(outSpec[1])[0]
-        if len(slurm_wdir) > 0:
-            if isSpyModule:
-                try:
-                    spy.shared.parsers.io_parser(slurm_wdir, varname="job_extra", isfile=False)
-                except Exception as exc:
-                    raise exc
-            else:
-                msg = "{} `slurmWorkingDirectory` has to be an existing directory, not {}"
-                if not os.path.isdir(os.path.expanduser(slurm_wdir)):
-                    raise ValueError(msg.format(funcName, str(slurm_wdir)))
+        if len(slurm_wdir) > 0 and not os.path.isdir(os.path.expanduser(slurm_wdir)):
+            msg = "SLURM output location has to be an existing directory, not %s"
+            log.error(msg, slurm_wdir)
+            raise ValueError("%s %s"%(funcName, msg%(slurm_wdir)))
+    else:
+        slurm_wdir = None
+    log.debug("Using `local_directory = %s`", slurm_wdir)
 
     # Create `SLURMCluster` object using provided parameters
+    log.debug("Instantiating `SLURMCluster` object")
     cluster = SLURMCluster(cores=n_cores,
-                           memory=mem_per_job,
-                           processes=workers_per_job,
+                           memory=mem_per_worker,
+                           processes=processes_per_worker,
                            local_directory=slurm_wdir,
                            queue=partition,
                            python=sys.executable,
-                           header_skip=["-t", "--mem"],
-                           job_extra=job_extra)
+                           job_directives_skip=["-t", "--mem"],
+                           job_extra_directives=job_extra)
                            # interface="asdf", # interface is set via `psutil.net_if_addrs()`
 
     # Compute total no. of workers and up-scale cluster accordingly
-    total_workers = n_jobs * workers_per_job
-    worker_count = min(total_workers, n_jobs_startup)
-    if worker_count < total_workers:
-        # cluster.adapt(minimum=worker_count, maximum=total_workers)
-        cluster.scale(total_workers)
-        msg = "{} Requested job-count {} exceeds `n_jobs_startup`: " +\
-            "waiting for {} jobs to come online, then proceed"
-        customPrint(msg.format(funcName, total_workers, n_jobs_startup))
-    else:
-        cluster.scale(total_workers)
+    if n_workers_startup < n_workers:
+        msg = "Requested worker-count %d exceeds `n_workers_startup = %d`, " +\
+            "waiting for %d workers to come online"
+        log.debug(msg, n_workers, n_workers_startup, n_workers_startup)
+    cluster.scale(n_workers)
 
-    # Fire up waiting routine to avoid unfinished cluster setups
-    if _cluster_waiter(cluster, funcName, worker_count, timeout, interactive, interactive_wait):
+    # Fire up waiting routine to avoid returning an undercooked cluster
+    if _cluster_waiter(cluster, funcName, n_workers, timeout, interactive, interactive_wait):
         return
 
     # Kill a zombie cluster in non-interactive mode
-    if not interactive and _count_running_workers(cluster) == 0:
+    if not interactive and count_online_workers(cluster) == 0:
         cluster.close()
-        err = "SLURM jobs could not be started within given time-out " +\
-              "interval of {0:d} seconds"
-        raise TimeoutError(err.format(timeout))
+        msg = "SLURM workers could not be started within given time-out " +\
+              "interval of %d seconds"
+        log.error(msg, timeout)
+        raise TimeoutError("%s %s"%(funcName, msg%(timeout)))
 
     # Highlight how to connect to dask performance monitor
-    customPrint(_successMsg.format(name=funcName, dash=cluster.dashboard_link))
+    msg = "Parallel computing client ready, dashboard accessible at %s"
+    log.info(msg, cluster.dashboard_link)
 
     # If client was requested, return that instead of the created cluster
     if start_client:
         return Client(cluster)
     return cluster
 
 
-def _get_slurm_partitions(funcName):
+def _get_slurm_partitions():
     """
-    Coming soon...
+    Local helper to fetch all partitions defined in SLURM
     """
 
+    # For later reference: dynamically fetch name of current function
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
+
     # Retrieve all partitions currently available in SLURM
+    log.debug("Use `sinfo` to fetch available partitions")
     proc = subprocess.Popen("sinfo -h -o %P",
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                             text=True, shell=True)
     out, err = proc.communicate()
 
     # Any non-zero return-code means SLURM is not ready to use
     if proc.returncode != 0:
-        msg = "{preamble:s}SLURM queuing system from node {node:s}. " +\
-              "Original error message below:\n{error:s}"
-        raise customIOError(msg.format(preamble=funcName + " Cannot access " if not isSpyModule else "",
-                                       node=socket.gethostname(),
-                                       error=err))
+        msg = "Error fetching SLURM partition setup from node %s: %s"
+        log.error(msg, socket.gethostname(), err)
+        raise IOError("%s %s"%(funcName, msg%(socket.gethostname(), err)))
 
     # Return formatted subprocess shell output
+    log.debug("Found partitions: %s", out)
     return out.split()
 
 
 def _cluster_waiter(cluster, funcName, total_workers, timeout, interactive, interactive_wait):
     """
     Local helper that can be called recursively
     """
 
-    # Re-direct printing/warnings to ACME logger outside SyNCoPy
-    customPrint, _ = _logging_setup()
-
     # Wait until all workers have been started successfully or we run out of time
-    wrkrs = _count_running_workers(cluster)
+    wrkrs = count_online_workers(cluster)
     to = str(timedelta(seconds=timeout))[2:]
     fmt = "{desc}: {n}/{total} \t[elapsed time {elapsed} | timeout at " + to + "]"
     ani = tqdm(desc="{} SLURM workers ready".format(funcName), total=total_workers,
                leave=True, bar_format=fmt, initial=wrkrs, position=0)
     counter = 0
-    while _count_running_workers(cluster) < total_workers and counter < timeout:
+    while count_online_workers(cluster) < total_workers and counter < timeout:
         time.sleep(1)
         counter += 1
-        ani.update(max(0, _count_running_workers(cluster) - wrkrs))
-        wrkrs = _count_running_workers(cluster)
+        ani.update(max(0, count_online_workers(cluster) - wrkrs))
+        wrkrs = count_online_workers(cluster)
         ani.refresh()   # force refresh to display elapsed time every second
     ani.close()
 
     # If we ran out of time before all workers could be started, ask what to do
     if counter == timeout and interactive:
-        msg = "{name:s} SLURM jobs could not be started within given time-out " +\
-              "interval of {time:d} seconds"
-        customPrint(msg.format(name=funcName, time=timeout))
+        msg = "SLURM workers could not be started within given time-out " +\
+              "interval of %d seconds"
+        log.info(msg, timeout)
         query = "{name:s} Do you want to [k]eep waiting for 60s, [a]bort or " +\
                 "[c]ontinue with {wrk:d} workers?"
         choice = user_input(query.format(name=funcName, wrk=wrkrs),
                             valid=["k", "a", "c"], default="c", timeout=interactive_wait)
 
         if choice == "k":
             return _cluster_waiter(cluster, funcName, total_workers, 60, True, 60)
         elif choice == "a":
-            customPrint("{} Closing cluster...".format(funcName))
+            log.info("Closing cluster...")
             cluster.close()
             return True
         else:
             if wrkrs == 0:
                 query = "{} Cannot continue with 0 workers. Do you want to " +\
                         "[k]eep waiting for 60s or [a]bort?"
                 choice = user_input(query.format(funcName), valid=["k", "a"],
                                     default="a", timeout=60)
                 if choice == "k":
                     _cluster_waiter(cluster, funcName, total_workers, 60, True, 60)
                 else:
-                    customPrint("{} Closing cluster...".format(funcName))
+                    log.info("Closing cluster...")
                     cluster.close()
                     return True
 
     return False
 
 
-def local_cluster_setup(interactive=True, start_client=True):
+def local_cluster_setup(n_workers=None,
+                        mem_per_worker=None,
+                        interactive=True,
+                        start_client=True):
     """
     Start a local distributed Dask multi-processing cluster
 
     Parameters
     ----------
+    n_workers : int
+        Number of local workers to start (this should align with the locally
+        available hardware, see :class:`distributed.LocalCluster` for details)
+    mem_per_worker : str
+        Memory cap for each local worker (corresponds to the `memory_limit`
+        keyword of a :class:`distributed.worker.Worker`)
     interactive : bool
         If `True`, a confirmation dialog is displayed to ensure proper encapsulation
         of calls to `local_cluster_setup` inside a script's main module block.
         See Notes for details. If `interactive` is `False`, the dialog is not shown.
     start_client : bool
         If `True`, a distributed computing client is launched and attached to
         the workers. If `start_client` is `False`, only a distributed
@@ -652,78 +697,85 @@
 
     The underlying distributed computing cluster can be accessed using
 
     >>> client.cluster
 
     See also
     --------
+    distributed.LocalCluster : create local worker cluster
     esi_cluster_setup : Start a distributed Dask cluster using SLURM
-    cluster_cleanup : remove dangling parallel processing job-clusters
+    cluster_cleanup : remove dangling parallel processing worker-clusters
     """
 
-    # Re-direct printing/warnings to ACME logger outside of SyNCoPy
-    customPrint, _ = _logging_setup()
-
     # For later reference: dynamically fetch name of current function
-    funcName = "{pre:s}<{pkg:s}{name:s}>".format(pre="Syncopy " if isSpyModule else "",
-                                                 pkg="ACME: " if isSpyModule else "",
-                                                 name=inspect.currentframe().f_code.co_name)
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
 
     # Determine if cluster allocation is happening interactively
     if not isinstance(interactive, bool):
-        msg = "{} `interactive` has to be Boolean, not {}"
-        raise customTypeError(interactive if isSpyModule else msg.format(funcName, str(interactive)),
-                              varname="interactive",
-                              expected="bool")
+        msg = "`interactive` has to be Boolean, not %s"
+        log.error(msg, str(type(interactive)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(interactive)))))
+    log.debug("Using `interactive = %s`", str(interactive))
 
     # Determine if a dask client was requested
     if not isinstance(start_client, bool):
-        msg = "{} `start_client` has to be Boolean, not {}"
-        raise customTypeError(start_client if isSpyModule else msg.format(funcName, str(start_client)),
-                              varname="start_client",
-                              expected="bool")
+        msg = "`start_client` has to be Boolean, not $s"
+        log.error(msg, str(type(start_client)))
+        raise TypeError("%s %s"%(funcName, msg%(str(type(start_client)))))
+    log.debug("Using `start_client = %s`", str(start_client))
 
     # Check, if we're running inside a Jupyter notebook...
     try:
         ipy = get_ipython()
         if ipy.__class__.__name__ == "ZMQInteractiveShell":
             maybeScript = False # Jupyter Notebook
+            log.debug("Running in a Jupyter Notebook")
         else:
             maybeScript = True  # iPython shell
+            log.debug("Running in an iPython shell")
     except NameError:
         maybeScript = True      # Python shell
+        log.debug("Running in a standard Python shell")
 
     # ...if not, print warning/info message
     if maybeScript:
         msg = """\
-        {name:s}If you use a script to start a local parallel computing client, please ensure
+        If you use a script to start a local parallel computing client, please ensure
         the call to `local_cluster_setup` is wrapped inside a main module block, i.e.,
 
             if __name__ == "__main__":
                 ...
                 local_cluster_setup()
                 ...
 
         Otherwise, a RuntimeError is raised due to an infinite recursion triggered by
         new processes being started before the calling process can finish its bootstrapping
         phase.
         """
-        customPrint(textwrap.dedent(msg.format(name=funcName + " " if not isSpyModule else "")))
+        msg = textwrap.dedent(msg)
+        log.debug(msg)
 
     # Additional safe-guard: if a script is executed, double-check with the user
     # for proper main idiom usage
     if interactive:
-        msg = "{name:s}If launched from a script, did you wrap your code inside a main module block?"
-        if not user_yesno(msg.format(name=funcName + " " if not isSpyModule else ""), default="no"):
+        msg = "{name:s} If launched from a script, did you wrap your code " +\
+            "inside a __main__ module block?"
+        if not user_yesno(msg.format(name=funcName), default="no"):
             return
 
     # Start the actual distributed client
-    client = Client()
-    successMsg = "{name:s} Local parallel computing client ready. \n" + _successMsg
-    customPrint(successMsg.format(name=funcName, dash=client.cluster.dashboard_link))
+    if n_workers is not None or mem_per_worker is not None:
+        msg = "Starting `LocalCluster` with `n_workers = %s` and `memory_limit = %s`"
+        log.debug(msg, str(n_workers), str(mem_per_worker))
+        cluster = LocalCluster(n_workers=n_workers, memory_limit=mem_per_worker)
+        client = Client(cluster)
+    else:
+        client = Client()
+    msg = "Local parallel computing client ready, dashboard accessible at %s"
+    log.info(msg, client.cluster.dashboard_link)
     if start_client:
         return client
     return client.cluster
 
 
 def cluster_cleanup(client=None):
     """
@@ -739,85 +791,57 @@
     Returns
     -------
     Nothing : None
 
     See also
     --------
     esi_cluster_setup : Launch SLURM workers on the ESI compute cluster
+    slurm_cluster_setup : start a distributed Dask cluster of parallel processing workers using SLURM
+    local_cluster_setup : start a local Dask multi-processing cluster on the host machine
     """
 
-    # Re-direct printing/warnings to ACME logger outside SyNCoPy
-    customPrint, customWarning = _logging_setup()
-
     # For later reference: dynamically fetch name of current function
-    funcName = "{pre:s}<{pkg:s}{name:s}>".format(pre="Syncopy " if isSpyModule else "",
-                                                 pkg="ACME: " if isSpyModule else "",
-                                                 name=inspect.currentframe().f_code.co_name)
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
 
     # Attempt to establish connection to dask client
     if client is None:
         try:
             client = get_client()
         except ValueError:
-            msg = "{name:s}No dangling clients or clusters found."
-            customWarning(msg.format(name="" if isSpyModule else funcName + " "),
-                          RuntimeWarning,
-                          __file__,
-                          inspect.currentframe().f_lineno)
+            log.warning("No dangling clients or clusters found.")
             return
         except Exception as exc:
+            log.error("Error looking for dask client")
             raise exc
     else:
         if not isinstance(client, Client):
-            msg = "{} `client` has to be a dask client object, not {}"
-            customTypeError(client if isSpyModule else msg.format(funcName, str(client)),
-                            varname="client",
-                            expected="dask client object")
+            msg = "`client` has to be a dask client object, not %s"
+            log.error(msg, str(type(client)))
+            raise TypeError("%s %s"%(funcName, msg%(str(type(client)))))
+    log.debug("Found client %s", str(client))
 
     # Prepare message for prompt
     if client.cluster.__class__.__name__ == "LocalCluster":
         userClust = "LocalCluster hosted on {}".format(client.scheduler_info()["address"])
     else:
         userName = getpass.getuser()
         outDir = client.cluster.job_header.partition("--output=")[-1]
         jobID = outDir.partition("{}_".format(userName))[-1].split(os.sep)[0]
         userClust = "cluster {0}_{1}".format(userName, jobID)
-    nWorkers = len(client.cluster.workers)
+    nWorkers = count_online_workers(client.cluster)
 
     # If connection was successful, first close the client, then the cluster
     client.close()
     client.cluster.close()
 
     # Communicate what just happened and get outta here
-    msg = "{fname:s} Successfully shut down {cname:s} containing {nj:d} workers"
-    customPrint(msg.format(fname=funcName,
-                     nj=nWorkers,
-                     cname=userClust))
+    msg = "Successfully shut down %s containing %d workers"
+    log.info(msg, userClust, nWorkers)
 
     return
 
 
-def _count_running_workers(cluster):
+def count_online_workers(cluster):
     """
     Local replacement for the late `._count_active_workers` class method
     """
-    return len(cluster.scheduler_info.get('workers'))
-
-
-def _logging_setup():
-    """
-    Local helper to customize warning and print functionality at runtime
-    """
-    if isSpyModule:
-        pFunc = print
-        wFunc = lambda msg, kind, caller, lineno : spy.shared.errors.SPYWarning(msg, caller=caller)
-    else:
-        pFunc = print
-        wFunc = showwarning
-        allLoggers = list(logging.root.manager.loggerDict.keys())
-        idxList = [allLoggers.index(loggerName) for loggerName in allLoggers \
-            for moduleName in ["ACME", "ParallelMap"] if moduleName in loggerName]
-        if len(idxList) > 0:
-            logger = logging.getLogger(allLoggers[idxList[0]])
-            pFunc = logger.info
-            wFunc = lambda msg, kind, caller, lineno: logger.warning(msg)
-    return pFunc, wFunc
+    return len([w["memory_limit"] for w in cluster.scheduler_info["workers"].values()])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/frontend.py` & `esi-acme-2023.4/acme/frontend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,58 @@
-# -*- coding: utf-8 -*-
 #
 # User-exposed interface of acme
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import inspect
-import sys
 import numpy as np
-import dask.array as da
+import logging
 
 # Local imports
+from acme import __deprecated__, __deprecation_wrng__, __version__
 from .backend import ACMEdaemon
+from .logger import prepare_log
+from .shared import _scalar_parser, sizeOf
 from . import shared as acs
-isSpyModule = False
-if "syncopy" in sys.modules:
-    isSpyModule = True
 
 __all__ = ["ParallelMap"]
 
+# Fetch logger
+log = logging.getLogger("ACME")
+
 
 # Main context manager for parallel execution of user-defined functions
 class ParallelMap(object):
 
-    msgName = "{pre:s}<{pkg:s}ParallelMap>".format(pre="Syncopy " if isSpyModule else "",
-                                                   pkg="ACME: " if isSpyModule else "")
+    objName = "<ParallelMap>"
     argv = None
     kwargv = None
     func = None
     n_inputs = None
-    log = None
     _maxArgSize = 1024
 
     def __init__(
         self,
         func,
         *args,
         n_inputs="auto",
         write_worker_results=True,
+        output_dir=None,
+        result_shape=None,
+        result_dtype="float",
+        single_file=False,
         write_pickle=False,
         partition="auto",
-        n_jobs="auto",
-        mem_per_job="auto",
+        n_workers="auto",
+        mem_per_worker="auto",
         setup_timeout=60,
         setup_interactive=True,
         stop_client="auto",
         verbose=None,
         dryrun=False,
         logfile=None,
         **kwargs):
@@ -52,94 +60,133 @@
         Context manager that executes user-defined functions in parallel
 
         Parameters
         ----------
         func : callable
             User-defined function to be executed concurrently. Input arguments
             and return values should be "simple" (i.e., regular Python objects or
-            NumPy arrays). See Notes for more information and Examples for
-            details.
+            NumPy arrays). See Examples and [1]_ for more information.
         args : arguments
             Positional arguments of `func`. Should be regular Python objects
-            (lists, tuples, scalars, strings etc.) or NumPy arrays. See Notes
-            for more information and Examples for details.
+            (lists, tuples, scalars, strings etc.) or NumPy arrays. See
+            Examples and [1]_ for more information.
         kwargs : keyword arguments
             Keyword arguments of `func` (if any). Should be regular Python objects
-            (lists, tuples, scalars, strings etc.) or NumPy arrays. See Notes
-            for more information and Examples for details.
+            (lists, tuples, scalars, strings etc.) or NumPy arrays. See Examples
+            and [1]_ for more information.
         n_inputs : int or "auto"
             Number of times `func` is supposed to be called in parallel. Usually,
             `n_inputs` does not have to be provided explicitly. If `n_inputs` is
             `"auto"` (default) this quantity is inferred from provided `args` and
             `kwargs`. This estimation may fail due to ambiguous input arguments
             (e.g., `args` and/or `kwargs` contain lists of differing lengths)
             triggering a `ValueError`. Only then is it required to set `n_input`
-            manually. See Examples for details.
+            manually. See Examples and [1]_ for more information.
         write_worker_results : bool
-            If `True`, the return value(s) of `func` is/are saved on disk (one
-            HDF5 file per parallel worker). If `False`, the output of all parallel calls
-            of `func` is collected in memory. See Examples and Notes for details.
+            If `True`, the return value(s) of `func` is/are saved on disk.
+            If `False`, the output of all parallel calls of `func` is collected
+            in memory. See Examples as well as [1]_ and [2]_ for more information.
+        output_dir : str or None
+            Only relevant if `write_worker_results` is `True`. If `output_dir` is `None`
+            (default) and `write_worker_results` is `True`, all files auto-generated
+            by `ParallelMap` are stored in a directory `'ACME_YYYYMMDD-hhmmss-ffffff'`
+            (encoding the current time as YearMonthDay-HourMinuteSecond-Microsecond).
+            The path to a custom output directory can be specified via providing
+            `output_dir`. See Examples and [1]_ for more information.
+        result_shape : tuple or None
+            Only relevant if `write_pickle` is `False`. If provided, return
+            values of `func` are slotted into a (virtual) dataset (if
+            `write_worker_results` is True) or array (otherwise) of shape
+            `result_shape`, where a single `None` entry designates the stacking
+            dimension. For instance, ``result_shape = (None, 100)`` implies
+            that `func` returns a 100-element array which is to be stacked
+            along the first dimension for each concurrent call of `func`
+            resulting in a ``(n_inputs, 100)`` dataset or array. See Notes
+            and Examples for details. See Examples as well as [1]_ and [2]_
+            for more information.
+        result_dtype : str or None
+            Only relevant if `result_shape` is not `None`. If provided, determines
+            the numerical datatype of the dataset laid out by `result_shape`.
+            By default, results are stored in `float64` format. See [2]_ for
+            more details.
+        single_file : bool
+            Only relevant if `write_worker_results` is `True` and `write_pickle`
+            is `False`. If `single_file` is `False` (default), the results of each parallel
+            call of `func` are stored in dedicated HDF5 files, such that the auto-
+            generated HDF5 results-container is a collection of symbolic links
+            pointing to these files.
+            Conversely, if `single_file` is `True`, all parallel workers
+            write to the same results container (using a distributed file-locking
+            mechanism). See [2]_ for more details.
         write_pickle : bool
-            If `True`, the return value(s) of `func` is/are pickled to disk (one
-            `'.pickle'`-file per parallel worker). Only effective if `write_worker_results`
-            is `True`.
+            Only relevant if `write_worker_results` is `True`. If `True`,
+            the return value(s) of `func` is/are pickled to disk (one
+            `'.pickle'`-file per parallel worker). See Examples as well as
+            [1]_ and [2]_ for more information.
         partition : str
             Name of SLURM partition to use. If `"auto"` (default), the memory footprint
             of `func` is estimated using dry-run stubs based on randomly sampling
             provided `args` and `kwargs`. Estimated memory usage dictates queue
             auto-selection under the assumption of short run-times (**currently only
             supported on the ESI HPC cluster**). For instance, on a predicted memory
             footprint of 6 GB causes the `"8GBXS"` partition to be selected (minimal
             but sufficient memory and shortest runtime).
             To override auto-selection, provide name of SLURM queue explicitly. See, e.g.,
             :func:`~acme.esi_cluster_setup` for details.
-        n_jobs : int or "auto"
-            Number of SLURM jobs (=workers) to spawn. If `"auto"` (default), then
-            ``n_jobs = n_inputs``, i.e., every SLURM worker performs a single
+        n_workers : int or "auto"
+            Number of SLURM workers (=jobs) to spawn. If `"auto"` (default), then
+            ``n_workers = n_inputs``, i.e., every SLURM worker performs a single
             call of `func`.
             If `n_inputs` is large and executing `func` is fast, setting
-            ``n_jobs = int(n_inputs / 2)`` might be beneficial. See Notes for details.
-        mem_per_job : str
+            ``n_workers = int(n_inputs / 2)`` might be beneficial. See Examples
+            as well as [1]_ and [2]_ for more information.
+        mem_per_worker : str
             Memory booking for each SLURM worker. If `"auto"` (default), the standard
-            value is inferred from the used partition (if possible). See, e.g.,
-            :func:`~acme.esi_cluster_setup` for details.
+            value is inferred from the used partition (if possible). See
+            :func:`~acme.slurm_cluster_setup` for details.
         setup_timeout : int
-            Timeout period (in seconds) for SLURM workers to come online. See, e.g.,
-            :func:`~acme.esi_cluster_setup` for details.
+            Timeout period (in seconds) for SLURM workers to come online. Refer to
+            keyword `timeout` in :func:`~acme.slurm_cluster_setup` for details.
         setup_interactive : bool
             If `True` (default), user input is queried in case not enough SLURM
             workers could be started within `setup_timeout` seconds. If no input
             is provided, the current number of spawned workers is used (even if
-            smaller than the amount requested by `n_jobs`). If `False`, no user
-            choice is requested.
+            smaller than the amount requested by `n_workers`). If `False`, no user
+            choice is requested. Refer to keyword `interactive` in :func:`~acme.slurm_cluster_setup`
         stop_client : bool or "auto"
             If `"auto"` (default), automatically started distributed computing clients
             are shut down at the end of computation, while user-provided clients
             are left untouched. If `False`, automatically started clients are
             left running after completion, user-provided clients are left untouched.
             If `True`, auto-generated clients *and* user-provided clients are
-            shut down at the end of the computation.
+            shut down at the end of the computation. See Examples as well
+            as [1]_ and [2]_ for more information.
         verbose : None or bool
             If `None` (default), general run-time information as well as warnings
             and errors are shown. If `True`, additionally debug information is
             shown. If `False`, only warnings and errors are propagated.
+            See [2]_ for more details.
         dryrun : bool
             If `True` the user-provided function `func` is executed once using
             one of the input argument tuples prepared for the parallel workers (picked
             at random). If `setup_interactive` is `True`, a prompt asks if the
             actual parallel execution of `func` is supposed to be launched after the
             dry-run. The `dryrun` keyword is intended to to estimate memory consumption
             as well as runtime of worker jobs prior to the actual concurrent
-            computation.
+            computation. See [1]_ and [2]_ for more information.
         logfile : None or bool or str
-            If `None` (default) or `False`, all run-time information as well as errors and
-            warnings are printed to the command line only. If `True`, an auto-generated
-            log-file is set up that records run-time progress. Alternatively, the
-            name of a custom log-file can be provided (must not exist). The verbosity
-            of recorded information can be controlled via setting `verbose`.
+            If `None` (default) and ``write_worker_results = True``,
+            a logfile is created alongside the auto-generated on-disk results.
+            If `None` and ``write_worker_results = False``, no logfile is
+            created. To override this mechanism, either explicitly set
+            `logfile` to `True` or `False` to enforce or suppress logfile
+            creation.
+            Alternatively, the name of a custom log-file can be provided.
+            The verbosity of recorded runtime information can be controlled
+            via setting `verbose`. See [2]_ for more details.
 
         Returns
         -------
         results : list
             If `write_worker_results` is `True`, `results` is a list of HDF5 file-names
             containing computed results. If `write_worker_results` is `False`,
             results is a list comprising the actual return values of `func`.
@@ -170,65 +217,93 @@
 
             with ParallelMap(f, [2, 4, 6, 8], y, n_inputs=4, write_worker_results=False) as pmap:
                 results = pmap.compute()
 
         More examples and tutorials are available in the
         `ACME online documentation <https://esi-acme.readthedocs.io>`_.
 
+        Notes
+        -----
+        Please consult [1]_ for detailed usage information.
+
         See also
         --------
         esi_cluster_setup : spawn custom SLURM worker clients on the ESI HPC cluster
         local_cluster_setup : start a local Dask multi-processing cluster on the host machine
         ACMEdaemon : Manager class performing the actual concurrent processing
+
+        References
+        ----------
+        .. [1] https://esi-acme.readthedocs.io/en/latest/userguide.html
+        .. [2] https://esi-acme.readthedocs.io/en/latest/advanced_usage.html
         """
 
-        # First and foremost, set up logging system (unless logger is already present)
-        self.log = acs.prepare_log(func, caller=self.msgName, logfile=logfile, verbose=verbose)
+        # First and foremost, set up logging system - logfile is processed later
+        prepare_log(logname="ACME", verbose=verbose)
+        log.announce("This is ACME v. %s", __version__)
+
+        # Backwards compatibility: legacy keywords are converted to new nomenclature
+        if any(kw in kwargs for kw in __deprecated__):
+            log.warning(__deprecation_wrng__)
+            n_workers = kwargs.pop("n_jobs", n_workers)
+            mem_per_worker = kwargs.pop("mem_per_job", mem_per_worker)
+            log.debug("Set `n_workers = n_jobs` and \
+                       mem_per_worker = mem_per_job`")
 
         # Either guess `n_inputs` or use provided value to duplicate input args
         # and set class attributes `n_inputs`, `argv` and `kwargv`
         self.prepare_input(func, n_inputs, *args, **kwargs)
 
         # Create an instance of `ACMEdaemon` that does the actual parallel computing work
+        log.debug("Instantiating `ACMEdaemon`")
         self.daemon = ACMEdaemon(self,
-                                 n_jobs=n_jobs,
+                                 n_workers=n_workers,
                                  write_worker_results=write_worker_results,
+                                 output_dir=output_dir,
+                                 result_shape=result_shape,
+                                 result_dtype=result_dtype,
+                                 single_file=single_file,
                                  write_pickle=write_pickle,
                                  dryrun=dryrun,
                                  partition=partition,
-                                 mem_per_job=mem_per_job,
+                                 mem_per_worker=mem_per_worker,
                                  setup_timeout=setup_timeout,
                                  setup_interactive=setup_interactive,
-                                 stop_client=stop_client)
+                                 stop_client=stop_client,
+                                 verbose=verbose,
+                                 logfile=logfile)
 
     def prepare_input(self, func, n_inputs, *args, **kwargs):
         """
         User input parser
 
         Ensure `func` can actually process provided arguments. If `n_inputs` was
         not set, attempt to infer the number of required concurrent function
         calls from `args` and `kwargs`. In addition, ensure the size of each
         argument is "reasonable" for propagation across multiple workers.
         """
 
         # Ensure `func` really is a function and `n_inputs` makes sense
         if not callable(func):
-            msg = "{} first input has to be a callable function, not {}"
-            raise TypeError(msg.format(self.msgName, str(type(func))))
-        msg = "{} `n_inputs` has to be 'auto' or an integer >= 2, not {}"
+            msg = "%s first input has to be a callable function, not %s"
+            raise TypeError(msg%(self.objName, str(type(func))))
         if isinstance(n_inputs, str):
             if n_inputs != "auto":
-                raise ValueError(msg.format(self.msgName, n_inputs))
+                msg = "%s `n_inputs` has to be 'auto' or an integer >= 2, not %s"
+                raise ValueError(msg%(self.objName, n_inputs))
             guessInputs = True
+            log.debug("Using `n_inputs = 'auto'`")
         else:
             try:
-                acs._scalar_parser(n_inputs, varname="n_inputs", ntype="int_like", lims=[1, np.inf])
+                _scalar_parser(n_inputs, varname="n_inputs", ntype="int_like", lims=[1, np.inf])
             except Exception as exc:
+                log.error("Error parsing `n_inputs`")
                 raise exc
             guessInputs = False
+            log.debug("Using provided `n_inputs = %d`", n_inputs)
 
         # Get `func`'s signature to extract its positional/keyword arguments
         funcSignature = inspect.signature(func)
         funcPosArgs = [name for name, value in funcSignature.parameters.items()\
             if value.default is value.empty and value.name != "kwargs"]
         funcKwargs = [name for name, value in funcSignature.parameters.items()\
             if value.default is not value.empty]
@@ -238,151 +313,166 @@
         posArgNames = []
         for name, value in kwargs.items():
             if name in funcPosArgs:
                 args.insert(funcPosArgs.index(name), value)
                 posArgNames.append(name)
         for name in posArgNames:
             kwargs.pop(name)
+            log.debug("Moved %s from `kwargs` to positional args", name)
 
         # If "taskID" is a keyword arg, include/overwrite it in `kwargs` - the rest
         # is done by `ACMEdaemon`
         if "taskID" in funcKwargs:
             kwargs["taskID"] = None
+            log.debug("Found `taskID` in kwargs - overriding it")
 
         # Compare provided `args`/`kwargs` to actually defined quantities in `func`
         if len(args) != len(funcPosArgs):
-            msg = "{} {} expects {} positional arguments ({}), found {}"
+            msg = "%s %s expects %d positional arguments (%s), found %d"
             validArgs = "'" + "'".join(arg + "', " for arg in funcPosArgs)[:-2]
-            raise ValueError(msg.format(self.msgName,
-                                        func.__name__,
-                                        len(funcPosArgs),
-                                        validArgs,
-                                        len(args)))
+            raise ValueError(msg%(self.objName,
+                                  func.__name__,
+                                  len(funcPosArgs),
+                                  validArgs,
+                                  len(args)))
         if len(kwargs) > len(funcKwargs):
-            msg = "{} {} accepts at maximum {} keyword arguments ({}), found {}"
+            msg = "%s %s accepts at maximum %d keyword arguments (%s), found %d"
             validArgs = "'" + "'".join(arg + "', " for arg in funcKwargs)[:-2]
-            raise ValueError(msg.format(self.msgName,
-                                        func.__name__,
-                                        len(funcKwargs),
-                                        validArgs,
-                                        len(kwargs)))
+            raise ValueError(msg%(self.objName,
+                                  func.__name__,
+                                  len(funcKwargs),
+                                  validArgs,
+                                  len(kwargs)))
 
         # Prepare argument parsing: collect the the length of anything 1D-array-like
         # in `argLens` and check the size of all provided positional and keyword args
         argLens = []
-        wrnMsg = "argument size {0:4.2f} MB exceeds recommended limit of {1} MB. " +\
+        wrnMsg = "argument size %4.2f MB exceeds recommended limit of %d MB. " +\
             "Distributing large variables across workers may result in poor performance. "
 
         # Cycle through positional args
         for k, arg in enumerate(args):
             if isinstance(arg, range):
                 arg = list(arg)
                 args[k] = arg
             acs.callCount = 0
-            argsize = acs.sizeOf(arg, "positional arguments")
+            argsize = sizeOf(arg, "positional arguments")
+            log.debug("Computed size of pos arg #%d as %4.2f bytes", k, argsize)
             if argsize > self._maxArgSize:
-                self.log.warning(wrnMsg.format(argsize, self._maxArgSize))
+                log.warning(wrnMsg, argsize, self._maxArgSize)
             if isinstance(arg, (list, tuple)):
                 argLens.append(len(arg))
             elif isinstance(arg, np.ndarray):
                 if len(arg.squeeze().shape) == 1:
                     argLens.append(arg.squeeze().size)
 
         # More complicated for keyword args: if provided value is 1D-array-like and
         # default value is not, interpret is as worker-arg list, and track its length
         for name, value in kwargs.items():
             defaultValue = funcSignature.parameters[name].default
             if isinstance(value, range):
                 value = list(value)
                 kwargs[name] = value
             acs.callCount = 0
-            valsize = acs.sizeOf(value, "keyword arguments")
+            valsize = sizeOf(value, "keyword arguments")
+            log.debug("Computed size of %s as %4.2f bytes", name, valsize)
             if valsize > self._maxArgSize:
-                self.log.warning(wrnMsg.format(valsize, self._maxArgSize))
+                log.warning(wrnMsg, valsize, self._maxArgSize)
             if isinstance(value, (list, tuple)):
                 if isinstance(defaultValue, (list, tuple)):
                     if len(defaultValue) != len(value):
                         argLens.append(len(value))
                 else:
                     argLens.append(len(value))
             elif isinstance(value, np.ndarray) and not isinstance(defaultValue, np.ndarray):
                 if len(value.squeeze().shape) == 1:
                     argLens.append(value.squeeze().size)
 
         # If `n_input` is `"auto"`, make an educated guess as to how many parallel
         # executions of `func` are intended; if input args contained multiple
         # 1D-array-likes, pump the brakes. If `n_input` was explicitly provided,
-        # ensure at least one input argument actually contains `n_input` elements
-        # for distribution across parallel workers
+        # either all input arguments must have unit length (or are nd-arrays)
+        # or at at least one input argument actually contains `n_input` elements
         if guessInputs:
-            if len(set(argLens)) > 1:
-                msg = "{} automatic input distribution failed: found {} objects " +\
-                    "containing {} to {} elements. Please specify `n_inputs` manually. "
-                raise ValueError(msg.format(self.msgName, len(argLens), min(argLens), max(argLens)))
+            if len(set(argLens)) > 1 or len(argLens) == 0:
+                msg = "%s automatic input distribution failed: found %d objects " +\
+                    "containing %d to %d elements. Please specify `n_inputs` manually. "
+                raise ValueError(msg%(self.objName,
+                                      len(argLens),
+                                      min(argLens, default=0),
+                                      max(argLens, default=0)))
             n_inputs = argLens[0]
         else:
-            if n_inputs not in set(argLens):
-                msg = "{} No object has required length of {} matching `n_inputs`. "
-                raise ValueError(msg.format(self.msgName, n_inputs))
+            if n_inputs not in set(argLens) and not all(arglen == 1 for arglen in argLens):
+                msg = "%s No object has required length of %d matching `n_inputs`. "
+                raise ValueError(msg%(self.objName, n_inputs))
         self.n_inputs = int(n_inputs)
+        log.debug("Inferred `n_inputs = %d`", n_inputs)
 
         # Anything that does not contain `n_input` elements is converted to a one-element list
         wrnMsg = "Found a single callable object in positional arguments. " +\
             "It will be executed just once and shared by all workers"
         self.argv = list(args)
         for ak, arg in enumerate(args):
             if isinstance(arg, (list, tuple)):
                 if len(arg) == self.n_inputs:
                     continue
             elif isinstance(arg, np.ndarray):
                 if len(arg.squeeze().shape) == 1 and arg.squeeze().size == self.n_inputs:
                     continue
             elif callable(arg):
-                self.log.warning(wrnMsg)
+                log.warning(wrnMsg)
             self.argv[ak] = [arg]
 
         # Same for keyword arguments with the caveat that default values have to
         # be taken into account (cf. above)
-        wrnMsg = "Found a single callable object in keyword arguments: {}. " +\
+        wrnMsg = "Found a single callable object in keyword arguments: %s. " +\
             "It will be executed just once and shared by all workers"
         self.kwargv = dict(kwargs)
         for name, value in kwargs.items():
             if isinstance(value, (list, tuple)):
                 if len(value) == self.n_inputs:
                     continue
             elif isinstance(value, np.ndarray) and \
                 not isinstance(funcSignature.parameters[name].default, np.ndarray):
                 if len(value.squeeze().shape) == 1 and value.squeeze().size == self.n_inputs:
                     continue
             elif callable(value):
-                self.log.warning(wrnMsg.format(name))
+                log.warning(wrnMsg, name)
             self.kwargv[name] = [value]
 
         # Finally, attach user-provided function to class instance
         self.func = func
 
+        # Get out
+        return
+
     def compute(self):
         """
         Shortcut to launch parallel computation via `ACMEdaemon`
         """
+        log.debug("Invoking `compute` method")
         if hasattr(self, "daemon"):
             self.daemon.compute()
 
     def cleanup(self):
         """
         Shortcut to corresponding cleanup-routine provided by `ACMEdaemon`
         """
+        log.debug("Invoking `cleanup` method")
         if hasattr(self, "daemon"):
-            self.daemon.cleanup
+            self.daemon.cleanup()
 
     def __enter__(self):
         """
         If `ParallelMap` is used as context manager, launch `ACMEdaemon`
         """
+        log.debug("Entering `ACMEdaemon` context")
         return self.daemon
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         """
         If `ParallelMap` is used as context manager, close any ad-hoc computing
         clients created by `ACMEdaemon`
         """
+        log.debug("Exiting `ACMEdaemon` context")
         self.daemon.cleanup()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/shared.py` & `esi-acme-2023.4/acme/shared.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-# -*- coding: utf-8 -*-
 #
 # Auxiliaries needed across the entire package
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import os
 import sys
 import socket
 import subprocess
 import inspect
 import logging
-import warnings
-import datetime
+import traceback
 import multiprocessing
 import time
 import numpy as np
 import dask.distributed as dd
 from tqdm import tqdm
+from logging import handlers
 
-# from .dask_helpers import cluster_cleanup
+# Local imports
+from acme import __version__
 from . import dask_helpers as dh
 
 callCount = 0
-callMax = 50000
+callMax = 1000000
 
 __all__ = []
 
 
 def sizeOf(obj, varname):
     """
     Estimate memory consumption of Python objects
@@ -48,20 +53,22 @@
     depth. This method was inspired by a routine in
     `Nifty <https://github.com/mwojnars/nifty/blob/master/util.py>`_.
     """
 
     # Keep track of the no. of recursive calls
     global callCount
 
+    # For later reference: dynamically fetch name of current function
+    funcName = "<{}>".format(inspect.currentframe().f_code.co_name)
+
     # Protect against circular object references
     callCount += 1
     if callCount >= callMax:
-        msgName = sys._getframe().f_back.f_code.co_name
-        msg = "{} maximum recursion depth {} exceeded when processing {}"
-        raise RecursionError(msg.format(msgName, callMax, varname))
+        msg = "%s maximum recursion depth %s exceeded while processing %s"
+        raise RecursionError(msg%(funcName, callMax, varname))
 
     # Use `sys.getsizeof` to estimate memory consumption of primitive objects
     objsize = sys.getsizeof(obj) / 1024**2
     if isinstance(obj, dict):
         return objsize + sum(list(map(sizeOf, obj.keys(), [varname] * len(obj.keys())))) + sum(list(map(sizeOf, obj.values(), [varname] * len(obj.values()))))
     if isinstance(obj, (list, tuple, set)):
         return objsize + sum(list(map(sizeOf, obj, [varname] * len(obj))))
@@ -70,58 +77,66 @@
 
 def is_slurm_node():
     """
     Returns `True` if code is running on a SLURM-managed cluster node, `False`
     otherwise
     """
 
+    # Fetch ACME logger
+    log = logging.getLogger("ACME")
+
     # Simply test if the srun command is available
+    log.debug("Test if `sinfo` is available")
     out, _ = subprocess.Popen("sinfo --version",
                               stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                               text=True, shell=True).communicate()
     return len(out) > 0
 
 
 def is_esi_node():
     """
     Returns `True` if code is running on an ESI cluster node, `False` otherwise
     """
+
+    # Fetch ACME logger and write debug message
+    log = logging.getLogger("ACME")
+    log.debug("Test if hostname matches the pattern 'esi-sv*'")
     return socket.gethostname().startswith("esi-sv") and os.path.isdir("/cs")
 
 
 def _scalar_parser(var, varname="varname", ntype="int_like", lims=[-np.inf, np.inf]):
     """
     ACME-specific version of Syncopy's `scalar_parser` (used for cross-compatibility)
     """
 
     # Get name of calling method/function
-    caller = "<{}>".format(inspect.currentframe().f_back.f_code.co_name)
+    funcName = "<{}>".format(inspect.currentframe().f_back.f_code.co_name)
 
     # Make sure `var` is a scalar-like number
-    msg = "{caller:s} `{varname:s}` has to be {scalartype:s} between {lower:s} and {upper:s}, not {var:s}"
+    msg = "%s `%s` has to be %s between %s and %s, not %s"
     if np.issubdtype(type(var), np.number):
         error = False
         if ntype == "int_like":
             scalartype = "an integer"
             if round(var) != var:
                 error = True
         else:
             scalartype = "a number"
         if var < lims[0] or var > lims[1]:
             error = True
         if error:
-            raise ValueError(msg.format(caller=caller,
-                                        varname=varname,
-                                        scalartype=scalartype,
-                                        lower=str(lims[0]),
-                                        upper=str(lims[1]),
-                                        var=str(var)))
+            raise ValueError(msg%(funcName,
+                                  varname,
+                                  scalartype,
+                                  str(lims[0]),
+                                  str(lims[1]),
+                                  str(var)))
     else:
-        msg = "{caller:s} `{varname:s}` has to be a scalar, not {var:s}"
-        raise TypeError(msg.format(caller=caller, varname=varname, var=str(var)))
+        msg = "%s `%s` has to be a scalar, not %s"
+        raise TypeError(msg%(funcName, varname, str(type(var))))
 
     return
 
 
 def user_yesno(msg, default=None):
     """
     ACME specific version of user-input query
@@ -212,111 +227,14 @@
     """
     Target routine to tie subprocess to (in case input-query is time-restricted)
     """
     sys.stdin = os.fdopen(stdin_fd)
     procQueue.put(_get_user_input(query, valid, default))
 
 
-def prepare_log(func, caller=None, logfile=False, verbose=None):
-    """
-    Convenience function to set up ACME logger
-
-    Parameters
-    ----------
-    func : callable
-        User-provided function to be called concurrently by ACME
-    caller : None or str
-        Routine/class that initiated logging (presumable :class:~`acme.ParallelMap`
-        or :class:~`acme.ACMEDaemon`)
-    logfile : None or bool or str
-        If `True` an auto-generated log-file is set up. If `logfile` is a string
-        it is interpreted as file-name for a new log-file (must not exist). If
-        `False` or `None` logging information is streamed to stdout only.
-    verbose : bool or None
-        If `None`, the logging-level only contains messages of `'INFO'` priority and
-        higher (`'WARNING'` and `'ERROR'`). If `verbose` is `True`, logging is
-        performed on ``DEBUG`', `'INFO`', `'WARNING'` and `'ERROR'` levels. If
-        `verbose` is `False` only `'WARNING'` and `'ERROR'` messages are propagated.
-
-    Returns
-    -------
-    log : logger object
-        A Python :class:`logging.Logger` instance
-    """
-
-    # If not provided, get name of calling method/function
-    if caller is None:
-        caller = "<{}>".format(inspect.currentframe().f_back.f_code.co_name)
-    elif not isinstance(caller, str):
-        msg = "{} `caller` has to be a string, not {}"
-        raise TypeError(msg.format(inspect.currentframe().f_back.f_code.co_name),
-                        str(caller))
-
-    # Basal sanity check for Boolean flag
-    if verbose is not None and not isinstance(verbose, bool):
-        msg = "{} `verbose` has to be `True`, `False` or `None`, not {}"
-        raise TypeError(msg.format(caller, str(verbose)))
-
-    # Either parse provided `logfile` or set up an auto-generated file
-    msg = "{} `logfile` has to be `None`, `True`, `False` or a valid file-name, not {}"
-    if logfile is None or isinstance(logfile, bool):
-        if logfile is True:
-            logfile = os.path.dirname(os.path.abspath(inspect.getfile(func)))
-            logfile = os.path.join(logfile, "ACME_{func:s}_{date:s}.log")
-            logfile = logfile.format(func=func.__name__,
-                                     date=datetime.datetime.now().strftime('%Y%m%d-%H%M%S'))
-        else:
-            logfile = None
-    elif isinstance(logfile, str):
-        if os.path.isdir(logfile):
-            raise IOError(msg.format(caller, "a directory"))
-        logfile = os.path.abspath(os.path.expanduser(logfile))
-    else:
-        raise TypeError(msg.format(caller, str(logfile)))
-    if logfile is not None and os.path.isfile(logfile):
-        msg = "{} log-file {} already exists, appending to it"
-        warnings.showwarning(msg.format(caller, logfile), RuntimeWarning,
-                             __file__, inspect.currentframe().f_lineno)
-
-    # Set logging verbosity based on `verbose` flag
-    if verbose is None:
-        loglevel = logging.INFO
-    elif verbose is True:
-        loglevel = logging.DEBUG
-    else:
-        loglevel = logging.WARNING
-    log = logging.getLogger(caller)
-    log.setLevel(loglevel)
-
-    # Create logging formatter
-    formatter = logging.Formatter("%(name)s %(levelname)s: %(message)s")
-
-    # Output handlers: print log messages to `stderr` via `StreamHandler` as well
-    # as to a provided text file `logfile using a `FileHandler`.
-    # Note: avoid adding the same log-file location as distinct handlers to the logger
-    # in case `ParallelMap` is executed repeatedly; also remove existing non-default
-    # logfile handlers to avoid generating multiple logs (and accidental writes to existing logs)
-    if len(log.handlers) == 0:
-        stdoutHandler = logging.StreamHandler()
-        stdoutHandler.setLevel(loglevel)
-        stdoutHandler.setFormatter(formatter)
-        log.addHandler(stdoutHandler)
-    if logfile is not None:
-        fHandlers = [h for h in log.handlers if isinstance(h, logging.FileHandler)]
-        for handler in fHandlers:
-            if handler.baseFilename == logfile:
-                break
-            else:
-                log.handlers.remove(handler)
-        fileHandler = logging.FileHandler(logfile)
-        fileHandler.setLevel(loglevel)
-        fileHandler.setFormatter(formatter)
-        log.addHandler(fileHandler)
-
-    return log
 
 
 def ctrlc_catcher(*excargs, **exckwargs):
     """
     Custom Traceback for properly handling CTRL + C interrupts while parallel
     computations are running
     """
@@ -326,39 +244,48 @@
     if len(excargs) == 3:
         isipy = False
         etype, evalue, etb = excargs
     else:
         shell, = excargs
         etype, evalue, etb = sys.exc_info()
         try:                            # careful: if iPython is used to launch a script, ``get_ipython`` is not defined
-            ipy = get_ipython()
+            get_ipython()
             isipy = True
             sys.last_traceback = etb    # smartify ``sys``
         except NameError:
             isipy = False
 
     # Prepare to log any uncaught exceptions
-    print, _ = dh._logging_setup()
+    log = logging.getLogger("ACME")
 
     # The only exception we really care about is a `KeyboardInterrupt`: if CTRL + C
     # is pressed, ensure graceful shutdown of any parallel processing clients
     if issubclass(etype, KeyboardInterrupt):
         try:
             client = dd.get_client()
         except ValueError:
             client = None
         if client is not None:
             for st in client.futures.values():
                 st.cancel()
             client.futures.clear()
             dh.cluster_cleanup(client)
-            print("<ACME> CTRL + C acknowledged, client and workers successfully killed")
-
-    # Log/print exception
-    print("<ACME> Exception received: {}: {}".format(str(etype), str(evalue)))
+            log.debug("CTRL + C acknowledged, client and workers successfully killed")
 
     # Relay exception handling back to appropriate system tools
     if isipy:
         shell.ipyTBshower(shell, exc_tuple=(etype, evalue, etb), **exckwargs)
     else:
         sys.__excepthook__(etype, evalue, etb)
+
+    # Write to all logging locations, manually print traceback to file (stdout
+    # printing was handled above)
+    log.error("Exception received.")
+    memHandler = [h for h in log.handlers if isinstance(h, handlers.MemoryHandler)][0]
+    if memHandler.target is not None:
+        memHandler.acquire()
+        with open(memHandler.target.baseFilename, "a", encoding="utf-8") as logfile:
+            logfile.write("".join(traceback.format_exception_only(etype, evalue)))
+            logfile.write("".join(traceback.format_tb(etb)))
+        memHandler.release()
+
     return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/tests/local_acme.py` & `esi-acme-2023.4/acme/tests/local_acme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# -*- coding: utf-8 -*-
 #
 # Simple script for testing acme w/o pip-installing it
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import numpy as np
 
 # Add acme to Python search path
 import os
 import sys
@@ -13,33 +17,40 @@
 if acme_path not in sys.path:
     sys.path.insert(0, acme_path)
 
 # Import package
 from acme import ParallelMap
 
 def f(x, y, z=3, w=np.zeros((3, 1)), **kwargs):
-    return (sum(x) + y) * z * w.max()
+    return (x + y) * z * w.max()
 
 import time
 
 def g(x, y, z=3):
     fSize = np.dtype("float").itemsize
     arrSize = 4
     time.sleep(10)
     arr = np.ones((int(arrSize * 1024**3 / fSize), ))
     time.sleep(300)
     return (sum(x) + y) * z * arr.max()
 
+def arr_test(x, y):
+    return x + y
 
 # Prepare code to be executed using, e.g., iPython's `%run` magic command
 if __name__ == "__main__":
 
     # Test stuff within here...
     # pass
 
-    pmap = ParallelMap(g, np.arange(100), 2)
-    pmap.daemon.estimate_memuse()
+    with ParallelMap(arr_test, [np.ones((20,)), 2 * np.ones((20,)), 3 * np.ones((20,))], 4, result_shape=(None, 20), verbose=True, single_file=True) as pmap:
+        results = pmap.compute()
+
+    1/0
+
+    # pmap = ParallelMap(g, np.arange(100), 2)
+    # pmap.daemon.estimate_memuse()
 
-    # with pmap as p:
-    #     p.compute()
+    # # with pmap as p:
+    # #     p.compute()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/tests/run_tests.cmd` & `esi-acme-2023.4/acme/tests/run_tests.cmd`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+::
+:: Copyright (c) 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+:: in Cooperation with Max Planck Society
+::
+:: SPDX-License-Identifier: BSD-3-Clause
+::
+
 @echo off
 for %%I in ("%cd%\..\..") do set "PYTHONPATH=%%~fI"
 
 set PYTEST_ADDOPTS="-v"
 
 if "%1" == "" goto usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/acme/tests/test_pmap.py` & `esi-acme-2023.4/acme/tests/test_pmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# -*- coding: utf-8 -*-
 #
 # Testing module for ACME's `ParallelMap` interface
 #
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
 
 # Builtin/3rd party package imports
 import os
 import sys
 import platform
 import pickle
 import shutil
@@ -16,24 +20,21 @@
 import itertools
 import logging
 import h5py
 import pytest
 import signal as sys_signal
 import numpy as np
 import dask.distributed as dd
+from logging import handlers
 from glob import glob
 from scipy import signal
 
 # Import main actors here
 from acme import ParallelMap, cluster_cleanup, esi_cluster_setup
-from acme.dask_helpers import customIOError
-from acme.shared import is_slurm_node, is_esi_node
-
-# Construct decorators for skipping certain tests
-skip_if_not_linux = pytest.mark.skipif(sys.platform != "linux", reason="Only works in Linux")
+from conftest import skip_if_not_linux, useSLURM, onESI, defaultQ
 
 # Functions that act as stand-ins for user-funcs
 def simple_func(x, y, z=3):
     return (x + y) * z
 
 def medium_func(x, y, z=3, w=np.ones((3, 3))):
     return (sum(x) + y) * z * w.max()
@@ -45,14 +46,22 @@
     with h5py.File(h5name, "r") as h5f:
         channel = h5f["data"][:, channel_no]
         b = h5f["data"].attrs["b"]
         a = h5f["data"].attrs["a"]
     res = signal.filtfilt(b, a, channel, padlen=200)
     return res
 
+def lowpass_medium(h5name, channel_no):
+    with h5py.File(h5name, "r") as h5f:
+        channel = h5f["data"][:, channel_no]
+        b = h5f["data"].attrs["b"]
+        a = h5f["data"].attrs["a"]
+    res = signal.filtfilt(b, a, channel, padlen=200)
+    return res, channel_no, b, a
+
 def lowpass_hard(arr_like, b, a, res_dir, res_base="lowpass_hard_", dset_name="custom_dset_name", padlen=200, taskID=None):
     channel = arr_like[:, taskID]
     res = signal.filtfilt(b, a, channel, padlen=padlen)
     h5name = os.path.join(res_dir, res_base +"{}.h5".format(taskID))
     with h5py.File(h5name, "w") as h5f:
         h5f.create_dataset(dset_name, data=res)
     return
@@ -68,20 +77,14 @@
     fSize = np.dtype("float").itemsize
     time.sleep(2)
     arr = np.ones((int(arrsize * 1024**3 / fSize), ))   # `arrsize` denotes array size in GB
     time.sleep(sleeper)
     return (x + y) * z * arr.max()
 
 
-# Perform SLURM-specific tests only on cluster nodes
-useSLURM = is_slurm_node()
-
-# Perform ESI-specific tests only the ESI HPC cluster
-onESI = is_esi_node()
-
 # Main testing class
 class TestParallelMap():
 
     # Construct linear combination of low- and high-frequency sine waves
     # and use an IIR filter to reconstruct the low-frequency component
     nChannels = 32
     nTrials = 8
@@ -102,51 +105,70 @@
     orig = np.repeat(orig.reshape(-1, 1), axis=1, repeats=nChannels)
     orig[:, ::2] *= -1
     orig = np.tile(orig, (nTrials, 1))
 
     # Error tolerance for low-pass filtered results
     tol = 1e-3
 
+    # Helper method for allocating data containers
+    def _prep_data(self, tmpName):
+
+        # Create tmp directory and create data-containers
+        tempDir = os.path.join(os.path.abspath(os.path.expanduser("~")), tmpName)
+        if useSLURM:
+            tempDir = "/cs/home/{}/{}".format(getpass.getuser(), tmpName)
+        os.makedirs(tempDir, exist_ok=True)
+        sigName = os.path.join(tempDir, "sigdata.h5")
+        origName = os.path.join(tempDir, "origdata.h5")
+        with h5py.File(sigName, "w") as sigFile:
+            dset = sigFile.create_dataset("data", data=self.sig)
+            dset.attrs["b"] = self.b
+            dset.attrs["a"] = self.a
+        with h5py.File(origName, "w") as origFile:
+            origFile.create_dataset("data", data=self.orig)
+
+        return tempDir, sigName
+
     # Test setup of `ParallelMap` w/different functions args/kwargs
-    def test_init(self):
+    def test_init(self, testclient=None):
 
         # Collected auto-generated output directories in list for later cleanup
         outDirs = []
 
         # Basic functionality w/simplest conceivable user-func
-        pmap = ParallelMap(simple_func, [2, 4, 6, 8], 4, setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(simple_func, [2, 4, 6, 8], y=4, setup_interactive=False)  # pos arg referenced via kwarg, cfg #2
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(simple_func, 0, 4, z=[3, 4, 5, 6], setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(simple_func, [2, 4, 6, 8], [2, 2], n_inputs=2, setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
+        pmap = ParallelMap(simple_func, [2, 4, 6, 8], 4, partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(simple_func, [2, 4, 6, 8], y=4, partition=defaultQ, setup_interactive=False)  # pos arg referenced via kwarg, cfg #2
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(simple_func, 0, 4, z=[3, 4, 5, 6], partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(simple_func, [2, 4, 6, 8], [2, 2], n_inputs=2, partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
 
         # User func has `np.ndarray` as keyword
-        pmap = ParallelMap(medium_func, [2, 4, 6, 8], y=[2, 2], n_inputs=2, setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(medium_func, None, None, w=[np.ones((3, 3)), 2 * np.ones((3,3))], setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(medium_func, None, None, z=np.zeros((3,)), setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(medium_func, None, None, z=np.zeros((3, 1)), setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
+        pmap = ParallelMap(medium_func, [2, 4, 6, 8], y=[2, 2], n_inputs=2, partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(medium_func, None, None, w=[np.ones((3, 3)), 2 * np.ones((3,3))], partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(medium_func, None, None, z=np.zeros((3,)), partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(medium_func, None, None, z=np.zeros((3, 1)), partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
 
         # Lots of ways for this to go wrong...
-        pmap = ParallelMap(hard_func, [2, 4, 6, 8], 2, w=np.ones((3,)), setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(hard_func, [2, 4, 6, 8], y=22, w=np.ones((7, 1)), setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(hard_func, np.ones((3,)), 1, w=np.ones((7, 1)), setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(hard_func, [2, 4, 6, 8], [2, 2], z=np.array([1, 2]), w=np.ones((8, 1)), n_inputs=2, setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap = ParallelMap(hard_func, [2, 4, 6, 8], [2, 2], w=np.ones((8, 1)), n_inputs=4, setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
+        pmap = ParallelMap(hard_func, [2, 4, 6, 8], 2, w=np.ones((3,)), partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(hard_func, [2, 4, 6, 8], y=22, w=np.ones((7, 1)), partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(hard_func, np.ones((3,)), 1, w=np.ones((7, 1)), partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(hard_func, [2, 4, 6, 8], [2, 2], z=np.array([1, 2]), w=np.ones((8, 1)), n_inputs=2, partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
+        pmap = ParallelMap(hard_func, [2, 4, 6, 8], [2, 2], w=np.ones((8, 1)), n_inputs=4, partition=defaultQ, setup_interactive=False)
+        outDirs.append(pmap.daemon.out_dir)
 
         # Ensure erroneous/ambiguous setups trigger the appropriate errors:
         # not enough positional args
         with pytest.raises(ValueError) as valerr:
             ParallelMap(simple_func, 4, setup_interactive=False)
             assert "simple_func expects 2 positional arguments ('x', 'y'), found 1" in str(valerr.value)
         # invalid kwargs
@@ -167,79 +189,160 @@
             assert "No object has required length of 3 matching `n_inputs`" in str(valerr.value)
         # invalid input spec: `w` expects a NumPy array, thus it is not considered for input distribution
         with pytest.raises(ValueError) as valerr:
             ParallelMap(hard_func, [2, 4, 6, 8], [2, 2], w=np.ones((8, 1)), n_inputs=8, setup_interactive=False)
             assert "No object has required length of 8 matching `n_inputs`" in str(valerr.value)
 
         # Clean up testing folder and any running clients
-        cluster_cleanup()
+        if testclient is None:
+            cluster_cleanup()
         for folder in outDirs:
             shutil.rmtree(folder, ignore_errors=True)
 
+        return testclient
+
     # Functionality tests: perform channel-concurrent low-pass filtering
-    def test_filter_example(self):
+    def test_simple_filter(self, testclient=None):
 
-        # If called by `test_existing_cluster` use pre-allocated client for all computations
-        try:
-            dd.get_client()
-            existingClient = True
-        except ValueError:
-            existingClient = False
+        # Prepare data containers
+        tempDir, sigName = self._prep_data("acme_tmp")
 
-        # Create tmp directory and create data-containers
-        tempDir = os.path.join(os.path.abspath(os.path.expanduser("~")), "acme_tmp")
-        if useSLURM:
-            tempDir = "/cs/home/{}/acme_tmp".format(getpass.getuser())
-        os.makedirs(tempDir, exist_ok=True)
-        sigName = os.path.join(tempDir, "sigdata.h5")
-        origName = os.path.join(tempDir, "origdata.h5")
-        with h5py.File(sigName, "w") as sigFile:
-            dset = sigFile.create_dataset("data", data=self.sig)
-            dset.attrs["b"] = self.b
-            dset.attrs["a"] = self.a
-        with h5py.File(origName, "w") as origFile:
-            origFile.create_dataset("data", data=self.orig)
-
-        # Collected auto-generated output directories in list for later cleanup
+        # Collect auto-generated output directories in list for later cleanup
         outDirs = []
 
         # Parallelize across channels, write results to disk
-        with ParallelMap(lowpass_simple, sigName, range(self.nChannels), setup_interactive=False) as pmap:
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
             resOnDisk = pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
+
+        # Ensure each compute run generated a dedicated HDF5 file
         assert len(pmap.kwargv["outFile"]) == pmap.n_calls
-        resFiles = [os.path.join(pmap.kwargv["outDir"][0], outFile) for outFile in pmap.kwargv["outFile"]]
-        assert resOnDisk == resFiles
+
+        # Query auto-generated output directory
+        outDirContents = glob(os.path.join(pmap.out_dir, "*"))
+        payloadDir = pmap.results_container.replace(".h5", "_payload")
+        assert pmap.results_container in outDirContents
+        assert payloadDir in outDirContents
+        resFiles = glob(os.path.join(payloadDir, "*.h5"))
+        assert len(resFiles) == pmap.n_calls
+        assert all(fle in resFiles for fle in resOnDisk)
         assert all(os.path.isfile(fle) for fle in resOnDisk)
+        log = logging.getLogger("ACME")
+        logFileList = [handler.target.baseFilename for handler in log.handlers if isinstance(handler, handlers.MemoryHandler)]
+        assert len(logFileList) == 1
+        assert logFileList[0] in outDirContents
+        assert len(outDirContents) == 3 # results container, payload dir and log
 
         # Compare computed single-channel results to expected low-freq signal
-        for chNo, h5name in enumerate(resOnDisk):
-            with h5py.File(h5name, "r") as h5f:
-                assert np.mean(np.abs(h5f["result_0"][()] - self.orig[:, chNo])) < self.tol
+        # and ensure collection container was assembled correctly
+        with h5py.File(pmap.results_container, "r") as h5col:
+            dset = "comp_{}/result_0"
+            for chNo, h5name in enumerate(resOnDisk):
+                with h5py.File(h5name, "r") as h5f:
+                    assert np.mean(np.abs(h5f["result_0"][()] - self.orig[:, chNo])) < self.tol
+                    assert np.array_equal(h5col[dset.format(chNo)][()], h5f["result_0"][()])
+
+        # Remember results for later use
+        colRes = str(pmap.results_container)
+        colResPayload = str(payloadDir)
 
-        # Same, but collect results in memory: ensure nothing freaky happens
+        # Same with `single_file`
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         partition=defaultQ,
+                         setup_interactive=False,
+                         single_file=True) as pmap:
+            singleResOnDisk = pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure only one file was generated
+        assert len(singleResOnDisk) == 1
+        outDirContents = glob(os.path.join(pmap.out_dir, "*.h5"))
+        assert outDirContents == singleResOnDisk
+        assert pmap.results_container in outDirContents[0]
+        assert os.path.isfile(singleResOnDisk[0])
+
+        # Compare results to container computed above
+        with h5py.File(colRes, "r") as h5col:
+            with h5py.File(pmap.results_container, "r") as h5single:
+                dset = "comp_{}/result_0"
+                for chNo in range(self.nChannels):
+                    assert np.array_equal(h5single[dset.format(chNo)][()], h5col[dset.format(chNo)][()])
+
+        # Now use non-standard output directory
+        outDir = os.path.join(tempDir, "somewhere")
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         output_dir=outDir,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            resOnDisk = pmap.compute()
+
+        # Query specified custom output directory
+        assert pmap.out_dir == outDir
+        outDirContents = glob(os.path.join(pmap.out_dir, "*"))
+        payloadDir = pmap.results_container.replace(".h5", "_payload")
+        assert pmap.results_container in outDirContents
+        assert payloadDir in outDirContents
+        resFiles = glob(os.path.join(payloadDir, "*.h5"))
+        assert len(resFiles) == pmap.n_calls
+        assert all(fle in resFiles for fle in resOnDisk)
+        assert all(os.path.isfile(fle) for fle in resOnDisk)
+
+        # A little overly paranoid, but compare results still...
+        with h5py.File(colRes, "r") as h5col:
+            with h5py.File(pmap.results_container, "r") as h5comp:
+                dset = "comp_{}/result_0"
+                for chNo in range(self.nChannels):
+                    assert np.array_equal(h5comp[dset.format(chNo)][()], h5col[dset.format(chNo)][()])
+
+        # Finally collect results in memory: ensure nothing freaky happens
         with ParallelMap(lowpass_simple,
                          sigName,
                          range(self.nChannels),
                          write_worker_results=False,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             resInMem = pmap.compute()
-        for chNo in range(self.nChannels):
-            assert np.mean(np.abs(resInMem[chNo] - self.orig[:, chNo])) < self.tol
 
         # Be double-paranoid: ensure on-disk and in-memory results match up
-        for chNo, h5name in enumerate(resOnDisk):
-            with h5py.File(h5name, "r") as h5f:
-                assert np.array_equal(h5f["result_0"][()], resInMem[chNo])
+        with h5py.File(colRes, "r") as h5col:
+            dset = "comp_{}/result_0"
+            for chNo in range(self.nChannels):
+                assert np.array_equal(h5col[dset.format(chNo)][()], resInMem[chNo])
+
+        # Comparisons are over, now remove payload and ensure container is broken
+        shutil.rmtree(colResPayload)
+        with pytest.raises(KeyError) as keyerr:
+            with h5py.File(colRes, "r") as h5col:
+                chNo = np.random.choice(self.nChannels, size=1)[0]
+                h5col["comp_{}".format(chNo)]["result_0"]
+            assert "unable to open external file" in str(keyerr.value)
 
-        # Simulate user-defined results-directory
+        # Ensure `output_dir` is properly ignored if `write_worker_results` is `False`
+        pmap = ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         output_dir=tempDir,
+                         write_worker_results=False,
+                         partition=defaultQ,
+                         setup_interactive=False)
+        assert pmap.daemon.out_dir is None
+        assert pmap.daemon.collect_results is True
+
+        # Simulate user-defined results-directory not auto-populated by ACME
         tempDir2 = os.path.join(os.path.abspath(os.path.expanduser("~")), "acme_tmp_lowpass_hard")
         if useSLURM:
             tempDir2 = "/cs/home/{}/acme_tmp_lowpass_hard".format(getpass.getuser())
-        shutil.rmtree(tempDir2, ignore_errors=True)
         os.makedirs(tempDir2, exist_ok=True)
 
         # Same task, different function: simulate user-defined saving scheme and "weird" inputs
         sigData = h5py.File(sigName, "r")["data"]
         res_base = "lowpass_hard_"
         dset_name = "custom_dset_name"
         with ParallelMap(lowpass_hard,
@@ -248,53 +351,60 @@
                          self.a,
                          res_dir=tempDir2,
                          res_base=res_base,
                          dset_name=dset_name,
                          padlen=[200] * self.nChannels,
                          n_inputs=self.nChannels,
                          write_worker_results=False,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             pmap.compute()
         resFiles = glob(os.path.join(tempDir2, res_base + "*"))
         assert len(resFiles) == pmap.n_calls
 
         # Compare computed single-channel results to expected low-freq signal
         for chNo in range(self.nChannels):
             h5name = res_base + "{}.h5".format(chNo)
             with h5py.File(os.path.join(tempDir2, h5name), "r") as h5f:
                 assert np.mean(np.abs(h5f[dset_name][()] - self.orig[:, chNo])) < self.tol
 
         # Ensure log-file generation produces a non-empty log-file at the expected location
         # Bonus: leave computing client alive and vet default SLURM settings
-        if not existingClient:
+        if testclient is None:
             cluster_cleanup(pmap.client)
-        for handler in pmap.log.handlers:
+        log = logging.getLogger("ACME")
+        for handler in log.handlers:
             if isinstance(handler, logging.FileHandler):
-                pmap.log.handlers.remove(handler)
+                log.handlers.remove(handler)
         with ParallelMap(lowpass_simple,
                          sigName,
                          range(self.nChannels),
                          logfile=True,
                          stop_client=False,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
-        logFileList = [handler.baseFilename for handler in pmap.log.handlers if isinstance(handler, logging.FileHandler)]
+        outDirs.append(pmap.out_dir)
+        logFileList = [handler.target.baseFilename for handler in log.handlers if isinstance(handler, handlers.MemoryHandler)]
         assert len(logFileList) == 1
         logFile = logFileList[0]
-        assert os.path.dirname(os.path.realpath(__file__)) in logFile
+        # If running on the ESI cluster, account for /cs/home
+        if onESI and useSLURM:
+            assert "/cs/home/" in logFile
+        else:
+            assert os.path.dirname(os.path.realpath(__file__)) in logFile
         with open(logFile, "r") as fl:
             assert len(fl.readlines()) > 1
 
         # Ensure client has not been killed; perform post-hoc check of default SLURM settings
         assert dd.get_client()
         client = dd.get_client()
-        if useSLURM and not existingClient:
-            assert pmap.n_calls == pmap.n_jobs
-            assert len(client.cluster.workers) == pmap.n_jobs
+        if useSLURM is True and testclient is None:
+            assert pmap.n_calls == pmap.n_workers
+            assert len(client.cluster.workers) == pmap.n_workers
             partition = client.cluster.job_header.split("-p ")[1].split("\n")[0]
             assert "8GB" in partition
             memory = np.unique([w["memory_limit"] for w in client.cluster.scheduler_info["workers"].values()])
             assert memory.size == 1
             assert round(memory[0] / 1000**3) == [int(s) for s in partition if s.isdigit()][0]
 
         # Wait a sec (literally) for dask to collect its bearings (after the
@@ -304,205 +414,623 @@
         # Same, but use custom log-file
         customLog = os.path.join(tempDir, "acme_log.txt")
         with ParallelMap(lowpass_simple,
                          sigName,
                          range(self.nChannels),
                          logfile=customLog,
                          verbose=True,
-                         stop_client=not existingClient,
+                         stop_client=testclient is None,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
         assert os.path.isfile(customLog)
         with open(customLog, "r") as fl:
             assert len(fl.readlines()) > 1
 
         # Ensure only single log file `customLog` is used
-        assert len([h for h in pmap.log.handlers if isinstance(h, logging.FileHandler)]) == 1
+        logFileList = [handler.target.baseFilename for handler in log.handlers if isinstance(handler, handlers.MemoryHandler)]
+        assert len(logFileList) == 1
+        assert logFileList[0] == customLog
 
         # Ensure client has been stopped
-        if not existingClient:
+        if testclient is None:
             with pytest.raises(ValueError):
                 dd.get_client()
 
         # Wait a sec (literally) to give dask enough time to close the client
         time.sleep(1.0)
 
-        # Underbook SLURM (more calls than jobs)
+        # Underbook SLURM (more calls than workers)
         partition = "8GBXS"
-        n_jobs = int(self.nChannels / 2)
-        mem_per_job = "2GB"
+        n_workers = int(self.nChannels / 2)
+        mem_per_worker = "2GB"
         with ParallelMap(lowpass_simple,
                          sigName,
                          range(self.nChannels),
                          partition=partition,
-                         n_jobs=n_jobs,
-                         mem_per_job=mem_per_job,
+                         n_workers=n_workers,
+                         mem_per_worker=mem_per_worker,
                          stop_client=False,
                          setup_interactive=False) as pmap:
             pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
 
         # Post-hoc check of client to ensure custom settings were respected
         client = pmap.client
         assert pmap.n_calls == self.nChannels
-        if useSLURM:
-            assert pmap.n_jobs == n_jobs
-            assert len(client.cluster.workers) == pmap.n_jobs
+        if useSLURM is True and testclient is None:
+            assert pmap.n_workers == n_workers
+            assert len(client.cluster.workers) == pmap.n_workers
             actualPartition = client.cluster.job_header.split("-p ")[1].split("\n")[0]
             assert actualPartition == partition
             memory = np.unique([w["memory_limit"] for w in client.cluster.scheduler_info["workers"].values()])
             assert memory.size == 1
-            assert round(memory[0] / 1000**3) == int(mem_per_job.replace("GB", ""))
+            assert round(memory[0] / 1000**3) == int(mem_per_worker.replace("GB", ""))
 
         # Let `cluster_cleanup` murder the custom setup and ensure it did its job
-        if not existingClient:
+        if testclient is None:
             cluster_cleanup(pmap.client)
             with pytest.raises(ValueError):
                 dd.get_client()
 
-        # Overbook SLURM (more jobs than calls)
+        # Overbook SLURM (more workers than calls)
         partition = "8GBXS"
-        n_jobs = self.nChannels + 2
-        mem_per_job = "3000MB"
+        n_workers = self.nChannels + 2
+        mem_per_worker = "3000MB"
         with ParallelMap(lowpass_simple,
                          sigName,
                          range(self.nChannels),
                          partition=partition,
-                         n_jobs=n_jobs,
-                         mem_per_job=mem_per_job,
+                         n_workers=n_workers,
+                         mem_per_worker=mem_per_worker,
                          stop_client=False,
                          setup_interactive=False) as pmap:
             pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
 
         # Post-hoc check of client to ensure custom settings were respected
         client = pmap.client
         assert pmap.n_calls == self.nChannels
-        if useSLURM:
-            assert pmap.n_jobs == n_jobs
-            assert len(client.cluster.workers) == pmap.n_jobs
+        if useSLURM and testclient is None:
+            assert pmap.n_workers == n_workers
+            assert len(client.cluster.workers) == pmap.n_workers
             actualPartition = client.cluster.job_header.split("-p ")[1].split("\n")[0]
             assert actualPartition == partition
             memory = np.unique([w["memory_limit"] for w in client.cluster.scheduler_info["workers"].values()])
             assert memory.size == 1
-            assert round(memory[0] / 1000**3) * 1000 == int(mem_per_job.replace("MB", ""))
-        if not existingClient:
+            assert round(memory[0] / 1000**3) * 1000 == int(mem_per_worker.replace("MB", ""))
+        if testclient is None:
             cluster_cleanup(pmap.client)
 
         # Close any open HDF5 files to not trigger any `OSError`s, close running clusters
         # and clean up tmp dirs and created directories/log-files
         sigData.file.close()
         try:
             os.unlink(logFile)
         except PermissionError:
             pass
         shutil.rmtree(tempDir, ignore_errors=True)
         shutil.rmtree(tempDir2, ignore_errors=True)
         for folder in outDirs:
             shutil.rmtree(folder, ignore_errors=True)
 
-        # Wait a second (literally) so that no new parallel jobs started by
+        # Wait a second (literally) so that no new parallel workers started by
+        # `test_existing_cluster` erroneously use existing HDF files
+        time.sleep(1.0)
+
+        return testclient
+
+    # More functionality tests: ensure user-funcs w/multiple outputs are processed correctly
+    def test_medium_filter(self, testclient=None):
+
+        # Prepare data containers
+        _, sigName = self._prep_data("acme_tmp2")
+
+        # Collect auto-generated output directories in list for later cleanup
+        outDirs = []
+
+        # Parallelize across channels, write results to disk
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+             pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure output container was created correctly
+        payloadDir = pmap.results_container.replace(".h5", "_payload")
+        assert len(glob(os.path.join(payloadDir, "*.h5"))) == pmap.n_calls
+
+        # Compare computed results to expected values
+        with h5py.File(pmap.results_container, "r") as h5col:
+            dset = "comp_{}/result_{}"
+            for chNo in range(self.nChannels):
+                assert len(h5col["comp_{}".format(chNo)].keys()) == 4
+                assert np.mean(np.abs(h5col[dset.format(chNo, 0)][()] - self.orig[:, chNo])) < self.tol
+                assert h5col[dset.format(chNo, 1)][()] == chNo
+                assert np.array_equal(h5col[dset.format(chNo, 2)][()], self.b)
+                assert np.array_equal(h5col[dset.format(chNo, 3)][()], self.a)
+
+        # Remember results for later use
+        colRes = str(pmap.results_container)
+
+        # Same with `single_file`
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         partition=defaultQ,
+                         setup_interactive=False,
+                         single_file=True) as pmap:
+            pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure only one (data) file was generated
+        assert glob(os.path.join(pmap.out_dir, "*.h5")) == [pmap.results_container]
+
+        # Compare single file to link collection computed above
+        with h5py.File(colRes, "r") as h5col:
+            with h5py.File(pmap.results_container, "r") as h5single:
+                dset = "comp_{}/result_{}"
+                for chNo in range(self.nChannels):
+                    assert len(h5single["comp_{}".format(chNo)].keys()) == 4
+                    assert np.array_equal(h5single[dset.format(chNo, 0)][()], h5col[dset.format(chNo, 0)][()])
+                    assert h5col[dset.format(chNo, 1)][()] == h5single[dset.format(chNo, 1)][()]
+                    assert np.array_equal(h5col[dset.format(chNo, 2)][()], h5single[dset.format(chNo, 2)][()])
+                    assert np.array_equal(h5col[dset.format(chNo, 3)][()], h5single[dset.format(chNo, 3)][()])
+
+        # Same, but collect results in memory: ensure nothing freaky happens
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         write_worker_results=False,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            resInMem = pmap.compute()
+
+        # Be double-paranoid: ensure on-disk and in-memory results match up
+        with h5py.File(colRes, "r") as h5col:
+            dset = "comp_{}/result_{}"
+            for chNo in range(self.nChannels):
+                assert len(resInMem[chNo]) == 4
+                assert np.array_equal(h5col[dset.format(chNo, 0)][()], resInMem[chNo][0])
+                assert h5col[dset.format(chNo, 1)][()] == resInMem[chNo][1]
+                assert np.array_equal(h5col[dset.format(chNo, 2)][()], resInMem[chNo][2])
+                assert np.array_equal(h5col[dset.format(chNo, 3)][()], resInMem[chNo][3])
+
+        # Clean up created results directories
+        for folder in outDirs:
+            shutil.rmtree(folder, ignore_errors=True)
+
+        # Wait a second (literally) so that no new parallel workers started by
+        # `test_existing_cluster` erroneously use existing HDF files
+        time.sleep(1.0)
+
+        return testclient
+
+    # Even more functionality tests: ensure output array stacking works
+    def test_outshape(self, testclient=None):
+
+        # Prepare data containers
+        _, sigName = self._prep_data("acme_tmp_outshape")
+
+        # Collect auto-generated output directories in list for later cleanup
+        outDirs = []
+
+        # Compute result length needed to determine final shape
+        nSamples = self.fs * self.nTrials
+
+        # Parallelize across channels, write results to disk
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            resOnDisk = pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Remember results for later use
+        colRes = str(pmap.results_container)
+
+        # Compare computed single-channel results to expected low-freq signal
+        # and ensure collection container was assembled correctly
+        with h5py.File(pmap.results_container, "r") as h5col:
+            assert len(h5col.keys()) == 1
+            assert h5col["result_0"].is_virtual
+            for chNo, h5name in enumerate(resOnDisk):
+                with h5py.File(h5name, "r") as h5f:
+                    assert np.mean(np.abs(h5f["result_0"][()] - self.orig[:, chNo])) < self.tol
+                    assert np.array_equal(h5col["result_0"][chNo, :], h5f["result_0"][()])
+
+        # Same but don't use a virtual dataset and transpose the final array
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(nSamples, None),
+                         single_file=True,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure only one (data) file was generated
+        assert glob(os.path.join(pmap.out_dir, "*.h5")) == [pmap.results_container]
+
+        # Compare single file to virtual dataset
+        with h5py.File(colRes, "r") as h5col:
+            with h5py.File(pmap.results_container, "r") as h5single:
+                assert len(h5single.keys()) == 1
+                assert h5single["result_0"].is_virtual is False
+                assert np.array_equal(h5single["result_0"][()].T, h5col["result_0"][()])
+
+        # Finally, ensure in-memory results-collection works as expected
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         write_worker_results=False,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            resInMem = pmap.compute()
+        with h5py.File(colRes, "r") as h5col:
+            assert np.array_equal(h5col["result_0"][()], resInMem)
+
+        # Ensure dtype is respected
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         result_dtype="float16",
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            pmap.compute()
+        outDirs.append(pmap.out_dir)
+        with h5py.File(pmap.results_container, "r") as h5f:
+            assert h5f["result_0"].dtype.name == "float16"
+
+        # Ensure invalid dtypes don't pass through
+        with pytest.raises(TypeError) as tperr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(None, nSamples),
+                             result_dtype=np.ones((3,)),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_dtype` has to be a string" in str(tperr)
+        with pytest.raises(TypeError) as tperr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(None, nSamples),
+                             result_dtype="invalid",
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_dtype` has to be a valid NumPy datatype" in str(tperr)
+
+        # Ensure borked shapes are caught
+        with pytest.raises(TypeError) as tperr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=3,
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` has to be either `None` or tuple" in str(tperr)
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(None, None, nSamples),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` must contain exactly one `None`" in str(valerr)
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(3, nSamples),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` must contain exactly one `None`" in str(valerr)
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=("invalid", None, nSamples),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` must only contain numerical values" in str(valerr)
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(-3, None, nSamples),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` must only contain non-negative integers" in str(valerr)
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(lowpass_simple,
+                             sigName,
+                             range(self.nChannels),
+                             result_shape=(np.pi, None, nSamples),
+                             partition=defaultQ,
+                             setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "`result_shape` must only contain non-negative integers" in str(valerr)
+
+        # Emergency pickling
+        with ParallelMap(pickle_func,
+                         self.sig,
+                         self.b,
+                         self.a,
+                         range(self.nChannels),
+                         sabotage_hdf5=True,
+                         n_inputs=self.nChannels,
+                         result_shape=(nSamples, None),
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            mixedResults = pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure pickles and hdf5's live together happily
+        resultsContainer = os.path.basename(mixedResults[0])
+        resultsContainer = os.path.join(os.path.dirname(mixedResults[0]),
+                                        resultsContainer[:resultsContainer.rfind("_0")] + ".h5")
+        payloadDir = resultsContainer.replace(".h5", "_payload")
+        assert pmap.results_container is None
+        assert not os.path.isfile(resultsContainer)
+        assert not os.path.isdir(payloadDir)
+        assert all(os.path.isfile(fle) for fle in mixedResults)
+        assert len(mixedResults) == pmap.n_calls
+
+        # Ensure deliberate pickling doesn't clash w/(erroneous) shape spec
+        with ParallelMap(pickle_func,
+                         self.sig,
+                         self.b,
+                         self.a,
+                         range(self.nChannels),
+                         sabotage_hdf5=False,
+                         n_inputs=self.nChannels,
+                         result_shape=(nSamples, None),
+                         write_pickle=True,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            pickles = pmap.compute()
+        outDirs.append(pmap.out_dir)
+        assert all(os.path.isfile(fle) for fle in pickles)
+        assert len(pickles) == pmap.n_calls
+
+        # Ensure multiple return values are handled correctly
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         single_file=False,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+             pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Save results for later
+        multiRet = str(pmap.results_container)
+
+        # Compare computed results to stored "reference"
+        with h5py.File(colRes, "r") as h5col:
+            with h5py.File(pmap.results_container, "r") as h5f:
+                assert len(h5f.keys()) == pmap.n_calls + 1
+                assert h5f["result_0"].is_virtual is True
+                assert np.array_equal(h5f["result_0"][()], h5col["result_0"][()])
+                for k in range(pmap.n_calls):
+                    assert len(h5f["comp_{}".format(k)].keys()) == 3
+                    assert h5f["comp_{}/{}".format(k, "result_1")][()] == k
+                    assert np.array_equal(h5f["comp_{}/{}".format(k, "result_2")][()], self.b)
+                    assert np.array_equal(h5f["comp_{}/{}".format(k, "result_3")][()], self.a)
+
+        # Same w/single output container
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         single_file=True,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+             pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Compare results
+        with h5py.File(multiRet, "r") as h5ref:
+            with h5py.File(pmap.results_container, "r") as h5f:
+                assert len(h5f.keys()) == pmap.n_calls + 1
+                for k in range(pmap.n_calls):
+                    for rk in range(1,4):
+                        dset = "comp_{}/result_{}".format(k, rk)
+                        assert np.array_equal(h5f[dset], h5ref[dset])
+
+        # Finally, ensure in-memory results-collection works w/multiple returns
+        with ParallelMap(lowpass_medium,
+                         sigName,
+                         range(self.nChannels),
+                         result_shape=(None, nSamples),
+                         write_worker_results=False,
+                         partition=defaultQ,
+                         setup_interactive=False) as pmap:
+            resInMem = pmap.compute()
+        with h5py.File(multiRet, "r") as h5ref:
+            assert np.array_equal(h5ref["result_0"][()], resInMem[0])
+            rCount = 1
+            for k in range(pmap.n_calls):
+                assert h5ref["comp_{}/{}".format(k, "result_1")][()] == resInMem[rCount]
+                rCount +=1
+                assert np.array_equal(h5ref["comp_{}/{}".format(k, "result_2")][()], resInMem[rCount])
+                rCount +=1
+                assert np.array_equal(h5ref["comp_{}/{}".format(k, "result_3")][()], resInMem[rCount])
+                rCount +=1
+
+        # Clean up created results directories
+        for folder in outDirs:
+            shutil.rmtree(folder, ignore_errors=True)
+
+        # Wait a second (literally) so that no new parallel workers started by
         # `test_existing_cluster` erroneously use existing HDF files
         time.sleep(1.0)
 
+        return testclient
+
     # Test if pickling/emergency pickling and I/O in general works as intended
-    def test_pickling(self):
+    def test_pickling(self, testclient=None):
 
         # Collected auto-generated output directories in list for later cleanup
         outDirs = []
 
         # Execute `pickle_func` w/regular HDF5 saving
         with ParallelMap(pickle_func,
                          self.sig,
                          self.b,
                          self.a,
                          range(self.nChannels),
                          sabotage_hdf5=False,
                          n_inputs=self.nChannels,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             hdfResults = pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        colRes = str(pmap.results_container)
+        outDirs.append(pmap.out_dir)
 
         # Execute `pickle_func` w/pickling
         with ParallelMap(pickle_func,
                          self.sig,
                          self.b,
                          self.a,
                          range(self.nChannels),
                          n_inputs=self.nChannels,
                          write_pickle=True,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             pklResults = pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
 
         # Ensure HDF5 and pickle match up
-        for chNo, h5name in enumerate(hdfResults):
-            with open(pklResults[chNo], "rb") as pkf:
-                pklRes = pickle.load(pkf)
-            with h5py.File(h5name, "r") as h5f:
-                assert np.array_equal(pklRes, h5f["result_0"][()])
+        with h5py.File(colRes, "r") as h5col:
+            dset = "comp_{}/result_0"
+            for chNo in range(self.nChannels):
+                with open(pklResults[chNo], "rb") as pkf:
+                    pklRes = pickle.load(pkf)
+                assert np.array_equal(pklRes, h5col[dset.format(chNo)][()])
+
+        # Ensure single_file and pickling does not work
+        with pytest.raises(ValueError) as valerr:
+            with ParallelMap(pickle_func,
+                            self.sig,
+                            self.b,
+                            self.a,
+                            range(self.nChannels),
+                            n_inputs=self.nChannels,
+                            write_pickle=True,
+                            single_file=True,
+                            partition=defaultQ,
+                            setup_interactive=False) as pmap:
+                pmap.compute()
+            assert "Pickling of results does not support single output file creation" in str(valerr.value)
 
         # Test emergency pickling
         with ParallelMap(pickle_func,
                          self.sig,
                          self.b,
                          self.a,
                          range(self.nChannels),
                          sabotage_hdf5=True,
                          n_inputs=self.nChannels,
+                         partition=defaultQ,
                          setup_interactive=False) as pmap:
             mixedResults = pmap.compute()
-        outDirs.append(pmap.kwargv["outDir"][0])
+        outDirs.append(pmap.out_dir)
+
+        # Collection container should have been auto-removed
+        resultsContainer = os.path.basename(mixedResults[0])
+        resultsContainer = os.path.join(os.path.dirname(mixedResults[0]),
+                                        resultsContainer[:resultsContainer.rfind("_0")] + ".h5")
+        payloadDir = resultsContainer.replace(".h5", "_payload")
+        assert pmap.results_container is None
+        assert not os.path.isfile(resultsContainer)
+        assert not os.path.isdir(payloadDir)
 
         # Ensure non-compliant dicts were pickled, rest is in HDF5
         for chNo, fname in enumerate(mixedResults):
             if chNo % 2 == 0:
                 assert fname.endswith(".pickle")
                 with open(fname, "rb") as pkf:
-                    assert np.array_equal(self.b, pickle.load(pkf)["b"])
+                    assert np.array_equal(self.b, pickle.load(pkf)[0]["b"])
             else:
                 assert fname.endswith(".h5")
                 with h5py.File(fname, "r") as h5f:
                     with h5py.File(hdfResults[chNo], "r") as h5ref:
                         assert np.array_equal(h5f["result_0"][()], h5ref["result_0"][()])
 
+        # Ensure emergency pickling and single file does not work
+        with pytest.raises(RuntimeError):
+            with ParallelMap(pickle_func,
+                            self.sig,
+                            self.b,
+                            self.a,
+                            range(self.nChannels),
+                            sabotage_hdf5=True,
+                            n_inputs=self.nChannels,
+                            single_file=True,
+                            partition=defaultQ,
+                            setup_interactive=False) as pmap:
+                pmap.compute()
+
+
         # Test write breakdown (both for HDF5 saving and pickling)
         pmap = ParallelMap(pickle_func,
                            self.sig,
                            self.b,
                            self.a,
                            range(self.nChannels),
                            sabotage_hdf5=True,
                            n_inputs=self.nChannels,
+                           partition=defaultQ,
                            setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap.kwargv["outDir"][0] = "/path/to/nowhere"
+        outDirs.append(pmap.daemon.out_dir)
+        pmap.kwargv["outFile"][0] = "/path/to/nowhere"
         with pytest.raises(RuntimeError) as runerr:
             pmap.compute()
             assert "<ACMEdaemon> Parallel computation failed" in str(runerr.value)
         pmap = ParallelMap(pickle_func,
                            self.sig,
                            self.b,
                            self.a,
                            range(self.nChannels),
                            sabotage_hdf5=True,
                            n_inputs=self.nChannels,
                            write_pickle=True,
+                           partition=defaultQ,
                            setup_interactive=False)
-        outDirs.append(pmap.kwargv["outDir"][0])
-        pmap.kwargv["outDir"][0] = "/path/to/nowhere"
+        outDirs.append(pmap.daemon.out_dir)
+        pmap.kwargv["outFile"][0] = "/path/to/nowhere"
         with pytest.raises(RuntimeError) as runerr:
             pmap.compute()
             assert "<ACMEdaemon> Parallel computation failed" in str(runerr.value)
 
         # Clean up testing folder
         for folder in outDirs:
             shutil.rmtree(folder, ignore_errors=True)
 
+        return testclient
+
     # test if KeyboardInterrupts are handled correctly
     @skip_if_not_linux
     def test_cancel(self):
 
         # Setup temp-directory layout for subprocess-scripts and prepare interpreters
         tempDir = os.path.join(os.path.abspath(os.path.expanduser("~")), "acme_tmp")
         os.makedirs(tempDir, exist_ok=True)
@@ -530,17 +1058,17 @@
             # Launch new process in background (`stdbuf` prevents buffering of stdout)
             proc = subprocess.Popen("stdbuf -o0 " + pshell + " " + scriptName,
                                     shell=True, start_new_session=True,
                                     stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=0)
 
             # Wait for ACME to start up (as soon as logging info is shown, `pmap.compute()` is running)
             # However: don't wait indefinitely - if `pmap.compute` is not started within 30s, abort
-            logStr = "<ParallelMap> INFO: Log information available at"
+            logStr = "Preparing 2 parallel calls"
             buffer = bytearray()
-            timeout = 30
+            timeout = 90
             t0 = time.time()
             for line in itertools.takewhile(lambda x: time.time() - t0 < timeout, iter(proc.stdout.readline, b"")):
                 buffer.extend(line)
                 if logStr in line.decode("utf8"):
                     break
             assert logStr in buffer.decode("utf8")
 
@@ -548,60 +1076,60 @@
             # impromptu script did not run to completion *but* the created client was
             # shut down with CTRL + C
             time.sleep(2)
             os.killpg(proc.pid, sys_signal.SIGINT)
             time.sleep(1)
             out = proc.stdout.read().decode()
             assert "ALL DONE" not in out
-            assert "INFO: <cluster_cleanup> Successfully shut down" in out
+            assert "Successfully shut down" in out
 
         # Almost identical script, this time use an externally started client
         scriptName = os.path.join(tempDir, "dummy2.py")
         scriptContents = \
             "from acme import ParallelMap, esi_cluster_setup\n" +\
             "import time\n" +\
             "def long_running(dummy):\n" +\
             "   time.sleep(10)\n" +\
             "   return\n" +\
             "if __name__ == '__main__':\n" +\
-            "   client = esi_cluster_setup(partition='8GBDEV',n_jobs=1, interactive=False)\n" +\
-            "   with ParallelMap(long_running, [None]*2, setup_interactive=False, write_worker_results=False) as pmap: \n" +\
+            "   client = esi_cluster_setup(partition='8GBDEV',n_workers=1, interactive=False)\n" +\
+            "   with ParallelMap(long_running, [None]*2, setup_interactive=False, write_worker_results=False, verbose=True) as pmap: \n" +\
             "       pmap.compute()\n" +\
             "   print('ALL DONE')\n"
         with open(scriptName, "w") as f:
             f.write(scriptContents)
 
         # Test script functionality in both Python and iPython
         for pshell in pshells:
             proc = subprocess.Popen("stdbuf -o0 " + sys.executable + " " + scriptName,
                                     shell=True, start_new_session=True,
                                     stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=0)
-            logStr = "<ParallelMap> INFO: Log information available at"
+            logStr = "This is ACME"
             buffer = bytearray()
-            timeout = 30
+            timeout = 60
             t0 = time.time()
             for line in itertools.takewhile(lambda x: time.time() - t0 < timeout, iter(proc.stdout.readline, b"")):
                 buffer.extend(line)
                 if logStr in line.decode("utf8"):
                     break
             assert logStr in buffer.decode("utf8")
             time.sleep(2)
             os.killpg(proc.pid, sys_signal.SIGINT)
             time.sleep(2)
             out = proc.stdout.read().decode()
             assert "ALL DONE" not in out
-            assert "<ParallelMap> INFO: <ACME> CTRL + C acknowledged, client and workers successfully killed" in out
+            assert "CTRL + C acknowledged, client and workers successfully killed" in out
 
         # Ensure random exception does not immediately kill an active client
         scriptName = os.path.join(tempDir, "dummy3.py")
         scriptContents = \
             "from acme import esi_cluster_setup\n" +\
             "import time\n" +\
             "if __name__ == '__main__':\n" +\
-            "   esi_cluster_setup(partition='8GBDEV',n_jobs=1, interactive=False)\n" +\
+            "   esi_cluster_setup(partition='8GBDEV',n_workers=1, interactive=False)\n" +\
             "   time.sleep(60)\n"
         with open(scriptName, "w") as f:
             f.write(scriptContents)
         proc = subprocess.Popen("stdbuf -o0 " + sys.executable + " " + scriptName,
                                 shell=True, start_new_session=True,
                                 stdout=subprocess.PIPE, stderr=subprocess.STDOUT, bufsize=0)
 
@@ -628,26 +1156,26 @@
         # using pytest's monkeypatch fixture user-input is simulated. If a user
         # decides to not move ahead after the dryrun the auto-generated output
         # directory must be cleaned up
         monkeypatch.setattr("builtins.input", lambda _ : "n")
         pmap = ParallelMap(simple_func, [2, 4, 6, 8], 4, setup_interactive=True, dryrun=True)
 
         # Ensure auto-generated output dir has been successfully removed
-        outDir = pmap.kwargv["outDir"][0]
+        outDir = pmap.daemon.out_dir
         assert os.path.exists(outDir) is False
 
     def test_memest(self):
 
         # First kill any existing client (otherwise profiling is not happening)
         cluster_cleanup()
 
         # Create tmp directory for logfile
         tempDir = os.path.join(os.path.abspath(os.path.expanduser("~")), "acme_tmp")
         os.makedirs(tempDir, exist_ok=True)
-        customLog = os.path.join(tempDir, "acme_log.txt")
+        customLog = os.path.join(tempDir, "mem_log.txt")
         outDirs = []
 
         # Set `arrsize` depending on available runner hardware and prepare expected
         # mem estimates accordingly
         arrsize = 2
         estMem = 3
         if platform.machine() == "ppc64le":
@@ -680,26 +1208,48 @@
             if sys.platform != "darwin":
                 assert memEst == "estimate_memuse:" + str(estMem)
 
             # Ensure profiler quit out early (since total runtime of `memtest_func` is below 30s)
             assert toc - tic < 30
 
         # Check that for 2 parallel calls only 2 workers were memory-profiled
+        # (we need to flush `MemoryHandler` manually so that its contents
+        # is actually written to `customLog`)
+        log = logging.getLogger("ACME")
+        for h in log.handlers:
+            if hasattr(h, "flush"):
+                h.flush()
         with open(customLog, "r", encoding="utf8") as f:
             logTxt = f.read()
         assert "Estimated memory consumption across 2 runs" in logTxt
 
         # If running on the ESI cluster, ensure the correct partition has been picked
         if onESI and useSLURM:
             assert "Picked partition 8GBXS based on estimated memory consumption of 3 GB" in logTxt
 
         # Profiling completed full run of `memtest_func`: ensure any auto-created
         # output HDF5 files were removed
-        outDirs.append(pmap.kwargv["outDir"][0])
-        assert len(os.listdir(outDirs[0])) == 0
+        outDirs.append(pmap.daemon.out_dir)
+        assert len(os.listdir(os.path.dirname(pmap.kwargv['outFile'][0]))) == 0
+
+        # Syncopy-related test: ensure memory profiling works also if ACME
+        # does not handle result collection
+        syncopylog = os.path.join(tempDir, "syncopylog.txt")
+        pmap = ParallelMap(memtest_func,
+                           np.arange(100),
+                           2,
+                           sleeper=300,
+                           arrsize=arrsize,
+                           logfile=syncopylog,
+                           setup_timeout=10,
+                           write_worker_results=False,
+                           setup_interactive=False)
+        with open(syncopylog, "r", encoding="utf8") as f:
+            logTxt = f.read()
+        assert "memEstRun" not in logTxt
 
         # Now prepare `ParallelMap` instance for 100 concurrent calls of `memtest_func`:
         # again a 2GB array is allocated, but set final sleep to 5 minutes, enforcing
         # abort of profiling runs (set `setup_interactive` low to not have 100
         # SLURM workers being actually started)
         del pmap
         cluster_cleanup()
@@ -723,25 +1273,31 @@
             if sys.platform != "darwin":
                 assert memEst == "estimate_memuse:" + str(estMem)
 
             # Ensure profiler went the whole mile (since total runtime of `memtest_func` > 5 min)
             assert 140 < toc - tic < 200
 
         # Check that for max 5 workers were memory-profiled
+        # (we need to flush `MemoryHandler` manually so that its contents
+        # is actually written to `customLog`)
+        log = logging.getLogger("ACME")
+        for h in log.handlers:
+            if hasattr(h, "flush"):
+                h.flush()
         with open(customLog2, "r", encoding="utf8") as f:
             logTxt = f.read()
         assert "Estimated memory consumption across 5 runs" in logTxt
 
         # If running on the ESI cluster, ensure the correct partition has been picked (again)
         if onESI and useSLURM:
             assert "Picked partition 8GBXS based on estimated memory consumption of 3 GB" in logTxt
 
         # Profiling should not have generated any output
-        outDirs.append(pmap.kwargv["outDir"][0])
-        assert len(os.listdir(outDirs[0])) == 0
+        outDirs.append(pmap.daemon.out_dir)
+        assert len(os.listdir(os.path.dirname(pmap.kwargv['outFile'][0]))) == 0
 
         # Prepare final "full" tests
         del pmap
         cluster_cleanup()
         customLog3 = os.path.join(tempDir, "acme_log3.txt")
 
         # Assert that `partition="auto"` has no effect in `LocalCluster` case
@@ -752,28 +1308,31 @@
                              sleeper=2,
                              arrsize=arrsize,
                              logfile=customLog3) as pmap:
                 pmap.compute()
             with open(customLog3, "r", encoding="utf8") as f:
                 logTxt = f.read()
             assert "Estimating memory consumption" not in logTxt
-            outDirs.append(pmap.kwargv["outDir"][0])
+            outDirs.append(pmap.out_dir)
 
         else:
 
+            # Simulate call of ParallelMap(partition="auto",...) but w/wrong mem_per_worker!
+            with pytest.raises(IOError):
+                esi_cluster_setup(partition="auto", mem_per_worker="invalid")
+
             # Simulate `ParallelMap(partition="auto",...)` call by invoking `esi_cluster_setup`
-            # with `mem_per_job='esstimate_memuse:XY'`
-            client = esi_cluster_setup(partition="auto", mem_per_job="estimate_memuse:12", n_jobs=1)
+            # with `mem_per_worker='esstimate_memuse:XY'`
+            client = esi_cluster_setup(partition="auto",
+                                       mem_per_worker="estimate_memuse:12",
+                                       n_workers=1,
+                                       interactive=False)
 
             # Ensure the right partition was picked (16GBXY, not 8GBXY)
             assert "16GB" in client.cluster.job_header.split("-p ")[1].split("\n")[0]
-
-            # Simulate call of ParallelMap(partition="auto",...) but w/wrong mem_per_job!
-            with pytest.raises(customIOError):
-                esi_cluster_setup(partition="auto", mem_per_job="invalid")
             cluster_cleanup(client)
 
             # Full run (finally) w/10 workers, 5 of em get mem-profiled
             with ParallelMap(memtest_func,
                              np.arange(10),
                              2,
                              sleeper=35,
@@ -784,68 +1343,103 @@
                 pmap.compute()
 
             # Check correct partition and no. of workers profiled
             with open(customLog3, "r", encoding="utf8") as f:
                 logTxt = f.read()
             assert "Estimated memory consumption across 5 runs" in logTxt
             assert "Picked partition 8GBXS" in logTxt
-            outDirs.append(pmap.kwargv["outDir"][0])
+            outDirs.append(pmap.out_dir)
 
         # Clean up
         shutil.rmtree(tempDir, ignore_errors=True)
         for folder in outDirs:
             shutil.rmtree(folder, ignore_errors=True)
         time.sleep(0.1)
 
-    # test esi-cluster-setup called separately before pmap
-    def test_existing_cluster(self):
+    # test if deprecated keywords are mapped onto new names correctly
+    def test_backcompat(self):
+
+        # Prepare data containers
+        _, sigName = self._prep_data("acme_tmp")
+
+        # Collect auto-generated output directories in list for later cleanup
+        outDirs = []
+
+        # Invoke `ParallelMap` w/deprecated `n_jobs` kw
+        with ParallelMap(lowpass_simple,
+                         sigName,
+                         range(self.nChannels),
+                         partition=defaultQ,
+                         n_jobs=2,
+                         logfile=True,
+                         setup_interactive=False) as pmap:
+            pmap.compute()
+        outDirs.append(pmap.out_dir)
+
+        # Ensure a deprecation warning was issued
+        log = logging.getLogger("ACME")
+        for handler in log.handlers:
+            if isinstance(handler, logging.FileHandler):
+                with open(handler.baseFilename, "r") as fl:
+                    logTxt = fl.read()
+                assert "DEPRECATED" in logTxt
 
-        # Test custom SLURM cluster setup
         if useSLURM:
 
-            # Ensure invalid partition/memory specifications are caught
-            with pytest.raises(customIOError):
-                esi_cluster_setup(partition="invalid", interactive=False)
-            cluster_cleanup()
-            with pytest.raises(ValueError):
-                esi_cluster_setup(mem_per_job="invalidGB", interactive=False)
-            cluster_cleanup()
-            with pytest.raises(ValueError):
-                esi_cluster_setup(mem_per_job="-20MB", interactive=False)
-            cluster_cleanup()
+            # Use the deprecated `n_jobs` and `mem_per_job` keywords
+            n_workers = 2
+            mem_per_worker = "2GB"
+            with ParallelMap(lowpass_simple,
+                            sigName,
+                            range(self.nChannels),
+                            partition=defaultQ,
+                            n_jobs=n_workers,
+                            mem_per_job=mem_per_worker,
+                            stop_client=False,
+                            setup_interactive=False) as pmap:
+                pmap.compute()
+            outDirs.append(pmap.out_dir)
 
-            # Over-allocation of memory should default to partition max
-            client = esi_cluster_setup(partition="8GBDEV", n_jobs=1, mem_per_job="9000MB", interactive=False)
+            # Ensure the provided input was interpreted correctly
+            client = dd.get_client()
+            assert pmap.n_workers == n_workers
+            assert len(client.cluster.workers) == pmap.n_workers
             memory = np.unique([w["memory_limit"] for w in client.cluster.scheduler_info["workers"].values()])
             assert memory.size == 1
-            assert np.round(memory / 1000**3)[0] == 8
-            cluster_cleanup(client)
+            assert round(memory[0] / 1000**3) == int(mem_per_worker.replace("GB", ""))
 
-            # Test if invalid extra args are caught
-            slurmOut = "/cs/home/{}/acme_out".format(getpass.getuser())
-            with pytest.raises(TypeError):
-                esi_cluster_setup(job_extra="--output={}".format(slurmOut), interactive=False)
-            cluster_cleanup()
-            with pytest.raises(ValueError):
-                esi_cluster_setup(job_extra=["output={}".format(slurmOut)], interactive=False)
-            cluster_cleanup()
-            with pytest.raises(ValueError):
-                esi_cluster_setup(job_extra=["--output=/path/to/nowhere"], interactive=False)
-            cluster_cleanup()
+        # Clean up
+        for folder in outDirs:
+            shutil.rmtree(folder, ignore_errors=True)
+        time.sleep(0.1)
+        cluster_cleanup()
+
+    # test esi-cluster-setup called separately before pmap
+    def test_existing_cluster(self):
+
+        # Test custom SLURM cluster setup
+        if useSLURM:
 
             # Supply extra args to start client for actual tests
-            client = esi_cluster_setup(partition="8GBXS", job_extra=["--output={}".format(slurmOut)], interactive=False)
+            slurmOut = "/cs/home/{}/acme_out".format(getpass.getuser())
+            client = esi_cluster_setup(partition=defaultQ,
+                                       n_workers=10,
+                                       job_extra=["--output={}".format(slurmOut)],
+                                       interactive=False)
             assert "--output={}".format(slurmOut) in client.cluster.job_header
 
         else:
-            client = esi_cluster_setup(n_jobs=6, interactive=False)
+            client = esi_cluster_setup(interactive=False)
 
-        # Re-run tests with pre-allocated client (except for those in `skipTests`)
-        skipTests = ["test_existing_cluster", "test_cancel", "test_dryrun", "test_memest"]
+        # Re-run tests with pre-allocated client (except for those in `skipTests`); ensure
+        # client "survives" multiple independent test runs and is not accidentally closed
+        skipTests = ["test_existing_cluster", "test_cancel", "test_dryrun",
+                     "test_memest", "test_backcompat", "_prep_data"]
         all_tests = [attr for attr in self.__dir__()
                      if (inspect.ismethod(getattr(self, attr)) and attr not in skipTests)]
         for test in all_tests:
-            getattr(self, test)()
+            clnt = getattr(self, test)(testclient=client)
+            assert clnt == client
         client.close()
         client.cluster.close()
         if useSLURM:
             shutil.rmtree(slurmOut, ignore_errors=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/esi_acme.egg-info/PKG-INFO` & `esi-acme-2023.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 Metadata-Version: 2.1
 Name: esi-acme
-Version: 2022.8
+Version: 2023.4
 Summary: Asynchronous Computing Made ESI
 Home-page: https://esi-acme.readthedocs.io/en/latest/
 Author: Ernst Strüngmann Institute (ESI) for Neuroscience in Cooperation with Max Planck Society
-Author-email: acme@esi-frankfurt.de
+Author-email: it@esi-frankfurt.de
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/esi-neuroscience/acme/issues
 Project-URL: Documentation, https://esi-acme.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/esi-neuroscience/acme
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: <3.10,>=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 License-File: LICENSE
 
+<!--
+Copyright (c) 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+in Cooperation with Max Planck Society
+SPDX-License-Identifier: CC-BY-NC-SA-1.0
+-->
+
 ![ACME_logo](https://raw.githubusercontent.com/esi-neuroscience/acme/master/doc/source/_static/acme_logo.png)
 
 # ACME: Asynchronous Computing Made ESI
 
-main: [![tests+codecov](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml/badge.svg?branch=main)](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml)
-[![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/main/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
+[![conda](https://img.shields.io/conda/vn/conda-forge/esi-acme.svg)](https://anaconda.org/conda-forge/esi-acme)
+[![pypi](https://badge.fury.io/py/esi-acme.svg)](https://badge.fury.io/py/esi-acme)
+[![license](https://img.shields.io/github/license/esi-neuroscience/acme)](https://github.com/esi-neuroscience/acme/blob/main/LICENSE)
+[![Open in Visual Studio Code](https://img.shields.io/badge/-Open_in_VS_Code-007ACC?logo=visual%20studio%20code&logoColor=ffffff)](https://github.dev/esi-neuroscience/acme)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7144/badge)](https://bestpractices.coreinfrastructure.org/projects/7144)
 
+main: [![tests](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml/badge.svg?branch=main)](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml)
+[![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/main/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
 
-dev: [![tests+codecov](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml/badge.svg?branch=dev)](https://github.com/esi-neuroscience/acme/actions/workflows/test_cov_workflow.yml)
+dev: [![tests](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml/badge.svg?branch=dev)](https://github.com/esi-neuroscience/acme/actions/workflows/tests_workflow.yml)
 [![codecov](https://codecov.io/gh/esi-neuroscience/acme/branch/dev/graph/badge.svg?token=LCB2RPBQJG)](https://codecov.io/gh/esi-neuroscience/acme)
 
 ## Summary
 
 The objective of ACME (pronounced *"ak-mee"*) is to provide easy-to-use
 wrappers for calling Python functions concurrently ("embarassingly parallel workloads").
 ACME is developed at the
 [Ernst Strüngmann Institute (ESI) gGmbH for Neuroscience in Cooperation with Max Planck Society](https://www.esi-frankfurt.de/>)
 and released free of charge under the
 [BSD 3-Clause "New" or "Revised" License](https://en.wikipedia.org/wiki/BSD_licenses#3-clause_license_(%22BSD_License_2.0%22,_%22Revised_BSD_License%22,_%22New_BSD_License%22,_or_%22Modified_BSD_License%22)).
-ACME relies on the concurrent processing library [Dask](https://docs.dask.org/en/latest/>)
+ACME relies heavily on the concurrent processing library [dask](https://docs.dask.org/en/latest/>)
 and was primarily designed to facilitate the use of [SLURM](https://slurm.schedmd.com/documentation.html)
 on the ESI HPC cluster (although other HPC infrastructure running SLURM can be
 leveraged as well). Local multi-processing hardware (i.e., multi-core CPUs)
 is fully supported too. ACME is itself used as the parallelization engine of [SyNCoPy](http://www.syncopy.org/).
 
 ![](https://github.com/esi-neuroscience/acme/blob/main/doc/source/_static/acme_demo.gif)
 
@@ -87,14 +98,16 @@
 def f(x, y, z=3):
   return (x + y) * z
 
 with ParallelMap(f, [2, 4, 6, 8], 4) as pmap:
   pmap.compute()
 ```
 
+See also our [Quickstart Guide](https://esi-acme.readthedocs.io/en/latest/quickstart.html).
+
 ### Intermediate Examples
 
 Set number of function calls via `n_inputs`
 
 ```python
 import numpy as np
 from acme import ParallelMap
@@ -104,14 +117,17 @@
 
 pmap = ParallelMap(f, [2, 4, 6, 8], [2, 2], z=np.array([1, 2]), w=np.ones((8, 1)), n_inputs=2)
 
 with pmap as p:
   p.compute()
 ```
 
+More details in
+[Override Automatic Input Argument Distribution](https://esi-acme.readthedocs.io/en/latest/userguide.html#override-automatic-input-argument-distribution)
+
 ### Advanced Use
 
 Allocate custom `client` object and recycle it for several computations
 (use `slurm_cluster_setup` on non-ESI HPC infrastructure or `local_cluster_setup`
 when working on your local machine)
 
 ```python
@@ -120,73 +136,119 @@
 
 def f(x, y, z=3, w=np.zeros((3, 1)), **kwargs):
     return (sum(x) + y) * z * w.max()
 
 def g(x, y, z=3, w=np.zeros((3, 1)), **kwargs):
     return (max(x) + y) * z * w.sum()
 
-n_jobs = 200
-client = esi_cluster_setup(partition="8GBXS", n_jobs=n_jobs)
+n_workers = 200
+client = esi_cluster_setup(partition="8GBXS", n_workers=n_workers)
 
 x = [2, 4, 6, 8]
-z = range(n_jobs)
+z = range(n_workers)
 w = np.ones((8, 1))
 
-pmap = ParallelMap(f, x, np.random.rand(n_jobs), z=z, w=w, n_inputs=n_jobs)
+pmap = ParallelMap(f, x, np.random.rand(n_workers), z=z, w=w, n_inputs=n_workers)
 with pmap as p:
     p.compute()
 
-pmap = ParallelMap(g, x, np.random.rand(n_jobs), z=z, w=w, n_inputs=n_jobs)
+pmap = ParallelMap(g, x, np.random.rand(n_workers), z=z, w=w, n_inputs=n_workers)
 with pmap as p:
     p.compute()
 ```
 
+For more information see [Reuse Worker Clients](https://esi-acme.readthedocs.io/en/latest/userguide.html#reuse-worker-clients)
+
 ## Handling results
 
 ### Load results from files
 
-The results are saved to disk in HDF5 format and the filenames are returned as a list of strings.
+By default, results are saved to disk in HDF5 format and can be accessed using
+the `results_container` attribute of `ParallelMap`:
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4) as pmap:
   filenames = pmap.compute()
 ```
 
 Example loading code:
 
 ```python
-out = np.zeros((4))
 import h5py
-for ii, fname in enumerate(filenames):
-    with h5py.File(fname, 'r') as f:
-        out[ii] = np.array(f['result_0'])
+import numpy as np
+out = np.zeros((4,))
+
+with h5py.File(pmap.results_container, "r") as h5f:
+  for k, key in enumerate(h5f.keys()):
+    out[k] = h5f[key]["result_0"][()]
+```
+
+See also [Where Are My Results?](https://esi-acme.readthedocs.io/en/latest/userguide.html#where-are-my-results)
+
+### Collect results in single HDF5 dataset
+
+If possible, results can be slotted into a single HDF5 dataset:
+
+```python
+def f(x, y, z=3):
+  return (x + y) * z
+
+with ParallelMap(f, [2, 4, 6, 8], 4, result_shape=(None,)) as pmap:
+  pmap.compute()
 ```
 
+Example loading code:
+
+```python
+import h5py
+
+with h5py.File(pmap.results_container, "r") as h5f:
+  out = h5f["result_0"][()] # returns a NumPy array of shape (4,)
+```
+
+More examples can be found in
+[Collect Results in Single Dataset](https://esi-acme.readthedocs.io/en/latest/userguide.html#collect-results-in-single-dataset)
+
 ### Collect results in local memory
 
 This is possible but not recommended.
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4, write_worker_results=False) as pmap:
-  results = pmap.compute() # returns a list of outputs
+  result = pmap.compute() # returns a 4-element list
+```
+
+Alternatively, create an in-memory NumPy array
+
+```python
+with ParallelMap(f, [2, 4, 6, 8], 4, write_worker_results=False, result_shape=(None,)) as pmap:
+  result = pmap.compute() # returns a NumPy array of shape (4,)
 ```
 
 ## Debugging
 
 Use the `debug` keyword to perform all function calls in the local thread of
 the active Python interpreter
 
 ```python
+def f(x, y, z=3):
+  return (x + y) * z
+
 with ParallelMap(f, [2, 4, 6, 8], 4, z=None) as pmap:
     results = pmap.compute(debug=True)
 ```
 
 This way tools like `pdb` or ``%debug`` IPython magics can be used.
+More information can be found in the `FAQ`[https://esi-acme.readthedocs.io/en/latest/troubleshooting_faq.html]
 
 ## Documentation and Contact
 
 To report bugs or ask questions please use our
 [GitHub issue tracker](https://github.com/esi-neuroscience/acme/issues).
 More usage details and background information is available in our
 [online documentation](https://esi-acme.readthedocs.io).
-
-
```

### Comparing `esi-acme-2022.8/setup.cfg` & `esi-acme-2023.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = esi-acme
 author = Ernst Strüngmann Institute (ESI) for Neuroscience in Cooperation with Max Planck Society
-author_email = acme@esi-frankfurt.de
+author_email = it@esi-frankfurt.de
 description = Asynchronous Computing Made ESI
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 license = BSD-3
-license_file = LICENSE
+license_files = LICENSE
 home_page = https://esi-acme.readthedocs.io/en/latest/
 project_urls = 
 	Bug Tracker = https://github.com/esi-neuroscience/acme/issues
 	Documentation = https://esi-acme.readthedocs.io/en/latest/
 	Source Code = https://github.com/esi-neuroscience/acme
 classifier = 
 	Development Status :: 4 - Beta
@@ -19,38 +19,41 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
-python_requires = >= 3.7, < 3.10
+python_requires = >= 3.7, < 3.11
 install_requires = 
 	colorama
-	dask < 2022.6
-	dask-jobqueue >= 0.7.1, < 0.8
+	dask >= 2021.09.0, < 2023.4
+	dask-jobqueue >= 0.8, < 0.9
 	h5py < 4
 	numpy >= 1.0, < 2.0
 	tqdm >= 4.31
 
 [options.extras_require]
 dev = 
 	ipdb
 	ipython
 	scipy >= 1.5, < 2.0
 	numpydoc
 	pytest-cov
+	sphinx < 6
 	sphinx_automodapi
 	sphinx_bootstrap_theme
+	sphinx-tabs
 	tox
 
 [options.data_files]
 acme = 
 	CHANGELOG.md
 	CITATION.cff
 	LICENSE
```

### Comparing `esi-acme-2022.8/setup.py` & `esi-acme-2023.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,52 @@
+#
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+
 # Builtins
 import datetime
 from setuptools import setup
 from setuptools.config.setupcfg import read_configuration
 import subprocess
 import toml
 
 # External packages
 import yaml
 from setuptools_scm import get_version
 
 # Set release version by hand
-releaseVersion = "2022.8"
+releaseVersion = "2023.4"
 
 # Read dependencies from setup.cfg + pyproject.toml and create conda environment file
 envFile = "acme.yml"
 setupOpts = read_configuration("setup.cfg")["options"]
 tomlPkgs = toml.load("pyproject.toml")["build-system"]["requires"]
 allPkgs = setupOpts["install_requires"] + setupOpts["extras_require"]["dev"] + tomlPkgs
-pipPkgs = ["dask-jobqueue", "sphinx_automodapi"]
+pipPkgs = ["sphinx_automodapi"]
 for k in range(len(pipPkgs)):
     pkg = pipPkgs[k]
     pipPkgs[k] = allPkgs.pop([allPkgs.index(dep) for dep in allPkgs if pkg in dep][0])
 pyVer = setupOpts
 allPkgs += ["python " + str(setupOpts["python_requires"]), "pip", {"pip" : pipPkgs}]
 ymlDict = {"name" : "acme",
            "channels" : ["defaults", "conda-forge"],
            "dependencies" : allPkgs}
-msg = "# This file was auto-generated by setup.py on {}. \n" +\
+header = "#\n" +\
+    "# Copyright © {} Ernst Strüngmann Institute (ESI) for Neuroscience " +\
+    "# in Cooperation with Max Planck Society\n#\n" +\
+    "# SPDX-License-Identifier: CC0-1.0\n#\n" +\
+    "# This file was auto-generated by setup.py on {}. \n" +\
     "# Do not edit, all of your changes will be overwritten. \n"
-msg = msg.format(datetime.datetime.now().strftime("%d/%m/%Y at %H:%M:%S"))
-with open(envFile, 'w') as ymlFile:
-    ymlFile.write(msg)
+header = header.format(datetime.datetime.now().strftime("%Y"),
+                       datetime.datetime.now().strftime("%d/%m/%Y at %H:%M:%S"))
+with open(envFile, "w") as ymlFile:
+    ymlFile.write(header)
     yaml.dump(ymlDict, ymlFile, default_flow_style=False)
 
 # If code has not been obtained via `git` or we're inside the main branch,
 # use the hard-coded `releaseVersion` as version. Otherwise keep the local `tag.devx`
 # scheme for TestPyPI uploads
 proc = subprocess.run("git branch --show-current", shell=True, capture_output=True, text=True)
 if proc.returncode !=0 or proc.stdout.strip() == "main":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esi-acme-2022.8/tox.ini` & `esi-acme-2023.4/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+#
+# Copyright © 2023 Ernst Strüngmann Institute (ESI) for Neuroscience
+# in Cooperation with Max Planck Society
+#
+# SPDX-License-Identifier: BSD-3-Clause
+#
+
 [tox]
-envlist = {py37,py38,py39}
+envlist = {py38,py39,py310}
 requires = tox-conda
 isolated_build = True
 
 [testenv]
 recreate = True
 changedir = acme/tests
 passenv = *
 allowlist_externals = sh
-deps =
-    pytest
 # Force tox to install major package dependencies via conda to avoid building
 # larger packages on POWER via pip
 conda_deps=
     ipython
     tqdm >= 4.31
     numpy >= 1.0, < 2.0
-    scipy
+    scipy >= 1.5, < 2.0
     h5py < 4
-    dask >= 2021.09.0, < 2022.6
-    dask-jobqueue >= 0.7.1, < 0.8
+    dask >= 2021.09.0, < 2023.4
+    dask-jobqueue >= 0.8, < 0.9
     bokeh
+    pytest
 conda_channels=
     defaults
     conda-forge
 commands_pre =
     python -c "import sys; import subprocess; subprocess.run('chmod +x no_slurm.sh', shell=True, check=True) if sys.platform == 'linux' else print('not on linux')"
     python -c "import sys; import subprocess; subprocess.run('./no_slurm.sh', shell=True, check=True) if sys.platform == 'linux' else print('not on linux')"
 commands =
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

