# Comparing `tmp/report-env-0.0.5.tar.gz` & `tmp/report_env-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report-env-0.0.5.tar", last modified: Sun Apr 16 08:18:22 2023, max compression
+gzip compressed data, was "report_env-0.6.tar", max compression
```

## Comparing `report-env-0.0.5.tar` & `report_env-0.6.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.620761 report-env-0.0.5/
--rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.5/LICENSE
--rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.5/MANIFEST.in
--rw-r--r--   0 swyx       (501) staff       (20)      827 2023-04-16 08:18:22.620639 report-env-0.0.5/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      501 2023-04-16 08:11:25.000000 report-env-0.0.5/README.md
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.619746 report-env-0.0.5/report-env/
--rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.5/report-env/__init__.py
--rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.5/report-env/__main__.py
--rw-r--r--   0 swyx       (501) staff       (20)      688 2023-04-16 08:18:07.000000 report-env-0.0.5/report-env/main.py
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.620460 report-env-0.0.5/report_env.egg-info/
--rw-r--r--   0 swyx       (501) staff       (20)      827 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      309 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/SOURCES.txt
--rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/dependency_links.txt
--rw-r--r--   0 swyx       (501) staff       (20)       52 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/entry_points.txt
--rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/not-zip-safe
--rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/top_level.txt
--rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 08:18:22.620802 report-env-0.0.5/setup.cfg
--rw-r--r--   0 swyx       (501) staff       (20)     2033 2023-04-16 08:17:09.000000 report-env-0.0.5/setup.py
+-rw-r--r--   0        0        0     1090 2023-04-16 07:33:25.826455 report_env-0.6/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-16 08:22:38.045519 report_env-0.6/README.md
+-rw-r--r--   0        0        0      532 2023-04-17 20:27:25.294374 report_env-0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 20:25:58.164048 report_env-0.6/report_env/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-17 20:25:58.164596 report_env-0.6/report_env/__main__.py
+-rw-r--r--   0        0        0      688 2023-04-17 20:25:58.164912 report_env-0.6/report_env/main.py
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 report_env-0.6/PKG-INFO
```

### Comparing `report-env-0.0.5/LICENSE` & `report_env-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `report-env-0.0.5/report-env/main.py` & `report_env-0.6/report_env/main.py`

 * *Files identical despite different names*

