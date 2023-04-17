# Comparing `tmp/tasxnat-0.0.4.tar.gz` & `tmp/tasxnat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasxnat-0.0.4.tar", last modified: Wed Apr  5 18:59:32 2023, max compression
+gzip compressed data, was "tasxnat-0.0.5.tar", last modified: Mon Apr 17 02:56:59 2023, max compression
```

## Comparing `tasxnat-0.0.4.tar` & `tasxnat-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:32.652711 tasxnat-0.0.4/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-02 01:19:17.000000 tasxnat-0.0.4/LICENSE.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      402 2023-04-05 18:59:32.652711 tasxnat-0.0.4/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-05 18:59:32.652711 tasxnat-0.0.4/setup.cfg
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      778 2023-04-05 18:58:02.000000 tasxnat-0.0.4/setup.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:32.648711 tasxnat-0.0.4/tasxnat/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      100 2023-04-02 19:13:54.000000 tasxnat-0.0.4/tasxnat/__init__.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)    10074 2023-04-05 18:54:01.000000 tasxnat-0.0.4/tasxnat/tasks.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:32.648711 tasxnat-0.0.4/tasxnat.egg-info/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      402 2023-04-05 18:59:32.000000 tasxnat-0.0.4/tasxnat.egg-info/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      181 2023-04-05 18:59:32.000000 tasxnat-0.0.4/tasxnat.egg-info/SOURCES.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-05 18:59:32.000000 tasxnat-0.0.4/tasxnat.egg-info/dependency_links.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-05 18:59:32.000000 tasxnat-0.0.4/tasxnat.egg-info/top_level.txt
+drwxr-xr-x   0 kwilkinson   (501) staff       (20)        0 2023-04-17 02:56:59.205356 tasxnat-0.0.5/
+-rw-r--r--   0 kwilkinson   (501) staff       (20)     1067 2023-04-15 16:48:58.000000 tasxnat-0.0.5/LICENSE.txt
+-rw-r--r--   0 kwilkinson   (501) staff       (20)      376 2023-04-17 02:56:59.205163 tasxnat-0.0.5/PKG-INFO
+-rw-r--r--   0 kwilkinson   (501) staff       (20)      594 2023-04-17 00:23:15.000000 tasxnat-0.0.5/pyproject.toml
+-rw-r--r--   0 kwilkinson   (501) staff       (20)       38 2023-04-17 02:56:59.205403 tasxnat-0.0.5/setup.cfg
+drwxr-xr-x   0 kwilkinson   (501) staff       (20)        0 2023-04-17 02:56:59.204298 tasxnat-0.0.5/tasxnat/
+-rw-r--r--   0 kwilkinson   (501) staff       (20)      104 2023-04-17 02:45:10.000000 tasxnat-0.0.5/tasxnat/__init__.py
+-rw-r--r--   0 kwilkinson   (501) staff       (20)     5538 2023-04-17 00:34:57.000000 tasxnat-0.0.5/tasxnat/objects.py
+-rw-r--r--   0 kwilkinson   (501) staff       (20)     3494 2023-04-17 00:33:10.000000 tasxnat-0.0.5/tasxnat/protocols.py
+-rw-r--r--   0 kwilkinson   (501) staff       (20)     4217 2023-04-17 01:16:04.000000 tasxnat-0.0.5/tasxnat/utilities.py
+drwxr-xr-x   0 kwilkinson   (501) staff       (20)        0 2023-04-17 02:56:59.204923 tasxnat-0.0.5/tasxnat.egg-info/
+-rw-r--r--   0 kwilkinson   (501) staff       (20)      376 2023-04-17 02:56:59.000000 tasxnat-0.0.5/tasxnat.egg-info/PKG-INFO
+-rw-r--r--   0 kwilkinson   (501) staff       (20)      231 2023-04-17 02:56:59.000000 tasxnat-0.0.5/tasxnat.egg-info/SOURCES.txt
+-rw-r--r--   0 kwilkinson   (501) staff       (20)        1 2023-04-17 02:56:59.000000 tasxnat-0.0.5/tasxnat.egg-info/dependency_links.txt
+-rw-r--r--   0 kwilkinson   (501) staff       (20)        8 2023-04-17 02:56:59.000000 tasxnat-0.0.5/tasxnat.egg-info/top_level.txt
```

### Comparing `tasxnat-0.0.4/LICENSE.txt` & `tasxnat-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

