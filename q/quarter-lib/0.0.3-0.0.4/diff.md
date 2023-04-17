# Comparing `tmp/Quarter-Lib-0.0.3.tar.gz` & `tmp/quarter-lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quarter-Lib-0.0.3.tar", last modified: Sun Apr 16 15:37:36 2023, max compression
+gzip compressed data, was "quarter-lib-0.0.4.tar", last modified: Mon Apr 17 17:25:13 2023, max compression
```

## Comparing `Quarter-Lib-0.0.3.tar` & `quarter-lib-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.618154 Quarter-Lib-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-16 15:37:36.626155 Quarter-Lib-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/src/Quarter_Lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 15:37:36.000000 Quarter-Lib-0.0.3/src/Quarter_Lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-16 15:37:36.000000 Quarter-Lib-0.0.3/src/Quarter_Lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:37:36.000000 Quarter-Lib-0.0.3/src/Quarter_Lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 15:37:36.000000 Quarter-Lib-0.0.3/src/Quarter_Lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:36.622154 Quarter-Lib-0.0.3/src/quarter_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/src/quarter_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-16 15:37:26.000000 Quarter-Lib-0.0.3/src/quarter_lib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.221923 quarter-lib-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.221923 quarter-lib-0.0.4/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.221923 quarter-lib-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/src/quarter_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/src/quarter_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/src/quarter_lib/akeyless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/src/quarter_lib/akeyless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 17:25:05.000000 quarter-lib-0.0.4/src/quarter_lib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:25:13.225923 quarter-lib-0.0.4/src/quarter_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 17:25:13.000000 quarter-lib-0.0.4/src/quarter_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 17:25:13.000000 quarter-lib-0.0.4/src/quarter_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:25:13.000000 quarter-lib-0.0.4/src/quarter_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 17:25:13.000000 quarter-lib-0.0.4/src/quarter_lib.egg-info/top_level.txt
```

### Comparing `Quarter-Lib-0.0.3/.github/scripts/release.py` & `quarter-lib-0.0.4/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `Quarter-Lib-0.0.3/.gitignore` & `quarter-lib-0.0.4/.gitignore`

 * *Files identical despite different names*

