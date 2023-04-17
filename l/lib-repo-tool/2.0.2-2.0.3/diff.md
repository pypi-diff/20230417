# Comparing `tmp/lib_repo_tool-2.0.2.tar.gz` & `tmp/lib_repo_tool-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_repo_tool-2.0.2.tar", last modified: Fri Mar 31 05:01:49 2023, max compression
+gzip compressed data, was "lib_repo_tool-2.0.3.tar", last modified: Mon Apr 17 02:14:39 2023, max compression
```

## Comparing `lib_repo_tool-2.0.2.tar` & `lib_repo_tool-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-03-31 05:01:49.666084 lib_repo_tool-2.0.2/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-03-31 05:01:49.665737 lib_repo_tool-2.0.2/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.2/README.md
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-03-31 05:01:49.663331 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/
--rw-r--r--   0 Andy       (501) staff       (20)      163 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      327 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/SOURCES.txt
--rw-r--r--   0 Andy       (501) staff       (20)        1 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/dependency_links.txt
--rw-r--r--   0 Andy       (501) staff       (20)       76 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/entry_points.txt
--rw-r--r--   0 Andy       (501) staff       (20)       36 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/requires.txt
--rw-r--r--   0 Andy       (501) staff       (20)       10 2023-03-31 05:01:49.000000 lib_repo_tool-2.0.2/lib_repo_tool.egg-info/top_level.txt
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-03-31 05:01:49.665115 lib_repo_tool-2.0.2/repo_tool/
--rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.2/repo_tool/__init__.py
--rw-r--r--   0 Andy       (501) staff       (20)     4181 2023-03-31 03:35:57.000000 lib_repo_tool-2.0.2/repo_tool/common.py
--rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.2/repo_tool/lib_get.py
--rw-r--r--   0 Andy       (501) staff       (20)    17096 2023-03-31 04:59:55.000000 lib_repo_tool-2.0.2/repo_tool/lib_repo.py
--rw-r--r--   0 Andy       (501) staff       (20)       38 2023-03-31 05:01:49.666197 lib_repo_tool-2.0.2/setup.cfg
--rw-r--r--   0 Andy       (501) staff       (20)      473 2023-03-31 05:01:10.000000 lib_repo_tool-2.0.2/setup.py
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.751685 lib_repo_tool-2.0.3/
+-rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 02:14:39.751384 lib_repo_tool-2.0.3/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      742 2021-08-25 06:19:20.000000 lib_repo_tool-2.0.3/README.md
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.749371 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/
+-rw-r--r--   0 Andy       (501) staff       (20)      163 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/PKG-INFO
+-rw-r--r--   0 Andy       (501) staff       (20)      327 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 Andy       (501) staff       (20)        1 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       76 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/entry_points.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       36 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/requires.txt
+-rw-r--r--   0 Andy       (501) staff       (20)       10 2023-04-17 02:14:39.000000 lib_repo_tool-2.0.3/lib_repo_tool.egg-info/top_level.txt
+drwxr-xr-x   0 Andy       (501) staff       (20)        0 2023-04-17 02:14:39.750891 lib_repo_tool-2.0.3/repo_tool/
+-rw-r--r--   0 Andy       (501) staff       (20)      146 2021-08-25 07:57:33.000000 lib_repo_tool-2.0.3/repo_tool/__init__.py
+-rw-r--r--   0 Andy       (501) staff       (20)     5287 2023-04-17 02:09:40.000000 lib_repo_tool-2.0.3/repo_tool/common.py
+-rw-r--r--   0 Andy       (501) staff       (20)     8458 2023-03-31 03:43:40.000000 lib_repo_tool-2.0.3/repo_tool/lib_get.py
+-rw-r--r--   0 Andy       (501) staff       (20)    17096 2023-03-31 04:59:55.000000 lib_repo_tool-2.0.3/repo_tool/lib_repo.py
+-rw-r--r--   0 Andy       (501) staff       (20)       38 2023-04-17 02:14:39.751793 lib_repo_tool-2.0.3/setup.cfg
+-rw-r--r--   0 Andy       (501) staff       (20)      473 2023-04-17 02:10:20.000000 lib_repo_tool-2.0.3/setup.py
```

### Comparing `lib_repo_tool-2.0.2/README.md` & `lib_repo_tool-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.2/repo_tool/lib_get.py` & `lib_repo_tool-2.0.3/repo_tool/lib_get.py`

 * *Files identical despite different names*

### Comparing `lib_repo_tool-2.0.2/repo_tool/lib_repo.py` & `lib_repo_tool-2.0.3/repo_tool/lib_repo.py`

 * *Files identical despite different names*

