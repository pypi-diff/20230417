# Comparing `tmp/manohelpers-2.6.3.tar.gz` & `tmp/manohelpers-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manohelpers-2.6.3.tar", last modified: Mon Apr 17 13:36:23 2023, max compression
+gzip compressed data, was "manohelpers-2.6.6.tar", last modified: Mon Apr 17 13:33:50 2023, max compression
```

## Comparing `manohelpers-2.6.3.tar` & `manohelpers-2.6.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:36:23.632296 manohelpers-2.6.3/
--rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:36:23.632369 manohelpers-2.6.3/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 manohelpers-2.6.3/README.md
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:36:23.632154 manohelpers-2.6.3/manohelpers.egg-info/
--rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:36:23.000000 manohelpers-2.6.3/manohelpers.egg-info/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)      168 2023-04-17 13:36:23.000000 manohelpers-2.6.3/manohelpers.egg-info/SOURCES.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:36:23.000000 manohelpers-2.6.3/manohelpers.egg-info/dependency_links.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:36:23.000000 manohelpers-2.6.3/manohelpers.egg-info/top_level.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:36:23.632665 manohelpers-2.6.3/setup.cfg
--rw-r--r--   0 roni.carta   (502) staff       (20)      886 2023-04-17 13:36:19.000000 manohelpers-2.6.3/setup.py
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:33:50.123095 manohelpers-2.6.6/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:33:50.123171 manohelpers-2.6.6/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 manohelpers-2.6.6/README.md
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:33:50.122970 manohelpers-2.6.6/manohelpers.egg-info/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:33:49.000000 manohelpers-2.6.6/manohelpers.egg-info/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)      168 2023-04-17 13:33:49.000000 manohelpers-2.6.6/manohelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:33:49.000000 manohelpers-2.6.6/manohelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:33:49.000000 manohelpers-2.6.6/manohelpers.egg-info/top_level.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:33:50.123465 manohelpers-2.6.6/setup.cfg
+-rw-r--r--   0 roni.carta   (502) staff       (20)      886 2023-04-17 13:33:45.000000 manohelpers-2.6.6/setup.py
```

### Comparing `manohelpers-2.6.3/setup.py` & `manohelpers-2.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         custom_command()
 
 
 custom_command()
 
 setup(
     name="manohelpers",
-    version="2.6.3",
+    version="2.6.6",
     packages=find_packages(),
     install_requires=[],
     cmdclass={
         'install': CustomInstallCommand,
         'develop': CustomDevelopCommand,
         'egg_info': CustomEggInfoCommand,
     },
```

