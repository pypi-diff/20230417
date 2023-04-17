# Comparing `tmp/adafruit-circuitpython-si7021-4.1.6.tar.gz` & `tmp/adafruit-circuitpython-si7021-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si7021-4.1.6.tar", last modified: Mon Nov 28 18:08:00 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-si7021-4.1.7.tar", last modified: Mon Apr 17 21:11:46 2023, max compression
```

## Comparing `adafruit-circuitpython-si7021-4.1.6.tar` & `adafruit-circuitpython-si7021-4.1.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.759492 adafruit-circuitpython-si7021-4.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.759492 adafruit-circuitpython-si7021-4.1.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4100 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4100 2022-11-28 18:08:00.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      994 2022-11-28 18:08:00.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:08:00.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:08:00.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:08:00.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/adafruit_si7021/
--rw-r--r--   0 runner    (1001) docker     (122)     9507 2022-11-28 18:07:49.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_si7021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2022-11-28 18:07:49.000000 adafruit-circuitpython-si7021-4.1.6/adafruit_si7021/i2c_bits.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5721 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2022-11-28 18:07:49.000000 adafruit-circuitpython-si7021-4.1.6/examples/si7021_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2022-11-28 18:07:49.000000 adafruit-circuitpython-si7021-4.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:07:33.000000 adafruit-circuitpython-si7021-4.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:08:00.763492 adafruit-circuitpython-si7021-4.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.354438 adafruit-circuitpython-si7021-4.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.346438 adafruit-circuitpython-si7021-4.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-17 21:11:46.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-17 21:11:46.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:11:46.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 21:11:46.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 21:11:46.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/adafruit_si7021/
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-04-17 21:11:38.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_si7021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-17 21:11:38.000000 adafruit-circuitpython-si7021-4.1.7/adafruit_si7021/i2c_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:11:46.350438 adafruit-circuitpython-si7021-4.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 21:11:38.000000 adafruit-circuitpython-si7021-4.1.7/examples/si7021_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-17 21:11:38.000000 adafruit-circuitpython-si7021-4.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 21:11:24.000000 adafruit-circuitpython-si7021-4.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:11:46.354438 adafruit-circuitpython-si7021-4.1.7/setup.cfg
```

### Comparing `adafruit-circuitpython-si7021-4.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si7021-4.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/.gitignore` & `adafruit-circuitpython-si7021-4.1.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-si7021-4.1.6/.pre-commit-config.yaml` & `adafruit-circuitpython-si7021-4.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/.pylintrc` & `adafruit-circuitpython-si7021-4.1.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si7021-4.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/LICENSE` & `adafruit-circuitpython-si7021-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si7021-4.1.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/LICENSES/MIT.txt` & `adafruit-circuitpython-si7021-4.1.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si7021-4.1.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/PKG-INFO` & `adafruit-circuitpython-si7021-4.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si7021
-Version: 4.1.6
+Version: 4.1.7
 Summary: CircuitPython library for SI7021 Temperature and Humidity Sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI7021
 Keywords: adafruit,si7021,temperature,humidity,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si7021-4.1.6/README.rst` & `adafruit-circuitpython-si7021-4.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/PKG-INFO` & `adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si7021
-Version: 4.1.6
+Version: 4.1.7
 Summary: CircuitPython library for SI7021 Temperature and Humidity Sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI7021
 Keywords: adafruit,si7021,temperature,humidity,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si7021-4.1.6/adafruit_circuitpython_si7021.egg-info/SOURCES.txt` & `adafruit-circuitpython-si7021-4.1.7/adafruit_circuitpython_si7021.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/adafruit_si7021/__init__.py` & `adafruit-circuitpython-si7021-4.1.7/adafruit_si7021/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 import struct
+import time
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from micropython import const
 from adafruit_si7021.i2c_bits import _RWDifferentBit, _RWDifferentBits
 
 try:
     from typing import Optional, Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "4.1.6"
+__version__ = "4.1.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI7021.git"
 
 HUMIDITY = const(0xF5)
 TEMPERATURE = const(0xF3)
 WRITE_HEATER_LEVEL = const(0x51)
 READ_HEATER_LEVEL = const(0x11)
 WRITE_HEATER_ENABLE = const(0xE6)
@@ -133,14 +134,20 @@
 
     _heater_enable = _RWDifferentBit(READ_HEATER_ENABLE, WRITE_HEATER_ENABLE, 2)
     _heater_level = _RWDifferentBits(4, READ_HEATER_LEVEL, WRITE_HEATER_LEVEL, 0)
 
     def __init__(self, i2c_bus: I2C, address: int = 0x40) -> None:
         self.i2c_device = I2CDevice(i2c_bus, address)
         self._command(_RESET)
+
+        # max 15ms Powerup Time after issuing software reset
+        # Table 2 inside of:
+        # https://cdn-learn.adafruit.com/assets/assets/000/035/931/original/Support_Documents_TechnicalDocs_Si7021-A20.pdf
+        time.sleep(0.015)
+
         # Make sure the USER1 settings are correct.
         while True:
             # While restarting, the sensor doesn't respond to reads or writes.
             try:
                 data = bytearray([_READ_USER1])
                 with self.i2c_device as i2c:
                     i2c.write_then_readinto(data, data)
```

### Comparing `adafruit-circuitpython-si7021-4.1.6/adafruit_si7021/i2c_bits.py` & `adafruit-circuitpython-si7021-4.1.7/adafruit_si7021/i2c_bits.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/docs/_static/favicon.ico` & `adafruit-circuitpython-si7021-4.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/docs/conf.py` & `adafruit-circuitpython-si7021-4.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/docs/index.rst` & `adafruit-circuitpython-si7021-4.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/examples/si7021_simpletest.py` & `adafruit-circuitpython-si7021-4.1.7/examples/si7021_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.6/pyproject.toml` & `adafruit-circuitpython-si7021-4.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si7021"
 description = "CircuitPython library for SI7021 Temperature and Humidity Sensor."
-version = "4.1.6"
+version = "4.1.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI7021"}
 keywords = [
     "adafruit",
```

