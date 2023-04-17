# Comparing `tmp/pyinflux3-0.8.1.tar.gz` & `tmp/pyinflux3-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-0.8.1.tar", last modified: Fri Apr 14 08:52:00 2023, max compression
+gzip compressed data, was "pyinflux3-0.8.2.tar", last modified: Mon Apr 17 16:12:35 2023, max compression
```

## Comparing `pyinflux3-0.8.1.tar` & `pyinflux3-0.8.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:52:00.426325 pyinflux3-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 08:52:00.426325 pyinflux3-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 08:51:53.000000 pyinflux3-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:52:00.426325 pyinflux3-0.8.1/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-14 08:51:53.000000 pyinflux3-0.8.1/influxdb_client_3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:52:00.426325 pyinflux3-0.8.1/pyinflux3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 08:52:00.000000 pyinflux3-0.8.1/pyinflux3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 08:52:00.000000 pyinflux3-0.8.1/pyinflux3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:52:00.000000 pyinflux3-0.8.1/pyinflux3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 08:52:00.000000 pyinflux3-0.8.1/pyinflux3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 08:52:00.000000 pyinflux3-0.8.1/pyinflux3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-14 08:51:53.000000 pyinflux3-0.8.1/setup-client.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:52:00.426325 pyinflux3-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/influxdb_client_3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/pyinflux3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 16:12:35.000000 pyinflux3-0.8.2/pyinflux3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-17 16:12:29.000000 pyinflux3-0.8.2/setup-client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:12:35.945612 pyinflux3-0.8.2/setup.cfg
```

### Comparing `pyinflux3-0.8.1/setup-client.py` & `pyinflux3-0.8.2/setup-client.py`

 * *Files identical despite different names*

