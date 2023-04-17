# Comparing `tmp/tamil-0.2.tar.gz` & `tmp/tamil-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamil-0.2.tar", last modified: Tue Dec 20 17:28:48 2022, max compression
+gzip compressed data, was "tamil-0.3.tar", last modified: Mon Apr 17 07:04:49 2023, max compression
```

## Comparing `tamil-0.2.tar` & `tamil-0.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.908354 tamil-0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)      182 2022-12-20 17:28:48.908354 tamil-0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-09-15 04:08:54.000000 tamil-0.2/README.rst
--rw-r--r--   0 kali      (1000) kali      (1000)      107 2022-12-20 17:28:48.908354 tamil-0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      346 2022-12-20 17:25:34.000000 tamil-0.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.900354 tamil-0.2/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-12-20 17:28:48.908354 tamil-0.2/src/tamil.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      182 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      161 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-12-20 17:28:48.000000 tamil-0.2/src/tamil.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 07:04:49.422976 tamil-0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1073 2023-04-15 11:08:56.000000 tamil-0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      437 2023-04-17 07:04:49.422976 tamil-0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       77 2023-04-17 07:03:22.000000 tamil-0.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)      433 2023-04-17 07:02:44.000000 tamil-0.3/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 07:04:49.422976 tamil-0.3/setup.cfg
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 07:04:49.414976 tamil-0.3/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 07:04:49.414976 tamil-0.3/src/tamil/
+-rw-r--r--   0 kali      (1000) kali      (1000)      115 2023-04-17 06:57:33.000000 tamil-0.3/src/tamil/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       37 2023-04-17 07:00:06.000000 tamil-0.3/src/tamil/tamil.py
+-rw-r--r--   0 kali      (1000) kali      (1000)  1174414 2023-04-17 06:58:31.000000 tamil-0.3/src/tamil/thirukural.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 07:04:49.422976 tamil-0.3/src/tamil.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      437 2023-04-17 07:04:49.000000 tamil-0.3/src/tamil.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      229 2023-04-17 07:04:49.000000 tamil-0.3/src/tamil.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 07:04:49.000000 tamil-0.3/src/tamil.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 07:04:49.000000 tamil-0.3/src/tamil.egg-info/top_level.txt
```

