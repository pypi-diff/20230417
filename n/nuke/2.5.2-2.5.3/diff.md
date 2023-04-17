# Comparing `tmp/nuke-2.5.2.tar.gz` & `tmp/nuke-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuke-2.5.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nuke-2.5.2.tar` & `nuke-2.5.3.tar`

### file list

```diff
@@ -1,8 +1,21 @@
--rw-r--r--   0        0        0     1070 2021-03-25 17:02:02.000000 nuke-2.5.2/LICENSE
--rw-r--r--   0        0        0      270 2023-01-13 17:25:14.449447 nuke-2.5.2/nuke/__init__.py
--rw-r--r--   0        0        0     3107 2021-03-25 17:02:06.000000 nuke-2.5.2/nuke/dirtree.py
--rwxr-xr-x   0        0        0     5310 2023-01-13 16:57:02.270003 nuke-2.5.2/nuke/nuke.py
--rw-r--r--   0        0        0     1334 2021-03-25 17:02:06.000000 nuke-2.5.2/nuke/utils.py
--rw-r--r--   0        0        0      428 2023-01-13 17:25:14.449447 nuke-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 nuke-2.5.2/setup.py
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 nuke-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 nuke-2.5.3/.DS_Store
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nuke-2.5.3/.travis.yml
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 nuke-2.5.3/DEV.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nuke-2.5.3/HISTORY.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nuke-2.5.3/Makefile
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 nuke-2.5.3/poetry.lock
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 nuke-2.5.3/setup.cfg
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nuke-2.5.3/setup.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 nuke-2.5.3/tox.ini
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 nuke-2.5.3/.vscode/settings.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/__init__.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/dirtree.py
+-rwxr-xr-x   0        0        0     5310 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/nuke.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 nuke-2.5.3/nuke/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuke-2.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 nuke-2.5.3/tests/test_nuke.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 nuke-2.5.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nuke-2.5.3/LICENSE
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 nuke-2.5.3/README.md
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 nuke-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 nuke-2.5.3/PKG-INFO
```

### Comparing `nuke-2.5.2/LICENSE` & `nuke-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nuke-2.5.2/nuke/dirtree.py` & `nuke-2.5.3/nuke/dirtree.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.2/nuke/nuke.py` & `nuke-2.5.3/nuke/nuke.py`

 * *Files identical despite different names*

### Comparing `nuke-2.5.2/nuke/utils.py` & `nuke-2.5.3/nuke/utils.py`

 * *Files identical despite different names*

