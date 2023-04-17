# Comparing `tmp/flake8-checker-0.0.1.tar.gz` & `tmp/flake8-checker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-checker-0.0.1.tar", last modified: Sun Apr 16 21:48:11 2023, max compression
+gzip compressed data, was "flake8-checker-0.0.2.tar", last modified: Mon Apr 17 21:30:18 2023, max compression
```

## Comparing `flake8-checker-0.0.1.tar` & `flake8-checker-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-16 21:48:11.532094 flake8-checker-0.0.1/
--rw-rw-r--   0 harish    (1000) harish    (1000)      277 2023-04-16 21:48:11.532094 flake8-checker-0.0.1/PKG-INFO
-drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-16 21:48:11.532094 flake8-checker-0.0.1/flake8_checker.egg-info/
--rw-rw-r--   0 harish    (1000) harish    (1000)      277 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/PKG-INFO
--rw-rw-r--   0 harish    (1000) harish    (1000)      256 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/SOURCES.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)        1 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/dependency_links.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)       75 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/entry_points.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)        7 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/requires.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)       15 2023-04-16 21:48:11.000000 flake8-checker-0.0.1/flake8_checker.egg-info/top_level.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)     1191 2023-04-16 20:53:51.000000 flake8-checker-0.0.1/flake8_checker.py
--rw-rw-r--   0 harish    (1000) harish    (1000)       38 2023-04-16 21:48:11.532094 flake8-checker-0.0.1/setup.cfg
--rw-rw-r--   0 harish    (1000) harish    (1000)      477 2023-04-16 21:48:06.000000 flake8-checker-0.0.1/setup.py
+drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/
+-rw-rw-r--   0 harish    (1000) harish    (1000)      300 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/PKG-INFO
+drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/flake8_checker.egg-info/
+-rw-rw-r--   0 harish    (1000) harish    (1000)      300 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/PKG-INFO
+-rw-rw-r--   0 harish    (1000) harish    (1000)      256 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/SOURCES.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)        1 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/dependency_links.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)       75 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/entry_points.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)        7 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/requires.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)       15 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/top_level.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)     1191 2023-04-16 20:53:51.000000 flake8-checker-0.0.2/flake8_checker.py
+-rw-rw-r--   0 harish    (1000) harish    (1000)       38 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/setup.cfg
+-rw-rw-r--   0 harish    (1000) harish    (1000)      504 2023-04-17 21:29:50.000000 flake8-checker-0.0.2/setup.py
```

### Comparing `flake8-checker-0.0.1/flake8_checker.py` & `flake8-checker-0.0.2/flake8_checker.py`

 * *Files identical despite different names*

