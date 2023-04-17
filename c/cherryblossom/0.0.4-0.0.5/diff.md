# Comparing `tmp/cherryblossom-0.0.4.tar.gz` & `tmp/cherryblossom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "cherryblossom-0.0.5.tar", last modified: Mon Apr 17 04:32:28 2023, max compression
```

## Comparing `cherryblossom-0.0.4.tar` & `cherryblossom-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,28 @@
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/.key
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Analyzer.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Blossom.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Channels.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Chat.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/DB.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Data.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Functions.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/GPTModel.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Index.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Plots.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/Timezone.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/get_file.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/imports.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/src/cherryblossom/main.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cherryblossom-0.0.4/PKG-INFO
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 04:32:28.756096 cherryblossom-0.0.5/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 04:32:28.755946 cherryblossom-0.0.5/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.5/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1436 2023-04-17 04:32:09.000000 cherryblossom-0.0.5/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 04:32:28.756137 cherryblossom-0.0.5/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 04:32:28.749367 cherryblossom-0.0.5/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 04:32:28.754746 cherryblossom-0.0.5/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.5/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.5/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.5/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.5/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.5/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.5/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.5/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.5/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.5/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.5/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.5/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.5/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.5/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.5/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.5/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 04:32:28.755748 cherryblossom-0.0.5/src/cherryblossom.egg-info/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 04:32:28.000000 cherryblossom-0.0.5/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)      653 2023-04-17 04:32:28.000000 cherryblossom-0.0.5/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 04:32:28.000000 cherryblossom-0.0.5/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 04:32:28.000000 cherryblossom-0.0.5/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 04:32:28.000000 cherryblossom-0.0.5/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.0.4/src/cherryblossom/get_file.py` & `cherryblossom-0.0.5/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.4/src/cherryblossom/main.py` & `cherryblossom-0.0.5/src/cherryblossom/main.py`

 * *Files identical despite different names*

