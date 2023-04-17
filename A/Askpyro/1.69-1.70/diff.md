# Comparing `tmp/askpyro-1.69.tar.gz` & `tmp/Askpyro-1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askpyro-1.69.tar", last modified: Sun Apr 16 19:13:33 2023, max compression
+gzip compressed data, was "Askpyro-1.70.tar", last modified: Mon Apr 17 04:24:10 2023, max compression
```

## Comparing `askpyro-1.69.tar` & `Askpyro-1.70.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:13:33.164964 askpyro-1.69/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-16 19:11:49.000000 askpyro-1.69/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-16 19:13:33.164964 askpyro-1.69/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-16 19:11:49.000000 askpyro-1.69/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:13:33.160964 askpyro-1.69/askpyro/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-16 19:11:49.000000 askpyro-1.69/askpyro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5553 2023-04-16 19:11:49.000000 askpyro-1.69/askpyro/conversation.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-16 19:11:49.000000 askpyro-1.69/askpyro/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:13:33.164964 askpyro-1.69/askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-16 19:13:33.000000 askpyro-1.69/askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-16 19:13:33.000000 askpyro-1.69/askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 19:13:33.000000 askpyro-1.69/askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-16 19:13:33.000000 askpyro-1.69/askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 19:13:33.164964 askpyro-1.69/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1354 2023-04-16 19:11:49.000000 askpyro-1.69/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.336058 Askpyro-1.70/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 04:24:10.000000 Askpyro-1.70/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 04:19:08.000000 Askpyro-1.70/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-04-17 04:24:10.336058 Askpyro-1.70/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-04-17 04:19:08.000000 Askpyro-1.70/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/askpyro/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.332059 Askpyro-1.70/askpyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      814 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-04-17 04:19:08.000000 Askpyro-1.70/askpyro/helpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 04:24:10.336058 Askpyro-1.70/examples/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/buttons.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/callback.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/filters.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-04-17 04:19:08.000000 Askpyro-1.70/examples/start.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 04:24:10.336058 Askpyro-1.70/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3252 2023-04-17 04:24:06.000000 Askpyro-1.70/setup.py
```

### Comparing `askpyro-1.69/LICENSE` & `Askpyro-1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `askpyro-1.69/askpyro/conversation.py` & `Askpyro-1.70/askpyro/conversation.py`

 * *Files identical despite different names*

### Comparing `askpyro-1.69/askpyro/errors.py` & `Askpyro-1.70/askpyro/errors.py`

 * *Files identical despite different names*

