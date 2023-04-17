# Comparing `tmp/grim-0.1.6.tar.gz` & `tmp/grim-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grim-0.1.6.tar", last modified: Sun Apr 16 16:53:54 2023, max compression
+gzip compressed data, was "grim-0.1.7.tar", last modified: Mon Apr 17 19:02:20 2023, max compression
```

## Comparing `grim-0.1.6.tar` & `grim-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.945343 grim-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 16:53:33.000000 grim-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-16 16:53:54.941343 grim-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-16 16:53:33.000000 grim-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.941343 grim-0.1.6/grim/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 16:53:33.000000 grim-0.1.6/grim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-16 16:53:33.000000 grim-0.1.6/grim/mean_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.941343 grim-0.1.6/grim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:53:54.945343 grim-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-16 16:53:33.000000 grim-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:02:20.227077 grim-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 19:02:12.000000 grim-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-17 19:02:20.227077 grim-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 19:02:12.000000 grim-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:02:20.223076 grim-0.1.7/grim/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 19:02:12.000000 grim-0.1.7/grim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-17 19:02:12.000000 grim-0.1.7/grim/mean_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:02:20.227077 grim-0.1.7/grim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-17 19:02:20.000000 grim-0.1.7/grim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 19:02:20.000000 grim-0.1.7/grim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:02:20.000000 grim-0.1.7/grim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 19:02:20.000000 grim-0.1.7/grim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:02:20.227077 grim-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 19:02:12.000000 grim-0.1.7/setup.py
```

### Comparing `grim-0.1.6/LICENSE` & `grim-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `grim-0.1.6/PKG-INFO` & `grim-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grim
-Version: 0.1.6
+Version: 0.1.7
 Summary: An implementation of the GRIM test, in Python
 Home-page: https://github.com/phoughton/grim_test
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,17 +22,19 @@
 
 You don't need the original integer values. You just need the _mean_ and the number (_n_) of items.
 
 ## What about rounding?
 
 Often the _mean_ you are testing has previously been rounded. You can check if the _mean_ is consistent with a particular rounding type by including that as an argument.
 
-This implementation supports all the rounding types currently found in Python 3.8's `decimal` [implementation](https://docs.python.org/3/library/decimal.html).
+This implementation supports all the rounding types found in the Python `decimal` [implementation](https://docs.python.org/3/library/decimal.html) (at least between versiuons 3.8 and 3.11).
+
+
+*(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)*
 
-(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)
 
 If no rounding type is included then the test assumes ROUND_HALF_UP.
 
 
 ### How do I install it?
 
 On the command line:
```

### Comparing `grim-0.1.6/README.md` & `grim-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 
 You don't need the original integer values. You just need the _mean_ and the number (_n_) of items.
 
 ## What about rounding?
 
 Often the _mean_ you are testing has previously been rounded. You can check if the _mean_ is consistent with a particular rounding type by including that as an argument.
 
-This implementation supports all the rounding types currently found in Python 3.8's `decimal` [implementation](https://docs.python.org/3/library/decimal.html).
+This implementation supports all the rounding types found in the Python `decimal` [implementation](https://docs.python.org/3/library/decimal.html) (at least between versiuons 3.8 and 3.11).
+
+
+*(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)*
 
-(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)
 
 If no rounding type is included then the test assumes ROUND_HALF_UP.
 
 
 ### How do I install it?
 
 On the command line:
```

### Comparing `grim-0.1.6/grim/mean_tester.py` & `grim-0.1.7/grim/mean_tester.py`

 * *Files identical despite different names*

### Comparing `grim-0.1.6/grim.egg-info/PKG-INFO` & `grim-0.1.7/grim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grim
-Version: 0.1.6
+Version: 0.1.7
 Summary: An implementation of the GRIM test, in Python
 Home-page: https://github.com/phoughton/grim_test
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,17 +22,19 @@
 
 You don't need the original integer values. You just need the _mean_ and the number (_n_) of items.
 
 ## What about rounding?
 
 Often the _mean_ you are testing has previously been rounded. You can check if the _mean_ is consistent with a particular rounding type by including that as an argument.
 
-This implementation supports all the rounding types currently found in Python 3.8's `decimal` [implementation](https://docs.python.org/3/library/decimal.html).
+This implementation supports all the rounding types found in the Python `decimal` [implementation](https://docs.python.org/3/library/decimal.html) (at least between versiuons 3.8 and 3.11).
+
+
+*(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)*
 
-(They are: ROUND_CEILING, ROUND_DOWN, ROUND_FLOOR, ROUND_HALF_DOWN, ROUND_HALF_EVEN, ROUND_HALF_UP, ROUND_UP, ROUND_05UP)
 
 If no rounding type is included then the test assumes ROUND_HALF_UP.
 
 
 ### How do I install it?
 
 On the command line:
```

### Comparing `grim-0.1.6/setup.py` & `grim-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grim",
-    version="0.1.6",
+    version="0.1.7",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="An implementation of the GRIM test, in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/grim_test",
     packages=setuptools.find_packages(),
```

