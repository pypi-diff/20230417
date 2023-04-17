# Comparing `tmp/gpt4all-j-0.0.0.tar.gz` & `tmp/gpt4all-j-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.0.0.tar", last modified: Mon Apr 17 17:30:57 2023, max compression
+gzip compressed data, was "gpt4all-j-0.0.1.tar", last modified: Mon Apr 17 19:33:48 2023, max compression
```

## Comparing `gpt4all-j-0.0.0.tar` & `gpt4all-j-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 17:30:57.692429 gpt4all-j-0.0.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      559 2023-04-17 17:30:57.692429 gpt4all-j-0.0.0/PKG-INFO
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 17:30:57.682429 gpt4all-j-0.0.0/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      559 2023-04-17 17:30:57.000000 gpt4all-j-0.0.0/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      193 2023-04-17 17:30:57.000000 gpt4all-j-0.0.0/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 17:30:57.000000 gpt4all-j-0.0.0/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 17:30:57.000000 gpt4all-j-0.0.0/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 17:30:57.000000 gpt4all-j-0.0.0/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 17:30:57.692429 gpt4all-j-0.0.0/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-03-15 17:27:36.000000 gpt4all-j-0.0.0/gpt4allj/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 17:30:57.692429 gpt4all-j-0.0.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      614 2023-04-17 17:28:29.000000 gpt4all-j-0.0.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:33:48.182443 gpt4all-j-0.0.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 19:33:48.182443 gpt4all-j-0.0.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1095 2023-04-17 19:11:04.000000 gpt4all-j-0.0.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:33:48.182443 gpt4all-j-0.0.1/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2102 2023-04-17 19:33:48.000000 gpt4all-j-0.0.1/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      237 2023-04-17 19:33:48.000000 gpt4all-j-0.0.1/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 19:33:48.000000 gpt4all-j-0.0.1/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-17 19:33:48.000000 gpt4all-j-0.0.1/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-17 19:33:48.000000 gpt4all-j-0.0.1/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-17 19:33:48.182443 gpt4all-j-0.0.1/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.0.1/gpt4allj/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1372 2023-04-17 19:15:23.000000 gpt4all-j-0.0.1/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1338 2023-04-17 19:12:58.000000 gpt4all-j-0.0.1/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-17 19:33:48.182443 gpt4all-j-0.0.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      838 2023-04-17 17:45:20.000000 gpt4all-j-0.0.1/setup.py
```

