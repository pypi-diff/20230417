# Comparing `tmp/rocketapi-1.0.2.tar.gz` & `tmp/rocketapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketapi-1.0.2.tar", last modified: Tue Jan  3 14:42:12 2023, max compression
+gzip compressed data, was "rocketapi-1.0.3.tar", last modified: Mon Apr 17 13:29:37 2023, max compression
```

## Comparing `rocketapi-1.0.2.tar` & `rocketapi-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-01-03 14:42:12.212591 rocketapi-1.0.2/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-01-03 14:42:12.212468 rocketapi-1.0.2/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.2/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.2/pyproject.toml
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-01-03 14:42:12.211744 rocketapi-1.0.2/rocketapi/
--rw-r--r--   0 sobolev    (501) staff       (20)       39 2022-10-08 15:10:45.000000 rocketapi-1.0.2/rocketapi/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.2/rocketapi/exceptions.py
--rw-r--r--   0 sobolev    (501) staff       (20)     6439 2023-01-03 14:38:11.000000 rocketapi-1.0.2/rocketapi/instagramapi.py
--rw-r--r--   0 sobolev    (501) staff       (20)      504 2023-01-03 14:38:11.000000 rocketapi-1.0.2/rocketapi/rocketapi.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-01-03 14:42:12.212282 rocketapi-1.0.2/rocketapi.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-01-03 14:42:12.000000 rocketapi-1.0.2/rocketapi.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      292 2023-01-03 14:42:12.000000 rocketapi-1.0.2/rocketapi.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-01-03 14:42:12.000000 rocketapi-1.0.2/rocketapi.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-01-03 14:42:12.000000 rocketapi-1.0.2/rocketapi.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-01-03 14:42:12.000000 rocketapi-1.0.2/rocketapi.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-01-03 14:42:12.212692 rocketapi-1.0.2/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-01-03 14:39:06.000000 rocketapi-1.0.2/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.359680 rocketapi-1.0.3/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-04-17 13:29:37.359551 rocketapi-1.0.3/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.3/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.3/pyproject.toml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.358811 rocketapi-1.0.3/rocketapi/
+-rw-r--r--   0 sobolev    (501) staff       (20)       39 2022-10-08 15:10:45.000000 rocketapi-1.0.3/rocketapi/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.3/rocketapi/exceptions.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    18054 2023-04-17 13:23:07.000000 rocketapi-1.0.3/rocketapi/instagramapi.py
+-rw-r--r--   0 sobolev    (501) staff       (20)      759 2023-04-17 13:26:36.000000 rocketapi-1.0.3/rocketapi/rocketapi.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.359370 rocketapi-1.0.3/rocketapi.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      292 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-04-17 13:29:37.359790 rocketapi-1.0.3/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-04-17 13:24:06.000000 rocketapi-1.0.3/setup.py
```

### Comparing `rocketapi-1.0.2/pyproject.toml` & `rocketapi-1.0.3/pyproject.toml`

 * *Files identical despite different names*

