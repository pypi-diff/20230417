# Comparing `tmp/quantumcomputingsim-1.0.5.tar.gz` & `tmp/quantumcomputingsim-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumcomputingsim-1.0.5.tar", last modified: Mon Apr 17 21:30:27 2023, max compression
+gzip compressed data, was "quantumcomputingsim-1.0.6.tar", last modified: Mon Apr 17 21:32:56 2023, max compression
```

## Comparing `quantumcomputingsim-1.0.5.tar` & `quantumcomputingsim-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:30:27.791071 quantumcomputingsim-1.0.5/
--rw-rw-rw-   0        0        0      742 2023-04-17 21:30:27.791071 quantumcomputingsim-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:30:27.781819 quantumcomputingsim-1.0.5/quantumcomputingsim/
--rw-rw-rw-   0        0        0       41 2023-04-17 21:27:14.000000 quantumcomputingsim-1.0.5/quantumcomputingsim/__init__.py
--rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.5/quantumcomputingsim/quantum.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:30:27.789616 quantumcomputingsim-1.0.5/quantumcomputingsim.egg-info/
--rw-rw-rw-   0        0        0      742 2023-04-17 21:30:27.000000 quantumcomputingsim-1.0.5/quantumcomputingsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-17 21:30:27.000000 quantumcomputingsim-1.0.5/quantumcomputingsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:30:27.000000 quantumcomputingsim-1.0.5/quantumcomputingsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 21:30:27.000000 quantumcomputingsim-1.0.5/quantumcomputingsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-17 21:30:27.793169 quantumcomputingsim-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1647 2023-04-17 21:30:11.000000 quantumcomputingsim-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.028334 quantumcomputingsim-1.0.6/
+-rw-rw-rw-   0        0        0     4638 2023-04-17 21:32:56.029338 quantumcomputingsim-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.012216 quantumcomputingsim-1.0.6/quantumcomputingsim/
+-rw-rw-rw-   0        0        0       41 2023-04-17 21:27:14.000000 quantumcomputingsim-1.0.6/quantumcomputingsim/__init__.py
+-rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim/quantum.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.027238 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/
+-rw-rw-rw-   0        0        0     4638 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      571 2023-04-17 21:32:56.031339 quantumcomputingsim-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1647 2023-04-17 21:32:50.000000 quantumcomputingsim-1.0.6/setup.py
```

### Comparing `quantumcomputingsim-1.0.5/README.md` & `quantumcomputingsim-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.5/quantumcomputingsim/quantum.py` & `quantumcomputingsim-1.0.6/quantumcomputingsim/quantum.py`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.5/setup.py` & `quantumcomputingsim-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'quantumcomputingsim',         # How you named your package folder (MyLib)
   packages = ['quantumcomputingsim'],   # Chose the same as "name"
-  version = '1.0.5',      # Start with a small number and increase it with every change you make
+  version = '1.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A library to simulate quantum computations',   # Give a short description about your library
   author = 'Shaik Mohammed Touseef',                   # Type in your name
   author_email = 'shaikm259@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/stealthypanda/quantumcomputingsim',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz',    # I explain this later on
   keywords = ['quantum', 'simulator'],   # Keywords that define your package best
```

