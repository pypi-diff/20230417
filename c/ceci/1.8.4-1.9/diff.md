# Comparing `tmp/ceci-1.8.4.tar.gz` & `tmp/ceci-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceci-1.8.4.tar", last modified: Mon Apr 11 16:05:48 2022, max compression
+gzip compressed data, was "ceci-1.9.tar", last modified: Wed Jun 15 17:13:16 2022, max compression
```

## Comparing `ceci-1.8.4.tar` & `ceci-1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.524479 ceci-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-11 16:05:44.000000 ceci-1.8.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.516479 ceci-1.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.516479 ceci-1.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-04-11 16:05:44.000000 ceci-1.8.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-11 16:05:44.000000 ceci-1.8.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-04-11 16:05:44.000000 ceci-1.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    12896 2022-04-11 16:05:44.000000 ceci-1.8.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-04-11 16:05:44.000000 ceci-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-04-11 16:05:48.524479 ceci-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-04-11 16:05:44.000000 ceci-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.516479 ceci-1.8.4/ceci/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    11171 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/minirunner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    53844 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.520479 ceci-1.8.4/ceci/sites/
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/sites/ccin2p3.py
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/sites/cori.py
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/sites/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/sites/site.py
--rw-r--r--   0 runner    (1001) docker     (121)    49644 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/stage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.520479 ceci-1.8.4/ceci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-11 16:05:48.000000 ceci-1.8.4/ceci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    28119 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.520479 ceci-1.8.4/ceci_example/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci_example/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6908 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci_example/example_stages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-04-11 16:05:44.000000 ceci-1.8.4/ceci_example/types.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       54 2022-04-11 16:05:44.000000 ceci-1.8.4/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.520479 ceci-1.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/config.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/config2.rst
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/launchers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    31866 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/sites.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/stages.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-04-11 16:05:44.000000 ceci-1.8.4/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.520479 ceci-1.8.4/nb/
--rw-r--r--   0 runner    (1001) docker     (121)     6944 2022-04-11 16:05:44.000000 ceci-1.8.4/nb/ceci_interactive_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-11 16:05:48.524479 ceci-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-04-11 16:05:44.000000 ceci-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.524479 ceci-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:48.524479 ceci-1.8.4/tests/inputs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/inputs/dm.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/inputs/fiducial_cosmology.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10976 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_minirunner.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_python_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_site.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     9194 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-04-11 16:05:44.000000 ceci-1.8.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.643406 ceci-1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-15 17:13:05.000000 ceci-1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.635406 ceci-1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.635406 ceci-1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-06-15 17:13:05.000000 ceci-1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-06-15 17:13:05.000000 ceci-1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-15 17:13:05.000000 ceci-1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    12896 2022-06-15 17:13:05.000000 ceci-1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-06-15 17:13:05.000000 ceci-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-15 17:13:16.643406 ceci-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-06-15 17:13:05.000000 ceci-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.635406 ceci-1.9/ceci/
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-06-15 17:13:05.000000 ceci-1.9/ceci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8608 2022-06-15 17:13:05.000000 ceci-1.9/ceci/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-06-15 17:13:05.000000 ceci-1.9/ceci/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5473 2022-06-15 17:13:05.000000 ceci-1.9/ceci/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11171 2022-06-15 17:13:05.000000 ceci-1.9/ceci/minirunner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-06-15 17:13:05.000000 ceci-1.9/ceci/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53844 2022-06-15 17:13:05.000000 ceci-1.9/ceci/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.639406 ceci-1.9/ceci/sites/
+-rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-06-15 17:13:05.000000 ceci-1.9/ceci/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-06-15 17:13:05.000000 ceci-1.9/ceci/sites/ccin2p3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-06-15 17:13:05.000000 ceci-1.9/ceci/sites/cori.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-06-15 17:13:05.000000 ceci-1.9/ceci/sites/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-06-15 17:13:05.000000 ceci-1.9/ceci/sites/site.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49845 2022-06-15 17:13:05.000000 ceci-1.9/ceci/stage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-06-15 17:13:05.000000 ceci-1.9/ceci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.639406 ceci-1.9/ceci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-15 17:13:16.000000 ceci-1.9/ceci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    28119 2022-06-15 17:13:05.000000 ceci-1.9/ceci.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.639406 ceci-1.9/ceci_example/
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-06-15 17:13:05.000000 ceci-1.9/ceci_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-06-15 17:13:05.000000 ceci-1.9/ceci_example/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6908 2022-06-15 17:13:05.000000 ceci-1.9/ceci_example/example_stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-06-15 17:13:05.000000 ceci-1.9/ceci_example/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)       54 2022-06-15 17:13:05.000000 ceci-1.9/do_cover.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.639406 ceci-1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-06-15 17:13:05.000000 ceci-1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     5423 2022-06-15 17:13:05.000000 ceci-1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-06-15 17:13:05.000000 ceci-1.9/docs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-06-15 17:13:05.000000 ceci-1.9/docs/config2.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-06-15 17:13:05.000000 ceci-1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-06-15 17:13:05.000000 ceci-1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-06-15 17:13:05.000000 ceci-1.9/docs/launchers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    31866 2022-06-15 17:13:05.000000 ceci-1.9/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-15 17:13:05.000000 ceci-1.9/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-06-15 17:13:05.000000 ceci-1.9/docs/sites.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-06-15 17:13:05.000000 ceci-1.9/docs/stages.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-06-15 17:13:05.000000 ceci-1.9/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.639406 ceci-1.9/nb/
+-rw-r--r--   0 runner    (1001) docker     (121)     6944 2022-06-15 17:13:05.000000 ceci-1.9/nb/ceci_interactive_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-15 17:13:16.643406 ceci-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-06-15 17:13:05.000000 ceci-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.643406 ceci-1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:05.000000 ceci-1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-15 17:13:05.000000 ceci-1.9/tests/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:16.643406 ceci-1.9/tests/inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:05.000000 ceci-1.9/tests/inputs/dm.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 17:13:05.000000 ceci-1.9/tests/inputs/fiducial_cosmology.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10976 2022-06-15 17:13:05.000000 ceci-1.9/tests/test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-06-15 17:13:05.000000 ceci-1.9/tests/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_minirunner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_python_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12468 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-06-15 17:13:05.000000 ceci-1.9/tests/test_utils.py
```

### Comparing `ceci-1.8.4/.github/workflows/ci.yml` & `ceci-1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/.pylintrc` & `ceci-1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/LICENSE` & `ceci-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/PKG-INFO` & `ceci-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceci
-Version: 1.8.4
+Version: 1.9
 Summary: Lightweight pipeline engine for LSST DESC
 Home-page: https://github.com/LSSTDESC/ceci
 Maintainer: Joe Zuntz
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ceci Version: 1.8.4 Summary: Lightweight pipeline
+Metadata-Version: 2.1 Name: ceci Version: 1.9 Summary: Lightweight pipeline
 engine for LSST DESC Home-page: https://github.com/LSSTDESC/ceci Maintainer:
 Joe Zuntz License: BSD Platform: UNKNOWN Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Development Status :: 3 -
 Alpha Description-Content-Type: text/markdown Provides-Extra: parsl Provides-
```

### Comparing `ceci-1.8.4/README.md` & `ceci-1.9/README.md`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/config.py` & `ceci-1.9/ceci/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,32 +56,38 @@
         return value.value
     return value
 
 
 class StageParameter:
     """A small class to manage a single parameter with basic type checking"""
 
-    def __init__(self, dtype=None, default=None, fmt="%s", msg="A parameter"):
+    def __init__(self, dtype=None, default=None, fmt="%s", required=None, msg="A parameter"):
         """Build from keywords
 
         Parameters
         ----------
         dtype : `type` or `None`
             The data type for this parameter
         default : `dtype` or `None`
             The default value
         fmt : `str`
             A formatting string for printout and representation
+        required : `bool` or `None`
+
         msg : `str`
             A help or docstring
         """
         self._help = msg
         self._format = fmt
         self._dtype = dtype
         self._default = default
+        if required is not None:
+            self._required = required
+        else:
+            self._required = self._default is None
         self._value = cast_value(self._dtype, self._default)
 
     @property
     def value(self):
         """Return the value"""
         return self._value
 
@@ -91,30 +97,40 @@
         return self._dtype
 
     @property
     def default(self):
         """Return the default value"""
         return self._default
 
+    @property
+    def required(self):
+        """Return the required flag"""
+        return self._required
+
     def copy(self):
         """Return a copy of self"""
         return StageParameter(
-            dtype=self._dtype, default=self._default, fmt=self._format, msg=self._help
+            dtype=self._dtype, default=self._default, fmt=self._format, required=self._required, msg=self._help
         )
 
     def set(self, value):
         """Set the value, raising a TypeError if the value is the wrong type"""
         self._value = cast_value(self._dtype, value)
         return self._value
 
     def set_to_default(self):
         """Set the value to the default"""
         self._value = cast_value(self._dtype, self._default)
         return self._value
 
+    def set_default(self, default):
+        """Set the default value"""
+        self._default = default
+        self.set_to_default()
+
 
 class StageConfig(dict):
     """A small class to manage a dictionary of configuration parameters with basic type checking"""
 
     def __init__(self, **kwargs):
         """Build from keywords
 
@@ -133,14 +149,16 @@
             param = None
             dtype = None
             default = None
             if val is None:
                 pass
             elif isinstance(val, StageParameter):
                 param = val.copy()
+            elif isinstance(val, StageConfig):
+                param = val.get(key).copy()
             elif isinstance(val, type):
                 dtype = val
             else:
                 dtype = type(val)
                 default = val
             if param is None:
                 param = StageParameter(dtype=dtype, default=default)
@@ -219,15 +237,15 @@
             val = None
             if key in input_config:
                 val = input_config[key]
             if args.get(key) is not None:
                 val = args[key]
             if val is None:
                 attr = self.get(key)
-                if attr.default is None:
+                if attr.required:
                     raise ValueError(f"Missing configuration option {key}")
                 val = attr.default
             self.__setattr__(key, val)
 
         for key, val in input_config.items():
             if key in self:
                 continue
```

### Comparing `ceci-1.8.4/ceci/main.py` & `ceci-1.9/ceci/main.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/minirunner.py` & `ceci-1.9/ceci/minirunner.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/monitor.py` & `ceci-1.9/ceci/monitor.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/pipeline.py` & `ceci-1.9/ceci/pipeline.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/sites/__init__.py` & `ceci-1.9/ceci/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/sites/ccin2p3.py` & `ceci-1.9/ceci/sites/ccin2p3.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/sites/cori.py` & `ceci-1.9/ceci/sites/cori.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/sites/local.py` & `ceci-1.9/ceci/sites/local.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/sites/site.py` & `ceci-1.9/ceci/sites/site.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci/stage.py` & `ceci-1.9/ceci/stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -843,15 +843,16 @@
         For general files this will simply return a standard
         python file object.
 
         For specialized file types like FITS or HDF5 it will return
         a more specific object - see the types.py file for more info.
 
         """
-        path = self.get_input(tag)
+        aliased_tag = self.get_aliased_tag(tag)
+        path = self.get_input(aliased_tag)
         input_class = self.get_input_type(tag)
         obj = input_class(path, "r", **kwargs)
 
         if wrapper:  # pragma: no cover
             return obj
         return obj.file
 
@@ -1073,15 +1074,17 @@
         """Find and retrun all the outputs associated to this stage
 
         These are returned as a dictionary of tag : path pairs
         """
         ret_dict = {}
         for tag, ftype in self.outputs_():
             aliased_tag = self.get_aliased_tag(tag)
-            ret_dict[aliased_tag] = f"{outdir}/{ftype.make_name(aliased_tag)}"
+            if not aliased_tag in self._outputs.keys(): # pragma: no cover
+                self._outputs[aliased_tag]=ftype.make_name(aliased_tag)
+            ret_dict[aliased_tag] = f"{outdir}/{self._outputs[aliased_tag]}"
         return ret_dict
 
     def print_io(self, stream=sys.stdout):
         """Print out the tags, paths and types for all the inputs and outputs of this stage"""
         stream.write("Inputs--------\n")
         for tag, ftype in self.inputs_():
             aliased_tag = self.get_aliased_tag(tag)
```

### Comparing `ceci-1.8.4/ceci/utils.py` & `ceci-1.9/ceci/utils.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci.egg-info/PKG-INFO` & `ceci-1.9/ceci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceci
-Version: 1.8.4
+Version: 1.9
 Summary: Lightweight pipeline engine for LSST DESC
 Home-page: https://github.com/LSSTDESC/ceci
 Maintainer: Joe Zuntz
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ceci Version: 1.8.4 Summary: Lightweight pipeline
+Metadata-Version: 2.1 Name: ceci Version: 1.9 Summary: Lightweight pipeline
 engine for LSST DESC Home-page: https://github.com/LSSTDESC/ceci Maintainer:
 Joe Zuntz License: BSD Platform: UNKNOWN Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Development Status :: 3 -
 Alpha Description-Content-Type: text/markdown Provides-Extra: parsl Provides-
```

### Comparing `ceci-1.8.4/ceci.egg-info/SOURCES.txt` & `ceci-1.9/ceci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci.png` & `ceci-1.9/ceci.png`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci_example/example_stages.py` & `ceci-1.9/ceci_example/example_stages.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/ceci_example/types.py` & `ceci-1.9/ceci_example/types.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/Makefile` & `ceci-1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/conf.py` & `ceci-1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/config.rst` & `ceci-1.9/docs/config.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/config2.rst` & `ceci-1.9/docs/config2.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/index.rst` & `ceci-1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/launchers.rst` & `ceci-1.9/docs/launchers.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/logo.png` & `ceci-1.9/docs/logo.png`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/sites.rst` & `ceci-1.9/docs/sites.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/stages.rst` & `ceci-1.9/docs/stages.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/docs/tutorial.rst` & `ceci-1.9/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/nb/ceci_interactive_example.ipynb` & `ceci-1.9/nb/ceci_interactive_example.ipynb`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/setup.py` & `ceci-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test.hdf5` & `ceci-1.9/tests/test.hdf5`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test.yml` & `ceci-1.9/tests/test.yml`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_cmd.py` & `ceci-1.9/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_dask.py` & `ceci-1.9/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_helpers.py` & `ceci-1.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_interactive.py` & `ceci-1.9/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_main.py` & `ceci-1.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_minirunner.py` & `ceci-1.9/tests/test_minirunner.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_monitor.py` & `ceci-1.9/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_pipeline.py` & `ceci-1.9/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_python_paths.py` & `ceci-1.9/tests/test_python_paths.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_site.py` & `ceci-1.9/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_snapshot.py` & `ceci-1.9/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `ceci-1.8.4/tests/test_stage.py` & `ceci-1.9/tests/test_stage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ceci.stage import PipelineStage
 from ceci.config import StageParameter
 from ceci_example.types import HDFFile
 import numpy as np
 from ceci.errors import *
 import pytest
+import h5py
+import os
 
 # TODO: test MPI facilities properly with:
 # https://github.com/rmjarvis/TreeCorr/blob/releases/4.1/tests/mock_mpi.py
 
 
 class MockCommunicator:
     def __init__(self, size, rank):
@@ -111,33 +113,96 @@
         inputs = [("inp1", HDFFile)]
         outputs = [("out", HDFFile)]
         config_options = {"a":"b"}
 
         def run(self):
             pass
 
-    stage = TestStage.make_stage(name="copy_of_test_stage", a='c', inp1='dummy')
-    assert stage.config.a == 'c'    
-        
+    stage = TestStage.make_stage(name="copy_of_test_stage", a='c', inp1='dummy', out="my_file.hdf5")
+    assert stage.find_outputs('.')['out_copy_of_test_stage'] =='./my_file.hdf5'
+    assert stage.config.a == 'c'
+
 
 def test_parameter():
     # This one should work
     class TestStage(PipelineStage):
         name = "test_stage_param"
         inputs = [("inp1", HDFFile)]
         outputs = []
         config_options = dict(a=StageParameter(float, 5., msg="a float"))
 
         def run(self):
             pass
 
-    stage = TestStage.make_stage(a=6., inp1='dummy')
-    assert stage.config.a == 6.    
-        
+    stage_1 = TestStage.make_stage(a=6., inp1='dummy')
+    assert stage_1.config.a == 6.
+
+    # This one should not work
+    class TestStage_2(PipelineStage):
+        name = "test_stage_param_2"
+        inputs = [("inp1", HDFFile)]
+        outputs = []
+        config_options = dict(a=StageParameter(float, None, msg="a float"))
+
+        def run(self):
+            pass
+
+    with pytest.raises(ValueError):
+        stage_2 = TestStage_2.make_stage(inp1='dummy')
 
+    # This one should work
+    class TestStage_3(PipelineStage):
+        name = "test_stage_param_3"
+        inputs = [("inp1", HDFFile)]
+        outputs = []
+        config_options = dict(a=StageParameter(float, None, required=False, msg="a float"))
+
+        def run(self):
+            pass
+
+    stage_3 = TestStage_3.make_stage(inp1='dummy')
+    assert stage_3.config.a is None
+
+    par = StageParameter(int, 0, msg="a float")
+    assert par.value == 0
+    par.set_default(1)
+    assert par.value == 1
+    assert par.default == 1
+
+    # This one should work
+    class TestStage_4(PipelineStage):
+        name = "test_stage_param_4"
+        inputs = [("inp1", HDFFile)]
+        outputs = []
+        config_options = dict(a=stage_1.config)
+
+        def run(self):
+            pass
+
+    stage_4 = TestStage_4.make_stage(inp1='dummy')
+    assert stage_4.config.a == 5.
+
+
+    stage_1.config.get('a').set_default(7.)
+    # This one should work
+    class TestStage_5(PipelineStage):
+        name = "test_stage_param_5"
+        inputs = [("inp1", HDFFile)]
+        outputs = []
+        config_options = dict(a=stage_1.config)
+
+        def run(self):
+            pass
+
+    stage_5 = TestStage_4.make_stage(inp1='dummy')
+    assert stage_5.config.a == 7.
+
+
+
+    
 
 def test_incomplete():
     class Alpha(PipelineStage):
         pass
 
     assert "Alpha" in PipelineStage.incomplete_pipeline_stages
 
@@ -326,14 +391,69 @@
     h = Hotel3(Hotel3.parse_command_line(cmd + ["--no-xyz", "--xyz"]))
     assert h.config['xyz'] is True
 
     h = Hotel3(Hotel3.parse_command_line(cmd))
     assert h.config['xyz'] is True
 
 
+def test_open_input():
+    class India(PipelineStage):
+        inputs = [("my_input", HDFFile)]
+        outputs = []
+        config_options = {}
+    cmd = "India", "--config", "tests/config.yml", "--my_input", "tests/test.hdf5"
+
+    # Testing without an alias
+    ii = India(India.parse_command_line(cmd))
+    assert os.path.exists(ii.get_input("my_input"))
+    f = ii.open_input("my_input")
+    print(f.keys())
+    f.close()
+
+    # Testing with an alias - config.yml defines an alias for my_input, my_alias
+    ii = India.make_stage(name="IndiaCopy", my_input="tests/test.hdf5", config="tests/config.yml")
+
+    print(ii.get_aliases())
+
+    # This currently works
+    assert os.path.exists(ii.get_input("my_alias"))
+
+    # This works now
+    f = ii.open_input("my_input")
+    print(f.keys())
+    f.close()
+
+
+def test_open_output():
+    class Juliett(PipelineStage):
+        inputs = []
+        outputs = [("my_output", HDFFile)]
+        config_options = {}
+    cmd = "Juliett", "--config", "tests/config.yml", "--my_output", "tests/test_out.hdf5"
+
+    # Testing without an alias
+    jj = Juliett(Juliett.parse_command_line(cmd))
+    #assert os.path.exists(jj.get_output("my_output"))
+    f = jj.open_output("my_output")
+    print(f.keys())
+    f.close()
+
+    # Testing with an alias - config.yml defines an alias for my_input, my_alias
+    jj = Juliett.make_stage(name="JuliettCopy", aliases=dict(my_output='my_alias'))
+
+    print(jj.get_aliases())
+
+    # This works now
+    f = jj.open_output("my_output")
+    print(f.keys())
+    f.close()
+
+
+
+
 
 def test_unknown_stage():
     with pytest.raises(StageNotFound):
         PipelineStage.get_stage("ThisStageIsDeliberatelyLeftBlank")
 
 
 # could add more tests here for constructor, but the regression tests here and in TXPipe are
```

### Comparing `ceci-1.8.4/tests/test_utils.py` & `ceci-1.9/tests/test_utils.py`

 * *Files identical despite different names*

