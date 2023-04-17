# Comparing `tmp/tamil-0.1.tar.gz` & `tmp/tamil-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamil-0.1.tar", last modified: Thu Sep 15 04:34:30 2022, max compression
+gzip compressed data, was "tamil-0.2.tar", last modified: Tue Dec 20 17:28:48 2022, max compression
```

## Comparing `tamil-0.1.tar` & `tamil-0.2.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-09-15 04:34:30.181982 tamil-0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)      227 2022-09-15 04:34:30.181982 tamil-0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-09-15 04:08:54.000000 tamil-0.1/README.rst
--rw-r--r--   0 kali      (1000) kali      (1000)      107 2022-09-15 04:34:30.185982 tamil-0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      346 2022-09-15 04:33:42.000000 tamil-0.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-09-15 04:34:30.177982 tamil-0.1/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-09-15 04:34:30.181982 tamil-0.1/src/tamil/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-09-15 04:11:24.000000 tamil-0.1/src/tamil/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-09-15 04:34:30.181982 tamil-0.1/src/tamil/tamil/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-09-15 04:11:37.000000 tamil-0.1/src/tamil/tamil/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       36 2022-09-15 04:15:48.000000 tamil-0.1/src/tamil/tamil/ravi.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-09-15 04:34:30.181982 tamil-0.1/src/tamil.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      227 2022-09-15 04:34:30.000000 tamil-0.1/src/tamil.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      235 2022-09-15 04:34:30.000000 tamil-0.1/src/tamil.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-09-15 04:34:30.000000 tamil-0.1/src/tamil.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2022-09-15 04:34:30.000000 tamil-0.1/src/tamil.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.908354 tamil-0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)      182 2022-12-20 17:28:48.908354 tamil-0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-09-15 04:08:54.000000 tamil-0.2/README.rst
+-rw-r--r--   0 kali      (1000) kali      (1000)      107 2022-12-20 17:28:48.908354 tamil-0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      346 2022-12-20 17:25:34.000000 tamil-0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.900354 tamil-0.2/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.908354 tamil-0.2/src/tamil.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      182 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      161 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/top_level.txt
```

