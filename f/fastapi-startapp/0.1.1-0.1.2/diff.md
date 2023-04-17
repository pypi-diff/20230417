# Comparing `tmp/fastapi-startapp-0.1.1.tar.gz` & `tmp/fastapi-startapp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fastapi-startapp-0.1.1.tar", last modified: Mon Apr 17 07:31:57 2023, max compression
+gzip compressed data, was "dist\fastapi-startapp-0.1.2.tar", last modified: Mon Apr 17 07:43:20 2023, max compression
```

## Comparing `fastapi-startapp-0.1.1.tar` & `fastapi-startapp-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:31:57.000000 fastapi-startapp-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-17 07:31:57.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      250 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0      300 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 07:31:56.000000 fastapi-startapp-0.1.1/fastapi_startapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      250 2023-04-17 07:31:57.000000 fastapi-startapp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-03-30 06:43:25.000000 fastapi-startapp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 07:31:57.000000 fastapi-startapp-0.1.1/scripts/
--rw-rw-rw-   0        0        0      357 2023-04-17 07:29:49.000000 fastapi-startapp-0.1.1/scripts/startapp.py
--rw-rw-rw-   0        0        0       22 2023-03-30 02:13:55.000000 fastapi-startapp-0.1.1/scripts/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-17 07:31:57.000000 fastapi-startapp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      480 2023-04-17 07:31:34.000000 fastapi-startapp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/core/
+-rw-rw-rw-   0        0        0     2189 2023-04-17 07:42:42.000000 fastapi-startapp-0.1.2/core/generate_app.py
+-rw-rw-rw-   0        0        0      250 2023-04-17 07:42:42.000000 fastapi-startapp-0.1.2/core/validators.py
+-rw-rw-rw-   0        0        0       22 2023-04-17 07:42:42.000000 fastapi-startapp-0.1.2/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      250 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      357 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/fastapi_startapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      250 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-03-30 06:43:25.000000 fastapi-startapp-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/scripts/
+-rw-rw-rw-   0        0        0      357 2023-04-17 07:42:31.000000 fastapi-startapp-0.1.2/scripts/startapp.py
+-rw-rw-rw-   0        0        0       22 2023-03-30 02:13:55.000000 fastapi-startapp-0.1.2/scripts/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 07:43:20.000000 fastapi-startapp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-04-17 07:43:18.000000 fastapi-startapp-0.1.2/setup.py
```

