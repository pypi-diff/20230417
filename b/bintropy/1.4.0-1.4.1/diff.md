# Comparing `tmp/bintropy-1.4.0.tar.gz` & `tmp/bintropy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.4.0.tar", last modified: Sun Apr  9 20:54:01 2023, max compression
+gzip compressed data, was "bintropy-1.4.1.tar", last modified: Mon Apr 17 15:40:24 2023, max compression
```

## Comparing `bintropy-1.4.0.tar` & `bintropy-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.181283 bintropy-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 20:53:53.000000 bintropy-1.4.0/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-09 20:53:53.000000 bintropy-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 20:53:53.000000 bintropy-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 20:54:01.185284 bintropy-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-09 20:53:53.000000 bintropy-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-09 20:53:53.000000 bintropy-1.4.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 20:53:53.000000 bintropy-1.4.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-09 20:53:53.000000 bintropy-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 20:54:01.185284 bintropy-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.181283 bintropy-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-09 20:53:53.000000 bintropy-1.4.0/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:54:01.185284 bintropy-1.4.0/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 20:54:01.000000 bintropy-1.4.0/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.550435 bintropy-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 15:40:15.000000 bintropy-1.4.1/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 15:40:15.000000 bintropy-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:40:15.000000 bintropy-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:40:24.550435 bintropy-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 15:40:15.000000 bintropy-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 15:40:15.000000 bintropy-1.4.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-17 15:40:15.000000 bintropy-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:40:24.550435 bintropy-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.4.0/.github/workflows/python-package.yml` & `bintropy-1.4.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/.gitignore` & `bintropy-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/LICENSE` & `bintropy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/PKG-INFO` & `bintropy-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.4.0/README.md` & `bintropy-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/docs/example-not-packed.png` & `bintropy-1.4.1/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/docs/example-packed.png` & `bintropy-1.4.1/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/docs/logo.png` & `bintropy-1.4.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/pyproject.toml` & `bintropy-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/src/bintropy/__info__.py` & `bintropy-1.4.1/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/src/bintropy/__init__.py` & `bintropy-1.4.1/src/bintropy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         # if not ignored, process it
         d = {}
         for c in block:
             d.setdefault(c, 0)
             d[c] += 1
         e.append(-sum([p * math.log2(p) for p in [float(ctr) / lb for ctr in d.values()]]) or .0)
     # return the entropies per block and the average entropy of all blocks if n_blocks > 1
-    return (e, sum([n or 0 for n in e]) / ((n_blocks - n_ignored) or 1)) if n_blocks > 1 else e[0]
+    return (e, sum([n or 0 for n in e]) / ((n_blocks - n_ignored) or 1)) if n_blocks > 1 or blocksize > 0 else e[0]
 
 
 def is_packed(entropies, average, threshold_average_entropy, threshold_highest_entropy, logger=None):
     """ Decision criteria as of https://ieeexplore.ieee.org/document/4140989.
     
     :param entropies:                 the list of block entropy values or the highest block entropy value
     :param average:                   the average block entropy
```

### Comparing `bintropy-1.4.0/src/bintropy/__main__.py` & `bintropy-1.4.1/src/bintropy/__main__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.0/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.4.1/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

