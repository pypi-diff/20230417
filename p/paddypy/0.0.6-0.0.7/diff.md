# Comparing `tmp/paddypy-0.0.6.tar.gz` & `tmp/paddypy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.0.6.tar", last modified: Wed Oct 19 07:58:39 2022, max compression
+gzip compressed data, was "paddypy-0.0.7.tar", last modified: Mon Apr 17 10:36:30 2023, max compression
```

## Comparing `paddypy-0.0.6.tar` & `paddypy-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-10-19 07:58:39.946128 paddypy-0.0.6/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1726 2022-10-19 07:58:39.945127 paddypy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      923 2022-10-19 05:46:59.000000 paddypy-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-10-19 07:58:39.929113 paddypy-0.0.6/paddypy/
--rw-rw-rw-   0        0        0       28 2022-10-19 05:46:44.000000 paddypy-0.0.6/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.6/paddypy/access.py
-drwxrwxrwx   0        0        0        0 2022-10-19 07:58:39.944126 paddypy-0.0.6/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1726 2022-10-19 07:58:39.000000 paddypy-0.0.6/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2022-10-19 07:58:39.000000 paddypy-0.0.6/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-19 07:58:39.000000 paddypy-0.0.6/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2022-10-19 07:58:39.000000 paddypy-0.0.6/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-19 07:58:39.000000 paddypy-0.0.6/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-19 07:58:39.946128 paddypy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1394 2022-10-19 07:58:18.000000 paddypy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.689571 paddypy-0.0.7/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-04-17 10:36:30.689072 paddypy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.677072 paddypy-0.0.7/paddypy/
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:31:46.000000 paddypy-0.0.7/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.7/paddypy/access.py
+-rw-rw-rw-   0        0        0     2851 2023-04-17 10:31:34.000000 paddypy-0.0.7/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.688072 paddypy-0.0.7/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:36:30.689571 paddypy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-04-17 10:36:10.000000 paddypy-0.0.7/setup.py
```

### Comparing `paddypy-0.0.6/LICENSE` & `paddypy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.6/PKG-INFO` & `paddypy-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.6
-Summary: Collection of helpfull appconfiguration extensions
-Author: broom (Patrik)
-Author-email: <patrikhartl@googlemail.com>
+Version: 0.0.7
+Summary: Collection of helpfull extensions
+Author: Patrik
+Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # paddypy
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
-Developed by Patrik Hart (c) 2022
+Developed by Patrik (c) 2022
 
 ## Examples of How To Use (Alpha Version)
 
  Print and get azure app-configuration keys and flags
 
 ```python
 from paddypy import access
```

### Comparing `paddypy-0.0.6/README.md` & `paddypy-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # paddypy
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
-Developed by Patrik Hart (c) 2022
+Developed by Patrik (c) 2022
 
 ## Examples of How To Use (Alpha Version)
 
  Print and get azure app-configuration keys and flags
 
 ```python
 from paddypy import access
```

### Comparing `paddypy-0.0.6/paddypy/access.py` & `paddypy-0.0.7/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.6/paddypy.egg-info/PKG-INFO` & `paddypy-0.0.7/paddypy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.6
-Summary: Collection of helpfull appconfiguration extensions
-Author: broom (Patrik)
-Author-email: <patrikhartl@googlemail.com>
+Version: 0.0.7
+Summary: Collection of helpfull extensions
+Author: Patrik
+Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # paddypy
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
-Developed by Patrik Hart (c) 2022
+Developed by Patrik (c) 2022
 
 ## Examples of How To Use (Alpha Version)
 
  Print and get azure app-configuration keys and flags
 
 ```python
 from paddypy import access
```

