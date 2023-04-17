# Comparing `tmp/manohelpers-0.0.1.tar.gz` & `tmp/manohelpers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manohelpers-0.0.1.tar", last modified: Mon Apr 17 13:24:40 2023, max compression
+gzip compressed data, was "manohelpers-0.0.9.tar", last modified: Mon Apr 17 13:30:17 2023, max compression
```

## Comparing `manohelpers-0.0.1.tar` & `manohelpers-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:24:40.818175 manohelpers-0.0.1/
--rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:24:40.818263 manohelpers-0.0.1/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 manohelpers-0.0.1/README.md
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:24:40.818024 manohelpers-0.0.1/manohelpers.egg-info/
--rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:24:30.000000 manohelpers-0.0.1/manohelpers.egg-info/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)      168 2023-04-17 13:24:30.000000 manohelpers-0.0.1/manohelpers.egg-info/SOURCES.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:24:30.000000 manohelpers-0.0.1/manohelpers.egg-info/dependency_links.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:24:30.000000 manohelpers-0.0.1/manohelpers.egg-info/top_level.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:24:40.818578 manohelpers-0.0.1/setup.cfg
--rw-r--r--   0 roni.carta   (502) staff       (20)      886 2023-04-17 13:22:39.000000 manohelpers-0.0.1/setup.py
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:30:17.353179 manohelpers-0.0.9/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:30:17.353259 manohelpers-0.0.9/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 manohelpers-0.0.9/README.md
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:30:17.353071 manohelpers-0.0.9/manohelpers.egg-info/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       55 2023-04-17 13:29:47.000000 manohelpers-0.0.9/manohelpers.egg-info/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)      168 2023-04-17 13:29:47.000000 manohelpers-0.0.9/manohelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:29:47.000000 manohelpers-0.0.9/manohelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:29:47.000000 manohelpers-0.0.9/manohelpers.egg-info/top_level.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:30:17.353517 manohelpers-0.0.9/setup.cfg
+-rw-r--r--   0 roni.carta   (502) staff       (20)      886 2023-04-17 13:28:51.000000 manohelpers-0.0.9/setup.py
```

### Comparing `manohelpers-0.0.1/setup.py` & `manohelpers-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         custom_command()
 
 
 custom_command()
 
 setup(
     name="manohelpers",
-    version="0.0.1",
+    version="0.0.9",
     packages=find_packages(),
     install_requires=[],
     cmdclass={
         'install': CustomInstallCommand,
         'develop': CustomDevelopCommand,
         'egg_info': CustomEggInfoCommand,
     },
```

