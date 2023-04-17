# Comparing `tmp/quantumcomputingsim-1.0.6.tar.gz` & `tmp/quantumcomputingsim-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumcomputingsim-1.0.6.tar", last modified: Mon Apr 17 21:32:56 2023, max compression
+gzip compressed data, was "quantumcomputingsim-1.0.7.tar", last modified: Mon Apr 17 21:37:11 2023, max compression
```

## Comparing `quantumcomputingsim-1.0.6.tar` & `quantumcomputingsim-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.028334 quantumcomputingsim-1.0.6/
--rw-rw-rw-   0        0        0     4638 2023-04-17 21:32:56.029338 quantumcomputingsim-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.012216 quantumcomputingsim-1.0.6/quantumcomputingsim/
--rw-rw-rw-   0        0        0       41 2023-04-17 21:27:14.000000 quantumcomputingsim-1.0.6/quantumcomputingsim/__init__.py
--rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim/quantum.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:32:56.027238 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/
--rw-rw-rw-   0        0        0     4638 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 21:32:55.000000 quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      571 2023-04-17 21:32:56.031339 quantumcomputingsim-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1647 2023-04-17 21:32:50.000000 quantumcomputingsim-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:11.425682 quantumcomputingsim-1.0.7/
+-rw-rw-rw-   0        0        0     4638 2023-04-17 21:37:11.425682 quantumcomputingsim-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:11.393538 quantumcomputingsim-1.0.7/quantum/
+-rw-rw-rw-   0        0        0       29 2023-04-17 21:36:35.000000 quantumcomputingsim-1.0.7/quantum/__init__.py
+-rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.7/quantum/quantum.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:11.421677 quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/
+-rw-rw-rw-   0        0        0     4638 2023-04-17 21:37:11.000000 quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-17 21:37:11.000000 quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:37:11.000000 quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 21:37:11.000000 quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      571 2023-04-17 21:37:11.428053 quantumcomputingsim-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-04-17 21:36:55.000000 quantumcomputingsim-1.0.7/setup.py
```

### Comparing `quantumcomputingsim-1.0.6/PKG-INFO` & `quantumcomputingsim-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library to simulate quantum computations
 Home-page: https://github.com/stealthypanda/quantumcomputingsim
 Download-URL: https://github.com/stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz
 Author: Shaik Mohammed Touseef
 Author-email: shaikm259@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/StealthyPanda/quantumcomputingsim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.6 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.7 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 stealthypanda/quantumcomputingsim Download-URL: https://github.com/
 stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz Author: Shaik Mohammed
 Touseef Author-email: shaikm259@gmail.com License: MIT Project-URL: repository,
 https://github.com/StealthyPanda/quantumcomputingsim Keywords:
 quantum,simulator Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
```

### Comparing `quantumcomputingsim-1.0.6/README.md` & `quantumcomputingsim-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.6/quantumcomputingsim/quantum.py` & `quantumcomputingsim-1.0.7/quantum/quantum.py`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.6/quantumcomputingsim.egg-info/PKG-INFO` & `quantumcomputingsim-1.0.7/quantumcomputingsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library to simulate quantum computations
 Home-page: https://github.com/stealthypanda/quantumcomputingsim
 Download-URL: https://github.com/stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz
 Author: Shaik Mohammed Touseef
 Author-email: shaikm259@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/StealthyPanda/quantumcomputingsim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.6 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.7 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 stealthypanda/quantumcomputingsim Download-URL: https://github.com/
 stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz Author: Shaik Mohammed
 Touseef Author-email: shaikm259@gmail.com License: MIT Project-URL: repository,
 https://github.com/StealthyPanda/quantumcomputingsim Keywords:
 quantum,simulator Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
```

### Comparing `quantumcomputingsim-1.0.6/setup.cfg` & `quantumcomputingsim-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.6/setup.py` & `quantumcomputingsim-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'quantumcomputingsim',         # How you named your package folder (MyLib)
-  packages = ['quantumcomputingsim'],   # Chose the same as "name"
-  version = '1.0.6',      # Start with a small number and increase it with every change you make
+  packages = ['quantum'],   # Chose the same as "name"
+  version = '1.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A library to simulate quantum computations',   # Give a short description about your library
   author = 'Shaik Mohammed Touseef',                   # Type in your name
   author_email = 'shaikm259@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/stealthypanda/quantumcomputingsim',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/stealthypanda/quantumcomputingsim/archive/v_1.0.1.tar.gz',    # I explain this later on
   keywords = ['quantum', 'simulator'],   # Keywords that define your package best
```

