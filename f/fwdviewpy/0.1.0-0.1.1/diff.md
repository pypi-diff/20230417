# Comparing `tmp/fwdviewpy-0.1.0.tar.gz` & `tmp/fwdviewpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.0.tar", last modified: Mon Apr 17 18:20:32 2023, max compression
+gzip compressed data, was "fwdviewpy-0.1.1.tar", last modified: Mon Apr 17 18:37:46 2023, max compression
```

## Comparing `fwdviewpy-0.1.0.tar` & `fwdviewpy-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:20:32.641043 fwdviewpy-0.1.0/
--rw-rw-rw-   0        0        0      465 2023-04-17 18:20:32.633101 fwdviewpy-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 18:20:32.578975 fwdviewpy-0.1.0/fwdviewpy/
--rw-rw-rw-   0        0        0    10482 2023-04-17 15:48:31.000000 fwdviewpy-0.1.0/fwdviewpy/fwdviewpy.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:20:32.628595 fwdviewpy-0.1.0/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      465 2023-04-17 18:20:32.000000 fwdviewpy-0.1.0/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-17 18:20:32.000000 fwdviewpy-0.1.0/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:20:32.000000 fwdviewpy-0.1.0/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-17 18:20:32.000000 fwdviewpy-0.1.0/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 18:20:32.000000 fwdviewpy-0.1.0/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 18:20:32.641043 fwdviewpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-04-17 18:09:36.000000 fwdviewpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:37:46.314951 fwdviewpy-0.1.1/
+-rw-rw-rw-   0        0        0      465 2023-04-17 18:37:46.308868 fwdviewpy-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 18:37:46.254995 fwdviewpy-0.1.1/fwdviewpy/
+-rw-rw-rw-   0        0        0    10482 2023-04-17 15:48:31.000000 fwdviewpy-0.1.1/fwdviewpy/fwdviewpy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:37:46.303895 fwdviewpy-0.1.1/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      465 2023-04-17 18:37:46.000000 fwdviewpy-0.1.1/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-04-17 18:37:46.000000 fwdviewpy-0.1.1/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:37:46.000000 fwdviewpy-0.1.1/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 18:37:46.000000 fwdviewpy-0.1.1/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 18:37:46.000000 fwdviewpy-0.1.1/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:37:46.315873 fwdviewpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-04-17 18:36:42.000000 fwdviewpy-0.1.1/setup.py
```

### Comparing `fwdviewpy-0.1.0/fwdviewpy/fwdviewpy.py` & `fwdviewpy-0.1.1/fwdviewpy/fwdviewpy.py`

 * *Files identical despite different names*

